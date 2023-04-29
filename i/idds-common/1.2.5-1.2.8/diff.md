# Comparing `tmp/idds-common-1.2.5.tar.gz` & `tmp/idds-common-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-common-1.2.5.tar", last modified: Tue Apr 25 19:17:57 2023, max compression
+gzip compressed data, was "idds-common-1.2.8.tar", last modified: Sat Apr 29 14:38:38 2023, max compression
```

## Comparing `idds-common-1.2.5.tar` & `idds-common-1.2.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.384358 idds-common-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-25 19:17:47.000000 idds-common-1.2.5/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-25 19:17:57.384358 idds-common-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-25 19:17:47.000000 idds-common-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.380358 idds-common-1.2.5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.380358 idds-common-1.2.5/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.384358 idds-common-1.2.5/lib/idds/common/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/dict_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.384358 idds-common-1.2.5/lib/idds/common/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/plugin/plugin_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-25 19:17:47.000000 idds-common-1.2.5/lib/idds/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 19:17:56.000000 idds-common-1.2.5/lib/idds/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.384358 idds-common-1.2.5/lib/idds_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-25 19:17:57.000000 idds-common-1.2.5/lib/idds_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 19:17:57.000000 idds-common-1.2.5/lib/idds_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 19:17:57.000000 idds-common-1.2.5/lib/idds_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-25 19:17:57.000000 idds-common-1.2.5/lib/idds_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-25 19:17:57.000000 idds-common-1.2.5/lib/idds_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-25 19:17:57.384358 idds-common-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-25 19:17:47.000000 idds-common-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.380358 idds-common-1.2.5/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 19:17:57.384358 idds-common-1.2.5/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-25 19:17:56.000000 idds-common-1.2.5/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.487873 idds-common-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-29 14:38:28.000000 idds-common-1.2.8/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-29 14:38:38.487873 idds-common-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-29 14:38:28.000000 idds-common-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.483873 idds-common-1.2.8/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.483873 idds-common-1.2.8/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.487873 idds-common-1.2.8/lib/idds/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/dict_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.487873 idds-common-1.2.8/lib/idds/common/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/plugin/plugin_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18657 2023-04-29 14:38:28.000000 idds-common-1.2.8/lib/idds/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-29 14:38:37.000000 idds-common-1.2.8/lib/idds/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.487873 idds-common-1.2.8/lib/idds_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-29 14:38:38.000000 idds-common-1.2.8/lib/idds_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-29 14:38:38.000000 idds-common-1.2.8/lib/idds_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:38:38.000000 idds-common-1.2.8/lib/idds_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 14:38:38.000000 idds-common-1.2.8/lib/idds_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-29 14:38:38.000000 idds-common-1.2.8/lib/idds_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-29 14:38:38.487873 idds-common-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-29 14:38:28.000000 idds-common-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.483873 idds-common-1.2.8/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:38:38.487873 idds-common-1.2.8/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-29 14:38:37.000000 idds-common-1.2.8/tools/env/environment.yml
```

### Comparing `idds-common-1.2.5/LICENSE.rst` & `idds-common-1.2.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/PKG-INFO` & `idds-common-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.2.5
+Version: 1.2.8
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.2.5/lib/idds/common/authentication.py` & `idds-common-1.2.8/lib/idds/common/authentication.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,19 +41,26 @@
 def decode_value(val):
     if isinstance(val, str):
         val = val.encode()
     decoded = base64.urlsafe_b64decode(val + b'==')
     return int.from_bytes(decoded, 'big')
 
 
-def should_verify(no_verify=False):
+def should_verify(no_verify=False, ssl_verify=None):
     if no_verify:
         return False
     if os.environ.get('IDDS_AUTH_NO_VERIFY', None):
         return False
+
+    if os.environ.get('IDDS_AUTH_SSL_VERIFY', None):
+        return os.environ.get('IDDS_AUTH_SSL_VERIFY', None)
+
+    if ssl_verify:
+        return ssl_verify
+
     return True
 
 
 class BaseAuthentication(object):
     def __init__(self, timeout=None):
         self.timeout = timeout
         self.config = self.load_auth_server_config()
@@ -85,32 +92,43 @@
                 allow_vos_temp = self.config.get(section, 'allow_vos')
                 allow_vos_temp = allow_vos_temp.split(',')
                 for t in allow_vos_temp:
                     t = t.strip()
                     allow_vos.append(t)
         return allow_vos
 
+    def get_ssl_verify(self):
+        section = 'common'
+        ssl_verify = None
+        if self.config and self.config.has_section(section):
+            if self.config.has_option(section, 'ssl_verify'):
+                ssl_verify = self.config.get(section, 'ssl_verify')
+        return ssl_verify
+
 
 class OIDCAuthentication(BaseAuthentication):
     def __init__(self, timeout=None):
         super(OIDCAuthentication, self).__init__(timeout=timeout)
 
     def get_auth_config(self, vo):
         ret = {'vo': vo, 'oidc_config_url': None, 'client_id': None,
-               'client_secret': None, 'audience': None, 'no_verify': True}
+               'client_secret': None, 'audience': None, 'no_verify': False}
 
         if self.config and self.config.has_section(vo):
