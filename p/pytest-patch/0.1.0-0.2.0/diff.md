# Comparing `tmp/pytest-patch-0.1.0.tar.gz` & `tmp/pytest-patch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-patch-0.1.0.tar", last modified: Tue Apr 25 23:52:45 2023, max compression
+gzip compressed data, was "pytest-patch-0.2.0.tar", last modified: Sat Apr 29 20:56:58 2023, max compression
```

## Comparing `pytest-patch-0.1.0.tar` & `pytest-patch-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 icarus    (1000) icarus    (1000)        0 2023-04-25 23:52:45.818836 pytest-patch-0.1.0/
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     1084 2023-04-16 20:55:07.000000 pytest-patch-0.1.0/LICENSE
--rw-rw-r--   0 icarus    (1000) icarus    (1000)       96 2023-04-16 20:58:17.000000 pytest-patch-0.1.0/MANIFEST.in
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     3033 2023-04-25 23:52:45.818836 pytest-patch-0.1.0/PKG-INFO
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     1803 2023-04-25 23:51:48.000000 pytest-patch-0.1.0/README.md
-drwxrwxr-x   0 icarus    (1000) icarus    (1000)        0 2023-04-25 23:52:45.818836 pytest-patch-0.1.0/pytest_patch.egg-info/
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     3033 2023-04-25 23:52:45.000000 pytest-patch-0.1.0/pytest_patch.egg-info/PKG-INFO
--rw-rw-r--   0 icarus    (1000) icarus    (1000)      391 2023-04-25 23:52:45.000000 pytest-patch-0.1.0/pytest_patch.egg-info/SOURCES.txt
--rw-rw-r--   0 icarus    (1000) icarus    (1000)        1 2023-04-25 23:52:45.000000 pytest-patch-0.1.0/pytest_patch.egg-info/dependency_links.txt
--rw-rw-r--   0 icarus    (1000) icarus    (1000)       32 2023-04-25 23:52:45.000000 pytest-patch-0.1.0/pytest_patch.egg-info/entry_points.txt
--rw-rw-r--   0 icarus    (1000) icarus    (1000)       19 2023-04-25 23:52:45.000000 pytest-patch-0.1.0/pytest_patch.egg-info/requires.txt
--rw-rw-r--   0 icarus    (1000) icarus    (1000)       37 2023-04-25 23:52:45.000000 pytest-patch-0.1.0/pytest_patch.egg-info/top_level.txt
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     3013 2023-04-21 01:35:47.000000 pytest-patch-0.1.0/pytest_patch.py
--rw-rw-r--   0 icarus    (1000) icarus    (1000)      158 2023-04-21 01:56:39.000000 pytest-patch-0.1.0/pytest_patch_testmodule.py
--rw-rw-r--   0 icarus    (1000) icarus    (1000)       38 2023-04-25 23:52:45.818836 pytest-patch-0.1.0/setup.cfg
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     1595 2023-04-25 23:51:48.000000 pytest-patch-0.1.0/setup.py
-drwxrwxr-x   0 icarus    (1000) icarus    (1000)        0 2023-04-25 23:52:45.818836 pytest-patch-0.1.0/tests/
--rw-rw-r--   0 icarus    (1000) icarus    (1000)     1430 2023-04-21 01:54:35.000000 pytest-patch-0.1.0/tests/test_patch_config.py
--rw-rw-r--   0 icarus    (1000) icarus    (1000)      271 2023-04-21 01:18:13.000000 pytest-patch-0.1.0/tests/test_pytest_patch.py
--rw-rw-r--   0 icarus    (1000) icarus    (1000)      859 2023-04-21 01:57:42.000000 pytest-patch-0.1.0/tests/test_pytest_patch_testmodule.py
+drwxrwxr-x   0 icarus    (1000) icarus    (1000)        0 2023-04-29 20:56:58.269954 pytest-patch-0.2.0/
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     1084 2023-04-16 20:55:07.000000 pytest-patch-0.2.0/LICENSE
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)       96 2023-04-16 20:58:17.000000 pytest-patch-0.2.0/MANIFEST.in
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     3108 2023-04-29 20:56:58.269954 pytest-patch-0.2.0/PKG-INFO
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     1878 2023-04-29 20:56:33.000000 pytest-patch-0.2.0/README.md
+drwxrwxr-x   0 icarus    (1000) icarus    (1000)        0 2023-04-29 20:56:58.269954 pytest-patch-0.2.0/pytest_patch.egg-info/
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     3108 2023-04-29 20:56:58.000000 pytest-patch-0.2.0/pytest_patch.egg-info/PKG-INFO
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)      364 2023-04-29 20:56:58.000000 pytest-patch-0.2.0/pytest_patch.egg-info/SOURCES.txt
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)        1 2023-04-29 20:56:58.000000 pytest-patch-0.2.0/pytest_patch.egg-info/dependency_links.txt
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)       32 2023-04-29 20:56:58.000000 pytest-patch-0.2.0/pytest_patch.egg-info/entry_points.txt
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)       19 2023-04-29 20:56:58.000000 pytest-patch-0.2.0/pytest_patch.egg-info/requires.txt
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)       13 2023-04-29 20:56:58.000000 pytest-patch-0.2.0/pytest_patch.egg-info/top_level.txt
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     3013 2023-04-29 20:11:17.000000 pytest-patch-0.2.0/pytest_patch.py
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)       38 2023-04-29 20:56:58.269954 pytest-patch-0.2.0/setup.cfg
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     1568 2023-04-29 19:38:43.000000 pytest-patch-0.2.0/setup.py
+drwxrwxr-x   0 icarus    (1000) icarus    (1000)        0 2023-04-29 20:56:58.269954 pytest-patch-0.2.0/tests/
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)     1430 2023-04-21 01:54:35.000000 pytest-patch-0.2.0/tests/test_patch_config.py
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)      271 2023-04-21 01:18:13.000000 pytest-patch-0.2.0/tests/test_pytest_patch.py
+-rw-rw-r--   0 icarus    (1000) icarus    (1000)      859 2023-04-21 01:57:42.000000 pytest-patch-0.2.0/tests/test_pytest_patch_testmodule.py
```

### Comparing `pytest-patch-0.1.0/LICENSE` & `pytest-patch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-patch-0.1.0/PKG-INFO` & `pytest-patch-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-patch
-Version: 0.1.0
+Version: 0.2.0
 Summary: An automagic `patch` fixture that can patch objects directly or by name.
 Home-page: https://github.com/megawidget/pytest-patch
 Author: Igor Kaplounenko
 Author-email: megawidget@gmail.com
 Maintainer: Igor Kaplounenko
 Maintainer-email: megawidget@gmail.com
 License: MIT
