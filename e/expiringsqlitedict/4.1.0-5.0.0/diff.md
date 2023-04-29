# Comparing `tmp/expiringsqlitedict-4.1.0.tar.gz` & `tmp/expiringsqlitedict-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expiringsqlitedict-4.1.0.tar", last modified: Thu Mar  2 01:46:06 2023, max compression
+gzip compressed data, was "expiringsqlitedict-5.0.0.tar", last modified: Sat Apr 29 13:13:00 2023, max compression
```

## Comparing `expiringsqlitedict-4.1.0.tar` & `expiringsqlitedict-5.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-4.1.0/.gitignore
--rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-4.1.0/.travis.yml
--rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-4.1.0/CHANGELOG.txt
--rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-4.1.0/LICENSE.apache
--rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-4.1.0/LICENSE.rst
--rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-4.1.0/Makefile
--rw-r--r--   0        0        0     3954 2022-07-01 21:44:56.963135 expiringsqlitedict-4.1.0/README.rst
--rwxr-xr-x   0        0        0      998 2023-01-17 18:22:36.894147 expiringsqlitedict-4.1.0/bench.py
--rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-4.1.0/docs/Makefile
--rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-4.1.0/docs/conf.py
--rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-4.1.0/docs/expiringsqlitedict.rst
--rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-4.1.0/docs/index.rst
--rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-4.1.0/docs/make.bat
--rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-4.1.0/docs/requirements.txt
--rw-r--r--   0        0        0      974 2023-03-02 01:42:41.930488 expiringsqlitedict-4.1.0/pyproject.toml
--rwxr-xr-x   0        0        0      315 2023-01-17 00:37:57.218823 expiringsqlitedict-4.1.0/run_all_tests.sh
--rwxr-xr-x   0        0        0    11187 2023-03-02 01:42:31.314481 expiringsqlitedict-4.1.0/src/expiringsqlitedict/__init__.py
--rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-4.1.0/src/expiringsqlitedict/py.typed
--rwxr-xr-x   0        0        0     6196 2023-03-02 01:45:10.197592 expiringsqlitedict-4.1.0/test.py
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 expiringsqlitedict-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0      249 2023-01-17 17:32:50.440949 expiringsqlitedict-5.0.0/.gitignore
+-rw-r--r--   0        0        0      271 2018-06-07 21:48:55.951133 expiringsqlitedict-5.0.0/.travis.yml
+-rw-r--r--   0        0        0     1900 2022-07-01 21:27:31.727826 expiringsqlitedict-5.0.0/CHANGELOG.txt
+-rw-r--r--   0        0        0    11401 2021-06-14 18:49:24.994306 expiringsqlitedict-5.0.0/LICENSE.apache
+-rw-r--r--   0        0        0      193 2021-06-14 18:49:22.590300 expiringsqlitedict-5.0.0/LICENSE.rst
+-rw-r--r--   0        0        0       52 2021-10-13 21:06:48.260857 expiringsqlitedict-5.0.0/Makefile
+-rw-r--r--   0        0        0     4042 2023-04-29 13:08:40.273027 expiringsqlitedict-5.0.0/README.rst
+-rwxr-xr-x   0        0        0      988 2023-04-29 13:08:50.374197 expiringsqlitedict-5.0.0/bench.py
+-rw-r--r--   0        0        0      634 2023-01-17 00:40:43.681234 expiringsqlitedict-5.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2302 2023-01-17 00:42:16.953463 expiringsqlitedict-5.0.0/docs/conf.py
+-rw-r--r--   0        0        0       87 2023-01-17 00:44:05.124729 expiringsqlitedict-5.0.0/docs/expiringsqlitedict.rst
+-rw-r--r--   0        0        0      520 2023-01-17 00:47:24.429206 expiringsqlitedict-5.0.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-01-17 00:40:43.682233 expiringsqlitedict-5.0.0/docs/make.bat
+-rw-r--r--   0        0        0       40 2023-01-17 00:43:04.237580 expiringsqlitedict-5.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0      972 2023-04-29 13:00:17.351526 expiringsqlitedict-5.0.0/pyproject.toml
+-rwxr-xr-x   0        0        0      415 2023-04-29 12:33:42.701348 expiringsqlitedict-5.0.0/run_all_tests.sh
+-rwxr-xr-x   0        0        0    10897 2023-04-29 13:12:01.647417 expiringsqlitedict-5.0.0/src/expiringsqlitedict/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-17 00:39:05.082991 expiringsqlitedict-5.0.0/src/expiringsqlitedict/py.typed
+-rwxr-xr-x   0        0        0     7186 2023-04-29 13:11:14.086617 expiringsqlitedict-5.0.0/test.py
+-rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 expiringsqlitedict-5.0.0/PKG-INFO
```

### Comparing `expiringsqlitedict-4.1.0/CHANGELOG.txt` & `expiringsqlitedict-5.0.0/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-4.1.0/LICENSE.apache` & `expiringsqlitedict-5.0.0/LICENSE.apache`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-4.1.0/README.rst` & `expiringsqlitedict-5.0.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -41,16 +41,18 @@
 
 * Values can be any json-capable objects (this can be customized to be as
   flexible as you need, through custom serializers)
 * Support for access from multiple programs or threads, with locking fully
   managed by sqlite itself.
 * A very simple codebase that is easy to read, relying on sqlite for as much
   behavior as possible.
-* A simple autocommit wrapper (``AutocommitSqliteDict``), if you really can't
+* A simple autocommit wrapper (``SimpleSqliteDict``), if you really can't
   handle a context manager and need something that fully handles like a dict.
+  You can specify a ``isolation_level`` on this to have to commit and roll back
+  yourself.
 * An on-demand wrapper (``OnDemand``), for situations where you want to open and
   close the database in as narrow a window as possible.
 * Support for custom serialization or compression:
 
 .. code-block:: python
 
   import json
```

