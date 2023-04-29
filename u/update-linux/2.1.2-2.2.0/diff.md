# Comparing `tmp/update-linux-2.1.2.tar.gz` & `tmp/update-linux-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "update-linux-2.1.2.tar", last modified: Mon Apr 24 14:10:06 2023, max compression
+gzip compressed data, was "update-linux-2.2.0.tar", last modified: Sat Apr 29 15:50:51 2023, max compression
```

## Comparing `update-linux-2.1.2.tar` & `update-linux-2.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-24 14:10:06.844797 update-linux-2.1.2/
--rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-24 14:10:06.844797 update-linux-2.1.2/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)     4854 2023-04-24 14:10:06.000000 update-linux-2.1.2/README.md
--rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-24 14:10:06.844797 update-linux-2.1.2/setup.cfg
--rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.1.2/setup_update_linux.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-24 14:10:06.844797 update-linux-2.1.2/update_linux/
--rwxr-xr-x   0 barry     (1000) barry     (1000)    18211 2023-04-24 14:09:38.000000 update-linux-2.1.2/update_linux/__init__.py
--rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.1.2/update_linux/__main__.py
-drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-24 14:10:06.844797 update-linux-2.1.2/update_linux.egg-info/
--rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/PKG-INFO
--rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/SOURCES.txt
--rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/dependency_links.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/entry_points.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/requires.txt
--rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-24 14:10:06.000000 update-linux-2.1.2/update_linux.egg-info/top_level.txt
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-29 15:50:51.417044 update-linux-2.2.0/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-29 15:50:51.417044 update-linux-2.2.0/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)     4854 2023-04-29 15:50:51.000000 update-linux-2.2.0/README.md
+-rw-r--r--   0 barry     (1000) barry     (1000)       38 2023-04-29 15:50:51.417044 update-linux-2.2.0/setup.cfg
+-rw-r--r--   0 barry     (1000) barry     (1000)     2127 2023-04-02 12:26:46.000000 update-linux-2.2.0/setup_update_linux.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-29 15:50:51.417044 update-linux-2.2.0/update_linux/
+-rwxr-xr-x   0 barry     (1000) barry     (1000)    18153 2023-04-29 12:17:06.000000 update-linux-2.2.0/update_linux/__init__.py
+-rw-r--r--   0 barry     (1000) barry     (1000)      144 2023-04-15 15:36:02.000000 update-linux-2.2.0/update_linux/__main__.py
+drwxr-xr-x   0 barry     (1000) barry     (1000)        0 2023-04-29 15:50:51.417044 update-linux-2.2.0/update_linux.egg-info/
+-rw-r--r--   0 barry     (1000) barry     (1000)     5408 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/PKG-INFO
+-rw-r--r--   0 barry     (1000) barry     (1000)      299 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/SOURCES.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)        1 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/dependency_links.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       60 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/entry_points.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       21 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/requires.txt
+-rw-r--r--   0 barry     (1000) barry     (1000)       13 2023-04-29 15:50:51.000000 update-linux-2.2.0/update_linux.egg-info/top_level.txt
```

### Comparing `update-linux-2.1.2/PKG-INFO` & `update-linux-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.1.2
+Version: 2.2.0
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `update-linux-2.1.2/README.md` & `update-linux-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `update-linux-2.1.2/setup_update_linux.py` & `update-linux-2.2.0/setup_update_linux.py`

 * *Files identical despite different names*

### Comparing `update-linux-2.1.2/update_linux/__init__.py` & `update-linux-2.2.0/update_linux/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import socket
 import platform
 import tempfile
 import json
 from config_path import ConfigPath  # type: ignore
 
-VERSION = '2.1.2'
+VERSION = '2.2.0'
 
 default_json_config_template = u'''{
     "group":
         {"all": []},
     "logdir":   "%(logdir)s"
 }
 '''
@@ -199,22 +199,15 @@
             print( 'Log directory: %s' % (self.logdir,) )
             return 0
 
         all_to_exclude = []
         if self.opt_exclude:
             all_to_exclude = self.all_groups.get( self.opt_exclude(), self.opt_exclude() )
 
-        for group_or_host in positional_args:
-            if group_or_host in self.all_groups:
-                for host in self.all_groups[ group_or_host ]:
-                    if host not in all_to_exclude:
-                        self.all_hosts.append( host )
-            else:
-                if group_or_host not in all_to_exclude:
-                    self.all_hosts.append( group_or_host )
+        self.all_hosts = list( self.hostIter( positional_args ) )
 
         if len(self.all_hosts) == 0:
             self.error( '', 'No hosts to update' )
             print('''
 For help:
     %s --help
 ''' % (appname.name,))
@@ -249,14 +242,22 @@
 
         print( '-' * 60 )
         for line in self.all_summary_lines:
             print( line )
 
         return 0
 
+    def hostIter( self, groups_or_hosts ):
+        for group_or_host in groups_or_hosts:
+            if group_or_host in self.all_groups:
+                yield from self.hostIter( self.all_groups[ group_or_host ] )
+
+            else:
+                yield group_or_host
+
     def isThisHost( self, other_host ):
         this_host = socket.gethostname()
         this_info = socket.getaddrinfo( this_host, 'ssh', proto=socket.IPPROTO_TCP )
         this_addrs = set(info[4][0] for info in this_info) | set(['::1', '127.0.0.1'])
 
         try:
             other_info = socket.getaddrinfo( other_host, 'ssh', proto=socket.IPPROTO_TCP )
```

### Comparing `update-linux-2.1.2/update_linux.egg-info/PKG-INFO` & `update-linux-2.2.0/update_linux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: update-linux
-Version: 2.1.2
+Version: 2.2.0
 Summary: Update Linux
 Home-page: https://github.com/barry-scott/CLI-tools
 Author: Barry Scott
 Author-email: barry@barrys-emacs.org
 License: Apache 2.0
 Keywords: development
 Classifier: Development Status :: 5 - Production/Stable
```

