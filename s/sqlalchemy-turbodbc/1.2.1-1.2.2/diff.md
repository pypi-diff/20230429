# Comparing `tmp/sqlalchemy_turbodbc-1.2.1.tar.gz` & `tmp/sqlalchemy_turbodbc-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlalchemy_turbodbc-1.2.1.tar", last modified: Wed Mar 15 16:38:40 2023, max compression
+gzip compressed data, was "sqlalchemy_turbodbc-1.2.2.tar", last modified: Sat Apr 29 15:28:14 2023, max compression
```

## Comparing `sqlalchemy_turbodbc-1.2.1.tar` & `sqlalchemy_turbodbc-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-03-15 16:38:40.241403 sqlalchemy_turbodbc-1.2.1/
--rw-r--r--   0 chen       (502) staff       (20)     1323 2023-03-15 16:38:40.241596 sqlalchemy_turbodbc-1.2.1/PKG-INFO
--rw-r--r--   0 chen       (502) staff       (20)     1517 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.1/README.md
--rw-r--r--   0 chen       (502) staff       (20)      136 2023-03-15 16:38:40.242307 sqlalchemy_turbodbc-1.2.1/setup.cfg
--rw-r--r--   0 chen       (502) staff       (20)     1779 2023-03-15 16:38:34.000000 sqlalchemy_turbodbc-1.2.1/setup.py
-drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-03-15 16:38:40.237269 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc/
--rw-r--r--   0 chen       (502) staff       (20)        0 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc/__init__.py
--rw-r--r--   0 chen       (502) staff       (20)     4541 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc/connector.py
--rw-r--r--   0 chen       (502) staff       (20)     3974 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc/dialect.py
-drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-03-15 16:38:40.239850 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/
--rw-r--r--   0 chen       (502) staff       (20)     1323 2023-03-15 16:38:40.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/PKG-INFO
--rw-r--r--   0 chen       (502) staff       (20)      426 2023-03-15 16:38:40.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/SOURCES.txt
--rw-r--r--   0 chen       (502) staff       (20)        1 2023-03-15 16:38:40.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/dependency_links.txt
--rw-r--r--   0 chen       (502) staff       (20)       87 2023-03-15 16:38:40.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/entry_points.txt
--rw-r--r--   0 chen       (502) staff       (20)       27 2023-03-15 16:38:40.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/requires.txt
--rw-r--r--   0 chen       (502) staff       (20)       20 2023-03-15 16:38:40.000000 sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/top_level.txt
-drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-03-15 16:38:40.240595 sqlalchemy_turbodbc-1.2.1/test/
--rw-r--r--   0 chen       (502) staff       (20)     1789 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.1/test/test_connect.py
--rw-r--r--   0 chen       (502) staff       (20)     1232 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.1/test/test_unicode.py
+drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-04-29 15:28:14.028132 sqlalchemy_turbodbc-1.2.2/
+-rw-r--r--   0 chen       (502) staff       (20)       35 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/AUTHORS
+-rw-r--r--   0 chen       (502) staff       (20)     1068 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/LICENSE
+-rw-r--r--   0 chen       (502) staff       (20)     1216 2023-04-29 15:28:14.028251 sqlalchemy_turbodbc-1.2.2/PKG-INFO
+-rw-r--r--   0 chen       (502) staff       (20)     1517 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/README.md
+-rw-r--r--   0 chen       (502) staff       (20)      136 2023-04-29 15:28:14.028924 sqlalchemy_turbodbc-1.2.2/setup.cfg
+-rw-r--r--   0 chen       (502) staff       (20)     1779 2023-04-29 15:27:48.000000 sqlalchemy_turbodbc-1.2.2/setup.py
+drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-04-29 15:28:14.024284 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc/
+-rw-r--r--   0 chen       (502) staff       (20)        0 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc/__init__.py
+-rw-r--r--   0 chen       (502) staff       (20)     4616 2023-04-29 15:25:52.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc/connector.py
+-rw-r--r--   0 chen       (502) staff       (20)     3974 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc/dialect.py
+drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-04-29 15:28:14.026827 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/
+-rw-r--r--   0 chen       (502) staff       (20)     1216 2023-04-29 15:28:13.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/PKG-INFO
+-rw-r--r--   0 chen       (502) staff       (20)      442 2023-04-29 15:28:13.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/SOURCES.txt
+-rw-r--r--   0 chen       (502) staff       (20)        1 2023-04-29 15:28:13.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/dependency_links.txt
+-rw-r--r--   0 chen       (502) staff       (20)       86 2023-04-29 15:28:13.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/entry_points.txt
+-rw-r--r--   0 chen       (502) staff       (20)       27 2023-04-29 15:28:13.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/requires.txt
+-rw-r--r--   0 chen       (502) staff       (20)       20 2023-04-29 15:28:13.000000 sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/top_level.txt
+drwxr-xr-x   0 chen       (502) staff       (20)        0 2023-04-29 15:28:14.027648 sqlalchemy_turbodbc-1.2.2/test/
+-rw-r--r--   0 chen       (502) staff       (20)     1789 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/test/test_connect.py
+-rw-r--r--   0 chen       (502) staff       (20)     1232 2023-03-15 16:35:17.000000 sqlalchemy_turbodbc-1.2.2/test/test_unicode.py
```

### Comparing `sqlalchemy_turbodbc-1.2.1/PKG-INFO` & `sqlalchemy_turbodbc-1.2.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlalchemy_turbodbc
-Version: 1.2.1
+Version: 1.2.2
 Summary: SQLAlchemy dialect for Turbodbc
 Home-page: https://github.com/dirkjonker/sqlalchemy-turbodbc
 Author: Dirk Jonker
 Author-email: dirkjonker@gmail.com
 License: MIT