### Comparing `expiringsqlitedict-4.1.0/bench.py` & `expiringsqlitedict-5.0.0/bench.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from datetime import timedelta
 import random
 import string
 from timeit import Timer
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from expiringsqlitedict import SqliteDict
-import gc
 population = string.ascii_letters + string.digits + string.punctuation
 
 with TemporaryDirectory() as dir:
     db_file = Path(dir) / 'test.db'
 
     def test():
         with SqliteDict(str(db_file), lifespan=timedelta(seconds=1)) as db:
```

### Comparing `expiringsqlitedict-4.1.0/docs/Makefile` & `expiringsqlitedict-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-4.1.0/docs/conf.py` & `expiringsqlitedict-5.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-4.1.0/docs/index.rst` & `expiringsqlitedict-5.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-4.1.0/docs/make.bat` & `expiringsqlitedict-5.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `expiringsqlitedict-4.1.0/pyproject.toml` & `expiringsqlitedict-5.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = 'expiringsqlitedict'
-description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and pickle'
-version = '4.1.0'
+description = 'Persistent compressed expiring dict in Python, backed up by sqlite3 and json'
+version = '5.0.0'
 readme = 'README.rst'
 requires-python = '>= 3.6, < 4'
 license = { text = 'Apache 2.0' }
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `expiringsqlitedict-4.1.0/src/expiringsqlitedict/__init__.py` & `expiringsqlitedict-5.0.0/src/expiringsqlitedict/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,57 +8,20 @@
 #
 # This code was inspired by:
 #  * http://code.activestate.com/recipes/576638-draft-for-an-sqlite3-based-dbm/
 #  * http://code.activestate.com/recipes/526618/
 
 
 import json
-import pickle
 import sqlite3
-import zlib
 from collections.abc import MutableMapping
-from contextlib import closing, contextmanager
+from contextlib import closing
 from datetime import timedelta
-from typing import Any, Iterator, Tuple
+from typing import Any, Iterator, Optional, Tuple, Type
 from weakref import finalize
-from functools import wraps
-
-class ZlibPickleSerializer:
-    '''Serializer that pickles and optionally zlib-compresses data.
-    '''
-
-    __slots__ = ()
-
-    @staticmethod
-    def dumps(value: Any) -> bytes:
-        """Serialize an object using pickle to a binary format accepted by SQLite."""
-
-        pickled = pickle.dumps(value)
-        compressed = zlib.compress(pickled)
-
-        # If compression didn't fail to save space:
-        if len(compressed) < len(pickled):
-            data = b'Z' + compressed
-        else:
-            data = b'R' + pickled
-
-        return data
-
-    @staticmethod
-    def loads(data: bytes) -> Any:
-        """Deserialize objects retrieved from SQLite."""
-        flag = data[0:1]
-        data = data[1:]
-
-        if flag == b'Z':
-            pickled = zlib.decompress(data)
-        else:
-            pickled = data
-
-        return pickle.loads(pickled)
 
 def _close(db):
     '''Optimize and close the database.
     '''
     with closing(db) as d, closing(d.cursor()) as cursor:
         cursor.execute('PRAGMA analysis_limit=8192')
         cursor.execute('PRAGMA optimize')
