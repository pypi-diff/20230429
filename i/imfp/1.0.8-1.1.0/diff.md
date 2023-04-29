# Comparing `tmp/imfp-1.0.8.tar.gz` & `tmp/imfp-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfp-1.0.8.tar", max compression
+gzip compressed data, was "imfp-1.1.0.tar", max compression
```

## Comparing `imfp-1.0.8.tar` & `imfp-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      497 2023-04-28 14:16:48.149409 imfp-1.0.8/imfp/__init__.py
--rw-r--r--   0        0        0     1440 2023-04-28 14:16:48.164413 imfp-1.0.8/imfp/admin.py
--rw-r--r--   0        0        0    16124 2023-04-28 18:38:01.551682 imfp-1.0.8/imfp/data.py
--rw-r--r--   0        0        0     8428 2023-04-28 20:04:12.389927 imfp-1.0.8/imfp/utils.py
--rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.0.8/LICENSE
--rw-r--r--   0        0        0     1025 2023-04-28 20:04:25.401778 imfp-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    20721 2023-04-28 20:00:12.618941 imfp-1.0.8/README.md
--rw-r--r--   0        0        0    21043 1970-01-01 00:00:00.000000 imfp-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      596 2023-04-29 21:06:07.370012 imfp-1.1.0/imfp/__init__.py
+-rw-r--r--   0        0        0     2239 2023-04-29 21:06:07.415432 imfp-1.1.0/imfp/admin.py
+-rw-r--r--   0        0        0    16124 2023-04-28 18:38:01.551682 imfp-1.1.0/imfp/data.py
+-rw-r--r--   0        0        0     9577 2023-04-29 21:06:07.573604 imfp-1.1.0/imfp/utils.py
+-rw-r--r--   0        0        0    11558 2023-03-25 14:05:34.578038 imfp-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1050 2023-04-29 21:09:08.385198 imfp-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    21042 2023-04-29 21:06:20.465633 imfp-1.1.0/README.md
+-rw-r--r--   0        0        0    21358 1970-01-01 00:00:00.000000 imfp-1.1.0/PKG-INFO
```

### Comparing `imfp-1.0.8/imfp/data.py` & `imfp-1.1.0/imfp/data.py`

 * *Files identical despite different names*

### Comparing `imfp-1.0.8/imfp/utils.py` & `imfp-1.1.0/imfp/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
-from os import environ
+from os import environ, path
+import hashlib
 from time import sleep, perf_counter
 from requests import get
-from json import loads, JSONDecodeError
+from json import loads, load, dump, JSONDecodeError
 from pandas import DataFrame
 from pkg_resources import get_distribution, DistributionNotFound
 import re
 
 
-def _min_wait_time_limited(min_wait_time):
+def _min_wait_time_limited(default_wait_time=1.5):
     def decorator(func):
         last_called = [0.0]
 
         def wrapper(*args, **kwargs):
+            min_wait_time = float(environ.get("IMF_WAIT_TIME", default_wait_time))
             elapsed = perf_counter() - last_called[0]
             left_to_wait = min_wait_time - elapsed
             if left_to_wait > 0:
                 sleep(left_to_wait)
             ret = func(*args, **kwargs)
             last_called[0] = perf_counter()
             return ret
 
         return wrapper
 
     return decorator
 
 
-_imf_wait_time = 1.5
-
-
-@_min_wait_time_limited(_imf_wait_time)  # 1.5 seconds wait time between calls
+@_min_wait_time_limited()
 def _imf_get(url, headers):
     """
     A rate-limited wrapper around the requests.get method.
 
     Args:
         url (str): The URL to send a GET request to.
         headers (dict): The headers to use in the API request.
@@ -45,14 +44,18 @@
                 'http://dataservices.imf.org/REST/SDMX_JSON.svc/Dataflow'
             )
         print(response.text)
     """
     return get(url, headers)
 
 
+_imf_use_cache = False
+_imf_save_response = False
+
+
 def _download_parse(URL, times=3):
     """
     (Internal) Download and parse JSON content from a URL with rate limiting
     and retries.
 
     This function is rate-limited and will perform a specified number of
     retries in case of failure.
@@ -66,28 +69,45 @@
         dict: The parsed JSON content as a Python dictionary.
 
     Raises:
         ValueError: If the content cannot be parsed as JSON after the specified
         number of retries.
     """
 
+    global _imf_use_cache, _imf_save_response
+    use_cache = _imf_use_cache
+    save_response = _imf_save_response
+
     app_name = environ.get("IMF_APP_NAME")
     if app_name:
         app_name = app_name[:255]
     else:
         try:
             app_name = f'imfp/{get_distribution("imfp").version}'
         except DistributionNotFound:
             app_name = "imfp"
 
     headers = {"Accept": "application/json", "User-Agent": app_name}
     for _ in range(times):
-        response = _imf_get(URL, headers=headers)
-        content = response.text
-        status = response.status_code
+        if use_cache:
+            cached_status, cached_content = _load_cached_response(URL)
+            if cached_content is not None:
+                content = cached_content
+                status = cached_status
+        else:
+            response = _imf_get(URL, headers=headers)
+            content = response.text
+            status = response.status_code
+
+        if save_response:
+            file_name = hashlib.sha256(URL.encode()).hexdigest()
+            file_path = f"tests/responses/{file_name}.json"
+            print(f"Saving response to: {file_path}")
+            with open(file_path, "w") as file:
+                dump({"status_code": status, "content": content}, file)
 
         if status != 200 or ("<" in content and ">" in content):
             matches = re.search("<[^>]+>(.*?)<\\/[^>]+>", content)
             inner_text = matches.group(1)
             output_string = re.sub(" GKey\\s*=\\s*[a-f0-9-]+", "", inner_text)
 
             if "Rejected" in content or "Bandwidth" in content:
@@ -143,14 +163,25 @@
                 else:
                     raise ValueError(
                         f"Content from API could not be parsed as JSON. URL: '{URL}' "
                         f"Status: '{status}', Content: '{content}'"
                     )
 
 
+def _load_cached_response(URL):
+    file_name = hashlib.sha256(URL.encode()).hexdigest()
+    file_path = f"tests/responses/{file_name}.json"
+
+    if path.exists(file_path):
+        with open(file_path, "r") as file:
+            data = load(file)
+            return data.get("status_code"), data.get("content")
+    return None, None
+
+
 def _imf_dimensions(database_id, times=3, inputs_only=True):
     """
     (Internal) Retrieve the list of codes for dimensions of an individual IMF
     database.
 
     Args:
         database_id (str): The ID of the IMF database.
```

### Comparing `imfp-1.0.8/LICENSE` & `imfp-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imfp-1.0.8/pyproject.toml` & `imfp-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imfp"
-version = "1.0.8"
+version = "1.1.0"
 description = "Python package for downloading economic data from the International Monetary Fund JSON RESTful API endpoint."
 authors = ["Christopher C. Smith <chriscarrollsmith@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/chriscarrollsmith/imfp"
 repository = "https://github.com/chriscarrollsmith/imfp"
 documentation = ""
@@ -25,11 +25,12 @@
 requests = "^2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 responses = "^0.23.1"
 pytest = "^7.2.2"
 pytest-runner = "^6.0.0"
 black = "^23.3.0"
+pytest-mock = "^3.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `imfp-1.0.8/README.md` & `imfp-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -71,1226 +71,1246 @@
 00000460: 6f6e 2e20 5468 6573 6520 7061 636b 6167  on. These packag
 00000470: 6573 2063 616e 2062 6520 696e 7374 616c  es can be instal
 00000480: 6c65 6420 7573 696e 6720 6070 6970 6020  led using `pip` 
 00000490: 616e 6420 6c6f 6164 6564 2075 7369 6e67  and loaded using
 000004a0: 2060 696d 706f 7274 603a 0d0a 0d0a 0d0a   `import`:......
 000004b0: 6060 6070 7974 686f 6e0d 0a69 6d70 6f72  ```python..impor
 000004c0: 7420 7365 6162 6f72 6e0d 0a60 6060 0d0a  t seaborn..```..
-000004d0: 0d0a 2323 2320 5365 7474 696e 6720 6120  ..### Setting a 
-000004e0: 556e 6971 7565 2041 7070 6c69 6361 7469  Unique Applicati
-000004f0: 6f6e 204e 616d 6520 7769 7468 2069 6d66  on Name with imf
-00000500: 5f61 7070 5f6e 616d 650d 0a0d 0a60 696d  _app_name....`im
-00000510: 6670 2e69 6d66 5f61 7070 5f6e 616d 6528  fp.imf_app_name(
-00000520: 2960 2061 6c6c 6f77 7320 7573 6572 7320  )` allows users 
-00000530: 746f 2073 6574 2061 2063 7573 746f 6d20  to set a custom 
-00000540: 6170 706c 6963 6174 696f 6e20 6e61 6d65  application name
-00000550: 2074 6f20 6265 2075 7365 6420 7768 656e   to be used when
-00000560: 206d 616b 696e 6720 4150 4920 6361 6c6c   making API call
-00000570: 7320 746f 2074 6865 2049 4d46 2041 5049  s to the IMF API
-00000580: 2e20 5468 6520 494d 4620 4150 4920 6861  . The IMF API ha
-00000590: 7320 616e 2061 7070 6c69 6361 7469 6f6e  s an application
-000005a0: 2d62 6173 6564 2072 6174 6520 6c69 6d69  -based rate limi
-000005b0: 7420 6f66 2035 3020 7265 7175 6573 7473  t of 50 requests
-000005c0: 2070 6572 2073 6563 6f6e 642c 2077 6974   per second, wit
-000005d0: 6820 7468 6520 6170 706c 6963 6174 696f  h the applicatio
-000005e0: 6e20 6964 656e 7469 6669 6564 2062 7920  n identified by 
-000005f0: 7468 6520 2275 7365 725f 6167 656e 7422  the "user_agent"
-00000600: 2076 6172 6961 626c 6520 696e 2074 6865   variable in the
-00000610: 2072 6571 7565 7374 2068 6561 6465 722e   request header.
-00000620: 0d0a 0d0a 5468 6973 2063 6f75 6c64 2070  ....This could p
-00000630: 726f 7665 2070 726f 626c 656d 6174 6963  rove problematic
-00000640: 2069 6620 7468 6520 6069 6d66 7060 206c   if the `imfp` l
-00000650: 6962 7261 7279 2062 6563 616d 6520 746f  ibrary became to
-00000660: 6f20 706f 7075 6c61 7220 616e 6420 746f  o popular and to
-00000670: 6f20 6d61 6e79 2075 7365 7273 2074 7269  o many users tri
-00000680: 6564 2074 6f20 6d61 6b65 2073 696d 756c  ed to make simul
-00000690: 7461 6e65 6f75 7320 4150 4920 7265 7175  taneous API requ
-000006a0: 6573 7473 2075 7369 6e67 2074 6865 2064  ests using the d
-000006b0: 6566 6175 6c74 2061 7070 206e 616d 652e  efault app name.
-000006c0: 2042 7920 7365 7474 696e 6720 6120 6375   By setting a cu
-000006d0: 7374 6f6d 2061 7070 6c69 6361 7469 6f6e  stom application
-000006e0: 206e 616d 652c 2075 7365 7273 2063 616e   name, users can
-000006f0: 2061 766f 6964 2068 6974 7469 6e67 2072   avoid hitting r
-00000700: 6174 6520 6c69 6d69 7473 2061 6e64 2062  ate limits and b
-00000710: 6569 6e67 2062 6c6f 636b 6564 2062 7920  eing blocked by 
-00000720: 7468 6520 4150 492e 2060 696d 6670 2e69  the API. `imfp.i
-00000730: 6d66 5f61 7070 5f6e 616d 6528 2960 2073  mf_app_name()` s
-00000740: 6574 7320 7468 6520 6170 706c 6963 6174  ets the applicat
-00000750: 696f 6e20 6e61 6d65 2062 7920 6368 616e  ion name by chan
-00000760: 6769 6e67 2074 6865 2060 494d 465f 4150  ging the `IMF_AP
-00000770: 505f 4e41 4d45 6020 7661 7269 6162 6c65  P_NAME` variable
-00000780: 2069 6e20 7468 6520 656e 7669 726f 6e6d   in the environm
-00000790: 656e 742e 2049 6620 7468 6973 2076 6172  ent. If this var
-000007a0: 6961 626c 6520 646f 6573 6e27 7420 6578  iable doesn't ex
-000007b0: 6973 742c 2060 696d 6670 2e69 6d66 5f61  ist, `imfp.imf_a
-000007c0: 7070 5f6e 616d 6528 2960 2077 696c 6c20  pp_name()` will 
-000007d0: 6372 6561 7465 2069 742e 0d0a 0d0a 546f  create it.....To
-000007e0: 2073 6574 2061 2063 7573 746f 6d20 6170   set a custom ap
-000007f0: 706c 6963 6174 696f 6e20 6e61 6d65 2c20  plication name, 
-00000800: 7369 6d70 6c79 2063 616c 6c20 7468 6520  simply call the 
-00000810: 6069 6d66 702e 696d 665f 6170 705f 6e61  `imfp.imf_app_na
-00000820: 6d65 2829 6020 6675 6e63 7469 6f6e 2077  me()` function w
-00000830: 6974 6820 796f 7572 2064 6573 6972 6564  ith your desired
-00000840: 2061 7070 6c69 6361 7469 6f6e 206e 616d   application nam
-00000850: 6520 6173 2061 6e20 6172 6775 6d65 6e74  e as an argument
-00000860: 3a0d 0a0d 0a0d 0a60 6060 7079 7468 6f6e  :......```python
-00000870: 0d0a 2320 5365 7420 6375 7374 6f6d 2061  ..# Set custom a
-00000880: 7070 206e 616d 6520 6173 2061 6e20 656e  pp name as an en
-00000890: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-000008a0: 6c65 0d0a 696d 6670 2e69 6d66 5f61 7070  le..imfp.imf_app
-000008b0: 5f6e 616d 6528 226d 795f 6375 7374 6f6d  _name("my_custom
-000008c0: 5f61 7070 5f6e 616d 6522 290d 0a60 6060  _app_name")..```
-000008d0: 0d0a 0d0a 0d0a 0d0a 5468 6520 6675 6e63  ........The func
-000008e0: 7469 6f6e 2077 696c 6c20 7468 726f 7720  tion will throw 
-000008f0: 616e 2065 7272 6f72 2069 6620 7468 6520  an error if the 
-00000900: 7072 6f76 6964 6564 206e 616d 6520 6973  provided name is
-00000910: 206d 6973 7369 6e67 2c20 4e55 4c4c 2c20   missing, NULL, 
-00000920: 4e41 2c20 6e6f 7420 6120 7374 7269 6e67  NA, not a string
-00000930: 2c20 6f72 206c 6f6e 6765 7220 7468 616e  , or longer than
-00000940: 2032 3535 2063 6861 7261 6374 6572 732e   255 characters.
-00000950: 2049 6620 7468 6520 7072 6f76 6964 6564   If the provided
-00000960: 206e 616d 6520 6973 2022 696d 6672 2220   name is "imfr" 
-00000970: 2874 6865 2064 6566 6175 6c74 2920 6f72  (the default) or
-00000980: 2061 6e20 656d 7074 7920 7374 7269 6e67   an empty string
-00000990: 2c20 7468 6520 6675 6e63 7469 6f6e 2077  , the function w
-000009a0: 696c 6c20 6973 7375 6520 6120 7761 726e  ill issue a warn
-000009b0: 696e 6720 7265 636f 6d6d 656e 6469 6e67  ing recommending
-000009c0: 2074 6865 2075 7365 206f 6620 6120 756e   the use of a un
-000009d0: 6971 7565 2061 7070 206e 616d 6520 746f  ique app name to
-000009e0: 2061 766f 6964 2068 6974 7469 6e67 2072   avoid hitting r
-000009f0: 6174 6520 6c69 6d69 7473 2e0d 0a0d 0a23  ate limits.....#
-00000a00: 2323 2041 646a 7573 7469 6e67 2074 6865  ## Adjusting the
-00000a10: 2072 6174 6520 6c69 6d69 7420 7769 7468   rate limit with
-00000a20: 205f 696d 665f 7761 6974 5f74 696d 650d   _imf_wait_time.
-00000a30: 0a0d 0a44 7572 696e 6720 696d 706f 7274  ...During import
-00000a40: 206f 6620 6069 6d66 7060 2c20 6120 7661   of `imfp`, a va
-00000a50: 7269 6162 6c65 2063 616c 6c65 6420 5f69  riable called _i
-00000a60: 6d66 5f77 6169 745f 7469 6d65 2069 7320  mf_wait_time is 
-00000a70: 7365 7420 746f 2061 2064 6566 6175 6c74  set to a default
-00000a80: 2076 616c 7565 206f 6620 312e 352e 2054   value of 1.5. T
-00000a90: 6869 7320 6973 2074 6865 206d 616e 6461  his is the manda
-00000aa0: 746f 7279 2065 6e66 6f72 6365 6420 7761  tory enforced wa
-00000ab0: 6974 2074 696d 6520 6265 7477 6565 6e20  it time between 
-00000ac0: 4150 4920 6361 6c6c 732c 2074 6f20 7072  API calls, to pr
-00000ad0: 6576 656e 7420 7265 7065 6174 6564 206f  event repeated o
-00000ae0: 7220 7265 6375 7273 6976 6520 6361 6c6c  r recursive call
-00000af0: 7320 6672 6f6d 2065 7863 6565 6469 6e67  s from exceeding
-00000b00: 2074 6865 206c 696d 6974 2e20 5468 6973   the limit. This
-00000b10: 2077 6169 7420 7469 6d65 2073 686f 756c   wait time shoul
-00000b20: 6420 6265 2073 7566 6669 6369 656e 7420  d be sufficient 
-00000b30: 666f 7220 6d6f 7374 2061 7070 6c69 6361  for most applica
-00000b40: 7469 6f6e 732e 2048 6f77 6576 6572 2c20  tions. However, 
-00000b50: 6966 2079 6f75 2061 7265 2072 756e 6e69  if you are runni
-00000b60: 6e67 2070 6172 616c 6c65 6c20 7072 6f63  ng parallel proc
-00000b70: 6573 7365 7320 7573 696e 6720 6069 6d66  esses using `imf
-00000b80: 7060 2028 652e 672e 2064 7572 696e 6720  p` (e.g. during 
-00000b90: 6372 6f73 732d 706c 6174 666f 726d 2074  cross-platform t
-00000ba0: 6573 7469 6e67 292c 2074 6869 7320 7761  esting), this wa
-00000bb0: 6974 2074 696d 6520 6d61 7920 6265 2069  it time may be i
-00000bc0: 6e73 7566 6669 6369 656e 7420 746f 2070  nsufficient to p
-00000bd0: 7265 7665 6e74 2079 6f75 2066 726f 6d20  revent you from 
-00000be0: 7275 6e6e 696e 6720 7570 2061 6761 696e  running up again
-00000bf0: 7374 2074 6865 2041 5049 2773 2072 6174  st the API's rat
-00000c00: 6520 616e 6420 6261 6e64 7769 6474 6820  e and bandwidth 
-00000c10: 6c69 6d69 7473 2e20 596f 7520 6361 6e20  limits. You can 
-00000c20: 696e 6372 6561 7365 2074 6869 7320 7761  increase this wa
-00000c30: 6974 2074 696d 6520 6279 2073 696d 706c  it time by simpl
-00000c40: 7920 6368 616e 6769 6e67 2074 6865 2076  y changing the v
-00000c50: 6172 6961 626c 6520 7661 6c75 652e 2046  ariable value. F
-00000c60: 6f72 2069 6e73 7461 6e63 652c 2074 6f20  or instance, to 
-00000c70: 696e 6372 6561 7365 2074 6865 2062 6574  increase the bet
-00000c80: 7765 656e 2d63 616c 6c20 7761 6974 2074  ween-call wait t
-00000c90: 696d 6520 6279 206f 6e65 2073 6563 6f6e  ime by one secon
-00000ca0: 642c 2075 7365 2060 5f69 6d66 5f77 6169  d, use `_imf_wai
-00000cb0: 745f 7469 6d65 202b 3d20 3160 2e0d 0a0d  t_time += 1`....
-00000cc0: 0a41 6c73 6f20 6e6f 7465 2074 6861 7420  .Also note that 
-00000cd0: 6279 2064 6566 6175 6c74 2c20 6069 6d66  by default, `imf
-00000ce0: 7060 2066 756e 6374 696f 6e73 2077 696c  p` functions wil
-00000cf0: 6c20 7265 7472 7920 616e 7920 4150 4920  l retry any API 
-00000d00: 6361 6c6c 2072 656a 6563 7465 6420 666f  call rejected fo
-00000d10: 7220 6261 6e64 7769 6474 6820 6f72 2072  r bandwidth or r
-00000d20: 6174 6520 6c69 6d69 7420 7265 6173 6f6e  ate limit reason
-00000d30: 732e 2054 6865 206e 756d 6265 7220 6f66  s. The number of
-00000d40: 2074 696d 6573 2060 696d 6670 6020 7769   times `imfp` wi
-00000d50: 6c6c 2061 7474 656d 7074 2074 6865 2063  ll attempt the c
-00000d60: 616c 6c20 6973 2073 6574 2062 7920 7468  all is set by th
-00000d70: 6520 6074 696d 6573 6020 6172 6775 6d65  e `times` argume
-00000d80: 6e74 2c20 7769 7468 2061 2064 6566 6175  nt, with a defau
-00000d90: 6c74 2076 616c 7565 206f 6620 332e 2028  lt value of 3. (
-00000da0: 5769 7468 2074 6869 7320 7661 6c75 652c  With this value,
-00000db0: 2072 6571 7565 7374 7320 7769 6c6c 2062   requests will b
-00000dc0: 6520 7265 7472 6965 6420 7477 6963 6520  e retried twice 
-00000dd0: 6166 7465 7220 616e 2069 6e69 7469 616c  after an initial
-00000de0: 2066 6169 6c75 7265 2e29 204e 6f74 6520   failure.) Note 
-00000df0: 7468 6174 2060 696d 6670 6020 656e 666f  that `imfp` enfo
-00000e00: 7263 6573 2061 6e20 6578 706f 6e65 6e74  rces an exponent
-00000e10: 6961 6c6c 7920 696e 6372 6561 7369 6e67  ially increasing
-00000e20: 2077 6169 7420 7469 6d65 2062 6574 7765   wait time betwe
-00000e30: 656e 2066 756e 6374 696f 6e20 6361 6c6c  en function call
-00000e40: 732c 2077 6974 6820 6120 6261 7365 2077  s, with a base w
-00000e50: 6169 7420 7469 6d65 206f 6620 3520 7365  ait time of 5 se
-00000e60: 636f 6e64 7320 6f6e 2074 6865 2066 6972  conds on the fir
-00000e70: 7374 2072 6574 7279 2c20 736f 2069 7420  st retry, so it 
-00000e80: 6973 206e 6f74 2072 6563 6f6d 6d65 6e64  is not recommend
-00000e90: 6564 2074 6f20 7365 7420 6120 6869 6768  ed to set a high
-00000ea0: 2076 616c 7565 2066 6f72 2060 7469 6d65   value for `time
-00000eb0: 7360 2e0d 0a0d 0a0d 0a23 2323 2046 6574  s`.......### Fet
-00000ec0: 6368 696e 6720 616e 2049 6e64 6578 206f  ching an Index o
-00000ed0: 6620 4461 7461 6261 7365 7320 7769 7468  f Databases with
-00000ee0: 2074 6865 2069 6d66 5f64 6174 6162 6173   the imf_databas
-00000ef0: 6573 2046 756e 6374 696f 6e0d 0a0d 0a54  es Function....T
-00000f00: 6865 2060 696d 6670 6020 7061 636b 6167  he `imfp` packag
-00000f10: 6520 696e 7472 6f64 7563 6573 2066 6f75  e introduces fou
-00000f20: 7220 636f 7265 2066 756e 6374 696f 6e73  r core functions
-00000f30: 3a20 6069 6d66 702e 696d 665f 6461 7461  : `imfp.imf_data
-00000f40: 6261 7365 7360 2c20 6069 6d66 702e 696d  bases`, `imfp.im
-00000f50: 665f 7061 7261 6d65 7465 7273 602c 2060  f_parameters`, `
-00000f60: 696d 6670 2e69 6d66 5f70 6172 616d 6574  imfp.imf_paramet
-00000f70: 6572 5f64 6566 7360 2c20 616e 6420 6069  er_defs`, and `i
-00000f80: 6d66 702e 696d 665f 6461 7461 7365 7460  mfp.imf_dataset`
-00000f90: 2e20 5468 6520 6675 6e63 7469 6f6e 2066  . The function f
-00000fa0: 6f72 2064 6f77 6e6c 6f61 6469 6e67 2064  or downloading d
-00000fb0: 6174 6173 6574 7320 6973 2060 696d 6670  atasets is `imfp
-00000fc0: 2e69 6d66 5f64 6174 6173 6574 602c 2062  .imf_dataset`, b
-00000fd0: 7574 2079 6f75 2077 696c 6c20 6e65 6564  ut you will need
-00000fe0: 2074 6865 206f 7468 6572 2066 756e 6374   the other funct
-00000ff0: 696f 6e73 2074 6f20 6465 7465 726d 696e  ions to determin
-00001000: 6520 7768 6174 2061 7267 756d 656e 7473  e what arguments
-00001010: 2074 6f20 7375 7070 6c79 2074 6f20 6069   to supply to `i
-00001020: 6d66 702e 696d 665f 6461 7461 7365 7460  mfp.imf_dataset`
-00001030: 2e20 466f 7220 696e 7374 616e 6365 2c20  . For instance, 
-00001040: 616c 6c20 6361 6c6c 7320 746f 2060 696d  all calls to `im
-00001050: 6670 2e69 6d66 5f64 6174 6173 6574 6020  fp.imf_dataset` 
-00001060: 7265 7175 6972 6520 6120 6064 6174 6162  require a `datab
-00001070: 6173 655f 6964 602e 2054 6869 7320 6973  ase_id`. This is
-00001080: 2062 6563 6175 7365 2074 6865 2049 4d46   because the IMF
-00001090: 2073 6572 7665 7320 6d61 6e79 2064 6966   serves many dif
-000010a0: 6665 7265 6e74 2064 6174 6162 6173 6573  ferent databases
-000010b0: 2074 6872 6f75 6768 2069 7473 2041 5049   through its API
-000010c0: 2c20 616e 6420 7468 6520 4150 4920 6e65  , and the API ne
-000010d0: 6564 7320 746f 206b 6e6f 7720 7768 6963  eds to know whic
-000010e0: 6820 6f66 2074 6865 7365 206d 616e 7920  h of these many 
-000010f0: 6461 7461 6261 7365 7320 796f 7527 7265  databases you're
-00001100: 2072 6571 7565 7374 696e 6720 6461 7461   requesting data
-00001110: 2066 726f 6d2e 2054 6f20 6f62 7461 696e   from. To obtain
-00001120: 2061 206c 6973 7420 6f66 2064 6174 6162   a list of datab
-00001130: 6173 6573 2c20 7573 6520 6069 6d66 702e  ases, use `imfp.
-00001140: 696d 665f 6461 7461 6261 7365 7360 2c20  imf_databases`, 
-00001150: 6c69 6b65 2073 6f3a 0d0a 0d0a 0d0a 6060  like so:......``
-00001160: 6070 7974 686f 6e0d 0a23 4665 7463 6820  `python..#Fetch 
-00001170: 7468 6520 6c69 7374 206f 6620 6461 7461  the list of data
-00001180: 6261 7365 7320 6176 6169 6c61 626c 6520  bases available 
-00001190: 7468 726f 7567 6820 7468 6520 494d 4620  through the IMF 
-000011a0: 4150 490d 0a64 6174 6162 6173 6573 203d  API..databases =
-000011b0: 2069 6d66 702e 696d 665f 6461 7461 6261   imfp.imf_databa
-000011c0: 7365 7328 290d 0a64 6174 6162 6173 6573  ses()..databases
-000011d0: 2e68 6561 6428 290d 0a60 6060 0d0a 0d0a  .head()..```....
-000011e0: 0d0a 0d0a 0d0a 3c64 6976 3e0d 0a0d 0a3c  ......<div>....<
-000011f0: 7461 626c 6520 626f 7264 6572 3d22 3122  table border="1"
-00001200: 2063 6c61 7373 3d22 6461 7461 6672 616d   class="datafram
-00001210: 6522 3e0d 0a20 203c 7468 6561 643e 0d0a  e">..  <thead>..
-00001220: 2020 2020 3c74 7220 7374 796c 653d 2274      <tr style="t
-00001230: 6578 742d 616c 6967 6e3a 2072 6967 6874  ext-align: right
-00001240: 3b22 3e0d 0a20 2020 2020 203c 7468 3e3c  ;">..      <th><
-00001250: 2f74 683e 0d0a 2020 2020 2020 3c74 683e  /th>..      <th>
-00001260: 6461 7461 6261 7365 5f69 643c 2f74 683e  database_id</th>
-00001270: 0d0a 2020 2020 2020 3c74 683e 6465 7363  ..      <th>desc
-00001280: 7269 7074 696f 6e3c 2f74 683e 0d0a 2020  ription</th>..  
-00001290: 2020 3c2f 7472 3e0d 0a20 203c 2f74 6865    </tr>..  </the
-000012a0: 6164 3e0d 0a20 203c 7462 6f64 793e 0d0a  ad>..  <tbody>..
-000012b0: 2020 2020 3c74 723e 0d0a 2020 2020 2020      <tr>..      
-000012c0: 3c74 683e 303c 2f74 683e 0d0a 2020 2020  <th>0</th>..    
-000012d0: 2020 3c74 643e 424f 505f 3230 3137 4d30    <td>BOP_2017M0
-000012e0: 363c 2f74 643e 0d0a 2020 2020 2020 3c74  6</td>..      <t
-000012f0: 643e 4261 6c61 6e63 6520 6f66 2050 6179  d>Balance of Pay
-00001300: 6d65 6e74 7320 2842 4f50 292c 2032 3031  ments (BOP), 201
-00001310: 3720 4d30 363c 2f74 643e 0d0a 2020 2020  7 M06</td>..    
-00001320: 3c2f 7472 3e0d 0a20 2020 203c 7472 3e0d  </tr>..    <tr>.
-00001330: 0a20 2020 2020 203c 7468 3e31 3c2f 7468  .      <th>1</th
-00001340: 3e0d 0a20 2020 2020 203c 7464 3e42 4f50  >..      <td>BOP
-00001350: 5f32 3032 304d 333c 2f74 643e 0d0a 2020  _2020M3</td>..  
-00001360: 2020 2020 3c74 643e 4261 6c61 6e63 6520      <td>Balance 
-00001370: 6f66 2050 6179 6d65 6e74 7320 2842 4f50  of Payments (BOP
-00001380: 292c 2032 3032 3020 4d30 333c 2f74 643e  ), 2020 M03</td>
-00001390: 0d0a 2020 2020 3c2f 7472 3e0d 0a20 2020  ..    </tr>..   
-000013a0: 203c 7472 3e0d 0a20 2020 2020 203c 7468   <tr>..      <th
-000013b0: 3e32 3c2f 7468 3e0d 0a20 2020 2020 203c  >2</th>..      <
-000013c0: 7464 3e42 4f50 5f32 3031 374d 3131 3c2f  td>BOP_2017M11</
-000013d0: 7464 3e0d 0a20 2020 2020 203c 7464 3e42  td>..      <td>B
-000013e0: 616c 616e 6365 206f 6620 5061 796d 656e  alance of Paymen
-000013f0: 7473 2028 424f 5029 2c20 3230 3137 204d  ts (BOP), 2017 M
-00001400: 3131 3c2f 7464 3e0d 0a20 2020 203c 2f74  11</td>..    </t
-00001410: 723e 0d0a 2020 2020 3c74 723e 0d0a 2020  r>..    <tr>..  
-00001420: 2020 2020 3c74 683e 333c 2f74 683e 0d0a      <th>3</th>..
-00001430: 2020 2020 2020 3c74 643e 444f 545f 3230        <td>DOT_20
-00001440: 3230 5131 3c2f 7464 3e0d 0a20 2020 2020  20Q1</td>..     
-00001450: 203c 7464 3e44 6972 6563 7469 6f6e 206f   <td>Direction o
-00001460: 6620 5472 6164 6520 5374 6174 6973 7469  f Trade Statisti
-00001470: 6373 2028 444f 5453 292c 2032 3032 3020  cs (DOTS), 2020 
-00001480: 5131 3c2f 7464 3e0d 0a20 2020 203c 2f74  Q1</td>..    </t
-00001490: 723e 0d0a 2020 2020 3c74 723e 0d0a 2020  r>..    <tr>..  
-000014a0: 2020 2020 3c74 683e 343c 2f74 683e 0d0a      <th>4</th>..
-000014b0: 2020 2020 2020 3c74 643e 4746 534d 4142        <td>GFSMAB
-000014c0: 3230 3136 3c2f 7464 3e0d 0a20 2020 2020  2016</td>..     
-000014d0: 203c 7464 3e47 6f76 6572 6e6d 656e 7420   <td>Government 
-000014e0: 4669 6e61 6e63 6520 5374 6174 6973 7469  Finance Statisti
-000014f0: 6373 2059 6561 7262 6f6f 6b20 2847 4653  cs Yearbook (GFS
-00001500: 5920 322e 2e2e 3c2f 7464 3e0d 0a20 2020  Y 2...</td>..   
-00001510: 203c 2f74 723e 0d0a 2020 3c2f 7462 6f64   </tr>..  </tbod
-00001520: 793e 0d0a 3c2f 7461 626c 653e 0d0a 3c2f  y>..</table>..</
-00001530: 6469 763e 0d0a 0d0a 0d0a 0d0a 5468 6973  div>........This
-00001540: 2066 756e 6374 696f 6e20 7265 7475 726e   function return
-00001550: 7320 7468 6520 494d 46e2 8099 7320 6c69  s the IMF...s li
-00001560: 7374 696e 6720 6f66 2032 3539 2064 6174  sting of 259 dat
-00001570: 6162 6173 6573 2061 7661 696c 6162 6c65  abases available
-00001580: 2074 6872 6f75 6768 2074 6865 2041 5049   through the API
-00001590: 2e20 2849 6e20 7265 616c 6974 792c 2037  . (In reality, 7
-000015a0: 206f 6620 7468 6520 6c69 7374 6564 2064   of the listed d
-000015b0: 6174 6162 6173 6573 2061 7265 2064 6566  atabases are def
-000015c0: 756e 6374 2061 6e64 206e 6f74 2061 6374  unct and not act
-000015d0: 7561 6c6c 7920 6176 6169 6c61 626c 653a  ually available:
-000015e0: 2046 4153 5f32 3031 352c 2047 4653 3031   FAS_2015, GFS01
-000015f0: 2c20 464d 3230 3230 3130 2c20 4150 4452  , FM202010, APDR
-00001600: 454f 3230 3230 3130 2c20 4146 5252 454f  EO202010, AFRREO
-00001610: 3230 3230 3130 2c20 5748 4452 454f 3230  202010, WHDREO20
-00001620: 3230 3130 2c20 424f 5041 4747 5f32 3032  2010, BOPAGG_202
-00001630: 302e 290d 0a0d 0a54 6f20 7669 6577 2061  0.)....To view a
-00001640: 6e64 2065 7870 6c6f 7265 2074 6865 2064  nd explore the d
-00001650: 6174 6162 6173 6520 6c69 7374 2c20 6974  atabase list, it
-00001660: e280 9973 2070 6f73 7369 626c 6520 746f  ...s possible to
-00001670: 2065 7870 6c6f 7265 2073 7562 7365 7473   explore subsets
-00001680: 206f 6620 7468 6520 6461 7461 2066 7261   of the data fra
-00001690: 6d65 2062 7920 726f 7720 6e75 6d62 6572  me by row number
-000016a0: 2077 6974 6820 6064 6174 6162 6173 6573   with `databases
-000016b0: 2e6c 6f63 603a 0d0a 0d0a 0d0a 0d0a 6060  .loc`:........``
-000016c0: 6070 7974 686f 6e0d 0a23 2056 6965 7720  `python..# View 
-000016d0: 6120 7375 6273 6574 2063 6f6e 7369 7374  a subset consist
-000016e0: 696e 6720 6f66 2072 6f77 7320 3520 7468  ing of rows 5 th
-000016f0: 726f 7567 6820 390d 0a64 6174 6162 6173  rough 9..databas
-00001700: 6573 2e6c 6f63 5b35 3a39 5d0d 0a60 6060  es.loc[5:9]..```
-00001710: 0d0a 0d0a 0d0a 0d0a 0d0a 3c64 6976 3e0d  ..........<div>.
-00001720: 0a0d 0a3c 7461 626c 6520 626f 7264 6572  ...<table border
-00001730: 3d22 3122 2063 6c61 7373 3d22 6461 7461  ="1" class="data
-00001740: 6672 616d 6522 3e0d 0a20 203c 7468 6561  frame">..  <thea
-00001750: 643e 0d0a 2020 2020 3c74 7220 7374 796c  d>..    <tr styl
-00001760: 653d 2274 6578 742d 616c 6967 6e3a 2072  e="text-align: r
-00001770: 6967 6874 3b22 3e0d 0a20 2020 2020 203c  ight;">..      <
-00001780: 7468 3e3c 2f74 683e 0d0a 2020 2020 2020  th></th>..      
-00001790: 3c74 683e 6461 7461 6261 7365 5f69 643c  <th>database_id<
-000017a0: 2f74 683e 0d0a 2020 2020 2020 3c74 683e  /th>..      <th>
-000017b0: 6465 7363 7269 7074 696f 6e3c 2f74 683e  description</th>
-000017c0: 0d0a 2020 2020 3c2f 7472 3e0d 0a20 203c  ..    </tr>..  <
-000017d0: 2f74 6865 6164 3e0d 0a20 203c 7462 6f64  /thead>..  <tbod
-000017e0: 793e 0d0a 2020 2020 3c74 723e 0d0a 2020  y>..    <tr>..  
-000017f0: 2020 2020 3c74 683e 353c 2f74 683e 0d0a      <th>5</th>..
-00001800: 2020 2020 2020 3c74 643e 424f 505f 3230        <td>BOP_20
-00001810: 3139 4d31 323c 2f74 643e 0d0a 2020 2020  19M12</td>..    
-00001820: 2020 3c74 643e 4261 6c61 6e63 6520 6f66    <td>Balance of
-00001830: 2050 6179 6d65 6e74 7320 2842 4f50 292c   Payments (BOP),
-00001840: 2032 3031 3920 4d31 323c 2f74 643e 0d0a   2019 M12</td>..
-00001850: 2020 2020 3c2f 7472 3e0d 0a20 2020 203c      </tr>..    <
-00001860: 7472 3e0d 0a20 2020 2020 203c 7468 3e36  tr>..      <th>6
-00001870: 3c2f 7468 3e0d 0a20 2020 2020 203c 7464  </th>..      <td
-00001880: 3e47 4653 5946 414c 4353 3230 3134 3c2f  >GFSYFALCS2014</
-00001890: 7464 3e0d 0a20 2020 2020 203c 7464 3e47  td>..      <td>G
-000018a0: 6f76 6572 6e6d 656e 7420 4669 6e61 6e63  overnment Financ
-000018b0: 6520 5374 6174 6973 7469 6373 2059 6561  e Statistics Yea
-000018c0: 7262 6f6f 6b20 2847 4653 5920 322e 2e2e  rbook (GFSY 2...
-000018d0: 3c2f 7464 3e0d 0a20 2020 203c 2f74 723e  </td>..    </tr>
-000018e0: 0d0a 2020 2020 3c74 723e 0d0a 2020 2020  ..    <tr>..    
-000018f0: 2020 3c74 683e 373c 2f74 683e 0d0a 2020    <th>7</th>..  
-00001900: 2020 2020 3c74 643e 4746 5345 3230 3136      <td>GFSE2016
-00001910: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-00001920: 3e47 6f76 6572 6e6d 656e 7420 4669 6e61  >Government Fina
-00001930: 6e63 6520 5374 6174 6973 7469 6373 2059  nce Statistics Y
-00001940: 6561 7262 6f6f 6b20 2847 4653 5920 322e  earbook (GFSY 2.
-00001950: 2e2e 3c2f 7464 3e0d 0a20 2020 203c 2f74  ..</td>..    </t
-00001960: 723e 0d0a 2020 2020 3c74 723e 0d0a 2020  r>..    <tr>..  
-00001970: 2020 2020 3c74 683e 383c 2f74 683e 0d0a      <th>8</th>..
-00001980: 2020 2020 2020 3c74 643e 464d 3230 3135        <td>FM2015
-00001990: 3130 3c2f 7464 3e0d 0a20 2020 2020 203c  10</td>..      <
-000019a0: 7464 3e46 6973 6361 6c20 4d6f 6e69 746f  td>Fiscal Monito
-000019b0: 7220 2846 4d29 204f 6374 6f62 6572 2032  r (FM) October 2
-000019c0: 3031 353c 2f74 643e 0d0a 2020 2020 3c2f  015</td>..    </
-000019d0: 7472 3e0d 0a20 2020 203c 7472 3e0d 0a20  tr>..    <tr>.. 
-000019e0: 2020 2020 203c 7468 3e39 3c2f 7468 3e0d       <th>9</th>.
-000019f0: 0a20 2020 2020 203c 7464 3e47 4653 4942  .      <td>GFSIB
-00001a00: 5332 3031 363c 2f74 643e 0d0a 2020 2020  S2016</td>..    
-00001a10: 2020 3c74 643e 476f 7665 726e 6d65 6e74    <td>Government
-00001a20: 2046 696e 616e 6365 2053 7461 7469 7374   Finance Statist
-00001a30: 6963 7320 5965 6172 626f 6f6b 2028 4746  ics Yearbook (GF
-00001a40: 5359 2032 2e2e 2e3c 2f74 643e 0d0a 2020  SY 2...</td>..  
-00001a50: 2020 3c2f 7472 3e0d 0a20 203c 2f74 626f    </tr>..  </tbo
-00001a60: 6479 3e0d 0a3c 2f74 6162 6c65 3e0d 0a3c  dy>..</table>..<
-00001a70: 2f64 6976 3e0d 0a0d 0a0d 0a0d 0a0d 0a20  /div>.......... 
-00001a80: 4f72 2c20 6966 2079 6f75 2061 6c72 6561  Or, if you alrea
-00001a90: 6479 206b 6e6f 7720 7768 6963 6820 6461  dy know which da
-00001aa0: 7461 6261 7365 2079 6f75 2077 616e 742c  tabase you want,
-00001ab0: 2079 6f75 2063 616e 2066 6574 6368 2074   you can fetch t
-00001ac0: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
-00001ad0: 2063 6f64 6520 6279 2073 6561 7263 6869   code by searchi
-00001ae0: 6e67 2066 6f72 2061 2073 7472 696e 6720  ng for a string 
-00001af0: 6d61 7463 6820 7573 696e 6720 6073 7472  match using `str
-00001b00: 2e63 6f6e 7461 696e 7360 2061 6e64 2073  .contains` and s
-00001b10: 7562 7365 7474 696e 6720 7468 6520 6461  ubsetting the da
-00001b20: 7461 2066 7261 6d65 2066 6f72 206d 6174  ta frame for mat
-00001b30: 6368 696e 6720 726f 7773 2e20 466f 7220  ching rows. For 
-00001b40: 696e 7374 616e 6365 2c20 6865 7265 e280  instance, here..
-00001b50: 9973 2068 6f77 2074 6f20 7365 6172 6368  .s how to search
-00001b60: 2066 6f72 2074 6865 2050 7269 6d61 7279   for the Primary
-00001b70: 2043 6f6d 6d6f 6469 7479 2050 7269 6365   Commodity Price
-00001b80: 2053 7973 7465 6d3a 0d0a 0d0a 0d0a 6060   System:......``
-00001b90: 6070 7974 686f 6e0d 0a64 6174 6162 6173  `python..databas
-00001ba0: 6573 5b64 6174 6162 6173 6573 5b27 6465  es[databases['de
-00001bb0: 7363 7269 7074 696f 6e27 5d2e 7374 722e  scription'].str.
-00001bc0: 636f 6e74 6169 6e73 2822 436f 6d6d 6f64  contains("Commod
-00001bd0: 6974 7922 295d 0d0a 6060 600d 0a0d 0a0d  ity")]..```.....
-00001be0: 0a0d 0a0d 0a3c 6469 763e 0d0a 0d0a 3c74  .....<div>....<t
-00001bf0: 6162 6c65 2062 6f72 6465 723d 2231 2220  able border="1" 
-00001c00: 636c 6173 733d 2264 6174 6166 7261 6d65  class="dataframe
-00001c10: 223e 0d0a 2020 3c74 6865 6164 3e0d 0a20  ">..  <thead>.. 
-00001c20: 2020 203c 7472 2073 7479 6c65 3d22 7465     <tr style="te
-00001c30: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
-00001c40: 223e 0d0a 2020 2020 2020 3c74 683e 3c2f  ">..      <th></
-00001c50: 7468 3e0d 0a20 2020 2020 203c 7468 3e64  th>..      <th>d
-00001c60: 6174 6162 6173 655f 6964 3c2f 7468 3e0d  atabase_id</th>.
-00001c70: 0a20 2020 2020 203c 7468 3e64 6573 6372  .      <th>descr
-00001c80: 6970 7469 6f6e 3c2f 7468 3e0d 0a20 2020  iption</th>..   
-00001c90: 203c 2f74 723e 0d0a 2020 3c2f 7468 6561   </tr>..  </thea
-00001ca0: 643e 0d0a 2020 3c74 626f 6479 3e0d 0a20  d>..  <tbody>.. 
-00001cb0: 2020 203c 7472 3e0d 0a20 2020 2020 203c     <tr>..      <
-00001cc0: 7468 3e32 3337 3c2f 7468 3e0d 0a20 2020  th>237</th>..   
-00001cd0: 2020 203c 7464 3e50 4354 4f54 3c2f 7464     <td>PCTOT</td
-00001ce0: 3e0d 0a20 2020 2020 203c 7464 3e43 6f6d  >..      <td>Com
-00001cf0: 6d6f 6469 7479 2054 6572 6d73 206f 6620  modity Terms of 
-00001d00: 5472 6164 653c 2f74 643e 0d0a 2020 2020  Trade</td>..    
-00001d10: 3c2f 7472 3e0d 0a20 2020 203c 7472 3e0d  </tr>..    <tr>.
-00001d20: 0a20 2020 2020 203c 7468 3e32 3339 3c2f  .      <th>239</
-00001d30: 7468 3e0d 0a20 2020 2020 203c 7464 3e50  th>..      <td>P
-00001d40: 4350 533c 2f74 643e 0d0a 2020 2020 2020  CPS</td>..      
-00001d50: 3c74 643e 5072 696d 6172 7920 436f 6d6d  <td>Primary Comm
-00001d60: 6f64 6974 7920 5072 6963 6520 5379 7374  odity Price Syst
-00001d70: 656d 2028 5043 5053 293c 2f74 643e 0d0a  em (PCPS)</td>..
-00001d80: 2020 2020 3c2f 7472 3e0d 0a20 203c 2f74      </tr>..  </t
-00001d90: 626f 6479 3e0d 0a3c 2f74 6162 6c65 3e0d  body>..</table>.
-00001da0: 0a3c 2f64 6976 3e0d 0a0d 0a0d 0a0d 0a23  .</div>........#
-00001db0: 2323 2046 6574 6368 696e 6720 6120 4c69  ## Fetching a Li
-00001dc0: 7374 206f 6620 5061 7261 6d65 7465 7273  st of Parameters
-00001dd0: 2061 6e64 2049 6e70 7574 2043 6f64 6573   and Input Codes
-00001de0: 2077 6974 6820 696d 665f 7061 7261 6d65   with imf_parame
-00001df0: 7465 7273 2061 6e64 2069 6d66 5f70 6172  ters and imf_par
-00001e00: 616d 6574 6572 5f64 6566 730d 0a0d 0a4f  ameter_defs....O
-00001e10: 6e63 6520 796f 7520 6861 7665 2061 2060  nce you have a `
-00001e20: 6461 7461 6261 7365 5f69 6460 2c20 6974  database_id`, it
-00001e30: e280 9973 2070 6f73 7369 626c 6520 746f  ...s possible to
-00001e40: 206d 616b 6520 6120 6361 6c6c 2074 6f20   make a call to 
-00001e50: 6069 6d66 702e 696d 665f 6461 7461 7365  `imfp.imf_datase
-00001e60: 7460 2074 6f20 6665 7463 6820 7468 6520  t` to fetch the 
-00001e70: 656e 7469 7265 2064 6174 6162 6173 653a  entire database:
-00001e80: 2060 696d 6670 2e69 6d66 5f64 6174 6173   `imfp.imf_datas
-00001e90: 6574 2864 6174 6162 6173 655f 6964 2960  et(database_id)`
-00001ea0: 2e20 486f 7765 7665 722c 2077 6869 6c65  . However, while
-00001eb0: 2074 6869 7320 7769 6c6c 2073 7563 6365   this will succe
-00001ec0: 6564 2066 6f72 2061 2066 6577 2073 6d61  ed for a few sma
-00001ed0: 6c6c 2064 6174 6162 6173 6573 2c20 6974  ll databases, it
-00001ee0: 2077 696c 6c20 6661 696c 2066 6f72 2061   will fail for a
-00001ef0: 6c6c 206f 6620 7468 6520 6c61 7267 6572  ll of the larger
-00001f00: 206f 6e65 732e 2041 6e64 2065 7665 6e20   ones. And even 
-00001f10: 696e 2074 6865 2072 6172 6520 6361 7365  in the rare case
-00001f20: 2077 6865 6e20 6974 2073 7563 6365 6564   when it succeed
-00001f30: 732c 2066 6574 6368 696e 6720 616e 2065  s, fetching an e
-00001f40: 6e74 6972 6520 6461 7461 6261 7365 2063  ntire database c
-00001f50: 616e 2074 616b 6520 6120 6c6f 6e67 2074  an take a long t
-00001f60: 696d 652e 2059 6f75 e280 9972 6520 6d75  ime. You...re mu
-00001f70: 6368 2062 6574 7465 7220 6f66 6620 7375  ch better off su
-00001f80: 7070 6c79 696e 6720 6164 6469 7469 6f6e  pplying addition
-00001f90: 616c 2066 696c 7465 7220 7061 7261 6d65  al filter parame
-00001fa0: 7465 7273 2074 6f20 7265 6475 6365 2074  ters to reduce t
-00001fb0: 6865 2073 697a 6520 6f66 2079 6f75 7220  he size of your 
-00001fc0: 7265 7175 6573 742e 0d0a 0d0a 5265 7175  request.....Requ
-00001fd0: 6573 7473 2074 6f20 6461 7461 6261 7365  ests to database
-00001fe0: 7320 6176 6169 6c61 626c 6520 7468 726f  s available thro
-00001ff0: 7567 6820 7468 6520 494d 4620 4150 4920  ugh the IMF API 
-00002000: 6172 6520 636f 6d70 6c69 6361 7465 6420  are complicated 
-00002010: 6279 2074 6865 2066 6163 7420 7468 6174  by the fact that
-00002020: 2065 6163 6820 6461 7461 6261 7365 2075   each database u
-00002030: 7365 7320 6120 6469 6666 6572 656e 7420  ses a different 
-00002040: 7365 7420 6f66 2070 6172 616d 6574 6572  set of parameter
-00002050: 7320 7768 656e 206d 616b 696e 6720 6120  s when making a 
-00002060: 7265 7175 6573 742e 2028 4174 206c 6173  request. (At las
-00002070: 7420 636f 756e 742c 2074 6865 7265 2077  t count, there w
-00002080: 6572 6520 3433 2075 6e69 7175 6520 7061  ere 43 unique pa
-00002090: 7261 6d65 7465 7273 2075 7365 6420 696e  rameters used in
-000020a0: 206d 616b 696e 6720 4150 4920 7265 7175   making API requ
-000020b0: 6573 7473 2066 726f 6d20 7468 6520 7661  ests from the va
-000020c0: 7269 6f75 7320 6461 7461 6261 7365 7321  rious databases!
-000020d0: 2920 596f 7520 616c 736f 2068 6176 6520  ) You also have 
-000020e0: 746f 2068 6176 6520 7468 6520 6c69 7374  to have the list
-000020f0: 206f 6620 7661 6c69 6420 696e 7075 7420   of valid input 
-00002100: 636f 6465 7320 666f 7220 6561 6368 2070  codes for each p
-00002110: 6172 616d 6574 6572 2e20 5468 6520 6069  arameter. The `i
-00002120: 6d66 702e 696d 665f 7061 7261 6d65 7465  mfp.imf_paramete
-00002130: 7273 6020 6675 6e63 7469 6f6e 2073 6f6c  rs` function sol
-00002140: 7665 7320 7468 6973 2070 726f 626c 656d  ves this problem
-00002150: 2e20 5573 6520 7468 6520 6675 6e63 7469  . Use the functi
-00002160: 6f6e 2074 6f20 6f62 7461 696e 2074 6865  on to obtain the
-00002170: 2066 756c 6c20 6c69 7374 206f 6620 7061   full list of pa
-00002180: 7261 6d65 7465 7273 2061 6e64 2076 616c  rameters and val
-00002190: 6964 2069 6e70 7574 2063 6f64 6573 2066  id input codes f
-000021a0: 6f72 2061 2067 6976 656e 2064 6174 6162  or a given datab
-000021b0: 6173 653a 0d0a 0d0a 0d0a 6060 6070 7974  ase:......```pyt
-000021c0: 686f 6e0d 0a23 2046 6574 6368 206c 6973  hon..# Fetch lis
-000021d0: 7420 6f66 2076 616c 6964 2070 6172 616d  t of valid param
-000021e0: 6574 6572 7320 616e 6420 696e 7075 7420  eters and input 
-000021f0: 636f 6465 7320 666f 7220 636f 6d6d 6f64  codes for commod
-00002200: 6974 7920 7072 6963 6520 6461 7461 6261  ity price databa
-00002210: 7365 0d0a 7061 7261 6d73 203d 2069 6d66  se..params = imf
-00002220: 702e 696d 665f 7061 7261 6d65 7465 7273  p.imf_parameters
-00002230: 2822 5043 5053 2229 0d0a 6060 600d 0a0d  ("PCPS")..```...
-00002240: 0a54 6865 2060 696d 6670 2e69 6d66 5f70  .The `imfp.imf_p
-00002250: 6172 616d 6574 6572 7360 2066 756e 6374  arameters` funct
-00002260: 696f 6e20 7265 7475 726e 7320 6120 6469  ion returns a di
-00002270: 6374 696f 6e61 7279 206f 6620 6461 7461  ctionary of data
-00002280: 2066 7261 6d65 732e 2045 6163 6820 6469   frames. Each di
-00002290: 6374 696f 6e61 7279 206b 6579 206e 616d  ctionary key nam
-000022a0: 6520 636f 7272 6573 706f 6e64 7320 746f  e corresponds to
-000022b0: 2061 2070 6172 616d 6574 6572 2075 7365   a parameter use
-000022c0: 6420 696e 206d 616b 696e 6720 7265 7175  d in making requ
-000022d0: 6573 7473 2066 726f 6d20 7468 6520 6461  ests from the da
-000022e0: 7461 6261 7365 3a0d 0a0d 0a0d 0a60 6060  tabase:......```
-000022f0: 7079 7468 6f6e 0d0a 2320 4765 7420 6b65  python..# Get ke
-00002300: 7920 6e61 6d65 7320 6672 6f6d 2074 6865  y names from the
-00002310: 2070 6172 616d 7320 6f62 6a65 6374 0d0a   params object..
-00002320: 7061 7261 6d73 2e6b 6579 7328 290d 0a60  params.keys()..`
-00002330: 6060 0d0a 0d0a 0d0a 0d0a 0d0a 2020 2020  ``..........    
-00002340: 6469 6374 5f6b 6579 7328 5b27 6672 6571  dict_keys(['freq
-00002350: 272c 2027 7265 665f 6172 6561 272c 2027  ', 'ref_area', '
-00002360: 636f 6d6d 6f64 6974 7927 2c20 2775 6e69  commodity', 'uni
-00002370: 745f 6d65 6173 7572 6527 5d29 0d0a 0d0a  t_measure'])....
-00002380: 0d0a 0d0a 496e 2074 6865 2065 7665 6e74  ....In the event
-00002390: 2074 6861 7420 6120 7061 7261 6d65 7465   that a paramete
-000023a0: 7220 6e61 6d65 2069 7320 6e6f 7420 7365  r name is not se
-000023b0: 6c66 2d65 7870 6c61 6e61 746f 7279 2c20  lf-explanatory, 
-000023c0: 7468 6520 6069 6d66 702e 696d 665f 7061  the `imfp.imf_pa
-000023d0: 7261 6d65 7465 725f 6465 6673 6020 6675  rameter_defs` fu
-000023e0: 6e63 7469 6f6e 2063 616e 2062 6520 7573  nction can be us
-000023f0: 6564 2074 6f20 6665 7463 6820 7368 6f72  ed to fetch shor
-00002400: 7420 7465 7874 2064 6573 6372 6970 7469  t text descripti
-00002410: 6f6e 7320 6f66 2065 6163 6820 7061 7261  ons of each para
-00002420: 6d65 7465 723a 0d0a 0d0a 0d0a 6060 6070  meter:......```p
-00002430: 7974 686f 6e0d 0a23 2046 6574 6368 2061  ython..# Fetch a
-00002440: 6e64 2064 6973 706c 6179 2070 6172 616d  nd display param
-00002450: 6574 6572 2074 6578 7420 6465 7363 7269  eter text descri
-00002460: 7074 696f 6e73 2066 6f72 2074 6865 2063  ptions for the c
-00002470: 6f6d 6d6f 6469 7479 2070 7269 6365 2064  ommodity price d
-00002480: 6174 6162 6173 650d 0a69 6d66 702e 696d  atabase..imfp.im
-00002490: 665f 7061 7261 6d65 7465 725f 6465 6673  f_parameter_defs
-000024a0: 2822 5043 5053 2229 0d0a 6060 600d 0a0d  ("PCPS")..```...
-000024b0: 0a0d 0a0d 0a0d 0a3c 6469 763e 0d0a 0d0a  .......<div>....
-000024c0: 3c74 6162 6c65 2062 6f72 6465 723d 2231  <table border="1
-000024d0: 2220 636c 6173 733d 2264 6174 6166 7261  " class="datafra
-000024e0: 6d65 223e 0d0a 2020 3c74 6865 6164 3e0d  me">..  <thead>.
-000024f0: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
-00002500: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
-00002510: 743b 223e 0d0a 2020 2020 2020 3c74 683e  t;">..      <th>
-00002520: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
-00002530: 3e70 6172 616d 6574 6572 3c2f 7468 3e0d  >parameter</th>.
-00002540: 0a20 2020 2020 203c 7468 3e64 6573 6372  .      <th>descr
-00002550: 6970 7469 6f6e 3c2f 7468 3e0d 0a20 2020  iption</th>..   
-00002560: 203c 2f74 723e 0d0a 2020 3c2f 7468 6561   </tr>..  </thea
-00002570: 643e 0d0a 2020 3c74 626f 6479 3e0d 0a20  d>..  <tbody>.. 
-00002580: 2020 203c 7472 3e0d 0a20 2020 2020 203c     <tr>..      <
-00002590: 7468 3e30 3c2f 7468 3e0d 0a20 2020 2020  th>0</th>..     
-000025a0: 203c 7464 3e66 7265 713c 2f74 643e 0d0a   <td>freq</td>..
-000025b0: 2020 2020 2020 3c74 643e 4672 6571 7565        <td>Freque
-000025c0: 6e63 793c 2f74 643e 0d0a 2020 2020 3c2f  ncy</td>..    </
-000025d0: 7472 3e0d 0a20 2020 203c 7472 3e0d 0a20  tr>..    <tr>.. 
-000025e0: 2020 2020 203c 7468 3e31 3c2f 7468 3e0d       <th>1</th>.
-000025f0: 0a20 2020 2020 203c 7464 3e72 6566 5f61  .      <td>ref_a
-00002600: 7265 613c 2f74 643e 0d0a 2020 2020 2020  rea</td>..      
-00002610: 3c74 643e 4765 6f67 7261 7068 6963 616c  <td>Geographical
-00002620: 2041 7265 6173 3c2f 7464 3e0d 0a20 2020   Areas</td>..   
-00002630: 203c 2f74 723e 0d0a 2020 2020 3c74 723e   </tr>..    <tr>
-00002640: 0d0a 2020 2020 2020 3c74 683e 323c 2f74  ..      <th>2</t
-00002650: 683e 0d0a 2020 2020 2020 3c74 643e 636f  h>..      <td>co
-00002660: 6d6d 6f64 6974 793c 2f74 643e 0d0a 2020  mmodity</td>..  
-00002670: 2020 2020 3c74 643e 496e 6469 6361 746f      <td>Indicato
-00002680: 723c 2f74 643e 0d0a 2020 2020 3c2f 7472  r</td>..    </tr
-00002690: 3e0d 0a20 2020 203c 7472 3e0d 0a20 2020  >..    <tr>..   
-000026a0: 2020 203c 7468 3e33 3c2f 7468 3e0d 0a20     <th>3</th>.. 
-000026b0: 2020 2020 203c 7464 3e75 6e69 745f 6d65       <td>unit_me
-000026c0: 6173 7572 653c 2f74 643e 0d0a 2020 2020  asure</td>..    
-000026d0: 2020 3c74 643e 556e 6974 3c2f 7464 3e0d    <td>Unit</td>.
-000026e0: 0a20 2020 203c 2f74 723e 0d0a 2020 3c2f  .    </tr>..  </
-000026f0: 7462 6f64 793e 0d0a 3c2f 7461 626c 653e  tbody>..</table>
-00002700: 0d0a 3c2f 6469 763e 0d0a 0d0a 0d0a 0d0a  ..</div>........
-00002710: 4561 6368 206e 616d 6564 206c 6973 7420  Each named list 
-00002720: 6974 656d 2069 7320 6120 6461 7461 2066  item is a data f
-00002730: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
-00002740: 6120 7665 6374 6f72 206f 6620 7661 6c69  a vector of vali
-00002750: 6420 696e 7075 7420 636f 6465 7320 7468  d input codes th
-00002760: 6174 2063 616e 2062 6520 7573 6564 2077  at can be used w
-00002770: 6974 6820 7468 6520 6e61 6d65 6420 7061  ith the named pa
-00002780: 7261 6d65 7465 722c 2061 6e64 2061 2076  rameter, and a v
-00002790: 6563 746f 7220 6f66 2074 6578 7420 6465  ector of text de
-000027a0: 7363 7269 7074 696f 6e73 206f 6620 7768  scriptions of wh
-000027b0: 6174 2065 6163 6820 636f 6465 2072 6570  at each code rep
-000027c0: 7265 7365 6e74 732e 0d0a 0d0a 546f 2061  resents.....To a
-000027d0: 6363 6573 7320 7468 6520 6461 7461 2066  ccess the data f
-000027e0: 7261 6d65 2063 6f6e 7461 696e 696e 6720  rame containing 
-000027f0: 7661 6c69 6420 7661 6c75 6573 2066 6f72  valid values for
-00002800: 2065 6163 6820 7061 7261 6d65 7465 722c   each parameter,
-00002810: 2073 7562 7365 7420 7468 6520 6070 6172   subset the `par
-00002820: 616d 7360 2064 6963 7420 6279 2074 6865  ams` dict by the
-00002830: 2070 6172 616d 6574 6572 206e 616d 653a   parameter name:
-00002840: 0d0a 0d0a 0d0a 6060 6070 7974 686f 6e0d  ......```python.
-00002850: 0a23 2056 6965 7720 7468 6520 6461 7461  .# View the data
-00002860: 2066 7261 6d65 206f 6620 7661 6c69 6420   frame of valid 
-00002870: 696e 7075 7420 636f 6465 7320 666f 7220  input codes for 
-00002880: 7468 6520 6672 6571 7565 6e63 7920 7061  the frequency pa
-00002890: 7261 6d65 7465 720d 0a70 6172 616d 735b  rameter..params[
-000028a0: 2766 7265 7127 5d0d 0a60 6060 0d0a 0d0a  'freq']..```....
-000028b0: 0d0a 0d0a 0d0a 3c64 6976 3e0d 0a0d 0a3c  ......<div>....<
-000028c0: 7461 626c 6520 626f 7264 6572 3d22 3122  table border="1"
-000028d0: 2063 6c61 7373 3d22 6461 7461 6672 616d   class="datafram
-000028e0: 6522 3e0d 0a20 203c 7468 6561 643e 0d0a  e">..  <thead>..
-000028f0: 2020 2020 3c74 7220 7374 796c 653d 2274      <tr style="t
-00002900: 6578 742d 616c 6967 6e3a 2072 6967 6874  ext-align: right
-00002910: 3b22 3e0d 0a20 2020 2020 203c 7468 3e3c  ;">..      <th><
-00002920: 2f74 683e 0d0a 2020 2020 2020 3c74 683e  /th>..      <th>
-00002930: 696e 7075 745f 636f 6465 3c2f 7468 3e0d  input_code</th>.
-00002940: 0a20 2020 2020 203c 7468 3e64 6573 6372  .      <th>descr
-00002950: 6970 7469 6f6e 3c2f 7468 3e0d 0a20 2020  iption</th>..   
-00002960: 203c 2f74 723e 0d0a 2020 3c2f 7468 6561   </tr>..  </thea
-00002970: 643e 0d0a 2020 3c74 626f 6479 3e0d 0a20  d>..  <tbody>.. 
-00002980: 2020 203c 7472 3e0d 0a20 2020 2020 203c     <tr>..      <
-00002990: 7468 3e30 3c2f 7468 3e0d 0a20 2020 2020  th>0</th>..     
-000029a0: 203c 7464 3e41 3c2f 7464 3e0d 0a20 2020   <td>A</td>..   
-000029b0: 2020 203c 7464 3e41 6e6e 7561 6c3c 2f74     <td>Annual</t
-000029c0: 643e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  d>..    </tr>.. 
-000029d0: 2020 203c 7472 3e0d 0a20 2020 2020 203c     <tr>..      <
-000029e0: 7468 3e31 3c2f 7468 3e0d 0a20 2020 2020  th>1</th>..     
-000029f0: 203c 7464 3e4d 3c2f 7464 3e0d 0a20 2020   <td>M</td>..   
-00002a00: 2020 203c 7464 3e4d 6f6e 7468 6c79 3c2f     <td>Monthly</
-00002a10: 7464 3e0d 0a20 2020 203c 2f74 723e 0d0a  td>..    </tr>..
-00002a20: 2020 2020 3c74 723e 0d0a 2020 2020 2020      <tr>..      
-00002a30: 3c74 683e 323c 2f74 683e 0d0a 2020 2020  <th>2</th>..    
-00002a40: 2020 3c74 643e 513c 2f74 643e 0d0a 2020    <td>Q</td>..  
-00002a50: 2020 2020 3c74 643e 5175 6172 7465 726c      <td>Quarterl
-00002a60: 793c 2f74 643e 0d0a 2020 2020 3c2f 7472  y</td>..    </tr
-00002a70: 3e0d 0a20 203c 2f74 626f 6479 3e0d 0a3c  >..  </tbody>..<
-00002a80: 2f74 6162 6c65 3e0d 0a3c 2f64 6976 3e0d  /table>..</div>.
-00002a90: 0a0d 0a0d 0a0d 0a23 2323 2056 6965 7769  .......### Viewi
-00002aa0: 6e67 2044 6174 6120 4672 616d 6573 0d0a  ng Data Frames..
-00002ab0: 0d0a 4e6f 7465 2074 6861 7420 6070 616e  ..Note that `pan
-00002ac0: 6461 7360 2064 6174 6120 6672 616d 6573  das` data frames
-00002ad0: 2069 6e20 5079 7468 6f6e 2063 616e 2062   in Python can b
-00002ae0: 6520 6120 6c69 7474 6c65 2064 6966 6669  e a little diffi
-00002af0: 6375 6c74 2074 6f20 776f 726b 2077 6974  cult to work wit
-00002b00: 682c 2062 6563 6175 7365 2050 7974 686f  h, because Pytho
-00002b10: 6e20 646f 6573 6e27 7420 6861 7665 2061  n doesn't have a
-00002b20: 2062 7569 6c74 2d69 6e20 7661 7269 6162   built-in variab
-00002b30: 6c65 2065 7870 6c6f 7265 722e 2049 6620  le explorer. If 
-00002b40: 796f 7527 7265 2064 6f69 6e67 2064 6174  you're doing dat
-00002b50: 6120 7363 6965 6e63 652c 2049 2072 6563  a science, I rec
-00002b60: 6f6d 6d65 6e64 2075 7369 6e67 2061 6e20  ommend using an 
-00002b70: 4944 4520 6c69 6b65 2052 5374 7564 696f  IDE like RStudio
-00002b80: 206f 7220 5370 7964 6572 2074 6861 7420   or Spyder that 
-00002b90: 6861 7320 6120 6275 696c 742d 696e 2076  has a built-in v
-00002ba0: 6172 6961 626c 6520 6578 706c 6f72 6572  ariable explorer
-00002bb0: 2e20 486f 7765 7665 722c 2069 6620 796f  . However, if yo
-00002bc0: 7520 646f 6e27 7420 6861 7665 2061 2076  u don't have a v
-00002bd0: 6172 6961 626c 6520 6578 706c 6f72 6572  ariable explorer
-00002be0: 2c20 796f 7520 6361 6e20 7072 6576 656e  , you can preven
-00002bf0: 7420 5079 7468 6f6e 2066 726f 6d20 7472  t Python from tr
-00002c00: 756e 6361 7469 6e67 2064 6174 6120 6672  uncating data fr
-00002c10: 616d 6573 2075 7369 6e67 2074 6865 2060  ames using the `
-00002c20: 6f70 7469 6f6e 7360 2069 6e20 6070 616e  options` in `pan
-00002c30: 6461 7360 2e20 466f 7220 696e 7374 616e  das`. For instan
-00002c40: 6365 2c20 746f 2069 6e63 7265 6173 6520  ce, to increase 
-00002c50: 7468 6520 6d61 7869 6d75 6d20 616c 6c6f  the maximum allo
-00002c60: 7765 6420 636f 6c75 6d6e 2077 6964 7468  wed column width
-00002c70: 2074 6f20 3130 3020 6368 6172 6163 7465   to 100 characte
-00002c80: 7273 2c20 7765 2063 616e 2075 7365 2060  rs, we can use `
-00002c90: 7061 6e64 6173 2e6f 7074 696f 6e73 2e64  pandas.options.d
-00002ca0: 6973 706c 6179 2e6d 6178 5f63 6f6c 7769  isplay.max_colwi
-00002cb0: 6474 6820 3d20 3130 3060 2e0d 0a0d 0a41  dth = 100`.....A
-00002cc0: 6c74 6572 6e61 7469 7665 6c79 2c20 6974  lternatively, it
-00002cd0: 2773 2070 6f73 7369 626c 6520 746f 206f  's possible to o
-00002ce0: 7065 6e20 7468 6520 6461 7461 2066 7261  pen the data fra
-00002cf0: 6d65 2069 6e20 6120 6e65 7720 7769 6e64  me in a new wind
-00002d00: 6f77 2074 6f20 7669 6577 2069 7420 696e  ow to view it in
-00002d10: 2066 756c 6c3a 0d0a 0d0a 0d0a 6060 6070   full:......```p
-00002d20: 7974 686f 6e0d 0a69 6d70 6f72 7420 696d  ython..import im
-00002d30: 6670 0d0a 696d 706f 7274 2074 656d 7066  fp..import tempf
-00002d40: 696c 650d 0a69 6d70 6f72 7420 7765 6262  ile..import webb
-00002d50: 726f 7773 6572 0d0a 0d0a 2320 4465 6669  rowser....# Defi
-00002d60: 6e65 2061 2073 696d 706c 6520 6675 6e63  ne a simple func
-00002d70: 7469 6f6e 2074 6f20 7669 6577 2064 6174  tion to view dat
-00002d80: 6120 6672 616d 6520 696e 2061 2062 726f  a frame in a bro
-00002d90: 7773 6572 2077 696e 646f 770d 0a64 6566  wser window..def
-00002da0: 2056 6965 7728 6466 293a 0d0a 2020 2020   View(df):..    
-00002db0: 6874 6d6c 203d 2064 662e 746f 5f68 746d  html = df.to_htm
-00002dc0: 6c28 290d 0a20 2020 2077 6974 6820 7465  l()..    with te
-00002dd0: 6d70 6669 6c65 2e4e 616d 6564 5465 6d70  mpfile.NamedTemp
-00002de0: 6f72 6172 7946 696c 6528 2777 272c 2064  oraryFile('w', d
-00002df0: 656c 6574 653d 4661 6c73 652c 2073 7566  elete=False, suf
-00002e00: 6669 783d 272e 6874 6d6c 2729 2061 7320  fix='.html') as 
-00002e10: 663a 0d0a 2020 2020 2020 2020 7572 6c20  f:..        url 
-00002e20: 3d20 2766 696c 653a 2f2f 2720 2b20 662e  = 'file://' + f.
-00002e30: 6e61 6d65 0d0a 2020 2020 2020 2020 662e  name..        f.
-00002e40: 7772 6974 6528 6874 6d6c 290d 0a20 2020  write(html)..   
-00002e50: 2077 6562 6272 6f77 7365 722e 6f70 656e   webbrowser.open
-00002e60: 2875 726c 290d 0a0d 0a23 204f 7065 6e20  (url)....# Open 
-00002e70: 6461 7461 2066 7261 6d65 2069 6e20 6120  data frame in a 
-00002e80: 6e65 7720 6272 6f77 7365 7220 7769 6e64  new browser wind
-00002e90: 6f77 2075 7369 6e67 2074 6865 2066 756e  ow using the fun
-00002ea0: 6374 696f 6e0d 0a64 6620 3d20 696d 6670  ction..df = imfp
-00002eb0: 2e69 6d66 5f64 6174 6162 6173 6573 2829  .imf_databases()
-00002ec0: 0d0a 5669 6577 2864 6629 0d0a 6060 600d  ..View(df)..```.
-00002ed0: 0a0d 0a23 2323 2053 7570 706c 7969 6e67  ...### Supplying
-00002ee0: 2050 6172 616d 6574 6572 2041 7267 756d   Parameter Argum
-00002ef0: 656e 7473 2074 6f20 696d 665f 6461 7461  ents to imf_data
-00002f00: 7365 743a 2041 2054 616c 6520 6f66 2054  set: A Tale of T
-00002f10: 776f 2057 6f72 6b66 6c6f 7773 0d0a 0d0a  wo Workflows....
-00002f20: 5468 6572 6520 6172 6520 7477 6f20 7761  There are two wa
-00002f30: 7973 2074 6f20 7375 7070 6c79 2070 6172  ys to supply par
-00002f40: 616d 6574 6572 7320 746f 2060 696d 6670  ameters to `imfp
-00002f50: 2e69 6d66 5f64 6174 6173 6574 603a 2062  .imf_dataset`: b
-00002f60: 7920 7375 7070 6c79 696e 6720 6c69 7374  y supplying list
-00002f70: 2061 7267 756d 656e 7473 206f 7220 6279   arguments or by
-00002f80: 2073 7570 706c 7969 6e67 2061 206d 6f64   supplying a mod
-00002f90: 6966 6965 6420 7061 7261 6d65 7465 7273  ified parameters
-00002fa0: 2064 6963 742e 2054 6865 206c 6973 7420   dict. The list 
-00002fb0: 6172 6775 6d65 6e74 7320 776f 726b 666c  arguments workfl
-00002fc0: 6f77 2077 696c 6c20 6265 206d 6f72 6520  ow will be more 
-00002fd0: 696e 7475 6974 6976 6520 666f 7220 6d6f  intuitive for mo
-00002fe0: 7374 2075 7365 7273 2c20 6275 7420 7468  st users, but th
-00002ff0: 6520 6469 6374 2061 7267 756d 656e 7420  e dict argument 
-00003000: 776f 726b 666c 6f77 2072 6571 7569 7265  workflow require
-00003010: 7320 6120 6c69 7474 6c65 206c 6573 7320  s a little less 
-00003020: 636f 6465 2e0d 0a0d 0a23 2323 2320 5468  code.....#### Th
-00003030: 6520 4c69 7374 2041 7267 756d 656e 7473  e List Arguments
-00003040: 2057 6f72 6b66 6c6f 770d 0a0d 0a54 6f20   Workflow....To 
-00003050: 7375 7070 6c79 206c 6973 7420 6172 6775  supply list argu
-00003060: 6d65 6e74 732c 206a 7573 7420 6669 6e64  ments, just find
-00003070: 2074 6865 2063 6f64 6573 2079 6f75 2077   the codes you w
-00003080: 616e 7420 616e 6420 7375 7070 6c79 2074  ant and supply t
-00003090: 6865 6d20 746f 2060 696d 6670 2e69 6d66  hem to `imfp.imf
-000030a0: 5f64 6174 6173 6574 6020 7573 696e 6720  _dataset` using 
-000030b0: 7468 6520 7061 7261 6d65 7465 7220 6e61  the parameter na
-000030c0: 6d65 2061 7320 7468 6520 6172 6775 6d65  me as the argume
-000030d0: 6e74 206e 616d 652e 2054 6865 2065 7861  nt name. The exa
-000030e0: 6d70 6c65 2062 656c 6f77 2073 686f 7773  mple below shows
-000030f0: 2068 6f77 2074 6f20 7265 7175 6573 7420   how to request 
-00003100: 3230 3030 e280 9332 3031 3520 616e 6e75  2000...2015 annu
-00003110: 616c 2063 6f61 6c20 7072 6963 6573 2066  al coal prices f
-00003120: 726f 6d20 7468 6520 5072 696d 6172 7920  rom the Primary 
-00003130: 436f 6d6d 6f64 6974 7920 5072 6963 6520  Commodity Price 
-00003140: 5379 7374 656d 2064 6174 6162 6173 653a  System database:
-00003150: 0d0a 0d0a 0d0a 6060 6070 7974 686f 6e0d  ......```python.
-00003160: 0a23 2046 6574 6368 2074 6865 2027 6672  .# Fetch the 'fr
-00003170: 6571 2720 696e 7075 7420 636f 6465 2066  eq' input code f
-00003180: 6f72 2061 6e6e 7561 6c20 6672 6571 7565  or annual freque
-00003190: 6e63 790d 0a73 656c 6563 7465 645f 6672  ncy..selected_fr
-000031a0: 6571 203d 206c 6973 7428 0d0a 2020 2020  eq = list(..    
-000031b0: 7061 7261 6d73 5b27 6672 6571 275d 5b27  params['freq']['
-000031c0: 696e 7075 745f 636f 6465 275d 5b70 6172  input_code'][par
-000031d0: 616d 735b 2766 7265 7127 5d5b 2764 6573  ams['freq']['des
-000031e0: 6372 6970 7469 6f6e 275d 2e73 7472 2e63  cription'].str.c
-000031f0: 6f6e 7461 696e 7328 2241 6e6e 7561 6c22  ontains("Annual"
-00003200: 295d 0d0a 290d 0a0d 0a23 2046 6574 6368  )]..)....# Fetch
-00003210: 2074 6865 2027 636f 6d6d 6f64 6974 7927   the 'commodity'
-00003220: 2069 6e70 7574 2063 6f64 6520 666f 7220   input code for 
-00003230: 636f 616c 0d0a 7365 6c65 6374 6564 5f63  coal..selected_c
-00003240: 6f6d 6d6f 6469 7479 203d 206c 6973 7428  ommodity = list(
-00003250: 0d0a 2020 2020 7061 7261 6d73 5b27 636f  ..    params['co
-00003260: 6d6d 6f64 6974 7927 5d5b 2769 6e70 7574  mmodity']['input
-00003270: 5f63 6f64 6527 5d5b 7061 7261 6d73 5b27  _code'][params['
-00003280: 636f 6d6d 6f64 6974 7927 5d5b 2764 6573  commodity']['des
-00003290: 6372 6970 7469 6f6e 275d 2e73 7472 2e63  cription'].str.c
-000032a0: 6f6e 7461 696e 7328 2243 6f61 6c22 295d  ontains("Coal")]
-000032b0: 0d0a 290d 0a0d 0a23 2046 6574 6368 2074  ..)....# Fetch t
-000032c0: 6865 2027 756e 6974 5f6d 6561 7375 7265  he 'unit_measure
-000032d0: 2720 696e 7075 7420 636f 6465 2066 6f72  ' input code for
-000032e0: 2069 6e64 6578 0d0a 7365 6c65 6374 6564   index..selected
-000032f0: 5f75 6e69 745f 6d65 6173 7572 6520 3d20  _unit_measure = 
-00003300: 6c69 7374 280d 0a20 2020 2070 6172 616d  list(..    param
-00003310: 735b 2775 6e69 745f 6d65 6173 7572 6527  s['unit_measure'
-00003320: 5d5b 2769 6e70 7574 5f63 6f64 6527 5d5b  ]['input_code'][
-00003330: 7061 7261 6d73 5b27 756e 6974 5f6d 6561  params['unit_mea
-00003340: 7375 7265 275d 5b27 6465 7363 7269 7074  sure']['descript
-00003350: 696f 6e27 5d2e 7374 722e 636f 6e74 6169  ion'].str.contai
-00003360: 6e73 2822 496e 6465 7822 295d 0d0a 290d  ns("Index")]..).
-00003370: 0a0d 0a23 2052 6571 7565 7374 2064 6174  ...# Request dat
-00003380: 6120 6672 6f6d 2074 6865 2041 5049 0d0a  a from the API..
-00003390: 6466 203d 2069 6d66 702e 696d 665f 6461  df = imfp.imf_da
-000033a0: 7461 7365 7428 6461 7461 6261 7365 5f69  taset(database_i
-000033b0: 6420 3d20 2250 4350 5322 2c0d 0a20 2020  d = "PCPS",..   
-000033c0: 2020 2020 2020 6672 6571 203d 2073 656c        freq = sel
-000033d0: 6563 7465 645f 6672 6571 2c20 636f 6d6d  ected_freq, comm
-000033e0: 6f64 6974 7920 3d20 7365 6c65 6374 6564  odity = selected
-000033f0: 5f63 6f6d 6d6f 6469 7479 2c0d 0a20 2020  _commodity,..   
-00003400: 2020 2020 2020 756e 6974 5f6d 6561 7375        unit_measu
-00003410: 7265 203d 2073 656c 6563 7465 645f 756e  re = selected_un
-00003420: 6974 5f6d 6561 7375 7265 2c0d 0a20 2020  it_measure,..   
-00003430: 2020 2020 2020 7374 6172 745f 7965 6172        start_year
-00003440: 203d 2032 3030 302c 2065 6e64 5f79 6561   = 2000, end_yea
-00003450: 7220 3d20 3230 3135 290d 0a0d 0a23 2044  r = 2015)....# D
-00003460: 6973 706c 6179 2074 6865 2066 6972 7374  isplay the first
-00003470: 2066 6577 2065 6e74 7269 6573 2069 6e20   few entries in 
-00003480: 7468 6520 7265 7472 6965 7665 6420 6461  the retrieved da
-00003490: 7461 2066 7261 6d65 0d0a 6466 2e68 6561  ta frame..df.hea
-000034a0: 6428 290d 0a60 6060 0d0a 0d0a 0d0a 0d0a  d()..```........
-000034b0: 0d0a 3c64 6976 3e0d 0a0d 0a3c 7461 626c  ..<div>....<tabl
-000034c0: 6520 626f 7264 6572 3d22 3122 2063 6c61  e border="1" cla
-000034d0: 7373 3d22 6461 7461 6672 616d 6522 3e0d  ss="dataframe">.
-000034e0: 0a20 203c 7468 6561 643e 0d0a 2020 2020  .  <thead>..    
-000034f0: 3c74 7220 7374 796c 653d 2274 6578 742d  <tr style="text-
-00003500: 616c 6967 6e3a 2072 6967 6874 3b22 3e0d  align: right;">.
-00003510: 0a20 2020 2020 203c 7468 3e3c 2f74 683e  .      <th></th>
-00003520: 0d0a 2020 2020 2020 3c74 683e 6672 6571  ..      <th>freq
-00003530: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
-00003540: 3e72 6566 5f61 7265 613c 2f74 683e 0d0a  >ref_area</th>..
-00003550: 2020 2020 2020 3c74 683e 636f 6d6d 6f64        <th>commod
-00003560: 6974 793c 2f74 683e 0d0a 2020 2020 2020  ity</th>..      
-00003570: 3c74 683e 756e 6974 5f6d 6561 7375 7265  <th>unit_measure
-00003580: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
-00003590: 3e75 6e69 745f 6d75 6c74 3c2f 7468 3e0d  >unit_mult</th>.
-000035a0: 0a20 2020 2020 203c 7468 3e74 696d 655f  .      <th>time_
-000035b0: 666f 726d 6174 3c2f 7468 3e0d 0a20 2020  format</th>..   
-000035c0: 2020 203c 7468 3e74 696d 655f 7065 7269     <th>time_peri
-000035d0: 6f64 3c2f 7468 3e0d 0a20 2020 2020 203c  od</th>..      <
-000035e0: 7468 3e6f 6273 5f76 616c 7565 3c2f 7468  th>obs_value</th
-000035f0: 3e0d 0a20 2020 203c 2f74 723e 0d0a 2020  >..    </tr>..  
-00003600: 3c2f 7468 6561 643e 0d0a 2020 3c74 626f  </thead>..  <tbo
-00003610: 6479 3e0d 0a20 2020 203c 7472 3e0d 0a20  dy>..    <tr>.. 
-00003620: 2020 2020 203c 7468 3e30 3c2f 7468 3e0d       <th>0</th>.
-00003630: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
-00003640: 3e0d 0a20 2020 2020 203c 7464 3e57 3030  >..      <td>W00
-00003650: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-00003660: 3e50 434f 414c 3c2f 7464 3e0d 0a20 2020  >PCOAL</td>..   
-00003670: 2020 203c 7464 3e49 583c 2f74 643e 0d0a     <td>IX</td>..
-00003680: 2020 2020 2020 3c74 643e 303c 2f74 643e        <td>0</td>
-00003690: 0d0a 2020 2020 2020 3c74 643e 5031 593c  ..      <td>P1Y<
-000036a0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-000036b0: 3230 3030 3c2f 7464 3e0d 0a20 2020 2020  2000</td>..     
-000036c0: 203c 7464 3e33 392e 3335 3130 3233 3032   <td>39.35102302
-000036d0: 3933 3230 323c 2f74 643e 0d0a 2020 2020  93202</td>..    
-000036e0: 3c2f 7472 3e0d 0a20 2020 203c 7472 3e0d  </tr>..    <tr>.
-000036f0: 0a20 2020 2020 203c 7468 3e31 3c2f 7468  .      <th>1</th
-00003700: 3e0d 0a20 2020 2020 203c 7464 3e41 3c2f  >..      <td>A</
-00003710: 7464 3e0d 0a20 2020 2020 203c 7464 3e57  td>..      <td>W
-00003720: 3030 3c2f 7464 3e0d 0a20 2020 2020 203c  00</td>..      <
-00003730: 7464 3e50 434f 414c 3c2f 7464 3e0d 0a20  td>PCOAL</td>.. 
-00003740: 2020 2020 203c 7464 3e49 583c 2f74 643e       <td>IX</td>
-00003750: 0d0a 2020 2020 2020 3c74 643e 303c 2f74  ..      <td>0</t
-00003760: 643e 0d0a 2020 2020 2020 3c74 643e 5031  d>..      <td>P1
-00003770: 593c 2f74 643e 0d0a 2020 2020 2020 3c74  Y</td>..      <t
-00003780: 643e 3230 3031 3c2f 7464 3e0d 0a20 2020  d>2001</td>..   
-00003790: 2020 203c 7464 3e34 392e 3333 3738 3538     <td>49.337858
-000037a0: 3732 3834 3033 393c 2f74 643e 0d0a 2020  7284039</td>..  
-000037b0: 2020 3c2f 7472 3e0d 0a20 2020 203c 7472    </tr>..    <tr
-000037c0: 3e0d 0a20 2020 2020 203c 7468 3e32 3c2f  >..      <th>2</
-000037d0: 7468 3e0d 0a20 2020 2020 203c 7464 3e41  th>..      <td>A
-000037e0: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-000037f0: 3e57 3030 3c2f 7464 3e0d 0a20 2020 2020  >W00</td>..     
-00003800: 203c 7464 3e50 434f 414c 3c2f 7464 3e0d   <td>PCOAL</td>.
-00003810: 0a20 2020 2020 203c 7464 3e49 583c 2f74  .      <td>IX</t
-00003820: 643e 0d0a 2020 2020 2020 3c74 643e 303c  d>..      <td>0<
-00003830: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-00003840: 5031 593c 2f74 643e 0d0a 2020 2020 2020  P1Y</td>..      
-00003850: 3c74 643e 3230 3032 3c2f 7464 3e0d 0a20  <td>2002</td>.. 
-00003860: 2020 2020 203c 7464 3e33 392e 3439 3439       <td>39.4949
-00003870: 3039 3136 3438 3030 363c 2f74 643e 0d0a  091648006</td>..
-00003880: 2020 2020 3c2f 7472 3e0d 0a20 2020 203c      </tr>..    <
-00003890: 7472 3e0d 0a20 2020 2020 203c 7468 3e33  tr>..      <th>3
-000038a0: 3c2f 7468 3e0d 0a20 2020 2020 203c 7464  </th>..      <td
-000038b0: 3e41 3c2f 7464 3e0d 0a20 2020 2020 203c  >A</td>..      <
-000038c0: 7464 3e57 3030 3c2f 7464 3e0d 0a20 2020  td>W00</td>..   
-000038d0: 2020 203c 7464 3e50 434f 414c 3c2f 7464     <td>PCOAL</td
-000038e0: 3e0d 0a20 2020 2020 203c 7464 3e49 583c  >..      <td>IX<
-000038f0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-00003900: 303c 2f74 643e 0d0a 2020 2020 2020 3c74  0</td>..      <t
-00003910: 643e 5031 593c 2f74 643e 0d0a 2020 2020  d>P1Y</td>..    
-00003920: 2020 3c74 643e 3230 3033 3c2f 7464 3e0d    <td>2003</td>.
-00003930: 0a20 2020 2020 203c 7464 3e34 332e 3238  .      <td>43.28
-00003940: 3738 3837 3639 3530 3738 383c 2f74 643e  78876950788</td>
-00003950: 0d0a 2020 2020 3c2f 7472 3e0d 0a20 2020  ..    </tr>..   
-00003960: 203c 7472 3e0d 0a20 2020 2020 203c 7468   <tr>..      <th
-00003970: 3e34 3c2f 7468 3e0d 0a20 2020 2020 203c  >4</th>..      <
-00003980: 7464 3e41 3c2f 7464 3e0d 0a20 2020 2020  td>A</td>..     
-00003990: 203c 7464 3e57 3030 3c2f 7464 3e0d 0a20   <td>W00</td>.. 
-000039a0: 2020 2020 203c 7464 3e50 434f 414c 3c2f       <td>PCOAL</
-000039b0: 7464 3e0d 0a20 2020 2020 203c 7464 3e49  td>..      <td>I
-000039c0: 583c 2f74 643e 0d0a 2020 2020 2020 3c74  X</td>..      <t
-000039d0: 643e 303c 2f74 643e 0d0a 2020 2020 2020  d>0</td>..      
-000039e0: 3c74 643e 5031 593c 2f74 643e 0d0a 2020  <td>P1Y</td>..  
-000039f0: 2020 2020 3c74 643e 3230 3034 3c2f 7464      <td>2004</td
-00003a00: 3e0d 0a20 2020 2020 203c 7464 3e38 322e  >..      <td>82.
-00003a10: 3931 3835 3835 3830 3532 3836 323c 2f74  9185858052862</t
-00003a20: 643e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  d>..    </tr>.. 
-00003a30: 203c 2f74 626f 6479 3e0d 0a3c 2f74 6162   </tbody>..</tab
-00003a40: 6c65 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a0d  le>..</div>.....
-00003a50: 0a0d 0a23 2323 2320 5468 6520 5061 7261  ...#### The Para
-00003a60: 6d65 7465 7273 2041 7267 756d 656e 7420  meters Argument 
-00003a70: 576f 726b 666c 6f77 0d0a 0d0a 546f 2073  Workflow....To s
-00003a80: 7570 706c 7920 6120 6c69 7374 206f 626a  upply a list obj
-00003a90: 6563 742c 206d 6f64 6966 7920 6561 6368  ect, modify each
-00003aa0: 2064 6174 6120 6672 616d 6520 696e 2074   data frame in t
-00003ab0: 6865 2060 7061 7261 6d73 6020 6c69 7374  he `params` list
-00003ac0: 206f 626a 6563 7420 746f 2072 6574 6169   object to retai
-00003ad0: 6e20 6f6e 6c79 2074 6865 2072 6f77 7320  n only the rows 
-00003ae0: 796f 7520 7761 6e74 2c20 616e 6420 7468  you want, and th
-00003af0: 656e 2073 7570 706c 7920 7468 6520 6d6f  en supply the mo
-00003b00: 6469 6669 6564 206c 6973 7420 6f62 6a65  dified list obje
-00003b10: 6374 2074 6f20 6069 6d66 702e 696d 665f  ct to `imfp.imf_
-00003b20: 6461 7461 7365 7460 2061 7320 6974 7320  dataset` as its 
-00003b30: 7061 7261 6d65 7465 7273 2061 7267 756d  parameters argum
-00003b40: 656e 742e 2048 6572 6520 6973 2068 6f77  ent. Here is how
-00003b50: 2074 6f20 6d61 6b65 2074 6865 2073 616d   to make the sam
-00003b60: 6520 7265 7175 6573 7420 666f 7220 616e  e request for an
-00003b70: 6e75 616c 2063 6f61 6c20 7072 6963 6520  nual coal price 
-00003b80: 6461 7461 2075 7369 6e67 2061 2070 6172  data using a par
-00003b90: 616d 6574 6572 7320 6c69 7374 3a0d 0a0d  ameters list:...
-00003ba0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 2320  ...```python..# 
-00003bb0: 4665 7463 6820 7468 6520 2766 7265 7127  Fetch the 'freq'
-00003bc0: 2069 6e70 7574 2063 6f64 6520 666f 7220   input code for 
-00003bd0: 616e 6e75 616c 2066 7265 7175 656e 6379  annual frequency
-00003be0: 0d0a 7061 7261 6d73 5b27 6672 6571 275d  ..params['freq']
-00003bf0: 203d 2070 6172 616d 735b 2766 7265 7127   = params['freq'
-00003c00: 5d5b 7061 7261 6d73 5b27 6672 6571 275d  ][params['freq']
-00003c10: 5b27 6465 7363 7269 7074 696f 6e27 5d2e  ['description'].
-00003c20: 7374 722e 636f 6e74 6169 6e73 2822 416e  str.contains("An
-00003c30: 6e75 616c 2229 5d0d 0a0d 0a23 2046 6574  nual")]....# Fet
-00003c40: 6368 2074 6865 2027 636f 6d6d 6f64 6974  ch the 'commodit
-00003c50: 7927 2069 6e70 7574 2063 6f64 6528 7329  y' input code(s)
-00003c60: 2066 6f72 2063 6f61 6c0d 0a70 6172 616d   for coal..param
-00003c70: 735b 2763 6f6d 6d6f 6469 7479 275d 203d  s['commodity'] =
-00003c80: 2070 6172 616d 735b 2763 6f6d 6d6f 6469   params['commodi
-00003c90: 7479 275d 5b70 6172 616d 735b 2763 6f6d  ty'][params['com
-00003ca0: 6d6f 6469 7479 275d 5b27 6465 7363 7269  modity']['descri
-00003cb0: 7074 696f 6e27 5d2e 7374 722e 636f 6e74  ption'].str.cont
-00003cc0: 6169 6e73 2822 436f 616c 2229 5d0d 0a0d  ains("Coal")]...
-00003cd0: 0a23 2046 6574 6368 2074 6865 2027 756e  .# Fetch the 'un
-00003ce0: 6974 5f6d 6561 7375 7265 2720 696e 7075  it_measure' inpu
-00003cf0: 7420 636f 6465 2066 6f72 2069 6e64 6578  t code for index
-00003d00: 0d0a 7061 7261 6d73 5b27 756e 6974 5f6d  ..params['unit_m
-00003d10: 6561 7375 7265 275d 203d 2070 6172 616d  easure'] = param
-00003d20: 735b 2775 6e69 745f 6d65 6173 7572 6527  s['unit_measure'
-00003d30: 5d5b 7061 7261 6d73 5b27 756e 6974 5f6d  ][params['unit_m
-00003d40: 6561 7375 7265 275d 5b27 6465 7363 7269  easure']['descri
-00003d50: 7074 696f 6e27 5d2e 7374 722e 636f 6e74  ption'].str.cont
-00003d60: 6169 6e73 2822 496e 6465 7822 295d 0d0a  ains("Index")]..
-00003d70: 0d0a 2320 5265 7175 6573 7420 6461 7461  ..# Request data
-00003d80: 2066 726f 6d20 7468 6520 4150 490d 0a64   from the API..d
-00003d90: 6620 3d20 696d 6670 2e69 6d66 5f64 6174  f = imfp.imf_dat
-00003da0: 6173 6574 2864 6174 6162 6173 655f 6964  aset(database_id
-00003db0: 203d 2022 5043 5053 222c 0d0a 2020 2020   = "PCPS",..    
-00003dc0: 2020 2020 2070 6172 616d 6574 6572 7320       parameters 
-00003dd0: 3d20 7061 7261 6d73 2c0d 0a20 2020 2020  = params,..     
-00003de0: 2020 2020 7374 6172 745f 7965 6172 203d      start_year =
-00003df0: 2032 3030 302c 2065 6e64 5f79 6561 7220   2000, end_year 
-00003e00: 3d20 3230 3135 290d 0a0d 0a23 2044 6973  = 2015)....# Dis
-00003e10: 706c 6179 2074 6865 2066 6972 7374 2066  play the first f
-00003e20: 6577 2065 6e74 7269 6573 2069 6e20 7468  ew entries in th
-00003e30: 6520 7265 7472 6965 7665 6420 6461 7461  e retrieved data
-00003e40: 2066 7261 6d65 0d0a 6466 2e68 6561 6428   frame..df.head(
-00003e50: 290d 0a60 6060 0d0a 0d0a 0d0a 0d0a 0d0a  )..```..........
-00003e60: 3c64 6976 3e0d 0a0d 0a3c 7461 626c 6520  <div>....<table 
-00003e70: 626f 7264 6572 3d22 3122 2063 6c61 7373  border="1" class
-00003e80: 3d22 6461 7461 6672 616d 6522 3e0d 0a20  ="dataframe">.. 
-00003e90: 203c 7468 6561 643e 0d0a 2020 2020 3c74   <thead>..    <t
-00003ea0: 7220 7374 796c 653d 2274 6578 742d 616c  r style="text-al
-00003eb0: 6967 6e3a 2072 6967 6874 3b22 3e0d 0a20  ign: right;">.. 
-00003ec0: 2020 2020 203c 7468 3e3c 2f74 683e 0d0a       <th></th>..
-00003ed0: 2020 2020 2020 3c74 683e 6672 6571 3c2f        <th>freq</
-00003ee0: 7468 3e0d 0a20 2020 2020 203c 7468 3e72  th>..      <th>r
-00003ef0: 6566 5f61 7265 613c 2f74 683e 0d0a 2020  ef_area</th>..  
-00003f00: 2020 2020 3c74 683e 636f 6d6d 6f64 6974      <th>commodit
-00003f10: 793c 2f74 683e 0d0a 2020 2020 2020 3c74  y</th>..      <t
-00003f20: 683e 756e 6974 5f6d 6561 7375 7265 3c2f  h>unit_measure</
-00003f30: 7468 3e0d 0a20 2020 2020 203c 7468 3e75  th>..      <th>u
-00003f40: 6e69 745f 6d75 6c74 3c2f 7468 3e0d 0a20  nit_mult</th>.. 
-00003f50: 2020 2020 203c 7468 3e74 696d 655f 666f       <th>time_fo
-00003f60: 726d 6174 3c2f 7468 3e0d 0a20 2020 2020  rmat</th>..     
-00003f70: 203c 7468 3e74 696d 655f 7065 7269 6f64   <th>time_period
-00003f80: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
-00003f90: 3e6f 6273 5f76 616c 7565 3c2f 7468 3e0d  >obs_value</th>.
-00003fa0: 0a20 2020 203c 2f74 723e 0d0a 2020 3c2f  .    </tr>..  </
-00003fb0: 7468 6561 643e 0d0a 2020 3c74 626f 6479  thead>..  <tbody
-00003fc0: 3e0d 0a20 2020 203c 7472 3e0d 0a20 2020  >..    <tr>..   
-00003fd0: 2020 203c 7468 3e30 3c2f 7468 3e0d 0a20     <th>0</th>.. 
-00003fe0: 2020 2020 203c 7464 3e41 3c2f 7464 3e0d       <td>A</td>.
-00003ff0: 0a20 2020 2020 203c 7464 3e57 3030 3c2f  .      <td>W00</
-00004000: 7464 3e0d 0a20 2020 2020 203c 7464 3e50  td>..      <td>P
-00004010: 434f 414c 3c2f 7464 3e0d 0a20 2020 2020  COAL</td>..     
-00004020: 203c 7464 3e49 583c 2f74 643e 0d0a 2020   <td>IX</td>..  
-00004030: 2020 2020 3c74 643e 303c 2f74 643e 0d0a      <td>0</td>..
-00004040: 2020 2020 2020 3c74 643e 5031 593c 2f74        <td>P1Y</t
-00004050: 643e 0d0a 2020 2020 2020 3c74 643e 3230  d>..      <td>20
-00004060: 3030 3c2f 7464 3e0d 0a20 2020 2020 203c  00</td>..      <
-00004070: 7464 3e33 392e 3335 3130 3233 3032 3933  td>39.3510230293
-00004080: 3230 323c 2f74 643e 0d0a 2020 2020 3c2f  202</td>..    </
-00004090: 7472 3e0d 0a20 2020 203c 7472 3e0d 0a20  tr>..    <tr>.. 
-000040a0: 2020 2020 203c 7468 3e31 3c2f 7468 3e0d       <th>1</th>.
-000040b0: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
-000040c0: 3e0d 0a20 2020 2020 203c 7464 3e57 3030  >..      <td>W00
-000040d0: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-000040e0: 3e50 434f 414c 3c2f 7464 3e0d 0a20 2020  >PCOAL</td>..   
-000040f0: 2020 203c 7464 3e49 583c 2f74 643e 0d0a     <td>IX</td>..
-00004100: 2020 2020 2020 3c74 643e 303c 2f74 643e        <td>0</td>
-00004110: 0d0a 2020 2020 2020 3c74 643e 5031 593c  ..      <td>P1Y<
-00004120: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-00004130: 3230 3031 3c2f 7464 3e0d 0a20 2020 2020  2001</td>..     
-00004140: 203c 7464 3e34 392e 3333 3738 3538 3732   <td>49.33785872
-00004150: 3834 3033 393c 2f74 643e 0d0a 2020 2020  84039</td>..    
-00004160: 3c2f 7472 3e0d 0a20 2020 203c 7472 3e0d  </tr>..    <tr>.
-00004170: 0a20 2020 2020 203c 7468 3e32 3c2f 7468  .      <th>2</th
-00004180: 3e0d 0a20 2020 2020 203c 7464 3e41 3c2f  >..      <td>A</
-00004190: 7464 3e0d 0a20 2020 2020 203c 7464 3e57  td>..      <td>W
-000041a0: 3030 3c2f 7464 3e0d 0a20 2020 2020 203c  00</td>..      <
-000041b0: 7464 3e50 434f 414c 3c2f 7464 3e0d 0a20  td>PCOAL</td>.. 
-000041c0: 2020 2020 203c 7464 3e49 583c 2f74 643e       <td>IX</td>
-000041d0: 0d0a 2020 2020 2020 3c74 643e 303c 2f74  ..      <td>0</t
-000041e0: 643e 0d0a 2020 2020 2020 3c74 643e 5031  d>..      <td>P1
-000041f0: 593c 2f74 643e 0d0a 2020 2020 2020 3c74  Y</td>..      <t
-00004200: 643e 3230 3032 3c2f 7464 3e0d 0a20 2020  d>2002</td>..   
-00004210: 2020 203c 7464 3e33 392e 3439 3439 3039     <td>39.494909
-00004220: 3136 3438 3030 363c 2f74 643e 0d0a 2020  1648006</td>..  
-00004230: 2020 3c2f 7472 3e0d 0a20 2020 203c 7472    </tr>..    <tr
-00004240: 3e0d 0a20 2020 2020 203c 7468 3e33 3c2f  >..      <th>3</
-00004250: 7468 3e0d 0a20 2020 2020 203c 7464 3e41  th>..      <td>A
-00004260: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-00004270: 3e57 3030 3c2f 7464 3e0d 0a20 2020 2020  >W00</td>..     
-00004280: 203c 7464 3e50 434f 414c 3c2f 7464 3e0d   <td>PCOAL</td>.
-00004290: 0a20 2020 2020 203c 7464 3e49 583c 2f74  .      <td>IX</t
-000042a0: 643e 0d0a 2020 2020 2020 3c74 643e 303c  d>..      <td>0<
-000042b0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-000042c0: 5031 593c 2f74 643e 0d0a 2020 2020 2020  P1Y</td>..      
-000042d0: 3c74 643e 3230 3033 3c2f 7464 3e0d 0a20  <td>2003</td>.. 
-000042e0: 2020 2020 203c 7464 3e34 332e 3238 3738       <td>43.2878
-000042f0: 3837 3639 3530 3738 383c 2f74 643e 0d0a  876950788</td>..
-00004300: 2020 2020 3c2f 7472 3e0d 0a20 2020 203c      </tr>..    <
-00004310: 7472 3e0d 0a20 2020 2020 203c 7468 3e34  tr>..      <th>4
-00004320: 3c2f 7468 3e0d 0a20 2020 2020 203c 7464  </th>..      <td
-00004330: 3e41 3c2f 7464 3e0d 0a20 2020 2020 203c  >A</td>..      <
-00004340: 7464 3e57 3030 3c2f 7464 3e0d 0a20 2020  td>W00</td>..   
-00004350: 2020 203c 7464 3e50 434f 414c 3c2f 7464     <td>PCOAL</td
-00004360: 3e0d 0a20 2020 2020 203c 7464 3e49 583c  >..      <td>IX<
-00004370: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-00004380: 303c 2f74 643e 0d0a 2020 2020 2020 3c74  0</td>..      <t
-00004390: 643e 5031 593c 2f74 643e 0d0a 2020 2020  d>P1Y</td>..    
-000043a0: 2020 3c74 643e 3230 3034 3c2f 7464 3e0d    <td>2004</td>.
-000043b0: 0a20 2020 2020 203c 7464 3e38 322e 3931  .      <td>82.91
-000043c0: 3835 3835 3830 3532 3836 323c 2f74 643e  85858052862</td>
-000043d0: 0d0a 2020 2020 3c2f 7472 3e0d 0a20 203c  ..    </tr>..  <
-000043e0: 2f74 626f 6479 3e0d 0a3c 2f74 6162 6c65  /tbody>..</table
-000043f0: 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a0d 0a0d  >..</div>.......
-00004400: 0a23 2323 2057 6f72 6b69 6e67 2077 6974  .### Working wit
-00004410: 6820 7468 6520 5265 7475 726e 6564 2044  h the Returned D
-00004420: 6174 6120 4672 616d 650d 0a0d 0a4e 6f74  ata Frame....Not
-00004430: 6520 7468 6174 2061 6c6c 2063 6f6c 756d  e that all colum
-00004440: 6e73 2069 6e20 7468 6520 7265 7475 726e  ns in the return
-00004450: 6564 2064 6174 6120 6672 616d 6520 6172  ed data frame ar
-00004460: 6520 6368 6172 6163 7465 7220 7665 6374  e character vect
-00004470: 6f72 732c 2061 6e64 2074 6861 7420 746f  ors, and that to
-00004480: 2070 6c6f 7420 7468 6520 7365 7269 6573   plot the series
-00004490: 2077 6520 7769 6c6c 206e 6565 6420 746f   we will need to
-000044a0: 2063 6f6e 7665 7274 2074 6f20 7661 6c69   convert to vali
-000044b0: 6420 6e75 6d65 7269 6320 6f72 2064 6174  d numeric or dat
-000044c0: 6520 666f 726d 6174 732e 2055 7369 6e67  e formats. Using
-000044d0: 2060 7365 6162 6f72 6e60 2077 6974 6820   `seaborn` with 
-000044e0: 6068 7565 602c 2077 6520 6361 6e20 706c  `hue`, we can pl
-000044f0: 6f74 2064 6966 6665 7265 6e74 2069 6e64  ot different ind
-00004500: 6963 6174 6f72 7320 696e 2064 6966 6665  icators in diffe
-00004510: 7265 6e74 2063 6f6c 6f72 733a 0d0a 0d0a  rent colors:....
-00004520: 0d0a 6060 6070 7974 686f 6e0d 0a23 2043  ..```python..# C
-00004530: 6f6e 7665 7274 206f 6273 5f76 616c 7565  onvert obs_value
-00004540: 2074 6f20 6e75 6d65 7269 6320 616e 6420   to numeric and 
-00004550: 7469 6d65 5f70 6572 696f 6420 746f 2069  time_period to i
-00004560: 6e74 6567 6572 2079 6561 720d 0a64 6620  nteger year..df 
-00004570: 3d20 6466 2e61 7374 7970 6528 7b22 7469  = df.astype({"ti
-00004580: 6d65 5f70 6572 696f 6422 203a 2069 6e74  me_period" : int
-00004590: 2c20 226f 6273 5f76 616c 7565 2220 3a20  , "obs_value" : 
-000045a0: 666c 6f61 747d 290d 0a0d 0a23 2050 6c6f  float})....# Plo
-000045b0: 7420 7072 6963 6573 206f 6620 6469 6666  t prices of diff
-000045c0: 6572 656e 7420 636f 6d6d 6f64 6974 6965  erent commoditie
-000045d0: 7320 696e 2064 6966 6665 7265 6e74 2063  s in different c
-000045e0: 6f6c 6f72 7320 7769 7468 2073 6561 626f  olors with seabo
-000045f0: 726e 0d0a 7365 6162 6f72 6e2e 6c69 6e65  rn..seaborn.line
-00004600: 706c 6f74 2864 6174 613d 6466 2c20 783d  plot(data=df, x=
-00004610: 2774 696d 655f 7065 7269 6f64 272c 2079  'time_period', y
-00004620: 3d27 6f62 735f 7661 6c75 6527 2c20 6875  ='obs_value', hu
-00004630: 653d 2763 6f6d 6d6f 6469 7479 2729 3b0d  e='commodity');.
-00004640: 0a60 6060 0d0a 0d0a 0d0a 2020 2020 0d0a  .```......    ..
-00004650: 215b 706e 675d 2852 4541 444d 455f 6669  ![png](README_fi
-00004660: 6c65 732f 706c 6f74 2e70 6e67 290d 0a20  les/plot.png).. 
-00004670: 2020 200d 0a0d 0a0d 0a0d 0a41 6c73 6f20     ........Also 
-00004680: 6e6f 7465 2074 6861 7420 7468 6520 7265  note that the re
-00004690: 7475 726e 6564 2064 6174 6120 6672 616d  turned data fram
-000046a0: 6520 6861 7320 6d79 7374 6572 696f 7573  e has mysterious
-000046b0: 2d6c 6f6f 6b69 6e67 2063 6f64 6573 2061  -looking codes a
-000046c0: 7320 7661 6c75 6573 2069 6e20 736f 6d65  s values in some
-000046d0: 2063 6f6c 756d 6e73 2e0d 0a0d 0a43 6f64   columns.....Cod
-000046e0: 6573 2069 6e20 7468 6520 6074 696d 655f  es in the `time_
-000046f0: 666f 726d 6174 6020 636f 6c75 6d6e 2061  format` column a
-00004700: 7265 2049 534f 2038 3630 3120 6475 7261  re ISO 8601 dura
-00004710: 7469 6f6e 2063 6f64 6573 2e20 496e 2074  tion codes. In t
-00004720: 6869 7320 6361 7365 2c20 e280 9c50 3159  his case, ...P1Y
-00004730: e280 9d20 6d65 616e 7320 e280 9c70 6572  ... means ...per
-00004740: 696f 6473 206f 6620 3120 7965 6172 2ee2  iods of 1 year..
-00004750: 809d 2054 6865 2060 756e 6974 5f6d 756c  .. The `unit_mul
-00004760: 7460 2063 6f6c 756d 6e20 7265 7072 6573  t` column repres
-00004770: 656e 7473 2074 6865 206e 756d 6265 7220  ents the number 
-00004780: 6f66 207a 6572 6f65 7320 796f 7520 7368  of zeroes you sh
-00004790: 6f75 6c64 2061 6464 2074 6f20 7468 6520  ould add to the 
-000047a0: 7661 6c75 6520 636f 6c75 6d6e 2e20 466f  value column. Fo
-000047b0: 7220 696e 7374 616e 6365 2c20 6966 2076  r instance, if v
-000047c0: 616c 7565 2069 7320 696e 206d 696c 6c69  alue is in milli
-000047d0: 6f6e 732c 2074 6865 6e20 7468 6520 756e  ons, then the un
-000047e0: 6974 206d 756c 7469 706c 6965 7220 7769  it multiplier wi
-000047f0: 6c6c 2062 6520 362e 2049 6620 696e 2062  ll be 6. If in b
-00004800: 696c 6c69 6f6e 732c 2074 6865 6e20 7468  illions, then th
-00004810: 6520 756e 6974 206d 756c 7469 706c 6965  e unit multiplie
-00004820: 7220 7769 6c6c 2062 6520 392e 0d0a 0d0a  r will be 9.....
-00004830: 5468 6520 6d65 616e 696e 6773 206f 6620  The meanings of 
-00004840: 7468 6520 6f74 6865 7220 636f 6465 7320  the other codes 
-00004850: 6172 6520 7374 6f72 6564 2069 6e20 6f75  are stored in ou
-00004860: 7220 6070 6172 616d 7360 206f 626a 6563  r `params` objec
-00004870: 7420 616e 6420 6361 6e20 6265 2066 6574  t and can be fet
-00004880: 6368 6564 2077 6974 6820 6120 6a6f 696e  ched with a join
-00004890: 2e20 466f 7220 696e 7374 616e 6365 2074  . For instance t
-000048a0: 6f20 6665 7463 6820 7468 6520 6d65 616e  o fetch the mean
-000048b0: 696e 6720 6f66 2074 6865 2060 7265 665f  ing of the `ref_
-000048c0: 6172 6561 6020 636f 6465 20e2 809c 5730  area` code ...W0
-000048d0: 30e2 809d 2c20 7765 2063 616e 2070 6572  0..., we can per
-000048e0: 666f 726d 2061 206c 6566 7420 6a6f 696e  form a left join
-000048f0: 2077 6974 6820 7468 6520 6070 6172 616d   with the `param
-00004900: 735b 2772 6566 5f61 7265 6127 5d60 2064  s['ref_area']` d
-00004910: 6174 6120 6672 616d 6520 616e 6420 7573  ata frame and us
-00004920: 6520 7365 6c65 6374 2074 6f20 7265 706c  e select to repl
-00004930: 6163 6520 6072 6566 5f61 7265 6160 2077  ace `ref_area` w
-00004940: 6974 6820 7468 6520 7061 7261 6d65 7465  ith the paramete
-00004950: 7220 6465 7363 7269 7074 696f 6e3a 0d0a  r description:..
-00004960: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
-00004970: 204a 6f69 6e20 6466 2077 6974 6820 7061   Join df with pa
-00004980: 7261 6d73 5b27 7265 665f 6172 6561 275d  rams['ref_area']
-00004990: 2074 6f20 6665 7463 6820 636f 6465 2064   to fetch code d
-000049a0: 6573 6372 6970 7469 6f6e 0d0a 6466 203d  escription..df =
-000049b0: 2064 662e 6d65 7267 6528 7061 7261 6d73   df.merge(params
-000049c0: 5b27 7265 665f 6172 6561 275d 2c20 6c65  ['ref_area'], le
-000049d0: 6674 5f6f 6e3d 2772 6566 5f61 7265 6127  ft_on='ref_area'
-000049e0: 2c72 6967 6874 5f6f 6e3d 2769 6e70 7574  ,right_on='input
-000049f0: 5f63 6f64 6527 2c68 6f77 3d27 6c65 6674  _code',how='left
-00004a00: 2729 0d0a 0d0a 2320 4472 6f70 2072 6564  ')....# Drop red
-00004a10: 756e 6461 6e74 2063 6f6c 756d 6e73 2061  undant columns a
-00004a20: 6e64 2072 656e 616d 6520 6465 7363 7269  nd rename descri
-00004a30: 7074 696f 6e20 636f 6c75 6d6e 0d0a 6466  ption column..df
-00004a40: 203d 2064 662e 6472 6f70 2863 6f6c 756d   = df.drop(colum
-00004a50: 6e73 3d5b 2772 6566 5f61 7265 6127 2c27  ns=['ref_area','
-00004a60: 696e 7075 745f 636f 6465 275d 292e 7265  input_code']).re
-00004a70: 6e61 6d65 2863 6f6c 756d 6e73 3d7b 2264  name(columns={"d
-00004a80: 6573 6372 6970 7469 6f6e 223a 2272 6566  escription":"ref
-00004a90: 5f61 7265 6122 7d29 0d0a 0d0a 2320 5669  _area"})....# Vi
-00004aa0: 6577 2066 6972 7374 2066 6577 2063 6f6c  ew first few col
-00004ab0: 756d 6e73 2069 6e20 7468 6520 6d6f 6469  umns in the modi
-00004ac0: 6669 6564 2064 6174 6120 6672 616d 650d  fied data frame.
-00004ad0: 0a64 662e 6865 6164 2829 0d0a 6060 600d  .df.head()..```.
-00004ae0: 0a0d 0a0d 0a0d 0a0d 0a3c 6469 763e 0d0a  .........<div>..
-00004af0: 0d0a 3c74 6162 6c65 2062 6f72 6465 723d  ..<table border=
-00004b00: 2231 2220 636c 6173 733d 2264 6174 6166  "1" class="dataf
-00004b10: 7261 6d65 223e 0d0a 2020 3c74 6865 6164  rame">..  <thead
-00004b20: 3e0d 0a20 2020 203c 7472 2073 7479 6c65  >..    <tr style
-00004b30: 3d22 7465 7874 2d61 6c69 676e 3a20 7269  ="text-align: ri
-00004b40: 6768 743b 223e 0d0a 2020 2020 2020 3c74  ght;">..      <t
-00004b50: 683e 3c2f 7468 3e0d 0a20 2020 2020 203c  h></th>..      <
-00004b60: 7468 3e66 7265 713c 2f74 683e 0d0a 2020  th>freq</th>..  
-00004b70: 2020 2020 3c74 683e 636f 6d6d 6f64 6974      <th>commodit
-00004b80: 793c 2f74 683e 0d0a 2020 2020 2020 3c74  y</th>..      <t
-00004b90: 683e 756e 6974 5f6d 6561 7375 7265 3c2f  h>unit_measure</
-00004ba0: 7468 3e0d 0a20 2020 2020 203c 7468 3e75  th>..      <th>u
-00004bb0: 6e69 745f 6d75 6c74 3c2f 7468 3e0d 0a20  nit_mult</th>.. 
-00004bc0: 2020 2020 203c 7468 3e74 696d 655f 666f       <th>time_fo
-00004bd0: 726d 6174 3c2f 7468 3e0d 0a20 2020 2020  rmat</th>..     
-00004be0: 203c 7468 3e74 696d 655f 7065 7269 6f64   <th>time_period
-00004bf0: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
-00004c00: 3e6f 6273 5f76 616c 7565 3c2f 7468 3e0d  >obs_value</th>.
-00004c10: 0a20 2020 2020 203c 7468 3e72 6566 5f61  .      <th>ref_a
-00004c20: 7265 613c 2f74 683e 0d0a 2020 2020 3c2f  rea</th>..    </
-00004c30: 7472 3e0d 0a20 203c 2f74 6865 6164 3e0d  tr>..  </thead>.
-00004c40: 0a20 203c 7462 6f64 793e 0d0a 2020 2020  .  <tbody>..    
-00004c50: 3c74 723e 0d0a 2020 2020 2020 3c74 683e  <tr>..      <th>
-00004c60: 303c 2f74 683e 0d0a 2020 2020 2020 3c74  0</th>..      <t
-00004c70: 643e 413c 2f74 643e 0d0a 2020 2020 2020  d>A</td>..      
-00004c80: 3c74 643e 5043 4f41 4c3c 2f74 643e 0d0a  <td>PCOAL</td>..
-00004c90: 2020 2020 2020 3c74 643e 4958 3c2f 7464        <td>IX</td
-00004ca0: 3e0d 0a20 2020 2020 203c 7464 3e30 3c2f  >..      <td>0</
-00004cb0: 7464 3e0d 0a20 2020 2020 203c 7464 3e50  td>..      <td>P
-00004cc0: 3159 3c2f 7464 3e0d 0a20 2020 2020 203c  1Y</td>..      <
-00004cd0: 7464 3e32 3030 303c 2f74 643e 0d0a 2020  td>2000</td>..  
-00004ce0: 2020 2020 3c74 643e 3339 2e33 3531 3032      <td>39.35102
-00004cf0: 333c 2f74 643e 0d0a 2020 2020 2020 3c74  3</td>..      <t
-00004d00: 643e 416c 6c20 436f 756e 7472 6965 732c  d>All Countries,
-00004d10: 2065 7863 6c75 6469 6e67 2074 6865 2049   excluding the I
-00004d20: 4f3c 2f74 643e 0d0a 2020 2020 3c2f 7472  O</td>..    </tr
-00004d30: 3e0d 0a20 2020 203c 7472 3e0d 0a20 2020  >..    <tr>..   
-00004d40: 2020 203c 7468 3e31 3c2f 7468 3e0d 0a20     <th>1</th>.. 
-00004d50: 2020 2020 203c 7464 3e41 3c2f 7464 3e0d       <td>A</td>.
-00004d60: 0a20 2020 2020 203c 7464 3e50 434f 414c  .      <td>PCOAL
-00004d70: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-00004d80: 3e49 583c 2f74 643e 0d0a 2020 2020 2020  >IX</td>..      
-00004d90: 3c74 643e 303c 2f74 643e 0d0a 2020 2020  <td>0</td>..    
-00004da0: 2020 3c74 643e 5031 593c 2f74 643e 0d0a    <td>P1Y</td>..
-00004db0: 2020 2020 2020 3c74 643e 3230 3031 3c2f        <td>2001</
-00004dc0: 7464 3e0d 0a20 2020 2020 203c 7464 3e34  td>..      <td>4
-00004dd0: 392e 3333 3738 3539 3c2f 7464 3e0d 0a20  9.337859</td>.. 
-00004de0: 2020 2020 203c 7464 3e41 6c6c 2043 6f75       <td>All Cou
-00004df0: 6e74 7269 6573 2c20 6578 636c 7564 696e  ntries, excludin
-00004e00: 6720 7468 6520 494f 3c2f 7464 3e0d 0a20  g the IO</td>.. 
-00004e10: 2020 203c 2f74 723e 0d0a 2020 2020 3c74     </tr>..    <t
-00004e20: 723e 0d0a 2020 2020 2020 3c74 683e 323c  r>..      <th>2<
-00004e30: 2f74 683e 0d0a 2020 2020 2020 3c74 643e  /th>..      <td>
-00004e40: 413c 2f74 643e 0d0a 2020 2020 2020 3c74  A</td>..      <t
-00004e50: 643e 5043 4f41 4c3c 2f74 643e 0d0a 2020  d>PCOAL</td>..  
-00004e60: 2020 2020 3c74 643e 4958 3c2f 7464 3e0d      <td>IX</td>.
-00004e70: 0a20 2020 2020 203c 7464 3e30 3c2f 7464  .      <td>0</td
-00004e80: 3e0d 0a20 2020 2020 203c 7464 3e50 3159  >..      <td>P1Y
-00004e90: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
-00004ea0: 3e32 3030 323c 2f74 643e 0d0a 2020 2020  >2002</td>..    
-00004eb0: 2020 3c74 643e 3339 2e34 3934 3930 393c    <td>39.494909<
-00004ec0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-00004ed0: 416c 6c20 436f 756e 7472 6965 732c 2065  All Countries, e
-00004ee0: 7863 6c75 6469 6e67 2074 6865 2049 4f3c  xcluding the IO<
-00004ef0: 2f74 643e 0d0a 2020 2020 3c2f 7472 3e0d  /td>..    </tr>.
-00004f00: 0a20 2020 203c 7472 3e0d 0a20 2020 2020  .    <tr>..     
-00004f10: 203c 7468 3e33 3c2f 7468 3e0d 0a20 2020   <th>3</th>..   
-00004f20: 2020 203c 7464 3e41 3c2f 7464 3e0d 0a20     <td>A</td>.. 
-00004f30: 2020 2020 203c 7464 3e50 434f 414c 3c2f       <td>PCOAL</
-00004f40: 7464 3e0d 0a20 2020 2020 203c 7464 3e49  td>..      <td>I
-00004f50: 583c 2f74 643e 0d0a 2020 2020 2020 3c74  X</td>..      <t
-00004f60: 643e 303c 2f74 643e 0d0a 2020 2020 2020  d>0</td>..      
-00004f70: 3c74 643e 5031 593c 2f74 643e 0d0a 2020  <td>P1Y</td>..  
-00004f80: 2020 2020 3c74 643e 3230 3033 3c2f 7464      <td>2003</td
-00004f90: 3e0d 0a20 2020 2020 203c 7464 3e34 332e  >..      <td>43.
-00004fa0: 3238 3738 3838 3c2f 7464 3e0d 0a20 2020  287888</td>..   
-00004fb0: 2020 203c 7464 3e41 6c6c 2043 6f75 6e74     <td>All Count
-00004fc0: 7269 6573 2c20 6578 636c 7564 696e 6720  ries, excluding 
-00004fd0: 7468 6520 494f 3c2f 7464 3e0d 0a20 2020  the IO</td>..   
-00004fe0: 203c 2f74 723e 0d0a 2020 2020 3c74 723e   </tr>..    <tr>
-00004ff0: 0d0a 2020 2020 2020 3c74 683e 343c 2f74  ..      <th>4</t
-00005000: 683e 0d0a 2020 2020 2020 3c74 643e 413c  h>..      <td>A<
-00005010: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
-00005020: 5043 4f41 4c3c 2f74 643e 0d0a 2020 2020  PCOAL</td>..    
-00005030: 2020 3c74 643e 4958 3c2f 7464 3e0d 0a20    <td>IX</td>.. 
-00005040: 2020 2020 203c 7464 3e30 3c2f 7464 3e0d       <td>0</td>.
-00005050: 0a20 2020 2020 203c 7464 3e50 3159 3c2f  .      <td>P1Y</
-00005060: 7464 3e0d 0a20 2020 2020 203c 7464 3e32  td>..      <td>2
-00005070: 3030 343c 2f74 643e 0d0a 2020 2020 2020  004</td>..      
-00005080: 3c74 643e 3832 2e39 3138 3538 363c 2f74  <td>82.918586</t
-00005090: 643e 0d0a 2020 2020 2020 3c74 643e 416c  d>..      <td>Al
-000050a0: 6c20 436f 756e 7472 6965 732c 2065 7863  l Countries, exc
-000050b0: 6c75 6469 6e67 2074 6865 2049 4f3c 2f74  luding the IO</t
-000050c0: 643e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  d>..    </tr>.. 
-000050d0: 203c 2f74 626f 6479 3e0d 0a3c 2f74 6162   </tbody>..</tab
-000050e0: 6c65 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a0d  le>..</div>.....
-000050f0: 0a                                       .
+000004d0: 0d0a 0d0a 2323 2320 4665 7463 6869 6e67  ....### Fetching
+000004e0: 2061 6e20 496e 6465 7820 6f66 2044 6174   an Index of Dat
+000004f0: 6162 6173 6573 2077 6974 6820 7468 6520  abases with the 
+00000500: 6069 6d66 5f64 6174 6162 6173 6573 6020  `imf_databases` 
+00000510: 4675 6e63 7469 6f6e 0d0a 0d0a 5468 6520  Function....The 
+00000520: 6069 6d66 7060 2070 6163 6b61 6765 2069  `imfp` package i
+00000530: 6e74 726f 6475 6365 7320 666f 7572 2063  ntroduces four c
+00000540: 6f72 6520 6675 6e63 7469 6f6e 733a 2060  ore functions: `
+00000550: 696d 6670 2e69 6d66 5f64 6174 6162 6173  imfp.imf_databas
+00000560: 6573 602c 2060 696d 6670 2e69 6d66 5f70  es`, `imfp.imf_p
+00000570: 6172 616d 6574 6572 7360 2c20 6069 6d66  arameters`, `imf
+00000580: 702e 696d 665f 7061 7261 6d65 7465 725f  p.imf_parameter_
+00000590: 6465 6673 602c 2061 6e64 2060 696d 6670  defs`, and `imfp
+000005a0: 2e69 6d66 5f64 6174 6173 6574 602e 2054  .imf_dataset`. T
+000005b0: 6865 2066 756e 6374 696f 6e20 666f 7220  he function for 
+000005c0: 646f 776e 6c6f 6164 696e 6720 6461 7461  downloading data
+000005d0: 7365 7473 2069 7320 6069 6d66 702e 696d  sets is `imfp.im
+000005e0: 665f 6461 7461 7365 7460 2c20 6275 7420  f_dataset`, but 
+000005f0: 796f 7520 7769 6c6c 206e 6565 6420 7468  you will need th
+00000600: 6520 6f74 6865 7220 6675 6e63 7469 6f6e  e other function
+00000610: 7320 746f 2064 6574 6572 6d69 6e65 2077  s to determine w
+00000620: 6861 7420 6172 6775 6d65 6e74 7320 746f  hat arguments to
+00000630: 2073 7570 706c 7920 746f 2060 696d 6670   supply to `imfp
+00000640: 2e69 6d66 5f64 6174 6173 6574 602e 2046  .imf_dataset`. F
+00000650: 6f72 2069 6e73 7461 6e63 652c 2061 6c6c  or instance, all
+00000660: 2063 616c 6c73 2074 6f20 6069 6d66 702e   calls to `imfp.
+00000670: 696d 665f 6461 7461 7365 7460 2072 6571  imf_dataset` req
+00000680: 7569 7265 2061 2060 6461 7461 6261 7365  uire a `database
+00000690: 5f69 6460 2e20 5468 6973 2069 7320 6265  _id`. This is be
+000006a0: 6361 7573 6520 7468 6520 494d 4620 7365  cause the IMF se
+000006b0: 7276 6573 206d 616e 7920 6469 6666 6572  rves many differ
+000006c0: 656e 7420 6461 7461 6261 7365 7320 7468  ent databases th
+000006d0: 726f 7567 6820 6974 7320 4150 492c 2061  rough its API, a
+000006e0: 6e64 2074 6865 2041 5049 206e 6565 6473  nd the API needs
+000006f0: 2074 6f20 6b6e 6f77 2077 6869 6368 206f   to know which o
+00000700: 6620 7468 6573 6520 6d61 6e79 2064 6174  f these many dat
+00000710: 6162 6173 6573 2079 6f75 2772 6520 7265  abases you're re
+00000720: 7175 6573 7469 6e67 2064 6174 6120 6672  questing data fr
+00000730: 6f6d 2e20 546f 206f 6274 6169 6e20 6120  om. To obtain a 
+00000740: 6c69 7374 206f 6620 6461 7461 6261 7365  list of database
+00000750: 732c 2075 7365 2060 696d 6670 2e69 6d66  s, use `imfp.imf
+00000760: 5f64 6174 6162 6173 6573 602c 206c 696b  _databases`, lik
+00000770: 6520 736f 3a0d 0a0d 0a0d 0a60 6060 7079  e so:......```py
+00000780: 7468 6f6e 0d0a 2346 6574 6368 2074 6865  thon..#Fetch the
+00000790: 206c 6973 7420 6f66 2064 6174 6162 6173   list of databas
+000007a0: 6573 2061 7661 696c 6162 6c65 2074 6872  es available thr
+000007b0: 6f75 6768 2074 6865 2049 4d46 2041 5049  ough the IMF API
+000007c0: 0d0a 6461 7461 6261 7365 7320 3d20 696d  ..databases = im
+000007d0: 6670 2e69 6d66 5f64 6174 6162 6173 6573  fp.imf_databases
+000007e0: 2829 0d0a 6461 7461 6261 7365 732e 6865  ()..databases.he
+000007f0: 6164 2829 0d0a 6060 600d 0a0d 0a0d 0a0d  ad()..```.......
+00000800: 0a0d 0a3c 6469 763e 0d0a 0d0a 3c74 6162  ...<div>....<tab
+00000810: 6c65 2062 6f72 6465 723d 2231 2220 636c  le border="1" cl
+00000820: 6173 733d 2264 6174 6166 7261 6d65 223e  ass="dataframe">
+00000830: 0d0a 2020 3c74 6865 6164 3e0d 0a20 2020  ..  <thead>..   
+00000840: 203c 7472 2073 7479 6c65 3d22 7465 7874   <tr style="text
+00000850: 2d61 6c69 676e 3a20 7269 6768 743b 223e  -align: right;">
+00000860: 0d0a 2020 2020 2020 3c74 683e 3c2f 7468  ..      <th></th
+00000870: 3e0d 0a20 2020 2020 203c 7468 3e64 6174  >..      <th>dat
+00000880: 6162 6173 655f 6964 3c2f 7468 3e0d 0a20  abase_id</th>.. 
+00000890: 2020 2020 203c 7468 3e64 6573 6372 6970       <th>descrip
+000008a0: 7469 6f6e 3c2f 7468 3e0d 0a20 2020 203c  tion</th>..    <
+000008b0: 2f74 723e 0d0a 2020 3c2f 7468 6561 643e  /tr>..  </thead>
+000008c0: 0d0a 2020 3c74 626f 6479 3e0d 0a20 2020  ..  <tbody>..   
+000008d0: 203c 7472 3e0d 0a20 2020 2020 203c 7468   <tr>..      <th
+000008e0: 3e30 3c2f 7468 3e0d 0a20 2020 2020 203c  >0</th>..      <
+000008f0: 7464 3e42 4f50 5f32 3031 374d 3036 3c2f  td>BOP_2017M06</
+00000900: 7464 3e0d 0a20 2020 2020 203c 7464 3e42  td>..      <td>B
+00000910: 616c 616e 6365 206f 6620 5061 796d 656e  alance of Paymen
+00000920: 7473 2028 424f 5029 2c20 3230 3137 204d  ts (BOP), 2017 M
+00000930: 3036 3c2f 7464 3e0d 0a20 2020 203c 2f74  06</td>..    </t
+00000940: 723e 0d0a 2020 2020 3c74 723e 0d0a 2020  r>..    <tr>..  
+00000950: 2020 2020 3c74 683e 313c 2f74 683e 0d0a      <th>1</th>..
+00000960: 2020 2020 2020 3c74 643e 424f 505f 3230        <td>BOP_20
+00000970: 3230 4d33 3c2f 7464 3e0d 0a20 2020 2020  20M3</td>..     
+00000980: 203c 7464 3e42 616c 616e 6365 206f 6620   <td>Balance of 
+00000990: 5061 796d 656e 7473 2028 424f 5029 2c20  Payments (BOP), 
+000009a0: 3230 3230 204d 3033 3c2f 7464 3e0d 0a20  2020 M03</td>.. 
+000009b0: 2020 203c 2f74 723e 0d0a 2020 2020 3c74     </tr>..    <t
+000009c0: 723e 0d0a 2020 2020 2020 3c74 683e 323c  r>..      <th>2<
+000009d0: 2f74 683e 0d0a 2020 2020 2020 3c74 643e  /th>..      <td>
+000009e0: 424f 505f 3230 3137 4d31 313c 2f74 643e  BOP_2017M11</td>
+000009f0: 0d0a 2020 2020 2020 3c74 643e 4261 6c61  ..      <td>Bala
+00000a00: 6e63 6520 6f66 2050 6179 6d65 6e74 7320  nce of Payments 
+00000a10: 2842 4f50 292c 2032 3031 3720 4d31 313c  (BOP), 2017 M11<
+00000a20: 2f74 643e 0d0a 2020 2020 3c2f 7472 3e0d  /td>..    </tr>.
+00000a30: 0a20 2020 203c 7472 3e0d 0a20 2020 2020  .    <tr>..     
+00000a40: 203c 7468 3e33 3c2f 7468 3e0d 0a20 2020   <th>3</th>..   
+00000a50: 2020 203c 7464 3e44 4f54 5f32 3032 3051     <td>DOT_2020Q
+00000a60: 313c 2f74 643e 0d0a 2020 2020 2020 3c74  1</td>..      <t
+00000a70: 643e 4469 7265 6374 696f 6e20 6f66 2054  d>Direction of T
+00000a80: 7261 6465 2053 7461 7469 7374 6963 7320  rade Statistics 
+00000a90: 2844 4f54 5329 2c20 3230 3230 2051 313c  (DOTS), 2020 Q1<
+00000aa0: 2f74 643e 0d0a 2020 2020 3c2f 7472 3e0d  /td>..    </tr>.
+00000ab0: 0a20 2020 203c 7472 3e0d 0a20 2020 2020  .    <tr>..     
+00000ac0: 203c 7468 3e34 3c2f 7468 3e0d 0a20 2020   <th>4</th>..   
+00000ad0: 2020 203c 7464 3e47 4653 4d41 4232 3031     <td>GFSMAB201
+00000ae0: 363c 2f74 643e 0d0a 2020 2020 2020 3c74  6</td>..      <t
+00000af0: 643e 476f 7665 726e 6d65 6e74 2046 696e  d>Government Fin
+00000b00: 616e 6365 2053 7461 7469 7374 6963 7320  ance Statistics 
+00000b10: 5965 6172 626f 6f6b 2028 4746 5359 2032  Yearbook (GFSY 2
+00000b20: 2e2e 2e3c 2f74 643e 0d0a 2020 2020 3c2f  ...</td>..    </
+00000b30: 7472 3e0d 0a20 203c 2f74 626f 6479 3e0d  tr>..  </tbody>.
+00000b40: 0a3c 2f74 6162 6c65 3e0d 0a3c 2f64 6976  .</table>..</div
+00000b50: 3e0d 0a0d 0a0d 0a0d 0a54 6869 7320 6675  >........This fu
+00000b60: 6e63 7469 6f6e 2072 6574 7572 6e73 2074  nction returns t
+00000b70: 6865 2049 4d46 e280 9973 206c 6973 7469  he IMF...s listi
+00000b80: 6e67 206f 6620 3235 3920 6461 7461 6261  ng of 259 databa
+00000b90: 7365 7320 6176 6169 6c61 626c 6520 7468  ses available th
+00000ba0: 726f 7567 6820 7468 6520 4150 492e 2028  rough the API. (
+00000bb0: 496e 2072 6561 6c69 7479 2c20 3720 6f66  In reality, 7 of
+00000bc0: 2074 6865 206c 6973 7465 6420 6461 7461   the listed data
+00000bd0: 6261 7365 7320 6172 6520 6465 6675 6e63  bases are defunc
+00000be0: 7420 616e 6420 6e6f 7420 6163 7475 616c  t and not actual
+00000bf0: 6c79 2061 7661 696c 6162 6c65 3a20 4641  ly available: FA
+00000c00: 535f 3230 3135 2c20 4746 5330 312c 2046  S_2015, GFS01, F
+00000c10: 4d32 3032 3031 302c 2041 5044 5245 4f32  M202010, APDREO2
+00000c20: 3032 3031 302c 2041 4652 5245 4f32 3032  02010, AFRREO202
+00000c30: 3031 302c 2057 4844 5245 4f32 3032 3031  010, WHDREO20201
+00000c40: 302c 2042 4f50 4147 475f 3230 3230 2e29  0, BOPAGG_2020.)
+00000c50: 0d0a 0d0a 546f 2076 6965 7720 616e 6420  ....To view and 
+00000c60: 6578 706c 6f72 6520 7468 6520 6461 7461  explore the data
+00000c70: 6261 7365 206c 6973 742c 2069 74e2 8099  base list, it...
+00000c80: 7320 706f 7373 6962 6c65 2074 6f20 6578  s possible to ex
+00000c90: 706c 6f72 6520 7375 6273 6574 7320 6f66  plore subsets of
+00000ca0: 2074 6865 2064 6174 6120 6672 616d 6520   the data frame 
+00000cb0: 6279 2072 6f77 206e 756d 6265 7220 7769  by row number wi
+00000cc0: 7468 2060 6461 7461 6261 7365 732e 6c6f  th `databases.lo
+00000cd0: 6360 3a0d 0a0d 0a0d 0a0d 0a60 6060 7079  c`:........```py
+00000ce0: 7468 6f6e 0d0a 2320 5669 6577 2061 2073  thon..# View a s
+00000cf0: 7562 7365 7420 636f 6e73 6973 7469 6e67  ubset consisting
+00000d00: 206f 6620 726f 7773 2035 2074 6872 6f75   of rows 5 throu
+00000d10: 6768 2039 0d0a 6461 7461 6261 7365 732e  gh 9..databases.
+00000d20: 6c6f 635b 353a 395d 0d0a 6060 600d 0a0d  loc[5:9]..```...
+00000d30: 0a0d 0a0d 0a0d 0a3c 6469 763e 0d0a 0d0a  .......<div>....
+00000d40: 3c74 6162 6c65 2062 6f72 6465 723d 2231  <table border="1
+00000d50: 2220 636c 6173 733d 2264 6174 6166 7261  " class="datafra
+00000d60: 6d65 223e 0d0a 2020 3c74 6865 6164 3e0d  me">..  <thead>.
+00000d70: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
+00000d80: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+00000d90: 743b 223e 0d0a 2020 2020 2020 3c74 683e  t;">..      <th>
+00000da0: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
+00000db0: 3e64 6174 6162 6173 655f 6964 3c2f 7468  >database_id</th
+00000dc0: 3e0d 0a20 2020 2020 203c 7468 3e64 6573  >..      <th>des
+00000dd0: 6372 6970 7469 6f6e 3c2f 7468 3e0d 0a20  cription</th>.. 
+00000de0: 2020 203c 2f74 723e 0d0a 2020 3c2f 7468     </tr>..  </th
+00000df0: 6561 643e 0d0a 2020 3c74 626f 6479 3e0d  ead>..  <tbody>.
+00000e00: 0a20 2020 203c 7472 3e0d 0a20 2020 2020  .    <tr>..     
+00000e10: 203c 7468 3e35 3c2f 7468 3e0d 0a20 2020   <th>5</th>..   
+00000e20: 2020 203c 7464 3e42 4f50 5f32 3031 394d     <td>BOP_2019M
+00000e30: 3132 3c2f 7464 3e0d 0a20 2020 2020 203c  12</td>..      <
+00000e40: 7464 3e42 616c 616e 6365 206f 6620 5061  td>Balance of Pa
+00000e50: 796d 656e 7473 2028 424f 5029 2c20 3230  yments (BOP), 20
+00000e60: 3139 204d 3132 3c2f 7464 3e0d 0a20 2020  19 M12</td>..   
+00000e70: 203c 2f74 723e 0d0a 2020 2020 3c74 723e   </tr>..    <tr>
+00000e80: 0d0a 2020 2020 2020 3c74 683e 363c 2f74  ..      <th>6</t
+00000e90: 683e 0d0a 2020 2020 2020 3c74 643e 4746  h>..      <td>GF
+00000ea0: 5359 4641 4c43 5332 3031 343c 2f74 643e  SYFALCS2014</td>
+00000eb0: 0d0a 2020 2020 2020 3c74 643e 476f 7665  ..      <td>Gove
+00000ec0: 726e 6d65 6e74 2046 696e 616e 6365 2053  rnment Finance S
+00000ed0: 7461 7469 7374 6963 7320 5965 6172 626f  tatistics Yearbo
+00000ee0: 6f6b 2028 4746 5359 2032 2e2e 2e3c 2f74  ok (GFSY 2...</t
+00000ef0: 643e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  d>..    </tr>.. 
+00000f00: 2020 203c 7472 3e0d 0a20 2020 2020 203c     <tr>..      <
+00000f10: 7468 3e37 3c2f 7468 3e0d 0a20 2020 2020  th>7</th>..     
+00000f20: 203c 7464 3e47 4653 4532 3031 363c 2f74   <td>GFSE2016</t
+00000f30: 643e 0d0a 2020 2020 2020 3c74 643e 476f  d>..      <td>Go
+00000f40: 7665 726e 6d65 6e74 2046 696e 616e 6365  vernment Finance
+00000f50: 2053 7461 7469 7374 6963 7320 5965 6172   Statistics Year
+00000f60: 626f 6f6b 2028 4746 5359 2032 2e2e 2e3c  book (GFSY 2...<
+00000f70: 2f74 643e 0d0a 2020 2020 3c2f 7472 3e0d  /td>..    </tr>.
+00000f80: 0a20 2020 203c 7472 3e0d 0a20 2020 2020  .    <tr>..     
+00000f90: 203c 7468 3e38 3c2f 7468 3e0d 0a20 2020   <th>8</th>..   
+00000fa0: 2020 203c 7464 3e46 4d32 3031 3531 303c     <td>FM201510<
+00000fb0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+00000fc0: 4669 7363 616c 204d 6f6e 6974 6f72 2028  Fiscal Monitor (
+00000fd0: 464d 2920 4f63 746f 6265 7220 3230 3135  FM) October 2015
+00000fe0: 3c2f 7464 3e0d 0a20 2020 203c 2f74 723e  </td>..    </tr>
+00000ff0: 0d0a 2020 2020 3c74 723e 0d0a 2020 2020  ..    <tr>..    
+00001000: 2020 3c74 683e 393c 2f74 683e 0d0a 2020    <th>9</th>..  
+00001010: 2020 2020 3c74 643e 4746 5349 4253 3230      <td>GFSIBS20
+00001020: 3136 3c2f 7464 3e0d 0a20 2020 2020 203c  16</td>..      <
+00001030: 7464 3e47 6f76 6572 6e6d 656e 7420 4669  td>Government Fi
+00001040: 6e61 6e63 6520 5374 6174 6973 7469 6373  nance Statistics
+00001050: 2059 6561 7262 6f6f 6b20 2847 4653 5920   Yearbook (GFSY 
+00001060: 322e 2e2e 3c2f 7464 3e0d 0a20 2020 203c  2...</td>..    <
+00001070: 2f74 723e 0d0a 2020 3c2f 7462 6f64 793e  /tr>..  </tbody>
+00001080: 0d0a 3c2f 7461 626c 653e 0d0a 3c2f 6469  ..</table>..</di
+00001090: 763e 0d0a 0d0a 0d0a 0d0a 0d0a 204f 722c  v>.......... Or,
+000010a0: 2069 6620 796f 7520 616c 7265 6164 7920   if you already 
+000010b0: 6b6e 6f77 2077 6869 6368 2064 6174 6162  know which datab
+000010c0: 6173 6520 796f 7520 7761 6e74 2c20 796f  ase you want, yo
+000010d0: 7520 6361 6e20 6665 7463 6820 7468 6520  u can fetch the 
+000010e0: 636f 7272 6573 706f 6e64 696e 6720 636f  corresponding co
+000010f0: 6465 2062 7920 7365 6172 6368 696e 6720  de by searching 
+00001100: 666f 7220 6120 7374 7269 6e67 206d 6174  for a string mat
+00001110: 6368 2075 7369 6e67 2060 7374 722e 636f  ch using `str.co
+00001120: 6e74 6169 6e73 6020 616e 6420 7375 6273  ntains` and subs
+00001130: 6574 7469 6e67 2074 6865 2064 6174 6120  etting the data 
+00001140: 6672 616d 6520 666f 7220 6d61 7463 6869  frame for matchi
+00001150: 6e67 2072 6f77 732e 2046 6f72 2069 6e73  ng rows. For ins
+00001160: 7461 6e63 652c 2068 6572 65e2 8099 7320  tance, here...s 
+00001170: 686f 7720 746f 2073 6561 7263 6820 666f  how to search fo
+00001180: 7220 7468 6520 5072 696d 6172 7920 436f  r the Primary Co
+00001190: 6d6d 6f64 6974 7920 5072 6963 6520 5379  mmodity Price Sy
+000011a0: 7374 656d 3a0d 0a0d 0a0d 0a60 6060 7079  stem:......```py
+000011b0: 7468 6f6e 0d0a 6461 7461 6261 7365 735b  thon..databases[
+000011c0: 6461 7461 6261 7365 735b 2764 6573 6372  databases['descr
+000011d0: 6970 7469 6f6e 275d 2e73 7472 2e63 6f6e  iption'].str.con
+000011e0: 7461 696e 7328 2243 6f6d 6d6f 6469 7479  tains("Commodity
+000011f0: 2229 5d0d 0a60 6060 0d0a 0d0a 0d0a 0d0a  ")]..```........
+00001200: 0d0a 3c64 6976 3e0d 0a0d 0a3c 7461 626c  ..<div>....<tabl
+00001210: 6520 626f 7264 6572 3d22 3122 2063 6c61  e border="1" cla
+00001220: 7373 3d22 6461 7461 6672 616d 6522 3e0d  ss="dataframe">.
+00001230: 0a20 203c 7468 6561 643e 0d0a 2020 2020  .  <thead>..    
+00001240: 3c74 7220 7374 796c 653d 2274 6578 742d  <tr style="text-
+00001250: 616c 6967 6e3a 2072 6967 6874 3b22 3e0d  align: right;">.
+00001260: 0a20 2020 2020 203c 7468 3e3c 2f74 683e  .      <th></th>
+00001270: 0d0a 2020 2020 2020 3c74 683e 6461 7461  ..      <th>data
+00001280: 6261 7365 5f69 643c 2f74 683e 0d0a 2020  base_id</th>..  
+00001290: 2020 2020 3c74 683e 6465 7363 7269 7074      <th>descript
+000012a0: 696f 6e3c 2f74 683e 0d0a 2020 2020 3c2f  ion</th>..    </
+000012b0: 7472 3e0d 0a20 203c 2f74 6865 6164 3e0d  tr>..  </thead>.
+000012c0: 0a20 203c 7462 6f64 793e 0d0a 2020 2020  .  <tbody>..    
+000012d0: 3c74 723e 0d0a 2020 2020 2020 3c74 683e  <tr>..      <th>
+000012e0: 3233 373c 2f74 683e 0d0a 2020 2020 2020  237</th>..      
+000012f0: 3c74 643e 5043 544f 543c 2f74 643e 0d0a  <td>PCTOT</td>..
+00001300: 2020 2020 2020 3c74 643e 436f 6d6d 6f64        <td>Commod
+00001310: 6974 7920 5465 726d 7320 6f66 2054 7261  ity Terms of Tra
+00001320: 6465 3c2f 7464 3e0d 0a20 2020 203c 2f74  de</td>..    </t
+00001330: 723e 0d0a 2020 2020 3c74 723e 0d0a 2020  r>..    <tr>..  
+00001340: 2020 2020 3c74 683e 3233 393c 2f74 683e      <th>239</th>
+00001350: 0d0a 2020 2020 2020 3c74 643e 5043 5053  ..      <td>PCPS
+00001360: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00001370: 3e50 7269 6d61 7279 2043 6f6d 6d6f 6469  >Primary Commodi
+00001380: 7479 2050 7269 6365 2053 7973 7465 6d20  ty Price System 
+00001390: 2850 4350 5329 3c2f 7464 3e0d 0a20 2020  (PCPS)</td>..   
+000013a0: 203c 2f74 723e 0d0a 2020 3c2f 7462 6f64   </tr>..  </tbod
+000013b0: 793e 0d0a 3c2f 7461 626c 653e 0d0a 3c2f  y>..</table>..</
+000013c0: 6469 763e 0d0a 0d0a 0d0a 0d0a 2323 2320  div>........### 
+000013d0: 4665 7463 6869 6e67 2061 204c 6973 7420  Fetching a List 
+000013e0: 6f66 2050 6172 616d 6574 6572 7320 616e  of Parameters an
+000013f0: 6420 496e 7075 7420 436f 6465 7320 7769  d Input Codes wi
+00001400: 7468 2060 696d 665f 7061 7261 6d65 7465  th `imf_paramete
+00001410: 7273 6020 616e 6420 6069 6d66 5f70 6172  rs` and `imf_par
+00001420: 616d 6574 6572 5f64 6566 7360 0d0a 0d0a  ameter_defs`....
+00001430: 4f6e 6365 2079 6f75 2068 6176 6520 6120  Once you have a 
+00001440: 6064 6174 6162 6173 655f 6964 602c 2069  `database_id`, i
+00001450: 74e2 8099 7320 706f 7373 6962 6c65 2074  t...s possible t
+00001460: 6f20 6d61 6b65 2061 2063 616c 6c20 746f  o make a call to
+00001470: 2060 696d 6670 2e69 6d66 5f64 6174 6173   `imfp.imf_datas
+00001480: 6574 6020 746f 2066 6574 6368 2074 6865  et` to fetch the
+00001490: 2065 6e74 6972 6520 6461 7461 6261 7365   entire database
+000014a0: 3a20 6069 6d66 702e 696d 665f 6461 7461  : `imfp.imf_data
+000014b0: 7365 7428 6461 7461 6261 7365 5f69 6429  set(database_id)
+000014c0: 602e 2048 6f77 6576 6572 2c20 7768 696c  `. However, whil
+000014d0: 6520 7468 6973 2077 696c 6c20 7375 6363  e this will succ
+000014e0: 6565 6420 666f 7220 6120 6665 7720 736d  eed for a few sm
+000014f0: 616c 6c20 6461 7461 6261 7365 732c 2069  all databases, i
+00001500: 7420 7769 6c6c 2066 6169 6c20 666f 7220  t will fail for 
+00001510: 616c 6c20 6f66 2074 6865 206c 6172 6765  all of the large
+00001520: 7220 6f6e 6573 2e20 416e 6420 6576 656e  r ones. And even
+00001530: 2069 6e20 7468 6520 7261 7265 2063 6173   in the rare cas
+00001540: 6520 7768 656e 2069 7420 7375 6363 6565  e when it succee
+00001550: 6473 2c20 6665 7463 6869 6e67 2061 6e20  ds, fetching an 
+00001560: 656e 7469 7265 2064 6174 6162 6173 6520  entire database 
+00001570: 6361 6e20 7461 6b65 2061 206c 6f6e 6720  can take a long 
+00001580: 7469 6d65 2e20 596f 75e2 8099 7265 206d  time. You...re m
+00001590: 7563 6820 6265 7474 6572 206f 6666 2073  uch better off s
+000015a0: 7570 706c 7969 6e67 2061 6464 6974 696f  upplying additio
+000015b0: 6e61 6c20 6669 6c74 6572 2070 6172 616d  nal filter param
+000015c0: 6574 6572 7320 746f 2072 6564 7563 6520  eters to reduce 
+000015d0: 7468 6520 7369 7a65 206f 6620 796f 7572  the size of your
+000015e0: 2072 6571 7565 7374 2e0d 0a0d 0a52 6571   request.....Req
+000015f0: 7565 7374 7320 746f 2064 6174 6162 6173  uests to databas
+00001600: 6573 2061 7661 696c 6162 6c65 2074 6872  es available thr
+00001610: 6f75 6768 2074 6865 2049 4d46 2041 5049  ough the IMF API
+00001620: 2061 7265 2063 6f6d 706c 6963 6174 6564   are complicated
+00001630: 2062 7920 7468 6520 6661 6374 2074 6861   by the fact tha
+00001640: 7420 6561 6368 2064 6174 6162 6173 6520  t each database 
+00001650: 7573 6573 2061 2064 6966 6665 7265 6e74  uses a different
+00001660: 2073 6574 206f 6620 7061 7261 6d65 7465   set of paramete
+00001670: 7273 2077 6865 6e20 6d61 6b69 6e67 2061  rs when making a
+00001680: 2072 6571 7565 7374 2e20 2841 7420 6c61   request. (At la
+00001690: 7374 2063 6f75 6e74 2c20 7468 6572 6520  st count, there 
+000016a0: 7765 7265 2034 3320 756e 6971 7565 2070  were 43 unique p
+000016b0: 6172 616d 6574 6572 7320 7573 6564 2069  arameters used i
+000016c0: 6e20 6d61 6b69 6e67 2041 5049 2072 6571  n making API req
+000016d0: 7565 7374 7320 6672 6f6d 2074 6865 2076  uests from the v
+000016e0: 6172 696f 7573 2064 6174 6162 6173 6573  arious databases
+000016f0: 2129 2059 6f75 2061 6c73 6f20 6861 7665  !) You also have
+00001700: 2074 6f20 6861 7665 2074 6865 206c 6973   to have the lis
+00001710: 7420 6f66 2076 616c 6964 2069 6e70 7574  t of valid input
+00001720: 2063 6f64 6573 2066 6f72 2065 6163 6820   codes for each 
+00001730: 7061 7261 6d65 7465 722e 2054 6865 2060  parameter. The `
+00001740: 696d 6670 2e69 6d66 5f70 6172 616d 6574  imfp.imf_paramet
+00001750: 6572 7360 2066 756e 6374 696f 6e20 736f  ers` function so
+00001760: 6c76 6573 2074 6869 7320 7072 6f62 6c65  lves this proble
+00001770: 6d2e 2055 7365 2074 6865 2066 756e 6374  m. Use the funct
+00001780: 696f 6e20 746f 206f 6274 6169 6e20 7468  ion to obtain th
+00001790: 6520 6675 6c6c 206c 6973 7420 6f66 2070  e full list of p
+000017a0: 6172 616d 6574 6572 7320 616e 6420 7661  arameters and va
+000017b0: 6c69 6420 696e 7075 7420 636f 6465 7320  lid input codes 
+000017c0: 666f 7220 6120 6769 7665 6e20 6461 7461  for a given data
+000017d0: 6261 7365 3a0d 0a0d 0a0d 0a60 6060 7079  base:......```py
+000017e0: 7468 6f6e 0d0a 2320 4665 7463 6820 6c69  thon..# Fetch li
+000017f0: 7374 206f 6620 7661 6c69 6420 7061 7261  st of valid para
+00001800: 6d65 7465 7273 2061 6e64 2069 6e70 7574  meters and input
+00001810: 2063 6f64 6573 2066 6f72 2063 6f6d 6d6f   codes for commo
+00001820: 6469 7479 2070 7269 6365 2064 6174 6162  dity price datab
+00001830: 6173 650d 0a70 6172 616d 7320 3d20 696d  ase..params = im
+00001840: 6670 2e69 6d66 5f70 6172 616d 6574 6572  fp.imf_parameter
+00001850: 7328 2250 4350 5322 290d 0a60 6060 0d0a  s("PCPS")..```..
+00001860: 0d0a 5468 6520 6069 6d66 702e 696d 665f  ..The `imfp.imf_
+00001870: 7061 7261 6d65 7465 7273 6020 6675 6e63  parameters` func
+00001880: 7469 6f6e 2072 6574 7572 6e73 2061 2064  tion returns a d
+00001890: 6963 7469 6f6e 6172 7920 6f66 2064 6174  ictionary of dat
+000018a0: 6120 6672 616d 6573 2e20 4561 6368 2064  a frames. Each d
+000018b0: 6963 7469 6f6e 6172 7920 6b65 7920 6e61  ictionary key na
+000018c0: 6d65 2063 6f72 7265 7370 6f6e 6473 2074  me corresponds t
+000018d0: 6f20 6120 7061 7261 6d65 7465 7220 7573  o a parameter us
+000018e0: 6564 2069 6e20 6d61 6b69 6e67 2072 6571  ed in making req
+000018f0: 7565 7374 7320 6672 6f6d 2074 6865 2064  uests from the d
+00001900: 6174 6162 6173 653a 0d0a 0d0a 0d0a 6060  atabase:......``
+00001910: 6070 7974 686f 6e0d 0a23 2047 6574 206b  `python..# Get k
+00001920: 6579 206e 616d 6573 2066 726f 6d20 7468  ey names from th
+00001930: 6520 7061 7261 6d73 206f 626a 6563 740d  e params object.
+00001940: 0a70 6172 616d 732e 6b65 7973 2829 0d0a  .params.keys()..
+00001950: 6060 600d 0a0d 0a0d 0a0d 0a0d 0a20 2020  ```..........   
+00001960: 2064 6963 745f 6b65 7973 285b 2766 7265   dict_keys(['fre
+00001970: 7127 2c20 2772 6566 5f61 7265 6127 2c20  q', 'ref_area', 
+00001980: 2763 6f6d 6d6f 6469 7479 272c 2027 756e  'commodity', 'un
+00001990: 6974 5f6d 6561 7375 7265 275d 290d 0a0d  it_measure'])...
+000019a0: 0a0d 0a0d 0a49 6e20 7468 6520 6576 656e  .....In the even
+000019b0: 7420 7468 6174 2061 2070 6172 616d 6574  t that a paramet
+000019c0: 6572 206e 616d 6520 6973 206e 6f74 2073  er name is not s
+000019d0: 656c 662d 6578 706c 616e 6174 6f72 792c  elf-explanatory,
+000019e0: 2074 6865 2060 696d 6670 2e69 6d66 5f70   the `imfp.imf_p
+000019f0: 6172 616d 6574 6572 5f64 6566 7360 2066  arameter_defs` f
+00001a00: 756e 6374 696f 6e20 6361 6e20 6265 2075  unction can be u
+00001a10: 7365 6420 746f 2066 6574 6368 2073 686f  sed to fetch sho
+00001a20: 7274 2074 6578 7420 6465 7363 7269 7074  rt text descript
+00001a30: 696f 6e73 206f 6620 6561 6368 2070 6172  ions of each par
+00001a40: 616d 6574 6572 3a0d 0a0d 0a0d 0a60 6060  ameter:......```
+00001a50: 7079 7468 6f6e 0d0a 2320 4665 7463 6820  python..# Fetch 
+00001a60: 616e 6420 6469 7370 6c61 7920 7061 7261  and display para
+00001a70: 6d65 7465 7220 7465 7874 2064 6573 6372  meter text descr
+00001a80: 6970 7469 6f6e 7320 666f 7220 7468 6520  iptions for the 
+00001a90: 636f 6d6d 6f64 6974 7920 7072 6963 6520  commodity price 
+00001aa0: 6461 7461 6261 7365 0d0a 696d 6670 2e69  database..imfp.i
+00001ab0: 6d66 5f70 6172 616d 6574 6572 5f64 6566  mf_parameter_def
+00001ac0: 7328 2250 4350 5322 290d 0a60 6060 0d0a  s("PCPS")..```..
+00001ad0: 0d0a 0d0a 0d0a 0d0a 3c64 6976 3e0d 0a0d  ........<div>...
+00001ae0: 0a3c 7461 626c 6520 626f 7264 6572 3d22  .<table border="
+00001af0: 3122 2063 6c61 7373 3d22 6461 7461 6672  1" class="datafr
+00001b00: 616d 6522 3e0d 0a20 203c 7468 6561 643e  ame">..  <thead>
+00001b10: 0d0a 2020 2020 3c74 7220 7374 796c 653d  ..    <tr style=
+00001b20: 2274 6578 742d 616c 6967 6e3a 2072 6967  "text-align: rig
+00001b30: 6874 3b22 3e0d 0a20 2020 2020 203c 7468  ht;">..      <th
+00001b40: 3e3c 2f74 683e 0d0a 2020 2020 2020 3c74  ></th>..      <t
+00001b50: 683e 7061 7261 6d65 7465 723c 2f74 683e  h>parameter</th>
+00001b60: 0d0a 2020 2020 2020 3c74 683e 6465 7363  ..      <th>desc
+00001b70: 7269 7074 696f 6e3c 2f74 683e 0d0a 2020  ription</th>..  
+00001b80: 2020 3c2f 7472 3e0d 0a20 203c 2f74 6865    </tr>..  </the
+00001b90: 6164 3e0d 0a20 203c 7462 6f64 793e 0d0a  ad>..  <tbody>..
+00001ba0: 2020 2020 3c74 723e 0d0a 2020 2020 2020      <tr>..      
+00001bb0: 3c74 683e 303c 2f74 683e 0d0a 2020 2020  <th>0</th>..    
+00001bc0: 2020 3c74 643e 6672 6571 3c2f 7464 3e0d    <td>freq</td>.
+00001bd0: 0a20 2020 2020 203c 7464 3e46 7265 7175  .      <td>Frequ
+00001be0: 656e 6379 3c2f 7464 3e0d 0a20 2020 203c  ency</td>..    <
+00001bf0: 2f74 723e 0d0a 2020 2020 3c74 723e 0d0a  /tr>..    <tr>..
+00001c00: 2020 2020 2020 3c74 683e 313c 2f74 683e        <th>1</th>
+00001c10: 0d0a 2020 2020 2020 3c74 643e 7265 665f  ..      <td>ref_
+00001c20: 6172 6561 3c2f 7464 3e0d 0a20 2020 2020  area</td>..     
+00001c30: 203c 7464 3e47 656f 6772 6170 6869 6361   <td>Geographica
+00001c40: 6c20 4172 6561 733c 2f74 643e 0d0a 2020  l Areas</td>..  
+00001c50: 2020 3c2f 7472 3e0d 0a20 2020 203c 7472    </tr>..    <tr
+00001c60: 3e0d 0a20 2020 2020 203c 7468 3e32 3c2f  >..      <th>2</
+00001c70: 7468 3e0d 0a20 2020 2020 203c 7464 3e63  th>..      <td>c
+00001c80: 6f6d 6d6f 6469 7479 3c2f 7464 3e0d 0a20  ommodity</td>.. 
+00001c90: 2020 2020 203c 7464 3e49 6e64 6963 6174       <td>Indicat
+00001ca0: 6f72 3c2f 7464 3e0d 0a20 2020 203c 2f74  or</td>..    </t
+00001cb0: 723e 0d0a 2020 2020 3c74 723e 0d0a 2020  r>..    <tr>..  
+00001cc0: 2020 2020 3c74 683e 333c 2f74 683e 0d0a      <th>3</th>..
+00001cd0: 2020 2020 2020 3c74 643e 756e 6974 5f6d        <td>unit_m
+00001ce0: 6561 7375 7265 3c2f 7464 3e0d 0a20 2020  easure</td>..   
+00001cf0: 2020 203c 7464 3e55 6e69 743c 2f74 643e     <td>Unit</td>
+00001d00: 0d0a 2020 2020 3c2f 7472 3e0d 0a20 203c  ..    </tr>..  <
+00001d10: 2f74 626f 6479 3e0d 0a3c 2f74 6162 6c65  /tbody>..</table
+00001d20: 3e0d 0a3c 2f64 6976 3e0d 0a0d 0a0d 0a0d  >..</div>.......
+00001d30: 0a45 6163 6820 6e61 6d65 6420 6c69 7374  .Each named list
+00001d40: 2069 7465 6d20 6973 2061 2064 6174 6120   item is a data 
+00001d50: 6672 616d 6520 636f 6e74 6169 6e69 6e67  frame containing
+00001d60: 2061 2076 6563 746f 7220 6f66 2076 616c   a vector of val
+00001d70: 6964 2069 6e70 7574 2063 6f64 6573 2074  id input codes t
+00001d80: 6861 7420 6361 6e20 6265 2075 7365 6420  hat can be used 
+00001d90: 7769 7468 2074 6865 206e 616d 6564 2070  with the named p
+00001da0: 6172 616d 6574 6572 2c20 616e 6420 6120  arameter, and a 
+00001db0: 7665 6374 6f72 206f 6620 7465 7874 2064  vector of text d
+00001dc0: 6573 6372 6970 7469 6f6e 7320 6f66 2077  escriptions of w
+00001dd0: 6861 7420 6561 6368 2063 6f64 6520 7265  hat each code re
+00001de0: 7072 6573 656e 7473 2e0d 0a0d 0a54 6f20  presents.....To 
+00001df0: 6163 6365 7373 2074 6865 2064 6174 6120  access the data 
+00001e00: 6672 616d 6520 636f 6e74 6169 6e69 6e67  frame containing
+00001e10: 2076 616c 6964 2076 616c 7565 7320 666f   valid values fo
+00001e20: 7220 6561 6368 2070 6172 616d 6574 6572  r each parameter
+00001e30: 2c20 7375 6273 6574 2074 6865 2060 7061  , subset the `pa
+00001e40: 7261 6d73 6020 6469 6374 2062 7920 7468  rams` dict by th
+00001e50: 6520 7061 7261 6d65 7465 7220 6e61 6d65  e parameter name
+00001e60: 3a0d 0a0d 0a0d 0a60 6060 7079 7468 6f6e  :......```python
+00001e70: 0d0a 2320 5669 6577 2074 6865 2064 6174  ..# View the dat
+00001e80: 6120 6672 616d 6520 6f66 2076 616c 6964  a frame of valid
+00001e90: 2069 6e70 7574 2063 6f64 6573 2066 6f72   input codes for
+00001ea0: 2074 6865 2066 7265 7175 656e 6379 2070   the frequency p
+00001eb0: 6172 616d 6574 6572 0d0a 7061 7261 6d73  arameter..params
+00001ec0: 5b27 6672 6571 275d 0d0a 6060 600d 0a0d  ['freq']..```...
+00001ed0: 0a0d 0a0d 0a0d 0a3c 6469 763e 0d0a 0d0a  .......<div>....
+00001ee0: 3c74 6162 6c65 2062 6f72 6465 723d 2231  <table border="1
+00001ef0: 2220 636c 6173 733d 2264 6174 6166 7261  " class="datafra
+00001f00: 6d65 223e 0d0a 2020 3c74 6865 6164 3e0d  me">..  <thead>.
+00001f10: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
+00001f20: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+00001f30: 743b 223e 0d0a 2020 2020 2020 3c74 683e  t;">..      <th>
+00001f40: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
+00001f50: 3e69 6e70 7574 5f63 6f64 653c 2f74 683e  >input_code</th>
+00001f60: 0d0a 2020 2020 2020 3c74 683e 6465 7363  ..      <th>desc
+00001f70: 7269 7074 696f 6e3c 2f74 683e 0d0a 2020  ription</th>..  
+00001f80: 2020 3c2f 7472 3e0d 0a20 203c 2f74 6865    </tr>..  </the
+00001f90: 6164 3e0d 0a20 203c 7462 6f64 793e 0d0a  ad>..  <tbody>..
+00001fa0: 2020 2020 3c74 723e 0d0a 2020 2020 2020      <tr>..      
+00001fb0: 3c74 683e 303c 2f74 683e 0d0a 2020 2020  <th>0</th>..    
+00001fc0: 2020 3c74 643e 413c 2f74 643e 0d0a 2020    <td>A</td>..  
+00001fd0: 2020 2020 3c74 643e 416e 6e75 616c 3c2f      <td>Annual</
+00001fe0: 7464 3e0d 0a20 2020 203c 2f74 723e 0d0a  td>..    </tr>..
+00001ff0: 2020 2020 3c74 723e 0d0a 2020 2020 2020      <tr>..      
+00002000: 3c74 683e 313c 2f74 683e 0d0a 2020 2020  <th>1</th>..    
+00002010: 2020 3c74 643e 4d3c 2f74 643e 0d0a 2020    <td>M</td>..  
+00002020: 2020 2020 3c74 643e 4d6f 6e74 686c 793c      <td>Monthly<
+00002030: 2f74 643e 0d0a 2020 2020 3c2f 7472 3e0d  /td>..    </tr>.
+00002040: 0a20 2020 203c 7472 3e0d 0a20 2020 2020  .    <tr>..     
+00002050: 203c 7468 3e32 3c2f 7468 3e0d 0a20 2020   <th>2</th>..   
+00002060: 2020 203c 7464 3e51 3c2f 7464 3e0d 0a20     <td>Q</td>.. 
+00002070: 2020 2020 203c 7464 3e51 7561 7274 6572       <td>Quarter
+00002080: 6c79 3c2f 7464 3e0d 0a20 2020 203c 2f74  ly</td>..    </t
+00002090: 723e 0d0a 2020 3c2f 7462 6f64 793e 0d0a  r>..  </tbody>..
+000020a0: 3c2f 7461 626c 653e 0d0a 3c2f 6469 763e  </table>..</div>
+000020b0: 0d0a 0d0a 0d0a 0d0a 2323 2320 5669 6577  ........### View
+000020c0: 696e 6720 4461 7461 2046 7261 6d65 730d  ing Data Frames.
+000020d0: 0a0d 0a4e 6f74 6520 7468 6174 2060 7061  ...Note that `pa
+000020e0: 6e64 6173 6020 6461 7461 2066 7261 6d65  ndas` data frame
+000020f0: 7320 696e 2050 7974 686f 6e20 6361 6e20  s in Python can 
+00002100: 6265 2061 206c 6974 746c 6520 6469 6666  be a little diff
+00002110: 6963 756c 7420 746f 2077 6f72 6b20 7769  icult to work wi
+00002120: 7468 2c20 6265 6361 7573 6520 5079 7468  th, because Pyth
+00002130: 6f6e 2064 6f65 736e 2774 2068 6176 6520  on doesn't have 
+00002140: 6120 6275 696c 742d 696e 2076 6172 6961  a built-in varia
+00002150: 626c 6520 6578 706c 6f72 6572 2e20 4966  ble explorer. If
+00002160: 2079 6f75 2772 6520 646f 696e 6720 6461   you're doing da
+00002170: 7461 2073 6369 656e 6365 2c20 4920 7265  ta science, I re
+00002180: 636f 6d6d 656e 6420 7573 696e 6720 616e  commend using an
+00002190: 2049 4445 206c 696b 6520 5253 7475 6469   IDE like RStudi
+000021a0: 6f20 6f72 2053 7079 6465 7220 7468 6174  o or Spyder that
+000021b0: 2068 6173 2061 2062 7569 6c74 2d69 6e20   has a built-in 
+000021c0: 7661 7269 6162 6c65 2065 7870 6c6f 7265  variable explore
+000021d0: 722e 2048 6f77 6576 6572 2c20 6966 2079  r. However, if y
+000021e0: 6f75 2064 6f6e 2774 2068 6176 6520 6120  ou don't have a 
+000021f0: 7661 7269 6162 6c65 2065 7870 6c6f 7265  variable explore
+00002200: 722c 2079 6f75 2063 616e 2070 7265 7665  r, you can preve
+00002210: 6e74 2050 7974 686f 6e20 6672 6f6d 2074  nt Python from t
+00002220: 7275 6e63 6174 696e 6720 6461 7461 2066  runcating data f
+00002230: 7261 6d65 7320 7573 696e 6720 7468 6520  rames using the 
+00002240: 606f 7074 696f 6e73 6020 696e 2060 7061  `options` in `pa
+00002250: 6e64 6173 602e 2046 6f72 2069 6e73 7461  ndas`. For insta
+00002260: 6e63 652c 2074 6f20 696e 6372 6561 7365  nce, to increase
+00002270: 2074 6865 206d 6178 696d 756d 2061 6c6c   the maximum all
+00002280: 6f77 6564 2063 6f6c 756d 6e20 7769 6474  owed column widt
+00002290: 6820 746f 2031 3030 2063 6861 7261 6374  h to 100 charact
+000022a0: 6572 732c 2077 6520 6361 6e20 7573 6520  ers, we can use 
+000022b0: 6070 616e 6461 732e 6f70 7469 6f6e 732e  `pandas.options.
+000022c0: 6469 7370 6c61 792e 6d61 785f 636f 6c77  display.max_colw
+000022d0: 6964 7468 203d 2031 3030 602e 0d0a 0d0a  idth = 100`.....
+000022e0: 416c 7465 726e 6174 6976 656c 792c 2069  Alternatively, i
+000022f0: 7427 7320 706f 7373 6962 6c65 2074 6f20  t's possible to 
+00002300: 6f70 656e 2074 6865 2064 6174 6120 6672  open the data fr
+00002310: 616d 6520 696e 2061 206e 6577 2077 696e  ame in a new win
+00002320: 646f 7720 746f 2076 6965 7720 6974 2069  dow to view it i
+00002330: 6e20 6675 6c6c 3a0d 0a0d 0a0d 0a60 6060  n full:......```
+00002340: 7079 7468 6f6e 0d0a 696d 706f 7274 2069  python..import i
+00002350: 6d66 700d 0a69 6d70 6f72 7420 7465 6d70  mfp..import temp
+00002360: 6669 6c65 0d0a 696d 706f 7274 2077 6562  file..import web
+00002370: 6272 6f77 7365 720d 0a0d 0a23 2044 6566  browser....# Def
+00002380: 696e 6520 6120 7369 6d70 6c65 2066 756e  ine a simple fun
+00002390: 6374 696f 6e20 746f 2076 6965 7720 6461  ction to view da
+000023a0: 7461 2066 7261 6d65 2069 6e20 6120 6272  ta frame in a br
+000023b0: 6f77 7365 7220 7769 6e64 6f77 0d0a 6465  owser window..de
+000023c0: 6620 5669 6577 2864 6629 3a0d 0a20 2020  f View(df):..   
+000023d0: 2068 746d 6c20 3d20 6466 2e74 6f5f 6874   html = df.to_ht
+000023e0: 6d6c 2829 0d0a 2020 2020 7769 7468 2074  ml()..    with t
+000023f0: 656d 7066 696c 652e 4e61 6d65 6454 656d  empfile.NamedTem
+00002400: 706f 7261 7279 4669 6c65 2827 7727 2c20  poraryFile('w', 
+00002410: 6465 6c65 7465 3d46 616c 7365 2c20 7375  delete=False, su
+00002420: 6666 6978 3d27 2e68 746d 6c27 2920 6173  ffix='.html') as
+00002430: 2066 3a0d 0a20 2020 2020 2020 2075 726c   f:..        url
+00002440: 203d 2027 6669 6c65 3a2f 2f27 202b 2066   = 'file://' + f
+00002450: 2e6e 616d 650d 0a20 2020 2020 2020 2066  .name..        f
+00002460: 2e77 7269 7465 2868 746d 6c29 0d0a 2020  .write(html)..  
+00002470: 2020 7765 6262 726f 7773 6572 2e6f 7065    webbrowser.ope
+00002480: 6e28 7572 6c29 0d0a 0d0a 2320 4f70 656e  n(url)....# Open
+00002490: 2064 6174 6120 6672 616d 6520 696e 2061   data frame in a
+000024a0: 206e 6577 2062 726f 7773 6572 2077 696e   new browser win
+000024b0: 646f 7720 7573 696e 6720 7468 6520 6675  dow using the fu
+000024c0: 6e63 7469 6f6e 0d0a 6466 203d 2069 6d66  nction..df = imf
+000024d0: 702e 696d 665f 6461 7461 6261 7365 7328  p.imf_databases(
+000024e0: 290d 0a56 6965 7728 6466 290d 0a60 6060  )..View(df)..```
+000024f0: 0d0a 0d0a 2323 2320 5375 7070 6c79 696e  ....### Supplyin
+00002500: 6720 5061 7261 6d65 7465 7220 4172 6775  g Parameter Argu
+00002510: 6d65 6e74 7320 746f 2060 696d 665f 6461  ments to `imf_da
+00002520: 7461 7365 7460 3a20 4120 5461 6c65 206f  taset`: A Tale o
+00002530: 6620 5477 6f20 576f 726b 666c 6f77 730d  f Two Workflows.
+00002540: 0a0d 0a54 6865 7265 2061 7265 2074 776f  ...There are two
+00002550: 2077 6179 7320 746f 2073 7570 706c 7920   ways to supply 
+00002560: 7061 7261 6d65 7465 7273 2074 6f20 6069  parameters to `i
+00002570: 6d66 702e 696d 665f 6461 7461 7365 7460  mfp.imf_dataset`
+00002580: 3a20 6279 2073 7570 706c 7969 6e67 206c  : by supplying l
+00002590: 6973 7420 6172 6775 6d65 6e74 7320 6f72  ist arguments or
+000025a0: 2062 7920 7375 7070 6c79 696e 6720 6120   by supplying a 
+000025b0: 6d6f 6469 6669 6564 2070 6172 616d 6574  modified paramet
+000025c0: 6572 7320 6469 6374 2e20 5468 6520 6c69  ers dict. The li
+000025d0: 7374 2061 7267 756d 656e 7473 2077 6f72  st arguments wor
+000025e0: 6b66 6c6f 7720 7769 6c6c 2062 6520 6d6f  kflow will be mo
+000025f0: 7265 2069 6e74 7569 7469 7665 2066 6f72  re intuitive for
+00002600: 206d 6f73 7420 7573 6572 732c 2062 7574   most users, but
+00002610: 2074 6865 2064 6963 7420 6172 6775 6d65   the dict argume
+00002620: 6e74 2077 6f72 6b66 6c6f 7720 7265 7175  nt workflow requ
+00002630: 6972 6573 2061 206c 6974 746c 6520 6c65  ires a little le
+00002640: 7373 2063 6f64 652e 0d0a 0d0a 2323 2323  ss code.....####
+00002650: 2054 6865 204c 6973 7420 4172 6775 6d65   The List Argume
+00002660: 6e74 7320 576f 726b 666c 6f77 0d0a 0d0a  nts Workflow....
+00002670: 546f 2073 7570 706c 7920 6c69 7374 2061  To supply list a
+00002680: 7267 756d 656e 7473 2c20 6a75 7374 2066  rguments, just f
+00002690: 696e 6420 7468 6520 636f 6465 7320 796f  ind the codes yo
+000026a0: 7520 7761 6e74 2061 6e64 2073 7570 706c  u want and suppl
+000026b0: 7920 7468 656d 2074 6f20 6069 6d66 702e  y them to `imfp.
+000026c0: 696d 665f 6461 7461 7365 7460 2075 7369  imf_dataset` usi
+000026d0: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
+000026e0: 206e 616d 6520 6173 2074 6865 2061 7267   name as the arg
+000026f0: 756d 656e 7420 6e61 6d65 2e20 5468 6520  ument name. The 
+00002700: 6578 616d 706c 6520 6265 6c6f 7720 7368  example below sh
+00002710: 6f77 7320 686f 7720 746f 2072 6571 7565  ows how to reque
+00002720: 7374 2032 3030 30e2 8093 3230 3135 2061  st 2000...2015 a
+00002730: 6e6e 7561 6c20 636f 616c 2070 7269 6365  nnual coal price
+00002740: 7320 6672 6f6d 2074 6865 2050 7269 6d61  s from the Prima
+00002750: 7279 2043 6f6d 6d6f 6469 7479 2050 7269  ry Commodity Pri
+00002760: 6365 2053 7973 7465 6d20 6461 7461 6261  ce System databa
+00002770: 7365 3a0d 0a0d 0a0d 0a60 6060 7079 7468  se:......```pyth
+00002780: 6f6e 0d0a 2320 4665 7463 6820 7468 6520  on..# Fetch the 
+00002790: 2766 7265 7127 2069 6e70 7574 2063 6f64  'freq' input cod
+000027a0: 6520 666f 7220 616e 6e75 616c 2066 7265  e for annual fre
+000027b0: 7175 656e 6379 0d0a 7365 6c65 6374 6564  quency..selected
+000027c0: 5f66 7265 7120 3d20 6c69 7374 280d 0a20  _freq = list(.. 
+000027d0: 2020 2070 6172 616d 735b 2766 7265 7127     params['freq'
+000027e0: 5d5b 2769 6e70 7574 5f63 6f64 6527 5d5b  ]['input_code'][
+000027f0: 7061 7261 6d73 5b27 6672 6571 275d 5b27  params['freq']['
+00002800: 6465 7363 7269 7074 696f 6e27 5d2e 7374  description'].st
+00002810: 722e 636f 6e74 6169 6e73 2822 416e 6e75  r.contains("Annu
+00002820: 616c 2229 5d0d 0a29 0d0a 0d0a 2320 4665  al")]..)....# Fe
+00002830: 7463 6820 7468 6520 2763 6f6d 6d6f 6469  tch the 'commodi
+00002840: 7479 2720 696e 7075 7420 636f 6465 2066  ty' input code f
+00002850: 6f72 2063 6f61 6c0d 0a73 656c 6563 7465  or coal..selecte
+00002860: 645f 636f 6d6d 6f64 6974 7920 3d20 6c69  d_commodity = li
+00002870: 7374 280d 0a20 2020 2070 6172 616d 735b  st(..    params[
+00002880: 2763 6f6d 6d6f 6469 7479 275d 5b27 696e  'commodity']['in
+00002890: 7075 745f 636f 6465 275d 5b70 6172 616d  put_code'][param
+000028a0: 735b 2763 6f6d 6d6f 6469 7479 275d 5b27  s['commodity']['
+000028b0: 6465 7363 7269 7074 696f 6e27 5d2e 7374  description'].st
+000028c0: 722e 636f 6e74 6169 6e73 2822 436f 616c  r.contains("Coal
+000028d0: 2229 5d0d 0a29 0d0a 0d0a 2320 4665 7463  ")]..)....# Fetc
+000028e0: 6820 7468 6520 2775 6e69 745f 6d65 6173  h the 'unit_meas
+000028f0: 7572 6527 2069 6e70 7574 2063 6f64 6520  ure' input code 
+00002900: 666f 7220 696e 6465 780d 0a73 656c 6563  for index..selec
+00002910: 7465 645f 756e 6974 5f6d 6561 7375 7265  ted_unit_measure
+00002920: 203d 206c 6973 7428 0d0a 2020 2020 7061   = list(..    pa
+00002930: 7261 6d73 5b27 756e 6974 5f6d 6561 7375  rams['unit_measu
+00002940: 7265 275d 5b27 696e 7075 745f 636f 6465  re']['input_code
+00002950: 275d 5b70 6172 616d 735b 2775 6e69 745f  '][params['unit_
+00002960: 6d65 6173 7572 6527 5d5b 2764 6573 6372  measure']['descr
+00002970: 6970 7469 6f6e 275d 2e73 7472 2e63 6f6e  iption'].str.con
+00002980: 7461 696e 7328 2249 6e64 6578 2229 5d0d  tains("Index")].
+00002990: 0a29 0d0a 0d0a 2320 5265 7175 6573 7420  .)....# Request 
+000029a0: 6461 7461 2066 726f 6d20 7468 6520 4150  data from the AP
+000029b0: 490d 0a64 6620 3d20 696d 6670 2e69 6d66  I..df = imfp.imf
+000029c0: 5f64 6174 6173 6574 2864 6174 6162 6173  _dataset(databas
+000029d0: 655f 6964 203d 2022 5043 5053 222c 0d0a  e_id = "PCPS",..
+000029e0: 2020 2020 2020 2020 2066 7265 7120 3d20           freq = 
+000029f0: 7365 6c65 6374 6564 5f66 7265 712c 2063  selected_freq, c
+00002a00: 6f6d 6d6f 6469 7479 203d 2073 656c 6563  ommodity = selec
+00002a10: 7465 645f 636f 6d6d 6f64 6974 792c 0d0a  ted_commodity,..
+00002a20: 2020 2020 2020 2020 2075 6e69 745f 6d65           unit_me
+00002a30: 6173 7572 6520 3d20 7365 6c65 6374 6564  asure = selected
+00002a40: 5f75 6e69 745f 6d65 6173 7572 652c 0d0a  _unit_measure,..
+00002a50: 2020 2020 2020 2020 2073 7461 7274 5f79           start_y
+00002a60: 6561 7220 3d20 3230 3030 2c20 656e 645f  ear = 2000, end_
+00002a70: 7965 6172 203d 2032 3031 3529 0d0a 0d0a  year = 2015)....
+00002a80: 2320 4469 7370 6c61 7920 7468 6520 6669  # Display the fi
+00002a90: 7273 7420 6665 7720 656e 7472 6965 7320  rst few entries 
+00002aa0: 696e 2074 6865 2072 6574 7269 6576 6564  in the retrieved
+00002ab0: 2064 6174 6120 6672 616d 650d 0a64 662e   data frame..df.
+00002ac0: 6865 6164 2829 0d0a 6060 600d 0a0d 0a0d  head()..```.....
+00002ad0: 0a0d 0a0d 0a3c 6469 763e 0d0a 0d0a 3c74  .....<div>....<t
+00002ae0: 6162 6c65 2062 6f72 6465 723d 2231 2220  able border="1" 
+00002af0: 636c 6173 733d 2264 6174 6166 7261 6d65  class="dataframe
+00002b00: 223e 0d0a 2020 3c74 6865 6164 3e0d 0a20  ">..  <thead>.. 
+00002b10: 2020 203c 7472 2073 7479 6c65 3d22 7465     <tr style="te
+00002b20: 7874 2d61 6c69 676e 3a20 7269 6768 743b  xt-align: right;
+00002b30: 223e 0d0a 2020 2020 2020 3c74 683e 3c2f  ">..      <th></
+00002b40: 7468 3e0d 0a20 2020 2020 203c 7468 3e66  th>..      <th>f
+00002b50: 7265 713c 2f74 683e 0d0a 2020 2020 2020  req</th>..      
+00002b60: 3c74 683e 7265 665f 6172 6561 3c2f 7468  <th>ref_area</th
+00002b70: 3e0d 0a20 2020 2020 203c 7468 3e63 6f6d  >..      <th>com
+00002b80: 6d6f 6469 7479 3c2f 7468 3e0d 0a20 2020  modity</th>..   
+00002b90: 2020 203c 7468 3e75 6e69 745f 6d65 6173     <th>unit_meas
+00002ba0: 7572 653c 2f74 683e 0d0a 2020 2020 2020  ure</th>..      
+00002bb0: 3c74 683e 756e 6974 5f6d 756c 743c 2f74  <th>unit_mult</t
+00002bc0: 683e 0d0a 2020 2020 2020 3c74 683e 7469  h>..      <th>ti
+00002bd0: 6d65 5f66 6f72 6d61 743c 2f74 683e 0d0a  me_format</th>..
+00002be0: 2020 2020 2020 3c74 683e 7469 6d65 5f70        <th>time_p
+00002bf0: 6572 696f 643c 2f74 683e 0d0a 2020 2020  eriod</th>..    
+00002c00: 2020 3c74 683e 6f62 735f 7661 6c75 653c    <th>obs_value<
+00002c10: 2f74 683e 0d0a 2020 2020 3c2f 7472 3e0d  /th>..    </tr>.
+00002c20: 0a20 203c 2f74 6865 6164 3e0d 0a20 203c  .  </thead>..  <
+00002c30: 7462 6f64 793e 0d0a 2020 2020 3c74 723e  tbody>..    <tr>
+00002c40: 0d0a 2020 2020 2020 3c74 683e 303c 2f74  ..      <th>0</t
+00002c50: 683e 0d0a 2020 2020 2020 3c74 643e 413c  h>..      <td>A<
+00002c60: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+00002c70: 5730 303c 2f74 643e 0d0a 2020 2020 2020  W00</td>..      
+00002c80: 3c74 643e 5043 4f41 4c3c 2f74 643e 0d0a  <td>PCOAL</td>..
+00002c90: 2020 2020 2020 3c74 643e 4958 3c2f 7464        <td>IX</td
+00002ca0: 3e0d 0a20 2020 2020 203c 7464 3e30 3c2f  >..      <td>0</
+00002cb0: 7464 3e0d 0a20 2020 2020 203c 7464 3e50  td>..      <td>P
+00002cc0: 3159 3c2f 7464 3e0d 0a20 2020 2020 203c  1Y</td>..      <
+00002cd0: 7464 3e32 3030 303c 2f74 643e 0d0a 2020  td>2000</td>..  
+00002ce0: 2020 2020 3c74 643e 3339 2e33 3531 3032      <td>39.35102
+00002cf0: 3330 3239 3332 3032 3c2f 7464 3e0d 0a20  30293202</td>.. 
+00002d00: 2020 203c 2f74 723e 0d0a 2020 2020 3c74     </tr>..    <t
+00002d10: 723e 0d0a 2020 2020 2020 3c74 683e 313c  r>..      <th>1<
+00002d20: 2f74 683e 0d0a 2020 2020 2020 3c74 643e  /th>..      <td>
+00002d30: 413c 2f74 643e 0d0a 2020 2020 2020 3c74  A</td>..      <t
+00002d40: 643e 5730 303c 2f74 643e 0d0a 2020 2020  d>W00</td>..    
+00002d50: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
+00002d60: 0d0a 2020 2020 2020 3c74 643e 4958 3c2f  ..      <td>IX</
+00002d70: 7464 3e0d 0a20 2020 2020 203c 7464 3e30  td>..      <td>0
+00002d80: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00002d90: 3e50 3159 3c2f 7464 3e0d 0a20 2020 2020  >P1Y</td>..     
+00002da0: 203c 7464 3e32 3030 313c 2f74 643e 0d0a   <td>2001</td>..
+00002db0: 2020 2020 2020 3c74 643e 3439 2e33 3337        <td>49.337
+00002dc0: 3835 3837 3238 3430 3339 3c2f 7464 3e0d  8587284039</td>.
+00002dd0: 0a20 2020 203c 2f74 723e 0d0a 2020 2020  .    </tr>..    
+00002de0: 3c74 723e 0d0a 2020 2020 2020 3c74 683e  <tr>..      <th>
+00002df0: 323c 2f74 683e 0d0a 2020 2020 2020 3c74  2</th>..      <t
+00002e00: 643e 413c 2f74 643e 0d0a 2020 2020 2020  d>A</td>..      
+00002e10: 3c74 643e 5730 303c 2f74 643e 0d0a 2020  <td>W00</td>..  
+00002e20: 2020 2020 3c74 643e 5043 4f41 4c3c 2f74      <td>PCOAL</t
+00002e30: 643e 0d0a 2020 2020 2020 3c74 643e 4958  d>..      <td>IX
+00002e40: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00002e50: 3e30 3c2f 7464 3e0d 0a20 2020 2020 203c  >0</td>..      <
+00002e60: 7464 3e50 3159 3c2f 7464 3e0d 0a20 2020  td>P1Y</td>..   
+00002e70: 2020 203c 7464 3e32 3030 323c 2f74 643e     <td>2002</td>
+00002e80: 0d0a 2020 2020 2020 3c74 643e 3339 2e34  ..      <td>39.4
+00002e90: 3934 3930 3931 3634 3830 3036 3c2f 7464  949091648006</td
+00002ea0: 3e0d 0a20 2020 203c 2f74 723e 0d0a 2020  >..    </tr>..  
+00002eb0: 2020 3c74 723e 0d0a 2020 2020 2020 3c74    <tr>..      <t
+00002ec0: 683e 333c 2f74 683e 0d0a 2020 2020 2020  h>3</th>..      
+00002ed0: 3c74 643e 413c 2f74 643e 0d0a 2020 2020  <td>A</td>..    
+00002ee0: 2020 3c74 643e 5730 303c 2f74 643e 0d0a    <td>W00</td>..
+00002ef0: 2020 2020 2020 3c74 643e 5043 4f41 4c3c        <td>PCOAL<
+00002f00: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+00002f10: 4958 3c2f 7464 3e0d 0a20 2020 2020 203c  IX</td>..      <
+00002f20: 7464 3e30 3c2f 7464 3e0d 0a20 2020 2020  td>0</td>..     
+00002f30: 203c 7464 3e50 3159 3c2f 7464 3e0d 0a20   <td>P1Y</td>.. 
+00002f40: 2020 2020 203c 7464 3e32 3030 333c 2f74       <td>2003</t
+00002f50: 643e 0d0a 2020 2020 2020 3c74 643e 3433  d>..      <td>43
+00002f60: 2e32 3837 3838 3736 3935 3037 3838 3c2f  .2878876950788</
+00002f70: 7464 3e0d 0a20 2020 203c 2f74 723e 0d0a  td>..    </tr>..
+00002f80: 2020 2020 3c74 723e 0d0a 2020 2020 2020      <tr>..      
+00002f90: 3c74 683e 343c 2f74 683e 0d0a 2020 2020  <th>4</th>..    
+00002fa0: 2020 3c74 643e 413c 2f74 643e 0d0a 2020    <td>A</td>..  
+00002fb0: 2020 2020 3c74 643e 5730 303c 2f74 643e      <td>W00</td>
+00002fc0: 0d0a 2020 2020 2020 3c74 643e 5043 4f41  ..      <td>PCOA
+00002fd0: 4c3c 2f74 643e 0d0a 2020 2020 2020 3c74  L</td>..      <t
+00002fe0: 643e 4958 3c2f 7464 3e0d 0a20 2020 2020  d>IX</td>..     
+00002ff0: 203c 7464 3e30 3c2f 7464 3e0d 0a20 2020   <td>0</td>..   
+00003000: 2020 203c 7464 3e50 3159 3c2f 7464 3e0d     <td>P1Y</td>.
+00003010: 0a20 2020 2020 203c 7464 3e32 3030 343c  .      <td>2004<
+00003020: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+00003030: 3832 2e39 3138 3538 3538 3035 3238 3632  82.9185858052862
+00003040: 3c2f 7464 3e0d 0a20 2020 203c 2f74 723e  </td>..    </tr>
+00003050: 0d0a 2020 3c2f 7462 6f64 793e 0d0a 3c2f  ..  </tbody>..</
+00003060: 7461 626c 653e 0d0a 3c2f 6469 763e 0d0a  table>..</div>..
+00003070: 0d0a 0d0a 0d0a 2323 2323 2054 6865 2050  ......#### The P
+00003080: 6172 616d 6574 6572 7320 4172 6775 6d65  arameters Argume
+00003090: 6e74 2057 6f72 6b66 6c6f 770d 0a0d 0a54  nt Workflow....T
+000030a0: 6f20 7375 7070 6c79 2061 206c 6973 7420  o supply a list 
+000030b0: 6f62 6a65 6374 2c20 6d6f 6469 6679 2065  object, modify e
+000030c0: 6163 6820 6461 7461 2066 7261 6d65 2069  ach data frame i
+000030d0: 6e20 7468 6520 6070 6172 616d 7360 206c  n the `params` l
+000030e0: 6973 7420 6f62 6a65 6374 2074 6f20 7265  ist object to re
+000030f0: 7461 696e 206f 6e6c 7920 7468 6520 726f  tain only the ro
+00003100: 7773 2079 6f75 2077 616e 742c 2061 6e64  ws you want, and
+00003110: 2074 6865 6e20 7375 7070 6c79 2074 6865   then supply the
+00003120: 206d 6f64 6966 6965 6420 6c69 7374 206f   modified list o
+00003130: 626a 6563 7420 746f 2060 696d 6670 2e69  bject to `imfp.i
+00003140: 6d66 5f64 6174 6173 6574 6020 6173 2069  mf_dataset` as i
+00003150: 7473 2070 6172 616d 6574 6572 7320 6172  ts parameters ar
+00003160: 6775 6d65 6e74 2e20 4865 7265 2069 7320  gument. Here is 
+00003170: 686f 7720 746f 206d 616b 6520 7468 6520  how to make the 
+00003180: 7361 6d65 2072 6571 7565 7374 2066 6f72  same request for
+00003190: 2061 6e6e 7561 6c20 636f 616c 2070 7269   annual coal pri
+000031a0: 6365 2064 6174 6120 7573 696e 6720 6120  ce data using a 
+000031b0: 7061 7261 6d65 7465 7273 206c 6973 743a  parameters list:
+000031c0: 0d0a 0d0a 0d0a 6060 6070 7974 686f 6e0d  ......```python.
+000031d0: 0a23 2046 6574 6368 2074 6865 2027 6672  .# Fetch the 'fr
+000031e0: 6571 2720 696e 7075 7420 636f 6465 2066  eq' input code f
+000031f0: 6f72 2061 6e6e 7561 6c20 6672 6571 7565  or annual freque
+00003200: 6e63 790d 0a70 6172 616d 735b 2766 7265  ncy..params['fre
+00003210: 7127 5d20 3d20 7061 7261 6d73 5b27 6672  q'] = params['fr
+00003220: 6571 275d 5b70 6172 616d 735b 2766 7265  eq'][params['fre
+00003230: 7127 5d5b 2764 6573 6372 6970 7469 6f6e  q']['description
+00003240: 275d 2e73 7472 2e63 6f6e 7461 696e 7328  '].str.contains(
+00003250: 2241 6e6e 7561 6c22 295d 0d0a 0d0a 2320  "Annual")]....# 
+00003260: 4665 7463 6820 7468 6520 2763 6f6d 6d6f  Fetch the 'commo
+00003270: 6469 7479 2720 696e 7075 7420 636f 6465  dity' input code
+00003280: 2873 2920 666f 7220 636f 616c 0d0a 7061  (s) for coal..pa
+00003290: 7261 6d73 5b27 636f 6d6d 6f64 6974 7927  rams['commodity'
+000032a0: 5d20 3d20 7061 7261 6d73 5b27 636f 6d6d  ] = params['comm
+000032b0: 6f64 6974 7927 5d5b 7061 7261 6d73 5b27  odity'][params['
+000032c0: 636f 6d6d 6f64 6974 7927 5d5b 2764 6573  commodity']['des
+000032d0: 6372 6970 7469 6f6e 275d 2e73 7472 2e63  cription'].str.c
+000032e0: 6f6e 7461 696e 7328 2243 6f61 6c22 295d  ontains("Coal")]
+000032f0: 0d0a 0d0a 2320 4665 7463 6820 7468 6520  ....# Fetch the 
+00003300: 2775 6e69 745f 6d65 6173 7572 6527 2069  'unit_measure' i
+00003310: 6e70 7574 2063 6f64 6520 666f 7220 696e  nput code for in
+00003320: 6465 780d 0a70 6172 616d 735b 2775 6e69  dex..params['uni
+00003330: 745f 6d65 6173 7572 6527 5d20 3d20 7061  t_measure'] = pa
+00003340: 7261 6d73 5b27 756e 6974 5f6d 6561 7375  rams['unit_measu
+00003350: 7265 275d 5b70 6172 616d 735b 2775 6e69  re'][params['uni
+00003360: 745f 6d65 6173 7572 6527 5d5b 2764 6573  t_measure']['des
+00003370: 6372 6970 7469 6f6e 275d 2e73 7472 2e63  cription'].str.c
+00003380: 6f6e 7461 696e 7328 2249 6e64 6578 2229  ontains("Index")
+00003390: 5d0d 0a0d 0a23 2052 6571 7565 7374 2064  ]....# Request d
+000033a0: 6174 6120 6672 6f6d 2074 6865 2041 5049  ata from the API
+000033b0: 0d0a 6466 203d 2069 6d66 702e 696d 665f  ..df = imfp.imf_
+000033c0: 6461 7461 7365 7428 6461 7461 6261 7365  dataset(database
+000033d0: 5f69 6420 3d20 2250 4350 5322 2c0d 0a20  _id = "PCPS",.. 
+000033e0: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
+000033f0: 7273 203d 2070 6172 616d 732c 0d0a 2020  rs = params,..  
+00003400: 2020 2020 2020 2073 7461 7274 5f79 6561         start_yea
+00003410: 7220 3d20 3230 3030 2c20 656e 645f 7965  r = 2000, end_ye
+00003420: 6172 203d 2032 3031 3529 0d0a 0d0a 2320  ar = 2015)....# 
+00003430: 4469 7370 6c61 7920 7468 6520 6669 7273  Display the firs
+00003440: 7420 6665 7720 656e 7472 6965 7320 696e  t few entries in
+00003450: 2074 6865 2072 6574 7269 6576 6564 2064   the retrieved d
+00003460: 6174 6120 6672 616d 650d 0a64 662e 6865  ata frame..df.he
+00003470: 6164 2829 0d0a 6060 600d 0a0d 0a0d 0a0d  ad()..```.......
+00003480: 0a0d 0a3c 6469 763e 0d0a 0d0a 3c74 6162  ...<div>....<tab
+00003490: 6c65 2062 6f72 6465 723d 2231 2220 636c  le border="1" cl
+000034a0: 6173 733d 2264 6174 6166 7261 6d65 223e  ass="dataframe">
+000034b0: 0d0a 2020 3c74 6865 6164 3e0d 0a20 2020  ..  <thead>..   
+000034c0: 203c 7472 2073 7479 6c65 3d22 7465 7874   <tr style="text
+000034d0: 2d61 6c69 676e 3a20 7269 6768 743b 223e  -align: right;">
+000034e0: 0d0a 2020 2020 2020 3c74 683e 3c2f 7468  ..      <th></th
+000034f0: 3e0d 0a20 2020 2020 203c 7468 3e66 7265  >..      <th>fre
+00003500: 713c 2f74 683e 0d0a 2020 2020 2020 3c74  q</th>..      <t
+00003510: 683e 7265 665f 6172 6561 3c2f 7468 3e0d  h>ref_area</th>.
+00003520: 0a20 2020 2020 203c 7468 3e63 6f6d 6d6f  .      <th>commo
+00003530: 6469 7479 3c2f 7468 3e0d 0a20 2020 2020  dity</th>..     
+00003540: 203c 7468 3e75 6e69 745f 6d65 6173 7572   <th>unit_measur
+00003550: 653c 2f74 683e 0d0a 2020 2020 2020 3c74  e</th>..      <t
+00003560: 683e 756e 6974 5f6d 756c 743c 2f74 683e  h>unit_mult</th>
+00003570: 0d0a 2020 2020 2020 3c74 683e 7469 6d65  ..      <th>time
+00003580: 5f66 6f72 6d61 743c 2f74 683e 0d0a 2020  _format</th>..  
+00003590: 2020 2020 3c74 683e 7469 6d65 5f70 6572      <th>time_per
+000035a0: 696f 643c 2f74 683e 0d0a 2020 2020 2020  iod</th>..      
+000035b0: 3c74 683e 6f62 735f 7661 6c75 653c 2f74  <th>obs_value</t
+000035c0: 683e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  h>..    </tr>.. 
+000035d0: 203c 2f74 6865 6164 3e0d 0a20 203c 7462   </thead>..  <tb
+000035e0: 6f64 793e 0d0a 2020 2020 3c74 723e 0d0a  ody>..    <tr>..
+000035f0: 2020 2020 2020 3c74 683e 303c 2f74 683e        <th>0</th>
+00003600: 0d0a 2020 2020 2020 3c74 643e 413c 2f74  ..      <td>A</t
+00003610: 643e 0d0a 2020 2020 2020 3c74 643e 5730  d>..      <td>W0
+00003620: 303c 2f74 643e 0d0a 2020 2020 2020 3c74  0</td>..      <t
+00003630: 643e 5043 4f41 4c3c 2f74 643e 0d0a 2020  d>PCOAL</td>..  
+00003640: 2020 2020 3c74 643e 4958 3c2f 7464 3e0d      <td>IX</td>.
+00003650: 0a20 2020 2020 203c 7464 3e30 3c2f 7464  .      <td>0</td
+00003660: 3e0d 0a20 2020 2020 203c 7464 3e50 3159  >..      <td>P1Y
+00003670: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00003680: 3e32 3030 303c 2f74 643e 0d0a 2020 2020  >2000</td>..    
+00003690: 2020 3c74 643e 3339 2e33 3531 3032 3330    <td>39.3510230
+000036a0: 3239 3332 3032 3c2f 7464 3e0d 0a20 2020  293202</td>..   
+000036b0: 203c 2f74 723e 0d0a 2020 2020 3c74 723e   </tr>..    <tr>
+000036c0: 0d0a 2020 2020 2020 3c74 683e 313c 2f74  ..      <th>1</t
+000036d0: 683e 0d0a 2020 2020 2020 3c74 643e 413c  h>..      <td>A<
+000036e0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+000036f0: 5730 303c 2f74 643e 0d0a 2020 2020 2020  W00</td>..      
+00003700: 3c74 643e 5043 4f41 4c3c 2f74 643e 0d0a  <td>PCOAL</td>..
+00003710: 2020 2020 2020 3c74 643e 4958 3c2f 7464        <td>IX</td
+00003720: 3e0d 0a20 2020 2020 203c 7464 3e30 3c2f  >..      <td>0</
+00003730: 7464 3e0d 0a20 2020 2020 203c 7464 3e50  td>..      <td>P
+00003740: 3159 3c2f 7464 3e0d 0a20 2020 2020 203c  1Y</td>..      <
+00003750: 7464 3e32 3030 313c 2f74 643e 0d0a 2020  td>2001</td>..  
+00003760: 2020 2020 3c74 643e 3439 2e33 3337 3835      <td>49.33785
+00003770: 3837 3238 3430 3339 3c2f 7464 3e0d 0a20  87284039</td>.. 
+00003780: 2020 203c 2f74 723e 0d0a 2020 2020 3c74     </tr>..    <t
+00003790: 723e 0d0a 2020 2020 2020 3c74 683e 323c  r>..      <th>2<
+000037a0: 2f74 683e 0d0a 2020 2020 2020 3c74 643e  /th>..      <td>
+000037b0: 413c 2f74 643e 0d0a 2020 2020 2020 3c74  A</td>..      <t
+000037c0: 643e 5730 303c 2f74 643e 0d0a 2020 2020  d>W00</td>..    
+000037d0: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
+000037e0: 0d0a 2020 2020 2020 3c74 643e 4958 3c2f  ..      <td>IX</
+000037f0: 7464 3e0d 0a20 2020 2020 203c 7464 3e30  td>..      <td>0
+00003800: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00003810: 3e50 3159 3c2f 7464 3e0d 0a20 2020 2020  >P1Y</td>..     
+00003820: 203c 7464 3e32 3030 323c 2f74 643e 0d0a   <td>2002</td>..
+00003830: 2020 2020 2020 3c74 643e 3339 2e34 3934        <td>39.494
+00003840: 3930 3931 3634 3830 3036 3c2f 7464 3e0d  9091648006</td>.
+00003850: 0a20 2020 203c 2f74 723e 0d0a 2020 2020  .    </tr>..    
+00003860: 3c74 723e 0d0a 2020 2020 2020 3c74 683e  <tr>..      <th>
+00003870: 333c 2f74 683e 0d0a 2020 2020 2020 3c74  3</th>..      <t
+00003880: 643e 413c 2f74 643e 0d0a 2020 2020 2020  d>A</td>..      
+00003890: 3c74 643e 5730 303c 2f74 643e 0d0a 2020  <td>W00</td>..  
+000038a0: 2020 2020 3c74 643e 5043 4f41 4c3c 2f74      <td>PCOAL</t
+000038b0: 643e 0d0a 2020 2020 2020 3c74 643e 4958  d>..      <td>IX
+000038c0: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+000038d0: 3e30 3c2f 7464 3e0d 0a20 2020 2020 203c  >0</td>..      <
+000038e0: 7464 3e50 3159 3c2f 7464 3e0d 0a20 2020  td>P1Y</td>..   
+000038f0: 2020 203c 7464 3e32 3030 333c 2f74 643e     <td>2003</td>
+00003900: 0d0a 2020 2020 2020 3c74 643e 3433 2e32  ..      <td>43.2
+00003910: 3837 3838 3736 3935 3037 3838 3c2f 7464  878876950788</td
+00003920: 3e0d 0a20 2020 203c 2f74 723e 0d0a 2020  >..    </tr>..  
+00003930: 2020 3c74 723e 0d0a 2020 2020 2020 3c74    <tr>..      <t
+00003940: 683e 343c 2f74 683e 0d0a 2020 2020 2020  h>4</th>..      
+00003950: 3c74 643e 413c 2f74 643e 0d0a 2020 2020  <td>A</td>..    
+00003960: 2020 3c74 643e 5730 303c 2f74 643e 0d0a    <td>W00</td>..
+00003970: 2020 2020 2020 3c74 643e 5043 4f41 4c3c        <td>PCOAL<
+00003980: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+00003990: 4958 3c2f 7464 3e0d 0a20 2020 2020 203c  IX</td>..      <
+000039a0: 7464 3e30 3c2f 7464 3e0d 0a20 2020 2020  td>0</td>..     
+000039b0: 203c 7464 3e50 3159 3c2f 7464 3e0d 0a20   <td>P1Y</td>.. 
+000039c0: 2020 2020 203c 7464 3e32 3030 343c 2f74       <td>2004</t
+000039d0: 643e 0d0a 2020 2020 2020 3c74 643e 3832  d>..      <td>82
+000039e0: 2e39 3138 3538 3538 3035 3238 3632 3c2f  .9185858052862</
+000039f0: 7464 3e0d 0a20 2020 203c 2f74 723e 0d0a  td>..    </tr>..
+00003a00: 2020 3c2f 7462 6f64 793e 0d0a 3c2f 7461    </tbody>..</ta
+00003a10: 626c 653e 0d0a 3c2f 6469 763e 0d0a 0d0a  ble>..</div>....
+00003a20: 0d0a 0d0a 2323 2057 6f72 6b69 6e67 2077  ....## Working w
+00003a30: 6974 6820 7468 6520 5265 7475 726e 6564  ith the Returned
+00003a40: 2044 6174 6120 4672 616d 650d 0a0d 0a4e   Data Frame....N
+00003a50: 6f74 6520 7468 6174 2061 6c6c 2063 6f6c  ote that all col
+00003a60: 756d 6e73 2069 6e20 7468 6520 7265 7475  umns in the retu
+00003a70: 726e 6564 2064 6174 6120 6672 616d 6520  rned data frame 
+00003a80: 6172 6520 6368 6172 6163 7465 7220 7665  are character ve
+00003a90: 6374 6f72 732c 2061 6e64 2074 6861 7420  ctors, and that 
+00003aa0: 746f 2070 6c6f 7420 7468 6520 7365 7269  to plot the seri
+00003ab0: 6573 2077 6520 7769 6c6c 206e 6565 6420  es we will need 
+00003ac0: 746f 2063 6f6e 7665 7274 2074 6f20 7661  to convert to va
+00003ad0: 6c69 6420 6e75 6d65 7269 6320 6f72 2064  lid numeric or d
+00003ae0: 6174 6520 666f 726d 6174 732e 2055 7369  ate formats. Usi
+00003af0: 6e67 2060 7365 6162 6f72 6e60 2077 6974  ng `seaborn` wit
+00003b00: 6820 6068 7565 602c 2077 6520 6361 6e20  h `hue`, we can 
+00003b10: 706c 6f74 2064 6966 6665 7265 6e74 2069  plot different i
+00003b20: 6e64 6963 6174 6f72 7320 696e 2064 6966  ndicators in dif
+00003b30: 6665 7265 6e74 2063 6f6c 6f72 733a 0d0a  ferent colors:..
+00003b40: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a23  ....```python..#
+00003b50: 2043 6f6e 7665 7274 206f 6273 5f76 616c   Convert obs_val
+00003b60: 7565 2074 6f20 6e75 6d65 7269 6320 616e  ue to numeric an
+00003b70: 6420 7469 6d65 5f70 6572 696f 6420 746f  d time_period to
+00003b80: 2069 6e74 6567 6572 2079 6561 720d 0a64   integer year..d
+00003b90: 6620 3d20 6466 2e61 7374 7970 6528 7b22  f = df.astype({"
+00003ba0: 7469 6d65 5f70 6572 696f 6422 203a 2069  time_period" : i
+00003bb0: 6e74 2c20 226f 6273 5f76 616c 7565 2220  nt, "obs_value" 
+00003bc0: 3a20 666c 6f61 747d 290d 0a0d 0a23 2050  : float})....# P
+00003bd0: 6c6f 7420 7072 6963 6573 206f 6620 6469  lot prices of di
+00003be0: 6666 6572 656e 7420 636f 6d6d 6f64 6974  fferent commodit
+00003bf0: 6965 7320 696e 2064 6966 6665 7265 6e74  ies in different
+00003c00: 2063 6f6c 6f72 7320 7769 7468 2073 6561   colors with sea
+00003c10: 626f 726e 0d0a 7365 6162 6f72 6e2e 6c69  born..seaborn.li
+00003c20: 6e65 706c 6f74 2864 6174 613d 6466 2c20  neplot(data=df, 
+00003c30: 783d 2774 696d 655f 7065 7269 6f64 272c  x='time_period',
+00003c40: 2079 3d27 6f62 735f 7661 6c75 6527 2c20   y='obs_value', 
+00003c50: 6875 653d 2763 6f6d 6d6f 6469 7479 2729  hue='commodity')
+00003c60: 3b0d 0a60 6060 0d0a 0d0a 0d0a 2020 2020  ;..```......    
+00003c70: 0d0a 215b 706e 675d 2852 4541 444d 455f  ..![png](README_
+00003c80: 6669 6c65 732f 706c 6f74 2e70 6e67 290d  files/plot.png).
+00003c90: 0a20 2020 200d 0a0d 0a0d 0a0d 0a41 6c73  .    ........Als
+00003ca0: 6f20 6e6f 7465 2074 6861 7420 7468 6520  o note that the 
+00003cb0: 7265 7475 726e 6564 2064 6174 6120 6672  returned data fr
+00003cc0: 616d 6520 6861 7320 6d79 7374 6572 696f  ame has mysterio
+00003cd0: 7573 2d6c 6f6f 6b69 6e67 2063 6f64 6573  us-looking codes
+00003ce0: 2061 7320 7661 6c75 6573 2069 6e20 736f   as values in so
+00003cf0: 6d65 2063 6f6c 756d 6e73 2e0d 0a0d 0a43  me columns.....C
+00003d00: 6f64 6573 2069 6e20 7468 6520 6074 696d  odes in the `tim
+00003d10: 655f 666f 726d 6174 6020 636f 6c75 6d6e  e_format` column
+00003d20: 2061 7265 2049 534f 2038 3630 3120 6475   are ISO 8601 du
+00003d30: 7261 7469 6f6e 2063 6f64 6573 2e20 496e  ration codes. In
+00003d40: 2074 6869 7320 6361 7365 2c20 e280 9c50   this case, ...P
+00003d50: 3159 e280 9d20 6d65 616e 7320 e280 9c70  1Y... means ...p
+00003d60: 6572 696f 6473 206f 6620 3120 7965 6172  eriods of 1 year
+00003d70: 2ee2 809d 2054 6865 2060 756e 6974 5f6d  .... The `unit_m
+00003d80: 756c 7460 2063 6f6c 756d 6e20 7265 7072  ult` column repr
+00003d90: 6573 656e 7473 2074 6865 206e 756d 6265  esents the numbe
+00003da0: 7220 6f66 207a 6572 6f65 7320 796f 7520  r of zeroes you 
+00003db0: 7368 6f75 6c64 2061 6464 2074 6f20 7468  should add to th
+00003dc0: 6520 7661 6c75 6520 636f 6c75 6d6e 2e20  e value column. 
+00003dd0: 466f 7220 696e 7374 616e 6365 2c20 6966  For instance, if
+00003de0: 2076 616c 7565 2069 7320 696e 206d 696c   value is in mil
+00003df0: 6c69 6f6e 732c 2074 6865 6e20 7468 6520  lions, then the 
+00003e00: 756e 6974 206d 756c 7469 706c 6965 7220  unit multiplier 
+00003e10: 7769 6c6c 2062 6520 362e 2049 6620 696e  will be 6. If in
+00003e20: 2062 696c 6c69 6f6e 732c 2074 6865 6e20   billions, then 
+00003e30: 7468 6520 756e 6974 206d 756c 7469 706c  the unit multipl
+00003e40: 6965 7220 7769 6c6c 2062 6520 392e 0d0a  ier will be 9...
+00003e50: 0d0a 5468 6520 6d65 616e 696e 6773 206f  ..The meanings o
+00003e60: 6620 7468 6520 6f74 6865 7220 636f 6465  f the other code
+00003e70: 7320 6172 6520 7374 6f72 6564 2069 6e20  s are stored in 
+00003e80: 6f75 7220 6070 6172 616d 7360 206f 626a  our `params` obj
+00003e90: 6563 7420 616e 6420 6361 6e20 6265 2066  ect and can be f
+00003ea0: 6574 6368 6564 2077 6974 6820 6120 6a6f  etched with a jo
+00003eb0: 696e 2e20 466f 7220 696e 7374 616e 6365  in. For instance
+00003ec0: 2074 6f20 6665 7463 6820 7468 6520 6d65   to fetch the me
+00003ed0: 616e 696e 6720 6f66 2074 6865 2060 7265  aning of the `re
+00003ee0: 665f 6172 6561 6020 636f 6465 20e2 809c  f_area` code ...
+00003ef0: 5730 30e2 809d 2c20 7765 2063 616e 2070  W00..., we can p
+00003f00: 6572 666f 726d 2061 206c 6566 7420 6a6f  erform a left jo
+00003f10: 696e 2077 6974 6820 7468 6520 6070 6172  in with the `par
+00003f20: 616d 735b 2772 6566 5f61 7265 6127 5d60  ams['ref_area']`
+00003f30: 2064 6174 6120 6672 616d 6520 616e 6420   data frame and 
+00003f40: 7573 6520 7365 6c65 6374 2074 6f20 7265  use select to re
+00003f50: 706c 6163 6520 6072 6566 5f61 7265 6160  place `ref_area`
+00003f60: 2077 6974 6820 7468 6520 7061 7261 6d65   with the parame
+00003f70: 7465 7220 6465 7363 7269 7074 696f 6e3a  ter description:
+00003f80: 0d0a 0d0a 0d0a 6060 6070 7974 686f 6e0d  ......```python.
+00003f90: 0a23 204a 6f69 6e20 6466 2077 6974 6820  .# Join df with 
+00003fa0: 7061 7261 6d73 5b27 7265 665f 6172 6561  params['ref_area
+00003fb0: 275d 2074 6f20 6665 7463 6820 636f 6465  '] to fetch code
+00003fc0: 2064 6573 6372 6970 7469 6f6e 0d0a 6466   description..df
+00003fd0: 203d 2064 662e 6d65 7267 6528 7061 7261   = df.merge(para
+00003fe0: 6d73 5b27 7265 665f 6172 6561 275d 2c20  ms['ref_area'], 
+00003ff0: 6c65 6674 5f6f 6e3d 2772 6566 5f61 7265  left_on='ref_are
+00004000: 6127 2c72 6967 6874 5f6f 6e3d 2769 6e70  a',right_on='inp
+00004010: 7574 5f63 6f64 6527 2c68 6f77 3d27 6c65  ut_code',how='le
+00004020: 6674 2729 0d0a 0d0a 2320 4472 6f70 2072  ft')....# Drop r
+00004030: 6564 756e 6461 6e74 2063 6f6c 756d 6e73  edundant columns
+00004040: 2061 6e64 2072 656e 616d 6520 6465 7363   and rename desc
+00004050: 7269 7074 696f 6e20 636f 6c75 6d6e 0d0a  ription column..
+00004060: 6466 203d 2064 662e 6472 6f70 2863 6f6c  df = df.drop(col
+00004070: 756d 6e73 3d5b 2772 6566 5f61 7265 6127  umns=['ref_area'
+00004080: 2c27 696e 7075 745f 636f 6465 275d 292e  ,'input_code']).
+00004090: 7265 6e61 6d65 2863 6f6c 756d 6e73 3d7b  rename(columns={
+000040a0: 2264 6573 6372 6970 7469 6f6e 223a 2272  "description":"r
+000040b0: 6566 5f61 7265 6122 7d29 0d0a 0d0a 2320  ef_area"})....# 
+000040c0: 5669 6577 2066 6972 7374 2066 6577 2063  View first few c
+000040d0: 6f6c 756d 6e73 2069 6e20 7468 6520 6d6f  olumns in the mo
+000040e0: 6469 6669 6564 2064 6174 6120 6672 616d  dified data fram
+000040f0: 650d 0a64 662e 6865 6164 2829 0d0a 6060  e..df.head()..``
+00004100: 600d 0a0d 0a0d 0a0d 0a0d 0a3c 6469 763e  `..........<div>
+00004110: 0d0a 0d0a 3c74 6162 6c65 2062 6f72 6465  ....<table borde
+00004120: 723d 2231 2220 636c 6173 733d 2264 6174  r="1" class="dat
+00004130: 6166 7261 6d65 223e 0d0a 2020 3c74 6865  aframe">..  <the
+00004140: 6164 3e0d 0a20 2020 203c 7472 2073 7479  ad>..    <tr sty
+00004150: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00004160: 7269 6768 743b 223e 0d0a 2020 2020 2020  right;">..      
+00004170: 3c74 683e 3c2f 7468 3e0d 0a20 2020 2020  <th></th>..     
+00004180: 203c 7468 3e66 7265 713c 2f74 683e 0d0a   <th>freq</th>..
+00004190: 2020 2020 2020 3c74 683e 636f 6d6d 6f64        <th>commod
+000041a0: 6974 793c 2f74 683e 0d0a 2020 2020 2020  ity</th>..      
+000041b0: 3c74 683e 756e 6974 5f6d 6561 7375 7265  <th>unit_measure
+000041c0: 3c2f 7468 3e0d 0a20 2020 2020 203c 7468  </th>..      <th
+000041d0: 3e75 6e69 745f 6d75 6c74 3c2f 7468 3e0d  >unit_mult</th>.
+000041e0: 0a20 2020 2020 203c 7468 3e74 696d 655f  .      <th>time_
+000041f0: 666f 726d 6174 3c2f 7468 3e0d 0a20 2020  format</th>..   
+00004200: 2020 203c 7468 3e74 696d 655f 7065 7269     <th>time_peri
+00004210: 6f64 3c2f 7468 3e0d 0a20 2020 2020 203c  od</th>..      <
+00004220: 7468 3e6f 6273 5f76 616c 7565 3c2f 7468  th>obs_value</th
+00004230: 3e0d 0a20 2020 2020 203c 7468 3e72 6566  >..      <th>ref
+00004240: 5f61 7265 613c 2f74 683e 0d0a 2020 2020  _area</th>..    
+00004250: 3c2f 7472 3e0d 0a20 203c 2f74 6865 6164  </tr>..  </thead
+00004260: 3e0d 0a20 203c 7462 6f64 793e 0d0a 2020  >..  <tbody>..  
+00004270: 2020 3c74 723e 0d0a 2020 2020 2020 3c74    <tr>..      <t
+00004280: 683e 303c 2f74 683e 0d0a 2020 2020 2020  h>0</th>..      
+00004290: 3c74 643e 413c 2f74 643e 0d0a 2020 2020  <td>A</td>..    
+000042a0: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
+000042b0: 0d0a 2020 2020 2020 3c74 643e 4958 3c2f  ..      <td>IX</
+000042c0: 7464 3e0d 0a20 2020 2020 203c 7464 3e30  td>..      <td>0
+000042d0: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+000042e0: 3e50 3159 3c2f 7464 3e0d 0a20 2020 2020  >P1Y</td>..     
+000042f0: 203c 7464 3e32 3030 303c 2f74 643e 0d0a   <td>2000</td>..
+00004300: 2020 2020 2020 3c74 643e 3339 2e33 3531        <td>39.351
+00004310: 3032 333c 2f74 643e 0d0a 2020 2020 2020  023</td>..      
+00004320: 3c74 643e 416c 6c20 436f 756e 7472 6965  <td>All Countrie
+00004330: 732c 2065 7863 6c75 6469 6e67 2074 6865  s, excluding the
+00004340: 2049 4f3c 2f74 643e 0d0a 2020 2020 3c2f   IO</td>..    </
+00004350: 7472 3e0d 0a20 2020 203c 7472 3e0d 0a20  tr>..    <tr>.. 
+00004360: 2020 2020 203c 7468 3e31 3c2f 7468 3e0d       <th>1</th>.
+00004370: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
+00004380: 3e0d 0a20 2020 2020 203c 7464 3e50 434f  >..      <td>PCO
+00004390: 414c 3c2f 7464 3e0d 0a20 2020 2020 203c  AL</td>..      <
+000043a0: 7464 3e49 583c 2f74 643e 0d0a 2020 2020  td>IX</td>..    
+000043b0: 2020 3c74 643e 303c 2f74 643e 0d0a 2020    <td>0</td>..  
+000043c0: 2020 2020 3c74 643e 5031 593c 2f74 643e      <td>P1Y</td>
+000043d0: 0d0a 2020 2020 2020 3c74 643e 3230 3031  ..      <td>2001
+000043e0: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+000043f0: 3e34 392e 3333 3738 3539 3c2f 7464 3e0d  >49.337859</td>.
+00004400: 0a20 2020 2020 203c 7464 3e41 6c6c 2043  .      <td>All C
+00004410: 6f75 6e74 7269 6573 2c20 6578 636c 7564  ountries, exclud
+00004420: 696e 6720 7468 6520 494f 3c2f 7464 3e0d  ing the IO</td>.
+00004430: 0a20 2020 203c 2f74 723e 0d0a 2020 2020  .    </tr>..    
+00004440: 3c74 723e 0d0a 2020 2020 2020 3c74 683e  <tr>..      <th>
+00004450: 323c 2f74 683e 0d0a 2020 2020 2020 3c74  2</th>..      <t
+00004460: 643e 413c 2f74 643e 0d0a 2020 2020 2020  d>A</td>..      
+00004470: 3c74 643e 5043 4f41 4c3c 2f74 643e 0d0a  <td>PCOAL</td>..
+00004480: 2020 2020 2020 3c74 643e 4958 3c2f 7464        <td>IX</td
+00004490: 3e0d 0a20 2020 2020 203c 7464 3e30 3c2f  >..      <td>0</
+000044a0: 7464 3e0d 0a20 2020 2020 203c 7464 3e50  td>..      <td>P
+000044b0: 3159 3c2f 7464 3e0d 0a20 2020 2020 203c  1Y</td>..      <
+000044c0: 7464 3e32 3030 323c 2f74 643e 0d0a 2020  td>2002</td>..  
+000044d0: 2020 2020 3c74 643e 3339 2e34 3934 3930      <td>39.49490
+000044e0: 393c 2f74 643e 0d0a 2020 2020 2020 3c74  9</td>..      <t
+000044f0: 643e 416c 6c20 436f 756e 7472 6965 732c  d>All Countries,
+00004500: 2065 7863 6c75 6469 6e67 2074 6865 2049   excluding the I
+00004510: 4f3c 2f74 643e 0d0a 2020 2020 3c2f 7472  O</td>..    </tr
+00004520: 3e0d 0a20 2020 203c 7472 3e0d 0a20 2020  >..    <tr>..   
+00004530: 2020 203c 7468 3e33 3c2f 7468 3e0d 0a20     <th>3</th>.. 
+00004540: 2020 2020 203c 7464 3e41 3c2f 7464 3e0d       <td>A</td>.
+00004550: 0a20 2020 2020 203c 7464 3e50 434f 414c  .      <td>PCOAL
+00004560: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00004570: 3e49 583c 2f74 643e 0d0a 2020 2020 2020  >IX</td>..      
+00004580: 3c74 643e 303c 2f74 643e 0d0a 2020 2020  <td>0</td>..    
+00004590: 2020 3c74 643e 5031 593c 2f74 643e 0d0a    <td>P1Y</td>..
+000045a0: 2020 2020 2020 3c74 643e 3230 3033 3c2f        <td>2003</
+000045b0: 7464 3e0d 0a20 2020 2020 203c 7464 3e34  td>..      <td>4
+000045c0: 332e 3238 3738 3838 3c2f 7464 3e0d 0a20  3.287888</td>.. 
+000045d0: 2020 2020 203c 7464 3e41 6c6c 2043 6f75       <td>All Cou
+000045e0: 6e74 7269 6573 2c20 6578 636c 7564 696e  ntries, excludin
+000045f0: 6720 7468 6520 494f 3c2f 7464 3e0d 0a20  g the IO</td>.. 
+00004600: 2020 203c 2f74 723e 0d0a 2020 2020 3c74     </tr>..    <t
+00004610: 723e 0d0a 2020 2020 2020 3c74 683e 343c  r>..      <th>4<
+00004620: 2f74 683e 0d0a 2020 2020 2020 3c74 643e  /th>..      <td>
+00004630: 413c 2f74 643e 0d0a 2020 2020 2020 3c74  A</td>..      <t
+00004640: 643e 5043 4f41 4c3c 2f74 643e 0d0a 2020  d>PCOAL</td>..  
+00004650: 2020 2020 3c74 643e 4958 3c2f 7464 3e0d      <td>IX</td>.
+00004660: 0a20 2020 2020 203c 7464 3e30 3c2f 7464  .      <td>0</td
+00004670: 3e0d 0a20 2020 2020 203c 7464 3e50 3159  >..      <td>P1Y
+00004680: 3c2f 7464 3e0d 0a20 2020 2020 203c 7464  </td>..      <td
+00004690: 3e32 3030 343c 2f74 643e 0d0a 2020 2020  >2004</td>..    
+000046a0: 2020 3c74 643e 3832 2e39 3138 3538 363c    <td>82.918586<
+000046b0: 2f74 643e 0d0a 2020 2020 2020 3c74 643e  /td>..      <td>
+000046c0: 416c 6c20 436f 756e 7472 6965 732c 2065  All Countries, e
+000046d0: 7863 6c75 6469 6e67 2074 6865 2049 4f3c  xcluding the IO<
+000046e0: 2f74 643e 0d0a 2020 2020 3c2f 7472 3e0d  /td>..    </tr>.
+000046f0: 0a20 203c 2f74 626f 6479 3e0d 0a3c 2f74  .  </tbody>..</t
+00004700: 6162 6c65 3e0d 0a3c 2f64 6976 3e0d 0a0d  able>..</div>...
+00004710: 0a0d 0a0d 0a23 2320 5261 7465 2061 6e64  .....## Rate and
+00004720: 2042 616e 6477 6964 7468 204c 696d 6974   Bandwidth Limit
+00004730: 204d 616e 6167 656d 656e 740d 0a0d 0a23   Management....#
+00004740: 2323 2053 6574 7469 6e67 2061 2055 6e69  ## Setting a Uni
+00004750: 7175 6520 4170 706c 6963 6174 696f 6e20  que Application 
+00004760: 4e61 6d65 2077 6974 6820 6073 6574 5f69  Name with `set_i
+00004770: 6d66 5f61 7070 5f6e 616d 6560 0d0a 0d0a  mf_app_name`....
+00004780: 6069 6d66 702e 7365 745f 696d 665f 6170  `imfp.set_imf_ap
+00004790: 705f 6e61 6d65 2829 6020 616c 6c6f 7773  p_name()` allows
+000047a0: 2075 7365 7273 2074 6f20 7365 7420 6120   users to set a 
+000047b0: 6375 7374 6f6d 2061 7070 6c69 6361 7469  custom applicati
+000047c0: 6f6e 206e 616d 6520 746f 2062 6520 7573  on name to be us
+000047d0: 6564 2077 6865 6e20 6d61 6b69 6e67 2041  ed when making A
+000047e0: 5049 2063 616c 6c73 2074 6f20 7468 6520  PI calls to the 
+000047f0: 494d 4620 4150 492e 2054 6865 2049 4d46  IMF API. The IMF
+00004800: 2041 5049 2068 6173 2061 6e20 6170 706c   API has an appl
+00004810: 6963 6174 696f 6e2d 6261 7365 6420 7261  ication-based ra
+00004820: 7465 206c 696d 6974 206f 6620 3530 2072  te limit of 50 r
+00004830: 6571 7565 7374 7320 7065 7220 7365 636f  equests per seco
+00004840: 6e64 2c20 7769 7468 2074 6865 2061 7070  nd, with the app
+00004850: 6c69 6361 7469 6f6e 2069 6465 6e74 6966  lication identif
+00004860: 6965 6420 6279 2074 6865 2022 7573 6572  ied by the "user
+00004870: 5f61 6765 6e74 2220 7661 7269 6162 6c65  _agent" variable
+00004880: 2069 6e20 7468 6520 7265 7175 6573 7420   in the request 
+00004890: 6865 6164 6572 2e0d 0a0d 0a54 6869 7320  header.....This 
+000048a0: 636f 756c 6420 7072 6f76 6520 7072 6f62  could prove prob
+000048b0: 6c65 6d61 7469 6320 6966 2074 6865 2060  lematic if the `
+000048c0: 696d 6670 6020 6c69 6272 6172 7920 6265  imfp` library be
+000048d0: 6361 6d65 2074 6f6f 2070 6f70 756c 6172  came too popular
+000048e0: 2061 6e64 2074 6f6f 206d 616e 7920 7573   and too many us
+000048f0: 6572 7320 7472 6965 6420 746f 206d 616b  ers tried to mak
+00004900: 6520 7369 6d75 6c74 616e 656f 7573 2041  e simultaneous A
+00004910: 5049 2072 6571 7565 7374 7320 7573 696e  PI requests usin
+00004920: 6720 7468 6520 6465 6661 756c 7420 6170  g the default ap
+00004930: 7020 6e61 6d65 2e20 4279 2073 6574 7469  p name. By setti
+00004940: 6e67 2061 2063 7573 746f 6d20 6170 706c  ng a custom appl
+00004950: 6963 6174 696f 6e20 6e61 6d65 2c20 7573  ication name, us
+00004960: 6572 7320 6361 6e20 6176 6f69 6420 6869  ers can avoid hi
+00004970: 7474 696e 6720 7261 7465 206c 696d 6974  tting rate limit
+00004980: 7320 616e 6420 6265 696e 6720 626c 6f63  s and being bloc
+00004990: 6b65 6420 6279 2074 6865 2041 5049 2e20  ked by the API. 
+000049a0: 6069 6d66 702e 7365 745f 696d 665f 6170  `imfp.set_imf_ap
+000049b0: 705f 6e61 6d65 2829 6020 7365 7473 2074  p_name()` sets t
+000049c0: 6865 2061 7070 6c69 6361 7469 6f6e 206e  he application n
+000049d0: 616d 6520 6279 2063 6861 6e67 696e 6720  ame by changing 
+000049e0: 7468 6520 6049 4d46 5f41 5050 5f4e 414d  the `IMF_APP_NAM
+000049f0: 4560 2076 6172 6961 626c 6520 696e 2074  E` variable in t
+00004a00: 6865 2065 6e76 6972 6f6e 6d65 6e74 2e20  he environment. 
+00004a10: 4966 2074 6869 7320 7661 7269 6162 6c65  If this variable
+00004a20: 2064 6f65 736e 2774 2065 7869 7374 2c20   doesn't exist, 
+00004a30: 6069 6d66 702e 7365 745f 696d 665f 6170  `imfp.set_imf_ap
+00004a40: 705f 6e61 6d65 2829 6020 7769 6c6c 2063  p_name()` will c
+00004a50: 7265 6174 6520 6974 2e0d 0a0d 0a54 6f20  reate it.....To 
+00004a60: 7365 7420 6120 6375 7374 6f6d 2061 7070  set a custom app
+00004a70: 6c69 6361 7469 6f6e 206e 616d 652c 2073  lication name, s
+00004a80: 696d 706c 7920 6361 6c6c 2074 6865 2060  imply call the `
+00004a90: 696d 6670 2e73 6574 5f69 6d66 5f61 7070  imfp.set_imf_app
+00004aa0: 5f6e 616d 6528 2960 2066 756e 6374 696f  _name()` functio
+00004ab0: 6e20 7769 7468 2079 6f75 7220 6465 7369  n with your desi
+00004ac0: 7265 6420 6170 706c 6963 6174 696f 6e20  red application 
+00004ad0: 6e61 6d65 2061 7320 616e 2061 7267 756d  name as an argum
+00004ae0: 656e 743a 0d0a 0d0a 0d0a 6060 6070 7974  ent:......```pyt
+00004af0: 686f 6e0d 0a23 2053 6574 2063 7573 746f  hon..# Set custo
+00004b00: 6d20 6170 7020 6e61 6d65 2061 7320 616e  m app name as an
+00004b10: 2065 6e76 6972 6f6e 6d65 6e74 2076 6172   environment var
+00004b20: 6961 626c 650d 0a69 6d66 702e 7365 745f  iable..imfp.set_
+00004b30: 696d 665f 6170 705f 6e61 6d65 2822 6d79  imf_app_name("my
+00004b40: 5f63 7573 746f 6d5f 6170 705f 6e61 6d65  _custom_app_name
+00004b50: 2229 0d0a 6060 600d 0a0d 0a0d 0a0d 0a54  ")..```........T
+00004b60: 6865 2066 756e 6374 696f 6e20 7769 6c6c  he function will
+00004b70: 2074 6872 6f77 2061 6e20 6572 726f 7220   throw an error 
+00004b80: 6966 2074 6865 2070 726f 7669 6465 6420  if the provided 
+00004b90: 6e61 6d65 2069 7320 6d69 7373 696e 672c  name is missing,
+00004ba0: 204e 554c 4c2c 204e 412c 206e 6f74 2061   NULL, NA, not a
+00004bb0: 2073 7472 696e 672c 206f 7220 6c6f 6e67   string, or long
+00004bc0: 6572 2074 6861 6e20 3235 3520 6368 6172  er than 255 char
+00004bd0: 6163 7465 7273 2e20 4966 2074 6865 2070  acters. If the p
+00004be0: 726f 7669 6465 6420 6e61 6d65 2069 7320  rovided name is 
+00004bf0: 2269 6d66 7222 2028 7468 6520 6465 6661  "imfr" (the defa
+00004c00: 756c 7429 206f 7220 616e 2065 6d70 7479  ult) or an empty
+00004c10: 2073 7472 696e 672c 2074 6865 2066 756e   string, the fun
+00004c20: 6374 696f 6e20 7769 6c6c 2069 7373 7565  ction will issue
+00004c30: 2061 2077 6172 6e69 6e67 2072 6563 6f6d   a warning recom
+00004c40: 6d65 6e64 696e 6720 7468 6520 7573 6520  mending the use 
+00004c50: 6f66 2061 2075 6e69 7175 6520 6170 7020  of a unique app 
+00004c60: 6e61 6d65 2074 6f20 6176 6f69 6420 6869  name to avoid hi
+00004c70: 7474 696e 6720 7261 7465 206c 696d 6974  tting rate limit
+00004c80: 732e 0d0a 0d0a 2323 2320 4368 616e 6769  s.....### Changi
+00004c90: 6e67 2074 6865 2065 6e66 6f72 6365 6420  ng the enforced 
+00004ca0: 7761 6974 2074 696d 6520 6265 7477 6565  wait time betwee
+00004cb0: 6e20 4150 4920 6361 6c6c 7320 7769 7468  n API calls with
+00004cc0: 2060 7365 745f 696d 665f 7761 6974 5f74   `set_imf_wait_t
+00004cd0: 696d 6560 0d0a 0d0a 4279 2064 6566 6175  ime`....By defau
+00004ce0: 6c74 2c20 6069 6d66 7060 2065 6e66 6f72  lt, `imfp` enfor
+00004cf0: 6365 7320 6120 6d61 6e64 6174 6f72 7920  ces a mandatory 
+00004d00: 312e 352d 7365 636f 6e64 2077 6169 7420  1.5-second wait 
+00004d10: 7469 6d65 2062 6574 7765 656e 2041 5049  time between API
+00004d20: 2063 616c 6c73 2074 6f20 7072 6576 656e   calls to preven
+00004d30: 7420 7265 7065 6174 6564 206f 7220 7265  t repeated or re
+00004d40: 6375 7273 6976 6520 6361 6c6c 7320 6672  cursive calls fr
+00004d50: 6f6d 2065 7863 6565 6469 6e67 2074 6865  om exceeding the
+00004d60: 2041 5049 2773 2062 616e 6477 6964 7468   API's bandwidth
+00004d70: 2f72 6174 6520 6c69 6d69 742e 2054 6869  /rate limit. Thi
+00004d80: 7320 7761 6974 2074 696d 6520 7368 6f75  s wait time shou
+00004d90: 6c64 2062 6520 7375 6666 6963 6965 6e74  ld be sufficient
+00004da0: 2066 6f72 206d 6f73 7420 6170 706c 6963   for most applic
+00004db0: 6174 696f 6e73 2e20 486f 7765 7665 722c  ations. However,
+00004dc0: 2069 6620 796f 7520 6172 6520 7275 6e6e   if you are runn
+00004dd0: 696e 6720 7061 7261 6c6c 656c 2070 726f  ing parallel pro
+00004de0: 6365 7373 6573 2075 7369 6e67 2060 696d  cesses using `im
+00004df0: 6670 6020 2865 2e67 2e20 6475 7269 6e67  fp` (e.g. during
+00004e00: 2063 726f 7373 2d70 6c61 7466 6f72 6d20   cross-platform 
+00004e10: 7465 7374 696e 6729 2c20 7468 6973 2077  testing), this w
+00004e20: 6169 7420 7469 6d65 206d 6179 2062 6520  ait time may be 
+00004e30: 696e 7375 6666 6963 6965 6e74 2074 6f20  insufficient to 
+00004e40: 7072 6576 656e 7420 796f 7520 6672 6f6d  prevent you from
+00004e50: 2072 756e 6e69 6e67 2075 7020 6167 6169   running up agai
+00004e60: 6e73 7420 7468 6520 4150 4927 7320 7261  nst the API's ra
+00004e70: 7465 2061 6e64 2062 616e 6477 6964 7468  te and bandwidth
+00004e80: 206c 696d 6974 732e 2059 6f75 2063 616e   limits. You can
+00004e90: 2063 6861 6e67 6520 7468 6973 2077 6169   change this wai
+00004ea0: 7420 7469 6d65 2062 7920 6361 6c6c 696e  t time by callin
+00004eb0: 6720 7468 6520 6073 6574 5f69 6d66 5f77  g the `set_imf_w
+00004ec0: 6169 745f 7469 6d65 6020 6675 6e63 7469  ait_time` functi
+00004ed0: 6f6e 2077 6974 6820 6120 6e75 6d65 7269  on with a numeri
+00004ee0: 6320 7661 6c75 652c 2069 6e20 7365 636f  c value, in seco
+00004ef0: 6e64 732e 2046 6f72 2069 6e73 7461 6e63  nds. For instanc
+00004f00: 652c 2074 6f20 656e 666f 7263 6520 6120  e, to enforce a 
+00004f10: 6669 7665 2d73 6563 6f6e 6420 7761 6974  five-second wait
+00004f20: 2074 696d 6520 6265 7477 6565 6e20 4150   time between AP
+00004f30: 4920 6361 6c6c 732c 2075 7365 2060 7365  I calls, use `se
+00004f40: 745f 696d 665f 7761 6974 5f74 696d 6528  t_imf_wait_time(
+00004f50: 3130 2960 2e0d 0a0d 0a41 6c73 6f20 6e6f  10)`.....Also no
+00004f60: 7465 2074 6861 7420 6279 2064 6566 6175  te that by defau
+00004f70: 6c74 2c20 6069 6d66 7060 2066 756e 6374  lt, `imfp` funct
+00004f80: 696f 6e73 2077 696c 6c20 7265 7472 7920  ions will retry 
+00004f90: 616e 7920 4150 4920 6361 6c6c 2072 656a  any API call rej
+00004fa0: 6563 7465 6420 666f 7220 6261 6e64 7769  ected for bandwi
+00004fb0: 6474 6820 6f72 2072 6174 6520 6c69 6d69  dth or rate limi
+00004fc0: 7420 7265 6173 6f6e 732e 2054 6865 206e  t reasons. The n
+00004fd0: 756d 6265 7220 6f66 2074 696d 6573 2060  umber of times `
+00004fe0: 696d 6670 6020 7769 6c6c 2061 7474 656d  imfp` will attem
+00004ff0: 7074 2074 6865 2063 616c 6c20 6973 2073  pt the call is s
+00005000: 6574 2062 7920 7468 6520 6074 696d 6573  et by the `times
+00005010: 6020 6172 6775 6d65 6e74 2c20 7769 7468  ` argument, with
+00005020: 2061 2064 6566 6175 6c74 2076 616c 7565   a default value
+00005030: 206f 6620 332e 2028 5769 7468 2074 6869   of 3. (With thi
+00005040: 7320 7661 6c75 652c 2072 6571 7565 7374  s value, request
+00005050: 7320 7769 6c6c 2062 6520 7265 7472 6965  s will be retrie
+00005060: 6420 7477 6963 6520 6166 7465 7220 616e  d twice after an
+00005070: 2069 6e69 7469 616c 2066 6169 6c75 7265   initial failure
+00005080: 2e29 204e 6f74 6520 7468 6174 2060 696d  .) Note that `im
+00005090: 6670 6020 656e 666f 7263 6573 2061 6e20  fp` enforces an 
+000050a0: 6578 706f 6e65 6e74 6961 6c6c 7920 696e  exponentially in
+000050b0: 6372 6561 7369 6e67 2077 6169 7420 7469  creasing wait ti
+000050c0: 6d65 2062 6574 7765 656e 2066 756e 6374  me between funct
+000050d0: 696f 6e20 6361 6c6c 732c 2077 6974 6820  ion calls, with 
+000050e0: 6120 6261 7365 2077 6169 7420 7469 6d65  a base wait time
+000050f0: 206f 6620 3520 7365 636f 6e64 7320 6f6e   of 5 seconds on
+00005100: 2074 6865 2066 6972 7374 2072 6574 7279   the first retry
+00005110: 2c20 736f 2069 7420 6973 206e 6f74 2072  , so it is not r
+00005120: 6563 6f6d 6d65 6e64 6564 2074 6f20 7365  ecommended to se
+00005130: 7420 6120 6869 6768 2076 616c 7565 2066  t a high value f
+00005140: 6f72 2060 7469 6d65 7360 2e0d 0a0d 0a23  or `times`.....#
+00005150: 2320 436f 6e74 7269 6275 7469 6e67 0d0a  # Contributing..
+00005160: 0d0a 4920 776f 756c 6420 6c6f 7665 2074  ..I would love t
+00005170: 6f20 6861 7665 2079 6f75 7220 6865 6c70  o have your help
+00005180: 2069 6e20 696d 7072 6f76 696e 6720 6069   in improving `i
+00005190: 6d66 7260 2e20 4966 2079 6f75 2065 6e63  mfr`. If you enc
+000051a0: 6f75 6e74 6572 2061 2062 7567 2077 6869  ounter a bug whi
+000051b0: 6c65 2075 7369 6e67 2074 6865 206c 6962  le using the lib
+000051c0: 7261 7279 2c20 706c 6561 7365 206f 7065  rary, please ope
+000051d0: 6e20 616e 2069 7373 7565 2e20 416c 7465  n an issue. Alte
+000051e0: 726e 6174 6976 656c 792c 2066 6978 2074  rnatively, fix t
+000051f0: 6865 2062 7567 2061 6e64 206f 7065 6e20  he bug and open 
+00005200: 6120 7075 6c6c 2072 6571 7565 7374 2e20  a pull request. 
+00005210: 5468 616e 6b73 2069 6e20 6164 7661 6e63  Thanks in advanc
+00005220: 6520 666f 7220 796f 7572 2068 656c 7021  e for your help!
+00005230: 0d0a                                     ..
```

### Comparing `imfp-1.0.8/PKG-INFO` & `imfp-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 696d 6670  : 2.1.Name: imfp
-00000020: 0a56 6572 7369 6f6e 3a20 312e 302e 380a  .Version: 1.0.8.
+00000020: 0a56 6572 7369 6f6e 3a20 312e 312e 300a  .Version: 1.1.0.
 00000030: 5375 6d6d 6172 793a 2050 7974 686f 6e20  Summary: Python 
 00000040: 7061 636b 6167 6520 666f 7220 646f 776e  package for down
 00000050: 6c6f 6164 696e 6720 6563 6f6e 6f6d 6963  loading economic
 00000060: 2064 6174 6120 6672 6f6d 2074 6865 2049   data from the I
 00000070: 6e74 6572 6e61 7469 6f6e 616c 204d 6f6e  nternational Mon
 00000080: 6574 6172 7920 4675 6e64 204a 534f 4e20  etary Fund JSON 
 00000090: 5245 5354 6675 6c20 4150 4920 656e 6470  RESTful API endp
@@ -132,1185 +132,1204 @@
 00000830: 7220 636f 6d70 7574 6174 696f 6e2e 2054  r computation. T
 00000840: 6865 7365 2070 6163 6b61 6765 7320 6361  hese packages ca
 00000850: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
 00000860: 7369 6e67 2060 7069 7060 2061 6e64 206c  sing `pip` and l
 00000870: 6f61 6465 6420 7573 696e 6720 6069 6d70  oaded using `imp
 00000880: 6f72 7460 3a0a 0a0a 6060 6070 7974 686f  ort`:...```pytho
 00000890: 6e0a 696d 706f 7274 2073 6561 626f 726e  n.import seaborn
-000008a0: 0a60 6060 0a0a 2323 2320 5365 7474 696e  .```..### Settin
-000008b0: 6720 6120 556e 6971 7565 2041 7070 6c69  g a Unique Appli
-000008c0: 6361 7469 6f6e 204e 616d 6520 7769 7468  cation Name with
-000008d0: 2069 6d66 5f61 7070 5f6e 616d 650a 0a60   imf_app_name..`
-000008e0: 696d 6670 2e69 6d66 5f61 7070 5f6e 616d  imfp.imf_app_nam
-000008f0: 6528 2960 2061 6c6c 6f77 7320 7573 6572  e()` allows user
-00000900: 7320 746f 2073 6574 2061 2063 7573 746f  s to set a custo
-00000910: 6d20 6170 706c 6963 6174 696f 6e20 6e61  m application na
-00000920: 6d65 2074 6f20 6265 2075 7365 6420 7768  me to be used wh
-00000930: 656e 206d 616b 696e 6720 4150 4920 6361  en making API ca
-00000940: 6c6c 7320 746f 2074 6865 2049 4d46 2041  lls to the IMF A
-00000950: 5049 2e20 5468 6520 494d 4620 4150 4920  PI. The IMF API 
-00000960: 6861 7320 616e 2061 7070 6c69 6361 7469  has an applicati
-00000970: 6f6e 2d62 6173 6564 2072 6174 6520 6c69  on-based rate li
-00000980: 6d69 7420 6f66 2035 3020 7265 7175 6573  mit of 50 reques
-00000990: 7473 2070 6572 2073 6563 6f6e 642c 2077  ts per second, w
-000009a0: 6974 6820 7468 6520 6170 706c 6963 6174  ith the applicat
-000009b0: 696f 6e20 6964 656e 7469 6669 6564 2062  ion identified b
-000009c0: 7920 7468 6520 2275 7365 725f 6167 656e  y the "user_agen
-000009d0: 7422 2076 6172 6961 626c 6520 696e 2074  t" variable in t
-000009e0: 6865 2072 6571 7565 7374 2068 6561 6465  he request heade
-000009f0: 722e 0a0a 5468 6973 2063 6f75 6c64 2070  r...This could p
-00000a00: 726f 7665 2070 726f 626c 656d 6174 6963  rove problematic
-00000a10: 2069 6620 7468 6520 6069 6d66 7060 206c   if the `imfp` l
-00000a20: 6962 7261 7279 2062 6563 616d 6520 746f  ibrary became to
-00000a30: 6f20 706f 7075 6c61 7220 616e 6420 746f  o popular and to
-00000a40: 6f20 6d61 6e79 2075 7365 7273 2074 7269  o many users tri
-00000a50: 6564 2074 6f20 6d61 6b65 2073 696d 756c  ed to make simul
-00000a60: 7461 6e65 6f75 7320 4150 4920 7265 7175  taneous API requ
-00000a70: 6573 7473 2075 7369 6e67 2074 6865 2064  ests using the d
-00000a80: 6566 6175 6c74 2061 7070 206e 616d 652e  efault app name.
-00000a90: 2042 7920 7365 7474 696e 6720 6120 6375   By setting a cu
-00000aa0: 7374 6f6d 2061 7070 6c69 6361 7469 6f6e  stom application
-00000ab0: 206e 616d 652c 2075 7365 7273 2063 616e   name, users can
-00000ac0: 2061 766f 6964 2068 6974 7469 6e67 2072   avoid hitting r
-00000ad0: 6174 6520 6c69 6d69 7473 2061 6e64 2062  ate limits and b
-00000ae0: 6569 6e67 2062 6c6f 636b 6564 2062 7920  eing blocked by 
-00000af0: 7468 6520 4150 492e 2060 696d 6670 2e69  the API. `imfp.i
-00000b00: 6d66 5f61 7070 5f6e 616d 6528 2960 2073  mf_app_name()` s
-00000b10: 6574 7320 7468 6520 6170 706c 6963 6174  ets the applicat
-00000b20: 696f 6e20 6e61 6d65 2062 7920 6368 616e  ion name by chan
-00000b30: 6769 6e67 2074 6865 2060 494d 465f 4150  ging the `IMF_AP
-00000b40: 505f 4e41 4d45 6020 7661 7269 6162 6c65  P_NAME` variable
-00000b50: 2069 6e20 7468 6520 656e 7669 726f 6e6d   in the environm
-00000b60: 656e 742e 2049 6620 7468 6973 2076 6172  ent. If this var
-00000b70: 6961 626c 6520 646f 6573 6e27 7420 6578  iable doesn't ex
-00000b80: 6973 742c 2060 696d 6670 2e69 6d66 5f61  ist, `imfp.imf_a
-00000b90: 7070 5f6e 616d 6528 2960 2077 696c 6c20  pp_name()` will 
-00000ba0: 6372 6561 7465 2069 742e 0a0a 546f 2073  create it...To s
-00000bb0: 6574 2061 2063 7573 746f 6d20 6170 706c  et a custom appl
-00000bc0: 6963 6174 696f 6e20 6e61 6d65 2c20 7369  ication name, si
-00000bd0: 6d70 6c79 2063 616c 6c20 7468 6520 6069  mply call the `i
-00000be0: 6d66 702e 696d 665f 6170 705f 6e61 6d65  mfp.imf_app_name
-00000bf0: 2829 6020 6675 6e63 7469 6f6e 2077 6974  ()` function wit
-00000c00: 6820 796f 7572 2064 6573 6972 6564 2061  h your desired a
-00000c10: 7070 6c69 6361 7469 6f6e 206e 616d 6520  pplication name 
-00000c20: 6173 2061 6e20 6172 6775 6d65 6e74 3a0a  as an argument:.
-00000c30: 0a0a 6060 6070 7974 686f 6e0a 2320 5365  ..```python.# Se
-00000c40: 7420 6375 7374 6f6d 2061 7070 206e 616d  t custom app nam
-00000c50: 6520 6173 2061 6e20 656e 7669 726f 6e6d  e as an environm
-00000c60: 656e 7420 7661 7269 6162 6c65 0a69 6d66  ent variable.imf
-00000c70: 702e 696d 665f 6170 705f 6e61 6d65 2822  p.imf_app_name("
-00000c80: 6d79 5f63 7573 746f 6d5f 6170 705f 6e61  my_custom_app_na
-00000c90: 6d65 2229 0a60 6060 0a0a 0a0a 5468 6520  me").```....The 
-00000ca0: 6675 6e63 7469 6f6e 2077 696c 6c20 7468  function will th
-00000cb0: 726f 7720 616e 2065 7272 6f72 2069 6620  row an error if 
-00000cc0: 7468 6520 7072 6f76 6964 6564 206e 616d  the provided nam
-00000cd0: 6520 6973 206d 6973 7369 6e67 2c20 4e55  e is missing, NU
-00000ce0: 4c4c 2c20 4e41 2c20 6e6f 7420 6120 7374  LL, NA, not a st
-00000cf0: 7269 6e67 2c20 6f72 206c 6f6e 6765 7220  ring, or longer 
-00000d00: 7468 616e 2032 3535 2063 6861 7261 6374  than 255 charact
-00000d10: 6572 732e 2049 6620 7468 6520 7072 6f76  ers. If the prov
-00000d20: 6964 6564 206e 616d 6520 6973 2022 696d  ided name is "im
-00000d30: 6672 2220 2874 6865 2064 6566 6175 6c74  fr" (the default
-00000d40: 2920 6f72 2061 6e20 656d 7074 7920 7374  ) or an empty st
-00000d50: 7269 6e67 2c20 7468 6520 6675 6e63 7469  ring, the functi
-00000d60: 6f6e 2077 696c 6c20 6973 7375 6520 6120  on will issue a 
-00000d70: 7761 726e 696e 6720 7265 636f 6d6d 656e  warning recommen
-00000d80: 6469 6e67 2074 6865 2075 7365 206f 6620  ding the use of 
-00000d90: 6120 756e 6971 7565 2061 7070 206e 616d  a unique app nam
-00000da0: 6520 746f 2061 766f 6964 2068 6974 7469  e to avoid hitti
-00000db0: 6e67 2072 6174 6520 6c69 6d69 7473 2e0a  ng rate limits..
-00000dc0: 0a23 2323 2041 646a 7573 7469 6e67 2074  .### Adjusting t
-00000dd0: 6865 2072 6174 6520 6c69 6d69 7420 7769  he rate limit wi
-00000de0: 7468 205f 696d 665f 7761 6974 5f74 696d  th _imf_wait_tim
-00000df0: 650a 0a44 7572 696e 6720 696d 706f 7274  e..During import
-00000e00: 206f 6620 6069 6d66 7060 2c20 6120 7661   of `imfp`, a va
-00000e10: 7269 6162 6c65 2063 616c 6c65 6420 5f69  riable called _i
-00000e20: 6d66 5f77 6169 745f 7469 6d65 2069 7320  mf_wait_time is 
-00000e30: 7365 7420 746f 2061 2064 6566 6175 6c74  set to a default
-00000e40: 2076 616c 7565 206f 6620 312e 352e 2054   value of 1.5. T
-00000e50: 6869 7320 6973 2074 6865 206d 616e 6461  his is the manda
-00000e60: 746f 7279 2065 6e66 6f72 6365 6420 7761  tory enforced wa
-00000e70: 6974 2074 696d 6520 6265 7477 6565 6e20  it time between 
-00000e80: 4150 4920 6361 6c6c 732c 2074 6f20 7072  API calls, to pr
-00000e90: 6576 656e 7420 7265 7065 6174 6564 206f  event repeated o
-00000ea0: 7220 7265 6375 7273 6976 6520 6361 6c6c  r recursive call
-00000eb0: 7320 6672 6f6d 2065 7863 6565 6469 6e67  s from exceeding
-00000ec0: 2074 6865 206c 696d 6974 2e20 5468 6973   the limit. This
-00000ed0: 2077 6169 7420 7469 6d65 2073 686f 756c   wait time shoul
-00000ee0: 6420 6265 2073 7566 6669 6369 656e 7420  d be sufficient 
-00000ef0: 666f 7220 6d6f 7374 2061 7070 6c69 6361  for most applica
-00000f00: 7469 6f6e 732e 2048 6f77 6576 6572 2c20  tions. However, 
-00000f10: 6966 2079 6f75 2061 7265 2072 756e 6e69  if you are runni
-00000f20: 6e67 2070 6172 616c 6c65 6c20 7072 6f63  ng parallel proc
-00000f30: 6573 7365 7320 7573 696e 6720 6069 6d66  esses using `imf
-00000f40: 7060 2028 652e 672e 2064 7572 696e 6720  p` (e.g. during 
-00000f50: 6372 6f73 732d 706c 6174 666f 726d 2074  cross-platform t
-00000f60: 6573 7469 6e67 292c 2074 6869 7320 7761  esting), this wa
-00000f70: 6974 2074 696d 6520 6d61 7920 6265 2069  it time may be i
-00000f80: 6e73 7566 6669 6369 656e 7420 746f 2070  nsufficient to p
-00000f90: 7265 7665 6e74 2079 6f75 2066 726f 6d20  revent you from 
-00000fa0: 7275 6e6e 696e 6720 7570 2061 6761 696e  running up again
-00000fb0: 7374 2074 6865 2041 5049 2773 2072 6174  st the API's rat
-00000fc0: 6520 616e 6420 6261 6e64 7769 6474 6820  e and bandwidth 
-00000fd0: 6c69 6d69 7473 2e20 596f 7520 6361 6e20  limits. You can 
-00000fe0: 696e 6372 6561 7365 2074 6869 7320 7761  increase this wa
-00000ff0: 6974 2074 696d 6520 6279 2073 696d 706c  it time by simpl
-00001000: 7920 6368 616e 6769 6e67 2074 6865 2076  y changing the v
-00001010: 6172 6961 626c 6520 7661 6c75 652e 2046  ariable value. F
-00001020: 6f72 2069 6e73 7461 6e63 652c 2074 6f20  or instance, to 
-00001030: 696e 6372 6561 7365 2074 6865 2062 6574  increase the bet
-00001040: 7765 656e 2d63 616c 6c20 7761 6974 2074  ween-call wait t
-00001050: 696d 6520 6279 206f 6e65 2073 6563 6f6e  ime by one secon
-00001060: 642c 2075 7365 2060 5f69 6d66 5f77 6169  d, use `_imf_wai
-00001070: 745f 7469 6d65 202b 3d20 3160 2e0a 0a41  t_time += 1`...A
-00001080: 6c73 6f20 6e6f 7465 2074 6861 7420 6279  lso note that by
-00001090: 2064 6566 6175 6c74 2c20 6069 6d66 7060   default, `imfp`
-000010a0: 2066 756e 6374 696f 6e73 2077 696c 6c20   functions will 
-000010b0: 7265 7472 7920 616e 7920 4150 4920 6361  retry any API ca
-000010c0: 6c6c 2072 656a 6563 7465 6420 666f 7220  ll rejected for 
-000010d0: 6261 6e64 7769 6474 6820 6f72 2072 6174  bandwidth or rat
-000010e0: 6520 6c69 6d69 7420 7265 6173 6f6e 732e  e limit reasons.
-000010f0: 2054 6865 206e 756d 6265 7220 6f66 2074   The number of t
-00001100: 696d 6573 2060 696d 6670 6020 7769 6c6c  imes `imfp` will
-00001110: 2061 7474 656d 7074 2074 6865 2063 616c   attempt the cal
-00001120: 6c20 6973 2073 6574 2062 7920 7468 6520  l is set by the 
-00001130: 6074 696d 6573 6020 6172 6775 6d65 6e74  `times` argument
-00001140: 2c20 7769 7468 2061 2064 6566 6175 6c74  , with a default
-00001150: 2076 616c 7565 206f 6620 332e 2028 5769   value of 3. (Wi
-00001160: 7468 2074 6869 7320 7661 6c75 652c 2072  th this value, r
-00001170: 6571 7565 7374 7320 7769 6c6c 2062 6520  equests will be 
-00001180: 7265 7472 6965 6420 7477 6963 6520 6166  retried twice af
-00001190: 7465 7220 616e 2069 6e69 7469 616c 2066  ter an initial f
-000011a0: 6169 6c75 7265 2e29 204e 6f74 6520 7468  ailure.) Note th
-000011b0: 6174 2060 696d 6670 6020 656e 666f 7263  at `imfp` enforc
-000011c0: 6573 2061 6e20 6578 706f 6e65 6e74 6961  es an exponentia
-000011d0: 6c6c 7920 696e 6372 6561 7369 6e67 2077  lly increasing w
-000011e0: 6169 7420 7469 6d65 2062 6574 7765 656e  ait time between
-000011f0: 2066 756e 6374 696f 6e20 6361 6c6c 732c   function calls,
-00001200: 2077 6974 6820 6120 6261 7365 2077 6169   with a base wai
-00001210: 7420 7469 6d65 206f 6620 3520 7365 636f  t time of 5 seco
-00001220: 6e64 7320 6f6e 2074 6865 2066 6972 7374  nds on the first
-00001230: 2072 6574 7279 2c20 736f 2069 7420 6973   retry, so it is
-00001240: 206e 6f74 2072 6563 6f6d 6d65 6e64 6564   not recommended
-00001250: 2074 6f20 7365 7420 6120 6869 6768 2076   to set a high v
-00001260: 616c 7565 2066 6f72 2060 7469 6d65 7360  alue for `times`
-00001270: 2e0a 0a0a 2323 2320 4665 7463 6869 6e67  ....### Fetching
-00001280: 2061 6e20 496e 6465 7820 6f66 2044 6174   an Index of Dat
-00001290: 6162 6173 6573 2077 6974 6820 7468 6520  abases with the 
-000012a0: 696d 665f 6461 7461 6261 7365 7320 4675  imf_databases Fu
-000012b0: 6e63 7469 6f6e 0a0a 5468 6520 6069 6d66  nction..The `imf
-000012c0: 7060 2070 6163 6b61 6765 2069 6e74 726f  p` package intro
-000012d0: 6475 6365 7320 666f 7572 2063 6f72 6520  duces four core 
-000012e0: 6675 6e63 7469 6f6e 733a 2060 696d 6670  functions: `imfp
-000012f0: 2e69 6d66 5f64 6174 6162 6173 6573 602c  .imf_databases`,
-00001300: 2060 696d 6670 2e69 6d66 5f70 6172 616d   `imfp.imf_param
-00001310: 6574 6572 7360 2c20 6069 6d66 702e 696d  eters`, `imfp.im
-00001320: 665f 7061 7261 6d65 7465 725f 6465 6673  f_parameter_defs
-00001330: 602c 2061 6e64 2060 696d 6670 2e69 6d66  `, and `imfp.imf
-00001340: 5f64 6174 6173 6574 602e 2054 6865 2066  _dataset`. The f
-00001350: 756e 6374 696f 6e20 666f 7220 646f 776e  unction for down
-00001360: 6c6f 6164 696e 6720 6461 7461 7365 7473  loading datasets
-00001370: 2069 7320 6069 6d66 702e 696d 665f 6461   is `imfp.imf_da
-00001380: 7461 7365 7460 2c20 6275 7420 796f 7520  taset`, but you 
-00001390: 7769 6c6c 206e 6565 6420 7468 6520 6f74  will need the ot
-000013a0: 6865 7220 6675 6e63 7469 6f6e 7320 746f  her functions to
-000013b0: 2064 6574 6572 6d69 6e65 2077 6861 7420   determine what 
-000013c0: 6172 6775 6d65 6e74 7320 746f 2073 7570  arguments to sup
-000013d0: 706c 7920 746f 2060 696d 6670 2e69 6d66  ply to `imfp.imf
-000013e0: 5f64 6174 6173 6574 602e 2046 6f72 2069  _dataset`. For i
-000013f0: 6e73 7461 6e63 652c 2061 6c6c 2063 616c  nstance, all cal
-00001400: 6c73 2074 6f20 6069 6d66 702e 696d 665f  ls to `imfp.imf_
-00001410: 6461 7461 7365 7460 2072 6571 7569 7265  dataset` require
-00001420: 2061 2060 6461 7461 6261 7365 5f69 6460   a `database_id`
-00001430: 2e20 5468 6973 2069 7320 6265 6361 7573  . This is becaus
-00001440: 6520 7468 6520 494d 4620 7365 7276 6573  e the IMF serves
-00001450: 206d 616e 7920 6469 6666 6572 656e 7420   many different 
-00001460: 6461 7461 6261 7365 7320 7468 726f 7567  databases throug
-00001470: 6820 6974 7320 4150 492c 2061 6e64 2074  h its API, and t
-00001480: 6865 2041 5049 206e 6565 6473 2074 6f20  he API needs to 
-00001490: 6b6e 6f77 2077 6869 6368 206f 6620 7468  know which of th
-000014a0: 6573 6520 6d61 6e79 2064 6174 6162 6173  ese many databas
-000014b0: 6573 2079 6f75 2772 6520 7265 7175 6573  es you're reques
-000014c0: 7469 6e67 2064 6174 6120 6672 6f6d 2e20  ting data from. 
-000014d0: 546f 206f 6274 6169 6e20 6120 6c69 7374  To obtain a list
-000014e0: 206f 6620 6461 7461 6261 7365 732c 2075   of databases, u
-000014f0: 7365 2060 696d 6670 2e69 6d66 5f64 6174  se `imfp.imf_dat
-00001500: 6162 6173 6573 602c 206c 696b 6520 736f  abases`, like so
-00001510: 3a0a 0a0a 6060 6070 7974 686f 6e0a 2346  :...```python.#F
-00001520: 6574 6368 2074 6865 206c 6973 7420 6f66  etch the list of
-00001530: 2064 6174 6162 6173 6573 2061 7661 696c   databases avail
-00001540: 6162 6c65 2074 6872 6f75 6768 2074 6865  able through the
-00001550: 2049 4d46 2041 5049 0a64 6174 6162 6173   IMF API.databas
-00001560: 6573 203d 2069 6d66 702e 696d 665f 6461  es = imfp.imf_da
-00001570: 7461 6261 7365 7328 290a 6461 7461 6261  tabases().databa
-00001580: 7365 732e 6865 6164 2829 0a60 6060 0a0a  ses.head().```..
-00001590: 0a0a 0a3c 6469 763e 0a0a 3c74 6162 6c65  ...<div>..<table
-000015a0: 2062 6f72 6465 723d 2231 2220 636c 6173   border="1" clas
-000015b0: 733d 2264 6174 6166 7261 6d65 223e 0a20  s="dataframe">. 
-000015c0: 203c 7468 6561 643e 0a20 2020 203c 7472   <thead>.    <tr
-000015d0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-000015e0: 676e 3a20 7269 6768 743b 223e 0a20 2020  gn: right;">.   
-000015f0: 2020 203c 7468 3e3c 2f74 683e 0a20 2020     <th></th>.   
-00001600: 2020 203c 7468 3e64 6174 6162 6173 655f     <th>database_
-00001610: 6964 3c2f 7468 3e0a 2020 2020 2020 3c74  id</th>.      <t
-00001620: 683e 6465 7363 7269 7074 696f 6e3c 2f74  h>description</t
-00001630: 683e 0a20 2020 203c 2f74 723e 0a20 203c  h>.    </tr>.  <
-00001640: 2f74 6865 6164 3e0a 2020 3c74 626f 6479  /thead>.  <tbody
-00001650: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001660: 203c 7468 3e30 3c2f 7468 3e0a 2020 2020   <th>0</th>.    
-00001670: 2020 3c74 643e 424f 505f 3230 3137 4d30    <td>BOP_2017M0
-00001680: 363c 2f74 643e 0a20 2020 2020 203c 7464  6</td>.      <td
-00001690: 3e42 616c 616e 6365 206f 6620 5061 796d  >Balance of Paym
-000016a0: 656e 7473 2028 424f 5029 2c20 3230 3137  ents (BOP), 2017
-000016b0: 204d 3036 3c2f 7464 3e0a 2020 2020 3c2f   M06</td>.    </
-000016c0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-000016d0: 2020 203c 7468 3e31 3c2f 7468 3e0a 2020     <th>1</th>.  
-000016e0: 2020 2020 3c74 643e 424f 505f 3230 3230      <td>BOP_2020
-000016f0: 4d33 3c2f 7464 3e0a 2020 2020 2020 3c74  M3</td>.      <t
-00001700: 643e 4261 6c61 6e63 6520 6f66 2050 6179  d>Balance of Pay
-00001710: 6d65 6e74 7320 2842 4f50 292c 2032 3032  ments (BOP), 202
-00001720: 3020 4d30 333c 2f74 643e 0a20 2020 203c  0 M03</td>.    <
-00001730: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
-00001740: 2020 2020 3c74 683e 323c 2f74 683e 0a20      <th>2</th>. 
-00001750: 2020 2020 203c 7464 3e42 4f50 5f32 3031       <td>BOP_201
-00001760: 374d 3131 3c2f 7464 3e0a 2020 2020 2020  7M11</td>.      
-00001770: 3c74 643e 4261 6c61 6e63 6520 6f66 2050  <td>Balance of P
-00001780: 6179 6d65 6e74 7320 2842 4f50 292c 2032  ayments (BOP), 2
-00001790: 3031 3720 4d31 313c 2f74 643e 0a20 2020  017 M11</td>.   
-000017a0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
-000017b0: 2020 2020 2020 3c74 683e 333c 2f74 683e        <th>3</th>
-000017c0: 0a20 2020 2020 203c 7464 3e44 4f54 5f32  .      <td>DOT_2
-000017d0: 3032 3051 313c 2f74 643e 0a20 2020 2020  020Q1</td>.     
-000017e0: 203c 7464 3e44 6972 6563 7469 6f6e 206f   <td>Direction o
-000017f0: 6620 5472 6164 6520 5374 6174 6973 7469  f Trade Statisti
-00001800: 6373 2028 444f 5453 292c 2032 3032 3020  cs (DOTS), 2020 
-00001810: 5131 3c2f 7464 3e0a 2020 2020 3c2f 7472  Q1</td>.    </tr
-00001820: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001830: 203c 7468 3e34 3c2f 7468 3e0a 2020 2020   <th>4</th>.    
-00001840: 2020 3c74 643e 4746 534d 4142 3230 3136    <td>GFSMAB2016
-00001850: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-00001860: 476f 7665 726e 6d65 6e74 2046 696e 616e  Government Finan
-00001870: 6365 2053 7461 7469 7374 6963 7320 5965  ce Statistics Ye
-00001880: 6172 626f 6f6b 2028 4746 5359 2032 2e2e  arbook (GFSY 2..
-00001890: 2e3c 2f74 643e 0a20 2020 203c 2f74 723e  .</td>.    </tr>
-000018a0: 0a20 203c 2f74 626f 6479 3e0a 3c2f 7461  .  </tbody>.</ta
-000018b0: 626c 653e 0a3c 2f64 6976 3e0a 0a0a 0a54  ble>.</div>....T
-000018c0: 6869 7320 6675 6e63 7469 6f6e 2072 6574  his function ret
-000018d0: 7572 6e73 2074 6865 2049 4d46 e280 9973  urns the IMF...s
-000018e0: 206c 6973 7469 6e67 206f 6620 3235 3920   listing of 259 
-000018f0: 6461 7461 6261 7365 7320 6176 6169 6c61  databases availa
-00001900: 626c 6520 7468 726f 7567 6820 7468 6520  ble through the 
-00001910: 4150 492e 2028 496e 2072 6561 6c69 7479  API. (In reality
-00001920: 2c20 3720 6f66 2074 6865 206c 6973 7465  , 7 of the liste
-00001930: 6420 6461 7461 6261 7365 7320 6172 6520  d databases are 
-00001940: 6465 6675 6e63 7420 616e 6420 6e6f 7420  defunct and not 
-00001950: 6163 7475 616c 6c79 2061 7661 696c 6162  actually availab
-00001960: 6c65 3a20 4641 535f 3230 3135 2c20 4746  le: FAS_2015, GF
-00001970: 5330 312c 2046 4d32 3032 3031 302c 2041  S01, FM202010, A
-00001980: 5044 5245 4f32 3032 3031 302c 2041 4652  PDREO202010, AFR
-00001990: 5245 4f32 3032 3031 302c 2057 4844 5245  REO202010, WHDRE
-000019a0: 4f32 3032 3031 302c 2042 4f50 4147 475f  O202010, BOPAGG_
-000019b0: 3230 3230 2e29 0a0a 546f 2076 6965 7720  2020.)..To view 
-000019c0: 616e 6420 6578 706c 6f72 6520 7468 6520  and explore the 
-000019d0: 6461 7461 6261 7365 206c 6973 742c 2069  database list, i
-000019e0: 74e2 8099 7320 706f 7373 6962 6c65 2074  t...s possible t
-000019f0: 6f20 6578 706c 6f72 6520 7375 6273 6574  o explore subset
-00001a00: 7320 6f66 2074 6865 2064 6174 6120 6672  s of the data fr
-00001a10: 616d 6520 6279 2072 6f77 206e 756d 6265  ame by row numbe
-00001a20: 7220 7769 7468 2060 6461 7461 6261 7365  r with `database
-00001a30: 732e 6c6f 6360 3a0a 0a0a 0a60 6060 7079  s.loc`:....```py
-00001a40: 7468 6f6e 0a23 2056 6965 7720 6120 7375  thon.# View a su
-00001a50: 6273 6574 2063 6f6e 7369 7374 696e 6720  bset consisting 
-00001a60: 6f66 2072 6f77 7320 3520 7468 726f 7567  of rows 5 throug
-00001a70: 6820 390a 6461 7461 6261 7365 732e 6c6f  h 9.databases.lo
-00001a80: 635b 353a 395d 0a60 6060 0a0a 0a0a 0a3c  c[5:9].```.....<
-00001a90: 6469 763e 0a0a 3c74 6162 6c65 2062 6f72  div>..<table bor
-00001aa0: 6465 723d 2231 2220 636c 6173 733d 2264  der="1" class="d
-00001ab0: 6174 6166 7261 6d65 223e 0a20 203c 7468  ataframe">.  <th
-00001ac0: 6561 643e 0a20 2020 203c 7472 2073 7479  ead>.    <tr sty
-00001ad0: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
-00001ae0: 7269 6768 743b 223e 0a20 2020 2020 203c  right;">.      <
-00001af0: 7468 3e3c 2f74 683e 0a20 2020 2020 203c  th></th>.      <
-00001b00: 7468 3e64 6174 6162 6173 655f 6964 3c2f  th>database_id</
-00001b10: 7468 3e0a 2020 2020 2020 3c74 683e 6465  th>.      <th>de
-00001b20: 7363 7269 7074 696f 6e3c 2f74 683e 0a20  scription</th>. 
-00001b30: 2020 203c 2f74 723e 0a20 203c 2f74 6865     </tr>.  </the
-00001b40: 6164 3e0a 2020 3c74 626f 6479 3e0a 2020  ad>.  <tbody>.  
-00001b50: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
-00001b60: 3e35 3c2f 7468 3e0a 2020 2020 2020 3c74  >5</th>.      <t
-00001b70: 643e 424f 505f 3230 3139 4d31 323c 2f74  d>BOP_2019M12</t
-00001b80: 643e 0a20 2020 2020 203c 7464 3e42 616c  d>.      <td>Bal
-00001b90: 616e 6365 206f 6620 5061 796d 656e 7473  ance of Payments
-00001ba0: 2028 424f 5029 2c20 3230 3139 204d 3132   (BOP), 2019 M12
-00001bb0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
-00001bc0: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
-00001bd0: 7468 3e36 3c2f 7468 3e0a 2020 2020 2020  th>6</th>.      
-00001be0: 3c74 643e 4746 5359 4641 4c43 5332 3031  <td>GFSYFALCS201
-00001bf0: 343c 2f74 643e 0a20 2020 2020 203c 7464  4</td>.      <td
-00001c00: 3e47 6f76 6572 6e6d 656e 7420 4669 6e61  >Government Fina
-00001c10: 6e63 6520 5374 6174 6973 7469 6373 2059  nce Statistics Y
-00001c20: 6561 7262 6f6f 6b20 2847 4653 5920 322e  earbook (GFSY 2.
-00001c30: 2e2e 3c2f 7464 3e0a 2020 2020 3c2f 7472  ..</td>.    </tr
-00001c40: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00001c50: 203c 7468 3e37 3c2f 7468 3e0a 2020 2020   <th>7</th>.    
-00001c60: 2020 3c74 643e 4746 5345 3230 3136 3c2f    <td>GFSE2016</
-00001c70: 7464 3e0a 2020 2020 2020 3c74 643e 476f  td>.      <td>Go
-00001c80: 7665 726e 6d65 6e74 2046 696e 616e 6365  vernment Finance
-00001c90: 2053 7461 7469 7374 6963 7320 5965 6172   Statistics Year
-00001ca0: 626f 6f6b 2028 4746 5359 2032 2e2e 2e3c  book (GFSY 2...<
-00001cb0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
-00001cc0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
-00001cd0: 683e 383c 2f74 683e 0a20 2020 2020 203c  h>8</th>.      <
-00001ce0: 7464 3e46 4d32 3031 3531 303c 2f74 643e  td>FM201510</td>
-00001cf0: 0a20 2020 2020 203c 7464 3e46 6973 6361  .      <td>Fisca
-00001d00: 6c20 4d6f 6e69 746f 7220 2846 4d29 204f  l Monitor (FM) O
-00001d10: 6374 6f62 6572 2032 3031 353c 2f74 643e  ctober 2015</td>
-00001d20: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
-00001d30: 7472 3e0a 2020 2020 2020 3c74 683e 393c  tr>.      <th>9<
-00001d40: 2f74 683e 0a20 2020 2020 203c 7464 3e47  /th>.      <td>G
-00001d50: 4653 4942 5332 3031 363c 2f74 643e 0a20  FSIBS2016</td>. 
-00001d60: 2020 2020 203c 7464 3e47 6f76 6572 6e6d       <td>Governm
-00001d70: 656e 7420 4669 6e61 6e63 6520 5374 6174  ent Finance Stat
-00001d80: 6973 7469 6373 2059 6561 7262 6f6f 6b20  istics Yearbook 
-00001d90: 2847 4653 5920 322e 2e2e 3c2f 7464 3e0a  (GFSY 2...</td>.
-00001da0: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7462      </tr>.  </tb
-00001db0: 6f64 793e 0a3c 2f74 6162 6c65 3e0a 3c2f  ody>.</table>.</
-00001dc0: 6469 763e 0a0a 0a0a 0a20 4f72 2c20 6966  div>..... Or, if
-00001dd0: 2079 6f75 2061 6c72 6561 6479 206b 6e6f   you already kno
-00001de0: 7720 7768 6963 6820 6461 7461 6261 7365  w which database
-00001df0: 2079 6f75 2077 616e 742c 2079 6f75 2063   you want, you c
-00001e00: 616e 2066 6574 6368 2074 6865 2063 6f72  an fetch the cor
-00001e10: 7265 7370 6f6e 6469 6e67 2063 6f64 6520  responding code 
-00001e20: 6279 2073 6561 7263 6869 6e67 2066 6f72  by searching for
-00001e30: 2061 2073 7472 696e 6720 6d61 7463 6820   a string match 
-00001e40: 7573 696e 6720 6073 7472 2e63 6f6e 7461  using `str.conta
-00001e50: 696e 7360 2061 6e64 2073 7562 7365 7474  ins` and subsett
-00001e60: 696e 6720 7468 6520 6461 7461 2066 7261  ing the data fra
-00001e70: 6d65 2066 6f72 206d 6174 6368 696e 6720  me for matching 
-00001e80: 726f 7773 2e20 466f 7220 696e 7374 616e  rows. For instan
-00001e90: 6365 2c20 6865 7265 e280 9973 2068 6f77  ce, here...s how
-00001ea0: 2074 6f20 7365 6172 6368 2066 6f72 2074   to search for t
-00001eb0: 6865 2050 7269 6d61 7279 2043 6f6d 6d6f  he Primary Commo
-00001ec0: 6469 7479 2050 7269 6365 2053 7973 7465  dity Price Syste
-00001ed0: 6d3a 0a0a 0a60 6060 7079 7468 6f6e 0a64  m:...```python.d
-00001ee0: 6174 6162 6173 6573 5b64 6174 6162 6173  atabases[databas
-00001ef0: 6573 5b27 6465 7363 7269 7074 696f 6e27  es['description'
-00001f00: 5d2e 7374 722e 636f 6e74 6169 6e73 2822  ].str.contains("
-00001f10: 436f 6d6d 6f64 6974 7922 295d 0a60 6060  Commodity")].```
-00001f20: 0a0a 0a0a 0a3c 6469 763e 0a0a 3c74 6162  .....<div>..<tab
-00001f30: 6c65 2062 6f72 6465 723d 2231 2220 636c  le border="1" cl
-00001f40: 6173 733d 2264 6174 6166 7261 6d65 223e  ass="dataframe">
-00001f50: 0a20 203c 7468 6561 643e 0a20 2020 203c  .  <thead>.    <
-00001f60: 7472 2073 7479 6c65 3d22 7465 7874 2d61  tr style="text-a
-00001f70: 6c69 676e 3a20 7269 6768 743b 223e 0a20  lign: right;">. 
-00001f80: 2020 2020 203c 7468 3e3c 2f74 683e 0a20       <th></th>. 
-00001f90: 2020 2020 203c 7468 3e64 6174 6162 6173       <th>databas
-00001fa0: 655f 6964 3c2f 7468 3e0a 2020 2020 2020  e_id</th>.      
-00001fb0: 3c74 683e 6465 7363 7269 7074 696f 6e3c  <th>description<
-00001fc0: 2f74 683e 0a20 2020 203c 2f74 723e 0a20  /th>.    </tr>. 
-00001fd0: 203c 2f74 6865 6164 3e0a 2020 3c74 626f   </thead>.  <tbo
-00001fe0: 6479 3e0a 2020 2020 3c74 723e 0a20 2020  dy>.    <tr>.   
-00001ff0: 2020 203c 7468 3e32 3337 3c2f 7468 3e0a     <th>237</th>.
-00002000: 2020 2020 2020 3c74 643e 5043 544f 543c        <td>PCTOT<
-00002010: 2f74 643e 0a20 2020 2020 203c 7464 3e43  /td>.      <td>C
-00002020: 6f6d 6d6f 6469 7479 2054 6572 6d73 206f  ommodity Terms o
-00002030: 6620 5472 6164 653c 2f74 643e 0a20 2020  f Trade</td>.   
-00002040: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
-00002050: 2020 2020 2020 3c74 683e 3233 393c 2f74        <th>239</t
-00002060: 683e 0a20 2020 2020 203c 7464 3e50 4350  h>.      <td>PCP
-00002070: 533c 2f74 643e 0a20 2020 2020 203c 7464  S</td>.      <td
-00002080: 3e50 7269 6d61 7279 2043 6f6d 6d6f 6469  >Primary Commodi
-00002090: 7479 2050 7269 6365 2053 7973 7465 6d20  ty Price System 
-000020a0: 2850 4350 5329 3c2f 7464 3e0a 2020 2020  (PCPS)</td>.    
-000020b0: 3c2f 7472 3e0a 2020 3c2f 7462 6f64 793e  </tr>.  </tbody>
-000020c0: 0a3c 2f74 6162 6c65 3e0a 3c2f 6469 763e  .</table>.</div>
-000020d0: 0a0a 0a0a 2323 2320 4665 7463 6869 6e67  ....### Fetching
-000020e0: 2061 204c 6973 7420 6f66 2050 6172 616d   a List of Param
-000020f0: 6574 6572 7320 616e 6420 496e 7075 7420  eters and Input 
-00002100: 436f 6465 7320 7769 7468 2069 6d66 5f70  Codes with imf_p
-00002110: 6172 616d 6574 6572 7320 616e 6420 696d  arameters and im
-00002120: 665f 7061 7261 6d65 7465 725f 6465 6673  f_parameter_defs
-00002130: 0a0a 4f6e 6365 2079 6f75 2068 6176 6520  ..Once you have 
-00002140: 6120 6064 6174 6162 6173 655f 6964 602c  a `database_id`,
-00002150: 2069 74e2 8099 7320 706f 7373 6962 6c65   it...s possible
-00002160: 2074 6f20 6d61 6b65 2061 2063 616c 6c20   to make a call 
-00002170: 746f 2060 696d 6670 2e69 6d66 5f64 6174  to `imfp.imf_dat
-00002180: 6173 6574 6020 746f 2066 6574 6368 2074  aset` to fetch t
-00002190: 6865 2065 6e74 6972 6520 6461 7461 6261  he entire databa
-000021a0: 7365 3a20 6069 6d66 702e 696d 665f 6461  se: `imfp.imf_da
-000021b0: 7461 7365 7428 6461 7461 6261 7365 5f69  taset(database_i
-000021c0: 6429 602e 2048 6f77 6576 6572 2c20 7768  d)`. However, wh
-000021d0: 696c 6520 7468 6973 2077 696c 6c20 7375  ile this will su
-000021e0: 6363 6565 6420 666f 7220 6120 6665 7720  cceed for a few 
-000021f0: 736d 616c 6c20 6461 7461 6261 7365 732c  small databases,
-00002200: 2069 7420 7769 6c6c 2066 6169 6c20 666f   it will fail fo
-00002210: 7220 616c 6c20 6f66 2074 6865 206c 6172  r all of the lar
-00002220: 6765 7220 6f6e 6573 2e20 416e 6420 6576  ger ones. And ev
-00002230: 656e 2069 6e20 7468 6520 7261 7265 2063  en in the rare c
-00002240: 6173 6520 7768 656e 2069 7420 7375 6363  ase when it succ
-00002250: 6565 6473 2c20 6665 7463 6869 6e67 2061  eeds, fetching a
-00002260: 6e20 656e 7469 7265 2064 6174 6162 6173  n entire databas
-00002270: 6520 6361 6e20 7461 6b65 2061 206c 6f6e  e can take a lon
-00002280: 6720 7469 6d65 2e20 596f 75e2 8099 7265  g time. You...re
-00002290: 206d 7563 6820 6265 7474 6572 206f 6666   much better off
-000022a0: 2073 7570 706c 7969 6e67 2061 6464 6974   supplying addit
-000022b0: 696f 6e61 6c20 6669 6c74 6572 2070 6172  ional filter par
-000022c0: 616d 6574 6572 7320 746f 2072 6564 7563  ameters to reduc
-000022d0: 6520 7468 6520 7369 7a65 206f 6620 796f  e the size of yo
-000022e0: 7572 2072 6571 7565 7374 2e0a 0a52 6571  ur request...Req
-000022f0: 7565 7374 7320 746f 2064 6174 6162 6173  uests to databas
-00002300: 6573 2061 7661 696c 6162 6c65 2074 6872  es available thr
-00002310: 6f75 6768 2074 6865 2049 4d46 2041 5049  ough the IMF API
-00002320: 2061 7265 2063 6f6d 706c 6963 6174 6564   are complicated
-00002330: 2062 7920 7468 6520 6661 6374 2074 6861   by the fact tha
-00002340: 7420 6561 6368 2064 6174 6162 6173 6520  t each database 
-00002350: 7573 6573 2061 2064 6966 6665 7265 6e74  uses a different
-00002360: 2073 6574 206f 6620 7061 7261 6d65 7465   set of paramete
-00002370: 7273 2077 6865 6e20 6d61 6b69 6e67 2061  rs when making a
-00002380: 2072 6571 7565 7374 2e20 2841 7420 6c61   request. (At la
-00002390: 7374 2063 6f75 6e74 2c20 7468 6572 6520  st count, there 
-000023a0: 7765 7265 2034 3320 756e 6971 7565 2070  were 43 unique p
-000023b0: 6172 616d 6574 6572 7320 7573 6564 2069  arameters used i
-000023c0: 6e20 6d61 6b69 6e67 2041 5049 2072 6571  n making API req
-000023d0: 7565 7374 7320 6672 6f6d 2074 6865 2076  uests from the v
-000023e0: 6172 696f 7573 2064 6174 6162 6173 6573  arious databases
-000023f0: 2129 2059 6f75 2061 6c73 6f20 6861 7665  !) You also have
-00002400: 2074 6f20 6861 7665 2074 6865 206c 6973   to have the lis
-00002410: 7420 6f66 2076 616c 6964 2069 6e70 7574  t of valid input
-00002420: 2063 6f64 6573 2066 6f72 2065 6163 6820   codes for each 
-00002430: 7061 7261 6d65 7465 722e 2054 6865 2060  parameter. The `
-00002440: 696d 6670 2e69 6d66 5f70 6172 616d 6574  imfp.imf_paramet
-00002450: 6572 7360 2066 756e 6374 696f 6e20 736f  ers` function so
-00002460: 6c76 6573 2074 6869 7320 7072 6f62 6c65  lves this proble
-00002470: 6d2e 2055 7365 2074 6865 2066 756e 6374  m. Use the funct
-00002480: 696f 6e20 746f 206f 6274 6169 6e20 7468  ion to obtain th
-00002490: 6520 6675 6c6c 206c 6973 7420 6f66 2070  e full list of p
-000024a0: 6172 616d 6574 6572 7320 616e 6420 7661  arameters and va
-000024b0: 6c69 6420 696e 7075 7420 636f 6465 7320  lid input codes 
-000024c0: 666f 7220 6120 6769 7665 6e20 6461 7461  for a given data
-000024d0: 6261 7365 3a0a 0a0a 6060 6070 7974 686f  base:...```pytho
-000024e0: 6e0a 2320 4665 7463 6820 6c69 7374 206f  n.# Fetch list o
-000024f0: 6620 7661 6c69 6420 7061 7261 6d65 7465  f valid paramete
-00002500: 7273 2061 6e64 2069 6e70 7574 2063 6f64  rs and input cod
-00002510: 6573 2066 6f72 2063 6f6d 6d6f 6469 7479  es for commodity
-00002520: 2070 7269 6365 2064 6174 6162 6173 650a   price database.
-00002530: 7061 7261 6d73 203d 2069 6d66 702e 696d  params = imfp.im
-00002540: 665f 7061 7261 6d65 7465 7273 2822 5043  f_parameters("PC
-00002550: 5053 2229 0a60 6060 0a0a 5468 6520 6069  PS").```..The `i
-00002560: 6d66 702e 696d 665f 7061 7261 6d65 7465  mfp.imf_paramete
-00002570: 7273 6020 6675 6e63 7469 6f6e 2072 6574  rs` function ret
-00002580: 7572 6e73 2061 2064 6963 7469 6f6e 6172  urns a dictionar
-00002590: 7920 6f66 2064 6174 6120 6672 616d 6573  y of data frames
-000025a0: 2e20 4561 6368 2064 6963 7469 6f6e 6172  . Each dictionar
-000025b0: 7920 6b65 7920 6e61 6d65 2063 6f72 7265  y key name corre
-000025c0: 7370 6f6e 6473 2074 6f20 6120 7061 7261  sponds to a para
-000025d0: 6d65 7465 7220 7573 6564 2069 6e20 6d61  meter used in ma
-000025e0: 6b69 6e67 2072 6571 7565 7374 7320 6672  king requests fr
-000025f0: 6f6d 2074 6865 2064 6174 6162 6173 653a  om the database:
-00002600: 0a0a 0a60 6060 7079 7468 6f6e 0a23 2047  ...```python.# G
-00002610: 6574 206b 6579 206e 616d 6573 2066 726f  et key names fro
-00002620: 6d20 7468 6520 7061 7261 6d73 206f 626a  m the params obj
-00002630: 6563 740a 7061 7261 6d73 2e6b 6579 7328  ect.params.keys(
-00002640: 290a 6060 600a 0a0a 0a0a 2020 2020 6469  ).```.....    di
-00002650: 6374 5f6b 6579 7328 5b27 6672 6571 272c  ct_keys(['freq',
-00002660: 2027 7265 665f 6172 6561 272c 2027 636f   'ref_area', 'co
-00002670: 6d6d 6f64 6974 7927 2c20 2775 6e69 745f  mmodity', 'unit_
-00002680: 6d65 6173 7572 6527 5d29 0a0a 0a0a 496e  measure'])....In
-00002690: 2074 6865 2065 7665 6e74 2074 6861 7420   the event that 
-000026a0: 6120 7061 7261 6d65 7465 7220 6e61 6d65  a parameter name
-000026b0: 2069 7320 6e6f 7420 7365 6c66 2d65 7870   is not self-exp
-000026c0: 6c61 6e61 746f 7279 2c20 7468 6520 6069  lanatory, the `i
-000026d0: 6d66 702e 696d 665f 7061 7261 6d65 7465  mfp.imf_paramete
-000026e0: 725f 6465 6673 6020 6675 6e63 7469 6f6e  r_defs` function
-000026f0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00002700: 6665 7463 6820 7368 6f72 7420 7465 7874  fetch short text
-00002710: 2064 6573 6372 6970 7469 6f6e 7320 6f66   descriptions of
-00002720: 2065 6163 6820 7061 7261 6d65 7465 723a   each parameter:
-00002730: 0a0a 0a60 6060 7079 7468 6f6e 0a23 2046  ...```python.# F
-00002740: 6574 6368 2061 6e64 2064 6973 706c 6179  etch and display
-00002750: 2070 6172 616d 6574 6572 2074 6578 7420   parameter text 
-00002760: 6465 7363 7269 7074 696f 6e73 2066 6f72  descriptions for
-00002770: 2074 6865 2063 6f6d 6d6f 6469 7479 2070   the commodity p
-00002780: 7269 6365 2064 6174 6162 6173 650a 696d  rice database.im
-00002790: 6670 2e69 6d66 5f70 6172 616d 6574 6572  fp.imf_parameter
-000027a0: 5f64 6566 7328 2250 4350 5322 290a 6060  _defs("PCPS").``
-000027b0: 600a 0a0a 0a0a 3c64 6976 3e0a 0a3c 7461  `.....<div>..<ta
-000027c0: 626c 6520 626f 7264 6572 3d22 3122 2063  ble border="1" c
-000027d0: 6c61 7373 3d22 6461 7461 6672 616d 6522  lass="dataframe"
-000027e0: 3e0a 2020 3c74 6865 6164 3e0a 2020 2020  >.  <thead>.    
-000027f0: 3c74 7220 7374 796c 653d 2274 6578 742d  <tr style="text-
-00002800: 616c 6967 6e3a 2072 6967 6874 3b22 3e0a  align: right;">.
-00002810: 2020 2020 2020 3c74 683e 3c2f 7468 3e0a        <th></th>.
-00002820: 2020 2020 2020 3c74 683e 7061 7261 6d65        <th>parame
-00002830: 7465 723c 2f74 683e 0a20 2020 2020 203c  ter</th>.      <
-00002840: 7468 3e64 6573 6372 6970 7469 6f6e 3c2f  th>description</
-00002850: 7468 3e0a 2020 2020 3c2f 7472 3e0a 2020  th>.    </tr>.  
-00002860: 3c2f 7468 6561 643e 0a20 203c 7462 6f64  </thead>.  <tbod
-00002870: 793e 0a20 2020 203c 7472 3e0a 2020 2020  y>.    <tr>.    
-00002880: 2020 3c74 683e 303c 2f74 683e 0a20 2020    <th>0</th>.   
-00002890: 2020 203c 7464 3e66 7265 713c 2f74 643e     <td>freq</td>
-000028a0: 0a20 2020 2020 203c 7464 3e46 7265 7175  .      <td>Frequ
-000028b0: 656e 6379 3c2f 7464 3e0a 2020 2020 3c2f  ency</td>.    </
-000028c0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
-000028d0: 2020 203c 7468 3e31 3c2f 7468 3e0a 2020     <th>1</th>.  
-000028e0: 2020 2020 3c74 643e 7265 665f 6172 6561      <td>ref_area
-000028f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-00002900: 4765 6f67 7261 7068 6963 616c 2041 7265  Geographical Are
-00002910: 6173 3c2f 7464 3e0a 2020 2020 3c2f 7472  as</td>.    </tr
-00002920: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00002930: 203c 7468 3e32 3c2f 7468 3e0a 2020 2020   <th>2</th>.    
-00002940: 2020 3c74 643e 636f 6d6d 6f64 6974 793c    <td>commodity<
-00002950: 2f74 643e 0a20 2020 2020 203c 7464 3e49  /td>.      <td>I
-00002960: 6e64 6963 6174 6f72 3c2f 7464 3e0a 2020  ndicator</td>.  
-00002970: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00002980: 0a20 2020 2020 203c 7468 3e33 3c2f 7468  .      <th>3</th
-00002990: 3e0a 2020 2020 2020 3c74 643e 756e 6974  >.      <td>unit
-000029a0: 5f6d 6561 7375 7265 3c2f 7464 3e0a 2020  _measure</td>.  
-000029b0: 2020 2020 3c74 643e 556e 6974 3c2f 7464      <td>Unit</td
-000029c0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 3c2f  >.    </tr>.  </
-000029d0: 7462 6f64 793e 0a3c 2f74 6162 6c65 3e0a  tbody>.</table>.
-000029e0: 3c2f 6469 763e 0a0a 0a0a 4561 6368 206e  </div>....Each n
-000029f0: 616d 6564 206c 6973 7420 6974 656d 2069  amed list item i
-00002a00: 7320 6120 6461 7461 2066 7261 6d65 2063  s a data frame c
-00002a10: 6f6e 7461 696e 696e 6720 6120 7665 6374  ontaining a vect
-00002a20: 6f72 206f 6620 7661 6c69 6420 696e 7075  or of valid inpu
-00002a30: 7420 636f 6465 7320 7468 6174 2063 616e  t codes that can
-00002a40: 2062 6520 7573 6564 2077 6974 6820 7468   be used with th
-00002a50: 6520 6e61 6d65 6420 7061 7261 6d65 7465  e named paramete
-00002a60: 722c 2061 6e64 2061 2076 6563 746f 7220  r, and a vector 
-00002a70: 6f66 2074 6578 7420 6465 7363 7269 7074  of text descript
-00002a80: 696f 6e73 206f 6620 7768 6174 2065 6163  ions of what eac
-00002a90: 6820 636f 6465 2072 6570 7265 7365 6e74  h code represent
-00002aa0: 732e 0a0a 546f 2061 6363 6573 7320 7468  s...To access th
-00002ab0: 6520 6461 7461 2066 7261 6d65 2063 6f6e  e data frame con
-00002ac0: 7461 696e 696e 6720 7661 6c69 6420 7661  taining valid va
-00002ad0: 6c75 6573 2066 6f72 2065 6163 6820 7061  lues for each pa
-00002ae0: 7261 6d65 7465 722c 2073 7562 7365 7420  rameter, subset 
-00002af0: 7468 6520 6070 6172 616d 7360 2064 6963  the `params` dic
-00002b00: 7420 6279 2074 6865 2070 6172 616d 6574  t by the paramet
-00002b10: 6572 206e 616d 653a 0a0a 0a60 6060 7079  er name:...```py
-00002b20: 7468 6f6e 0a23 2056 6965 7720 7468 6520  thon.# View the 
-00002b30: 6461 7461 2066 7261 6d65 206f 6620 7661  data frame of va
-00002b40: 6c69 6420 696e 7075 7420 636f 6465 7320  lid input codes 
-00002b50: 666f 7220 7468 6520 6672 6571 7565 6e63  for the frequenc
-00002b60: 7920 7061 7261 6d65 7465 720a 7061 7261  y parameter.para
-00002b70: 6d73 5b27 6672 6571 275d 0a60 6060 0a0a  ms['freq'].```..
-00002b80: 0a0a 0a3c 6469 763e 0a0a 3c74 6162 6c65  ...<div>..<table
-00002b90: 2062 6f72 6465 723d 2231 2220 636c 6173   border="1" clas
-00002ba0: 733d 2264 6174 6166 7261 6d65 223e 0a20  s="dataframe">. 
-00002bb0: 203c 7468 6561 643e 0a20 2020 203c 7472   <thead>.    <tr
-00002bc0: 2073 7479 6c65 3d22 7465 7874 2d61 6c69   style="text-ali
-00002bd0: 676e 3a20 7269 6768 743b 223e 0a20 2020  gn: right;">.   
-00002be0: 2020 203c 7468 3e3c 2f74 683e 0a20 2020     <th></th>.   
-00002bf0: 2020 203c 7468 3e69 6e70 7574 5f63 6f64     <th>input_cod
-00002c00: 653c 2f74 683e 0a20 2020 2020 203c 7468  e</th>.      <th
-00002c10: 3e64 6573 6372 6970 7469 6f6e 3c2f 7468  >description</th
-00002c20: 3e0a 2020 2020 3c2f 7472 3e0a 2020 3c2f  >.    </tr>.  </
-00002c30: 7468 6561 643e 0a20 203c 7462 6f64 793e  thead>.  <tbody>
-00002c40: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
-00002c50: 3c74 683e 303c 2f74 683e 0a20 2020 2020  <th>0</th>.     
-00002c60: 203c 7464 3e41 3c2f 7464 3e0a 2020 2020   <td>A</td>.    
-00002c70: 2020 3c74 643e 416e 6e75 616c 3c2f 7464    <td>Annual</td
-00002c80: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
-00002c90: 3c74 723e 0a20 2020 2020 203c 7468 3e31  <tr>.      <th>1
-00002ca0: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
-00002cb0: 4d3c 2f74 643e 0a20 2020 2020 203c 7464  M</td>.      <td
-00002cc0: 3e4d 6f6e 7468 6c79 3c2f 7464 3e0a 2020  >Monthly</td>.  
-00002cd0: 2020 3c2f 7472 3e0a 2020 2020 3c74 723e    </tr>.    <tr>
-00002ce0: 0a20 2020 2020 203c 7468 3e32 3c2f 7468  .      <th>2</th
-00002cf0: 3e0a 2020 2020 2020 3c74 643e 513c 2f74  >.      <td>Q</t
-00002d00: 643e 0a20 2020 2020 203c 7464 3e51 7561  d>.      <td>Qua
-00002d10: 7274 6572 6c79 3c2f 7464 3e0a 2020 2020  rterly</td>.    
-00002d20: 3c2f 7472 3e0a 2020 3c2f 7462 6f64 793e  </tr>.  </tbody>
-00002d30: 0a3c 2f74 6162 6c65 3e0a 3c2f 6469 763e  .</table>.</div>
-00002d40: 0a0a 0a0a 2323 2320 5669 6577 696e 6720  ....### Viewing 
-00002d50: 4461 7461 2046 7261 6d65 730a 0a4e 6f74  Data Frames..Not
-00002d60: 6520 7468 6174 2060 7061 6e64 6173 6020  e that `pandas` 
-00002d70: 6461 7461 2066 7261 6d65 7320 696e 2050  data frames in P
-00002d80: 7974 686f 6e20 6361 6e20 6265 2061 206c  ython can be a l
-00002d90: 6974 746c 6520 6469 6666 6963 756c 7420  ittle difficult 
-00002da0: 746f 2077 6f72 6b20 7769 7468 2c20 6265  to work with, be
-00002db0: 6361 7573 6520 5079 7468 6f6e 2064 6f65  cause Python doe
-00002dc0: 736e 2774 2068 6176 6520 6120 6275 696c  sn't have a buil
-00002dd0: 742d 696e 2076 6172 6961 626c 6520 6578  t-in variable ex
-00002de0: 706c 6f72 6572 2e20 4966 2079 6f75 2772  plorer. If you'r
-00002df0: 6520 646f 696e 6720 6461 7461 2073 6369  e doing data sci
-00002e00: 656e 6365 2c20 4920 7265 636f 6d6d 656e  ence, I recommen
-00002e10: 6420 7573 696e 6720 616e 2049 4445 206c  d using an IDE l
-00002e20: 696b 6520 5253 7475 6469 6f20 6f72 2053  ike RStudio or S
-00002e30: 7079 6465 7220 7468 6174 2068 6173 2061  pyder that has a
-00002e40: 2062 7569 6c74 2d69 6e20 7661 7269 6162   built-in variab
-00002e50: 6c65 2065 7870 6c6f 7265 722e 2048 6f77  le explorer. How
-00002e60: 6576 6572 2c20 6966 2079 6f75 2064 6f6e  ever, if you don
-00002e70: 2774 2068 6176 6520 6120 7661 7269 6162  't have a variab
-00002e80: 6c65 2065 7870 6c6f 7265 722c 2079 6f75  le explorer, you
-00002e90: 2063 616e 2070 7265 7665 6e74 2050 7974   can prevent Pyt
-00002ea0: 686f 6e20 6672 6f6d 2074 7275 6e63 6174  hon from truncat
-00002eb0: 696e 6720 6461 7461 2066 7261 6d65 7320  ing data frames 
-00002ec0: 7573 696e 6720 7468 6520 606f 7074 696f  using the `optio
-00002ed0: 6e73 6020 696e 2060 7061 6e64 6173 602e  ns` in `pandas`.
-00002ee0: 2046 6f72 2069 6e73 7461 6e63 652c 2074   For instance, t
-00002ef0: 6f20 696e 6372 6561 7365 2074 6865 206d  o increase the m
-00002f00: 6178 696d 756d 2061 6c6c 6f77 6564 2063  aximum allowed c
-00002f10: 6f6c 756d 6e20 7769 6474 6820 746f 2031  olumn width to 1
-00002f20: 3030 2063 6861 7261 6374 6572 732c 2077  00 characters, w
-00002f30: 6520 6361 6e20 7573 6520 6070 616e 6461  e can use `panda
-00002f40: 732e 6f70 7469 6f6e 732e 6469 7370 6c61  s.options.displa
-00002f50: 792e 6d61 785f 636f 6c77 6964 7468 203d  y.max_colwidth =
-00002f60: 2031 3030 602e 0a0a 416c 7465 726e 6174   100`...Alternat
-00002f70: 6976 656c 792c 2069 7427 7320 706f 7373  ively, it's poss
-00002f80: 6962 6c65 2074 6f20 6f70 656e 2074 6865  ible to open the
-00002f90: 2064 6174 6120 6672 616d 6520 696e 2061   data frame in a
-00002fa0: 206e 6577 2077 696e 646f 7720 746f 2076   new window to v
-00002fb0: 6965 7720 6974 2069 6e20 6675 6c6c 3a0a  iew it in full:.
-00002fc0: 0a0a 6060 6070 7974 686f 6e0a 696d 706f  ..```python.impo
-00002fd0: 7274 2069 6d66 700a 696d 706f 7274 2074  rt imfp.import t
-00002fe0: 656d 7066 696c 650a 696d 706f 7274 2077  empfile.import w
-00002ff0: 6562 6272 6f77 7365 720a 0a23 2044 6566  ebbrowser..# Def
-00003000: 696e 6520 6120 7369 6d70 6c65 2066 756e  ine a simple fun
-00003010: 6374 696f 6e20 746f 2076 6965 7720 6461  ction to view da
-00003020: 7461 2066 7261 6d65 2069 6e20 6120 6272  ta frame in a br
-00003030: 6f77 7365 7220 7769 6e64 6f77 0a64 6566  owser window.def
-00003040: 2056 6965 7728 6466 293a 0a20 2020 2068   View(df):.    h
-00003050: 746d 6c20 3d20 6466 2e74 6f5f 6874 6d6c  tml = df.to_html
-00003060: 2829 0a20 2020 2077 6974 6820 7465 6d70  ().    with temp
-00003070: 6669 6c65 2e4e 616d 6564 5465 6d70 6f72  file.NamedTempor
-00003080: 6172 7946 696c 6528 2777 272c 2064 656c  aryFile('w', del
-00003090: 6574 653d 4661 6c73 652c 2073 7566 6669  ete=False, suffi
-000030a0: 783d 272e 6874 6d6c 2729 2061 7320 663a  x='.html') as f:
-000030b0: 0a20 2020 2020 2020 2075 726c 203d 2027  .        url = '
-000030c0: 6669 6c65 3a2f 2f27 202b 2066 2e6e 616d  file://' + f.nam
-000030d0: 650a 2020 2020 2020 2020 662e 7772 6974  e.        f.writ
-000030e0: 6528 6874 6d6c 290a 2020 2020 7765 6262  e(html).    webb
-000030f0: 726f 7773 6572 2e6f 7065 6e28 7572 6c29  rowser.open(url)
-00003100: 0a0a 2320 4f70 656e 2064 6174 6120 6672  ..# Open data fr
-00003110: 616d 6520 696e 2061 206e 6577 2062 726f  ame in a new bro
-00003120: 7773 6572 2077 696e 646f 7720 7573 696e  wser window usin
-00003130: 6720 7468 6520 6675 6e63 7469 6f6e 0a64  g the function.d
-00003140: 6620 3d20 696d 6670 2e69 6d66 5f64 6174  f = imfp.imf_dat
-00003150: 6162 6173 6573 2829 0a56 6965 7728 6466  abases().View(df
-00003160: 290a 6060 600a 0a23 2323 2053 7570 706c  ).```..### Suppl
-00003170: 7969 6e67 2050 6172 616d 6574 6572 2041  ying Parameter A
-00003180: 7267 756d 656e 7473 2074 6f20 696d 665f  rguments to imf_
-00003190: 6461 7461 7365 743a 2041 2054 616c 6520  dataset: A Tale 
-000031a0: 6f66 2054 776f 2057 6f72 6b66 6c6f 7773  of Two Workflows
-000031b0: 0a0a 5468 6572 6520 6172 6520 7477 6f20  ..There are two 
-000031c0: 7761 7973 2074 6f20 7375 7070 6c79 2070  ways to supply p
-000031d0: 6172 616d 6574 6572 7320 746f 2060 696d  arameters to `im
-000031e0: 6670 2e69 6d66 5f64 6174 6173 6574 603a  fp.imf_dataset`:
-000031f0: 2062 7920 7375 7070 6c79 696e 6720 6c69   by supplying li
-00003200: 7374 2061 7267 756d 656e 7473 206f 7220  st arguments or 
-00003210: 6279 2073 7570 706c 7969 6e67 2061 206d  by supplying a m
-00003220: 6f64 6966 6965 6420 7061 7261 6d65 7465  odified paramete
-00003230: 7273 2064 6963 742e 2054 6865 206c 6973  rs dict. The lis
-00003240: 7420 6172 6775 6d65 6e74 7320 776f 726b  t arguments work
-00003250: 666c 6f77 2077 696c 6c20 6265 206d 6f72  flow will be mor
-00003260: 6520 696e 7475 6974 6976 6520 666f 7220  e intuitive for 
-00003270: 6d6f 7374 2075 7365 7273 2c20 6275 7420  most users, but 
-00003280: 7468 6520 6469 6374 2061 7267 756d 656e  the dict argumen
-00003290: 7420 776f 726b 666c 6f77 2072 6571 7569  t workflow requi
-000032a0: 7265 7320 6120 6c69 7474 6c65 206c 6573  res a little les
-000032b0: 7320 636f 6465 2e0a 0a23 2323 2320 5468  s code...#### Th
-000032c0: 6520 4c69 7374 2041 7267 756d 656e 7473  e List Arguments
-000032d0: 2057 6f72 6b66 6c6f 770a 0a54 6f20 7375   Workflow..To su
-000032e0: 7070 6c79 206c 6973 7420 6172 6775 6d65  pply list argume
-000032f0: 6e74 732c 206a 7573 7420 6669 6e64 2074  nts, just find t
-00003300: 6865 2063 6f64 6573 2079 6f75 2077 616e  he codes you wan
-00003310: 7420 616e 6420 7375 7070 6c79 2074 6865  t and supply the
-00003320: 6d20 746f 2060 696d 6670 2e69 6d66 5f64  m to `imfp.imf_d
-00003330: 6174 6173 6574 6020 7573 696e 6720 7468  ataset` using th
-00003340: 6520 7061 7261 6d65 7465 7220 6e61 6d65  e parameter name
-00003350: 2061 7320 7468 6520 6172 6775 6d65 6e74   as the argument
-00003360: 206e 616d 652e 2054 6865 2065 7861 6d70   name. The examp
-00003370: 6c65 2062 656c 6f77 2073 686f 7773 2068  le below shows h
-00003380: 6f77 2074 6f20 7265 7175 6573 7420 3230  ow to request 20
-00003390: 3030 e280 9332 3031 3520 616e 6e75 616c  00...2015 annual
-000033a0: 2063 6f61 6c20 7072 6963 6573 2066 726f   coal prices fro
-000033b0: 6d20 7468 6520 5072 696d 6172 7920 436f  m the Primary Co
-000033c0: 6d6d 6f64 6974 7920 5072 6963 6520 5379  mmodity Price Sy
-000033d0: 7374 656d 2064 6174 6162 6173 653a 0a0a  stem database:..
-000033e0: 0a60 6060 7079 7468 6f6e 0a23 2046 6574  .```python.# Fet
-000033f0: 6368 2074 6865 2027 6672 6571 2720 696e  ch the 'freq' in
-00003400: 7075 7420 636f 6465 2066 6f72 2061 6e6e  put code for ann
-00003410: 7561 6c20 6672 6571 7565 6e63 790a 7365  ual frequency.se
-00003420: 6c65 6374 6564 5f66 7265 7120 3d20 6c69  lected_freq = li
-00003430: 7374 280a 2020 2020 7061 7261 6d73 5b27  st(.    params['
-00003440: 6672 6571 275d 5b27 696e 7075 745f 636f  freq']['input_co
-00003450: 6465 275d 5b70 6172 616d 735b 2766 7265  de'][params['fre
-00003460: 7127 5d5b 2764 6573 6372 6970 7469 6f6e  q']['description
-00003470: 275d 2e73 7472 2e63 6f6e 7461 696e 7328  '].str.contains(
-00003480: 2241 6e6e 7561 6c22 295d 0a29 0a0a 2320  "Annual")].)..# 
-00003490: 4665 7463 6820 7468 6520 2763 6f6d 6d6f  Fetch the 'commo
-000034a0: 6469 7479 2720 696e 7075 7420 636f 6465  dity' input code
-000034b0: 2066 6f72 2063 6f61 6c0a 7365 6c65 6374   for coal.select
-000034c0: 6564 5f63 6f6d 6d6f 6469 7479 203d 206c  ed_commodity = l
-000034d0: 6973 7428 0a20 2020 2070 6172 616d 735b  ist(.    params[
-000034e0: 2763 6f6d 6d6f 6469 7479 275d 5b27 696e  'commodity']['in
-000034f0: 7075 745f 636f 6465 275d 5b70 6172 616d  put_code'][param
-00003500: 735b 2763 6f6d 6d6f 6469 7479 275d 5b27  s['commodity']['
-00003510: 6465 7363 7269 7074 696f 6e27 5d2e 7374  description'].st
-00003520: 722e 636f 6e74 6169 6e73 2822 436f 616c  r.contains("Coal
-00003530: 2229 5d0a 290a 0a23 2046 6574 6368 2074  ")].)..# Fetch t
-00003540: 6865 2027 756e 6974 5f6d 6561 7375 7265  he 'unit_measure
-00003550: 2720 696e 7075 7420 636f 6465 2066 6f72  ' input code for
-00003560: 2069 6e64 6578 0a73 656c 6563 7465 645f   index.selected_
-00003570: 756e 6974 5f6d 6561 7375 7265 203d 206c  unit_measure = l
-00003580: 6973 7428 0a20 2020 2070 6172 616d 735b  ist(.    params[
-00003590: 2775 6e69 745f 6d65 6173 7572 6527 5d5b  'unit_measure'][
-000035a0: 2769 6e70 7574 5f63 6f64 6527 5d5b 7061  'input_code'][pa
-000035b0: 7261 6d73 5b27 756e 6974 5f6d 6561 7375  rams['unit_measu
-000035c0: 7265 275d 5b27 6465 7363 7269 7074 696f  re']['descriptio
-000035d0: 6e27 5d2e 7374 722e 636f 6e74 6169 6e73  n'].str.contains
-000035e0: 2822 496e 6465 7822 295d 0a29 0a0a 2320  ("Index")].)..# 
-000035f0: 5265 7175 6573 7420 6461 7461 2066 726f  Request data fro
-00003600: 6d20 7468 6520 4150 490a 6466 203d 2069  m the API.df = i
-00003610: 6d66 702e 696d 665f 6461 7461 7365 7428  mfp.imf_dataset(
-00003620: 6461 7461 6261 7365 5f69 6420 3d20 2250  database_id = "P
-00003630: 4350 5322 2c0a 2020 2020 2020 2020 2066  CPS",.         f
-00003640: 7265 7120 3d20 7365 6c65 6374 6564 5f66  req = selected_f
-00003650: 7265 712c 2063 6f6d 6d6f 6469 7479 203d  req, commodity =
-00003660: 2073 656c 6563 7465 645f 636f 6d6d 6f64   selected_commod
-00003670: 6974 792c 0a20 2020 2020 2020 2020 756e  ity,.         un
-00003680: 6974 5f6d 6561 7375 7265 203d 2073 656c  it_measure = sel
-00003690: 6563 7465 645f 756e 6974 5f6d 6561 7375  ected_unit_measu
-000036a0: 7265 2c0a 2020 2020 2020 2020 2073 7461  re,.         sta
-000036b0: 7274 5f79 6561 7220 3d20 3230 3030 2c20  rt_year = 2000, 
-000036c0: 656e 645f 7965 6172 203d 2032 3031 3529  end_year = 2015)
-000036d0: 0a0a 2320 4469 7370 6c61 7920 7468 6520  ..# Display the 
-000036e0: 6669 7273 7420 6665 7720 656e 7472 6965  first few entrie
-000036f0: 7320 696e 2074 6865 2072 6574 7269 6576  s in the retriev
-00003700: 6564 2064 6174 6120 6672 616d 650a 6466  ed data frame.df
-00003710: 2e68 6561 6428 290a 6060 600a 0a0a 0a0a  .head().```.....
-00003720: 3c64 6976 3e0a 0a3c 7461 626c 6520 626f  <div>..<table bo
-00003730: 7264 6572 3d22 3122 2063 6c61 7373 3d22  rder="1" class="
-00003740: 6461 7461 6672 616d 6522 3e0a 2020 3c74  dataframe">.  <t
-00003750: 6865 6164 3e0a 2020 2020 3c74 7220 7374  head>.    <tr st
-00003760: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
-00003770: 2072 6967 6874 3b22 3e0a 2020 2020 2020   right;">.      
-00003780: 3c74 683e 3c2f 7468 3e0a 2020 2020 2020  <th></th>.      
-00003790: 3c74 683e 6672 6571 3c2f 7468 3e0a 2020  <th>freq</th>.  
-000037a0: 2020 2020 3c74 683e 7265 665f 6172 6561      <th>ref_area
-000037b0: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
-000037c0: 636f 6d6d 6f64 6974 793c 2f74 683e 0a20  commodity</th>. 
-000037d0: 2020 2020 203c 7468 3e75 6e69 745f 6d65       <th>unit_me
-000037e0: 6173 7572 653c 2f74 683e 0a20 2020 2020  asure</th>.     
-000037f0: 203c 7468 3e75 6e69 745f 6d75 6c74 3c2f   <th>unit_mult</
-00003800: 7468 3e0a 2020 2020 2020 3c74 683e 7469  th>.      <th>ti
-00003810: 6d65 5f66 6f72 6d61 743c 2f74 683e 0a20  me_format</th>. 
-00003820: 2020 2020 203c 7468 3e74 696d 655f 7065       <th>time_pe
-00003830: 7269 6f64 3c2f 7468 3e0a 2020 2020 2020  riod</th>.      
-00003840: 3c74 683e 6f62 735f 7661 6c75 653c 2f74  <th>obs_value</t
-00003850: 683e 0a20 2020 203c 2f74 723e 0a20 203c  h>.    </tr>.  <
-00003860: 2f74 6865 6164 3e0a 2020 3c74 626f 6479  /thead>.  <tbody
-00003870: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
-00003880: 203c 7468 3e30 3c2f 7468 3e0a 2020 2020   <th>0</th>.    
-00003890: 2020 3c74 643e 413c 2f74 643e 0a20 2020    <td>A</td>.   
-000038a0: 2020 203c 7464 3e57 3030 3c2f 7464 3e0a     <td>W00</td>.
-000038b0: 2020 2020 2020 3c74 643e 5043 4f41 4c3c        <td>PCOAL<
-000038c0: 2f74 643e 0a20 2020 2020 203c 7464 3e49  /td>.      <td>I
-000038d0: 583c 2f74 643e 0a20 2020 2020 203c 7464  X</td>.      <td
-000038e0: 3e30 3c2f 7464 3e0a 2020 2020 2020 3c74  >0</td>.      <t
-000038f0: 643e 5031 593c 2f74 643e 0a20 2020 2020  d>P1Y</td>.     
-00003900: 203c 7464 3e32 3030 303c 2f74 643e 0a20   <td>2000</td>. 
-00003910: 2020 2020 203c 7464 3e33 392e 3335 3130       <td>39.3510
-00003920: 3233 3032 3933 3230 323c 2f74 643e 0a20  230293202</td>. 
-00003930: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-00003940: 3e0a 2020 2020 2020 3c74 683e 313c 2f74  >.      <th>1</t
-00003950: 683e 0a20 2020 2020 203c 7464 3e41 3c2f  h>.      <td>A</
-00003960: 7464 3e0a 2020 2020 2020 3c74 643e 5730  td>.      <td>W0
-00003970: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
-00003980: 3e50 434f 414c 3c2f 7464 3e0a 2020 2020  >PCOAL</td>.    
-00003990: 2020 3c74 643e 4958 3c2f 7464 3e0a 2020    <td>IX</td>.  
-000039a0: 2020 2020 3c74 643e 303c 2f74 643e 0a20      <td>0</td>. 
-000039b0: 2020 2020 203c 7464 3e50 3159 3c2f 7464       <td>P1Y</td
-000039c0: 3e0a 2020 2020 2020 3c74 643e 3230 3031  >.      <td>2001
-000039d0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-000039e0: 3439 2e33 3337 3835 3837 3238 3430 3339  49.3378587284039
-000039f0: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
-00003a00: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
-00003a10: 7468 3e32 3c2f 7468 3e0a 2020 2020 2020  th>2</th>.      
-00003a20: 3c74 643e 413c 2f74 643e 0a20 2020 2020  <td>A</td>.     
-00003a30: 203c 7464 3e57 3030 3c2f 7464 3e0a 2020   <td>W00</td>.  
-00003a40: 2020 2020 3c74 643e 5043 4f41 4c3c 2f74      <td>PCOAL</t
-00003a50: 643e 0a20 2020 2020 203c 7464 3e49 583c  d>.      <td>IX<
-00003a60: 2f74 643e 0a20 2020 2020 203c 7464 3e30  /td>.      <td>0
-00003a70: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-00003a80: 5031 593c 2f74 643e 0a20 2020 2020 203c  P1Y</td>.      <
-00003a90: 7464 3e32 3030 323c 2f74 643e 0a20 2020  td>2002</td>.   
-00003aa0: 2020 203c 7464 3e33 392e 3439 3439 3039     <td>39.494909
-00003ab0: 3136 3438 3030 363c 2f74 643e 0a20 2020  1648006</td>.   
-00003ac0: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
-00003ad0: 2020 2020 2020 3c74 683e 333c 2f74 683e        <th>3</th>
-00003ae0: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
-00003af0: 3e0a 2020 2020 2020 3c74 643e 5730 303c  >.      <td>W00<
-00003b00: 2f74 643e 0a20 2020 2020 203c 7464 3e50  /td>.      <td>P
-00003b10: 434f 414c 3c2f 7464 3e0a 2020 2020 2020  COAL</td>.      
-00003b20: 3c74 643e 4958 3c2f 7464 3e0a 2020 2020  <td>IX</td>.    
-00003b30: 2020 3c74 643e 303c 2f74 643e 0a20 2020    <td>0</td>.   
-00003b40: 2020 203c 7464 3e50 3159 3c2f 7464 3e0a     <td>P1Y</td>.
-00003b50: 2020 2020 2020 3c74 643e 3230 3033 3c2f        <td>2003</
-00003b60: 7464 3e0a 2020 2020 2020 3c74 643e 3433  td>.      <td>43
-00003b70: 2e32 3837 3838 3736 3935 3037 3838 3c2f  .2878876950788</
-00003b80: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
-00003b90: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
-00003ba0: 3e34 3c2f 7468 3e0a 2020 2020 2020 3c74  >4</th>.      <t
-00003bb0: 643e 413c 2f74 643e 0a20 2020 2020 203c  d>A</td>.      <
-00003bc0: 7464 3e57 3030 3c2f 7464 3e0a 2020 2020  td>W00</td>.    
-00003bd0: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
-00003be0: 0a20 2020 2020 203c 7464 3e49 583c 2f74  .      <td>IX</t
-00003bf0: 643e 0a20 2020 2020 203c 7464 3e30 3c2f  d>.      <td>0</
-00003c00: 7464 3e0a 2020 2020 2020 3c74 643e 5031  td>.      <td>P1
-00003c10: 593c 2f74 643e 0a20 2020 2020 203c 7464  Y</td>.      <td
-00003c20: 3e32 3030 343c 2f74 643e 0a20 2020 2020  >2004</td>.     
-00003c30: 203c 7464 3e38 322e 3931 3835 3835 3830   <td>82.91858580
-00003c40: 3532 3836 323c 2f74 643e 0a20 2020 203c  52862</td>.    <
-00003c50: 2f74 723e 0a20 203c 2f74 626f 6479 3e0a  /tr>.  </tbody>.
-00003c60: 3c2f 7461 626c 653e 0a3c 2f64 6976 3e0a  </table>.</div>.
-00003c70: 0a0a 0a23 2323 2320 5468 6520 5061 7261  ...#### The Para
-00003c80: 6d65 7465 7273 2041 7267 756d 656e 7420  meters Argument 
-00003c90: 576f 726b 666c 6f77 0a0a 546f 2073 7570  Workflow..To sup
-00003ca0: 706c 7920 6120 6c69 7374 206f 626a 6563  ply a list objec
-00003cb0: 742c 206d 6f64 6966 7920 6561 6368 2064  t, modify each d
-00003cc0: 6174 6120 6672 616d 6520 696e 2074 6865  ata frame in the
-00003cd0: 2060 7061 7261 6d73 6020 6c69 7374 206f   `params` list o
-00003ce0: 626a 6563 7420 746f 2072 6574 6169 6e20  bject to retain 
-00003cf0: 6f6e 6c79 2074 6865 2072 6f77 7320 796f  only the rows yo
-00003d00: 7520 7761 6e74 2c20 616e 6420 7468 656e  u want, and then
-00003d10: 2073 7570 706c 7920 7468 6520 6d6f 6469   supply the modi
-00003d20: 6669 6564 206c 6973 7420 6f62 6a65 6374  fied list object
-00003d30: 2074 6f20 6069 6d66 702e 696d 665f 6461   to `imfp.imf_da
-00003d40: 7461 7365 7460 2061 7320 6974 7320 7061  taset` as its pa
-00003d50: 7261 6d65 7465 7273 2061 7267 756d 656e  rameters argumen
-00003d60: 742e 2048 6572 6520 6973 2068 6f77 2074  t. Here is how t
-00003d70: 6f20 6d61 6b65 2074 6865 2073 616d 6520  o make the same 
-00003d80: 7265 7175 6573 7420 666f 7220 616e 6e75  request for annu
-00003d90: 616c 2063 6f61 6c20 7072 6963 6520 6461  al coal price da
-00003da0: 7461 2075 7369 6e67 2061 2070 6172 616d  ta using a param
-00003db0: 6574 6572 7320 6c69 7374 3a0a 0a0a 6060  eters list:...``
-00003dc0: 6070 7974 686f 6e0a 2320 4665 7463 6820  `python.# Fetch 
-00003dd0: 7468 6520 2766 7265 7127 2069 6e70 7574  the 'freq' input
-00003de0: 2063 6f64 6520 666f 7220 616e 6e75 616c   code for annual
-00003df0: 2066 7265 7175 656e 6379 0a70 6172 616d   frequency.param
-00003e00: 735b 2766 7265 7127 5d20 3d20 7061 7261  s['freq'] = para
-00003e10: 6d73 5b27 6672 6571 275d 5b70 6172 616d  ms['freq'][param
-00003e20: 735b 2766 7265 7127 5d5b 2764 6573 6372  s['freq']['descr
-00003e30: 6970 7469 6f6e 275d 2e73 7472 2e63 6f6e  iption'].str.con
-00003e40: 7461 696e 7328 2241 6e6e 7561 6c22 295d  tains("Annual")]
-00003e50: 0a0a 2320 4665 7463 6820 7468 6520 2763  ..# Fetch the 'c
-00003e60: 6f6d 6d6f 6469 7479 2720 696e 7075 7420  ommodity' input 
-00003e70: 636f 6465 2873 2920 666f 7220 636f 616c  code(s) for coal
-00003e80: 0a70 6172 616d 735b 2763 6f6d 6d6f 6469  .params['commodi
-00003e90: 7479 275d 203d 2070 6172 616d 735b 2763  ty'] = params['c
-00003ea0: 6f6d 6d6f 6469 7479 275d 5b70 6172 616d  ommodity'][param
-00003eb0: 735b 2763 6f6d 6d6f 6469 7479 275d 5b27  s['commodity']['
-00003ec0: 6465 7363 7269 7074 696f 6e27 5d2e 7374  description'].st
-00003ed0: 722e 636f 6e74 6169 6e73 2822 436f 616c  r.contains("Coal
-00003ee0: 2229 5d0a 0a23 2046 6574 6368 2074 6865  ")]..# Fetch the
-00003ef0: 2027 756e 6974 5f6d 6561 7375 7265 2720   'unit_measure' 
-00003f00: 696e 7075 7420 636f 6465 2066 6f72 2069  input code for i
-00003f10: 6e64 6578 0a70 6172 616d 735b 2775 6e69  ndex.params['uni
-00003f20: 745f 6d65 6173 7572 6527 5d20 3d20 7061  t_measure'] = pa
-00003f30: 7261 6d73 5b27 756e 6974 5f6d 6561 7375  rams['unit_measu
-00003f40: 7265 275d 5b70 6172 616d 735b 2775 6e69  re'][params['uni
-00003f50: 745f 6d65 6173 7572 6527 5d5b 2764 6573  t_measure']['des
-00003f60: 6372 6970 7469 6f6e 275d 2e73 7472 2e63  cription'].str.c
-00003f70: 6f6e 7461 696e 7328 2249 6e64 6578 2229  ontains("Index")
-00003f80: 5d0a 0a23 2052 6571 7565 7374 2064 6174  ]..# Request dat
-00003f90: 6120 6672 6f6d 2074 6865 2041 5049 0a64  a from the API.d
-00003fa0: 6620 3d20 696d 6670 2e69 6d66 5f64 6174  f = imfp.imf_dat
-00003fb0: 6173 6574 2864 6174 6162 6173 655f 6964  aset(database_id
-00003fc0: 203d 2022 5043 5053 222c 0a20 2020 2020   = "PCPS",.     
-00003fd0: 2020 2020 7061 7261 6d65 7465 7273 203d      parameters =
-00003fe0: 2070 6172 616d 732c 0a20 2020 2020 2020   params,.       
-00003ff0: 2020 7374 6172 745f 7965 6172 203d 2032    start_year = 2
-00004000: 3030 302c 2065 6e64 5f79 6561 7220 3d20  000, end_year = 
-00004010: 3230 3135 290a 0a23 2044 6973 706c 6179  2015)..# Display
-00004020: 2074 6865 2066 6972 7374 2066 6577 2065   the first few e
-00004030: 6e74 7269 6573 2069 6e20 7468 6520 7265  ntries in the re
-00004040: 7472 6965 7665 6420 6461 7461 2066 7261  trieved data fra
-00004050: 6d65 0a64 662e 6865 6164 2829 0a60 6060  me.df.head().```
-00004060: 0a0a 0a0a 0a3c 6469 763e 0a0a 3c74 6162  .....<div>..<tab
-00004070: 6c65 2062 6f72 6465 723d 2231 2220 636c  le border="1" cl
-00004080: 6173 733d 2264 6174 6166 7261 6d65 223e  ass="dataframe">
-00004090: 0a20 203c 7468 6561 643e 0a20 2020 203c  .  <thead>.    <
-000040a0: 7472 2073 7479 6c65 3d22 7465 7874 2d61  tr style="text-a
-000040b0: 6c69 676e 3a20 7269 6768 743b 223e 0a20  lign: right;">. 
-000040c0: 2020 2020 203c 7468 3e3c 2f74 683e 0a20       <th></th>. 
-000040d0: 2020 2020 203c 7468 3e66 7265 713c 2f74       <th>freq</t
-000040e0: 683e 0a20 2020 2020 203c 7468 3e72 6566  h>.      <th>ref
-000040f0: 5f61 7265 613c 2f74 683e 0a20 2020 2020  _area</th>.     
-00004100: 203c 7468 3e63 6f6d 6d6f 6469 7479 3c2f   <th>commodity</
-00004110: 7468 3e0a 2020 2020 2020 3c74 683e 756e  th>.      <th>un
-00004120: 6974 5f6d 6561 7375 7265 3c2f 7468 3e0a  it_measure</th>.
-00004130: 2020 2020 2020 3c74 683e 756e 6974 5f6d        <th>unit_m
-00004140: 756c 743c 2f74 683e 0a20 2020 2020 203c  ult</th>.      <
-00004150: 7468 3e74 696d 655f 666f 726d 6174 3c2f  th>time_format</
-00004160: 7468 3e0a 2020 2020 2020 3c74 683e 7469  th>.      <th>ti
-00004170: 6d65 5f70 6572 696f 643c 2f74 683e 0a20  me_period</th>. 
-00004180: 2020 2020 203c 7468 3e6f 6273 5f76 616c       <th>obs_val
-00004190: 7565 3c2f 7468 3e0a 2020 2020 3c2f 7472  ue</th>.    </tr
-000041a0: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
-000041b0: 7462 6f64 793e 0a20 2020 203c 7472 3e0a  tbody>.    <tr>.
-000041c0: 2020 2020 2020 3c74 683e 303c 2f74 683e        <th>0</th>
-000041d0: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
-000041e0: 3e0a 2020 2020 2020 3c74 643e 5730 303c  >.      <td>W00<
-000041f0: 2f74 643e 0a20 2020 2020 203c 7464 3e50  /td>.      <td>P
-00004200: 434f 414c 3c2f 7464 3e0a 2020 2020 2020  COAL</td>.      
-00004210: 3c74 643e 4958 3c2f 7464 3e0a 2020 2020  <td>IX</td>.    
-00004220: 2020 3c74 643e 303c 2f74 643e 0a20 2020    <td>0</td>.   
-00004230: 2020 203c 7464 3e50 3159 3c2f 7464 3e0a     <td>P1Y</td>.
-00004240: 2020 2020 2020 3c74 643e 3230 3030 3c2f        <td>2000</
-00004250: 7464 3e0a 2020 2020 2020 3c74 643e 3339  td>.      <td>39
-00004260: 2e33 3531 3032 3330 3239 3332 3032 3c2f  .3510230293202</
-00004270: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
-00004280: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
-00004290: 3e31 3c2f 7468 3e0a 2020 2020 2020 3c74  >1</th>.      <t
-000042a0: 643e 413c 2f74 643e 0a20 2020 2020 203c  d>A</td>.      <
-000042b0: 7464 3e57 3030 3c2f 7464 3e0a 2020 2020  td>W00</td>.    
-000042c0: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
-000042d0: 0a20 2020 2020 203c 7464 3e49 583c 2f74  .      <td>IX</t
-000042e0: 643e 0a20 2020 2020 203c 7464 3e30 3c2f  d>.      <td>0</
-000042f0: 7464 3e0a 2020 2020 2020 3c74 643e 5031  td>.      <td>P1
-00004300: 593c 2f74 643e 0a20 2020 2020 203c 7464  Y</td>.      <td
-00004310: 3e32 3030 313c 2f74 643e 0a20 2020 2020  >2001</td>.     
-00004320: 203c 7464 3e34 392e 3333 3738 3538 3732   <td>49.33785872
-00004330: 3834 3033 393c 2f74 643e 0a20 2020 203c  84039</td>.    <
-00004340: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
-00004350: 2020 2020 3c74 683e 323c 2f74 683e 0a20      <th>2</th>. 
-00004360: 2020 2020 203c 7464 3e41 3c2f 7464 3e0a       <td>A</td>.
-00004370: 2020 2020 2020 3c74 643e 5730 303c 2f74        <td>W00</t
-00004380: 643e 0a20 2020 2020 203c 7464 3e50 434f  d>.      <td>PCO
-00004390: 414c 3c2f 7464 3e0a 2020 2020 2020 3c74  AL</td>.      <t
-000043a0: 643e 4958 3c2f 7464 3e0a 2020 2020 2020  d>IX</td>.      
-000043b0: 3c74 643e 303c 2f74 643e 0a20 2020 2020  <td>0</td>.     
-000043c0: 203c 7464 3e50 3159 3c2f 7464 3e0a 2020   <td>P1Y</td>.  
-000043d0: 2020 2020 3c74 643e 3230 3032 3c2f 7464      <td>2002</td
-000043e0: 3e0a 2020 2020 2020 3c74 643e 3339 2e34  >.      <td>39.4
-000043f0: 3934 3930 3931 3634 3830 3036 3c2f 7464  949091648006</td
-00004400: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
-00004410: 3c74 723e 0a20 2020 2020 203c 7468 3e33  <tr>.      <th>3
-00004420: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
-00004430: 413c 2f74 643e 0a20 2020 2020 203c 7464  A</td>.      <td
-00004440: 3e57 3030 3c2f 7464 3e0a 2020 2020 2020  >W00</td>.      
-00004450: 3c74 643e 5043 4f41 4c3c 2f74 643e 0a20  <td>PCOAL</td>. 
-00004460: 2020 2020 203c 7464 3e49 583c 2f74 643e       <td>IX</td>
-00004470: 0a20 2020 2020 203c 7464 3e30 3c2f 7464  .      <td>0</td
-00004480: 3e0a 2020 2020 2020 3c74 643e 5031 593c  >.      <td>P1Y<
-00004490: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
-000044a0: 3030 333c 2f74 643e 0a20 2020 2020 203c  003</td>.      <
-000044b0: 7464 3e34 332e 3238 3738 3837 3639 3530  td>43.2878876950
-000044c0: 3738 383c 2f74 643e 0a20 2020 203c 2f74  788</td>.    </t
-000044d0: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
-000044e0: 2020 3c74 683e 343c 2f74 683e 0a20 2020    <th>4</th>.   
-000044f0: 2020 203c 7464 3e41 3c2f 7464 3e0a 2020     <td>A</td>.  
-00004500: 2020 2020 3c74 643e 5730 303c 2f74 643e      <td>W00</td>
-00004510: 0a20 2020 2020 203c 7464 3e50 434f 414c  .      <td>PCOAL
-00004520: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
-00004530: 4958 3c2f 7464 3e0a 2020 2020 2020 3c74  IX</td>.      <t
-00004540: 643e 303c 2f74 643e 0a20 2020 2020 203c  d>0</td>.      <
-00004550: 7464 3e50 3159 3c2f 7464 3e0a 2020 2020  td>P1Y</td>.    
-00004560: 2020 3c74 643e 3230 3034 3c2f 7464 3e0a    <td>2004</td>.
-00004570: 2020 2020 2020 3c74 643e 3832 2e39 3138        <td>82.918
-00004580: 3538 3538 3035 3238 3632 3c2f 7464 3e0a  5858052862</td>.
-00004590: 2020 2020 3c2f 7472 3e0a 2020 3c2f 7462      </tr>.  </tb
-000045a0: 6f64 793e 0a3c 2f74 6162 6c65 3e0a 3c2f  ody>.</table>.</
-000045b0: 6469 763e 0a0a 0a0a 2323 2320 576f 726b  div>....### Work
-000045c0: 696e 6720 7769 7468 2074 6865 2052 6574  ing with the Ret
-000045d0: 7572 6e65 6420 4461 7461 2046 7261 6d65  urned Data Frame
-000045e0: 0a0a 4e6f 7465 2074 6861 7420 616c 6c20  ..Note that all 
-000045f0: 636f 6c75 6d6e 7320 696e 2074 6865 2072  columns in the r
-00004600: 6574 7572 6e65 6420 6461 7461 2066 7261  eturned data fra
-00004610: 6d65 2061 7265 2063 6861 7261 6374 6572  me are character
-00004620: 2076 6563 746f 7273 2c20 616e 6420 7468   vectors, and th
-00004630: 6174 2074 6f20 706c 6f74 2074 6865 2073  at to plot the s
-00004640: 6572 6965 7320 7765 2077 696c 6c20 6e65  eries we will ne
-00004650: 6564 2074 6f20 636f 6e76 6572 7420 746f  ed to convert to
-00004660: 2076 616c 6964 206e 756d 6572 6963 206f   valid numeric o
-00004670: 7220 6461 7465 2066 6f72 6d61 7473 2e20  r date formats. 
-00004680: 5573 696e 6720 6073 6561 626f 726e 6020  Using `seaborn` 
-00004690: 7769 7468 2060 6875 6560 2c20 7765 2063  with `hue`, we c
-000046a0: 616e 2070 6c6f 7420 6469 6666 6572 656e  an plot differen
-000046b0: 7420 696e 6469 6361 746f 7273 2069 6e20  t indicators in 
-000046c0: 6469 6666 6572 656e 7420 636f 6c6f 7273  different colors
-000046d0: 3a0a 0a0a 6060 6070 7974 686f 6e0a 2320  :...```python.# 
-000046e0: 436f 6e76 6572 7420 6f62 735f 7661 6c75  Convert obs_valu
-000046f0: 6520 746f 206e 756d 6572 6963 2061 6e64  e to numeric and
-00004700: 2074 696d 655f 7065 7269 6f64 2074 6f20   time_period to 
-00004710: 696e 7465 6765 7220 7965 6172 0a64 6620  integer year.df 
-00004720: 3d20 6466 2e61 7374 7970 6528 7b22 7469  = df.astype({"ti
-00004730: 6d65 5f70 6572 696f 6422 203a 2069 6e74  me_period" : int
-00004740: 2c20 226f 6273 5f76 616c 7565 2220 3a20  , "obs_value" : 
-00004750: 666c 6f61 747d 290a 0a23 2050 6c6f 7420  float})..# Plot 
-00004760: 7072 6963 6573 206f 6620 6469 6666 6572  prices of differ
-00004770: 656e 7420 636f 6d6d 6f64 6974 6965 7320  ent commodities 
-00004780: 696e 2064 6966 6665 7265 6e74 2063 6f6c  in different col
-00004790: 6f72 7320 7769 7468 2073 6561 626f 726e  ors with seaborn
-000047a0: 0a73 6561 626f 726e 2e6c 696e 6570 6c6f  .seaborn.lineplo
-000047b0: 7428 6461 7461 3d64 662c 2078 3d27 7469  t(data=df, x='ti
-000047c0: 6d65 5f70 6572 696f 6427 2c20 793d 276f  me_period', y='o
-000047d0: 6273 5f76 616c 7565 272c 2068 7565 3d27  bs_value', hue='
-000047e0: 636f 6d6d 6f64 6974 7927 293b 0a60 6060  commodity');.```
-000047f0: 0a0a 0a20 2020 200a 215b 706e 675d 2852  ...    .![png](R
-00004800: 4541 444d 455f 6669 6c65 732f 706c 6f74  EADME_files/plot
-00004810: 2e70 6e67 290a 2020 2020 0a0a 0a0a 416c  .png).    ....Al
-00004820: 736f 206e 6f74 6520 7468 6174 2074 6865  so note that the
-00004830: 2072 6574 7572 6e65 6420 6461 7461 2066   returned data f
-00004840: 7261 6d65 2068 6173 206d 7973 7465 7269  rame has mysteri
-00004850: 6f75 732d 6c6f 6f6b 696e 6720 636f 6465  ous-looking code
-00004860: 7320 6173 2076 616c 7565 7320 696e 2073  s as values in s
-00004870: 6f6d 6520 636f 6c75 6d6e 732e 0a0a 436f  ome columns...Co
-00004880: 6465 7320 696e 2074 6865 2060 7469 6d65  des in the `time
-00004890: 5f66 6f72 6d61 7460 2063 6f6c 756d 6e20  _format` column 
-000048a0: 6172 6520 4953 4f20 3836 3031 2064 7572  are ISO 8601 dur
-000048b0: 6174 696f 6e20 636f 6465 732e 2049 6e20  ation codes. In 
-000048c0: 7468 6973 2063 6173 652c 20e2 809c 5031  this case, ...P1
-000048d0: 59e2 809d 206d 6561 6e73 20e2 809c 7065  Y... means ...pe
-000048e0: 7269 6f64 7320 6f66 2031 2079 6561 722e  riods of 1 year.
-000048f0: e280 9d20 5468 6520 6075 6e69 745f 6d75  ... The `unit_mu
-00004900: 6c74 6020 636f 6c75 6d6e 2072 6570 7265  lt` column repre
-00004910: 7365 6e74 7320 7468 6520 6e75 6d62 6572  sents the number
-00004920: 206f 6620 7a65 726f 6573 2079 6f75 2073   of zeroes you s
-00004930: 686f 756c 6420 6164 6420 746f 2074 6865  hould add to the
-00004940: 2076 616c 7565 2063 6f6c 756d 6e2e 2046   value column. F
-00004950: 6f72 2069 6e73 7461 6e63 652c 2069 6620  or instance, if 
-00004960: 7661 6c75 6520 6973 2069 6e20 6d69 6c6c  value is in mill
-00004970: 696f 6e73 2c20 7468 656e 2074 6865 2075  ions, then the u
-00004980: 6e69 7420 6d75 6c74 6970 6c69 6572 2077  nit multiplier w
-00004990: 696c 6c20 6265 2036 2e20 4966 2069 6e20  ill be 6. If in 
-000049a0: 6269 6c6c 696f 6e73 2c20 7468 656e 2074  billions, then t
-000049b0: 6865 2075 6e69 7420 6d75 6c74 6970 6c69  he unit multipli
-000049c0: 6572 2077 696c 6c20 6265 2039 2e0a 0a54  er will be 9...T
-000049d0: 6865 206d 6561 6e69 6e67 7320 6f66 2074  he meanings of t
-000049e0: 6865 206f 7468 6572 2063 6f64 6573 2061  he other codes a
-000049f0: 7265 2073 746f 7265 6420 696e 206f 7572  re stored in our
-00004a00: 2060 7061 7261 6d73 6020 6f62 6a65 6374   `params` object
-00004a10: 2061 6e64 2063 616e 2062 6520 6665 7463   and can be fetc
-00004a20: 6865 6420 7769 7468 2061 206a 6f69 6e2e  hed with a join.
-00004a30: 2046 6f72 2069 6e73 7461 6e63 6520 746f   For instance to
-00004a40: 2066 6574 6368 2074 6865 206d 6561 6e69   fetch the meani
-00004a50: 6e67 206f 6620 7468 6520 6072 6566 5f61  ng of the `ref_a
-00004a60: 7265 6160 2063 6f64 6520 e280 9c57 3030  rea` code ...W00
-00004a70: e280 9d2c 2077 6520 6361 6e20 7065 7266  ..., we can perf
-00004a80: 6f72 6d20 6120 6c65 6674 206a 6f69 6e20  orm a left join 
-00004a90: 7769 7468 2074 6865 2060 7061 7261 6d73  with the `params
-00004aa0: 5b27 7265 665f 6172 6561 275d 6020 6461  ['ref_area']` da
-00004ab0: 7461 2066 7261 6d65 2061 6e64 2075 7365  ta frame and use
-00004ac0: 2073 656c 6563 7420 746f 2072 6570 6c61   select to repla
-00004ad0: 6365 2060 7265 665f 6172 6561 6020 7769  ce `ref_area` wi
-00004ae0: 7468 2074 6865 2070 6172 616d 6574 6572  th the parameter
-00004af0: 2064 6573 6372 6970 7469 6f6e 3a0a 0a0a   description:...
-00004b00: 6060 6070 7974 686f 6e0a 2320 4a6f 696e  ```python.# Join
-00004b10: 2064 6620 7769 7468 2070 6172 616d 735b   df with params[
-00004b20: 2772 6566 5f61 7265 6127 5d20 746f 2066  'ref_area'] to f
-00004b30: 6574 6368 2063 6f64 6520 6465 7363 7269  etch code descri
-00004b40: 7074 696f 6e0a 6466 203d 2064 662e 6d65  ption.df = df.me
-00004b50: 7267 6528 7061 7261 6d73 5b27 7265 665f  rge(params['ref_
-00004b60: 6172 6561 275d 2c20 6c65 6674 5f6f 6e3d  area'], left_on=
-00004b70: 2772 6566 5f61 7265 6127 2c72 6967 6874  'ref_area',right
-00004b80: 5f6f 6e3d 2769 6e70 7574 5f63 6f64 6527  _on='input_code'
-00004b90: 2c68 6f77 3d27 6c65 6674 2729 0a0a 2320  ,how='left')..# 
-00004ba0: 4472 6f70 2072 6564 756e 6461 6e74 2063  Drop redundant c
-00004bb0: 6f6c 756d 6e73 2061 6e64 2072 656e 616d  olumns and renam
-00004bc0: 6520 6465 7363 7269 7074 696f 6e20 636f  e description co
-00004bd0: 6c75 6d6e 0a64 6620 3d20 6466 2e64 726f  lumn.df = df.dro
-00004be0: 7028 636f 6c75 6d6e 733d 5b27 7265 665f  p(columns=['ref_
-00004bf0: 6172 6561 272c 2769 6e70 7574 5f63 6f64  area','input_cod
-00004c00: 6527 5d29 2e72 656e 616d 6528 636f 6c75  e']).rename(colu
-00004c10: 6d6e 733d 7b22 6465 7363 7269 7074 696f  mns={"descriptio
-00004c20: 6e22 3a22 7265 665f 6172 6561 227d 290a  n":"ref_area"}).
-00004c30: 0a23 2056 6965 7720 6669 7273 7420 6665  .# View first fe
-00004c40: 7720 636f 6c75 6d6e 7320 696e 2074 6865  w columns in the
-00004c50: 206d 6f64 6966 6965 6420 6461 7461 2066   modified data f
-00004c60: 7261 6d65 0a64 662e 6865 6164 2829 0a60  rame.df.head().`
-00004c70: 6060 0a0a 0a0a 0a3c 6469 763e 0a0a 3c74  ``.....<div>..<t
-00004c80: 6162 6c65 2062 6f72 6465 723d 2231 2220  able border="1" 
-00004c90: 636c 6173 733d 2264 6174 6166 7261 6d65  class="dataframe
-00004ca0: 223e 0a20 203c 7468 6561 643e 0a20 2020  ">.  <thead>.   
-00004cb0: 203c 7472 2073 7479 6c65 3d22 7465 7874   <tr style="text
-00004cc0: 2d61 6c69 676e 3a20 7269 6768 743b 223e  -align: right;">
-00004cd0: 0a20 2020 2020 203c 7468 3e3c 2f74 683e  .      <th></th>
-00004ce0: 0a20 2020 2020 203c 7468 3e66 7265 713c  .      <th>freq<
-00004cf0: 2f74 683e 0a20 2020 2020 203c 7468 3e63  /th>.      <th>c
-00004d00: 6f6d 6d6f 6469 7479 3c2f 7468 3e0a 2020  ommodity</th>.  
-00004d10: 2020 2020 3c74 683e 756e 6974 5f6d 6561      <th>unit_mea
-00004d20: 7375 7265 3c2f 7468 3e0a 2020 2020 2020  sure</th>.      
-00004d30: 3c74 683e 756e 6974 5f6d 756c 743c 2f74  <th>unit_mult</t
-00004d40: 683e 0a20 2020 2020 203c 7468 3e74 696d  h>.      <th>tim
-00004d50: 655f 666f 726d 6174 3c2f 7468 3e0a 2020  e_format</th>.  
-00004d60: 2020 2020 3c74 683e 7469 6d65 5f70 6572      <th>time_per
-00004d70: 696f 643c 2f74 683e 0a20 2020 2020 203c  iod</th>.      <
-00004d80: 7468 3e6f 6273 5f76 616c 7565 3c2f 7468  th>obs_value</th
-00004d90: 3e0a 2020 2020 2020 3c74 683e 7265 665f  >.      <th>ref_
-00004da0: 6172 6561 3c2f 7468 3e0a 2020 2020 3c2f  area</th>.    </
-00004db0: 7472 3e0a 2020 3c2f 7468 6561 643e 0a20  tr>.  </thead>. 
-00004dc0: 203c 7462 6f64 793e 0a20 2020 203c 7472   <tbody>.    <tr
-00004dd0: 3e0a 2020 2020 2020 3c74 683e 303c 2f74  >.      <th>0</t
-00004de0: 683e 0a20 2020 2020 203c 7464 3e41 3c2f  h>.      <td>A</
-00004df0: 7464 3e0a 2020 2020 2020 3c74 643e 5043  td>.      <td>PC
-00004e00: 4f41 4c3c 2f74 643e 0a20 2020 2020 203c  OAL</td>.      <
-00004e10: 7464 3e49 583c 2f74 643e 0a20 2020 2020  td>IX</td>.     
-00004e20: 203c 7464 3e30 3c2f 7464 3e0a 2020 2020   <td>0</td>.    
-00004e30: 2020 3c74 643e 5031 593c 2f74 643e 0a20    <td>P1Y</td>. 
-00004e40: 2020 2020 203c 7464 3e32 3030 303c 2f74       <td>2000</t
-00004e50: 643e 0a20 2020 2020 203c 7464 3e33 392e  d>.      <td>39.
-00004e60: 3335 3130 3233 3c2f 7464 3e0a 2020 2020  351023</td>.    
-00004e70: 2020 3c74 643e 416c 6c20 436f 756e 7472    <td>All Countr
-00004e80: 6965 732c 2065 7863 6c75 6469 6e67 2074  ies, excluding t
-00004e90: 6865 2049 4f3c 2f74 643e 0a20 2020 203c  he IO</td>.    <
-00004ea0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
-00004eb0: 2020 2020 3c74 683e 313c 2f74 683e 0a20      <th>1</th>. 
-00004ec0: 2020 2020 203c 7464 3e41 3c2f 7464 3e0a       <td>A</td>.
-00004ed0: 2020 2020 2020 3c74 643e 5043 4f41 4c3c        <td>PCOAL<
-00004ee0: 2f74 643e 0a20 2020 2020 203c 7464 3e49  /td>.      <td>I
-00004ef0: 583c 2f74 643e 0a20 2020 2020 203c 7464  X</td>.      <td
-00004f00: 3e30 3c2f 7464 3e0a 2020 2020 2020 3c74  >0</td>.      <t
-00004f10: 643e 5031 593c 2f74 643e 0a20 2020 2020  d>P1Y</td>.     
-00004f20: 203c 7464 3e32 3030 313c 2f74 643e 0a20   <td>2001</td>. 
-00004f30: 2020 2020 203c 7464 3e34 392e 3333 3738       <td>49.3378
-00004f40: 3539 3c2f 7464 3e0a 2020 2020 2020 3c74  59</td>.      <t
-00004f50: 643e 416c 6c20 436f 756e 7472 6965 732c  d>All Countries,
-00004f60: 2065 7863 6c75 6469 6e67 2074 6865 2049   excluding the I
-00004f70: 4f3c 2f74 643e 0a20 2020 203c 2f74 723e  O</td>.    </tr>
-00004f80: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
-00004f90: 3c74 683e 323c 2f74 683e 0a20 2020 2020  <th>2</th>.     
-00004fa0: 203c 7464 3e41 3c2f 7464 3e0a 2020 2020   <td>A</td>.    
-00004fb0: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
-00004fc0: 0a20 2020 2020 203c 7464 3e49 583c 2f74  .      <td>IX</t
-00004fd0: 643e 0a20 2020 2020 203c 7464 3e30 3c2f  d>.      <td>0</
-00004fe0: 7464 3e0a 2020 2020 2020 3c74 643e 5031  td>.      <td>P1
-00004ff0: 593c 2f74 643e 0a20 2020 2020 203c 7464  Y</td>.      <td
-00005000: 3e32 3030 323c 2f74 643e 0a20 2020 2020  >2002</td>.     
-00005010: 203c 7464 3e33 392e 3439 3439 3039 3c2f   <td>39.494909</
-00005020: 7464 3e0a 2020 2020 2020 3c74 643e 416c  td>.      <td>Al
-00005030: 6c20 436f 756e 7472 6965 732c 2065 7863  l Countries, exc
-00005040: 6c75 6469 6e67 2074 6865 2049 4f3c 2f74  luding the IO</t
-00005050: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
-00005060: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
-00005070: 333c 2f74 683e 0a20 2020 2020 203c 7464  3</th>.      <td
-00005080: 3e41 3c2f 7464 3e0a 2020 2020 2020 3c74  >A</td>.      <t
-00005090: 643e 5043 4f41 4c3c 2f74 643e 0a20 2020  d>PCOAL</td>.   
-000050a0: 2020 203c 7464 3e49 583c 2f74 643e 0a20     <td>IX</td>. 
-000050b0: 2020 2020 203c 7464 3e30 3c2f 7464 3e0a       <td>0</td>.
-000050c0: 2020 2020 2020 3c74 643e 5031 593c 2f74        <td>P1Y</t
-000050d0: 643e 0a20 2020 2020 203c 7464 3e32 3030  d>.      <td>200
-000050e0: 333c 2f74 643e 0a20 2020 2020 203c 7464  3</td>.      <td
-000050f0: 3e34 332e 3238 3738 3838 3c2f 7464 3e0a  >43.287888</td>.
-00005100: 2020 2020 2020 3c74 643e 416c 6c20 436f        <td>All Co
-00005110: 756e 7472 6965 732c 2065 7863 6c75 6469  untries, excludi
-00005120: 6e67 2074 6865 2049 4f3c 2f74 643e 0a20  ng the IO</td>. 
-00005130: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
-00005140: 3e0a 2020 2020 2020 3c74 683e 343c 2f74  >.      <th>4</t
-00005150: 683e 0a20 2020 2020 203c 7464 3e41 3c2f  h>.      <td>A</
-00005160: 7464 3e0a 2020 2020 2020 3c74 643e 5043  td>.      <td>PC
-00005170: 4f41 4c3c 2f74 643e 0a20 2020 2020 203c  OAL</td>.      <
-00005180: 7464 3e49 583c 2f74 643e 0a20 2020 2020  td>IX</td>.     
-00005190: 203c 7464 3e30 3c2f 7464 3e0a 2020 2020   <td>0</td>.    
-000051a0: 2020 3c74 643e 5031 593c 2f74 643e 0a20    <td>P1Y</td>. 
-000051b0: 2020 2020 203c 7464 3e32 3030 343c 2f74       <td>2004</t
-000051c0: 643e 0a20 2020 2020 203c 7464 3e38 322e  d>.      <td>82.
-000051d0: 3931 3835 3836 3c2f 7464 3e0a 2020 2020  918586</td>.    
-000051e0: 2020 3c74 643e 416c 6c20 436f 756e 7472    <td>All Countr
-000051f0: 6965 732c 2065 7863 6c75 6469 6e67 2074  ies, excluding t
-00005200: 6865 2049 4f3c 2f74 643e 0a20 2020 203c  he IO</td>.    <
-00005210: 2f74 723e 0a20 203c 2f74 626f 6479 3e0a  /tr>.  </tbody>.
-00005220: 3c2f 7461 626c 653e 0a3c 2f64 6976 3e0a  </table>.</div>.
-00005230: 0a0a 0a                                  ...
+000008a0: 0a60 6060 0a0a 0a23 2323 2046 6574 6368  .```...### Fetch
+000008b0: 696e 6720 616e 2049 6e64 6578 206f 6620  ing an Index of 
+000008c0: 4461 7461 6261 7365 7320 7769 7468 2074  Databases with t
+000008d0: 6865 2060 696d 665f 6461 7461 6261 7365  he `imf_database
+000008e0: 7360 2046 756e 6374 696f 6e0a 0a54 6865  s` Function..The
+000008f0: 2060 696d 6670 6020 7061 636b 6167 6520   `imfp` package 
+00000900: 696e 7472 6f64 7563 6573 2066 6f75 7220  introduces four 
+00000910: 636f 7265 2066 756e 6374 696f 6e73 3a20  core functions: 
+00000920: 6069 6d66 702e 696d 665f 6461 7461 6261  `imfp.imf_databa
+00000930: 7365 7360 2c20 6069 6d66 702e 696d 665f  ses`, `imfp.imf_
+00000940: 7061 7261 6d65 7465 7273 602c 2060 696d  parameters`, `im
+00000950: 6670 2e69 6d66 5f70 6172 616d 6574 6572  fp.imf_parameter
+00000960: 5f64 6566 7360 2c20 616e 6420 6069 6d66  _defs`, and `imf
+00000970: 702e 696d 665f 6461 7461 7365 7460 2e20  p.imf_dataset`. 
+00000980: 5468 6520 6675 6e63 7469 6f6e 2066 6f72  The function for
+00000990: 2064 6f77 6e6c 6f61 6469 6e67 2064 6174   downloading dat
+000009a0: 6173 6574 7320 6973 2060 696d 6670 2e69  asets is `imfp.i
+000009b0: 6d66 5f64 6174 6173 6574 602c 2062 7574  mf_dataset`, but
+000009c0: 2079 6f75 2077 696c 6c20 6e65 6564 2074   you will need t
+000009d0: 6865 206f 7468 6572 2066 756e 6374 696f  he other functio
+000009e0: 6e73 2074 6f20 6465 7465 726d 696e 6520  ns to determine 
+000009f0: 7768 6174 2061 7267 756d 656e 7473 2074  what arguments t
+00000a00: 6f20 7375 7070 6c79 2074 6f20 6069 6d66  o supply to `imf
+00000a10: 702e 696d 665f 6461 7461 7365 7460 2e20  p.imf_dataset`. 
+00000a20: 466f 7220 696e 7374 616e 6365 2c20 616c  For instance, al
+00000a30: 6c20 6361 6c6c 7320 746f 2060 696d 6670  l calls to `imfp
+00000a40: 2e69 6d66 5f64 6174 6173 6574 6020 7265  .imf_dataset` re
+00000a50: 7175 6972 6520 6120 6064 6174 6162 6173  quire a `databas
+00000a60: 655f 6964 602e 2054 6869 7320 6973 2062  e_id`. This is b
+00000a70: 6563 6175 7365 2074 6865 2049 4d46 2073  ecause the IMF s
+00000a80: 6572 7665 7320 6d61 6e79 2064 6966 6665  erves many diffe
+00000a90: 7265 6e74 2064 6174 6162 6173 6573 2074  rent databases t
+00000aa0: 6872 6f75 6768 2069 7473 2041 5049 2c20  hrough its API, 
+00000ab0: 616e 6420 7468 6520 4150 4920 6e65 6564  and the API need
+00000ac0: 7320 746f 206b 6e6f 7720 7768 6963 6820  s to know which 
+00000ad0: 6f66 2074 6865 7365 206d 616e 7920 6461  of these many da
+00000ae0: 7461 6261 7365 7320 796f 7527 7265 2072  tabases you're r
+00000af0: 6571 7565 7374 696e 6720 6461 7461 2066  equesting data f
+00000b00: 726f 6d2e 2054 6f20 6f62 7461 696e 2061  rom. To obtain a
+00000b10: 206c 6973 7420 6f66 2064 6174 6162 6173   list of databas
+00000b20: 6573 2c20 7573 6520 6069 6d66 702e 696d  es, use `imfp.im
+00000b30: 665f 6461 7461 6261 7365 7360 2c20 6c69  f_databases`, li
+00000b40: 6b65 2073 6f3a 0a0a 0a60 6060 7079 7468  ke so:...```pyth
+00000b50: 6f6e 0a23 4665 7463 6820 7468 6520 6c69  on.#Fetch the li
+00000b60: 7374 206f 6620 6461 7461 6261 7365 7320  st of databases 
+00000b70: 6176 6169 6c61 626c 6520 7468 726f 7567  available throug
+00000b80: 6820 7468 6520 494d 4620 4150 490a 6461  h the IMF API.da
+00000b90: 7461 6261 7365 7320 3d20 696d 6670 2e69  tabases = imfp.i
+00000ba0: 6d66 5f64 6174 6162 6173 6573 2829 0a64  mf_databases().d
+00000bb0: 6174 6162 6173 6573 2e68 6561 6428 290a  atabases.head().
+00000bc0: 6060 600a 0a0a 0a0a 3c64 6976 3e0a 0a3c  ```.....<div>..<
+00000bd0: 7461 626c 6520 626f 7264 6572 3d22 3122  table border="1"
+00000be0: 2063 6c61 7373 3d22 6461 7461 6672 616d   class="datafram
+00000bf0: 6522 3e0a 2020 3c74 6865 6164 3e0a 2020  e">.  <thead>.  
+00000c00: 2020 3c74 7220 7374 796c 653d 2274 6578    <tr style="tex
+00000c10: 742d 616c 6967 6e3a 2072 6967 6874 3b22  t-align: right;"
+00000c20: 3e0a 2020 2020 2020 3c74 683e 3c2f 7468  >.      <th></th
+00000c30: 3e0a 2020 2020 2020 3c74 683e 6461 7461  >.      <th>data
+00000c40: 6261 7365 5f69 643c 2f74 683e 0a20 2020  base_id</th>.   
+00000c50: 2020 203c 7468 3e64 6573 6372 6970 7469     <th>descripti
+00000c60: 6f6e 3c2f 7468 3e0a 2020 2020 3c2f 7472  on</th>.    </tr
+00000c70: 3e0a 2020 3c2f 7468 6561 643e 0a20 203c  >.  </thead>.  <
+00000c80: 7462 6f64 793e 0a20 2020 203c 7472 3e0a  tbody>.    <tr>.
+00000c90: 2020 2020 2020 3c74 683e 303c 2f74 683e        <th>0</th>
+00000ca0: 0a20 2020 2020 203c 7464 3e42 4f50 5f32  .      <td>BOP_2
+00000cb0: 3031 374d 3036 3c2f 7464 3e0a 2020 2020  017M06</td>.    
+00000cc0: 2020 3c74 643e 4261 6c61 6e63 6520 6f66    <td>Balance of
+00000cd0: 2050 6179 6d65 6e74 7320 2842 4f50 292c   Payments (BOP),
+00000ce0: 2032 3031 3720 4d30 363c 2f74 643e 0a20   2017 M06</td>. 
+00000cf0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+00000d00: 3e0a 2020 2020 2020 3c74 683e 313c 2f74  >.      <th>1</t
+00000d10: 683e 0a20 2020 2020 203c 7464 3e42 4f50  h>.      <td>BOP
+00000d20: 5f32 3032 304d 333c 2f74 643e 0a20 2020  _2020M3</td>.   
+00000d30: 2020 203c 7464 3e42 616c 616e 6365 206f     <td>Balance o
+00000d40: 6620 5061 796d 656e 7473 2028 424f 5029  f Payments (BOP)
+00000d50: 2c20 3230 3230 204d 3033 3c2f 7464 3e0a  , 2020 M03</td>.
+00000d60: 2020 2020 3c2f 7472 3e0a 2020 2020 3c74      </tr>.    <t
+00000d70: 723e 0a20 2020 2020 203c 7468 3e32 3c2f  r>.      <th>2</
+00000d80: 7468 3e0a 2020 2020 2020 3c74 643e 424f  th>.      <td>BO
+00000d90: 505f 3230 3137 4d31 313c 2f74 643e 0a20  P_2017M11</td>. 
+00000da0: 2020 2020 203c 7464 3e42 616c 616e 6365       <td>Balance
+00000db0: 206f 6620 5061 796d 656e 7473 2028 424f   of Payments (BO
+00000dc0: 5029 2c20 3230 3137 204d 3131 3c2f 7464  P), 2017 M11</td
+00000dd0: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00000de0: 3c74 723e 0a20 2020 2020 203c 7468 3e33  <tr>.      <th>3
+00000df0: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+00000e00: 444f 545f 3230 3230 5131 3c2f 7464 3e0a  DOT_2020Q1</td>.
+00000e10: 2020 2020 2020 3c74 643e 4469 7265 6374        <td>Direct
+00000e20: 696f 6e20 6f66 2054 7261 6465 2053 7461  ion of Trade Sta
+00000e30: 7469 7374 6963 7320 2844 4f54 5329 2c20  tistics (DOTS), 
+00000e40: 3230 3230 2051 313c 2f74 643e 0a20 2020  2020 Q1</td>.   
+00000e50: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00000e60: 2020 2020 2020 3c74 683e 343c 2f74 683e        <th>4</th>
+00000e70: 0a20 2020 2020 203c 7464 3e47 4653 4d41  .      <td>GFSMA
+00000e80: 4232 3031 363c 2f74 643e 0a20 2020 2020  B2016</td>.     
+00000e90: 203c 7464 3e47 6f76 6572 6e6d 656e 7420   <td>Government 
+00000ea0: 4669 6e61 6e63 6520 5374 6174 6973 7469  Finance Statisti
+00000eb0: 6373 2059 6561 7262 6f6f 6b20 2847 4653  cs Yearbook (GFS
+00000ec0: 5920 322e 2e2e 3c2f 7464 3e0a 2020 2020  Y 2...</td>.    
+00000ed0: 3c2f 7472 3e0a 2020 3c2f 7462 6f64 793e  </tr>.  </tbody>
+00000ee0: 0a3c 2f74 6162 6c65 3e0a 3c2f 6469 763e  .</table>.</div>
+00000ef0: 0a0a 0a0a 5468 6973 2066 756e 6374 696f  ....This functio
+00000f00: 6e20 7265 7475 726e 7320 7468 6520 494d  n returns the IM
+00000f10: 46e2 8099 7320 6c69 7374 696e 6720 6f66  F...s listing of
+00000f20: 2032 3539 2064 6174 6162 6173 6573 2061   259 databases a
+00000f30: 7661 696c 6162 6c65 2074 6872 6f75 6768  vailable through
+00000f40: 2074 6865 2041 5049 2e20 2849 6e20 7265   the API. (In re
+00000f50: 616c 6974 792c 2037 206f 6620 7468 6520  ality, 7 of the 
+00000f60: 6c69 7374 6564 2064 6174 6162 6173 6573  listed databases
+00000f70: 2061 7265 2064 6566 756e 6374 2061 6e64   are defunct and
+00000f80: 206e 6f74 2061 6374 7561 6c6c 7920 6176   not actually av
+00000f90: 6169 6c61 626c 653a 2046 4153 5f32 3031  ailable: FAS_201
+00000fa0: 352c 2047 4653 3031 2c20 464d 3230 3230  5, GFS01, FM2020
+00000fb0: 3130 2c20 4150 4452 454f 3230 3230 3130  10, APDREO202010
+00000fc0: 2c20 4146 5252 454f 3230 3230 3130 2c20  , AFRREO202010, 
+00000fd0: 5748 4452 454f 3230 3230 3130 2c20 424f  WHDREO202010, BO
+00000fe0: 5041 4747 5f32 3032 302e 290a 0a54 6f20  PAGG_2020.)..To 
+00000ff0: 7669 6577 2061 6e64 2065 7870 6c6f 7265  view and explore
+00001000: 2074 6865 2064 6174 6162 6173 6520 6c69   the database li
+00001010: 7374 2c20 6974 e280 9973 2070 6f73 7369  st, it...s possi
+00001020: 626c 6520 746f 2065 7870 6c6f 7265 2073  ble to explore s
+00001030: 7562 7365 7473 206f 6620 7468 6520 6461  ubsets of the da
+00001040: 7461 2066 7261 6d65 2062 7920 726f 7720  ta frame by row 
+00001050: 6e75 6d62 6572 2077 6974 6820 6064 6174  number with `dat
+00001060: 6162 6173 6573 2e6c 6f63 603a 0a0a 0a0a  abases.loc`:....
+00001070: 6060 6070 7974 686f 6e0a 2320 5669 6577  ```python.# View
+00001080: 2061 2073 7562 7365 7420 636f 6e73 6973   a subset consis
+00001090: 7469 6e67 206f 6620 726f 7773 2035 2074  ting of rows 5 t
+000010a0: 6872 6f75 6768 2039 0a64 6174 6162 6173  hrough 9.databas
+000010b0: 6573 2e6c 6f63 5b35 3a39 5d0a 6060 600a  es.loc[5:9].```.
+000010c0: 0a0a 0a0a 3c64 6976 3e0a 0a3c 7461 626c  ....<div>..<tabl
+000010d0: 6520 626f 7264 6572 3d22 3122 2063 6c61  e border="1" cla
+000010e0: 7373 3d22 6461 7461 6672 616d 6522 3e0a  ss="dataframe">.
+000010f0: 2020 3c74 6865 6164 3e0a 2020 2020 3c74    <thead>.    <t
+00001100: 7220 7374 796c 653d 2274 6578 742d 616c  r style="text-al
+00001110: 6967 6e3a 2072 6967 6874 3b22 3e0a 2020  ign: right;">.  
+00001120: 2020 2020 3c74 683e 3c2f 7468 3e0a 2020      <th></th>.  
+00001130: 2020 2020 3c74 683e 6461 7461 6261 7365      <th>database
+00001140: 5f69 643c 2f74 683e 0a20 2020 2020 203c  _id</th>.      <
+00001150: 7468 3e64 6573 6372 6970 7469 6f6e 3c2f  th>description</
+00001160: 7468 3e0a 2020 2020 3c2f 7472 3e0a 2020  th>.    </tr>.  
+00001170: 3c2f 7468 6561 643e 0a20 203c 7462 6f64  </thead>.  <tbod
+00001180: 793e 0a20 2020 203c 7472 3e0a 2020 2020  y>.    <tr>.    
+00001190: 2020 3c74 683e 353c 2f74 683e 0a20 2020    <th>5</th>.   
+000011a0: 2020 203c 7464 3e42 4f50 5f32 3031 394d     <td>BOP_2019M
+000011b0: 3132 3c2f 7464 3e0a 2020 2020 2020 3c74  12</td>.      <t
+000011c0: 643e 4261 6c61 6e63 6520 6f66 2050 6179  d>Balance of Pay
+000011d0: 6d65 6e74 7320 2842 4f50 292c 2032 3031  ments (BOP), 201
+000011e0: 3920 4d31 323c 2f74 643e 0a20 2020 203c  9 M12</td>.    <
+000011f0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+00001200: 2020 2020 3c74 683e 363c 2f74 683e 0a20      <th>6</th>. 
+00001210: 2020 2020 203c 7464 3e47 4653 5946 414c       <td>GFSYFAL
+00001220: 4353 3230 3134 3c2f 7464 3e0a 2020 2020  CS2014</td>.    
+00001230: 2020 3c74 643e 476f 7665 726e 6d65 6e74    <td>Government
+00001240: 2046 696e 616e 6365 2053 7461 7469 7374   Finance Statist
+00001250: 6963 7320 5965 6172 626f 6f6b 2028 4746  ics Yearbook (GF
+00001260: 5359 2032 2e2e 2e3c 2f74 643e 0a20 2020  SY 2...</td>.   
+00001270: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00001280: 2020 2020 2020 3c74 683e 373c 2f74 683e        <th>7</th>
+00001290: 0a20 2020 2020 203c 7464 3e47 4653 4532  .      <td>GFSE2
+000012a0: 3031 363c 2f74 643e 0a20 2020 2020 203c  016</td>.      <
+000012b0: 7464 3e47 6f76 6572 6e6d 656e 7420 4669  td>Government Fi
+000012c0: 6e61 6e63 6520 5374 6174 6973 7469 6373  nance Statistics
+000012d0: 2059 6561 7262 6f6f 6b20 2847 4653 5920   Yearbook (GFSY 
+000012e0: 322e 2e2e 3c2f 7464 3e0a 2020 2020 3c2f  2...</td>.    </
+000012f0: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+00001300: 2020 203c 7468 3e38 3c2f 7468 3e0a 2020     <th>8</th>.  
+00001310: 2020 2020 3c74 643e 464d 3230 3135 3130      <td>FM201510
+00001320: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00001330: 4669 7363 616c 204d 6f6e 6974 6f72 2028  Fiscal Monitor (
+00001340: 464d 2920 4f63 746f 6265 7220 3230 3135  FM) October 2015
+00001350: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00001360: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+00001370: 7468 3e39 3c2f 7468 3e0a 2020 2020 2020  th>9</th>.      
+00001380: 3c74 643e 4746 5349 4253 3230 3136 3c2f  <td>GFSIBS2016</
+00001390: 7464 3e0a 2020 2020 2020 3c74 643e 476f  td>.      <td>Go
+000013a0: 7665 726e 6d65 6e74 2046 696e 616e 6365  vernment Finance
+000013b0: 2053 7461 7469 7374 6963 7320 5965 6172   Statistics Year
+000013c0: 626f 6f6b 2028 4746 5359 2032 2e2e 2e3c  book (GFSY 2...<
+000013d0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000013e0: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+000013f0: 653e 0a3c 2f64 6976 3e0a 0a0a 0a0a 204f  e>.</div>..... O
+00001400: 722c 2069 6620 796f 7520 616c 7265 6164  r, if you alread
+00001410: 7920 6b6e 6f77 2077 6869 6368 2064 6174  y know which dat
+00001420: 6162 6173 6520 796f 7520 7761 6e74 2c20  abase you want, 
+00001430: 796f 7520 6361 6e20 6665 7463 6820 7468  you can fetch th
+00001440: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
+00001450: 636f 6465 2062 7920 7365 6172 6368 696e  code by searchin
+00001460: 6720 666f 7220 6120 7374 7269 6e67 206d  g for a string m
+00001470: 6174 6368 2075 7369 6e67 2060 7374 722e  atch using `str.
+00001480: 636f 6e74 6169 6e73 6020 616e 6420 7375  contains` and su
+00001490: 6273 6574 7469 6e67 2074 6865 2064 6174  bsetting the dat
+000014a0: 6120 6672 616d 6520 666f 7220 6d61 7463  a frame for matc
+000014b0: 6869 6e67 2072 6f77 732e 2046 6f72 2069  hing rows. For i
+000014c0: 6e73 7461 6e63 652c 2068 6572 65e2 8099  nstance, here...
+000014d0: 7320 686f 7720 746f 2073 6561 7263 6820  s how to search 
+000014e0: 666f 7220 7468 6520 5072 696d 6172 7920  for the Primary 
+000014f0: 436f 6d6d 6f64 6974 7920 5072 6963 6520  Commodity Price 
+00001500: 5379 7374 656d 3a0a 0a0a 6060 6070 7974  System:...```pyt
+00001510: 686f 6e0a 6461 7461 6261 7365 735b 6461  hon.databases[da
+00001520: 7461 6261 7365 735b 2764 6573 6372 6970  tabases['descrip
+00001530: 7469 6f6e 275d 2e73 7472 2e63 6f6e 7461  tion'].str.conta
+00001540: 696e 7328 2243 6f6d 6d6f 6469 7479 2229  ins("Commodity")
+00001550: 5d0a 6060 600a 0a0a 0a0a 3c64 6976 3e0a  ].```.....<div>.
+00001560: 0a3c 7461 626c 6520 626f 7264 6572 3d22  .<table border="
+00001570: 3122 2063 6c61 7373 3d22 6461 7461 6672  1" class="datafr
+00001580: 616d 6522 3e0a 2020 3c74 6865 6164 3e0a  ame">.  <thead>.
+00001590: 2020 2020 3c74 7220 7374 796c 653d 2274      <tr style="t
+000015a0: 6578 742d 616c 6967 6e3a 2072 6967 6874  ext-align: right
+000015b0: 3b22 3e0a 2020 2020 2020 3c74 683e 3c2f  ;">.      <th></
+000015c0: 7468 3e0a 2020 2020 2020 3c74 683e 6461  th>.      <th>da
+000015d0: 7461 6261 7365 5f69 643c 2f74 683e 0a20  tabase_id</th>. 
+000015e0: 2020 2020 203c 7468 3e64 6573 6372 6970       <th>descrip
+000015f0: 7469 6f6e 3c2f 7468 3e0a 2020 2020 3c2f  tion</th>.    </
+00001600: 7472 3e0a 2020 3c2f 7468 6561 643e 0a20  tr>.  </thead>. 
+00001610: 203c 7462 6f64 793e 0a20 2020 203c 7472   <tbody>.    <tr
+00001620: 3e0a 2020 2020 2020 3c74 683e 3233 373c  >.      <th>237<
+00001630: 2f74 683e 0a20 2020 2020 203c 7464 3e50  /th>.      <td>P
+00001640: 4354 4f54 3c2f 7464 3e0a 2020 2020 2020  CTOT</td>.      
+00001650: 3c74 643e 436f 6d6d 6f64 6974 7920 5465  <td>Commodity Te
+00001660: 726d 7320 6f66 2054 7261 6465 3c2f 7464  rms of Trade</td
+00001670: 3e0a 2020 2020 3c2f 7472 3e0a 2020 2020  >.    </tr>.    
+00001680: 3c74 723e 0a20 2020 2020 203c 7468 3e32  <tr>.      <th>2
+00001690: 3339 3c2f 7468 3e0a 2020 2020 2020 3c74  39</th>.      <t
+000016a0: 643e 5043 5053 3c2f 7464 3e0a 2020 2020  d>PCPS</td>.    
+000016b0: 2020 3c74 643e 5072 696d 6172 7920 436f    <td>Primary Co
+000016c0: 6d6d 6f64 6974 7920 5072 6963 6520 5379  mmodity Price Sy
+000016d0: 7374 656d 2028 5043 5053 293c 2f74 643e  stem (PCPS)</td>
+000016e0: 0a20 2020 203c 2f74 723e 0a20 203c 2f74  .    </tr>.  </t
+000016f0: 626f 6479 3e0a 3c2f 7461 626c 653e 0a3c  body>.</table>.<
+00001700: 2f64 6976 3e0a 0a0a 0a23 2323 2046 6574  /div>....### Fet
+00001710: 6368 696e 6720 6120 4c69 7374 206f 6620  ching a List of 
+00001720: 5061 7261 6d65 7465 7273 2061 6e64 2049  Parameters and I
+00001730: 6e70 7574 2043 6f64 6573 2077 6974 6820  nput Codes with 
+00001740: 6069 6d66 5f70 6172 616d 6574 6572 7360  `imf_parameters`
+00001750: 2061 6e64 2060 696d 665f 7061 7261 6d65   and `imf_parame
+00001760: 7465 725f 6465 6673 600a 0a4f 6e63 6520  ter_defs`..Once 
+00001770: 796f 7520 6861 7665 2061 2060 6461 7461  you have a `data
+00001780: 6261 7365 5f69 6460 2c20 6974 e280 9973  base_id`, it...s
+00001790: 2070 6f73 7369 626c 6520 746f 206d 616b   possible to mak
+000017a0: 6520 6120 6361 6c6c 2074 6f20 6069 6d66  e a call to `imf
+000017b0: 702e 696d 665f 6461 7461 7365 7460 2074  p.imf_dataset` t
+000017c0: 6f20 6665 7463 6820 7468 6520 656e 7469  o fetch the enti
+000017d0: 7265 2064 6174 6162 6173 653a 2060 696d  re database: `im
+000017e0: 6670 2e69 6d66 5f64 6174 6173 6574 2864  fp.imf_dataset(d
+000017f0: 6174 6162 6173 655f 6964 2960 2e20 486f  atabase_id)`. Ho
+00001800: 7765 7665 722c 2077 6869 6c65 2074 6869  wever, while thi
+00001810: 7320 7769 6c6c 2073 7563 6365 6564 2066  s will succeed f
+00001820: 6f72 2061 2066 6577 2073 6d61 6c6c 2064  or a few small d
+00001830: 6174 6162 6173 6573 2c20 6974 2077 696c  atabases, it wil
+00001840: 6c20 6661 696c 2066 6f72 2061 6c6c 206f  l fail for all o
+00001850: 6620 7468 6520 6c61 7267 6572 206f 6e65  f the larger one
+00001860: 732e 2041 6e64 2065 7665 6e20 696e 2074  s. And even in t
+00001870: 6865 2072 6172 6520 6361 7365 2077 6865  he rare case whe
+00001880: 6e20 6974 2073 7563 6365 6564 732c 2066  n it succeeds, f
+00001890: 6574 6368 696e 6720 616e 2065 6e74 6972  etching an entir
+000018a0: 6520 6461 7461 6261 7365 2063 616e 2074  e database can t
+000018b0: 616b 6520 6120 6c6f 6e67 2074 696d 652e  ake a long time.
+000018c0: 2059 6f75 e280 9972 6520 6d75 6368 2062   You...re much b
+000018d0: 6574 7465 7220 6f66 6620 7375 7070 6c79  etter off supply
+000018e0: 696e 6720 6164 6469 7469 6f6e 616c 2066  ing additional f
+000018f0: 696c 7465 7220 7061 7261 6d65 7465 7273  ilter parameters
+00001900: 2074 6f20 7265 6475 6365 2074 6865 2073   to reduce the s
+00001910: 697a 6520 6f66 2079 6f75 7220 7265 7175  ize of your requ
+00001920: 6573 742e 0a0a 5265 7175 6573 7473 2074  est...Requests t
+00001930: 6f20 6461 7461 6261 7365 7320 6176 6169  o databases avai
+00001940: 6c61 626c 6520 7468 726f 7567 6820 7468  lable through th
+00001950: 6520 494d 4620 4150 4920 6172 6520 636f  e IMF API are co
+00001960: 6d70 6c69 6361 7465 6420 6279 2074 6865  mplicated by the
+00001970: 2066 6163 7420 7468 6174 2065 6163 6820   fact that each 
+00001980: 6461 7461 6261 7365 2075 7365 7320 6120  database uses a 
+00001990: 6469 6666 6572 656e 7420 7365 7420 6f66  different set of
+000019a0: 2070 6172 616d 6574 6572 7320 7768 656e   parameters when
+000019b0: 206d 616b 696e 6720 6120 7265 7175 6573   making a reques
+000019c0: 742e 2028 4174 206c 6173 7420 636f 756e  t. (At last coun
+000019d0: 742c 2074 6865 7265 2077 6572 6520 3433  t, there were 43
+000019e0: 2075 6e69 7175 6520 7061 7261 6d65 7465   unique paramete
+000019f0: 7273 2075 7365 6420 696e 206d 616b 696e  rs used in makin
+00001a00: 6720 4150 4920 7265 7175 6573 7473 2066  g API requests f
+00001a10: 726f 6d20 7468 6520 7661 7269 6f75 7320  rom the various 
+00001a20: 6461 7461 6261 7365 7321 2920 596f 7520  databases!) You 
+00001a30: 616c 736f 2068 6176 6520 746f 2068 6176  also have to hav
+00001a40: 6520 7468 6520 6c69 7374 206f 6620 7661  e the list of va
+00001a50: 6c69 6420 696e 7075 7420 636f 6465 7320  lid input codes 
+00001a60: 666f 7220 6561 6368 2070 6172 616d 6574  for each paramet
+00001a70: 6572 2e20 5468 6520 6069 6d66 702e 696d  er. The `imfp.im
+00001a80: 665f 7061 7261 6d65 7465 7273 6020 6675  f_parameters` fu
+00001a90: 6e63 7469 6f6e 2073 6f6c 7665 7320 7468  nction solves th
+00001aa0: 6973 2070 726f 626c 656d 2e20 5573 6520  is problem. Use 
+00001ab0: 7468 6520 6675 6e63 7469 6f6e 2074 6f20  the function to 
+00001ac0: 6f62 7461 696e 2074 6865 2066 756c 6c20  obtain the full 
+00001ad0: 6c69 7374 206f 6620 7061 7261 6d65 7465  list of paramete
+00001ae0: 7273 2061 6e64 2076 616c 6964 2069 6e70  rs and valid inp
+00001af0: 7574 2063 6f64 6573 2066 6f72 2061 2067  ut codes for a g
+00001b00: 6976 656e 2064 6174 6162 6173 653a 0a0a  iven database:..
+00001b10: 0a60 6060 7079 7468 6f6e 0a23 2046 6574  .```python.# Fet
+00001b20: 6368 206c 6973 7420 6f66 2076 616c 6964  ch list of valid
+00001b30: 2070 6172 616d 6574 6572 7320 616e 6420   parameters and 
+00001b40: 696e 7075 7420 636f 6465 7320 666f 7220  input codes for 
+00001b50: 636f 6d6d 6f64 6974 7920 7072 6963 6520  commodity price 
+00001b60: 6461 7461 6261 7365 0a70 6172 616d 7320  database.params 
+00001b70: 3d20 696d 6670 2e69 6d66 5f70 6172 616d  = imfp.imf_param
+00001b80: 6574 6572 7328 2250 4350 5322 290a 6060  eters("PCPS").``
+00001b90: 600a 0a54 6865 2060 696d 6670 2e69 6d66  `..The `imfp.imf
+00001ba0: 5f70 6172 616d 6574 6572 7360 2066 756e  _parameters` fun
+00001bb0: 6374 696f 6e20 7265 7475 726e 7320 6120  ction returns a 
+00001bc0: 6469 6374 696f 6e61 7279 206f 6620 6461  dictionary of da
+00001bd0: 7461 2066 7261 6d65 732e 2045 6163 6820  ta frames. Each 
+00001be0: 6469 6374 696f 6e61 7279 206b 6579 206e  dictionary key n
+00001bf0: 616d 6520 636f 7272 6573 706f 6e64 7320  ame corresponds 
+00001c00: 746f 2061 2070 6172 616d 6574 6572 2075  to a parameter u
+00001c10: 7365 6420 696e 206d 616b 696e 6720 7265  sed in making re
+00001c20: 7175 6573 7473 2066 726f 6d20 7468 6520  quests from the 
+00001c30: 6461 7461 6261 7365 3a0a 0a0a 6060 6070  database:...```p
+00001c40: 7974 686f 6e0a 2320 4765 7420 6b65 7920  ython.# Get key 
+00001c50: 6e61 6d65 7320 6672 6f6d 2074 6865 2070  names from the p
+00001c60: 6172 616d 7320 6f62 6a65 6374 0a70 6172  arams object.par
+00001c70: 616d 732e 6b65 7973 2829 0a60 6060 0a0a  ams.keys().```..
+00001c80: 0a0a 0a20 2020 2064 6963 745f 6b65 7973  ...    dict_keys
+00001c90: 285b 2766 7265 7127 2c20 2772 6566 5f61  (['freq', 'ref_a
+00001ca0: 7265 6127 2c20 2763 6f6d 6d6f 6469 7479  rea', 'commodity
+00001cb0: 272c 2027 756e 6974 5f6d 6561 7375 7265  ', 'unit_measure
+00001cc0: 275d 290a 0a0a 0a49 6e20 7468 6520 6576  '])....In the ev
+00001cd0: 656e 7420 7468 6174 2061 2070 6172 616d  ent that a param
+00001ce0: 6574 6572 206e 616d 6520 6973 206e 6f74  eter name is not
+00001cf0: 2073 656c 662d 6578 706c 616e 6174 6f72   self-explanator
+00001d00: 792c 2074 6865 2060 696d 6670 2e69 6d66  y, the `imfp.imf
+00001d10: 5f70 6172 616d 6574 6572 5f64 6566 7360  _parameter_defs`
+00001d20: 2066 756e 6374 696f 6e20 6361 6e20 6265   function can be
+00001d30: 2075 7365 6420 746f 2066 6574 6368 2073   used to fetch s
+00001d40: 686f 7274 2074 6578 7420 6465 7363 7269  hort text descri
+00001d50: 7074 696f 6e73 206f 6620 6561 6368 2070  ptions of each p
+00001d60: 6172 616d 6574 6572 3a0a 0a0a 6060 6070  arameter:...```p
+00001d70: 7974 686f 6e0a 2320 4665 7463 6820 616e  ython.# Fetch an
+00001d80: 6420 6469 7370 6c61 7920 7061 7261 6d65  d display parame
+00001d90: 7465 7220 7465 7874 2064 6573 6372 6970  ter text descrip
+00001da0: 7469 6f6e 7320 666f 7220 7468 6520 636f  tions for the co
+00001db0: 6d6d 6f64 6974 7920 7072 6963 6520 6461  mmodity price da
+00001dc0: 7461 6261 7365 0a69 6d66 702e 696d 665f  tabase.imfp.imf_
+00001dd0: 7061 7261 6d65 7465 725f 6465 6673 2822  parameter_defs("
+00001de0: 5043 5053 2229 0a60 6060 0a0a 0a0a 0a3c  PCPS").```.....<
+00001df0: 6469 763e 0a0a 3c74 6162 6c65 2062 6f72  div>..<table bor
+00001e00: 6465 723d 2231 2220 636c 6173 733d 2264  der="1" class="d
+00001e10: 6174 6166 7261 6d65 223e 0a20 203c 7468  ataframe">.  <th
+00001e20: 6561 643e 0a20 2020 203c 7472 2073 7479  ead>.    <tr sty
+00001e30: 6c65 3d22 7465 7874 2d61 6c69 676e 3a20  le="text-align: 
+00001e40: 7269 6768 743b 223e 0a20 2020 2020 203c  right;">.      <
+00001e50: 7468 3e3c 2f74 683e 0a20 2020 2020 203c  th></th>.      <
+00001e60: 7468 3e70 6172 616d 6574 6572 3c2f 7468  th>parameter</th
+00001e70: 3e0a 2020 2020 2020 3c74 683e 6465 7363  >.      <th>desc
+00001e80: 7269 7074 696f 6e3c 2f74 683e 0a20 2020  ription</th>.   
+00001e90: 203c 2f74 723e 0a20 203c 2f74 6865 6164   </tr>.  </thead
+00001ea0: 3e0a 2020 3c74 626f 6479 3e0a 2020 2020  >.  <tbody>.    
+00001eb0: 3c74 723e 0a20 2020 2020 203c 7468 3e30  <tr>.      <th>0
+00001ec0: 3c2f 7468 3e0a 2020 2020 2020 3c74 643e  </th>.      <td>
+00001ed0: 6672 6571 3c2f 7464 3e0a 2020 2020 2020  freq</td>.      
+00001ee0: 3c74 643e 4672 6571 7565 6e63 793c 2f74  <td>Frequency</t
+00001ef0: 643e 0a20 2020 203c 2f74 723e 0a20 2020  d>.    </tr>.   
+00001f00: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+00001f10: 313c 2f74 683e 0a20 2020 2020 203c 7464  1</th>.      <td
+00001f20: 3e72 6566 5f61 7265 613c 2f74 643e 0a20  >ref_area</td>. 
+00001f30: 2020 2020 203c 7464 3e47 656f 6772 6170       <td>Geograp
+00001f40: 6869 6361 6c20 4172 6561 733c 2f74 643e  hical Areas</td>
+00001f50: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00001f60: 7472 3e0a 2020 2020 2020 3c74 683e 323c  tr>.      <th>2<
+00001f70: 2f74 683e 0a20 2020 2020 203c 7464 3e63  /th>.      <td>c
+00001f80: 6f6d 6d6f 6469 7479 3c2f 7464 3e0a 2020  ommodity</td>.  
+00001f90: 2020 2020 3c74 643e 496e 6469 6361 746f      <td>Indicato
+00001fa0: 723c 2f74 643e 0a20 2020 203c 2f74 723e  r</td>.    </tr>
+00001fb0: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+00001fc0: 3c74 683e 333c 2f74 683e 0a20 2020 2020  <th>3</th>.     
+00001fd0: 203c 7464 3e75 6e69 745f 6d65 6173 7572   <td>unit_measur
+00001fe0: 653c 2f74 643e 0a20 2020 2020 203c 7464  e</td>.      <td
+00001ff0: 3e55 6e69 743c 2f74 643e 0a20 2020 203c  >Unit</td>.    <
+00002000: 2f74 723e 0a20 203c 2f74 626f 6479 3e0a  /tr>.  </tbody>.
+00002010: 3c2f 7461 626c 653e 0a3c 2f64 6976 3e0a  </table>.</div>.
+00002020: 0a0a 0a45 6163 6820 6e61 6d65 6420 6c69  ...Each named li
+00002030: 7374 2069 7465 6d20 6973 2061 2064 6174  st item is a dat
+00002040: 6120 6672 616d 6520 636f 6e74 6169 6e69  a frame containi
+00002050: 6e67 2061 2076 6563 746f 7220 6f66 2076  ng a vector of v
+00002060: 616c 6964 2069 6e70 7574 2063 6f64 6573  alid input codes
+00002070: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+00002080: 6420 7769 7468 2074 6865 206e 616d 6564  d with the named
+00002090: 2070 6172 616d 6574 6572 2c20 616e 6420   parameter, and 
+000020a0: 6120 7665 6374 6f72 206f 6620 7465 7874  a vector of text
+000020b0: 2064 6573 6372 6970 7469 6f6e 7320 6f66   descriptions of
+000020c0: 2077 6861 7420 6561 6368 2063 6f64 6520   what each code 
+000020d0: 7265 7072 6573 656e 7473 2e0a 0a54 6f20  represents...To 
+000020e0: 6163 6365 7373 2074 6865 2064 6174 6120  access the data 
+000020f0: 6672 616d 6520 636f 6e74 6169 6e69 6e67  frame containing
+00002100: 2076 616c 6964 2076 616c 7565 7320 666f   valid values fo
+00002110: 7220 6561 6368 2070 6172 616d 6574 6572  r each parameter
+00002120: 2c20 7375 6273 6574 2074 6865 2060 7061  , subset the `pa
+00002130: 7261 6d73 6020 6469 6374 2062 7920 7468  rams` dict by th
+00002140: 6520 7061 7261 6d65 7465 7220 6e61 6d65  e parameter name
+00002150: 3a0a 0a0a 6060 6070 7974 686f 6e0a 2320  :...```python.# 
+00002160: 5669 6577 2074 6865 2064 6174 6120 6672  View the data fr
+00002170: 616d 6520 6f66 2076 616c 6964 2069 6e70  ame of valid inp
+00002180: 7574 2063 6f64 6573 2066 6f72 2074 6865  ut codes for the
+00002190: 2066 7265 7175 656e 6379 2070 6172 616d   frequency param
+000021a0: 6574 6572 0a70 6172 616d 735b 2766 7265  eter.params['fre
+000021b0: 7127 5d0a 6060 600a 0a0a 0a0a 3c64 6976  q'].```.....<div
+000021c0: 3e0a 0a3c 7461 626c 6520 626f 7264 6572  >..<table border
+000021d0: 3d22 3122 2063 6c61 7373 3d22 6461 7461  ="1" class="data
+000021e0: 6672 616d 6522 3e0a 2020 3c74 6865 6164  frame">.  <thead
+000021f0: 3e0a 2020 2020 3c74 7220 7374 796c 653d  >.    <tr style=
+00002200: 2274 6578 742d 616c 6967 6e3a 2072 6967  "text-align: rig
+00002210: 6874 3b22 3e0a 2020 2020 2020 3c74 683e  ht;">.      <th>
+00002220: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+00002230: 696e 7075 745f 636f 6465 3c2f 7468 3e0a  input_code</th>.
+00002240: 2020 2020 2020 3c74 683e 6465 7363 7269        <th>descri
+00002250: 7074 696f 6e3c 2f74 683e 0a20 2020 203c  ption</th>.    <
+00002260: 2f74 723e 0a20 203c 2f74 6865 6164 3e0a  /tr>.  </thead>.
+00002270: 2020 3c74 626f 6479 3e0a 2020 2020 3c74    <tbody>.    <t
+00002280: 723e 0a20 2020 2020 203c 7468 3e30 3c2f  r>.      <th>0</
+00002290: 7468 3e0a 2020 2020 2020 3c74 643e 413c  th>.      <td>A<
+000022a0: 2f74 643e 0a20 2020 2020 203c 7464 3e41  /td>.      <td>A
+000022b0: 6e6e 7561 6c3c 2f74 643e 0a20 2020 203c  nnual</td>.    <
+000022c0: 2f74 723e 0a20 2020 203c 7472 3e0a 2020  /tr>.    <tr>.  
+000022d0: 2020 2020 3c74 683e 313c 2f74 683e 0a20      <th>1</th>. 
+000022e0: 2020 2020 203c 7464 3e4d 3c2f 7464 3e0a       <td>M</td>.
+000022f0: 2020 2020 2020 3c74 643e 4d6f 6e74 686c        <td>Monthl
+00002300: 793c 2f74 643e 0a20 2020 203c 2f74 723e  y</td>.    </tr>
+00002310: 0a20 2020 203c 7472 3e0a 2020 2020 2020  .    <tr>.      
+00002320: 3c74 683e 323c 2f74 683e 0a20 2020 2020  <th>2</th>.     
+00002330: 203c 7464 3e51 3c2f 7464 3e0a 2020 2020   <td>Q</td>.    
+00002340: 2020 3c74 643e 5175 6172 7465 726c 793c    <td>Quarterly<
+00002350: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00002360: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+00002370: 653e 0a3c 2f64 6976 3e0a 0a0a 0a23 2323  e>.</div>....###
+00002380: 2056 6965 7769 6e67 2044 6174 6120 4672   Viewing Data Fr
+00002390: 616d 6573 0a0a 4e6f 7465 2074 6861 7420  ames..Note that 
+000023a0: 6070 616e 6461 7360 2064 6174 6120 6672  `pandas` data fr
+000023b0: 616d 6573 2069 6e20 5079 7468 6f6e 2063  ames in Python c
+000023c0: 616e 2062 6520 6120 6c69 7474 6c65 2064  an be a little d
+000023d0: 6966 6669 6375 6c74 2074 6f20 776f 726b  ifficult to work
+000023e0: 2077 6974 682c 2062 6563 6175 7365 2050   with, because P
+000023f0: 7974 686f 6e20 646f 6573 6e27 7420 6861  ython doesn't ha
+00002400: 7665 2061 2062 7569 6c74 2d69 6e20 7661  ve a built-in va
+00002410: 7269 6162 6c65 2065 7870 6c6f 7265 722e  riable explorer.
+00002420: 2049 6620 796f 7527 7265 2064 6f69 6e67   If you're doing
+00002430: 2064 6174 6120 7363 6965 6e63 652c 2049   data science, I
+00002440: 2072 6563 6f6d 6d65 6e64 2075 7369 6e67   recommend using
+00002450: 2061 6e20 4944 4520 6c69 6b65 2052 5374   an IDE like RSt
+00002460: 7564 696f 206f 7220 5370 7964 6572 2074  udio or Spyder t
+00002470: 6861 7420 6861 7320 6120 6275 696c 742d  hat has a built-
+00002480: 696e 2076 6172 6961 626c 6520 6578 706c  in variable expl
+00002490: 6f72 6572 2e20 486f 7765 7665 722c 2069  orer. However, i
+000024a0: 6620 796f 7520 646f 6e27 7420 6861 7665  f you don't have
+000024b0: 2061 2076 6172 6961 626c 6520 6578 706c   a variable expl
+000024c0: 6f72 6572 2c20 796f 7520 6361 6e20 7072  orer, you can pr
+000024d0: 6576 656e 7420 5079 7468 6f6e 2066 726f  event Python fro
+000024e0: 6d20 7472 756e 6361 7469 6e67 2064 6174  m truncating dat
+000024f0: 6120 6672 616d 6573 2075 7369 6e67 2074  a frames using t
+00002500: 6865 2060 6f70 7469 6f6e 7360 2069 6e20  he `options` in 
+00002510: 6070 616e 6461 7360 2e20 466f 7220 696e  `pandas`. For in
+00002520: 7374 616e 6365 2c20 746f 2069 6e63 7265  stance, to incre
+00002530: 6173 6520 7468 6520 6d61 7869 6d75 6d20  ase the maximum 
+00002540: 616c 6c6f 7765 6420 636f 6c75 6d6e 2077  allowed column w
+00002550: 6964 7468 2074 6f20 3130 3020 6368 6172  idth to 100 char
+00002560: 6163 7465 7273 2c20 7765 2063 616e 2075  acters, we can u
+00002570: 7365 2060 7061 6e64 6173 2e6f 7074 696f  se `pandas.optio
+00002580: 6e73 2e64 6973 706c 6179 2e6d 6178 5f63  ns.display.max_c
+00002590: 6f6c 7769 6474 6820 3d20 3130 3060 2e0a  olwidth = 100`..
+000025a0: 0a41 6c74 6572 6e61 7469 7665 6c79 2c20  .Alternatively, 
+000025b0: 6974 2773 2070 6f73 7369 626c 6520 746f  it's possible to
+000025c0: 206f 7065 6e20 7468 6520 6461 7461 2066   open the data f
+000025d0: 7261 6d65 2069 6e20 6120 6e65 7720 7769  rame in a new wi
+000025e0: 6e64 6f77 2074 6f20 7669 6577 2069 7420  ndow to view it 
+000025f0: 696e 2066 756c 6c3a 0a0a 0a60 6060 7079  in full:...```py
+00002600: 7468 6f6e 0a69 6d70 6f72 7420 696d 6670  thon.import imfp
+00002610: 0a69 6d70 6f72 7420 7465 6d70 6669 6c65  .import tempfile
+00002620: 0a69 6d70 6f72 7420 7765 6262 726f 7773  .import webbrows
+00002630: 6572 0a0a 2320 4465 6669 6e65 2061 2073  er..# Define a s
+00002640: 696d 706c 6520 6675 6e63 7469 6f6e 2074  imple function t
+00002650: 6f20 7669 6577 2064 6174 6120 6672 616d  o view data fram
+00002660: 6520 696e 2061 2062 726f 7773 6572 2077  e in a browser w
+00002670: 696e 646f 770a 6465 6620 5669 6577 2864  indow.def View(d
+00002680: 6629 3a0a 2020 2020 6874 6d6c 203d 2064  f):.    html = d
+00002690: 662e 746f 5f68 746d 6c28 290a 2020 2020  f.to_html().    
+000026a0: 7769 7468 2074 656d 7066 696c 652e 4e61  with tempfile.Na
+000026b0: 6d65 6454 656d 706f 7261 7279 4669 6c65  medTemporaryFile
+000026c0: 2827 7727 2c20 6465 6c65 7465 3d46 616c  ('w', delete=Fal
+000026d0: 7365 2c20 7375 6666 6978 3d27 2e68 746d  se, suffix='.htm
+000026e0: 6c27 2920 6173 2066 3a0a 2020 2020 2020  l') as f:.      
+000026f0: 2020 7572 6c20 3d20 2766 696c 653a 2f2f    url = 'file://
+00002700: 2720 2b20 662e 6e61 6d65 0a20 2020 2020  ' + f.name.     
+00002710: 2020 2066 2e77 7269 7465 2868 746d 6c29     f.write(html)
+00002720: 0a20 2020 2077 6562 6272 6f77 7365 722e  .    webbrowser.
+00002730: 6f70 656e 2875 726c 290a 0a23 204f 7065  open(url)..# Ope
+00002740: 6e20 6461 7461 2066 7261 6d65 2069 6e20  n data frame in 
+00002750: 6120 6e65 7720 6272 6f77 7365 7220 7769  a new browser wi
+00002760: 6e64 6f77 2075 7369 6e67 2074 6865 2066  ndow using the f
+00002770: 756e 6374 696f 6e0a 6466 203d 2069 6d66  unction.df = imf
+00002780: 702e 696d 665f 6461 7461 6261 7365 7328  p.imf_databases(
+00002790: 290a 5669 6577 2864 6629 0a60 6060 0a0a  ).View(df).```..
+000027a0: 2323 2320 5375 7070 6c79 696e 6720 5061  ### Supplying Pa
+000027b0: 7261 6d65 7465 7220 4172 6775 6d65 6e74  rameter Argument
+000027c0: 7320 746f 2060 696d 665f 6461 7461 7365  s to `imf_datase
+000027d0: 7460 3a20 4120 5461 6c65 206f 6620 5477  t`: A Tale of Tw
+000027e0: 6f20 576f 726b 666c 6f77 730a 0a54 6865  o Workflows..The
+000027f0: 7265 2061 7265 2074 776f 2077 6179 7320  re are two ways 
+00002800: 746f 2073 7570 706c 7920 7061 7261 6d65  to supply parame
+00002810: 7465 7273 2074 6f20 6069 6d66 702e 696d  ters to `imfp.im
+00002820: 665f 6461 7461 7365 7460 3a20 6279 2073  f_dataset`: by s
+00002830: 7570 706c 7969 6e67 206c 6973 7420 6172  upplying list ar
+00002840: 6775 6d65 6e74 7320 6f72 2062 7920 7375  guments or by su
+00002850: 7070 6c79 696e 6720 6120 6d6f 6469 6669  pplying a modifi
+00002860: 6564 2070 6172 616d 6574 6572 7320 6469  ed parameters di
+00002870: 6374 2e20 5468 6520 6c69 7374 2061 7267  ct. The list arg
+00002880: 756d 656e 7473 2077 6f72 6b66 6c6f 7720  uments workflow 
+00002890: 7769 6c6c 2062 6520 6d6f 7265 2069 6e74  will be more int
+000028a0: 7569 7469 7665 2066 6f72 206d 6f73 7420  uitive for most 
+000028b0: 7573 6572 732c 2062 7574 2074 6865 2064  users, but the d
+000028c0: 6963 7420 6172 6775 6d65 6e74 2077 6f72  ict argument wor
+000028d0: 6b66 6c6f 7720 7265 7175 6972 6573 2061  kflow requires a
+000028e0: 206c 6974 746c 6520 6c65 7373 2063 6f64   little less cod
+000028f0: 652e 0a0a 2323 2323 2054 6865 204c 6973  e...#### The Lis
+00002900: 7420 4172 6775 6d65 6e74 7320 576f 726b  t Arguments Work
+00002910: 666c 6f77 0a0a 546f 2073 7570 706c 7920  flow..To supply 
+00002920: 6c69 7374 2061 7267 756d 656e 7473 2c20  list arguments, 
+00002930: 6a75 7374 2066 696e 6420 7468 6520 636f  just find the co
+00002940: 6465 7320 796f 7520 7761 6e74 2061 6e64  des you want and
+00002950: 2073 7570 706c 7920 7468 656d 2074 6f20   supply them to 
+00002960: 6069 6d66 702e 696d 665f 6461 7461 7365  `imfp.imf_datase
+00002970: 7460 2075 7369 6e67 2074 6865 2070 6172  t` using the par
+00002980: 616d 6574 6572 206e 616d 6520 6173 2074  ameter name as t
+00002990: 6865 2061 7267 756d 656e 7420 6e61 6d65  he argument name
+000029a0: 2e20 5468 6520 6578 616d 706c 6520 6265  . The example be
+000029b0: 6c6f 7720 7368 6f77 7320 686f 7720 746f  low shows how to
+000029c0: 2072 6571 7565 7374 2032 3030 30e2 8093   request 2000...
+000029d0: 3230 3135 2061 6e6e 7561 6c20 636f 616c  2015 annual coal
+000029e0: 2070 7269 6365 7320 6672 6f6d 2074 6865   prices from the
+000029f0: 2050 7269 6d61 7279 2043 6f6d 6d6f 6469   Primary Commodi
+00002a00: 7479 2050 7269 6365 2053 7973 7465 6d20  ty Price System 
+00002a10: 6461 7461 6261 7365 3a0a 0a0a 6060 6070  database:...```p
+00002a20: 7974 686f 6e0a 2320 4665 7463 6820 7468  ython.# Fetch th
+00002a30: 6520 2766 7265 7127 2069 6e70 7574 2063  e 'freq' input c
+00002a40: 6f64 6520 666f 7220 616e 6e75 616c 2066  ode for annual f
+00002a50: 7265 7175 656e 6379 0a73 656c 6563 7465  requency.selecte
+00002a60: 645f 6672 6571 203d 206c 6973 7428 0a20  d_freq = list(. 
+00002a70: 2020 2070 6172 616d 735b 2766 7265 7127     params['freq'
+00002a80: 5d5b 2769 6e70 7574 5f63 6f64 6527 5d5b  ]['input_code'][
+00002a90: 7061 7261 6d73 5b27 6672 6571 275d 5b27  params['freq']['
+00002aa0: 6465 7363 7269 7074 696f 6e27 5d2e 7374  description'].st
+00002ab0: 722e 636f 6e74 6169 6e73 2822 416e 6e75  r.contains("Annu
+00002ac0: 616c 2229 5d0a 290a 0a23 2046 6574 6368  al")].)..# Fetch
+00002ad0: 2074 6865 2027 636f 6d6d 6f64 6974 7927   the 'commodity'
+00002ae0: 2069 6e70 7574 2063 6f64 6520 666f 7220   input code for 
+00002af0: 636f 616c 0a73 656c 6563 7465 645f 636f  coal.selected_co
+00002b00: 6d6d 6f64 6974 7920 3d20 6c69 7374 280a  mmodity = list(.
+00002b10: 2020 2020 7061 7261 6d73 5b27 636f 6d6d      params['comm
+00002b20: 6f64 6974 7927 5d5b 2769 6e70 7574 5f63  odity']['input_c
+00002b30: 6f64 6527 5d5b 7061 7261 6d73 5b27 636f  ode'][params['co
+00002b40: 6d6d 6f64 6974 7927 5d5b 2764 6573 6372  mmodity']['descr
+00002b50: 6970 7469 6f6e 275d 2e73 7472 2e63 6f6e  iption'].str.con
+00002b60: 7461 696e 7328 2243 6f61 6c22 295d 0a29  tains("Coal")].)
+00002b70: 0a0a 2320 4665 7463 6820 7468 6520 2775  ..# Fetch the 'u
+00002b80: 6e69 745f 6d65 6173 7572 6527 2069 6e70  nit_measure' inp
+00002b90: 7574 2063 6f64 6520 666f 7220 696e 6465  ut code for inde
+00002ba0: 780a 7365 6c65 6374 6564 5f75 6e69 745f  x.selected_unit_
+00002bb0: 6d65 6173 7572 6520 3d20 6c69 7374 280a  measure = list(.
+00002bc0: 2020 2020 7061 7261 6d73 5b27 756e 6974      params['unit
+00002bd0: 5f6d 6561 7375 7265 275d 5b27 696e 7075  _measure']['inpu
+00002be0: 745f 636f 6465 275d 5b70 6172 616d 735b  t_code'][params[
+00002bf0: 2775 6e69 745f 6d65 6173 7572 6527 5d5b  'unit_measure'][
+00002c00: 2764 6573 6372 6970 7469 6f6e 275d 2e73  'description'].s
+00002c10: 7472 2e63 6f6e 7461 696e 7328 2249 6e64  tr.contains("Ind
+00002c20: 6578 2229 5d0a 290a 0a23 2052 6571 7565  ex")].)..# Reque
+00002c30: 7374 2064 6174 6120 6672 6f6d 2074 6865  st data from the
+00002c40: 2041 5049 0a64 6620 3d20 696d 6670 2e69   API.df = imfp.i
+00002c50: 6d66 5f64 6174 6173 6574 2864 6174 6162  mf_dataset(datab
+00002c60: 6173 655f 6964 203d 2022 5043 5053 222c  ase_id = "PCPS",
+00002c70: 0a20 2020 2020 2020 2020 6672 6571 203d  .         freq =
+00002c80: 2073 656c 6563 7465 645f 6672 6571 2c20   selected_freq, 
+00002c90: 636f 6d6d 6f64 6974 7920 3d20 7365 6c65  commodity = sele
+00002ca0: 6374 6564 5f63 6f6d 6d6f 6469 7479 2c0a  cted_commodity,.
+00002cb0: 2020 2020 2020 2020 2075 6e69 745f 6d65           unit_me
+00002cc0: 6173 7572 6520 3d20 7365 6c65 6374 6564  asure = selected
+00002cd0: 5f75 6e69 745f 6d65 6173 7572 652c 0a20  _unit_measure,. 
+00002ce0: 2020 2020 2020 2020 7374 6172 745f 7965          start_ye
+00002cf0: 6172 203d 2032 3030 302c 2065 6e64 5f79  ar = 2000, end_y
+00002d00: 6561 7220 3d20 3230 3135 290a 0a23 2044  ear = 2015)..# D
+00002d10: 6973 706c 6179 2074 6865 2066 6972 7374  isplay the first
+00002d20: 2066 6577 2065 6e74 7269 6573 2069 6e20   few entries in 
+00002d30: 7468 6520 7265 7472 6965 7665 6420 6461  the retrieved da
+00002d40: 7461 2066 7261 6d65 0a64 662e 6865 6164  ta frame.df.head
+00002d50: 2829 0a60 6060 0a0a 0a0a 0a3c 6469 763e  ().```.....<div>
+00002d60: 0a0a 3c74 6162 6c65 2062 6f72 6465 723d  ..<table border=
+00002d70: 2231 2220 636c 6173 733d 2264 6174 6166  "1" class="dataf
+00002d80: 7261 6d65 223e 0a20 203c 7468 6561 643e  rame">.  <thead>
+00002d90: 0a20 2020 203c 7472 2073 7479 6c65 3d22  .    <tr style="
+00002da0: 7465 7874 2d61 6c69 676e 3a20 7269 6768  text-align: righ
+00002db0: 743b 223e 0a20 2020 2020 203c 7468 3e3c  t;">.      <th><
+00002dc0: 2f74 683e 0a20 2020 2020 203c 7468 3e66  /th>.      <th>f
+00002dd0: 7265 713c 2f74 683e 0a20 2020 2020 203c  req</th>.      <
+00002de0: 7468 3e72 6566 5f61 7265 613c 2f74 683e  th>ref_area</th>
+00002df0: 0a20 2020 2020 203c 7468 3e63 6f6d 6d6f  .      <th>commo
+00002e00: 6469 7479 3c2f 7468 3e0a 2020 2020 2020  dity</th>.      
+00002e10: 3c74 683e 756e 6974 5f6d 6561 7375 7265  <th>unit_measure
+00002e20: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+00002e30: 756e 6974 5f6d 756c 743c 2f74 683e 0a20  unit_mult</th>. 
+00002e40: 2020 2020 203c 7468 3e74 696d 655f 666f       <th>time_fo
+00002e50: 726d 6174 3c2f 7468 3e0a 2020 2020 2020  rmat</th>.      
+00002e60: 3c74 683e 7469 6d65 5f70 6572 696f 643c  <th>time_period<
+00002e70: 2f74 683e 0a20 2020 2020 203c 7468 3e6f  /th>.      <th>o
+00002e80: 6273 5f76 616c 7565 3c2f 7468 3e0a 2020  bs_value</th>.  
+00002e90: 2020 3c2f 7472 3e0a 2020 3c2f 7468 6561    </tr>.  </thea
+00002ea0: 643e 0a20 203c 7462 6f64 793e 0a20 2020  d>.  <tbody>.   
+00002eb0: 203c 7472 3e0a 2020 2020 2020 3c74 683e   <tr>.      <th>
+00002ec0: 303c 2f74 683e 0a20 2020 2020 203c 7464  0</th>.      <td
+00002ed0: 3e41 3c2f 7464 3e0a 2020 2020 2020 3c74  >A</td>.      <t
+00002ee0: 643e 5730 303c 2f74 643e 0a20 2020 2020  d>W00</td>.     
+00002ef0: 203c 7464 3e50 434f 414c 3c2f 7464 3e0a   <td>PCOAL</td>.
+00002f00: 2020 2020 2020 3c74 643e 4958 3c2f 7464        <td>IX</td
+00002f10: 3e0a 2020 2020 2020 3c74 643e 303c 2f74  >.      <td>0</t
+00002f20: 643e 0a20 2020 2020 203c 7464 3e50 3159  d>.      <td>P1Y
+00002f30: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00002f40: 3230 3030 3c2f 7464 3e0a 2020 2020 2020  2000</td>.      
+00002f50: 3c74 643e 3339 2e33 3531 3032 3330 3239  <td>39.351023029
+00002f60: 3332 3032 3c2f 7464 3e0a 2020 2020 3c2f  3202</td>.    </
+00002f70: 7472 3e0a 2020 2020 3c74 723e 0a20 2020  tr>.    <tr>.   
+00002f80: 2020 203c 7468 3e31 3c2f 7468 3e0a 2020     <th>1</th>.  
+00002f90: 2020 2020 3c74 643e 413c 2f74 643e 0a20      <td>A</td>. 
+00002fa0: 2020 2020 203c 7464 3e57 3030 3c2f 7464       <td>W00</td
+00002fb0: 3e0a 2020 2020 2020 3c74 643e 5043 4f41  >.      <td>PCOA
+00002fc0: 4c3c 2f74 643e 0a20 2020 2020 203c 7464  L</td>.      <td
+00002fd0: 3e49 583c 2f74 643e 0a20 2020 2020 203c  >IX</td>.      <
+00002fe0: 7464 3e30 3c2f 7464 3e0a 2020 2020 2020  td>0</td>.      
+00002ff0: 3c74 643e 5031 593c 2f74 643e 0a20 2020  <td>P1Y</td>.   
+00003000: 2020 203c 7464 3e32 3030 313c 2f74 643e     <td>2001</td>
+00003010: 0a20 2020 2020 203c 7464 3e34 392e 3333  .      <td>49.33
+00003020: 3738 3538 3732 3834 3033 393c 2f74 643e  78587284039</td>
+00003030: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+00003040: 7472 3e0a 2020 2020 2020 3c74 683e 323c  tr>.      <th>2<
+00003050: 2f74 683e 0a20 2020 2020 203c 7464 3e41  /th>.      <td>A
+00003060: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00003070: 5730 303c 2f74 643e 0a20 2020 2020 203c  W00</td>.      <
+00003080: 7464 3e50 434f 414c 3c2f 7464 3e0a 2020  td>PCOAL</td>.  
+00003090: 2020 2020 3c74 643e 4958 3c2f 7464 3e0a      <td>IX</td>.
+000030a0: 2020 2020 2020 3c74 643e 303c 2f74 643e        <td>0</td>
+000030b0: 0a20 2020 2020 203c 7464 3e50 3159 3c2f  .      <td>P1Y</
+000030c0: 7464 3e0a 2020 2020 2020 3c74 643e 3230  td>.      <td>20
+000030d0: 3032 3c2f 7464 3e0a 2020 2020 2020 3c74  02</td>.      <t
+000030e0: 643e 3339 2e34 3934 3930 3931 3634 3830  d>39.49490916480
+000030f0: 3036 3c2f 7464 3e0a 2020 2020 3c2f 7472  06</td>.    </tr
+00003100: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00003110: 203c 7468 3e33 3c2f 7468 3e0a 2020 2020   <th>3</th>.    
+00003120: 2020 3c74 643e 413c 2f74 643e 0a20 2020    <td>A</td>.   
+00003130: 2020 203c 7464 3e57 3030 3c2f 7464 3e0a     <td>W00</td>.
+00003140: 2020 2020 2020 3c74 643e 5043 4f41 4c3c        <td>PCOAL<
+00003150: 2f74 643e 0a20 2020 2020 203c 7464 3e49  /td>.      <td>I
+00003160: 583c 2f74 643e 0a20 2020 2020 203c 7464  X</td>.      <td
+00003170: 3e30 3c2f 7464 3e0a 2020 2020 2020 3c74  >0</td>.      <t
+00003180: 643e 5031 593c 2f74 643e 0a20 2020 2020  d>P1Y</td>.     
+00003190: 203c 7464 3e32 3030 333c 2f74 643e 0a20   <td>2003</td>. 
+000031a0: 2020 2020 203c 7464 3e34 332e 3238 3738       <td>43.2878
+000031b0: 3837 3639 3530 3738 383c 2f74 643e 0a20  876950788</td>. 
+000031c0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000031d0: 3e0a 2020 2020 2020 3c74 683e 343c 2f74  >.      <th>4</t
+000031e0: 683e 0a20 2020 2020 203c 7464 3e41 3c2f  h>.      <td>A</
+000031f0: 7464 3e0a 2020 2020 2020 3c74 643e 5730  td>.      <td>W0
+00003200: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+00003210: 3e50 434f 414c 3c2f 7464 3e0a 2020 2020  >PCOAL</td>.    
+00003220: 2020 3c74 643e 4958 3c2f 7464 3e0a 2020    <td>IX</td>.  
+00003230: 2020 2020 3c74 643e 303c 2f74 643e 0a20      <td>0</td>. 
+00003240: 2020 2020 203c 7464 3e50 3159 3c2f 7464       <td>P1Y</td
+00003250: 3e0a 2020 2020 2020 3c74 643e 3230 3034  >.      <td>2004
+00003260: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00003270: 3832 2e39 3138 3538 3538 3035 3238 3632  82.9185858052862
+00003280: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00003290: 2020 3c2f 7462 6f64 793e 0a3c 2f74 6162    </tbody>.</tab
+000032a0: 6c65 3e0a 3c2f 6469 763e 0a0a 0a0a 2323  le>.</div>....##
+000032b0: 2323 2054 6865 2050 6172 616d 6574 6572  ## The Parameter
+000032c0: 7320 4172 6775 6d65 6e74 2057 6f72 6b66  s Argument Workf
+000032d0: 6c6f 770a 0a54 6f20 7375 7070 6c79 2061  low..To supply a
+000032e0: 206c 6973 7420 6f62 6a65 6374 2c20 6d6f   list object, mo
+000032f0: 6469 6679 2065 6163 6820 6461 7461 2066  dify each data f
+00003300: 7261 6d65 2069 6e20 7468 6520 6070 6172  rame in the `par
+00003310: 616d 7360 206c 6973 7420 6f62 6a65 6374  ams` list object
+00003320: 2074 6f20 7265 7461 696e 206f 6e6c 7920   to retain only 
+00003330: 7468 6520 726f 7773 2079 6f75 2077 616e  the rows you wan
+00003340: 742c 2061 6e64 2074 6865 6e20 7375 7070  t, and then supp
+00003350: 6c79 2074 6865 206d 6f64 6966 6965 6420  ly the modified 
+00003360: 6c69 7374 206f 626a 6563 7420 746f 2060  list object to `
+00003370: 696d 6670 2e69 6d66 5f64 6174 6173 6574  imfp.imf_dataset
+00003380: 6020 6173 2069 7473 2070 6172 616d 6574  ` as its paramet
+00003390: 6572 7320 6172 6775 6d65 6e74 2e20 4865  ers argument. He
+000033a0: 7265 2069 7320 686f 7720 746f 206d 616b  re is how to mak
+000033b0: 6520 7468 6520 7361 6d65 2072 6571 7565  e the same reque
+000033c0: 7374 2066 6f72 2061 6e6e 7561 6c20 636f  st for annual co
+000033d0: 616c 2070 7269 6365 2064 6174 6120 7573  al price data us
+000033e0: 696e 6720 6120 7061 7261 6d65 7465 7273  ing a parameters
+000033f0: 206c 6973 743a 0a0a 0a60 6060 7079 7468   list:...```pyth
+00003400: 6f6e 0a23 2046 6574 6368 2074 6865 2027  on.# Fetch the '
+00003410: 6672 6571 2720 696e 7075 7420 636f 6465  freq' input code
+00003420: 2066 6f72 2061 6e6e 7561 6c20 6672 6571   for annual freq
+00003430: 7565 6e63 790a 7061 7261 6d73 5b27 6672  uency.params['fr
+00003440: 6571 275d 203d 2070 6172 616d 735b 2766  eq'] = params['f
+00003450: 7265 7127 5d5b 7061 7261 6d73 5b27 6672  req'][params['fr
+00003460: 6571 275d 5b27 6465 7363 7269 7074 696f  eq']['descriptio
+00003470: 6e27 5d2e 7374 722e 636f 6e74 6169 6e73  n'].str.contains
+00003480: 2822 416e 6e75 616c 2229 5d0a 0a23 2046  ("Annual")]..# F
+00003490: 6574 6368 2074 6865 2027 636f 6d6d 6f64  etch the 'commod
+000034a0: 6974 7927 2069 6e70 7574 2063 6f64 6528  ity' input code(
+000034b0: 7329 2066 6f72 2063 6f61 6c0a 7061 7261  s) for coal.para
+000034c0: 6d73 5b27 636f 6d6d 6f64 6974 7927 5d20  ms['commodity'] 
+000034d0: 3d20 7061 7261 6d73 5b27 636f 6d6d 6f64  = params['commod
+000034e0: 6974 7927 5d5b 7061 7261 6d73 5b27 636f  ity'][params['co
+000034f0: 6d6d 6f64 6974 7927 5d5b 2764 6573 6372  mmodity']['descr
+00003500: 6970 7469 6f6e 275d 2e73 7472 2e63 6f6e  iption'].str.con
+00003510: 7461 696e 7328 2243 6f61 6c22 295d 0a0a  tains("Coal")]..
+00003520: 2320 4665 7463 6820 7468 6520 2775 6e69  # Fetch the 'uni
+00003530: 745f 6d65 6173 7572 6527 2069 6e70 7574  t_measure' input
+00003540: 2063 6f64 6520 666f 7220 696e 6465 780a   code for index.
+00003550: 7061 7261 6d73 5b27 756e 6974 5f6d 6561  params['unit_mea
+00003560: 7375 7265 275d 203d 2070 6172 616d 735b  sure'] = params[
+00003570: 2775 6e69 745f 6d65 6173 7572 6527 5d5b  'unit_measure'][
+00003580: 7061 7261 6d73 5b27 756e 6974 5f6d 6561  params['unit_mea
+00003590: 7375 7265 275d 5b27 6465 7363 7269 7074  sure']['descript
+000035a0: 696f 6e27 5d2e 7374 722e 636f 6e74 6169  ion'].str.contai
+000035b0: 6e73 2822 496e 6465 7822 295d 0a0a 2320  ns("Index")]..# 
+000035c0: 5265 7175 6573 7420 6461 7461 2066 726f  Request data fro
+000035d0: 6d20 7468 6520 4150 490a 6466 203d 2069  m the API.df = i
+000035e0: 6d66 702e 696d 665f 6461 7461 7365 7428  mfp.imf_dataset(
+000035f0: 6461 7461 6261 7365 5f69 6420 3d20 2250  database_id = "P
+00003600: 4350 5322 2c0a 2020 2020 2020 2020 2070  CPS",.         p
+00003610: 6172 616d 6574 6572 7320 3d20 7061 7261  arameters = para
+00003620: 6d73 2c0a 2020 2020 2020 2020 2073 7461  ms,.         sta
+00003630: 7274 5f79 6561 7220 3d20 3230 3030 2c20  rt_year = 2000, 
+00003640: 656e 645f 7965 6172 203d 2032 3031 3529  end_year = 2015)
+00003650: 0a0a 2320 4469 7370 6c61 7920 7468 6520  ..# Display the 
+00003660: 6669 7273 7420 6665 7720 656e 7472 6965  first few entrie
+00003670: 7320 696e 2074 6865 2072 6574 7269 6576  s in the retriev
+00003680: 6564 2064 6174 6120 6672 616d 650a 6466  ed data frame.df
+00003690: 2e68 6561 6428 290a 6060 600a 0a0a 0a0a  .head().```.....
+000036a0: 3c64 6976 3e0a 0a3c 7461 626c 6520 626f  <div>..<table bo
+000036b0: 7264 6572 3d22 3122 2063 6c61 7373 3d22  rder="1" class="
+000036c0: 6461 7461 6672 616d 6522 3e0a 2020 3c74  dataframe">.  <t
+000036d0: 6865 6164 3e0a 2020 2020 3c74 7220 7374  head>.    <tr st
+000036e0: 796c 653d 2274 6578 742d 616c 6967 6e3a  yle="text-align:
+000036f0: 2072 6967 6874 3b22 3e0a 2020 2020 2020   right;">.      
+00003700: 3c74 683e 3c2f 7468 3e0a 2020 2020 2020  <th></th>.      
+00003710: 3c74 683e 6672 6571 3c2f 7468 3e0a 2020  <th>freq</th>.  
+00003720: 2020 2020 3c74 683e 7265 665f 6172 6561      <th>ref_area
+00003730: 3c2f 7468 3e0a 2020 2020 2020 3c74 683e  </th>.      <th>
+00003740: 636f 6d6d 6f64 6974 793c 2f74 683e 0a20  commodity</th>. 
+00003750: 2020 2020 203c 7468 3e75 6e69 745f 6d65       <th>unit_me
+00003760: 6173 7572 653c 2f74 683e 0a20 2020 2020  asure</th>.     
+00003770: 203c 7468 3e75 6e69 745f 6d75 6c74 3c2f   <th>unit_mult</
+00003780: 7468 3e0a 2020 2020 2020 3c74 683e 7469  th>.      <th>ti
+00003790: 6d65 5f66 6f72 6d61 743c 2f74 683e 0a20  me_format</th>. 
+000037a0: 2020 2020 203c 7468 3e74 696d 655f 7065       <th>time_pe
+000037b0: 7269 6f64 3c2f 7468 3e0a 2020 2020 2020  riod</th>.      
+000037c0: 3c74 683e 6f62 735f 7661 6c75 653c 2f74  <th>obs_value</t
+000037d0: 683e 0a20 2020 203c 2f74 723e 0a20 203c  h>.    </tr>.  <
+000037e0: 2f74 6865 6164 3e0a 2020 3c74 626f 6479  /thead>.  <tbody
+000037f0: 3e0a 2020 2020 3c74 723e 0a20 2020 2020  >.    <tr>.     
+00003800: 203c 7468 3e30 3c2f 7468 3e0a 2020 2020   <th>0</th>.    
+00003810: 2020 3c74 643e 413c 2f74 643e 0a20 2020    <td>A</td>.   
+00003820: 2020 203c 7464 3e57 3030 3c2f 7464 3e0a     <td>W00</td>.
+00003830: 2020 2020 2020 3c74 643e 5043 4f41 4c3c        <td>PCOAL<
+00003840: 2f74 643e 0a20 2020 2020 203c 7464 3e49  /td>.      <td>I
+00003850: 583c 2f74 643e 0a20 2020 2020 203c 7464  X</td>.      <td
+00003860: 3e30 3c2f 7464 3e0a 2020 2020 2020 3c74  >0</td>.      <t
+00003870: 643e 5031 593c 2f74 643e 0a20 2020 2020  d>P1Y</td>.     
+00003880: 203c 7464 3e32 3030 303c 2f74 643e 0a20   <td>2000</td>. 
+00003890: 2020 2020 203c 7464 3e33 392e 3335 3130       <td>39.3510
+000038a0: 3233 3032 3933 3230 323c 2f74 643e 0a20  230293202</td>. 
+000038b0: 2020 203c 2f74 723e 0a20 2020 203c 7472     </tr>.    <tr
+000038c0: 3e0a 2020 2020 2020 3c74 683e 313c 2f74  >.      <th>1</t
+000038d0: 683e 0a20 2020 2020 203c 7464 3e41 3c2f  h>.      <td>A</
+000038e0: 7464 3e0a 2020 2020 2020 3c74 643e 5730  td>.      <td>W0
+000038f0: 303c 2f74 643e 0a20 2020 2020 203c 7464  0</td>.      <td
+00003900: 3e50 434f 414c 3c2f 7464 3e0a 2020 2020  >PCOAL</td>.    
+00003910: 2020 3c74 643e 4958 3c2f 7464 3e0a 2020    <td>IX</td>.  
+00003920: 2020 2020 3c74 643e 303c 2f74 643e 0a20      <td>0</td>. 
+00003930: 2020 2020 203c 7464 3e50 3159 3c2f 7464       <td>P1Y</td
+00003940: 3e0a 2020 2020 2020 3c74 643e 3230 3031  >.      <td>2001
+00003950: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00003960: 3439 2e33 3337 3835 3837 3238 3430 3339  49.3378587284039
+00003970: 3c2f 7464 3e0a 2020 2020 3c2f 7472 3e0a  </td>.    </tr>.
+00003980: 2020 2020 3c74 723e 0a20 2020 2020 203c      <tr>.      <
+00003990: 7468 3e32 3c2f 7468 3e0a 2020 2020 2020  th>2</th>.      
+000039a0: 3c74 643e 413c 2f74 643e 0a20 2020 2020  <td>A</td>.     
+000039b0: 203c 7464 3e57 3030 3c2f 7464 3e0a 2020   <td>W00</td>.  
+000039c0: 2020 2020 3c74 643e 5043 4f41 4c3c 2f74      <td>PCOAL</t
+000039d0: 643e 0a20 2020 2020 203c 7464 3e49 583c  d>.      <td>IX<
+000039e0: 2f74 643e 0a20 2020 2020 203c 7464 3e30  /td>.      <td>0
+000039f0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00003a00: 5031 593c 2f74 643e 0a20 2020 2020 203c  P1Y</td>.      <
+00003a10: 7464 3e32 3030 323c 2f74 643e 0a20 2020  td>2002</td>.   
+00003a20: 2020 203c 7464 3e33 392e 3439 3439 3039     <td>39.494909
+00003a30: 3136 3438 3030 363c 2f74 643e 0a20 2020  1648006</td>.   
+00003a40: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+00003a50: 2020 2020 2020 3c74 683e 333c 2f74 683e        <th>3</th>
+00003a60: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
+00003a70: 3e0a 2020 2020 2020 3c74 643e 5730 303c  >.      <td>W00<
+00003a80: 2f74 643e 0a20 2020 2020 203c 7464 3e50  /td>.      <td>P
+00003a90: 434f 414c 3c2f 7464 3e0a 2020 2020 2020  COAL</td>.      
+00003aa0: 3c74 643e 4958 3c2f 7464 3e0a 2020 2020  <td>IX</td>.    
+00003ab0: 2020 3c74 643e 303c 2f74 643e 0a20 2020    <td>0</td>.   
+00003ac0: 2020 203c 7464 3e50 3159 3c2f 7464 3e0a     <td>P1Y</td>.
+00003ad0: 2020 2020 2020 3c74 643e 3230 3033 3c2f        <td>2003</
+00003ae0: 7464 3e0a 2020 2020 2020 3c74 643e 3433  td>.      <td>43
+00003af0: 2e32 3837 3838 3736 3935 3037 3838 3c2f  .2878876950788</
+00003b00: 7464 3e0a 2020 2020 3c2f 7472 3e0a 2020  td>.    </tr>.  
+00003b10: 2020 3c74 723e 0a20 2020 2020 203c 7468    <tr>.      <th
+00003b20: 3e34 3c2f 7468 3e0a 2020 2020 2020 3c74  >4</th>.      <t
+00003b30: 643e 413c 2f74 643e 0a20 2020 2020 203c  d>A</td>.      <
+00003b40: 7464 3e57 3030 3c2f 7464 3e0a 2020 2020  td>W00</td>.    
+00003b50: 2020 3c74 643e 5043 4f41 4c3c 2f74 643e    <td>PCOAL</td>
+00003b60: 0a20 2020 2020 203c 7464 3e49 583c 2f74  .      <td>IX</t
+00003b70: 643e 0a20 2020 2020 203c 7464 3e30 3c2f  d>.      <td>0</
+00003b80: 7464 3e0a 2020 2020 2020 3c74 643e 5031  td>.      <td>P1
+00003b90: 593c 2f74 643e 0a20 2020 2020 203c 7464  Y</td>.      <td
+00003ba0: 3e32 3030 343c 2f74 643e 0a20 2020 2020  >2004</td>.     
+00003bb0: 203c 7464 3e38 322e 3931 3835 3835 3830   <td>82.91858580
+00003bc0: 3532 3836 323c 2f74 643e 0a20 2020 203c  52862</td>.    <
+00003bd0: 2f74 723e 0a20 203c 2f74 626f 6479 3e0a  /tr>.  </tbody>.
+00003be0: 3c2f 7461 626c 653e 0a3c 2f64 6976 3e0a  </table>.</div>.
+00003bf0: 0a0a 0a23 2320 576f 726b 696e 6720 7769  ...## Working wi
+00003c00: 7468 2074 6865 2052 6574 7572 6e65 6420  th the Returned 
+00003c10: 4461 7461 2046 7261 6d65 0a0a 4e6f 7465  Data Frame..Note
+00003c20: 2074 6861 7420 616c 6c20 636f 6c75 6d6e   that all column
+00003c30: 7320 696e 2074 6865 2072 6574 7572 6e65  s in the returne
+00003c40: 6420 6461 7461 2066 7261 6d65 2061 7265  d data frame are
+00003c50: 2063 6861 7261 6374 6572 2076 6563 746f   character vecto
+00003c60: 7273 2c20 616e 6420 7468 6174 2074 6f20  rs, and that to 
+00003c70: 706c 6f74 2074 6865 2073 6572 6965 7320  plot the series 
+00003c80: 7765 2077 696c 6c20 6e65 6564 2074 6f20  we will need to 
+00003c90: 636f 6e76 6572 7420 746f 2076 616c 6964  convert to valid
+00003ca0: 206e 756d 6572 6963 206f 7220 6461 7465   numeric or date
+00003cb0: 2066 6f72 6d61 7473 2e20 5573 696e 6720   formats. Using 
+00003cc0: 6073 6561 626f 726e 6020 7769 7468 2060  `seaborn` with `
+00003cd0: 6875 6560 2c20 7765 2063 616e 2070 6c6f  hue`, we can plo
+00003ce0: 7420 6469 6666 6572 656e 7420 696e 6469  t different indi
+00003cf0: 6361 746f 7273 2069 6e20 6469 6666 6572  cators in differ
+00003d00: 656e 7420 636f 6c6f 7273 3a0a 0a0a 6060  ent colors:...``
+00003d10: 6070 7974 686f 6e0a 2320 436f 6e76 6572  `python.# Conver
+00003d20: 7420 6f62 735f 7661 6c75 6520 746f 206e  t obs_value to n
+00003d30: 756d 6572 6963 2061 6e64 2074 696d 655f  umeric and time_
+00003d40: 7065 7269 6f64 2074 6f20 696e 7465 6765  period to intege
+00003d50: 7220 7965 6172 0a64 6620 3d20 6466 2e61  r year.df = df.a
+00003d60: 7374 7970 6528 7b22 7469 6d65 5f70 6572  stype({"time_per
+00003d70: 696f 6422 203a 2069 6e74 2c20 226f 6273  iod" : int, "obs
+00003d80: 5f76 616c 7565 2220 3a20 666c 6f61 747d  _value" : float}
+00003d90: 290a 0a23 2050 6c6f 7420 7072 6963 6573  )..# Plot prices
+00003da0: 206f 6620 6469 6666 6572 656e 7420 636f   of different co
+00003db0: 6d6d 6f64 6974 6965 7320 696e 2064 6966  mmodities in dif
+00003dc0: 6665 7265 6e74 2063 6f6c 6f72 7320 7769  ferent colors wi
+00003dd0: 7468 2073 6561 626f 726e 0a73 6561 626f  th seaborn.seabo
+00003de0: 726e 2e6c 696e 6570 6c6f 7428 6461 7461  rn.lineplot(data
+00003df0: 3d64 662c 2078 3d27 7469 6d65 5f70 6572  =df, x='time_per
+00003e00: 696f 6427 2c20 793d 276f 6273 5f76 616c  iod', y='obs_val
+00003e10: 7565 272c 2068 7565 3d27 636f 6d6d 6f64  ue', hue='commod
+00003e20: 6974 7927 293b 0a60 6060 0a0a 0a20 2020  ity');.```...   
+00003e30: 200a 215b 706e 675d 2852 4541 444d 455f   .![png](README_
+00003e40: 6669 6c65 732f 706c 6f74 2e70 6e67 290a  files/plot.png).
+00003e50: 2020 2020 0a0a 0a0a 416c 736f 206e 6f74      ....Also not
+00003e60: 6520 7468 6174 2074 6865 2072 6574 7572  e that the retur
+00003e70: 6e65 6420 6461 7461 2066 7261 6d65 2068  ned data frame h
+00003e80: 6173 206d 7973 7465 7269 6f75 732d 6c6f  as mysterious-lo
+00003e90: 6f6b 696e 6720 636f 6465 7320 6173 2076  oking codes as v
+00003ea0: 616c 7565 7320 696e 2073 6f6d 6520 636f  alues in some co
+00003eb0: 6c75 6d6e 732e 0a0a 436f 6465 7320 696e  lumns...Codes in
+00003ec0: 2074 6865 2060 7469 6d65 5f66 6f72 6d61   the `time_forma
+00003ed0: 7460 2063 6f6c 756d 6e20 6172 6520 4953  t` column are IS
+00003ee0: 4f20 3836 3031 2064 7572 6174 696f 6e20  O 8601 duration 
+00003ef0: 636f 6465 732e 2049 6e20 7468 6973 2063  codes. In this c
+00003f00: 6173 652c 20e2 809c 5031 59e2 809d 206d  ase, ...P1Y... m
+00003f10: 6561 6e73 20e2 809c 7065 7269 6f64 7320  eans ...periods 
+00003f20: 6f66 2031 2079 6561 722e e280 9d20 5468  of 1 year.... Th
+00003f30: 6520 6075 6e69 745f 6d75 6c74 6020 636f  e `unit_mult` co
+00003f40: 6c75 6d6e 2072 6570 7265 7365 6e74 7320  lumn represents 
+00003f50: 7468 6520 6e75 6d62 6572 206f 6620 7a65  the number of ze
+00003f60: 726f 6573 2079 6f75 2073 686f 756c 6420  roes you should 
+00003f70: 6164 6420 746f 2074 6865 2076 616c 7565  add to the value
+00003f80: 2063 6f6c 756d 6e2e 2046 6f72 2069 6e73   column. For ins
+00003f90: 7461 6e63 652c 2069 6620 7661 6c75 6520  tance, if value 
+00003fa0: 6973 2069 6e20 6d69 6c6c 696f 6e73 2c20  is in millions, 
+00003fb0: 7468 656e 2074 6865 2075 6e69 7420 6d75  then the unit mu
+00003fc0: 6c74 6970 6c69 6572 2077 696c 6c20 6265  ltiplier will be
+00003fd0: 2036 2e20 4966 2069 6e20 6269 6c6c 696f   6. If in billio
+00003fe0: 6e73 2c20 7468 656e 2074 6865 2075 6e69  ns, then the uni
+00003ff0: 7420 6d75 6c74 6970 6c69 6572 2077 696c  t multiplier wil
+00004000: 6c20 6265 2039 2e0a 0a54 6865 206d 6561  l be 9...The mea
+00004010: 6e69 6e67 7320 6f66 2074 6865 206f 7468  nings of the oth
+00004020: 6572 2063 6f64 6573 2061 7265 2073 746f  er codes are sto
+00004030: 7265 6420 696e 206f 7572 2060 7061 7261  red in our `para
+00004040: 6d73 6020 6f62 6a65 6374 2061 6e64 2063  ms` object and c
+00004050: 616e 2062 6520 6665 7463 6865 6420 7769  an be fetched wi
+00004060: 7468 2061 206a 6f69 6e2e 2046 6f72 2069  th a join. For i
+00004070: 6e73 7461 6e63 6520 746f 2066 6574 6368  nstance to fetch
+00004080: 2074 6865 206d 6561 6e69 6e67 206f 6620   the meaning of 
+00004090: 7468 6520 6072 6566 5f61 7265 6160 2063  the `ref_area` c
+000040a0: 6f64 6520 e280 9c57 3030 e280 9d2c 2077  ode ...W00..., w
+000040b0: 6520 6361 6e20 7065 7266 6f72 6d20 6120  e can perform a 
+000040c0: 6c65 6674 206a 6f69 6e20 7769 7468 2074  left join with t
+000040d0: 6865 2060 7061 7261 6d73 5b27 7265 665f  he `params['ref_
+000040e0: 6172 6561 275d 6020 6461 7461 2066 7261  area']` data fra
+000040f0: 6d65 2061 6e64 2075 7365 2073 656c 6563  me and use selec
+00004100: 7420 746f 2072 6570 6c61 6365 2060 7265  t to replace `re
+00004110: 665f 6172 6561 6020 7769 7468 2074 6865  f_area` with the
+00004120: 2070 6172 616d 6574 6572 2064 6573 6372   parameter descr
+00004130: 6970 7469 6f6e 3a0a 0a0a 6060 6070 7974  iption:...```pyt
+00004140: 686f 6e0a 2320 4a6f 696e 2064 6620 7769  hon.# Join df wi
+00004150: 7468 2070 6172 616d 735b 2772 6566 5f61  th params['ref_a
+00004160: 7265 6127 5d20 746f 2066 6574 6368 2063  rea'] to fetch c
+00004170: 6f64 6520 6465 7363 7269 7074 696f 6e0a  ode description.
+00004180: 6466 203d 2064 662e 6d65 7267 6528 7061  df = df.merge(pa
+00004190: 7261 6d73 5b27 7265 665f 6172 6561 275d  rams['ref_area']
+000041a0: 2c20 6c65 6674 5f6f 6e3d 2772 6566 5f61  , left_on='ref_a
+000041b0: 7265 6127 2c72 6967 6874 5f6f 6e3d 2769  rea',right_on='i
+000041c0: 6e70 7574 5f63 6f64 6527 2c68 6f77 3d27  nput_code',how='
+000041d0: 6c65 6674 2729 0a0a 2320 4472 6f70 2072  left')..# Drop r
+000041e0: 6564 756e 6461 6e74 2063 6f6c 756d 6e73  edundant columns
+000041f0: 2061 6e64 2072 656e 616d 6520 6465 7363   and rename desc
+00004200: 7269 7074 696f 6e20 636f 6c75 6d6e 0a64  ription column.d
+00004210: 6620 3d20 6466 2e64 726f 7028 636f 6c75  f = df.drop(colu
+00004220: 6d6e 733d 5b27 7265 665f 6172 6561 272c  mns=['ref_area',
+00004230: 2769 6e70 7574 5f63 6f64 6527 5d29 2e72  'input_code']).r
+00004240: 656e 616d 6528 636f 6c75 6d6e 733d 7b22  ename(columns={"
+00004250: 6465 7363 7269 7074 696f 6e22 3a22 7265  description":"re
+00004260: 665f 6172 6561 227d 290a 0a23 2056 6965  f_area"})..# Vie
+00004270: 7720 6669 7273 7420 6665 7720 636f 6c75  w first few colu
+00004280: 6d6e 7320 696e 2074 6865 206d 6f64 6966  mns in the modif
+00004290: 6965 6420 6461 7461 2066 7261 6d65 0a64  ied data frame.d
+000042a0: 662e 6865 6164 2829 0a60 6060 0a0a 0a0a  f.head().```....
+000042b0: 0a3c 6469 763e 0a0a 3c74 6162 6c65 2062  .<div>..<table b
+000042c0: 6f72 6465 723d 2231 2220 636c 6173 733d  order="1" class=
+000042d0: 2264 6174 6166 7261 6d65 223e 0a20 203c  "dataframe">.  <
+000042e0: 7468 6561 643e 0a20 2020 203c 7472 2073  thead>.    <tr s
+000042f0: 7479 6c65 3d22 7465 7874 2d61 6c69 676e  tyle="text-align
+00004300: 3a20 7269 6768 743b 223e 0a20 2020 2020  : right;">.     
+00004310: 203c 7468 3e3c 2f74 683e 0a20 2020 2020   <th></th>.     
+00004320: 203c 7468 3e66 7265 713c 2f74 683e 0a20   <th>freq</th>. 
+00004330: 2020 2020 203c 7468 3e63 6f6d 6d6f 6469       <th>commodi
+00004340: 7479 3c2f 7468 3e0a 2020 2020 2020 3c74  ty</th>.      <t
+00004350: 683e 756e 6974 5f6d 6561 7375 7265 3c2f  h>unit_measure</
+00004360: 7468 3e0a 2020 2020 2020 3c74 683e 756e  th>.      <th>un
+00004370: 6974 5f6d 756c 743c 2f74 683e 0a20 2020  it_mult</th>.   
+00004380: 2020 203c 7468 3e74 696d 655f 666f 726d     <th>time_form
+00004390: 6174 3c2f 7468 3e0a 2020 2020 2020 3c74  at</th>.      <t
+000043a0: 683e 7469 6d65 5f70 6572 696f 643c 2f74  h>time_period</t
+000043b0: 683e 0a20 2020 2020 203c 7468 3e6f 6273  h>.      <th>obs
+000043c0: 5f76 616c 7565 3c2f 7468 3e0a 2020 2020  _value</th>.    
+000043d0: 2020 3c74 683e 7265 665f 6172 6561 3c2f    <th>ref_area</
+000043e0: 7468 3e0a 2020 2020 3c2f 7472 3e0a 2020  th>.    </tr>.  
+000043f0: 3c2f 7468 6561 643e 0a20 203c 7462 6f64  </thead>.  <tbod
+00004400: 793e 0a20 2020 203c 7472 3e0a 2020 2020  y>.    <tr>.    
+00004410: 2020 3c74 683e 303c 2f74 683e 0a20 2020    <th>0</th>.   
+00004420: 2020 203c 7464 3e41 3c2f 7464 3e0a 2020     <td>A</td>.  
+00004430: 2020 2020 3c74 643e 5043 4f41 4c3c 2f74      <td>PCOAL</t
+00004440: 643e 0a20 2020 2020 203c 7464 3e49 583c  d>.      <td>IX<
+00004450: 2f74 643e 0a20 2020 2020 203c 7464 3e30  /td>.      <td>0
+00004460: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00004470: 5031 593c 2f74 643e 0a20 2020 2020 203c  P1Y</td>.      <
+00004480: 7464 3e32 3030 303c 2f74 643e 0a20 2020  td>2000</td>.   
+00004490: 2020 203c 7464 3e33 392e 3335 3130 3233     <td>39.351023
+000044a0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000044b0: 416c 6c20 436f 756e 7472 6965 732c 2065  All Countries, e
+000044c0: 7863 6c75 6469 6e67 2074 6865 2049 4f3c  xcluding the IO<
+000044d0: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+000044e0: 2020 203c 7472 3e0a 2020 2020 2020 3c74     <tr>.      <t
+000044f0: 683e 313c 2f74 683e 0a20 2020 2020 203c  h>1</th>.      <
+00004500: 7464 3e41 3c2f 7464 3e0a 2020 2020 2020  td>A</td>.      
+00004510: 3c74 643e 5043 4f41 4c3c 2f74 643e 0a20  <td>PCOAL</td>. 
+00004520: 2020 2020 203c 7464 3e49 583c 2f74 643e       <td>IX</td>
+00004530: 0a20 2020 2020 203c 7464 3e30 3c2f 7464  .      <td>0</td
+00004540: 3e0a 2020 2020 2020 3c74 643e 5031 593c  >.      <td>P1Y<
+00004550: 2f74 643e 0a20 2020 2020 203c 7464 3e32  /td>.      <td>2
+00004560: 3030 313c 2f74 643e 0a20 2020 2020 203c  001</td>.      <
+00004570: 7464 3e34 392e 3333 3738 3539 3c2f 7464  td>49.337859</td
+00004580: 3e0a 2020 2020 2020 3c74 643e 416c 6c20  >.      <td>All 
+00004590: 436f 756e 7472 6965 732c 2065 7863 6c75  Countries, exclu
+000045a0: 6469 6e67 2074 6865 2049 4f3c 2f74 643e  ding the IO</td>
+000045b0: 0a20 2020 203c 2f74 723e 0a20 2020 203c  .    </tr>.    <
+000045c0: 7472 3e0a 2020 2020 2020 3c74 683e 323c  tr>.      <th>2<
+000045d0: 2f74 683e 0a20 2020 2020 203c 7464 3e41  /th>.      <td>A
+000045e0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000045f0: 5043 4f41 4c3c 2f74 643e 0a20 2020 2020  PCOAL</td>.     
+00004600: 203c 7464 3e49 583c 2f74 643e 0a20 2020   <td>IX</td>.   
+00004610: 2020 203c 7464 3e30 3c2f 7464 3e0a 2020     <td>0</td>.  
+00004620: 2020 2020 3c74 643e 5031 593c 2f74 643e      <td>P1Y</td>
+00004630: 0a20 2020 2020 203c 7464 3e32 3030 323c  .      <td>2002<
+00004640: 2f74 643e 0a20 2020 2020 203c 7464 3e33  /td>.      <td>3
+00004650: 392e 3439 3439 3039 3c2f 7464 3e0a 2020  9.494909</td>.  
+00004660: 2020 2020 3c74 643e 416c 6c20 436f 756e      <td>All Coun
+00004670: 7472 6965 732c 2065 7863 6c75 6469 6e67  tries, excluding
+00004680: 2074 6865 2049 4f3c 2f74 643e 0a20 2020   the IO</td>.   
+00004690: 203c 2f74 723e 0a20 2020 203c 7472 3e0a   </tr>.    <tr>.
+000046a0: 2020 2020 2020 3c74 683e 333c 2f74 683e        <th>3</th>
+000046b0: 0a20 2020 2020 203c 7464 3e41 3c2f 7464  .      <td>A</td
+000046c0: 3e0a 2020 2020 2020 3c74 643e 5043 4f41  >.      <td>PCOA
+000046d0: 4c3c 2f74 643e 0a20 2020 2020 203c 7464  L</td>.      <td
+000046e0: 3e49 583c 2f74 643e 0a20 2020 2020 203c  >IX</td>.      <
+000046f0: 7464 3e30 3c2f 7464 3e0a 2020 2020 2020  td>0</td>.      
+00004700: 3c74 643e 5031 593c 2f74 643e 0a20 2020  <td>P1Y</td>.   
+00004710: 2020 203c 7464 3e32 3030 333c 2f74 643e     <td>2003</td>
+00004720: 0a20 2020 2020 203c 7464 3e34 332e 3238  .      <td>43.28
+00004730: 3738 3838 3c2f 7464 3e0a 2020 2020 2020  7888</td>.      
+00004740: 3c74 643e 416c 6c20 436f 756e 7472 6965  <td>All Countrie
+00004750: 732c 2065 7863 6c75 6469 6e67 2074 6865  s, excluding the
+00004760: 2049 4f3c 2f74 643e 0a20 2020 203c 2f74   IO</td>.    </t
+00004770: 723e 0a20 2020 203c 7472 3e0a 2020 2020  r>.    <tr>.    
+00004780: 2020 3c74 683e 343c 2f74 683e 0a20 2020    <th>4</th>.   
+00004790: 2020 203c 7464 3e41 3c2f 7464 3e0a 2020     <td>A</td>.  
+000047a0: 2020 2020 3c74 643e 5043 4f41 4c3c 2f74      <td>PCOAL</t
+000047b0: 643e 0a20 2020 2020 203c 7464 3e49 583c  d>.      <td>IX<
+000047c0: 2f74 643e 0a20 2020 2020 203c 7464 3e30  /td>.      <td>0
+000047d0: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+000047e0: 5031 593c 2f74 643e 0a20 2020 2020 203c  P1Y</td>.      <
+000047f0: 7464 3e32 3030 343c 2f74 643e 0a20 2020  td>2004</td>.   
+00004800: 2020 203c 7464 3e38 322e 3931 3835 3836     <td>82.918586
+00004810: 3c2f 7464 3e0a 2020 2020 2020 3c74 643e  </td>.      <td>
+00004820: 416c 6c20 436f 756e 7472 6965 732c 2065  All Countries, e
+00004830: 7863 6c75 6469 6e67 2074 6865 2049 4f3c  xcluding the IO<
+00004840: 2f74 643e 0a20 2020 203c 2f74 723e 0a20  /td>.    </tr>. 
+00004850: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+00004860: 653e 0a3c 2f64 6976 3e0a 0a0a 0a23 2320  e>.</div>....## 
+00004870: 5261 7465 2061 6e64 2042 616e 6477 6964  Rate and Bandwid
+00004880: 7468 204c 696d 6974 204d 616e 6167 656d  th Limit Managem
+00004890: 656e 740a 0a23 2323 2053 6574 7469 6e67  ent..### Setting
+000048a0: 2061 2055 6e69 7175 6520 4170 706c 6963   a Unique Applic
+000048b0: 6174 696f 6e20 4e61 6d65 2077 6974 6820  ation Name with 
+000048c0: 6073 6574 5f69 6d66 5f61 7070 5f6e 616d  `set_imf_app_nam
+000048d0: 6560 0a0a 6069 6d66 702e 7365 745f 696d  e`..`imfp.set_im
+000048e0: 665f 6170 705f 6e61 6d65 2829 6020 616c  f_app_name()` al
+000048f0: 6c6f 7773 2075 7365 7273 2074 6f20 7365  lows users to se
+00004900: 7420 6120 6375 7374 6f6d 2061 7070 6c69  t a custom appli
+00004910: 6361 7469 6f6e 206e 616d 6520 746f 2062  cation name to b
+00004920: 6520 7573 6564 2077 6865 6e20 6d61 6b69  e used when maki
+00004930: 6e67 2041 5049 2063 616c 6c73 2074 6f20  ng API calls to 
+00004940: 7468 6520 494d 4620 4150 492e 2054 6865  the IMF API. The
+00004950: 2049 4d46 2041 5049 2068 6173 2061 6e20   IMF API has an 
+00004960: 6170 706c 6963 6174 696f 6e2d 6261 7365  application-base
+00004970: 6420 7261 7465 206c 696d 6974 206f 6620  d rate limit of 
+00004980: 3530 2072 6571 7565 7374 7320 7065 7220  50 requests per 
+00004990: 7365 636f 6e64 2c20 7769 7468 2074 6865  second, with the
+000049a0: 2061 7070 6c69 6361 7469 6f6e 2069 6465   application ide
+000049b0: 6e74 6966 6965 6420 6279 2074 6865 2022  ntified by the "
+000049c0: 7573 6572 5f61 6765 6e74 2220 7661 7269  user_agent" vari
+000049d0: 6162 6c65 2069 6e20 7468 6520 7265 7175  able in the requ
+000049e0: 6573 7420 6865 6164 6572 2e0a 0a54 6869  est header...Thi
+000049f0: 7320 636f 756c 6420 7072 6f76 6520 7072  s could prove pr
+00004a00: 6f62 6c65 6d61 7469 6320 6966 2074 6865  oblematic if the
+00004a10: 2060 696d 6670 6020 6c69 6272 6172 7920   `imfp` library 
+00004a20: 6265 6361 6d65 2074 6f6f 2070 6f70 756c  became too popul
+00004a30: 6172 2061 6e64 2074 6f6f 206d 616e 7920  ar and too many 
+00004a40: 7573 6572 7320 7472 6965 6420 746f 206d  users tried to m
+00004a50: 616b 6520 7369 6d75 6c74 616e 656f 7573  ake simultaneous
+00004a60: 2041 5049 2072 6571 7565 7374 7320 7573   API requests us
+00004a70: 696e 6720 7468 6520 6465 6661 756c 7420  ing the default 
+00004a80: 6170 7020 6e61 6d65 2e20 4279 2073 6574  app name. By set
+00004a90: 7469 6e67 2061 2063 7573 746f 6d20 6170  ting a custom ap
+00004aa0: 706c 6963 6174 696f 6e20 6e61 6d65 2c20  plication name, 
+00004ab0: 7573 6572 7320 6361 6e20 6176 6f69 6420  users can avoid 
+00004ac0: 6869 7474 696e 6720 7261 7465 206c 696d  hitting rate lim
+00004ad0: 6974 7320 616e 6420 6265 696e 6720 626c  its and being bl
+00004ae0: 6f63 6b65 6420 6279 2074 6865 2041 5049  ocked by the API
+00004af0: 2e20 6069 6d66 702e 7365 745f 696d 665f  . `imfp.set_imf_
+00004b00: 6170 705f 6e61 6d65 2829 6020 7365 7473  app_name()` sets
+00004b10: 2074 6865 2061 7070 6c69 6361 7469 6f6e   the application
+00004b20: 206e 616d 6520 6279 2063 6861 6e67 696e   name by changin
+00004b30: 6720 7468 6520 6049 4d46 5f41 5050 5f4e  g the `IMF_APP_N
+00004b40: 414d 4560 2076 6172 6961 626c 6520 696e  AME` variable in
+00004b50: 2074 6865 2065 6e76 6972 6f6e 6d65 6e74   the environment
+00004b60: 2e20 4966 2074 6869 7320 7661 7269 6162  . If this variab
+00004b70: 6c65 2064 6f65 736e 2774 2065 7869 7374  le doesn't exist
+00004b80: 2c20 6069 6d66 702e 7365 745f 696d 665f  , `imfp.set_imf_
+00004b90: 6170 705f 6e61 6d65 2829 6020 7769 6c6c  app_name()` will
+00004ba0: 2063 7265 6174 6520 6974 2e0a 0a54 6f20   create it...To 
+00004bb0: 7365 7420 6120 6375 7374 6f6d 2061 7070  set a custom app
+00004bc0: 6c69 6361 7469 6f6e 206e 616d 652c 2073  lication name, s
+00004bd0: 696d 706c 7920 6361 6c6c 2074 6865 2060  imply call the `
+00004be0: 696d 6670 2e73 6574 5f69 6d66 5f61 7070  imfp.set_imf_app
+00004bf0: 5f6e 616d 6528 2960 2066 756e 6374 696f  _name()` functio
+00004c00: 6e20 7769 7468 2079 6f75 7220 6465 7369  n with your desi
+00004c10: 7265 6420 6170 706c 6963 6174 696f 6e20  red application 
+00004c20: 6e61 6d65 2061 7320 616e 2061 7267 756d  name as an argum
+00004c30: 656e 743a 0a0a 0a60 6060 7079 7468 6f6e  ent:...```python
+00004c40: 0a23 2053 6574 2063 7573 746f 6d20 6170  .# Set custom ap
+00004c50: 7020 6e61 6d65 2061 7320 616e 2065 6e76  p name as an env
+00004c60: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
+00004c70: 650a 696d 6670 2e73 6574 5f69 6d66 5f61  e.imfp.set_imf_a
+00004c80: 7070 5f6e 616d 6528 226d 795f 6375 7374  pp_name("my_cust
+00004c90: 6f6d 5f61 7070 5f6e 616d 6522 290a 6060  om_app_name").``
+00004ca0: 600a 0a0a 0a54 6865 2066 756e 6374 696f  `....The functio
+00004cb0: 6e20 7769 6c6c 2074 6872 6f77 2061 6e20  n will throw an 
+00004cc0: 6572 726f 7220 6966 2074 6865 2070 726f  error if the pro
+00004cd0: 7669 6465 6420 6e61 6d65 2069 7320 6d69  vided name is mi
+00004ce0: 7373 696e 672c 204e 554c 4c2c 204e 412c  ssing, NULL, NA,
+00004cf0: 206e 6f74 2061 2073 7472 696e 672c 206f   not a string, o
+00004d00: 7220 6c6f 6e67 6572 2074 6861 6e20 3235  r longer than 25
+00004d10: 3520 6368 6172 6163 7465 7273 2e20 4966  5 characters. If
+00004d20: 2074 6865 2070 726f 7669 6465 6420 6e61   the provided na
+00004d30: 6d65 2069 7320 2269 6d66 7222 2028 7468  me is "imfr" (th
+00004d40: 6520 6465 6661 756c 7429 206f 7220 616e  e default) or an
+00004d50: 2065 6d70 7479 2073 7472 696e 672c 2074   empty string, t
+00004d60: 6865 2066 756e 6374 696f 6e20 7769 6c6c  he function will
+00004d70: 2069 7373 7565 2061 2077 6172 6e69 6e67   issue a warning
+00004d80: 2072 6563 6f6d 6d65 6e64 696e 6720 7468   recommending th
+00004d90: 6520 7573 6520 6f66 2061 2075 6e69 7175  e use of a uniqu
+00004da0: 6520 6170 7020 6e61 6d65 2074 6f20 6176  e app name to av
+00004db0: 6f69 6420 6869 7474 696e 6720 7261 7465  oid hitting rate
+00004dc0: 206c 696d 6974 732e 0a0a 2323 2320 4368   limits...### Ch
+00004dd0: 616e 6769 6e67 2074 6865 2065 6e66 6f72  anging the enfor
+00004de0: 6365 6420 7761 6974 2074 696d 6520 6265  ced wait time be
+00004df0: 7477 6565 6e20 4150 4920 6361 6c6c 7320  tween API calls 
+00004e00: 7769 7468 2060 7365 745f 696d 665f 7761  with `set_imf_wa
+00004e10: 6974 5f74 696d 6560 0a0a 4279 2064 6566  it_time`..By def
+00004e20: 6175 6c74 2c20 6069 6d66 7060 2065 6e66  ault, `imfp` enf
+00004e30: 6f72 6365 7320 6120 6d61 6e64 6174 6f72  orces a mandator
+00004e40: 7920 312e 352d 7365 636f 6e64 2077 6169  y 1.5-second wai
+00004e50: 7420 7469 6d65 2062 6574 7765 656e 2041  t time between A
+00004e60: 5049 2063 616c 6c73 2074 6f20 7072 6576  PI calls to prev
+00004e70: 656e 7420 7265 7065 6174 6564 206f 7220  ent repeated or 
+00004e80: 7265 6375 7273 6976 6520 6361 6c6c 7320  recursive calls 
+00004e90: 6672 6f6d 2065 7863 6565 6469 6e67 2074  from exceeding t
+00004ea0: 6865 2041 5049 2773 2062 616e 6477 6964  he API's bandwid
+00004eb0: 7468 2f72 6174 6520 6c69 6d69 742e 2054  th/rate limit. T
+00004ec0: 6869 7320 7761 6974 2074 696d 6520 7368  his wait time sh
+00004ed0: 6f75 6c64 2062 6520 7375 6666 6963 6965  ould be sufficie
+00004ee0: 6e74 2066 6f72 206d 6f73 7420 6170 706c  nt for most appl
+00004ef0: 6963 6174 696f 6e73 2e20 486f 7765 7665  ications. Howeve
+00004f00: 722c 2069 6620 796f 7520 6172 6520 7275  r, if you are ru
+00004f10: 6e6e 696e 6720 7061 7261 6c6c 656c 2070  nning parallel p
+00004f20: 726f 6365 7373 6573 2075 7369 6e67 2060  rocesses using `
+00004f30: 696d 6670 6020 2865 2e67 2e20 6475 7269  imfp` (e.g. duri
+00004f40: 6e67 2063 726f 7373 2d70 6c61 7466 6f72  ng cross-platfor
+00004f50: 6d20 7465 7374 696e 6729 2c20 7468 6973  m testing), this
+00004f60: 2077 6169 7420 7469 6d65 206d 6179 2062   wait time may b
+00004f70: 6520 696e 7375 6666 6963 6965 6e74 2074  e insufficient t
+00004f80: 6f20 7072 6576 656e 7420 796f 7520 6672  o prevent you fr
+00004f90: 6f6d 2072 756e 6e69 6e67 2075 7020 6167  om running up ag
+00004fa0: 6169 6e73 7420 7468 6520 4150 4927 7320  ainst the API's 
+00004fb0: 7261 7465 2061 6e64 2062 616e 6477 6964  rate and bandwid
+00004fc0: 7468 206c 696d 6974 732e 2059 6f75 2063  th limits. You c
+00004fd0: 616e 2063 6861 6e67 6520 7468 6973 2077  an change this w
+00004fe0: 6169 7420 7469 6d65 2062 7920 6361 6c6c  ait time by call
+00004ff0: 696e 6720 7468 6520 6073 6574 5f69 6d66  ing the `set_imf
+00005000: 5f77 6169 745f 7469 6d65 6020 6675 6e63  _wait_time` func
+00005010: 7469 6f6e 2077 6974 6820 6120 6e75 6d65  tion with a nume
+00005020: 7269 6320 7661 6c75 652c 2069 6e20 7365  ric value, in se
+00005030: 636f 6e64 732e 2046 6f72 2069 6e73 7461  conds. For insta
+00005040: 6e63 652c 2074 6f20 656e 666f 7263 6520  nce, to enforce 
+00005050: 6120 6669 7665 2d73 6563 6f6e 6420 7761  a five-second wa
+00005060: 6974 2074 696d 6520 6265 7477 6565 6e20  it time between 
+00005070: 4150 4920 6361 6c6c 732c 2075 7365 2060  API calls, use `
+00005080: 7365 745f 696d 665f 7761 6974 5f74 696d  set_imf_wait_tim
+00005090: 6528 3130 2960 2e0a 0a41 6c73 6f20 6e6f  e(10)`...Also no
+000050a0: 7465 2074 6861 7420 6279 2064 6566 6175  te that by defau
+000050b0: 6c74 2c20 6069 6d66 7060 2066 756e 6374  lt, `imfp` funct
+000050c0: 696f 6e73 2077 696c 6c20 7265 7472 7920  ions will retry 
+000050d0: 616e 7920 4150 4920 6361 6c6c 2072 656a  any API call rej
+000050e0: 6563 7465 6420 666f 7220 6261 6e64 7769  ected for bandwi
+000050f0: 6474 6820 6f72 2072 6174 6520 6c69 6d69  dth or rate limi
+00005100: 7420 7265 6173 6f6e 732e 2054 6865 206e  t reasons. The n
+00005110: 756d 6265 7220 6f66 2074 696d 6573 2060  umber of times `
+00005120: 696d 6670 6020 7769 6c6c 2061 7474 656d  imfp` will attem
+00005130: 7074 2074 6865 2063 616c 6c20 6973 2073  pt the call is s
+00005140: 6574 2062 7920 7468 6520 6074 696d 6573  et by the `times
+00005150: 6020 6172 6775 6d65 6e74 2c20 7769 7468  ` argument, with
+00005160: 2061 2064 6566 6175 6c74 2076 616c 7565   a default value
+00005170: 206f 6620 332e 2028 5769 7468 2074 6869   of 3. (With thi
+00005180: 7320 7661 6c75 652c 2072 6571 7565 7374  s value, request
+00005190: 7320 7769 6c6c 2062 6520 7265 7472 6965  s will be retrie
+000051a0: 6420 7477 6963 6520 6166 7465 7220 616e  d twice after an
+000051b0: 2069 6e69 7469 616c 2066 6169 6c75 7265   initial failure
+000051c0: 2e29 204e 6f74 6520 7468 6174 2060 696d  .) Note that `im
+000051d0: 6670 6020 656e 666f 7263 6573 2061 6e20  fp` enforces an 
+000051e0: 6578 706f 6e65 6e74 6961 6c6c 7920 696e  exponentially in
+000051f0: 6372 6561 7369 6e67 2077 6169 7420 7469  creasing wait ti
+00005200: 6d65 2062 6574 7765 656e 2066 756e 6374  me between funct
+00005210: 696f 6e20 6361 6c6c 732c 2077 6974 6820  ion calls, with 
+00005220: 6120 6261 7365 2077 6169 7420 7469 6d65  a base wait time
+00005230: 206f 6620 3520 7365 636f 6e64 7320 6f6e   of 5 seconds on
+00005240: 2074 6865 2066 6972 7374 2072 6574 7279   the first retry
+00005250: 2c20 736f 2069 7420 6973 206e 6f74 2072  , so it is not r
+00005260: 6563 6f6d 6d65 6e64 6564 2074 6f20 7365  ecommended to se
+00005270: 7420 6120 6869 6768 2076 616c 7565 2066  t a high value f
+00005280: 6f72 2060 7469 6d65 7360 2e0a 0a23 2320  or `times`...## 
+00005290: 436f 6e74 7269 6275 7469 6e67 0a0a 4920  Contributing..I 
+000052a0: 776f 756c 6420 6c6f 7665 2074 6f20 6861  would love to ha
+000052b0: 7665 2079 6f75 7220 6865 6c70 2069 6e20  ve your help in 
+000052c0: 696d 7072 6f76 696e 6720 6069 6d66 7260  improving `imfr`
+000052d0: 2e20 4966 2079 6f75 2065 6e63 6f75 6e74  . If you encount
+000052e0: 6572 2061 2062 7567 2077 6869 6c65 2075  er a bug while u
+000052f0: 7369 6e67 2074 6865 206c 6962 7261 7279  sing the library
+00005300: 2c20 706c 6561 7365 206f 7065 6e20 616e  , please open an
+00005310: 2069 7373 7565 2e20 416c 7465 726e 6174   issue. Alternat
+00005320: 6976 656c 792c 2066 6978 2074 6865 2062  ively, fix the b
+00005330: 7567 2061 6e64 206f 7065 6e20 6120 7075  ug and open a pu
+00005340: 6c6c 2072 6571 7565 7374 2e20 5468 616e  ll request. Than
+00005350: 6b73 2069 6e20 6164 7661 6e63 6520 666f  ks in advance fo
+00005360: 7220 796f 7572 2068 656c 7021 0a0a       r your help!..
```

