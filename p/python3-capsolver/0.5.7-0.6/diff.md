# Comparing `tmp/python3-capsolver-0.5.7.tar.gz` & `tmp/python3-capsolver-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-capsolver-0.5.7.tar", last modified: Fri Apr 28 18:41:37 2023, max compression
+gzip compressed data, was "python3-capsolver-0.6.tar", last modified: Fri Apr 28 23:26:53 2023, max compression
```

## Comparing `python3-capsolver-0.5.7.tar` & `python3-capsolver-0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/
--rw-r--r--   0 homea     (1000) homea     (1000)     4701 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/PKG-INFO
--rw-r--r--   0 homea     (1000) homea     (1000)      389 2022-11-19 01:26:43.000000 python3-capsolver-0.5.7/pyproject.toml
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/python3_capsolver/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.5.7/python3_capsolver/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)       22 2023-04-28 18:41:27.000000 python3-capsolver-0.5.7/python3_capsolver/__version__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     2477 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/control.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/python3_capsolver/core/
--rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.5.7/python3_capsolver/core/__init__.py
--rw-r--r--   0 homea     (1000) homea     (1000)     8850 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/core/base.py
--rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.5.7/python3_capsolver/core/config.py
--rw-r--r--   0 homea     (1000) homea     (1000)     3489 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/core/enum.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4212 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/core/serializer.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6374 2023-04-28 18:34:47.000000 python3-capsolver-0.5.7/python3_capsolver/datadome_slider.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7880 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/fun_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4323 2023-04-28 18:30:07.000000 python3-capsolver-0.5.7/python3_capsolver/gee_test.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4831 2023-04-28 18:20:01.000000 python3-capsolver-0.5.7/python3_capsolver/hcaptcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     6350 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/image_to_text.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7509 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/kasada.py
--rw-r--r--   0 homea     (1000) homea     (1000)     7072 2023-04-28 18:34:47.000000 python3-capsolver-0.5.7/python3_capsolver/mt_captcha.py
--rw-r--r--   0 homea     (1000) homea     (1000)     4780 2023-04-28 18:41:20.000000 python3-capsolver-0.5.7/python3_capsolver/recaptcha.py
-drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/python3_capsolver.egg-info/
--rw-r--r--   0 homea     (1000) homea     (1000)     4701 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/PKG-INFO
--rw-r--r--   0 homea     (1000) homea     (1000)      782 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/SOURCES.txt
--rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/dependency_links.txt
--rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/not-zip-safe
--rw-r--r--   0 homea     (1000) homea     (1000)       60 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/requires.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       18 2023-04-28 18:41:37.000000 python3-capsolver-0.5.7/python3_capsolver.egg-info/top_level.txt
--rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 18:41:37.612970 python3-capsolver-0.5.7/setup.cfg
--rw-r--r--   0 homea     (1000) homea     (1000)     4053 2023-04-28 17:36:49.000000 python3-capsolver-0.5.7/setup.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/
+-rw-r--r--   0 homea     (1000) homea     (1000)     4699 2023-04-28 23:26:53.840542 python3-capsolver-0.6/PKG-INFO
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/python3_capsolver/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-10-28 01:40:08.000000 python3-capsolver-0.6/python3_capsolver/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)       20 2023-04-28 23:26:49.000000 python3-capsolver-0.6/python3_capsolver/__version__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4919 2023-04-28 23:01:33.000000 python3-capsolver-0.6/python3_capsolver/cloudflare.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1959 2023-04-28 23:25:46.000000 python3-capsolver-0.6/python3_capsolver/control.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/python3_capsolver/core/
+-rw-r--r--   0 homea     (1000) homea     (1000)        0 2022-11-07 03:20:28.000000 python3-capsolver-0.6/python3_capsolver/core/__init__.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     8722 2023-04-28 23:25:45.000000 python3-capsolver-0.6/python3_capsolver/core/base.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     1008 2023-04-28 16:29:39.000000 python3-capsolver-0.6/python3_capsolver/core/config.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3398 2023-04-28 23:03:36.000000 python3-capsolver-0.6/python3_capsolver/core/enum.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4381 2023-04-28 23:23:41.000000 python3-capsolver-0.6/python3_capsolver/core/serializer.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     3924 2023-04-28 23:01:33.000000 python3-capsolver-0.6/python3_capsolver/datadome_slider.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7880 2023-04-28 18:30:07.000000 python3-capsolver-0.6/python3_capsolver/fun_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4323 2023-04-28 18:30:07.000000 python3-capsolver-0.6/python3_capsolver/gee_test.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4831 2023-04-28 18:20:01.000000 python3-capsolver-0.6/python3_capsolver/hcaptcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6350 2023-04-28 18:41:20.000000 python3-capsolver-0.6/python3_capsolver/image_to_text.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     7509 2023-04-28 18:41:20.000000 python3-capsolver-0.6/python3_capsolver/kasada.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     4972 2023-04-28 22:33:29.000000 python3-capsolver-0.6/python3_capsolver/mt_captcha.py
+-rw-r--r--   0 homea     (1000) homea     (1000)     6394 2023-04-28 22:02:43.000000 python3-capsolver-0.6/python3_capsolver/recaptcha.py
+drwxr-xr-x   0 homea     (1000) homea     (1000)        0 2023-04-28 23:26:53.840542 python3-capsolver-0.6/python3_capsolver.egg-info/
+-rw-r--r--   0 homea     (1000) homea     (1000)     4699 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/PKG-INFO
+-rw-r--r--   0 homea     (1000) homea     (1000)      799 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)        1 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/not-zip-safe
+-rw-r--r--   0 homea     (1000) homea     (1000)       60 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/requires.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       18 2023-04-28 23:26:53.000000 python3-capsolver-0.6/python3_capsolver.egg-info/top_level.txt
+-rw-r--r--   0 homea     (1000) homea     (1000)       38 2023-04-28 23:26:53.840542 python3-capsolver-0.6/setup.cfg
+-rw-r--r--   0 homea     (1000) homea     (1000)     4053 2023-04-28 17:36:49.000000 python3-capsolver-0.6/setup.py
```

### Comparing `python3-capsolver-0.5.7/PKG-INFO` & `python3-capsolver-0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.5.7
+Version: 0.6
 Summary: Python 3.7+ Capsolver library with AIO module.
 Home-page: https://andreidrang.github.io/python3-capsolver/
 Author: AndreiDrang
 Author-email: python-captcha@pm.me
 License: MIT
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Source, https://github.com/AndreiDrang/python3-captchaai
@@ -38,30 +38,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
 
 # python3-capsolver