@@ -66,43 +29,44 @@
 class SqliteDict:
     """
     Set up the sqlite dictionary manager.
 
     This needs to be used as a context manager.  It will not operate at all
     otherwise. args and kwargs are directly passed to sqlite3.connect.  Use
     these to customize your connection, such as making it read-only.
+
+    This is lazy, and won't even open the database until it is entered.  It may
+    be re-opened after it has closed.
     """
 
     __slots__ = (
-        '_db',
+        '_args',
+        '_kwargs',
+        '_connection',
         '_serializer',
         '_lifespan',
         '_begin',
         '_table',
-        '_finalizer',
         '__weakref__'
     )
 
     def __init__(self,
         *args,
         serializer: Any = json,
         lifespan: timedelta = timedelta(weeks=1),
         transaction: str = 'IMMEDIATE',
         table: str = 'expiringsqlitedict',
         **kwargs,
     ) -> None:
-        self._db = sqlite3.connect(*args, isolation_level=None, **kwargs)
-        with closing(self._db.cursor()) as cursor:
-            cursor.execute('PRAGMA journal_mode=WAL')
-            cursor.execute('PRAGMA synchronous=NORMAL')
+        self._args = args
+        self._kwargs = kwargs
         self._serializer = serializer
         self._lifespan = lifespan
         self._begin = f'BEGIN {transaction} TRANSACTION'
         self._table = table
-        self._finalizer = finalize(self, _close, self._db)
 
     @property
     def lifespan(self) -> timedelta:
         '''The current lifespan.
 
         Changing this will change the calculated expiration time of future set
         items.  It will not retroactively apply to existing items unless you explicitly
@@ -111,59 +75,62 @@
         return self._lifespan
 
     @lifespan.setter
     def lifespan(self, value: timedelta) -> None:
         self._lifespan = value
 
     def __enter__(self) -> 'Connection':
-        with closing(self._db.cursor()) as cursor:
+        self._connection = sqlite3.connect(
+            *self._args,
+            isolation_level=None,
+            **self._kwargs,
+        )
+        with closing(self._connection.cursor()) as cursor:
+            cursor.execute('PRAGMA journal_mode=WAL')
+            cursor.execute('PRAGMA synchronous=NORMAL')
             cursor.execute(self._begin)
 
         return Connection(
-            self._db,
+            self._connection,
             serializer=self._serializer,
             lifespan=self._lifespan,
             table=self._table,
         )
 
-    def __exit__(self, type, value, traceback) -> None:
-        if (type and value and traceback) is None:
-            with closing(self._db.cursor()) as cursor:
+    def __exit__(
+        self,
+        type: Optional[Type[BaseException]],
+        value: Optional[BaseException],
+        traceback: Optional[BaseException],
+    ) -> None:
+        with closing(self._connection) as db, closing(db.cursor()) as cursor:
+            if (type and value and traceback) is None:
                 cursor.execute('COMMIT')
-        else:
-            with closing(self._db.cursor()) as cursor:
+            else:
                 cursor.execute('ROLLBACK')
 
-    def close(self):
-        '''Close and optimize the database.'''
-
-        self._finalizer()
-
-@wraps(SqliteDict)
-@contextmanager
-def OnDemand(*args, **kwargs):
-    '''A wrapper around a database that is a context-manager that opens the
-    database on-demand and closes it immediately when finished with it.
-    '''
-    manager = SqliteDict(*args, **kwargs)
-    with closing(manager), manager as connection:
-        yield connection
+            cursor.execute('PRAGMA analysis_limit=8192')
+            cursor.execute('PRAGMA optimize')
 
-def AutocommitSqliteDict(
+def SimpleSqliteDict(
     *args,
     serializer: Any = json,
     lifespan: timedelta = timedelta(weeks=1),
+    isolation_level: Optional[str] = None,
     table: str = 'expiringsqlitedict',
     **kwargs,
 ) -> 'Connection':
     """
-    Set up the sqlite dictionary manager as a non-contextmanager in autocommit mode.
+    Set up the sqlite dictionary manager as a non-contextmanager with a finalizer.
+
+    If you set the isolation_level, you will be responsible for calling
+    d.connection.commit() and d.connection.rollback() appropriately.
     """
 
-    db = sqlite3.connect(*args, isolation_level=None, **kwargs)
+    db = sqlite3.connect(*args, isolation_level=isolation_level, **kwargs)
     with closing(db.cursor()) as cursor:
         cursor.execute('PRAGMA journal_mode=WAL')
         cursor.execute('PRAGMA synchronous=NORMAL')
 
     connection = Connection(
         db,
         serializer=serializer,
@@ -171,14 +138,30 @@
         table=table,
     )
 
     finalize(connection, _close, db)
 
     return connection
 
+if sqlite3.sqlite_version_info >= (3, 8, 2):
+    _create_table_trailer = ' WITHOUT ROWID'
+else:
+    _create_table_trailer = ''
+
+if sqlite3.sqlite_version_info >= (3, 37):
+    _create_table_trailer += ' STRICT'
+    _valuetype = 'ANY' 
+else:
+    _valuetype = 'BLOB' 
+
+if sqlite3.sqlite_version_info >= (3, 38):
+    _unixepoch = 'UNIXEPOCH()'
+else:
+    _unixepoch = "CAST(strftime('%s', 'now') AS INTEGER)"
+
 class Connection(MutableMapping):
     '''The actual connection object, as a MutableMapping[str, Any].
 
     Items are expired when a value is inserted or updated.  Deletion or
     postponement does not expire items.
     '''
 
@@ -204,41 +187,45 @@
         self._safe_table = table.replace('"', '""')
 
         with closing(self._connection.cursor()) as cursor:
             create_statement = f'''
             CREATE TABLE IF NOT EXISTS "{self._safe_table}" (
                 key TEXT PRIMARY KEY NOT NULL,
                 expire INTEGER NOT NULL,
-                value BLOB NOT NULL)'''
+                value {_valuetype} NOT NULL){_create_table_trailer}'''
 
