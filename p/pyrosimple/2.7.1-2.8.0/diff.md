# Comparing `tmp/pyrosimple-2.7.1.tar.gz` & `tmp/pyrosimple-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrosimple-2.7.1.tar", max compression
+gzip compressed data, was "pyrosimple-2.8.0.tar", max compression
```

## Comparing `pyrosimple-2.7.1.tar` & `pyrosimple-2.8.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0     2131 2023-03-04 03:16:06.914134 pyrosimple-2.7.1/README.md
--rw-r--r--   0        0        0     3349 2023-04-10 02:50:11.296848 pyrosimple-2.7.1/pyproject.toml
--rw-r--r--   0        0        0      538 2022-12-19 17:11:38.923701 pyrosimple-2.7.1/src/pyrosimple/__init__.py
--rw-r--r--   0        0        0     8752 2023-03-04 03:16:46.423995 pyrosimple-2.7.1/src/pyrosimple/config.py
--rw-r--r--   0        0        0       67 2023-02-28 18:23:01.538870 pyrosimple-2.7.1/src/pyrosimple/data/__init__.py
--rw-r--r--   0        0        0    10194 2023-02-28 18:06:46.631474 pyrosimple-2.7.1/src/pyrosimple/data/full-example.rc
--rw-r--r--   0        0        0     1273 2022-12-19 17:11:38.923701 pyrosimple-2.7.1/src/pyrosimple/error.py
--rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/io/__init__.py
--rw-r--r--   0        0        0     8616 2023-04-02 15:39:14.262135 pyrosimple-2.7.1/src/pyrosimple/io/scgi.py
--rw-r--r--   0        0        0        0 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/job/__init__.py
--rw-r--r--   0        0        0     2963 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/job/action.py
--rw-r--r--   0        0        0     2977 2022-12-29 19:15:58.212292 pyrosimple-2.7.1/src/pyrosimple/job/base.py
--rw-r--r--   0        0        0     9444 2023-02-18 20:32:42.360835 pyrosimple-2.7.1/src/pyrosimple/job/metrics.py
--rw-r--r--   0        0        0     1691 2023-02-04 21:14:43.625074 pyrosimple-2.7.1/src/pyrosimple/job/move_path.py
--rw-r--r--   0        0        0     1743 2022-12-19 17:11:41.443698 pyrosimple-2.7.1/src/pyrosimple/job/move_torrent.py
--rw-r--r--   0        0        0     4197 2023-01-22 17:54:55.278327 pyrosimple-2.7.1/src/pyrosimple/job/queue.py
--rw-r--r--   0        0        0     9954 2023-03-28 00:31:31.950154 pyrosimple-2.7.1/src/pyrosimple/job/watch.py
--rw-r--r--   0        0        0        0 2022-12-18 17:48:03.812685 pyrosimple-2.7.1/src/pyrosimple/py.typed
--rw-r--r--   0        0        0      112 2023-01-15 15:15:41.811874 pyrosimple-2.7.1/src/pyrosimple/scripts/__init__.py
--rw-r--r--   0        0        0     8190 2023-04-08 13:35:58.048768 pyrosimple-2.7.1/src/pyrosimple/scripts/base.py
--rw-r--r--   0        0        0    17593 2023-04-08 13:23:16.125477 pyrosimple-2.7.1/src/pyrosimple/scripts/chtor.py
--rw-r--r--   0        0        0     6590 2023-03-25 15:45:13.757347 pyrosimple-2.7.1/src/pyrosimple/scripts/lstor.py
--rw-r--r--   0        0        0     9723 2023-03-27 23:30:07.160434 pyrosimple-2.7.1/src/pyrosimple/scripts/mktor.py
--rw-r--r--   0        0        0    13634 2023-03-27 23:36:36.156689 pyrosimple-2.7.1/src/pyrosimple/scripts/pyroadmin.py
--rw-r--r--   0        0        0     9555 2023-03-18 01:42:48.673745 pyrosimple-2.7.1/src/pyrosimple/scripts/pyrotorque.py
--rw-r--r--   0        0        0    35338 2023-03-04 03:16:46.760660 pyrosimple-2.7.1/src/pyrosimple/scripts/rtcontrol.py
--rw-r--r--   0        0        0    10294 2023-03-30 18:14:33.472926 pyrosimple-2.7.1/src/pyrosimple/scripts/rtxmlrpc.py
--rw-r--r--   0        0        0      117 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/torrent/__init__.py
--rw-r--r--   0        0        0    29545 2023-03-28 02:07:56.670430 pyrosimple-2.7.1/src/pyrosimple/torrent/engine.py
--rw-r--r--   0        0        0    37489 2023-03-28 02:04:30.984695 pyrosimple-2.7.1/src/pyrosimple/torrent/rtorrent.py
--rw-r--r--   0        0        0      118 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/ui/__init__.py
--rw-r--r--   0        0        0     2903 2022-12-19 17:12:53.930262 pyrosimple-2.7.1/src/pyrosimple/ui/categories.py
--rw-r--r--   0        0        0      122 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/__init__.py
--rw-r--r--   0        0        0     2106 2022-12-29 14:05:43.470686 pyrosimple-2.7.1/src/pyrosimple/util/cache.py
--rw-r--r--   0        0        0     7891 2023-02-08 18:31:37.923717 pyrosimple-2.7.1/src/pyrosimple/util/fmt.py
--rw-r--r--   0        0        0      459 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/logutil.py
--rw-r--r--   0        0        0    31824 2023-04-03 02:55:17.578411 pyrosimple-2.7.1/src/pyrosimple/util/matching.py
--rw-r--r--   0        0        0    26411 2023-03-25 15:41:05.564729 pyrosimple-2.7.1/src/pyrosimple/util/metafile.py
--rw-r--r--   0        0        0     1999 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/pymagic.py
--rwxr-xr-x   0        0        0     9554 2023-04-02 15:37:53.245666 pyrosimple-2.7.1/src/pyrosimple/util/rpc.py
--rw-r--r--   0        0        0     8584 2022-12-19 17:11:41.447031 pyrosimple-2.7.1/src/pyrosimple/util/traits.py
--rw-r--r--   0        0        0     2187 2023-01-10 16:31:49.350547 pyrosimple-2.7.1/src/pyrosimple/util/ui.py
--rw-r--r--   0        0        0     4166 1970-01-01 00:00:00.000000 pyrosimple-2.7.1/setup.py
--rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.7.1/PKG-INFO
+-rw-r--r--   0        0        0     2131 2023-04-13 23:28:24.964236 pyrosimple-2.8.0/README.md
+-rw-r--r--   0        0        0     3349 2023-04-29 17:00:31.095411 pyrosimple-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0      538 2023-04-13 23:28:24.974236 pyrosimple-2.8.0/src/pyrosimple/__init__.py
+-rw-r--r--   0        0        0     8723 2023-04-29 15:30:45.920385 pyrosimple-2.8.0/src/pyrosimple/config.py
+-rw-r--r--   0        0        0       67 2023-04-13 23:29:22.257480 pyrosimple-2.8.0/src/pyrosimple/data/__init__.py
+-rw-r--r--   0        0        0    10194 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/data/full-example.rc
+-rw-r--r--   0        0        0     1273 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/error.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/io/__init__.py
+-rw-r--r--   0        0        0     8616 2023-04-20 06:43:18.099234 pyrosimple-2.8.0/src/pyrosimple/io/scgi.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/__init__.py
+-rw-r--r--   0        0        0     2963 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/action.py
+-rw-r--r--   0        0        0     2977 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/base.py
+-rw-r--r--   0        0        0     9444 2023-04-13 23:29:22.257480 pyrosimple-2.8.0/src/pyrosimple/job/metrics.py
+-rw-r--r--   0        0        0     1691 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/move_path.py
+-rw-r--r--   0        0        0     1743 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/move_torrent.py
+-rw-r--r--   0        0        0     4197 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/job/queue.py
+-rw-r--r--   0        0        0     9954 2023-04-13 23:29:54.100762 pyrosimple-2.8.0/src/pyrosimple/job/watch.py
+-rw-r--r--   0        0        0        0 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/py.typed
+-rw-r--r--   0        0        0      112 2023-04-13 23:28:24.977569 pyrosimple-2.8.0/src/pyrosimple/scripts/__init__.py
+-rw-r--r--   0        0        0     8094 2023-04-14 00:40:44.581127 pyrosimple-2.8.0/src/pyrosimple/scripts/base.py
+-rw-r--r--   0        0        0    17593 2023-04-13 23:38:22.673176 pyrosimple-2.8.0/src/pyrosimple/scripts/chtor.py
+-rw-r--r--   0        0        0     6590 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/lstor.py
+-rw-r--r--   0        0        0     9723 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/mktor.py
+-rw-r--r--   0        0        0    13632 2023-04-29 15:30:45.910385 pyrosimple-2.8.0/src/pyrosimple/scripts/pyroadmin.py
+-rw-r--r--   0        0        0     9555 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/pyrotorque.py
+-rw-r--r--   0        0        0    35338 2023-04-13 23:29:22.260813 pyrosimple-2.8.0/src/pyrosimple/scripts/rtcontrol.py
+-rw-r--r--   0        0        0    10294 2023-04-13 23:28:24.980902 pyrosimple-2.8.0/src/pyrosimple/scripts/rtxmlrpc.py
+-rw-r--r--   0        0        0      117 2023-04-13 23:28:24.980902 pyrosimple-2.8.0/src/pyrosimple/torrent/__init__.py
+-rw-r--r--   0        0        0    30437 2023-04-29 17:00:31.095411 pyrosimple-2.8.0/src/pyrosimple/torrent/engine.py
+-rw-r--r--   0        0        0    37020 2023-04-19 03:02:54.236669 pyrosimple-2.8.0/src/pyrosimple/torrent/rtorrent.py
+-rw-r--r--   0        0        0      118 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/ui/__init__.py
+-rw-r--r--   0        0        0     2903 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/ui/categories.py
+-rw-r--r--   0        0        0      122 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/__init__.py
+-rw-r--r--   0        0        0     2164 2023-04-19 02:04:04.304690 pyrosimple-2.8.0/src/pyrosimple/util/cache.py
+-rw-r--r--   0        0        0     7891 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/fmt.py
+-rw-r--r--   0        0        0      459 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/logutil.py
+-rw-r--r--   0        0        0    31824 2023-04-13 23:38:22.676510 pyrosimple-2.8.0/src/pyrosimple/util/matching.py
+-rw-r--r--   0        0        0    26411 2023-04-13 23:29:22.267480 pyrosimple-2.8.0/src/pyrosimple/util/metafile.py
+-rw-r--r--   0        0        0     1999 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/pymagic.py
+-rwxr-xr-x   0        0        0     9554 2023-04-13 23:29:22.267480 pyrosimple-2.8.0/src/pyrosimple/util/rpc.py
+-rw-r--r--   0        0        0     8584 2023-04-19 02:15:38.352321 pyrosimple-2.8.0/src/pyrosimple/util/traits.py
+-rw-r--r--   0        0        0     2187 2023-04-13 23:28:24.984236 pyrosimple-2.8.0/src/pyrosimple/util/ui.py
+-rw-r--r--   0        0        0     4287 1970-01-01 00:00:00.000000 pyrosimple-2.8.0/PKG-INFO
```

### Comparing `pyrosimple-2.7.1/README.md` & `pyrosimple-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/pyproject.toml` & `pyrosimple-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyrosimple"
-version = "2.7.1"
+version = "2.8.0"
 description = "A stripped-down version of the pyrocore tools for working with rTorrent"
 authors = ["kannibalox <kannibalox@gmail.com>"]
 repository = "https://github.com/kannibalox/pyrosimple"
 documentation = "https://kannibalox.github.io/pyrosimple/"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 classifiers = [
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/__init__.py` & `pyrosimple-2.8.0/src/pyrosimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/config.py` & `pyrosimple-2.8.0/src/pyrosimple/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,19 @@
             "action": "{{now()|iso}} {{action}}\t {{d.name}} [{{d.alias}}]",
         },
     }
 )
 
 
 def load_settings() -> Box:
-    """Load settings from (in order of precedenc): the defaults, a
+    """Load settings from (in order of precedence): the defaults, a
     TOML config file, environment variables
     """
     settings_box: Box = DEFAULT_SETTINGS.copy()
-    settings_file = Path(
-        os.getenv(ENVVAR, "~/.config/pyrosimple/config.toml")
-    ).expanduser()
+    settings_file = Path(os.getenv(ENVVAR, str(SETTINGS_FILE))).expanduser()
     if settings_file.exists():
         settings_file_box = Box(
             {
                 k.upper(): v
                 for k, v in tomllib.loads(settings_file.read_text("utf-8")).items()
             }
         )
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/data/full-example.rc` & `pyrosimple-2.8.0/src/pyrosimple/data/full-example.rc`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/error.py` & `pyrosimple-2.8.0/src/pyrosimple/error.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/io/scgi.py` & `pyrosimple-2.8.0/src/pyrosimple/io/scgi.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/action.py` & `pyrosimple-2.8.0/src/pyrosimple/job/action.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/base.py` & `pyrosimple-2.8.0/src/pyrosimple/job/base.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/metrics.py` & `pyrosimple-2.8.0/src/pyrosimple/job/metrics.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/move_path.py` & `pyrosimple-2.8.0/src/pyrosimple/job/move_path.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/move_torrent.py` & `pyrosimple-2.8.0/src/pyrosimple/job/move_torrent.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/queue.py` & `pyrosimple-2.8.0/src/pyrosimple/job/queue.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/job/watch.py` & `pyrosimple-2.8.0/src/pyrosimple/job/watch.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/base.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -231,17 +231,15 @@
         self.parser.add_argument("-U", "--url", help="URL to rtorrent instance")
 
     def get_options(self):
         """Get program options."""
         super().get_options()
         # pylint: disable=import-outside-toplevel
         from pyrosimple import config
-        from pyrosimple.torrent import rtorrent
 
         # pylint: enable=import-outside-toplevel
 
         if self.options.url:
             config.settings["SCGI_URL"] = config.lookup_connection_alias(
                 self.options.url
             )
         config.load_custom_py()
-        self.engine = rtorrent.RtorrentEngine()
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/chtor.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/chtor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/lstor.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/lstor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/mktor.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/mktor.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/pyroadmin.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/pyroadmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
                     i.rpc_call("d.custom.set", ["tm_completed", str(mtime)])
                     i.flush()
             except Exception as e:
                 self.log.error("Could not set tm_loaded for %s: %s", i.hash, e)
 
     def create_config(self):
         """Create a configuration file"""
-        config_path = Path(config.settings.CONFIG)
+        config_path = Path(config.SETTINGS_FILE)
         if config_path.exists():
             self.log.info(
                 "Pyrosimple config path %s already exists, not overwriting", config_path
             )
         else:
             self.log.info("Creating pyrosimple config file '%s'", config_path)
             config_path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/pyrotorque.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/pyrotorque.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/rtcontrol.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/rtcontrol.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/scripts/rtxmlrpc.py` & `pyrosimple-2.8.0/src/pyrosimple/scripts/rtxmlrpc.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/torrent/engine.py` & `pyrosimple-2.8.0/src/pyrosimple/torrent/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,25 +157,26 @@
 
             for dirname in path[common:]:
                 if dirname == "\uFFFE":
                     break
                 result.append(f"{base_indent}{' ' * indent}\\ {dirname}")
                 indent += 1
 
-        prio = {0: "off ", 1: "    ", 2: "high"}.get(fileinfo.prio, "????")
+        prio = {0: "off ", 1: "    ", 2: "high"}.get(fileinfo.priority, "????")
         result.append(
-            f"  {prio} {fmt.iso_datetime(fileinfo.mtime)} {fmt.human_size(fileinfo.size)} {' ' * indent}| {name}"
+            f"  {prio} {fmt.iso_datetime(int(fileinfo.last_touched)/1000000.0)} {fmt.human_size(fileinfo.size_bytes)} {' ' * indent}| {name}"
         )
 
         prev_path = path
 
     while indent > 0:
         indent -= 1
         result.append(f"{base_indent}{' ' * indent}/")
-    result.append(f"{base_indent}= {len(filelist)} file(s)")
+    file_text = "files" if len(filelist) > 1 else "file"
+    result.append(f"{base_indent}= {len(filelist)} {file_text}")
 
     return "\n".join(result)
 
 
 def detect_traits(item):
     """Build traits list from attributes of the passed item. Currently,
     "kind_51", "name" and "alias" are considered.