@@ -31,43 +31,39 @@
 # Pytest Patch
 
 An automagic replacement for `monkeypatch` or `unittest.mock.patch` that can be
 used on objects either directly or by name.
 
 ![tests](https://github.com/megawidget/pytest-patch/actions/workflows/python-package.yml/badge.svg)
 
-## Usage Examples
+## Usage
 
 ### patching objects directly
 
 ```
 from pytest import fixture
+from mock import MagicMock, sentinel
 
-from mymodule import callee, caller
+from mymodule import callee, caller  # `caller` returns `callee()`
 
 
 @fixture
 def callee_mock(patch):
-  return patch(callee)  # returns `MagicMock` by default
+  # returns the second argument if provided, `MagicMock()` otherwise
+  return patch(callee, MagicMock(return_value=sentinel.callee))
 
 
 def test_caller(callee_mock):
-  caller()
-  assert callee_mock.called
+  assert caller() == sentinel.callee
 ```
 
 
 ### patching objects by name
 
 ```
-from pytest import fixture
-
-from mymodule import caller
-
-
 @fixture
 def callee_mock(patch):
   return patch('callee')  # assumes `callee` is in `mymodule`
 ```
 
 
 ### patching by full path
```

### Comparing `pytest-patch-0.1.0/README.md` & `pytest-patch-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 # Pytest Patch
 
 An automagic replacement for `monkeypatch` or `unittest.mock.patch` that can be
 used on objects either directly or by name.
 
 ![tests](https://github.com/megawidget/pytest-patch/actions/workflows/python-package.yml/badge.svg)
 
-## Usage Examples
+## Usage
 
 ### patching objects directly
 
 ```
 from pytest import fixture
+from mock import MagicMock, sentinel
 
-from mymodule import callee, caller
+from mymodule import callee, caller  # `caller` returns `callee()`
 
 
 @fixture
 def callee_mock(patch):
-  return patch(callee)  # returns `MagicMock` by default
+  # returns the second argument if provided, `MagicMock()` otherwise
+  return patch(callee, MagicMock(return_value=sentinel.callee))
 
 
 def test_caller(callee_mock):
-  caller()
-  assert callee_mock.called
+  assert caller() == sentinel.callee
 ```
 
 
 ### patching objects by name
 
 ```
-from pytest import fixture
-
-from mymodule import caller
-
-
 @fixture
 def callee_mock(patch):
   return patch('callee')  # assumes `callee` is in `mymodule`
 ```
 
 
 ### patching by full path
```

### Comparing `pytest-patch-0.1.0/pytest_patch.egg-info/PKG-INFO` & `pytest-patch-0.2.0/pytest_patch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-patch
-Version: 0.1.0
+Version: 0.2.0
 Summary: An automagic `patch` fixture that can patch objects directly or by name.
 Home-page: https://github.com/megawidget/pytest-patch
 Author: Igor Kaplounenko
 Author-email: megawidget@gmail.com
 Maintainer: Igor Kaplounenko
 Maintainer-email: megawidget@gmail.com
 License: MIT
@@ -31,43 +31,39 @@
 # Pytest Patch
 
 An automagic replacement for `monkeypatch` or `unittest.mock.patch` that can be
 used on objects either directly or by name.
 
 ![tests](https://github.com/megawidget/pytest-patch/actions/workflows/python-package.yml/badge.svg)
 
-## Usage Examples
+## Usage
 
 ### patching objects directly
 
 ```
 from pytest import fixture
+from mock import MagicMock, sentinel
 
-from mymodule import callee, caller
+from mymodule import callee, caller  # `caller` returns `callee()`
 
 
 @fixture
 def callee_mock(patch):
-  return patch(callee)  # returns `MagicMock` by default
+  # returns the second argument if provided, `MagicMock()` otherwise
+  return patch(callee, MagicMock(return_value=sentinel.callee))
 
 
 def test_caller(callee_mock):
-  caller()
-  assert callee_mock.called
+  assert caller() == sentinel.callee
 ```
 
 
 ### patching objects by name
 
 ```
-from pytest import fixture
-
-from mymodule import caller
-
-
 @fixture
 def callee_mock(patch):
   return patch('callee')  # assumes `callee` is in `mymodule`
 ```
 
 
 ### patching by full path
```

### Comparing `pytest-patch-0.1.0/pytest_patch.py` & `pytest-patch-0.2.0/pytest_patch.py`

 * *Files identical despite different names*

### Comparing `pytest-patch-0.1.0/setup.py` & `pytest-patch-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 
 setup(
     name='pytest-patch',
-    version='0.1.0',
+    version='0.2.0',
     author='Igor Kaplounenko',
     author_email='megawidget@gmail.com',
     maintainer='Igor Kaplounenko',
     maintainer_email='megawidget@gmail.com',
     license='MIT',
     url='https://github.com/megawidget/pytest-patch',
     description='An automagic `patch` fixture that can patch '
                 'objects directly or by name.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    py_modules=['pytest_patch', 'pytest_patch_testmodule'],
+    py_modules=['pytest_patch'],
     python_requires='>=3.7',
     install_requires=['pytest>=7.0.0', 'mock'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
```

### Comparing `pytest-patch-0.1.0/tests/test_patch_config.py` & `pytest-patch-0.2.0/tests/test_patch_config.py`

 * *Files identical despite different names*

### Comparing `pytest-patch-0.1.0/tests/test_pytest_patch_testmodule.py` & `pytest-patch-0.2.0/tests/test_pytest_patch_testmodule.py`

 * *Files identical despite different names*