-            if sqlite3.sqlite_version_info >= (3, 8, 2):
-                create_statement += ' WITHOUT ROWID'
 
             cursor.execute(create_statement)
             cursor.execute(
-                f'CREATE INDEX IF NOT EXISTS "{self._safe_table}_expire_index" ON "{self._safe_table}" (expire)'
+                f'CREATE INDEX IF NOT EXISTS "{self._safe_table}_expire_index"'
+                f' ON "{self._safe_table}" (expire)'
             )
 
             cursor.execute(
                 f'''
-                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_insert_trigger" AFTER INSERT ON "{self._safe_table}"
+                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_insert_trigger"'''
+                f''' AFTER INSERT ON "{self._safe_table}"
                 BEGIN
-                    DELETE FROM "{self._safe_table}" WHERE expire <= strftime('%s', 'now');
+                    DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
                 END
                 '''
             )
 
             cursor.execute(
                 f'''
-                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_update_trigger" AFTER UPDATE OF value ON "{self._safe_table}"
+                CREATE TRIGGER IF NOT EXISTS "{self._safe_table}_update_trigger"'''
+                f''' AFTER UPDATE OF value ON "{self._safe_table}"
                 BEGIN
-                    DELETE FROM "{self._safe_table}" WHERE expire <= strftime('%s', 'now');
+                    DELETE FROM "{self._safe_table}" WHERE expire <= {_unixepoch};
                 END
                 '''
             )
