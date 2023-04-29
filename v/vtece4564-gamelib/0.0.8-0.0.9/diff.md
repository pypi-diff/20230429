# Comparing `tmp/vtece4564-gamelib-0.0.8.tar.gz` & `tmp/vtece4564-gamelib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtece4564-gamelib-0.0.8.tar", last modified: Sat Apr 22 20:03:44 2023, max compression
+gzip compressed data, was "vtece4564-gamelib-0.0.9.tar", last modified: Sat Apr 22 20:08:49 2023, max compression
```

## Comparing `vtece4564-gamelib-0.0.8.tar` & `vtece4564-gamelib-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.578627 vtece4564-gamelib-0.0.8/
--rw-r--r--   0 ceharris   (501) staff       (20)     1262 2023-04-22 20:03:44.579120 vtece4564-gamelib-0.0.8/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)      757 2023-04-22 19:06:37.000000 vtece4564-gamelib-0.0.8/README.md
--rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 vtece4564-gamelib-0.0.8/pyproject.toml
--rw-r--r--   0 ceharris   (501) staff       (20)      785 2023-04-22 20:03:44.582525 vtece4564-gamelib-0.0.8/setup.cfg
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.555892 vtece4564-gamelib-0.0.8/src/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.556024 vtece4564-gamelib-0.0.8/src/main/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.557284 vtece4564-gamelib-0.0.8/src/main/python/
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.561066 vtece4564-gamelib-0.0.8/src/main/python/gameauth/
--rw-r--r--   0 ceharris   (501) staff       (20)      210 2023-04-20 13:57:00.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2004 2023-04-19 17:45:40.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/__main__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1515 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/key_util.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1285 2023-04-22 18:42:22.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/password.py
--rw-r--r--   0 ceharris   (501) staff       (20)      260 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/token.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1861 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/token_generator.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2155 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.8/src/main/python/gameauth/token_validator.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.561730 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/
--rw-r--r--   0 ceharris   (501) staff       (20)        0 2023-04-19 19:21:49.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/__init__.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.566462 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/
--rw-r--r--   0 ceharris   (501) staff       (20)      188 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     4949 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/game_client.py
--rw-r--r--   0 ceharris   (501) staff       (20)      348 2023-04-20 10:13:04.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/game_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3914 2023-04-21 19:49:31.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/tcp_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1596 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/ws_connection.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.569132 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/
--rw-r--r--   0 ceharris   (501) staff       (20)      187 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     7178 2023-04-21 16:16:01.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/game_connection.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3489 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/tcp_listener.py
--rw-r--r--   0 ceharris   (501) staff       (20)     3835 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/ws_listener.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.570741 vtece4564-gamelib-0.0.8/src/main/python/gamedb/
--rw-r--r--   0 ceharris   (501) staff       (20)      156 2023-04-19 10:45:29.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)      884 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/game_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.572639 vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/
--rw-r--r--   0 ceharris   (501) staff       (20)      130 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2154 2023-04-21 19:23:56.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/game_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1473 2023-04-21 19:24:11.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/json_db.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2299 2023-04-21 19:28:13.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/user_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.574128 vtece4564-gamelib-0.0.8/src/main/python/gamedb/mongo/
--rw-r--r--   0 ceharris   (501) staff       (20)       98 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/mongo/__init__.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1936 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/mongo/game_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     2344 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/mongo/user_repository.py
--rw-r--r--   0 ceharris   (501) staff       (20)     1085 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.8/src/main/python/gamedb/user_repository.py
-drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:03:44.577810 vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/
--rw-r--r--   0 ceharris   (501) staff       (20)     1262 2023-04-22 20:03:44.000000 vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO
--rw-r--r--   0 ceharris   (501) staff       (20)     1485 2023-04-22 20:03:44.000000 vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt
--rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-22 20:03:44.000000 vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/dependency_links.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       85 2023-04-22 20:03:44.000000 vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/requires.txt
--rw-r--r--   0 ceharris   (501) staff       (20)       25 2023-04-22 20:03:44.000000 vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/top_level.txt
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.654787 vtece4564-gamelib-0.0.9/
+-rw-r--r--   0 ceharris   (501) staff       (20)     1262 2023-04-22 20:08:49.654974 vtece4564-gamelib-0.0.9/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)      757 2023-04-22 19:06:37.000000 vtece4564-gamelib-0.0.9/README.md
+-rw-r--r--   0 ceharris   (501) staff       (20)       41 2023-04-21 18:22:43.000000 vtece4564-gamelib-0.0.9/pyproject.toml
+-rw-r--r--   0 ceharris   (501) staff       (20)      788 2023-04-22 20:08:49.656476 vtece4564-gamelib-0.0.9/setup.cfg
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.635166 vtece4564-gamelib-0.0.9/src/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.635256 vtece4564-gamelib-0.0.9/src/main/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.636454 vtece4564-gamelib-0.0.9/src/main/python/
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.640319 vtece4564-gamelib-0.0.9/src/main/python/gameauth/
+-rw-r--r--   0 ceharris   (501) staff       (20)      210 2023-04-20 13:57:00.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2004 2023-04-19 17:45:40.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/__main__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1515 2023-04-19 17:39:08.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/key_util.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1285 2023-04-22 18:42:22.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/password.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      260 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/token.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1861 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/token_generator.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2155 2023-04-20 11:44:01.000000 vtece4564-gamelib-0.0.9/src/main/python/gameauth/token_validator.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.640914 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/
+-rw-r--r--   0 ceharris   (501) staff       (20)        0 2023-04-19 19:21:49.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/__init__.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.643246 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/
+-rw-r--r--   0 ceharris   (501) staff       (20)      188 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     4949 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/game_client.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      348 2023-04-20 10:13:04.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/game_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3914 2023-04-21 19:49:31.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/tcp_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1596 2023-04-21 16:13:42.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/ws_connection.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.645363 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/
+-rw-r--r--   0 ceharris   (501) staff       (20)      187 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     7178 2023-04-21 16:16:01.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/game_connection.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3489 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/tcp_listener.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     3835 2023-04-21 16:14:58.000000 vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/ws_listener.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.647765 vtece4564-gamelib-0.0.9/src/main/python/gamedb/
+-rw-r--r--   0 ceharris   (501) staff       (20)      156 2023-04-19 10:45:29.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)      884 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/game_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.649492 vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/
+-rw-r--r--   0 ceharris   (501) staff       (20)      130 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2154 2023-04-21 19:23:56.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/game_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1473 2023-04-21 19:24:11.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/json_db.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2299 2023-04-21 19:28:13.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/user_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.650898 vtece4564-gamelib-0.0.9/src/main/python/gamedb/mongo/
+-rw-r--r--   0 ceharris   (501) staff       (20)       98 2023-04-21 14:47:05.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/mongo/__init__.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1936 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/mongo/game_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     2344 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/mongo/user_repository.py
+-rw-r--r--   0 ceharris   (501) staff       (20)     1085 2023-04-21 14:57:04.000000 vtece4564-gamelib-0.0.9/src/main/python/gamedb/user_repository.py
+drwxr-xr-x   0 ceharris   (501) staff       (20)        0 2023-04-22 20:08:49.654380 vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/
+-rw-r--r--   0 ceharris   (501) staff       (20)     1262 2023-04-22 20:08:49.000000 vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO
+-rw-r--r--   0 ceharris   (501) staff       (20)     1485 2023-04-22 20:08:49.000000 vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)        1 2023-04-22 20:08:49.000000 vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/dependency_links.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       88 2023-04-22 20:08:49.000000 vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/requires.txt
+-rw-r--r--   0 ceharris   (501) staff       (20)       25 2023-04-22 20:08:49.000000 vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/top_level.txt
```

### Comparing `vtece4564-gamelib-0.0.8/PKG-INFO` & `vtece4564-gamelib-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtece4564-gamelib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A support library for the ECE 4564 Final Project
 Home-page: https://code.vt.edu/ece4564/gamelib
 Author: Carl Harris
 Author-email: ceharris414@gmail.com
 Project-URL: Bug Tracker, https://code.vt.edu/ece4564/gamelib/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtece4564-gamelib-0.0.8/README.md` & `vtece4564-gamelib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/setup.cfg` & `vtece4564-gamelib-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vtece4564-gamelib
