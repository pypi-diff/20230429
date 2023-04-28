# Comparing `tmp/python3-capsolver-0.6.tar.gz` & `tmp/python3-capsolver-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-capsolver-0.6.tar", last modified: Fri Apr 28 23:26:53 2023, max compression
+gzip compressed data, was "python3-capsolver-0.6.1.tar", last modified: Fri Apr 28 23:51:26 2023, max compression
```

## Comparing `python3-capsolver-0.6.tar` & `python3-capsolver-0.6.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/
--rw-r--r--   0 homea     (1000) homea     (1000)     4699 2023-04-28 23:26:53.840542 python3-capsolver-0.6/PKG-INFO
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/python3_capsolver/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.6/python3_capsolver/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)       20 2023-04-28 23:26:49.000000 python3-capsolver-0.6/python3_capsolver/__version__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4919 2023-04-28 23:01:33.000000 python3-capsolver-0.6/python3_capsolver/cloudflare.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1959 2023-04-28 23:25:46.000000 python3-capsolver-0.6/python3_capsolver/control.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/python3_capsolver/core/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.6/python3_capsolver/core/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3-capsolver-0.6/python3_capsolver/core/base.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.6/python3_capsolver/core/config.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3398 2023-04-28 23:03:36.000000 python3-capsolver-0.6/python3_capsolver/core/enum.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4381 2023-04-28 23:23:41.000000 python3-capsolver-0.6/python3_capsolver/core/serializer.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3924 2023-04-28 23:01:33.000000 python3-capsolver-0.6/python3_capsolver/datadome_slider.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7880 2023-04-28 18:30:07.000000 python3-capsolver-0.6/python3_capsolver/fun_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4323 2023-04-28 18:30:07.000000 python3-capsolver-0.6/python3_capsolver/gee_test.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4831 2023-04-28 18:20:01.000000 python3-capsolver-0.6/python3_capsolver/hcaptcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6350 2023-04-28 18:41:20.000000 python3-capsolver-0.6/python3_capsolver/image_to_text.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7509 2023-04-28 18:41:20.000000 python3-capsolver-0.6/python3_capsolver/kasada.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4972 2023-04-28 22:33:29.000000 python3-capsolver-0.6/python3_capsolver/mt_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6394 2023-04-28 22:02:43.000000 python3-capsolver-0.6/python3_capsolver/recaptcha.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/python3_capsolver.egg-info/
--rw-r--r--   0 homea     (1000) homea     (1000)     4699 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/PKG-INFO
--rw-r--r--   0 homea     (1000) homea     (1000)      799 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/SOURCES.txt
--rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/dependency_links.txt
--rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/not-zip-safe
--rw-r--r--   0 homea     (1000) homea     (1000)       60 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/requires.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       18 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/top_level.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 23:26:53.840542 python3-capsolver-0.6/setup.cfg
--rw-r--r--   0 homea     (1000) homea     (1000)     4053 2023-04-28 17:36:49.000000 python3-capsolver-0.6/setup.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/
+-rw-r--r--   0 homea     (1000) homea     (1000)     5065 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/PKG-INFO
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/python3_capsolver/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.6.1/python3_capsolver/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-04-28 23:51:22.000000 python3-capsolver-0.6.1/python3_capsolver/__version__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4919 2023-04-28 23:01:33.000000 python3-capsolver-0.6.1/python3_capsolver/cloudflare.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1958 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/control.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/python3_capsolver/core/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.6.1/python3_capsolver/core/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3-capsolver-0.6.1/python3_capsolver/core/base.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.6.1/python3_capsolver/core/config.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3398 2023-04-28 23:03:36.000000 python3-capsolver-0.6.1/python3_capsolver/core/enum.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4381 2023-04-28 23:23:41.000000 python3-capsolver-0.6.1/python3_capsolver/core/serializer.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3923 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/datadome_slider.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7880 2023-04-28 18:30:07.000000 python3-capsolver-0.6.1/python3_capsolver/fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4322 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/gee_test.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4830 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6349 2023-04-28 23:31:25.000000 python3-capsolver-0.6.1/python3_capsolver/image_to_text.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4972 2023-04-28 22:33:29.000000 python3-capsolver-0.6.1/python3_capsolver/mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6394 2023-04-28 22:02:43.000000 python3-capsolver-0.6.1/python3_capsolver/recaptcha.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/python3_capsolver.egg-info/
+-rw-rw-r--   0 homea     (1000) homea     (1000)     5065 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/PKG-INFO
+-rw-rw-r--   0 homea     (1000) homea     (1000)      771 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:33:01.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/not-zip-safe
+-rw-rw-r--   0 homea     (1000) homea     (1000)       60 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/requires.txt
+-rw-rw-r--   0 homea     (1000) homea     (1000)       18 2023-04-28 23:51:26.000000 python3-capsolver-0.6.1/python3_capsolver.egg-info/top_level.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 23:51:26.597251 python3-capsolver-0.6.1/setup.cfg
+-rw-r--r--   0 homea     (1000) homea     (1000)     4137 2023-04-28 23:50:54.000000 python3-capsolver-0.6.1/setup.py
```

### Comparing `python3-capsolver-0.6/PKG-INFO` & `python3-capsolver-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.6
+Version: 0.6.1
 Summary: Python 3.7+ Capsolver library with AIO module.
 Home-page: https://andreidrang.github.io/python3-capsolver/
 Author: AndreiDrang
 Author-email: python-captcha@pm.me
 License: MIT
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Source, https://github.com/AndreiDrang/python3-captchaai
 Keywords: captcha 
                 recaptcha
                 geetest
                 hcaptcha
                 capypuzzle
