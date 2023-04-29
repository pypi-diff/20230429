# Comparing `tmp/msgraphlib-0.1.1.tar.gz` & `tmp/msgraphlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgraphlib-0.1.1.tar", last modified: Wed Apr 26 08:30:59 2023, max compression
+gzip compressed data, was "msgraphlib-0.1.2.tar", last modified: Sat Apr 29 17:22:07 2023, max compression
```

## Comparing `msgraphlib-0.1.1.tar` & `msgraphlib-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 08:30:59.512354 msgraphlib-0.1.1/
--rw-rw-rw-   0        0        0     1073 2023-03-09 21:23:05.000000 msgraphlib-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      543 2023-04-26 08:30:59.511357 msgraphlib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2023-03-08 17:22:08.000000 msgraphlib-0.1.1/README.md
--rw-rw-rw-   0        0        0     1797 2023-04-24 22:23:15.000000 msgraphlib-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 08:30:59.513351 msgraphlib-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-26 08:30:59.184207 msgraphlib-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-26 08:30:59.446530 msgraphlib-0.1.1/src/msgraphlib/
--rw-rw-rw-   0        0        0      313 2023-04-11 08:07:09.000000 msgraphlib-0.1.1/src/msgraphlib/__init__.py
--rw-rw-rw-   0        0        0      209 2023-04-07 07:17:39.000000 msgraphlib-0.1.1/src/msgraphlib/common.py
--rw-rw-rw-   0        0        0    19509 2023-04-26 07:27:22.000000 msgraphlib-0.1.1/src/msgraphlib/core.py
--rw-rw-rw-   0        0        0    17541 2023-04-25 14:28:01.000000 msgraphlib-0.1.1/src/msgraphlib/drive.py
--rw-rw-rw-   0        0        0    18196 2023-04-11 09:38:58.000000 msgraphlib-0.1.1/src/msgraphlib/excel.py
--rw-rw-rw-   0        0        0     3912 2023-04-04 15:00:56.000000 msgraphlib-0.1.1/src/msgraphlib/files_old.py
--rw-rw-rw-   0        0        0      327 2023-03-12 14:16:28.000000 msgraphlib-0.1.1/src/msgraphlib/metadata.py
--rw-rw-rw-   0        0        0     1851 2023-04-24 22:34:59.000000 msgraphlib-0.1.1/src/msgraphlib/sharepoint.py
--rw-rw-rw-   0        0        0      256 2023-03-29 15:39:27.000000 msgraphlib-0.1.1/src/msgraphlib/testmodule.py
-drwxrwxrwx   0        0        0        0 2023-04-26 08:30:59.506371 msgraphlib-0.1.1/src/msgraphlib.egg-info/
--rw-rw-rw-   0        0        0      543 2023-04-26 08:30:59.000000 msgraphlib-0.1.1/src/msgraphlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      457 2023-04-26 08:30:59.000000 msgraphlib-0.1.1/src/msgraphlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 08:30:59.000000 msgraphlib-0.1.1/src/msgraphlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-26 08:30:59.000000 msgraphlib-0.1.1/src/msgraphlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 08:30:59.000000 msgraphlib-0.1.1/src/msgraphlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 17:22:07.193149 msgraphlib-0.1.2/
+-rw-rw-rw-   0        0        0     1073 2023-03-09 21:23:05.000000 msgraphlib-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      543 2023-04-29 17:22:07.192183 msgraphlib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2023-03-08 17:22:08.000000 msgraphlib-0.1.2/README.md
+-rw-rw-rw-   0        0        0     1797 2023-04-29 17:21:21.000000 msgraphlib-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 17:22:07.194181 msgraphlib-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 17:22:06.886274 msgraphlib-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 17:22:07.109372 msgraphlib-0.1.2/src/msgraphlib/
+-rw-rw-rw-   0        0        0      313 2023-04-11 08:07:09.000000 msgraphlib-0.1.2/src/msgraphlib/__init__.py
+-rw-rw-rw-   0        0        0      209 2023-04-07 07:17:39.000000 msgraphlib-0.1.2/src/msgraphlib/common.py
+-rw-rw-rw-   0        0        0    19961 2023-04-29 17:20:30.000000 msgraphlib-0.1.2/src/msgraphlib/core.py
+-rw-rw-rw-   0        0        0    17541 2023-04-25 14:28:01.000000 msgraphlib-0.1.2/src/msgraphlib/drive.py
+-rw-rw-rw-   0        0        0    18196 2023-04-11 09:38:58.000000 msgraphlib-0.1.2/src/msgraphlib/excel.py
+-rw-rw-rw-   0        0        0     3912 2023-04-04 15:00:56.000000 msgraphlib-0.1.2/src/msgraphlib/files_old.py
+-rw-rw-rw-   0        0        0      327 2023-03-12 14:16:28.000000 msgraphlib-0.1.2/src/msgraphlib/metadata.py
+-rw-rw-rw-   0        0        0     1851 2023-04-24 22:34:59.000000 msgraphlib-0.1.2/src/msgraphlib/sharepoint.py
+-rw-rw-rw-   0        0        0      256 2023-03-29 15:39:27.000000 msgraphlib-0.1.2/src/msgraphlib/testmodule.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:22:07.186601 msgraphlib-0.1.2/src/msgraphlib.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-04-29 17:22:06.000000 msgraphlib-0.1.2/src/msgraphlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2023-04-29 17:22:06.000000 msgraphlib-0.1.2/src/msgraphlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:22:06.000000 msgraphlib-0.1.2/src/msgraphlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-04-29 17:22:06.000000 msgraphlib-0.1.2/src/msgraphlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-29 17:22:06.000000 msgraphlib-0.1.2/src/msgraphlib.egg-info/top_level.txt
```

### Comparing `msgraphlib-0.1.1/LICENSE` & `msgraphlib-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msgraphlib-0.1.1/PKG-INFO` & `msgraphlib-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Microsoft Graph API Explorer
 Author-email: Pawel Musial <pawel.r.musial@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `msgraphlib-0.1.1/pyproject.toml` & `msgraphlib-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgraphlib"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Pawel Musial", email="pawel.r.musial@gmail.com" },
 ]
 description = "Microsoft Graph API Explorer"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `msgraphlib-0.1.1/src/msgraphlib/core.py` & `msgraphlib-0.1.2/src/msgraphlib/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,18 +88,28 @@
     _stock = {}
     
 class _CredsPool:
     _stock = {}
 
     @classmethod
     def get_creds(cls, arn):