-Description: 
-        # sqlalchemy-turbodbc
-        
-        SQLAlchemy connector/dialect for connecting to MS SQL Server using Turbodbc.
-        
-        This works exactly like the `mssql+pyodbc` dialect as described in the [SQLAlchemy documentation here](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
-        To create a connection using this simply use the `mssql+turbodbc` protocol.
-        
-        For example:
-        
-        ```python
-        engine = create_engine('mssql+turbodbc://scott:tiger@mydsn')
-        ```
-        
-        For more information please see the [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
-        
 Keywords: sql server sqlalchemy turbodbc mssql
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+
+# sqlalchemy-turbodbc
+
+SQLAlchemy connector/dialect for connecting to MS SQL Server using Turbodbc.
+
+This works exactly like the `mssql+pyodbc` dialect as described in the [SQLAlchemy documentation here](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
+To create a connection using this simply use the `mssql+turbodbc` protocol.
+
+For example:
+
+```python
+engine = create_engine('mssql+turbodbc://scott:tiger@mydsn')
+```
+
+For more information please see the [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
```

### Comparing `sqlalchemy_turbodbc-1.2.1/README.md` & `sqlalchemy_turbodbc-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_turbodbc-1.2.1/setup.py` & `sqlalchemy_turbodbc-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 For more information please see the [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
 """
 
 
 setup(
     name='sqlalchemy_turbodbc',
-    version='1.2.1',
+    version='1.2.2',
     description='SQLAlchemy dialect for Turbodbc',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Dirk Jonker',
     author_email='dirkjonker@gmail.com',
     url='https://github.com/dirkjonker/sqlalchemy-turbodbc',
     classifiers=[
```

### Comparing `sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc/connector.py` & `sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,12 +129,14 @@
         else:
             connect_args['trusted_connection'] = 'Yes'
 
         return [dsn, connect_args]
 
     def is_disconnect(self, e, connection, cursor):
         if isinstance(e, self.dbapi.Error):
-            return "The cursor's connection has been closed." in str(
-                e
-            ) or "Attempt to use a closed connection." in str(e)
+            return (
+                "The cursor's connection has been closed." in str(e)
+                or "Attempt to use a closed connection." in str(e)
+                or "Connection already closed" in str(e)
+            )
         else:
             return False
```

### Comparing `sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc/dialect.py` & `sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc/dialect.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_turbodbc-1.2.1/sqlalchemy_turbodbc.egg-info/PKG-INFO` & `sqlalchemy_turbodbc-1.2.2/sqlalchemy_turbodbc.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-turbodbc
-Version: 1.2.1
+Version: 1.2.2
 Summary: SQLAlchemy dialect for Turbodbc
 Home-page: https://github.com/dirkjonker/sqlalchemy-turbodbc
 Author: Dirk Jonker
 Author-email: dirkjonker@gmail.com
 License: MIT
-Description: 
-        # sqlalchemy-turbodbc
-        
-        SQLAlchemy connector/dialect for connecting to MS SQL Server using Turbodbc.
-        
-        This works exactly like the `mssql+pyodbc` dialect as described in the [SQLAlchemy documentation here](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
-        To create a connection using this simply use the `mssql+turbodbc` protocol.
-        
-        For example:
-        
-        ```python
-        engine = create_engine('mssql+turbodbc://scott:tiger@mydsn')
-        ```
-        
-        For more information please see the [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
-        
 Keywords: sql server sqlalchemy turbodbc mssql
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Database
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+
+# sqlalchemy-turbodbc
+
+SQLAlchemy connector/dialect for connecting to MS SQL Server using Turbodbc.
+
+This works exactly like the `mssql+pyodbc` dialect as described in the [SQLAlchemy documentation here](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
+To create a connection using this simply use the `mssql+turbodbc` protocol.
+
+For example:
+
+```python
+engine = create_engine('mssql+turbodbc://scott:tiger@mydsn')
+```
+
+For more information please see the [SQLAlchemy documentation](https://docs.sqlalchemy.org/en/13/dialects/mssql.html#module-sqlalchemy.dialects.mssql.pyodbc).
```

### Comparing `sqlalchemy_turbodbc-1.2.1/test/test_connect.py` & `sqlalchemy_turbodbc-1.2.2/test/test_connect.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_turbodbc-1.2.1/test/test_unicode.py` & `sqlalchemy_turbodbc-1.2.2/test/test_unicode.py`

 * *Files identical despite different names*