-                tiktok
                 rotatecaptcha
                 funcaptcha
                 keycaptcha
                 python3
                 python-library
                 capsolver
-                kasada
                 datadomeslider
+                datadome
                 mtcaptcha
+				turnstile
+				cloudflare
+				amazon
+				amazon_waf
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
@@ -50,17 +54,18 @@
 [![Python versions](https://img.shields.io/pypi/pyversions/python3-capsolver.svg?logo=python&logoColor=FBE072)](https://badge.fury.io/py/python3-capsolver)
 [![Downloads](https://pepy.tech/badge/python3-capsolver/month)](https://pepy.tech/project/python3-capsolver)
 
 [![Maintainability](https://api.codeclimate.com/v1/badges/3c30167b5fb37a0775ea/maintainability)](https://codeclimate.com/github/AndreiDrang/python3-capsolver/maintainability)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/323d4eda0fe1477bbea8fe8902b9e97e)](https://www.codacy.com/gh/AndreiDrang/python3-capsolver/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AndreiDrang/python3-capsolver&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/AndreiDrang/python3-capsolver/branch/main/graph/badge.svg?token=2L4VVIF4G8)](https://codecov.io/gh/AndreiDrang/python3-capsolver)
 
-[![Build check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml)
-[![Installation check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml)
-[![Test](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml)
+[![Sphinx build](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/sphinx.yml/badge.svg?branch=release)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/sphinx.yml)
+[![Build](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/build.yml)
+[![Installation](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml)
+[![Tests](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml)
 [![Lint](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml)
 
 
 Python 3 library for [Capsolver](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1) service API.
 
 Tested on UNIX based OS.
 
@@ -90,10 +95,15 @@
 
 
 ## How to test?
 
 1. You need set ``API_KEY`` in your environment(get this value from you account).
 2. Run command ``make tests``, from root directory.
 
+
+### Changelog
+
+Check [releases page](https://github.com/AndreiDrang/python3-capsolver/releases).
+
 ### How to get API Key to work with the library
 1. On the page - https://dashboard.capsolver.com/overview/user-center
 2. Find it: ![img.png](files/img.png)
```

### Comparing `python3-capsolver-0.6/python3_capsolver/cloudflare.py` & `python3-capsolver-0.6.1/python3_capsolver/cloudflare.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/control.py` & `python3-capsolver-0.6.1/python3_capsolver/control.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     serializer = PostRequestSer
 
     def __init__(
         self,
         *args,
         **kwargs,
     ):
-
         super().__init__(*args, **kwargs)
 
     def get_balance(self) -> ControlResponseSer:
         """
         Synchronous method to view the balance
 
         Examples:
```

### Comparing `python3-capsolver-0.6/python3_capsolver/core/base.py` & `python3-capsolver-0.6.1/python3_capsolver/core/base.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/core/config.py` & `python3-capsolver-0.6.1/python3_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/core/enum.py` & `python3-capsolver-0.6.1/python3_capsolver/core/enum.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/core/serializer.py` & `python3-capsolver-0.6.1/python3_capsolver/core/serializer.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/datadome_slider.py` & `python3-capsolver-0.6.1/python3_capsolver/datadome_slider.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         websiteURL: str,
         captchaUrl: str,
         proxy: str,
         userAgent: str,
         *args,
         **kwargs,
     ):
-
         super().__init__(*args, **kwargs)
 
         if captcha_type in DatadomeSliderTypeEnm.list():
             self.task_params = DatadomeSliderSer(**locals()).dict()
         else:
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
```

### Comparing `python3-capsolver-0.6/python3_capsolver/fun_captcha.py` & `python3-capsolver-0.6.1/python3_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/gee_test.py` & `python3-capsolver-0.6.1/python3_capsolver/gee_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     Notes:
         https://docs.capsolver.com/guide/captcha/Geetest.html
     """
 
     def __init__(
         self, captcha_type: Union[GeeTestCaptchaTypeEnm, str], websiteURL: str, gt: str, challenge: str, *args, **kwargs
     ):
-
         super().__init__(*args, **kwargs)
 
         if captcha_type in GeeTestCaptchaTypeEnm.list():
             self.task_params = GeeTestSer(**locals()).dict()
         else:
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
```

### Comparing `python3-capsolver-0.6/python3_capsolver/hcaptcha.py` & `python3-capsolver-0.6.1/python3_capsolver/hcaptcha.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,14 @@
         CaptchaResponseSer model with full server response
 
     Notes:
         https://docs.capsolver.com/guide/captcha/HCaptcha.html
     """
 
     def __init__(self, captcha_type: Union[HCaptchaTypeEnm, str], websiteURL: str, websiteKey: str, *args, **kwargs):
-
         super().__init__(*args, **kwargs)
 
         if captcha_type in HCaptchaTypeEnm.list():
             self.task_params = WebsiteDataOptionsSer(**locals()).dict()
         else:
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
```

### Comparing `python3-capsolver-0.6/python3_capsolver/image_to_text.py` & `python3-capsolver-0.6.1/python3_capsolver/image_to_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 
     def __init__(
         self,
         api_key: str,
         sleep_time: int = 10,
         request_url: str = REQUEST_URL,
     ):
-
         super().__init__(api_key=api_key, sleep_time=sleep_time, request_url=request_url)
 
 
 class ImageToText(BaseImageToText):
     __doc__ = BaseImageToText.__doc__
 
     def captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
```

### Comparing `python3-capsolver-0.6/python3_capsolver/mt_captcha.py` & `python3-capsolver-0.6.1/python3_capsolver/mt_captcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver/recaptcha.py` & `python3-capsolver-0.6.1/python3_capsolver/recaptcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.6/python3_capsolver.egg-info/PKG-INFO` & `python3-capsolver-0.6.1/python3_capsolver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.6
+Version: 0.6.1
 Summary: Python 3.7+ Capsolver library with AIO module.
 Home-page: https://andreidrang.github.io/python3-capsolver/
 Author: AndreiDrang
 Author-email: python-captcha@pm.me
 License: MIT
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Source, https://github.com/AndreiDrang/python3-captchaai
 Keywords: captcha 
                 recaptcha
                 geetest
                 hcaptcha
                 capypuzzle
-                tiktok
                 rotatecaptcha
                 funcaptcha
                 keycaptcha
                 python3
                 python-library
                 capsolver
-                kasada
                 datadomeslider
+                datadome
                 mtcaptcha
+				turnstile
+				cloudflare
+				amazon
+				amazon_waf
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
@@ -50,17 +54,18 @@
 [![Python versions](https://img.shields.io/pypi/pyversions/python3-capsolver.svg?logo=python&logoColor=FBE072)](https://badge.fury.io/py/python3-capsolver)
 [![Downloads](https://pepy.tech/badge/python3-capsolver/month)](https://pepy.tech/project/python3-capsolver)
 
 [![Maintainability](https://api.codeclimate.com/v1/badges/3c30167b5fb37a0775ea/maintainability)](https://codeclimate.com/github/AndreiDrang/python3-capsolver/maintainability)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/323d4eda0fe1477bbea8fe8902b9e97e)](https://www.codacy.com/gh/AndreiDrang/python3-capsolver/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AndreiDrang/python3-capsolver&amp;utm_campaign=Badge_Grade)
 [![codecov](https://codecov.io/gh/AndreiDrang/python3-capsolver/branch/main/graph/badge.svg?token=2L4VVIF4G8)](https://codecov.io/gh/AndreiDrang/python3-capsolver)
 
-[![Build check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml)
-[![Installation check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml)
-[![Test](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml)
+[![Sphinx build](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/sphinx.yml/badge.svg?branch=release)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/sphinx.yml)
+[![Build](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/build.yml)
+[![Installation](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml)
+[![Tests](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml)
 [![Lint](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml)
 
 
 Python 3 library for [Capsolver](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1) service API.
 
 Tested on UNIX based OS.
 
@@ -90,10 +95,15 @@
 
 
 ## How to test?
 
 1. You need set ``API_KEY`` in your environment(get this value from you account).
 2. Run command ``make tests``, from root directory.
 
+
+### Changelog
+
+Check [releases page](https://github.com/AndreiDrang/python3-capsolver/releases).
+
 ### How to get API Key to work with the library
 1. On the page - https://dashboard.capsolver.com/overview/user-center
 2. Find it: ![img.png](files/img.png)
```

### Comparing `python3-capsolver-0.6/python3_capsolver.egg-info/SOURCES.txt` & `python3-capsolver-0.6.1/python3_capsolver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 python3_capsolver/cloudflare.py
 python3_capsolver/control.py
 python3_capsolver/datadome_slider.py
 python3_capsolver/fun_captcha.py
 python3_capsolver/gee_test.py
 python3_capsolver/hcaptcha.py
 python3_capsolver/image_to_text.py
-python3_capsolver/kasada.py
 python3_capsolver/mt_captcha.py
 python3_capsolver/recaptcha.py
 python3_capsolver.egg-info/PKG-INFO
 python3_capsolver.egg-info/SOURCES.txt
 python3_capsolver.egg-info/dependency_links.txt
 python3_capsolver.egg-info/not-zip-safe
 python3_capsolver.egg-info/requires.txt
```

### Comparing `python3-capsolver-0.6/setup.py` & `python3-capsolver-0.6.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,24 +90,27 @@
     license="MIT",
     keywords="""
               	captcha 
                 recaptcha
                 geetest
                 hcaptcha
                 capypuzzle
-                tiktok
                 rotatecaptcha
                 funcaptcha
                 keycaptcha
                 python3
                 python-library
                 capsolver
-                kasada
                 datadomeslider
+                datadome
                 mtcaptcha
+				turnstile
+				cloudflare
+				amazon
+				amazon_waf
                """,
     python_requires=REQUIRES_PYTHON,
     zip_safe=False,
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
@@ -116,14 +119,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Framework :: AsyncIO",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
     ],
     # Build - `python setup.py bdist_wheel`
     # Upload package: `python3 setup.py upload`
```

