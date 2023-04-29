# Comparing `tmp/jinja2_inflection-0.1.3.tar.gz` & `tmp/jinja2_inflection-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_inflection-0.1.3.tar", last modified: Wed Apr 26 17:37:34 2023, max compression
+gzip compressed data, was "jinja2_inflection-0.1.4.tar", last modified: Sat Apr 29 17:50:51 2023, max compression
```

## Comparing `jinja2_inflection-0.1.3.tar` & `jinja2_inflection-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       57 2023-04-26 17:35:55.976076 jinja2_inflection-0.1.3/README.md
--rw-r--r--   0        0        0     1100 2023-04-26 17:36:02.707150 jinja2_inflection-0.1.3/jinja2_inflection/__init__.py
--rw-r--r--   0        0        0      877 2023-04-26 17:37:34.519737 jinja2_inflection-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 jinja2_inflection-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-04-26 17:35:55.976076 jinja2_inflection-0.1.4/README.md
+-rw-r--r--   0        0        0     1119 2023-04-29 17:50:06.906677 jinja2_inflection-0.1.4/jinja2_inflection/__init__.py
+-rw-r--r--   0        0        0      877 2023-04-29 17:50:51.070519 jinja2_inflection-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      318 1970-01-01 00:00:00.000000 jinja2_inflection-0.1.4/PKG-INFO
```

### Comparing `jinja2_inflection-0.1.3/jinja2_inflection/__init__.py` & `jinja2_inflection-0.1.4/jinja2_inflection/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from inflection import singularize
 from inflection import tableize
 from inflection import titleize
 from inflection import transliterate
 from inflection import underscore
 
 from jinja2.ext import Extension
+from jinja2 import Environment
 
 
 class InflectionExtension(Extension):
-    def __init__(self, environment) -> None:
-        super(InflectionExtension, self).__init__(environment)
+    def __init__(self, environment: Environment) -> None:
+        super().__init__(environment)
         inflection_filters = dict(
             camelize=camelize,
             dasherize=dasherize,
             humanize_inflection=humanize,
             ordinal=ordinal,
             ordinalize=ordinalize,
             parameterize=parameterize,
```

### Comparing `jinja2_inflection-0.1.3/pyproject.toml` & `jinja2_inflection-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 [tool.pytype]
 inputs = [
     "package_name",
 ]
 
 [project]
 name = "jinja2-inflection"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 dependencies = [
     "inflection>=0.5.1",
     "jinja2>=3.1.2",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
```

