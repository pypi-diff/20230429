# Comparing `tmp/pycircleci-0.6.1.tar.gz` & `tmp/pycircleci-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycircleci-0.6.1.tar", last modified: Sat Feb  4 20:01:00 2023, max compression
+gzip compressed data, was "pycircleci-0.7.0.tar", last modified: Sat Apr 29 13:14:10 2023, max compression
```

## Comparing `pycircleci-0.6.1.tar` & `pycircleci-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-02-04 20:01:00.394485 pycircleci-0.6.1/
--rw-rw-r--   0 acazacu    (502) staff       (20)     3653 2023-02-04 20:01:00.394014 pycircleci-0.6.1/PKG-INFO
--rw-rw-r--   0 acazacu    (502) staff       (20)     2100 2023-01-30 07:14:14.000000 pycircleci-0.6.1/README.md
-drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-02-04 20:01:00.380110 pycircleci-0.6.1/pycircleci/
--rw-rw-r--   0 acazacu    (502) staff       (20)        0 2020-02-18 02:19:21.000000 pycircleci-0.6.1/pycircleci/__init__.py
--rw-rw-r--   0 acazacu    (502) staff       (20)    54520 2023-02-04 19:56:16.000000 pycircleci-0.6.1/pycircleci/api.py
--rwxrwxr-x   0 acazacu    (502) staff       (20)      784 2021-11-12 09:07:27.000000 pycircleci-0.6.1/pycircleci/console.py
-drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-02-04 20:01:00.391384 pycircleci-0.6.1/pycircleci.egg-info/
--rw-rw-r--   0 acazacu    (502) staff       (20)     3653 2023-02-04 20:01:00.000000 pycircleci-0.6.1/pycircleci.egg-info/PKG-INFO
--rw-rw-r--   0 acazacu    (502) staff       (20)      319 2023-02-04 20:01:00.000000 pycircleci-0.6.1/pycircleci.egg-info/SOURCES.txt
--rw-rw-r--   0 acazacu    (502) staff       (20)        1 2023-02-04 20:01:00.000000 pycircleci-0.6.1/pycircleci.egg-info/dependency_links.txt
--rw-rw-r--   0 acazacu    (502) staff       (20)        1 2023-02-04 20:01:00.000000 pycircleci-0.6.1/pycircleci.egg-info/not-zip-safe
--rw-rw-r--   0 acazacu    (502) staff       (20)       27 2023-02-04 20:01:00.000000 pycircleci-0.6.1/pycircleci.egg-info/requires.txt
--rw-rw-r--   0 acazacu    (502) staff       (20)       17 2023-02-04 20:01:00.000000 pycircleci-0.6.1/pycircleci.egg-info/top_level.txt
--rw-rw-r--   0 acazacu    (502) staff       (20)       38 2023-02-04 20:01:00.394668 pycircleci-0.6.1/setup.cfg
--rw-rw-r--   0 acazacu    (502) staff       (20)     1526 2023-02-04 19:56:35.000000 pycircleci-0.6.1/setup.py
-drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-02-04 20:01:00.392810 pycircleci-0.6.1/tests/
--rw-rw-r--   0 acazacu    (502) staff       (20)        0 2020-02-18 01:02:31.000000 pycircleci-0.6.1/tests/__init__.py
--rw-rw-r--   0 acazacu    (502) staff       (20)    17834 2023-02-04 19:56:16.000000 pycircleci-0.6.1/tests/test_api.py
+drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-04-29 13:14:10.520071 pycircleci-0.7.0/
+-rw-rw-r--   0 acazacu    (502) staff       (20)     3653 2023-04-29 13:14:10.505670 pycircleci-0.7.0/PKG-INFO
+-rw-rw-r--   0 acazacu    (502) staff       (20)     2100 2023-01-30 07:14:14.000000 pycircleci-0.7.0/README.md
+drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-04-29 13:14:10.500511 pycircleci-0.7.0/pycircleci/
+-rw-rw-r--   0 acazacu    (502) staff       (20)        0 2020-02-18 02:19:21.000000 pycircleci-0.7.0/pycircleci/__init__.py
+-rw-rw-r--   0 acazacu    (502) staff       (20)    55106 2023-04-29 12:57:59.000000 pycircleci-0.7.0/pycircleci/api.py
+-rwxrwxr-x   0 acazacu    (502) staff       (20)      784 2021-11-12 09:07:27.000000 pycircleci-0.7.0/pycircleci/console.py
+drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-04-29 13:14:10.503877 pycircleci-0.7.0/pycircleci.egg-info/
+-rw-rw-r--   0 acazacu    (502) staff       (20)     3653 2023-04-29 13:14:10.000000 pycircleci-0.7.0/pycircleci.egg-info/PKG-INFO
+-rw-rw-r--   0 acazacu    (502) staff       (20)      334 2023-04-29 13:14:10.000000 pycircleci-0.7.0/pycircleci.egg-info/SOURCES.txt
+-rw-rw-r--   0 acazacu    (502) staff       (20)        1 2023-04-29 13:14:10.000000 pycircleci-0.7.0/pycircleci.egg-info/dependency_links.txt
+-rw-rw-r--   0 acazacu    (502) staff       (20)        1 2023-04-29 13:14:10.000000 pycircleci-0.7.0/pycircleci.egg-info/not-zip-safe
+-rw-rw-r--   0 acazacu    (502) staff       (20)       27 2023-04-29 13:14:10.000000 pycircleci-0.7.0/pycircleci.egg-info/requires.txt
+-rw-rw-r--   0 acazacu    (502) staff       (20)       17 2023-04-29 13:14:10.000000 pycircleci-0.7.0/pycircleci.egg-info/top_level.txt
+-rw-rw-r--   0 acazacu    (502) staff       (20)       81 2023-04-29 13:09:17.000000 pycircleci-0.7.0/pyproject.toml
+-rw-rw-r--   0 acazacu    (502) staff       (20)       38 2023-04-29 13:14:10.520349 pycircleci-0.7.0/setup.cfg
+-rw-rw-r--   0 acazacu    (502) staff       (20)     1526 2023-02-04 19:56:35.000000 pycircleci-0.7.0/setup.py
+drwxrwxr-x   0 acazacu    (502) staff       (20)        0 2023-04-29 13:14:10.504946 pycircleci-0.7.0/tests/
+-rw-rw-r--   0 acazacu    (502) staff       (20)        0 2020-02-18 01:02:31.000000 pycircleci-0.7.0/tests/__init__.py
+-rw-rw-r--   0 acazacu    (502) staff       (20)    18102 2023-04-29 12:57:59.000000 pycircleci-0.7.0/tests/test_api.py
```

### Comparing `pycircleci-0.6.1/PKG-INFO` & `pycircleci-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycircleci
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python client for CircleCI API
 Home-page: https://github.com/alpinweis/pycircleci
 Author: Adrian Kazaku
 Author-email: alpinweis@gmail.com
 License: MIT
 Description: # pycircleci
