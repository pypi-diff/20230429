# Comparing `tmp/ext-mongo-0.3.0.tar.gz` & `tmp/ext-mongo-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ext-mongo-0.3.0.tar", last modified: Sat Apr 29 17:26:34 2023, max compression
+gzip compressed data, was "ext-mongo-0.4.0.tar", last modified: Sat Apr 29 17:52:56 2023, max compression
```

## Comparing `ext-mongo-0.3.0.tar` & `ext-mongo-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      395 2023-04-29 12:07:25.855827 ext-mongo-0.3.0/mongo/__init__.py
--rw-r--r--   0        0        0      453 2023-04-29 10:30:44.699476 ext-mongo-0.3.0/mongo/connect.py
--rw-r--r--   0        0        0       60 2023-04-29 10:01:06.786503 ext-mongo-0.3.0/mongo/deps.py
--rw-r--r--   0        0        0      795 2023-04-29 12:25:07.701795 ext-mongo-0.3.0/mongo/document.py
--rw-r--r--   0        0        0     1557 2023-04-29 12:41:58.626422 ext-mongo-0.3.0/mongo/document_meta.py
--rw-r--r--   0        0        0      541 2023-04-29 17:26:19.862938 ext-mongo-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1091 2023-04-29 12:44:30.408958 ext-mongo-0.3.0/README.md
--rw-r--r--   0        0        0      874 2023-04-29 12:42:46.025658 ext-mongo-0.3.0/tests/__main__.py
--rw-r--r--   0        0        0     1242 1970-01-01 00:00:00.000000 ext-mongo-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      395 2023-04-29 12:07:25.855827 ext-mongo-0.4.0/mongo/__init__.py
+-rw-r--r--   0        0        0      453 2023-04-29 10:30:44.699476 ext-mongo-0.4.0/mongo/connect.py
+-rw-r--r--   0        0        0       60 2023-04-29 10:01:06.786503 ext-mongo-0.4.0/mongo/deps.py
+-rw-r--r--   0        0        0      795 2023-04-29 12:25:07.701795 ext-mongo-0.4.0/mongo/document.py
+-rw-r--r--   0        0        0     1356 2023-04-29 17:50:25.052023 ext-mongo-0.4.0/mongo/document_meta.py
+-rw-r--r--   0        0        0      541 2023-04-29 17:52:51.106723 ext-mongo-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1057 2023-04-29 17:52:16.748800 ext-mongo-0.4.0/README.md
+-rw-r--r--   0        0        0      840 2023-04-29 17:50:55.218695 ext-mongo-0.4.0/tests/__main__.py
+-rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 ext-mongo-0.4.0/PKG-INFO
```

### Comparing `ext-mongo-0.3.0/mongo/document.py` & `ext-mongo-0.4.0/mongo/document.py`

 * *Files identical despite different names*

### Comparing `ext-mongo-0.3.0/pyproject.toml` & `ext-mongo-0.4.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "ext-mongo"
-version = "0.3.0"
+version = "0.4.0"
 description = "Extended mongoengine"
 authors = [
     { name = "levch", email = "levchenko.d.a1998@gmail.com" },
 ]
 dependencies = [
     "mongoengine>=0.27.0",
-    "parsenv>=0.1.4",
+    "parsenv>=0.2.2",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `ext-mongo-0.3.0/README.md` & `ext-mongo-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from bson import ObjectId
 
 from mongo import Document, PrimaryKey
 
 
 class Doc(Document):
-    key: PrimaryKey[int]
+    key: int | PrimaryKey
     a1: str  # Required
     a2: int | None
     a3: bool | None
     a4: float | None
     a5: ObjectId | None
     a6: datetime | None
     a7: date | None
@@ -29,15 +29,14 @@
     b2: list[int]
     b3: list[bool]
     b4: list[float]
     b5: list[ObjectId]
     b6: list[datetime]
     b7: list[date]
     c1: dict
-    c2: list[dict]
 
 
 KEY = 0
 A1 = "a1"
 
 d = Doc(key=KEY, a1=A1).save()
 
@@ -52,10 +51,9 @@
     "b2": [],
     "b3": [],
     "b4": [],
     "b5": [],
     "b6": [],
     "b7": [],
     "c1": {},
-    "c2": [],
 }
 ```
```

### Comparing `ext-mongo-0.3.0/tests/__main__.py` & `ext-mongo-0.4.0/tests/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from bson import ObjectId
 
 from mongo import Document, PrimaryKey
 
 
 class Doc(Document):
-    key: PrimaryKey[int]
+    key: int | PrimaryKey
     a1: str  # Required
     a2: int | None
     a3: bool | None
     a4: float | None
     a5: ObjectId | None
     a6: datetime | None
     a7: date | None
@@ -18,15 +18,14 @@
     b2: list[int]
     b3: list[bool]
     b4: list[float]
     b5: list[ObjectId]
     b6: list[datetime]
     b7: list[date]
     c1: dict
-    c2: list[dict]
 
 
 KEY = 0
 A1 = "a1"
 
 d = Doc(key=KEY, a1=A1).save()
 
@@ -41,9 +40,8 @@
     "b2": [],
     "b3": [],
     "b4": [],
     "b5": [],
     "b6": [],
     "b7": [],
     "c1": {},
-    "c2": [],
 }
```

### Comparing `ext-mongo-0.3.0/PKG-INFO` & `ext-mongo-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ext-mongo
-Version: 0.3.0
+Version: 0.4.0
 Summary: Extended mongoengine
 License: MIT
 Author-email: levch <levchenko.d.a1998@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 
 ### Depends on environment variables:
@@ -22,15 +22,15 @@
 
 from bson import ObjectId
 
 from mongo import Document, PrimaryKey
 
 
 class Doc(Document):
-    key: PrimaryKey[int]
+    key: int | PrimaryKey
     a1: str  # Required
     a2: int | None
     a3: bool | None
     a4: float | None
     a5: ObjectId | None
     a6: datetime | None
     a7: date | None
@@ -38,15 +38,14 @@
     b2: list[int]
     b3: list[bool]
     b4: list[float]
     b5: list[ObjectId]
     b6: list[datetime]
     b7: list[date]
     c1: dict
-    c2: list[dict]
 
 
 KEY = 0
 A1 = "a1"
 
 d = Doc(key=KEY, a1=A1).save()
 
@@ -61,11 +60,10 @@
     "b2": [],
     "b3": [],
     "b4": [],
     "b5": [],
     "b6": [],
     "b7": [],
     "c1": {},
-    "c2": [],
 }
 ```
```