-version = 0.0.8
+version = 0.0.9
 author = Carl Harris
 author_email = ceharris414@gmail.com
 description = A support library for the ECE 4564 Final Project
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.vt.edu/ece4564/gamelib
 project_urls = 
@@ -20,15 +20,15 @@
 packages = find:
 python_requires = >=3.10
 install_requires = 
 	cryptography==40.0.2
 	pyjwt==2.6.0
 	pymongo==4.3.3
 	websockets==11.0.2
-	purecrypt==0.0.2
+	py-purecrypt==0.0.2
 
 [options.packages.find]
 where = src/main/python
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gameauth/__main__.py` & `vtece4564-gamelib-0.0.9/src/main/python/gameauth/__main__.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gameauth/key_util.py` & `vtece4564-gamelib-0.0.9/src/main/python/gameauth/key_util.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gameauth/password.py` & `vtece4564-gamelib-0.0.9/src/main/python/gameauth/password.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gameauth/token_generator.py` & `vtece4564-gamelib-0.0.9/src/main/python/gameauth/token_generator.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gameauth/token_validator.py` & `vtece4564-gamelib-0.0.9/src/main/python/gameauth/token_validator.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/game_client.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/game_client.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/tcp_connection.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/tcp_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamecomm/client/ws_connection.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamecomm/client/ws_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/game_connection.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/game_connection.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/tcp_listener.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/tcp_listener.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamecomm/server/ws_listener.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamecomm/server/ws_listener.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/game_repository.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/game_repository.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/json_db.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/json_db.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/json/user_repository.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/json/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/mongo/game_repository.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/mongo/game_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/mongo/user_repository.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/mongo/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/gamedb/user_repository.py` & `vtece4564-gamelib-0.0.9/src/main/python/gamedb/user_repository.py`

 * *Files identical despite different names*

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO` & `vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtece4564-gamelib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A support library for the ECE 4564 Final Project
 Home-page: https://code.vt.edu/ece4564/gamelib
 Author: Carl Harris
 Author-email: ceharris414@gmail.com
 Project-URL: Bug Tracker, https://code.vt.edu/ece4564/gamelib/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vtece4564-gamelib-0.0.8/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt` & `vtece4564-gamelib-0.0.9/src/main/python/vtece4564_gamelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

