# Comparing `tmp/ext-mongo-0.1.0.tar.gz` & `tmp/ext-mongo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext-mongo-0.1.0.tar", last modified: Sat Apr 29 12:30:32 2023, max compression
+gzip compressed data, was "ext-mongo-0.2.0.tar", last modified: Sat Apr 29 12:44:35 2023, max compression
```

## Comparing `ext-mongo-0.1.0.tar` & `ext-mongo-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      395 2023-04-29 12:07:25.855827 ext-mongo-0.1.0/mongo/__init__.py
--rw-r--r--   0        0        0      453 2023-04-29 10:30:44.699476 ext-mongo-0.1.0/mongo/connect.py
--rw-r--r--   0        0        0       60 2023-04-29 10:01:06.786503 ext-mongo-0.1.0/mongo/deps.py
--rw-r--r--   0        0        0      795 2023-04-29 12:25:07.701795 ext-mongo-0.1.0/mongo/document.py
--rw-r--r--   0        0        0     1448 2023-04-29 12:21:36.930724 ext-mongo-0.1.0/mongo/document_meta.py
--rw-r--r--   0        0        0      593 2023-04-29 12:30:24.281277 ext-mongo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1089 2023-04-29 12:28:12.878758 ext-mongo-0.1.0/README.md
--rw-r--r--   0        0        0      872 2023-04-29 12:25:27.028790 ext-mongo-0.1.0/tests/__main__.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 ext-mongo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      395 2023-04-29 12:07:25.855827 ext-mongo-0.2.0/mongo/__init__.py
+-rw-r--r--   0        0        0      453 2023-04-29 10:30:44.699476 ext-mongo-0.2.0/mongo/connect.py
+-rw-r--r--   0        0        0       60 2023-04-29 10:01:06.786503 ext-mongo-0.2.0/mongo/deps.py
+-rw-r--r--   0        0        0      795 2023-04-29 12:25:07.701795 ext-mongo-0.2.0/mongo/document.py
+-rw-r--r--   0        0        0     1557 2023-04-29 12:41:58.626422 ext-mongo-0.2.0/mongo/document_meta.py
+-rw-r--r--   0        0        0      593 2023-04-29 12:43:36.718251 ext-mongo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1091 2023-04-29 12:44:30.408958 ext-mongo-0.2.0/README.md
+-rw-r--r--   0        0        0      874 2023-04-29 12:42:46.025658 ext-mongo-0.2.0/tests/__main__.py
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 ext-mongo-0.2.0/PKG-INFO
```

### Comparing `ext-mongo-0.1.0/mongo/document.py` & `ext-mongo-0.2.0/mongo/document.py`

 * *Files identical despite different names*

### Comparing `ext-mongo-0.1.0/mongo/document_meta.py` & `ext-mongo-0.2.0/mongo/document_meta.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,18 +31,21 @@
     kwargs = {}
 
     if getattr(_type, "__origin__", None) == PrimaryKey:
         _type = getattr(_type, "__args__")[0]
         kwargs = {"primary_key": True}
 
     for t, Field in FIELD_BY_TYPE.items():
+        if _type == t and _type != dict:
+            kwargs["required"] = True
         field = Field(**kwargs)
         if _type in [t, t | None]:
             return field
         if _type == list[t]:
+            me.DictField()
             return me.ListField(field)
 
     msg = f"Can't make field `{name}` with type {repr(_type)}"
     raise ValueError(msg)
 
 
 FIELD_BY_TYPE = {
```

### Comparing `ext-mongo-0.1.0/pyproject.toml` & `ext-mongo-0.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ext-mongo"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = [
     { name = "levch", email = "levchenko.d.a1998@gmail.com" },
 ]
 dependencies = [
     "mongoengine>=0.27.0",
     "parsenv>=0.1.4",
```

### Comparing `ext-mongo-0.1.0/README.md` & `ext-mongo-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 
 from bson import ObjectId
 
 from mongo import Document, PrimaryKey
 
 
 class Doc(Document):
-    key: PrimaryKey[str]
-    a1: str | None
+    key: PrimaryKey[int]
+    a1: str  # Required
     a2: int | None
     a3: bool | None
     a4: float | None
     a5: ObjectId | None
     a6: datetime | None
     a7: date | None
     b1: list[str]
@@ -32,26 +32,26 @@
     b5: list[ObjectId]
     b6: list[datetime]
     b7: list[date]
     c1: dict
     c2: list[dict]
 
 
-KEY = "key"
+KEY = 0
 A1 = "a1"
 
 d = Doc(key=KEY, a1=A1).save()
 
 assert Doc.get(KEY) == d
 assert Doc.find(a1=A1) == d
 assert Doc.find_all(a1=A1) == [d]
-assert d.str_id == KEY
+assert d.str_id == str(KEY)
 assert d.to_dict() == {
-    "_id": "key",
-    "a1": "a1",
+    "_id": KEY,
+    "a1": A1,
     "b1": [],
     "b2": [],
     "b3": [],
     "b4": [],
     "b5": [],
     "b6": [],
     "b7": [],
```

### Comparing `ext-mongo-0.1.0/tests/__main__.py` & `ext-mongo-0.2.0/tests/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from bson import ObjectId
 
 from mongo import Document, PrimaryKey
 
 
 class Doc(Document):
-    key: PrimaryKey[str]
-    a1: str | None
+    key: PrimaryKey[int]
+    a1: str  # Required
     a2: int | None
     a3: bool | None
     a4: float | None
     a5: ObjectId | None
     a6: datetime | None
     a7: date | None
     b1: list[str]
@@ -21,26 +21,26 @@
     b5: list[ObjectId]
     b6: list[datetime]
     b7: list[date]
     c1: dict
     c2: list[dict]
 
 
-KEY = "key"
+KEY = 0
 A1 = "a1"
 
 d = Doc(key=KEY, a1=A1).save()
 
 assert Doc.get(KEY) == d
 assert Doc.find(a1=A1) == d
 assert Doc.find_all(a1=A1) == [d]
-assert d.str_id == KEY
+assert d.str_id == str(KEY)
 assert d.to_dict() == {
-    "_id": "key",
-    "a1": "a1",
+    "_id": KEY,
+    "a1": A1,
     "b1": [],
     "b2": [],
     "b3": [],
     "b4": [],
     "b5": [],
     "b6": [],
     "b7": [],
```

### Comparing `ext-mongo-0.1.0/PKG-INFO` & `ext-mongo-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext-mongo
-Version: 0.1.0
+Version: 0.2.0
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ### Depends on environment variables:
 
@@ -21,16 +21,16 @@
 
 from bson import ObjectId
 
 from mongo import Document, PrimaryKey
 
 
 class Doc(Document):
-    key: PrimaryKey[str]
-    a1: str | None
+    key: PrimaryKey[int]
+    a1: str  # Required
     a2: int | None
     a3: bool | None
     a4: float | None
     a5: ObjectId | None
     a6: datetime | None
     a7: date | None
     b1: list[str]
@@ -40,26 +40,26 @@
     b5: list[ObjectId]
     b6: list[datetime]
     b7: list[date]
     c1: dict
     c2: list[dict]
 
 
-KEY = "key"
+KEY = 0
 A1 = "a1"
 
 d = Doc(key=KEY, a1=A1).save()
 
 assert Doc.get(KEY) == d
 assert Doc.find(a1=A1) == d
 assert Doc.find_all(a1=A1) == [d]
-assert d.str_id == KEY
+assert d.str_id == str(KEY)
 assert d.to_dict() == {
-    "_id": "key",
-    "a1": "a1",
+    "_id": KEY,
+    "a1": A1,
     "b1": [],
     "b2": [],
     "b3": [],
     "b4": [],
     "b5": [],
     "b6": [],
     "b7": [],
```

