# Comparing `tmp/pydantic_view-0.1.2.tar.gz` & `tmp/pydantic_view-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_view-0.1.2.tar", max compression
+gzip compressed data, was "pydantic_view-0.1.3.tar", max compression
```

## Comparing `pydantic_view-0.1.2.tar` & `pydantic_view-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.1.2/LICENSE
--rw-r--r--   0        0        0     5625 2023-04-28 19:14:58.000000 pydantic_view-0.1.2/README.md
--rw-r--r--   0        0        0      142 2023-04-28 16:02:37.000000 pydantic_view-0.1.2/pydantic_view/__init__.py
--rw-r--r--   0        0        0     4842 2023-04-28 19:02:19.000000 pydantic_view-0.1.2/pydantic_view/pydantic_view.py
--rw-r--r--   0        0        0      872 2023-04-28 19:19:55.000000 pydantic_view-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 pydantic_view-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-22 16:35:00.000000 pydantic_view-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5625 2023-04-28 19:14:58.000000 pydantic_view-0.1.3/README.md
+-rw-r--r--   0        0        0      142 2023-04-28 16:02:37.000000 pydantic_view-0.1.3/pydantic_view/__init__.py
+-rw-r--r--   0        0        0     4867 2023-04-28 21:54:10.000000 pydantic_view-0.1.3/pydantic_view/pydantic_view.py
+-rw-r--r--   0        0        0      872 2023-04-28 22:11:40.000000 pydantic_view-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 pydantic_view-0.1.3/PKG-INFO
```

### Comparing `pydantic_view-0.1.2/LICENSE` & `pydantic_view-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.1.2/README.md` & `pydantic_view-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_view-0.1.2/pydantic_view/pydantic_view.py` & `pydantic_view-0.1.3/pydantic_view/pydantic_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
                 field.default_factory = v.default_factory
 
         if recursive is True:
 
             def update_type(tp):
                 if isinstance(tp, _GenericAlias):
                     tp.__args__ = tuple(update_type(arg) for arg in tp.__args__)
-                elif issubclass(tp, BaseModel) and hasattr(tp, name):
+                elif isinstance(tp, type) and issubclass(tp, BaseModel) and hasattr(tp, name):
                     tp = getattr(tp, name)
                 return tp
 
             for k, v in fields.items():
                 if v.sub_fields:
                     for sub_field in v.sub_fields:
                         sub_field.type_ = update_type(sub_field.type_)
```

### Comparing `pydantic_view-0.1.2/pyproject.toml` & `pydantic_view-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-view"
-version = "0.1.2"
+version = "0.1.3"
 description = "View decorator to create the child pydantic models from the root model."
 authors = ["Roman Koshel <roma.koshel@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["pydantic", "model", "view", "utils"]
 packages = [{include = "pydantic_view"}]
 classifiers = [
```

### Comparing `pydantic_view-0.1.2/PKG-INFO` & `pydantic_view-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-view
-Version: 0.1.2
+Version: 0.1.3
 Summary: View decorator to create the child pydantic models from the root model.
 License: MIT
 Keywords: pydantic,model,view,utils
 Author: Roman Koshel
 Author-email: roma.koshel@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