@@ -185,14 +186,36 @@
     return traits.detect_traits(
         name=item.name,
         alias=item.alias,
         filetype=(list(item.kind_51) or [None]).pop(),
     )
 
 
+def memoize(func, custom_key, empty_value="<empty>"):
+    """Store an expensive result in a custom key
+
+    The reason for `empty_value` is that some results might be
+    indistinguishable from the custom key being unset.
+    """
+
+    def wrapper(item):
+        memoized_value = item.rpc_call("d.custom", [custom_key])
+        if memoized_value == empty_value:
+            return ""
+        if not memoized_value:
+            memoized_value = func(item)
+            if memoized_value:
+                item.rpc_call("d.custom.set", [custom_key, memoized_value])
+            else:
+                item.rpc_call("d.custom.set", [custom_key, empty_value])
+        return memoized_value
+
+    return wrapper
+
+
 class FieldDefinition:
     """Download item field."""
 
     CONSTANT_FIELDS = {"hash"}
 
     def __init__(
         self,
@@ -338,22 +361,24 @@
     yield DynamicField(
         set,
         "kind",
         "ALL kinds of files in this item (the same as kind_0)",
         matcher=matching.TaggedAsFilter,
         formatter=_fmt_tags,
         accessor=lambda o: o.kind_0,
+        requires=["d.custom=kind"],
     )
     yield DynamicField(
         list,
         "traits",
         "automatic classification of this item (audio, video, tv, movie, etc.)",
         matcher=matching.TaggedAsFilter,
         formatter=lambda v: "/".join(v or ["misc", "other"]),
         accessor=detect_traits,
+        requires=["d.custom=memo_alias", "d.custom=kind"],
     )
 
     # Basic fields
     yield ConstantField(
         str,
         "name",
         "name (file or root directory)",
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/torrent/rtorrent.py` & `pyrosimple-2.8.0/src/pyrosimple/torrent/rtorrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,18 +71,20 @@
         self._engine = engine_
         self._fields = ExpiringCache(
             static_keys=engine.FieldDefinition.CONSTANT_FIELDS, expires=cache_expires
         )  # Acts a cache for the item
         self._fields.update(dict(fields))
         self._rpc_cache = ExpiringCache(
             static_keys={
+                "d.hash",
                 "d.name",
                 "d.size_bytes",
                 "d.size_chunks",
-            }
+            },
+            expires=cache_expires,
         )
         if rpc_fields is not None:
             self._rpc_cache.update(rpc_fields)
         if "hash" not in fields:
             self._fields["hash"] = self.rpc_call("d.hash")
 
     def _make_it_so(
@@ -103,59 +105,43 @@
                 if observer is not None:
                     observer(result)
         except rpc.ERRORS as exc:
             raise error.EngineError(
                 f"While {command} torrent {self._fields['hash']}: {exc}"
             ) from exc
 
-    def _get_files(self, attrs: Optional[List[str]] = None):
-        """Get a list of all files in this download; each entry has the
-        attributes C{path} (relative to root), C{size} (in bytes),
-        C{mtime}, C{prio} (0=off, 1=normal, 2=high), C{created},
-        and C{opened}.
+    def _get_files(
+        self,
+        attrs: Optional[List[str]] = None,
+    ) -> List[Box]:
+        """Get a list of all files in this download.
 
         @param attrs: Optional list of additional attributes to fetch.
         """
         try:
             # Get info for all files
-            f_multicall = self._engine.rpc.f.multicall
-            f_params = [
-                self._fields["hash"],
-                rpc.NOHASH,
-                "f.path=",
-                "f.size_bytes=",
-                "f.last_touched=",
-                "f.priority=",
-                "f.is_created=",
-                "f.is_open=",
-            ]
-            for attr in attrs or []:
-                f_params.append(f"f.{attr}=")
-            rpc_result = f_multicall(*tuple(f_params))
+            if attrs is None:
+                attrs = [
+                    "path",
+                    "size_bytes",
+                    "last_touched",
+                    "priority",
+                    "is_created",
+                    "is_open",
+                ]
+
+            rpc_result = self.rpc_call(
+                "f.multicall", [rpc.NOHASH] + [f"f.{attr}=" for attr in attrs]
+            )
         except rpc.ERRORS as exc:
             raise error.EngineError(
                 f"While getting files for torrent #{self._fields['hash']}: {exc}"
             )
         # Return results
-        result = [
-            Box(
-                path=i[0],
-                size=i[1],
-                mtime=i[2] / 1000000.0,
-                prio=i[3],
-                created=i[4],
-                opened=i[5],
-            )
-            for i in rpc_result
-        ]
-
-        if attrs:
-            for idx, attr in enumerate(attrs):
-                for item, rpc_item in zip(result, rpc_result):
-                    item[attr] = rpc_item[6 + idx]
+        result = [Box(**dict(zip(attrs, i))) for i in rpc_result]
 
         return result
 
     def memoize(self, name: str, getter: Callable, *args, **kwargs):
         """Cache a stable expensive-to-get item value for later
         (optimized) retrieval."""
         field = "custom_memo_" + name
@@ -182,17 +168,17 @@
         if histo:
             # Parse histogram from cached field
             histo = [i.split("%_") for i in str(histo).split()]
             histo = [(int(val, 10), ext) for val, ext in histo]
         else:
             # Get file types
             histo = traits.get_filetypes(
-                self._get_files(),
+                self._get_files(["path", "size_bytes"]),
                 path=operator.attrgetter("path"),
-                size=operator.attrgetter("size"),
+                size=operator.attrgetter("size_bytes"),
             )
 
             # Set custom cache field with value formatted like "80%_flac 20%_jpg" (sorted by percentage)
             histo_str = " ".join([f'{i[0]}%_{i[1].replace(" ", "_")}' for i in histo])
             self._make_it_so(
                 f"setting kind cache {histo_str!r} on",
                 ["d.custom.set"],
@@ -488,15 +474,15 @@
         # Do some basic escaping, nothing else should be necessary.
         base_dir = proxy.d.directory_base(self.hash).replace('"', r"\"")
         extra_cmds.insert(0, f'd.directory_base.set="{base_dir}"')
         rpc_metafile = xmlrpclib.Binary(bencode.bencode(dict(torrent)))
         if not copy:
             proxy.d.stop(self.hash)
         self._engine.logger.debug("Running extra commands on load: %s", extra_cmds)
-        if rpc_protocol == "json":
+        if rpc_protocol == "json" and not os.getenv("PYRO_FORCE_JSONRPC_LOAD_RAW"):
             remote_proxy.load.verbose("", rpc_metafile, *extra_cmds)
         else:
             remote_proxy.load.raw_verbose("", rpc_metafile, *extra_cmds)
         for _ in range(0, 10):
             try:
                 remote_proxy.d.hash(self.hash)
                 break
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/ui/categories.py` & `pyrosimple-2.8.0/src/pyrosimple/ui/categories.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/cache.py` & `pyrosimple-2.8.0/src/pyrosimple/util/cache.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,38 +20,38 @@
         # When 3.7 support is dropped, the type can be made more specific:
         # Dict[str, tuple[float, Any]]
         self.data: Dict[Hashable, tuple] = {}
         self.lock = RLock()
         self.static_keys = static_keys or set()
         if items:
             for key, val in items:
-                if key in self.static_keys:
+                if key in self.static_keys or expires == 0:
                     expire_at = 0.0
                 else:
                     expire_at = self.expires + time.time()
                 self.data[key] = (expire_at, val)
 
     def __delitem__(self, key: Hashable):
         with self.lock:
             del self.data[key]
 
     def __setitem__(self, key: Hashable, val: Any, expire: Optional[float] = None):
         with self.lock:
-            if key in self.static_keys or expire == 0:
+            if key in self.static_keys or expire == 0 or self.expires == 0:
                 expire_at = 0.0
             else:
                 expire_at = (expire or self.expires) + time.time()
             self.data[key] = (expire_at, val)
 
     def __getitem__(
         self, key: Hashable, with_age: bool = False
     ) -> Union[Tuple[Any, float], Any]:
         with self.lock:
             expires_at, item = self.data[key]
-            if expires_at == 0 or expires_at > time.time():
+            if expires_at == 0 or self.expires == 0 or expires_at > time.time():
                 if with_age:
                     return item, expires_at - time.time()
                 return item
             del self[key]
             raise KeyError(key)
 
     def __len__(self):
```

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/fmt.py` & `pyrosimple-2.8.0/src/pyrosimple/util/fmt.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/matching.py` & `pyrosimple-2.8.0/src/pyrosimple/util/matching.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/metafile.py` & `pyrosimple-2.8.0/src/pyrosimple/util/metafile.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/pymagic.py` & `pyrosimple-2.8.0/src/pyrosimple/util/pymagic.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/rpc.py` & `pyrosimple-2.8.0/src/pyrosimple/util/rpc.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/traits.py` & `pyrosimple-2.8.0/src/pyrosimple/util/traits.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/src/pyrosimple/util/ui.py` & `pyrosimple-2.8.0/src/pyrosimple/util/ui.py`

 * *Files identical despite different names*

### Comparing `pyrosimple-2.7.1/PKG-INFO` & `pyrosimple-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrosimple
-Version: 2.7.1
+Version: 2.8.0
 Summary: A stripped-down version of the pyrocore tools for working with rTorrent
 Home-page: https://github.com/kannibalox/pyrosimple
 License: GPL-3.0-or-later
 Author: kannibalox
 Author-email: kannibalox@gmail.com
 Requires-Python: >=3.7.2,<4
 Classifier: Development Status :: 4 - Beta
```

