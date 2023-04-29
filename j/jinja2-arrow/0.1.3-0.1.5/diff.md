# Comparing `tmp/jinja2-arrow-0.1.3.tar.gz` & `tmp/jinja2-arrow-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2-arrow-0.1.3.tar", last modified: Wed Apr 26 17:32:14 2023, max compression
+gzip compressed data, was "jinja2-arrow-0.1.5.tar", last modified: Sat Apr 29 17:47:41 2023, max compression
```

## Comparing `jinja2-arrow-0.1.3.tar` & `jinja2-arrow-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       46 2023-04-26 17:30:24.003706 jinja2-arrow-0.1.3/README.md
--rw-r--r--   0        0        0      860 2023-04-26 17:30:31.788812 jinja2-arrow-0.1.3/jinja2_arrow/__init__.py
--rw-r--r--   0        0        0      874 2023-04-26 17:31:53.932668 jinja2-arrow-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 jinja2-arrow-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       46 2023-04-26 17:30:24.003706 jinja2-arrow-0.1.5/README.md
+-rw-r--r--   0        0        0      945 2023-04-29 17:46:18.488758 jinja2-arrow-0.1.5/jinja2_arrow/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-29 17:47:33.458533 jinja2-arrow-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 jinja2-arrow-0.1.5/PKG-INFO
```

### Comparing `jinja2-arrow-0.1.3/pyproject.toml` & `jinja2-arrow-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "jinja2-arrow"
-version = "0.1.3"
+version = "0.1.5"
 description = ""
 dependencies = [
     "arrow>=1.2.3",
     "jinja2>=3.1.2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
```