+    @property
+    def connection(self) -> sqlite3.Connection:
+        return self._connection
 
     @property
     def lifespan(self) -> timedelta:
         '''The current lifespan.
 
         Changing this will change the calculated expiration time of future set
         items.  It will not retroactively apply to existing items unless you explicitly
@@ -291,15 +278,18 @@
                 yield row[0], self._serializer.loads(row[1])
 
     def __contains__(self, key: str) -> bool:
         '''Check if the table contains the given key.
         '''
 
         with closing(self._connection.cursor()) as cursor:
-            for _ in cursor.execute(f'SELECT 1 FROM "{self._safe_table}" WHERE key = ?', (key,)):
+            for _ in cursor.execute(
+                f'SELECT 1 FROM "{self._safe_table}" WHERE key = ?',
+                (key,),
+            ):
                 return True
         return False
 
     def __getitem__(self, key: str) -> Any:
         '''Fetch the key.
         '''
 
@@ -314,15 +304,16 @@
         '''Set or replace the item.
 
         This also triggers cleaning up expired values.
         '''
 
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(
-                f'REPLACE INTO "{self._safe_table}"' " (key, expire, value) VALUES (?, strftime('%s', 'now') + ?, ?)",
+                f'REPLACE INTO "{self._safe_table}" (key, expire, value)'
+                f'VALUES (?, {_unixepoch} + ?, ?)',
                 (key, self._lifespan, self._serializer.dumps(value)),
                 )
 
     def __delitem__(self, key: str) -> None:
         '''Delete an item from the table.
         '''
 
@@ -339,19 +330,19 @@
             cursor.execute(f'DELETE FROM "{self._safe_table}"')
 
     def postpone(self, key: str) -> None:
         '''Push back the expiration date of the given entry, if it exists.
         '''
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(
-                f'UPDATE "{self._safe_table}"' " SET expire=strftime('%s', 'now') + ? WHERE key=?",
+                f'UPDATE "{self._safe_table}" SET expire={_unixepoch} + ? WHERE key=?',
                 (self._lifespan, key),
             )
 
     def postpone_all(self) -> None:
         '''Push back the expiration date of all entries at once.
         '''
         with closing(self._connection.cursor()) as cursor:
             cursor.execute(
-                f'UPDATE "{self._safe_table}"' " SET expire=strftime('%s', 'now') + ?",
+                f'UPDATE "{self._safe_table}" SET expire={_unixepoch} + ?',
                 (self._lifespan,),
             )
```

### Comparing `expiringsqlitedict-4.1.0/test.py` & `expiringsqlitedict-5.0.0/test.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,89 +2,117 @@
 # -*- coding: utf-8 -*-
 # Copyright © 2021 Taylor C. Richberger
 # This code is released under the license described in the LICENSE file
 
 import unittest
 from datetime import timedelta
 from tempfile import TemporaryDirectory
-import time
 from pathlib import Path
-from expiringsqlitedict import SqliteDict, AutocommitSqliteDict, ZlibPickleSerializer, OnDemand
-from typing import Any
+from expiringsqlitedict import SqliteDict, SimpleSqliteDict
 import json
 import marshal
 import pickle
 
 class TestExpiringDict(unittest.TestCase):
     def test_simple(self):
         with TemporaryDirectory() as temporary_directory:
             db_path = Path(temporary_directory) / 'test.db'
 
-            with OnDemand(str(db_path), serializer=ZlibPickleSerializer) as d:
+            with SqliteDict(str(db_path)) as d:
                 self.assertFalse(bool(d))
                 self.assertEqual(set(d), set())
                 self.assertEqual(set(d.keys()), set())
                 self.assertEqual(set(d.items()), set())
                 self.assertEqual(set(d.values()), set())
                 self.assertEqual(len(d), 0)
                 d['foo'] = 'bar'
                 d['baz'] = 1337
 
-            with SqliteDict(str(db_path), serializer=ZlibPickleSerializer) as d:
+            with SqliteDict(str(db_path)) as d:
                 self.assertTrue(bool(d))
                 self.assertEqual(set(d), {'foo', 'baz'})
                 self.assertEqual(set(d.keys()), {'foo', 'baz'})
                 self.assertEqual(set(d.items()), {('foo', 'bar'), ('baz', 1337)})
                 self.assertEqual(set(d.values()), {'bar', 1337})
                 self.assertEqual(len(d), 2)
 
     def test_quotes(self):
         with TemporaryDirectory() as temporary_directory:
             db_path = Path(temporary_directory) / 'test.db'
 
-            with OnDemand(str(db_path), table = 'Name\\with"special\t-_ char""ac"""ters') as d:
+            with SqliteDict(
+                str(db_path),
+                table = 'Name\\with"special\t-_ char""ac"""ters',
+            ) as d:
                 self.assertFalse(bool(d))
                 self.assertEqual(set(d), set())
                 self.assertEqual(set(d.keys()), set())
                 self.assertEqual(set(d.items()), set())
                 self.assertEqual(set(d.values()), set())
                 self.assertEqual(len(d), 0)
                 d['foo'] = 'bar'
                 d['baz'] = 1337
 
-            with SqliteDict(str(db_path), table = 'Name\\with"special\t-_ char""ac"""ters') as d:
+            with SqliteDict(
+                str(db_path),
+                table = 'Name\\with"special\t-_ char""ac"""ters',
+            ) as d:
                 self.assertTrue(bool(d))
                 self.assertEqual(set(d), {'foo', 'baz'})
                 self.assertEqual(set(d.keys()), {'foo', 'baz'})
                 self.assertEqual(set(d.items()), {('foo', 'bar'), ('baz', 1337)})
                 self.assertEqual(set(d.values()), {'bar', 1337})
                 self.assertEqual(len(d), 2)
 
     def test_autocommit(self):
         with TemporaryDirectory() as temporary_directory:
             db_path = Path(temporary_directory) / 'test.db'
 
-            d = AutocommitSqliteDict(str(db_path))
+            d = SimpleSqliteDict(str(db_path))
             self.assertFalse(bool(d))
             self.assertEqual(set(d), set())
             self.assertEqual(set(d.keys()), set())
             self.assertEqual(set(d.items()), set())
             self.assertEqual(set(d.values()), set())
             self.assertEqual(len(d), 0)
             d['foo'] = 'bar'
             d['baz'] = 1337
 
-            d = AutocommitSqliteDict(str(db_path))
+            d = SimpleSqliteDict(str(db_path))
             self.assertTrue(bool(d))
             self.assertEqual(set(d), {'foo', 'baz'})
             self.assertEqual(set(d.keys()), {'foo', 'baz'})
             self.assertEqual(set(d.items()), {('foo', 'bar'), ('baz', 1337)})
             self.assertEqual(set(d.values()), {'bar', 1337})
             self.assertEqual(len(d), 2)
 
+    def test_isolation_level(self):
+        with TemporaryDirectory() as temporary_directory:
+            db_path = Path(temporary_directory) / 'test.db'
+
+            d = SimpleSqliteDict(str(db_path), isolation_level='DEFERRED')
+            self.assertFalse(bool(d))
+            self.assertEqual(set(d), set())
+            self.assertEqual(set(d.keys()), set())
+            self.assertEqual(set(d.items()), set())
+            self.assertEqual(set(d.values()), set())
+            self.assertEqual(len(d), 0)
+            d['foo'] = 'bar'
+            d.connection.commit()
+            d['baz'] = 1337
+            d.connection.rollback()
+
+            d = SimpleSqliteDict(str(db_path))
+            self.assertTrue(bool(d))
+            self.assertEqual(set(d), {'foo'})
+            self.assertEqual(set(d.keys()), {'foo'})
+            self.assertEqual(set(d.items()), {('foo', 'bar')})
+            self.assertEqual(set(d.values()), {'bar'})
+            self.assertEqual(len(d), 1)
+
     def test_nested(self):
         with TemporaryDirectory() as temporary_directory:
             db_path = Path(temporary_directory) / 'test.db'
 
             with SqliteDict(str(db_path)) as d:
                 d['foo'] = {'foo': 'bar', 'baz': [2, 'two']}
 
@@ -137,13 +165,16 @@
                 # This triggers the actual expiry
                 d['baz'] = 1337
 
             with SqliteDict(str(db_path)) as d:
                 self.assertTrue(bool(d))
                 self.assertEqual(set(d), {'baz', 'postponed'})
                 self.assertEqual(set(d.keys()), {'baz', 'postponed'})
-                self.assertEqual(set(d.items()), {('baz', 1337), ('postponed', 'worked')})
+                self.assertEqual(
+                    set(d.items()),
+                    {('baz', 1337), ('postponed', 'worked')},
+                )
                 self.assertEqual(set(d.values()), {1337, 'worked'})
                 self.assertEqual(len(d), 2)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `expiringsqlitedict-4.1.0/PKG-INFO` & `expiringsqlitedict-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: expiringsqlitedict
-Version: 4.1.0
-Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and pickle
+Version: 5.0.0
+Summary: Persistent compressed expiring dict in Python, backed up by sqlite3 and json
 Author-email: "Taylor C. Richberger" <tcr@absolute-performance.com>
 Requires-Python: >= 3.6, < 4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -59,16 +59,18 @@
 
 * Values can be any json-capable objects (this can be customized to be as
   flexible as you need, through custom serializers)
 * Support for access from multiple programs or threads, with locking fully
   managed by sqlite itself.
 * A very simple codebase that is easy to read, relying on sqlite for as much
   behavior as possible.
-* A simple autocommit wrapper (``AutocommitSqliteDict``), if you really can't
+* A simple autocommit wrapper (``SimpleSqliteDict``), if you really can't
   handle a context manager and need something that fully handles like a dict.
+  You can specify a ``isolation_level`` on this to have to commit and roll back
+  yourself.
 * An on-demand wrapper (``OnDemand``), for situations where you want to open and
   close the database in as narrow a window as possible.
 * Support for custom serialization or compression:
 
 .. code-block:: python
 
   import json
```