-![Python3-Capsolver](https://github.com/AndreiDrang/python3-capsolver/blob/main/files/CaptchaAISm.png)
+![Python3-Capsolver](https://github.com/AndreiDrang/python3-capsolver/blob/main/files/CapsolverSm.png)
 
 [![Capsolver](https://user-images.githubusercontent.com/16991365/234852229-6e4b3f3c-f498-4fd5-9a6b-f7f269dd4bfc.gif)](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1)
 
-[![PyPI version](https://badge.fury.io/py/python3-captchaai.svg)](https://badge.fury.io/py/python3-captchaai)
-[![Python versions](https://img.shields.io/pypi/pyversions/python3-captchaai.svg?logo=python&logoColor=FBE072)](https://badge.fury.io/py/python3-captchaai)
-[![Downloads](https://pepy.tech/badge/python3-captchaai/month)](https://pepy.tech/project/python3-captchaai)
-
-[![Maintainability](https://api.codeclimate.com/v1/badges/3431fd3fe71baf7eb9da/maintainability)](https://codeclimate.com/github/AndreiDrang/python3-captchaai/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/323d4eda0fe1477bbea8fe8902b9e97e)](https://www.codacy.com/gh/AndreiDrang/python3-captchaai/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AndreiDrang/python3-captchaai&amp;utm_campaign=Badge_Grade)
-[![codecov](https://codecov.io/gh/AndreiDrang/python3-captchaai/branch/main/graph/badge.svg?token=2L4VVIF4G8)](https://codecov.io/gh/AndreiDrang/python3-captchaai)
-
-[![Build check](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test_build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test_build.yml)
-[![Installation check](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/install.yml)
-[![Test](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test.yml)
-[![Lint](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/lint.yml)
+[![PyPI version](https://badge.fury.io/py/python3-capsolver.svg)](https://badge.fury.io/py/python3-capsolver)
+[![Python versions](https://img.shields.io/pypi/pyversions/python3-capsolver.svg?logo=python&logoColor=FBE072)](https://badge.fury.io/py/python3-capsolver)
+[![Downloads](https://pepy.tech/badge/python3-capsolver/month)](https://pepy.tech/project/python3-capsolver)
+
+[![Maintainability](https://api.codeclimate.com/v1/badges/3c30167b5fb37a0775ea/maintainability)](https://codeclimate.com/github/AndreiDrang/python3-capsolver/maintainability)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/323d4eda0fe1477bbea8fe8902b9e97e)](https://www.codacy.com/gh/AndreiDrang/python3-capsolver/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AndreiDrang/python3-capsolver&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/AndreiDrang/python3-capsolver/branch/main/graph/badge.svg?token=2L4VVIF4G8)](https://codecov.io/gh/AndreiDrang/python3-capsolver)
+
+[![Build check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml)
+[![Installation check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml)
+[![Test](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml)
+[![Lint](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml)
 
 
 Python 3 library for [Capsolver](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1) service API.
 
 Tested on UNIX based OS.
 
 The library is intended for software developers and is used to work with the [Capsolver](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1) service API.
@@ -72,25 +72,25 @@
 
 Or email python-captcha@pm.me
 
 ***
 
 ## How to install?
 
-We recommend using the latest version of Python. `python3-captchaai` supports Python 3.7+.
+We recommend using the latest version of Python. `python3-capsolver` supports Python 3.7+.
 
 ### pip
 
 ```bash
-pip install python3-captchaai
+pip install python3-capsolver
 ```
 
 ## How to use?
 
-Is described in the [documentation-website](https://andreidrang.github.io/python3-captchaai/).
+Is described in the [documentation-website](https://andreidrang.github.io/python3-capsolver/).
 
 
 ## How to test?
 
 1. You need set ``API_KEY`` in your environment(get this value from you account).
 2. Run command ``make tests``, from root directory.
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver/core/base.py` & `python3-capsolver-0.6/python3_capsolver/core/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,17 @@
         return self.created_task_data
 
     def _create_task(self, url_postfix: str = EndpointPostfixEnm.CREATE_TASK.value) -> dict:
         """
         Function send SYNC request to service and wait for result
         """
         try:
-            print(self.task_payload.dict(exclude_none=True))
             resp = self.__session.post(
                 parse.urljoin(self.__request_url, url_postfix), json=self.task_payload.dict(exclude_none=True)
             )
-            print(resp.status_code)
-            print(resp.json())
             if resp.status_code in VALID_STATUS_CODES:
                 return resp.json()
             else:
                 raise ValueError(resp.raise_for_status())
         except Exception as error:
             logging.exception(error)
             raise
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver/core/config.py` & `python3-capsolver-0.6/python3_capsolver/core/config.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.7/python3_capsolver/core/enum.py` & `python3-capsolver-0.6/python3_capsolver/core/enum.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,23 +48,20 @@
     """
     Enum with all available captcha types
 
     Notes:
         https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/393295
     """
 
-    Control = "Control"  # custom captcha type
     ImageToTextTask = "ImageToTextTask"
     # HCaptcha
     HCaptchaClassification = "HCaptchaClassification"
     # FunCaptcha
     FunCaptchaClassification = "FunCaptchaClassification"
     # Other types
-    MtCaptchaTask = "MtCaptchaTask"
-    DatadomeSliderTask = "DatadomeSliderTask"
     AntiKasadaTask = "AntiKasadaTask"
     AntiAkamaiBMPTask = "AntiAkamaiBMPTask"
 
 
 class HCaptchaTypeEnm(str, MyEnum):
     HCaptchaTask = "HCaptchaTask"
     HCaptchaTaskProxyless = "HCaptchaTaskProxyless"
@@ -95,33 +92,32 @@
 class ReCaptchaV3TypeEnm(str, MyEnum):
     ReCaptchaV3Task = "ReCaptchaV3Task"
     ReCaptchaV3EnterpriseTask = "ReCaptchaV3EnterpriseTask"
     ReCaptchaV3TaskProxyLess = "ReCaptchaV3TaskProxyLess"
     ReCaptchaV3EnterpriseTaskProxyLess = "ReCaptchaV3EnterpriseTaskProxyLess"
 
 
+class MtCaptchaTypeEnm(str, MyEnum):
+    MtCaptchaTask = "MtCaptchaTask"
+    MtCaptchaTaskProxyLess = "MtCaptchaTaskProxyLess"
+
+
+class DatadomeSliderTypeEnm(str, MyEnum):
+    DatadomeSliderTask = "DatadomeSliderTask"
+
+
+class CloudflareTypeEnm(str, MyEnum):
+    AntiCloudflareTask = "AntiCloudflareTask"
+
+
 class ResponseStatusEnm(str, MyEnum):
     """
     Enum store results `status` field variants
 
     Notes:
         https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426124
     """
 
     Idle = "idle"  # Task created
     Processing = "processing"  # Task is not ready yet
     Ready = "ready"  # Task completed, solution object can be found in solution property
     Failed = "failed"  # Task failed, check the errorDescription to know why failed.
-
-
-class ProxyType(str, MyEnum):
-    """
-    Enum store proxy types
-
-    Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426124
-    """
-
-    http = "http"  # usual http / https
-    https = "https"
-    socks4 = "socks4"
-    socks5 = "socks5"
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver/core/serializer.py` & `python3-capsolver-0.6/python3_capsolver/core/serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 """
 HTTP API Request ser
 """
 
 
 class PostRequestSer(BaseModel):
     clientKey: str = Field(..., description="Client account key, can be found in user account")
+    task: dict = Field(None, description="Task object")
 
 
 class TaskSer(BaseModel):
     type: str = Field(..., description="Task type name", alias="captcha_type")
 
 
 class RequestCreateTaskSer(PostRequestSer):
-    task: dict = Field(None, description="Task object")
     appId: str = Field(APP_ID, description="AppID", const=True)
 
 
 class RequestGetTaskResultSer(PostRequestSer):
     taskId: Optional[str] = Field(None, description="ID created by the createTask method")
 
 
@@ -46,15 +46,14 @@
 
     class Config:
         allow_population_by_field_name = True
 
 
 class ControlResponseSer(ResponseSer):
     balance: Optional[float] = Field(0, description="Account balance value in USD")
-    packages: List = Field(None, description="Monthly Packages")
 
 
 """
 Other ser
 """
 
 
@@ -66,15 +65,15 @@
 """
 Captcha tasks ser
 """
 
 
 class WebsiteDataOptionsSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with Captcha")
-    websiteKey: str = Field(..., description="Website key")
+    websiteKey: Optional[str] = Field(None, description="Website key")
 
 
 class ReCaptchaV3Ser(WebsiteDataOptionsSer):
     pageAction: str = Field(
         "verify",
         description="Widget action value."
         "Website owner defines what user is doing on the page through this parameter",
@@ -103,24 +102,29 @@
     funcaptchaApiJSSubdomain: Optional[str] = Field(
         None,
         description="A special subdomain of funcaptcha.com, from which the JS captcha widget should be loaded."
         "Most FunCaptcha installations work from shared domains.",
     )
 
 
-class DatadomeSliderOptionsSer(BaseModel):
+class DatadomeSliderSer(TaskSer):
     websiteURL: str = Field(..., description="Address of a webpage with DatadomeSlider")
     captchaUrl: str = Field(..., description="Captcha Url where is the captcha")
-
-
-class MtCaptchaOptionsSer(WebsiteDataOptionsSer):
-    proxy: str = Field(..., description="String with proxy connection params, example: `198.22.3.1:10001:user:pwd`")
+    proxy: str = Field(..., description="Proxy data")
+    userAgent: str = Field(..., description="Browser's User-Agent which is used in emulation")
 
 
 class KasadaOptionsSer(BaseModel):
     pageURL: str = Field(..., description="Address of a webpage with Kasada")
     proxyLogin: str = Field(
         ...,
         description="Login for proxy which requires authorizaiton (basic)."
         "This isn’t required if you are using proxies authenticated by IP",
     )
     proxyPassword: str = Field(..., description="This isn’t required if you are using proxies authenticated by IP")
+
+
+class CloudflareTurnstileSer(WebsiteDataOptionsSer):
+    metadata: dict = Field(..., description="Extra data")
+    html: Optional[str] = Field(
+        None, description="You can pass in the entire html source code for the challenge directly."
+    )
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver/datadome_slider.py` & `python3-capsolver-0.6/python3_capsolver/image_to_text.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,160 +1,148 @@
-from typing import Union, Optional
-
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import ProxyType
 from python3_capsolver.core.config import REQUEST_URL
-from python3_capsolver.core.serializer import CaptchaResponseSer, RequestCreateTaskSer, DatadomeSliderOptionsSer
+from python3_capsolver.core.serializer import CaptchaResponseSer, RequestCreateTaskSer
 
 
-class BaseDatadomeSlider(BaseCaptcha):
+class BaseImageToText(BaseCaptcha):
     """
-    The class is used to work with Capsolver DatadomeSlider method.
+    The class is used to work with Capsolver Image captcha solving methods.
 
     Args:
         api_key: Capsolver API key
-        websiteURL: Address of the webpage
-        captchaUrl: Captcha Url where is the captcha
-        proxyType: Type of the proxy
-        proxyAddress: Proxy IP address IPv4/IPv6. Not allowed to use:
-                        host names instead of IPs,
-                        transparent proxies (where client IP is visible),
-                        proxies from local networks (192.., 10.., 127...)
-        proxyPort: Proxy port.
         sleep_time: The waiting time between requests to get the result of the Captcha
         request_url: API address for sending requests
 
     Examples:
-        >>> DatadomeSlider(api_key="CAI-1324...",
-        ...         websiteURL="https://www.some-url.com/",
-        ...         captchaUrl="https://www.some-url.com/to-page-with-captcha",
-        ...         proxyType="http",
-        ...         proxyAddress="0.0.0.0",
-        ...         proxyPort=9090,
-        ...        ).captcha_handler()
+        >>> with open('some_image.jpeg', 'rb') as img_file:
+        ...    img_data = img_file.read()
+        >>> body = base64.b64encode(img_data).decode("utf-8")
+        >>> ImageToText(api_key="CAI-12345....").captcha_handler(body=body)
+        CaptchaResponseSer(errorId=False,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={'gRecaptchaResponse': '44795sds...'}
+                          )
+
+        >>> with open('some_image.jpeg', 'rb') as img_file:
+        ...    img_data = img_file.read()
+        >>> body = base64.b64encode(img_data).decode("utf-8")
+        >>> with ImageToText(api_key="CAI-12345....") as image_to_text_inst:
+        ...    image_to_text_inst.captcha_handler(body=body)
+        CaptchaResponseSer(errorId=False,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                           solution={'gRecaptchaResponse': '44795sds...'}
+                          )
+
+        >>> with open('some_image.jpeg', 'rb') as img_file:
+        ...    img_data = img_file.read()
+        >>> body = base64.b64encode(img_data).decode("utf-8")
+        >>> await ImageToText(api_key="CAI-12345....").aio_captcha_handler(body=body)
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
-        >>> await DatadomeSlider(api_key="CAI-1324...",
-        ...         websiteURL="https://www.some-url.com/",
-        ...         captchaUrl="https://www.some-url.com/to-page-with-captcha",
-        ...         proxyType="http",
-        ...         proxyAddress="0.0.0.0",
-        ...         proxyPort=9090,
-        ...        ).aio_captcha_handler()
+        >>> with open('some_image.jpeg', 'rb') as img_file:
+        ...    img_data = img_file.read()
+        >>> body = base64.b64encode(img_data).decode("utf-8")
+        >>> with ImageToText(api_key="CAI-12345....") as image_to_text_inst:
+        ...    await image_to_text_inst.aio_captcha_handler(body=body)
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
                            solution={'gRecaptchaResponse': '44795sds...'}
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/426393/
+        https://captchaai.atlassian.net/wiki/spaces/CAPTCHAAI/pages/393427
     """
 
     def __init__(
         self,
         api_key: str,
-        websiteURL: str,
-        captchaUrl: str,
-        proxyType: Union[ProxyType, str],
-        proxyAddress: str,
-        proxyPort: int,
-        sleep_time: Optional[int] = 5,
-        request_url: Optional[str] = REQUEST_URL,
+        sleep_time: int = 10,
+        request_url: str = REQUEST_URL,
     ):
 
-        super().__init__(
-            api_key=api_key,
-            sleep_time=sleep_time,
-            request_url=request_url,
-        )
-
-        self.task_params = DatadomeSliderOptionsSer(**locals()).dict()
+        super().__init__(api_key=api_key, sleep_time=sleep_time, request_url=request_url)
 
 
-class DatadomeSlider(BaseDatadomeSlider):
-    __doc__ = BaseDatadomeSlider.__doc__
+class ImageToText(BaseImageToText):
+    __doc__ = BaseImageToText.__doc__
 
-    def captcha_handler(
-        self,
-        **additional_params,
-    ) -> CaptchaResponseSer:
+    def captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
         """
         Synchronous method for captcha solving
 
         Args:
+            body: Base64 encoded content of the image
             additional_params: Some additional parameters that will be used in creating the task
-                                and will be passed to the payload under ``task`` key.
-                                Like ``proxyPassword``, ``userAgent`` and etc. - more info in service docs
+                                and will be passed to the payload under ``task`` key
 
         Examples:
-            >>> DatadomeSlider(api_key="CAI-1324...",
-            ...         websiteURL="https://www.some-url.com/",
-            ...         captchaUrl="https://www.some-url.com/to-page-with-captcha",
-            ...         proxyType="http",
-            ...         proxyAddress="0.0.0.0",
-            ...         proxyPort=9090,
-            ...        ).captcha_handler()
+            >>> with open('some_image.jpeg', 'rb') as img_file:
+            ...    img_data = img_file.read()
+            >>> body = base64.b64encode(img_data).decode("utf-8")
+            >>> ImageToText(api_key="CAI-12345....").captcha_handler(body=body)
             CaptchaResponseSer(errorId=False,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'gRecaptchaResponse': '44795sds...'}
                               )
 
         Returns:
-            CaptchaResponseSer model with full service response
+            CaptchaResponseSer model with full server response
 
         Notes:
             Check class docstring for more info
         """
-        return self._processing_captcha(serializer=RequestCreateTaskSer, type=self.captcha_type, **additional_params)
+        return self._processing_captcha(
+            serializer=RequestCreateTaskSer, type=self.captcha_type, body=body, **additional_params
+        )
 
-    async def aio_captcha_handler(
-        self,
-        **additional_params,
-    ) -> CaptchaResponseSer:
+    async def aio_captcha_handler(self, body: str, **additional_params) -> CaptchaResponseSer:
         """
         Asynchronous method for captcha solving
 
         Args:
+            body: Base64 encoded content of the image
             additional_params: Some additional parameters that will be used in creating the task
-                                and will be passed to the payload under ``task`` key.
-                                Like ``coordinate``, ``enterprisePayload`` and etc. - more info in service docs
+                                and will be passed to the payload under ``task`` key
 
         Examples:
-            >>> await DatadomeSlider(api_key="CAI-1324...",
-            ...         websiteURL="https://www.some-url.com/",
-            ...         captchaUrl="https://www.some-url.com/to-page-with-captcha",
-            ...         proxyType="http",
-            ...         proxyAddress="0.0.0.0",
-            ...         proxyPort=9090,
-            ...        ).aio_captcha_handler()
+            >>> with open('some_image.jpeg', 'rb') as img_file:
+            ...    img_data = img_file.read()
+            >>> body = base64.b64encode(img_data).decode("utf-8")
+            >>> await ImageToText(api_key="CAI-12345....").aio_captcha_handler(body=body)
             CaptchaResponseSer(errorId=False,
                                errorCode=None,
                                errorDescription=None,
                                taskId='73bdcd28-6c77-4414-8....',
                                status=<ResponseStatusEnm.Ready: 'ready'>,
                                solution={'gRecaptchaResponse': '44795sds...'}
                               )
 
         Returns:
-            CaptchaResponseSer model with full service response
+            CaptchaResponseSer model with full server response
 
         Notes:
             Check class docstring for more info
         """
         return await self._aio_processing_captcha(
-            serializer=RequestCreateTaskSer, type=self.captcha_type, **additional_params
+            serializer=RequestCreateTaskSer, type=self.captcha_type, body=body, **additional_params
         )
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver/fun_captcha.py` & `python3-capsolver-0.6/python3_capsolver/fun_captcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.7/python3_capsolver/gee_test.py` & `python3-capsolver-0.6/python3_capsolver/gee_test.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.7/python3_capsolver/hcaptcha.py` & `python3-capsolver-0.6/python3_capsolver/hcaptcha.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.7/python3_capsolver/kasada.py` & `python3-capsolver-0.6/python3_capsolver/kasada.py`

 * *Files identical despite different names*

### Comparing `python3-capsolver-0.5.7/python3_capsolver/recaptcha.py` & `python3-capsolver-0.6/python3_capsolver/mt_captcha.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,94 +1,104 @@
-from typing import Union, Optional
+from typing import Union
 
 from python3_capsolver.core.base import BaseCaptcha
-from python3_capsolver.core.enum import ReCaptchaV2TypeEnm, ReCaptchaV3TypeEnm
-from python3_capsolver.core.serializer import ReCaptchaV3Ser, CaptchaResponseSer, WebsiteDataOptionsSer
+from python3_capsolver.core.enum import MtCaptchaTypeEnm
+from python3_capsolver.core.serializer import CaptchaResponseSer, WebsiteDataOptionsSer
 
 
-class ReCaptcha(BaseCaptcha):
+class MtCaptcha(BaseCaptcha):
     """
-    The class is used to work with Capsolver ReCaptcha methods.
+    The class is used to work with Capsolver MtCaptcha method.
 
     Args:
         api_key: Capsolver API key
-        captcha_type: Captcha type name, like ``ReCaptchaV2Task`` and etc.
+        captcha_type: Captcha type name, like ``MtCaptchaTask`` and etc.
         websiteURL: Address of a webpage with Google ReCaptcha
         websiteKey: Recaptcha website key. <div class="g-recaptcha" data-sitekey="THAT_ONE"></div>
-        pageAction: Widget action value. Website owner defines what user is doing on the page through this parameter.
-                    Default value: ``verify``. Example: grecaptcha.execute('site_key', {action:'login_test'}).
 
     Examples:
-        >>> ReCaptcha(api_key="CAI-1324...",
-        ...           captcha_type="ReCaptchaV2TaskProxyLess",
-        ...           websiteURL="https://www.google.com/recaptcha/api2/demo",
-        ...           websiteKey="6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
-        ...          ).captcha_handler()
+        >>> MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTaskProxyLess,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).captcha_handler()
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
-        >>> ReCaptcha(api_key="CAI-1324...",
-        ...           captcha_type=ReCaptchaV2TypeEnm.ReCaptchaV2TaskProxyLess,
-        ...           websiteURL="https://www.google.com/recaptcha/api2/demo",
-        ...           websiteKey="6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-"
-        ...          ).captcha_handler()
+        >>> MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).captcha_handler()
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
-        >>> ReCaptcha(api_key="CAI-1324...",
-        ...           captcha_type=ReCaptchaV2TypeEnm.ReCaptchaV2Task,
-        ...           websiteURL="https://www.google.com/recaptcha/api2/demo",
-        ...           websiteKey="6Le-wvkSAAAAAPBMRTvw0Q4Muexq9bi0DJwx_mJ-",
-        ...           proxy="socks5:192.191.100.10:4780:user:pwd"
-        ...          ).captcha_handler()
+        >>> await MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).aio_captcha_handler()
         CaptchaResponseSer(errorId=False,
                            errorCode=None,
                            errorDescription=None,
                            taskId='73bdcd28-6c77-4414-8....',
                            status=<ResponseStatusEnm.Ready: 'ready'>,
-                           solution={'gRecaptchaResponse': '44795sds...'}
+                           solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
+                          )
+
+        >>> await MtCaptcha(api_key="CAI-1324...",
+        ...         captcha_type=MtCaptchaTypeEnm.MtCaptchaTask,
+        ...         websiteURL="https://www.mtcaptcha.com/#mtcaptcha-demo",
+        ...         websiteKey="MTPublic-tqNCRE0GS",
+        ...         proxy="198.22.3.1:10001:user:pwd"
+        ...        ).aio_captcha_handler()
+        CaptchaResponseSer(errorId=False,
+                           errorCode=None,
+                           errorDescription=None,
+                           taskId='73bdcd28-6c77-4414-8....',
+                           status=<ResponseStatusEnm.Ready: 'ready'>,
+                            solution={'token': 'v1(03,79a,MTPublic-tqNCRE0GS,c9...'}
                           )
 
     Returns:
         CaptchaResponseSer model with full server response
 
     Notes:
-        https://docs.capsolver.com/guide/captcha/ReCaptchaV2.html
-        https://docs.capsolver.com/guide/captcha/ReCaptchaV3.html
+        https://docs.capsolver.com/guide/captcha/MtCaptcha.html
     """
 
     def __init__(
         self,
-        captcha_type: Union[ReCaptchaV2TypeEnm, ReCaptchaV3TypeEnm, str],
+        captcha_type: Union[MtCaptchaTypeEnm, str],
         websiteURL: str,
         websiteKey: str,
-        pageAction: Optional[str] = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
 
-        if captcha_type in ReCaptchaV2TypeEnm.list():
+        if captcha_type in MtCaptchaTypeEnm.list():
             self.task_params = WebsiteDataOptionsSer(**locals()).dict()
-        elif captcha_type in ReCaptchaV3TypeEnm.list():
-            self.task_params = ReCaptchaV3Ser(**locals()).dict()
         else:
             raise ValueError(
                 f"""Invalid `captcha_type` parameter set for `{self.__class__.__name__}`,
-                available - {ReCaptchaV2TypeEnm.list(), ReCaptchaV3TypeEnm.list()}"""
+                available - {MtCaptchaTypeEnm}"""
             )
         for key in kwargs:
             self.task_params.update({key: kwargs[key]})
 
     def captcha_handler(self) -> CaptchaResponseSer:
         """
         Sync method for captcha solving
@@ -101,15 +111,14 @@
         """
         return self._processing_captcha(create_params=self.task_params)
 
     async def aio_captcha_handler(self) -> CaptchaResponseSer:
         """
         Async method for captcha solving
 
-
         Returns:
             CaptchaResponseSer model with full service response
 
         Notes:
             Check class docstring for more info
         """
         return await self._aio_processing_captcha(create_params=self.task_params)
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver.egg-info/PKG-INFO` & `python3-capsolver-0.6/python3_capsolver.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-capsolver
-Version: 0.5.7
+Version: 0.6
 Summary: Python 3.7+ Capsolver library with AIO module.
 Home-page: https://andreidrang.github.io/python3-capsolver/
 Author: AndreiDrang
 Author-email: python-captcha@pm.me
 License: MIT
 Project-URL: Documentation, https://andreidrang.github.io/python3-capsolver/
 Project-URL: Source, https://github.com/AndreiDrang/python3-captchaai
@@ -38,30 +38,30 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 
 
 # python3-capsolver
-![Python3-Capsolver](https://github.com/AndreiDrang/python3-capsolver/blob/main/files/CaptchaAISm.png)
+![Python3-Capsolver](https://github.com/AndreiDrang/python3-capsolver/blob/main/files/CapsolverSm.png)
 
 [![Capsolver](https://user-images.githubusercontent.com/16991365/234852229-6e4b3f3c-f498-4fd5-9a6b-f7f269dd4bfc.gif)](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1)
 
-[![PyPI version](https://badge.fury.io/py/python3-captchaai.svg)](https://badge.fury.io/py/python3-captchaai)
-[![Python versions](https://img.shields.io/pypi/pyversions/python3-captchaai.svg?logo=python&logoColor=FBE072)](https://badge.fury.io/py/python3-captchaai)
-[![Downloads](https://pepy.tech/badge/python3-captchaai/month)](https://pepy.tech/project/python3-captchaai)
-
-[![Maintainability](https://api.codeclimate.com/v1/badges/3431fd3fe71baf7eb9da/maintainability)](https://codeclimate.com/github/AndreiDrang/python3-captchaai/maintainability)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/323d4eda0fe1477bbea8fe8902b9e97e)](https://www.codacy.com/gh/AndreiDrang/python3-captchaai/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AndreiDrang/python3-captchaai&amp;utm_campaign=Badge_Grade)
-[![codecov](https://codecov.io/gh/AndreiDrang/python3-captchaai/branch/main/graph/badge.svg?token=2L4VVIF4G8)](https://codecov.io/gh/AndreiDrang/python3-captchaai)
-
-[![Build check](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test_build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test_build.yml)
-[![Installation check](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/install.yml)
-[![Test](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/test.yml)
-[![Lint](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-captchaai/actions/workflows/lint.yml)
+[![PyPI version](https://badge.fury.io/py/python3-capsolver.svg)](https://badge.fury.io/py/python3-capsolver)
+[![Python versions](https://img.shields.io/pypi/pyversions/python3-capsolver.svg?logo=python&logoColor=FBE072)](https://badge.fury.io/py/python3-capsolver)
+[![Downloads](https://pepy.tech/badge/python3-capsolver/month)](https://pepy.tech/project/python3-capsolver)
+
+[![Maintainability](https://api.codeclimate.com/v1/badges/3c30167b5fb37a0775ea/maintainability)](https://codeclimate.com/github/AndreiDrang/python3-capsolver/maintainability)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/323d4eda0fe1477bbea8fe8902b9e97e)](https://www.codacy.com/gh/AndreiDrang/python3-capsolver/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=AndreiDrang/python3-capsolver&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/AndreiDrang/python3-capsolver/branch/main/graph/badge.svg?token=2L4VVIF4G8)](https://codecov.io/gh/AndreiDrang/python3-capsolver)
+
+[![Build check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test_build.yml)
+[![Installation check](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/install.yml)
+[![Test](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/test.yml)
+[![Lint](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/AndreiDrang/python3-capsolver/actions/workflows/lint.yml)
 
 
 Python 3 library for [Capsolver](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1) service API.
 
 Tested on UNIX based OS.
 
 The library is intended for software developers and is used to work with the [Capsolver](https://dashboard.capsolver.com/passport/register?inviteCode=kQTn-tG07Jb1) service API.
@@ -72,25 +72,25 @@
 
 Or email python-captcha@pm.me
 
 ***
 
 ## How to install?
 
-We recommend using the latest version of Python. `python3-captchaai` supports Python 3.7+.
+We recommend using the latest version of Python. `python3-capsolver` supports Python 3.7+.
 
 ### pip
 
 ```bash
-pip install python3-captchaai
+pip install python3-capsolver
 ```
 
 ## How to use?
 
-Is described in the [documentation-website](https://andreidrang.github.io/python3-captchaai/).
+Is described in the [documentation-website](https://andreidrang.github.io/python3-capsolver/).
 
 
 ## How to test?
 
 1. You need set ``API_KEY`` in your environment(get this value from you account).
 2. Run command ``make tests``, from root directory.
```

### Comparing `python3-capsolver-0.5.7/python3_capsolver.egg-info/SOURCES.txt` & `python3-capsolver-0.6/python3_capsolver.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyproject.toml
 setup.py
 python3_capsolver/__init__.py
 python3_capsolver/__version__.py
+python3_capsolver/cloudflare.py
 python3_capsolver/control.py
 python3_capsolver/datadome_slider.py
 python3_capsolver/fun_captcha.py
 python3_capsolver/gee_test.py
 python3_capsolver/hcaptcha.py
 python3_capsolver/image_to_text.py
 python3_capsolver/kasada.py
```

### Comparing `python3-capsolver-0.5.7/setup.py` & `python3-capsolver-0.6/setup.py`

 * *Files identical despite different names*