```

### Comparing `pycircleci-0.6.1/README.md` & `pycircleci-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pycircleci-0.6.1/pycircleci/api.py` & `pycircleci-0.7.0/pycircleci/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1011,14 +1011,29 @@
         params = {"workflow-name": workflow_name} if workflow_name else None
 
         slug = self.project_slug(username, project, vcs_type)
         endpoint = f"insights/{slug}/branches"
         resp = self._request(GET, endpoint, params=params, api_version=API_VER_V2)
         return resp
 
+    def get_flaky_tests(self, username, project, vcs_type=GITHUB):
+        """Get a list of flaky tests for a given project.
+
+        :param username: Org or user name.
+        :param project: Repo name.
+        :param vcs_type: VCS type (github, bitbucket). Defaults to ``github``.
+
+        Endpoint:
+            GET ``/insights/:vcs-type/:username/:project/flaky-tests``
+        """
+        slug = self.project_slug(username, project, vcs_type)
+        endpoint = f"insights/{slug}/flaky-tests"
+        resp = self._request(GET, endpoint, api_version=API_VER_V2)
+        return resp
+
     def get_project_workflows_metrics(self, username, project, params=None, vcs_type=GITHUB, paginate=False, limit=None):
         """Get summary metrics for a project's workflows.
 
         :param username: Org or user name.
         :param project: Repo name.
         :param params: Optional query parameters.
         :param vcs_type: VCS type (github, bitbucket). Defaults to ``github``.
```

### Comparing `pycircleci-0.6.1/pycircleci/console.py` & `pycircleci-0.7.0/pycircleci/console.py`

 * *Files identical despite different names*

### Comparing `pycircleci-0.6.1/pycircleci.egg-info/PKG-INFO` & `pycircleci-0.7.0/pycircleci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycircleci
-Version: 0.6.1
+Version: 0.7.0
 Summary: Python client for CircleCI API
 Home-page: https://github.com/alpinweis/pycircleci
 Author: Adrian Kazaku
 Author-email: alpinweis@gmail.com
 License: MIT
 Description: # pycircleci
```

### Comparing `pycircleci-0.6.1/setup.py` & `pycircleci-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `pycircleci-0.6.1/tests/test_api.py` & `pycircleci-0.7.0/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -476,14 +476,22 @@
 
 def test_get_project_branches(cci):
     get_mock(cci, "get_project_branches_response.json")
     resp = cci.get_project_branches("foo", "bar")
     assert "master" in resp["branches"]
 
 
+def test_get_flaky_tests(cci):
+    get_mock(cci, "get_flaky_tests_response.json")
+    resp = cci.get_flaky_tests("foo", "bar")
+    assert resp["total_flaky_tests"] == 2
+    assert len(resp["flaky_tests"]) == 2
+    assert resp["flaky_tests"][0]["times_flaked"] == 10
+
+
 def test_get_project_workflows_metrics_depaginated(cci):
     get_mock(cci, "get_project_workflows_metrics_response.json")
     resp = cci.get_project_workflows_metrics("foo", "bar")
     assert "metrics" in resp[0]
     assert "duration_metrics" in resp[0]["metrics"]
```

