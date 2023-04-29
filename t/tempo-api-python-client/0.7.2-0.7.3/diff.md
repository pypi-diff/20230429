# Comparing `tmp/tempo-api-python-client-0.7.2.tar.gz` & `tmp/tempo-api-python-client-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempo-api-python-client-0.7.2.tar", last modified: Fri Apr 21 07:31:55 2023, max compression
+gzip compressed data, was "tempo-api-python-client-0.7.3.tar", last modified: Sat Apr 29 06:43:34 2023, max compression
```

## Comparing `tempo-api-python-client-0.7.2.tar` & `tempo-api-python-client-0.7.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:31:55.436619 tempo-api-python-client-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-21 07:31:55.436619 tempo-api-python-client-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-21 07:31:55.436619 tempo-api-python-client-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:31:55.432619 tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-21 07:31:55.000000 tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-21 07:31:55.000000 tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:31:55.000000 tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 07:31:55.000000 tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 07:31:55.000000 tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:31:55.432619 tempo-api-python-client-0.7.2/tempoapiclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/tempoapiclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/tempoapiclient/client_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    18825 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/tempoapiclient/client_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/tempoapiclient/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:31:55.436619 tempo-api-python-client-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/tests/test_client_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-21 07:31:39.000000 tempo-api-python-client-0.7.2/tests/test_client_v4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:43:34.532554 tempo-api-python-client-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-29 06:43:34.532554 tempo-api-python-client-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-29 06:43:34.532554 tempo-api-python-client-0.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:43:34.532554 tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-04-29 06:43:34.000000 tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-29 06:43:34.000000 tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:43:34.000000 tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 06:43:34.000000 tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 06:43:34.000000 tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:43:34.532554 tempo-api-python-client-0.7.3/tempoapiclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/tempoapiclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/tempoapiclient/client_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/tempoapiclient/client_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/tempoapiclient/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:43:34.532554 tempo-api-python-client-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/tests/test_client_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-29 06:43:21.000000 tempo-api-python-client-0.7.3/tests/test_client_v4.py
```

### Comparing `tempo-api-python-client-0.7.2/LICENSE` & `tempo-api-python-client-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tempo-api-python-client-0.7.2/PKG-INFO` & `tempo-api-python-client-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempo-api-python-client
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python bindings for Tempo (https://apidocs.tempo.io/)
 Home-page: https://github.com/stanislavulrych/tempo-api-python-client
 Author: Stanislav Ulrych
 Author-email: stanislav.ulrych@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tempo-api-python-client-0.7.2/README.md` & `tempo-api-python-client-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `tempo-api-python-client-0.7.2/setup.py` & `tempo-api-python-client-0.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tempo-api-python-client",
-    version="0.7.2",
+    version="0.7.3",
     author="Stanislav Ulrych",
     author_email="stanislav.ulrych@gmail.com",
     description="Python bindings for Tempo (https://apidocs.tempo.io/)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stanislavulrych/tempo-api-python-client",
     packages=setuptools.find_packages(exclude=('tests',)),
```

### Comparing `tempo-api-python-client-0.7.2/tempo_api_python_client.egg-info/PKG-INFO` & `tempo-api-python-client-0.7.3/tempo_api_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempo-api-python-client
-Version: 0.7.2
+Version: 0.7.3
 Summary: Python bindings for Tempo (https://apidocs.tempo.io/)
 Home-page: https://github.com/stanislavulrych/tempo-api-python-client
 Author: Stanislav Ulrych
 Author-email: stanislav.ulrych@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tempo-api-python-client-0.7.2/tempoapiclient/client_v3.py` & `tempo-api-python-client-0.7.3/tempoapiclient/client_v3.py`

 * *Files identical despite different names*

### Comparing `tempo-api-python-client-0.7.2/tempoapiclient/client_v4.py` & `tempo-api-python-client-0.7.3/tempoapiclient/client_v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,21 +328,21 @@
         url = f"/teams/{teamId}/members"
         return self.get(url)
 
     # Team - Links
     ## TBD
 
     # Team - Memberships
-    def get_team_memberships(self, membershipId):
+    def get_team_memberships(self, teamId):
         """
         Returns members.
-        :param membershipId:
+        :param teamId:
         """
 
-        url = f"/team-memberships/{membershipId}"
+        url = f"/team-memberships/team/{teamId}"
         return self.get(url)
 
     def get_account_team_membership(self, teamId, accountId):
         """
         Returns the active team membership.
         :param accountId:
         :param teamId:
```

### Comparing `tempo-api-python-client-0.7.2/tempoapiclient/rest_client.py` & `tempo-api-python-client-0.7.3/tempoapiclient/rest_client.py`

 * *Files identical despite different names*

### Comparing `tempo-api-python-client-0.7.2/tests/test_client_v3.py` & `tempo-api-python-client-0.7.3/tests/test_client_v3.py`

 * *Files identical despite different names*

### Comparing `tempo-api-python-client-0.7.2/tests/test_client_v4.py` & `tempo-api-python-client-0.7.3/tests/test_client_v4.py`

 * *Files identical despite different names*