-            for name in ['oidc_config_url', 'client_id', 'client_secret', 'vo', 'audience', 'no_verify']:
+            for name in ['oidc_config_url', 'client_id', 'client_secret', 'vo', 'audience']:
                 if self.config.has_option(vo, name):
                     ret[name] = self.config.get(vo, name)
+            for name in ['no_verify']:
+                if self.config.has_option(vo, name):
+                    ret[name] = self.config.getboolean(vo, name)
         return ret
 
     def get_http_content(self, url, no_verify=False):
         try:
-            r = requests.get(url, allow_redirects=True, verify=should_verify(no_verify))
+            r = requests.get(url, allow_redirects=True, verify=should_verify(no_verify, self.get_ssl_verify()))
             return r.content
         except Exception as error:
             return False, 'Failed to get http content for %s: %s' (str(url), str(error))
 
     def get_endpoint_config(self, auth_config):
         content = self.get_http_content(auth_config['oidc_config_url'], no_verify=auth_config['no_verify'])
         endpoint_config = json.loads(content)
@@ -132,15 +150,15 @@
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
 
             result = requests.session().post(endpoint_config['device_authorization_endpoint'],
                                              # data=json.dumps(data),
                                              urlencode(data).encode(),
                                              timeout=self.timeout,
-                                             verify=should_verify(auth_config['no_verify']),
+                                             verify=should_verify(auth_config['no_verify'], self.get_ssl_verify()),
                                              headers=headers)
 
             if result is not None:
                 if result.status_code == HTTP_STATUS_CODE.OK and result.text:
                     return True, json.loads(result.text)
                 else:
                     return False, "Failed to get oidc sign in URL (status: %s, text: %s)" % (result.status_code, result.text)
@@ -177,15 +195,15 @@
             if expires_in > self.max_expires_in:
                 expires_in = self.max_expires_in
 
             result = requests.session().post(endpoint_config['token_endpoint'],
                                              # data=json.dumps(data),
                                              urlencode(data).encode(),
                                              timeout=self.timeout,
-                                             verify=should_verify(auth_config['no_verify']),
+                                             verify=should_verify(auth_config['no_verify'], self.get_ssl_verify()),
                                              headers=headers)
             if result is not None:
                 if result.status_code == HTTP_STATUS_CODE.OK and result.text:
                     return True, json.loads(result.text)
                 else:
                     return False, json.loads(result.text)
             else:
@@ -209,15 +227,15 @@
 
             headers = {'content-type': 'application/x-www-form-urlencoded'}
 
             result = requests.session().post(endpoint_config['token_endpoint'],
                                              # data=json.dumps(data),
                                              urlencode(data).encode(),
                                              timeout=self.timeout,
-                                             verify=should_verify(auth_config['no_verify']),
+                                             verify=should_verify(auth_config['no_verify'], self.get_ssl_verify()),
                                              headers=headers)
 
             if result is not None:
                 if result.status_code == HTTP_STATUS_CODE.OK and result.text:
                     return True, json.loads(result.text)
                 else:
                     return False, "Failed to refresh oidc token (status: %s, text: %s)" % (result.status_code, result.text)
@@ -230,15 +248,15 @@
 
     def get_public_key(self, token, jwks_uri, no_verify=False):
         headers = jwt.get_unverified_header(token)
         if headers is None or 'kid' not in headers:
             raise jwt.exceptions.InvalidTokenError('cannot extract kid from headers')
         kid = headers['kid']
 
-        jwks_content = self.get_http_content(jwks_uri)
+        jwks_content = self.get_http_content(jwks_uri, no_verify=no_verify)
         jwks = json.loads(jwks_content)
         jwk = None
         for j in jwks.get('keys', []):
             if j.get('kid') == kid:
                 jwk = j
         if jwk is None:
             raise jwt.exceptions.InvalidTokenError('JWK not found for kid={0}: {1}'.format(kid, str(jwks)))
```

### Comparing `idds-common-1.2.5/lib/idds/common/cache.py` & `idds-common-1.2.8/lib/idds/common/cache.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/config.py` & `idds-common-1.2.8/lib/idds/common/config.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/constants.py` & `idds-common-1.2.8/lib/idds/common/constants.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/dict_class.py` & `idds-common-1.2.8/lib/idds/common/dict_class.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/event.py` & `idds-common-1.2.8/lib/idds/common/event.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/exceptions.py` & `idds-common-1.2.8/lib/idds/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/plugin/plugin_base.py` & `idds-common-1.2.8/lib/idds/common/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/plugin/plugin_utils.py` & `idds-common-1.2.8/lib/idds/common/plugin/plugin_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/status_utils.py` & `idds-common-1.2.8/lib/idds/common/status_utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds/common/utils.py` & `idds-common-1.2.8/lib/idds/common/utils.py`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/lib/idds_common.egg-info/PKG-INFO` & `idds-common-1.2.8/lib/idds_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-common
-Version: 1.2.5
+Version: 1.2.8
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-common-1.2.5/lib/idds_common.egg-info/SOURCES.txt` & `idds-common-1.2.8/lib/idds_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-common-1.2.5/setup.py` & `idds-common-1.2.8/setup.py`

 * *Files identical despite different names*