-        return cls._stock.get(arn, cls.__get_aws_creds(arn))
+        creds = cls._stock.get(arn)
+        if not creds:
+            aws_creds = cls._get_aws_creds(arn)
+            if aws_creds:
+                user_key = ('id', 'user', 'username', 'secret_id', 'name')
+                pswd_key = ('pswd', 'password', 'secret', 'secret_value', 'value')
+                username = [v for (k,v) in aws_creds.items() if k.lower() in user_key]
+                password = [v for (k,v) in aws_creds.items() if k.lower() in pswd_key]
+                if username and password:
+                    cls._stock[arn] = {'username': username[-1], 'password': password[-1]}
+        return cls._stock.get(arn)
     
     @staticmethod
-    def __get_aws_creds(creds_arn):
+    def _get_aws_creds(creds_arn):
         # Requires layer 'AWS Parameters and Secrets Lambda Extension'
         # https://docs.aws.amazon.com/secretsmanager/latest/apireference/API_Operations.html
         # The secret name can contain ASCII letters, numbers, and the following characters: /_+=.@-
         # Secret's ARN includes the name of the secret followed by six random characters
         port = os.getenv('PARAMETERS_SECRETS_EXTENSION_HTTP_PORT', 2773) #AWS default: 2773
         secrets_url = (f"http://localhost:{port}/secretsmanager/get?secretId={creds_arn}")
         headers = { "X-Aws-Parameters-Secrets-Token": os.environ.get('AWS_SESSION_TOKEN') }
@@ -283,30 +293,30 @@
                         time.sleep(pause); continue
                     elif response.status_code == 409 and error['code'] == 'resourceModified':
                         time.sleep(5); continue
 
                 # Otherwise re-throw with HTTP data from the response
                 err_msg = {'status': response.status_code, 'reason': response.reason}
                 err_msg |= {'error': error, 'text': response.text} 
-                # AccessDenied - Could not obtain a WAC access token
-                if response.status_code == 403 and 'WAC access token' in response.text:
-                    raise 
-                # Not found
-                if response.status_code == 404 and error['code'] == 'itemNotFound': 
-                    raise ResourceNotFoundError(err_msg)
-                # Locked resource errors
-                if response.status_code == 423 and error['code'] == 'resourceCheckedOut': 
-                    raise ResourceCheckedOutError(err_msg)
-                elif response.status_code == 423:
-                    raise ResourceLockedError(err_msg)
-                elif response.status_code == 409 and error['code'] == 'nameAlreadyExists':
-                    raise NameAlreadyExistsError(err_msg)
-                elif response.status_code == 409 and error['code'] == 'resourceModified':
-                    raise ResourceModifiedError(err_msg)                    
-                else: raise requests.exceptions.HTTPError(err_msg)
+
+                match response.status_code:
+                    case 403 if 'WAC access token' in response.text:
+                         raise # AccessDenied - Could not obtain a WAC access token
+                    case 404 if error['code'] == 'itemNotFound':
+                         raise ResourceNotFoundError(err_msg)
+                    case 423 if error['code'] == 'resourceCheckedOut': 
+                        raise ResourceCheckedOutError(err_msg)
+                    case 423:
+                        raise ResourceLockedError(err_msg)
+                    case 409 if error['code'] == 'nameAlreadyExists':
+                        raise NameAlreadyExistsError(err_msg)
+                    case 409 if error['code'] == 'resourceModified':
+                        raise ResourceModifiedError(err_msg)                    
+                    case _: raise requests.exceptions.HTTPError(err_msg)
+
             except requests.exceptions.ConnectionError as err_c:
                 if attempt < self.config.retry['count']: time.sleep(self.config.retry['pause'])
                 else: raise (err_c)
             except requests.exceptions.Timeout as err_t:
                 raise (err_t)
             except requests.exceptions.RequestException as err_r:
                 raise (err_r)
```

### Comparing `msgraphlib-0.1.1/src/msgraphlib/drive.py` & `msgraphlib-0.1.2/src/msgraphlib/drive.py`

 * *Files identical despite different names*

### Comparing `msgraphlib-0.1.1/src/msgraphlib/excel.py` & `msgraphlib-0.1.2/src/msgraphlib/excel.py`

 * *Files identical despite different names*

### Comparing `msgraphlib-0.1.1/src/msgraphlib/files_old.py` & `msgraphlib-0.1.2/src/msgraphlib/files_old.py`

 * *Files identical despite different names*

### Comparing `msgraphlib-0.1.1/src/msgraphlib/sharepoint.py` & `msgraphlib-0.1.2/src/msgraphlib/sharepoint.py`

 * *Files identical despite different names*

### Comparing `msgraphlib-0.1.1/src/msgraphlib.egg-info/PKG-INFO` & `msgraphlib-0.1.2/src/msgraphlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Microsoft Graph API Explorer
 Author-email: Pawel Musial <pawel.r.musial@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

