# Comparing `tmp/absl_extra-0.0.4.tar.gz` & `tmp/absl_extra-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.4.tar", last modified: Fri Apr 28 18:05:13 2023, max compression
+gzip compressed data, was "absl_extra-0.0.5.tar", last modified: Sat Apr 29 00:40:11 2023, max compression
```

## Comparing `absl_extra-0.0.4.tar` & `absl_extra-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1266 2023-04-28 18:05:05.808629 absl_extra-0.0.4/Readme.md
--rw-r--r--   0        0        0     5463 2023-04-28 18:05:05.808629 absl_extra-0.0.4/absl_extra.py
--rw-r--r--   0        0        0     6066 2023-04-28 18:05:05.808629 absl_extra-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 absl_extra-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1266 2023-04-29 00:39:56.816630 absl_extra-0.0.5/Readme.md
+-rw-r--r--   0        0        0     5481 2023-04-29 00:39:56.816630 absl_extra-0.0.5/absl_extra.py
+-rw-r--r--   0        0        0     6066 2023-04-29 00:39:56.816630 absl_extra-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 absl_extra-0.0.5/PKG-INFO
```

### Comparing `absl_extra-0.0.4/Readme.md` & `absl_extra-0.0.5/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.4/absl_extra.py` & `absl_extra-0.0.5/absl_extra.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 class ExceptionHandlerImpl(app.ExceptionHandler):
     def __init__(self, cmd: str, notifier: Notifier):
         self.cmd = cmd
         self.notifier = notifier
 
     def handle(self, exc: Exception):
         self.notifier.notify_job_failed(self.cmd, exc)
+        raise exc
 
 
 def hook_main(
     main: Callable,
     app_name: str | None = None,
     notifier: Notifier | None = None,
     config_file: str | None = None,
```

### Comparing `absl_extra-0.0.4/pyproject.toml` & `absl_extra-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "absl_extra"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "0.0.4"  # Required
+version = "0.0.5"  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "A wrapper to run and monitor absl app."  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `absl_extra-0.0.4/PKG-INFO` & `absl_extra-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.4
+Version: 0.0.5
 Summary: A wrapper to run and monitor absl app.
 Keywords: 
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

