# Comparing `tmp/mama-0.7.7.tar.gz` & `tmp/mama-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.7.7.tar", last modified: Wed Feb  8 12:30:14 2023, max compression
+gzip compressed data, was "mama-0.7.9.tar", last modified: Mon Feb 13 15:33:31 2023, max compression
```

## Comparing `mama-0.7.7.tar` & `mama-0.7.9.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-08 12:30:14.549287 mama-0.7.7/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2023-01-17 13:35:55.000000 mama-0.7.7/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11908 2023-02-08 12:30:14.549287 mama-0.7.7/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11098 2023-02-08 12:22:13.000000 mama-0.7.7/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-08 12:30:14.539287 mama-0.7.7/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2023-01-17 13:35:55.000000 mama-0.7.7/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12094 2023-02-08 12:22:13.000000 mama-0.7.7/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    35427 2023-01-17 13:35:55.000000 mama-0.7.7/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    19901 2023-02-08 12:25:09.000000 mama-0.7.7/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    48509 2023-01-30 21:57:58.000000 mama-0.7.7/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12836 2023-01-18 12:49:22.000000 mama-0.7.7/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    13149 2023-01-30 22:00:52.000000 mama-0.7.7/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2023-01-17 13:35:55.000000 mama-0.7.7/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10608 2023-01-30 22:01:24.000000 mama-0.7.7/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2023-01-17 13:35:55.000000 mama-0.7.7/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7023 2023-01-17 13:35:55.000000 mama-0.7.7/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     6781 2023-01-30 15:22:01.000000 mama-0.7.7/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-18 13:01:37.000000 mama-0.7.7/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-08 12:30:14.549287 mama-0.7.7/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-01-17 13:35:55.000000 mama-0.7.7/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-30 15:17:16.000000 mama-0.7.7/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2023-01-17 13:35:55.000000 mama-0.7.7/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-30 22:10:20.000000 mama-0.7.7/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     9969 2023-02-08 12:22:13.000000 mama-0.7.7/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2023-01-17 13:35:55.000000 mama-0.7.7/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    13797 2023-01-30 21:54:34.000000 mama-0.7.7/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-08 12:30:14.549287 mama-0.7.7/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-01-17 13:35:55.000000 mama-0.7.7/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2023-01-17 13:35:55.000000 mama-0.7.7/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5739 2023-01-30 15:55:08.000000 mama-0.7.7/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1221 2023-01-30 19:27:23.000000 mama-0.7.7/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-08 12:30:14.539287 mama-0.7.7/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11908 2023-02-08 12:30:14.000000 mama-0.7.7/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      719 2023-02-08 12:30:14.000000 mama-0.7.7/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-02-08 12:30:14.000000 mama-0.7.7/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-02-08 12:30:14.000000 mama-0.7.7/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       44 2023-02-08 12:30:14.000000 mama-0.7.7/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-02-08 12:30:14.000000 mama-0.7.7/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1127 2023-02-08 12:28:30.000000 mama-0.7.7/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-02-08 12:30:14.549287 mama-0.7.7/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2023-01-17 13:35:55.000000 mama-0.7.9/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11908 2023-02-13 15:33:31.315010 mama-0.7.9/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11098 2023-02-08 12:22:13.000000 mama-0.7.9/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2023-01-17 13:35:55.000000 mama-0.7.9/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12341 2023-02-09 15:58:10.000000 mama-0.7.9/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    34198 2023-02-09 14:32:53.000000 mama-0.7.9/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    19930 2023-02-13 10:05:48.000000 mama-0.7.9/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    48418 2023-02-09 12:33:47.000000 mama-0.7.9/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12118 2023-02-09 14:04:24.000000 mama-0.7.9/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    13149 2023-01-30 22:00:52.000000 mama-0.7.9/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2023-01-17 13:35:55.000000 mama-0.7.9/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10595 2023-02-09 13:58:46.000000 mama-0.7.9/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2023-01-17 13:35:55.000000 mama-0.7.9/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7023 2023-01-17 13:35:55.000000 mama-0.7.9/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     6781 2023-01-30 15:22:01.000000 mama-0.7.9/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-18 13:01:37.000000 mama-0.7.9/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-09 13:03:03.000000 mama-0.7.9/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3880 2023-02-09 15:04:34.000000 mama-0.7.9/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-01-17 13:35:55.000000 mama-0.7.9/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-30 15:17:16.000000 mama-0.7.9/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2023-01-17 13:35:55.000000 mama-0.7.9/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-30 22:10:20.000000 mama-0.7.9/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    10157 2023-02-09 11:39:01.000000 mama-0.7.9/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2023-01-17 13:35:55.000000 mama-0.7.9/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15125 2023-02-13 15:30:38.000000 mama-0.7.9/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-01-17 13:35:55.000000 mama-0.7.9/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2023-01-17 13:35:55.000000 mama-0.7.9/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5739 2023-01-30 15:55:08.000000 mama-0.7.9/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1221 2023-01-30 19:27:23.000000 mama-0.7.9/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11908 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      770 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       44 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1127 2023-02-13 10:05:09.000000 mama-0.7.9/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-02-13 15:33:31.315010 mama-0.7.9/setup.cfg
```

### Comparing `mama-0.7.7/LICENSE` & `mama-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/PKG-INFO` & `mama-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.7.7
+Version: 0.7.9
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.7.7/README.md` & `mama-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/artifactory.py` & `mama-0.7.9/mama/artifactory.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             return # success
 
 
 def artifactory_sanitize_url(url):
     return url.replace('ftp://', '').replace('http://','').replace('https://','')
 
 
-def artifactory_upload(ftp:ftplib.FTP_TLS, file_path:str):
+def artifactory_upload(ftp:ftplib.FTP_TLS, target_name:str, file_path:str):
     size = os.path.getsize(file_path)
     transferred = 0
     lastpercent = 0
     with open(file_path, 'rb') as f:
         def print_progress(bytes):
             nonlocal transferred, lastpercent, size
             transferred += len(bytes)
@@ -144,14 +144,20 @@
             if abs(lastpercent - percent) >= 5:
                 lastpercent = percent
                 n = int(percent / 2)
                 left = '=' * n
                 right = ' ' * int(50 - n)
                 print(f'\r    |{left}>{right}| {percent:>3} %', end='')
         print(f'    |>{" ":50}| {0:>3} %', end='')
+        # chdir into FTP_ROOT/target_name/
+        try:
+            ftp.cwd(target_name)
+        except:
+            ftp.mkd(target_name) # create subdirectory if needed
+            ftp.cwd(target_name)
         ftp.storbinary(f'STOR {os.path.basename(file_path)}', f, callback=print_progress)
         print(f'\r    |{"="*50}>| 100 %')
 
 
 def artifact_already_exists(ftp:ftplib.FTP_TLS, file_path:str):
     items = []
     ftp.dir(os.path.basename(file_path), items.append)
@@ -168,15 +174,15 @@
         try:
             # sanitize url for ftplib
             url = artifactory_sanitize_url(url)
             artifactory_ftp_login(ftp, config, url)
             if config.if_needed and artifact_already_exists(ftp, file_path):
                 if config.verbose: console(f'  - Artifactory Upload skipped: artifact already exists')
                 return False # skip upload
-            artifactory_upload(ftp, file_path)
+            artifactory_upload(ftp, target.name, file_path)
             return True
         except:
             traceback.print_exc()
         finally:
             ftp.quit()
     return False
 
@@ -240,15 +246,15 @@
         git: Git = target.dep.dep_source
         git.save_status(target.dep)
 
     return (True, dependencies)
 
 
 def _fetch_package(target:BuildTarget, url, archive, build_dir):
-    remote_file = f'http://{url}/{archive}.zip'
+    remote_file = f'http://{url}/{target.name}/{archive}.zip'
     try:
         return download_file(remote_file, build_dir, force=True, 
                              message=f'    Artifactory fetch {url}/{archive} ')
     except Exception as e:
         if target.config.verbose:
             error(f'    Artifactory fetch failed with {e} {url}/{archive}.zip')
```

### Comparing `mama-0.7.7/mama/build_config.py` & `mama-0.7.9/mama/build_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os, sys, multiprocessing, tempfile
+from mama.platforms.oclea import Oclea
 import mama.util as util
 from .utils.system import System, console
 from .utils.sub_process import execute, execute_piped
 
 if System.linux:
     import distro
 
@@ -34,15 +35,15 @@
         # supported platforms
         self.windows = False
         self.linux   = False
         self.macos   = False
         self.ios     = False
         self.android = False
         self.raspi   = False
-        self.oclea    = False
+        self.oclea : Oclea = None
         # compilers
         self.clang = True # prefer clang on linux
         self.gcc   = False
         self.clang_path = ''
         self.gcc_path = ''
         # can be used to overide C and C++ compiler paths
         self.cc_path = ''
@@ -81,18 +82,14 @@
         self.android_ndk_release = ''
         self.android_api     = 'android-26' # 26: Android 8.0 (2017)
         self.android_ndk_stl = 'c++_shared' # LLVM libc++
         ## Raspberry PI - Raspi
         self.raspi_compilers  = ''  ## Raspberry g++ and gcc
         self.raspi_system     = ''  ## path to Raspberry system libraries
         self.raspi_include_paths = [] ## path to additional Raspberry include dirs
-        ## Oclea CV25/CVXX
-        self.oclea_compilers = ''  ## Oclea g++, gcc and ld
-        self.oclea_system    = ''  ## Path to Oclea system libraries
-        self.oclea_include_paths = []  ## Path to additional Oclea include dirs
         ## Convenient installation utils:
         self.convenient_install = []
         ## Workspace and parsing
         self.parallel_load = False  ## Whether to load dependencies in parallel?
         self.global_workspace = False
         if System.windows:
             self.workspaces_root = util.normalized_path(os.getenv('HOMEPATH'))
@@ -204,15 +201,16 @@
                            ios=False, android=False, raspi=False, oclea=False):
         self.windows = windows
         self.linux   = linux
         self.macos   = macos
         self.ios     = ios
         self.android = android
         self.raspi   = raspi
-        self.oclea   = oclea
+        if not oclea: self.oclea = None
+        elif not self.oclea: self.oclea = Oclea(self)
         return True
 
 
     def is_platform_set(self):
         return self.windows or self.linux or self.macos \
             or self.ios or self.android or self.raspi or self.oclea
 
@@ -401,19 +399,19 @@
     def get_preferred_compiler_paths(self):
         if self.cc_path and self.cxx_path and self.cxx_version:
             return (self.cc_path, self.cxx_path, self.cxx_version)
         if self.raspi:  # only GCC available for this platform
             ext = '.exe' if System.windows else ''
             self.cc_path  = f'{self.raspi_bin()}arm-linux-gnueabihf-gcc{ext}'
             self.cxx_path = f'{self.raspi_bin()}arm-linux-gnueabihf-g++{ext}'
-            self.cxx_version = self._get_gcc_clang_version(self.cc_path)
+            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path)
         elif self.oclea:
-            self.cc_path  = f'{self.oclea_bin()}aarch64-oclea-linux-gcc'
-            self.cxx_path = f'{self.oclea_bin()}aarch64-oclea-linux-g++'
-            self.cxx_version = self._get_gcc_clang_version(self.cc_path)
+            self.cc_path  = f'{self.oclea.bin()}aarch64-oclea-linux-gcc'
+            self.cxx_path = f'{self.oclea.bin()}aarch64-oclea-linux-g++'
+            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path)
         elif self.clang:
             suffixes = ['-12','-11','-10','-9','-8','-7','-6','']
             self.clang_path, suffix, ver = self.find_compiler_root(self.clang_path, 'clang++', suffixes)
             self.cc_path = f'{self.clang_path}clang{suffix}'
             self.cxx_path = f'{self.clang_path}clang++{suffix}'
             self.cxx_version = ver
         elif self.gcc:
@@ -482,44 +480,14 @@
         if not self.android_sdk_path: self.init_ndk_path()
         return self.android_sdk_path
 
 
     def android_ndk(self):
         if not self.android_ndk_path: self.init_ndk_path()
         return self.android_ndk_path
-    
-
-    def raspi_bin(self):
-        if not self.raspi_compilers: self.init_raspi_path()
-        return self.raspi_compilers
-
-
-    def raspi_sysroot(self):
-        if not self.raspi_compilers: self.init_raspi_path()
-        return self.raspi_system
-
-    
-    def raspi_includes(self):
-        if not self.raspi_compilers: self.init_raspi_path()
-        return self.raspi_include_paths
-    
-
-    def oclea_bin(self):
-        if not self.oclea_compilers: self.init_oclea_path()
-        return self.oclea_compilers
-
-
-    def oclea_sysroot(self):
-        if not self.oclea_compilers: self.init_oclea_path()
-        return self.oclea_system
-
-    
-    def oclea_includes(self):
-        if not self.oclea_compilers: self.init_oclea_path()
-        return self.oclea_include_paths
 
 
     def init_ndk_path(self):
         paths = []
         self.append_env_path(paths, 'ANDROID_HOME')
         if System.windows: paths += [f'{os.getenv("LOCALAPPDATA")}\\Android\\Sdk']
         elif System.linux: paths += [f'{os.getenv("HOME")}/Android/Sdk', '/usr/bin/android-sdk', '/opt/android-sdk']
@@ -533,14 +501,29 @@
                 if self.print: console(f'Found Android NDK: {self.android_ndk_path}')
                 return
         raise EnvironmentError(f'''Could not detect any Android NDK installations. 
 Default search paths: {paths} 
 Define env ANDROID_HOME with path to Android SDK with NDK at ${{ANDROID_HOME}}/ndk-bundle.''')
 
 
+    def raspi_bin(self):
+        if not self.raspi_compilers: self.init_raspi_path()
+        return self.raspi_compilers
+
+
+    def raspi_sysroot(self):
+        if not self.raspi_compilers: self.init_raspi_path()
+        return self.raspi_system
+
+    
+    def raspi_includes(self):
+        if not self.raspi_compilers: self.init_raspi_path()
+        return self.raspi_include_paths
+
+
     def init_raspi_path(self):
         paths = []
         self.append_env_path(paths, 'RASPI_HOME')
         self.append_env_path(paths, 'RASPBERRY_HOME')
         if System.windows: paths += ['/SysGCC/raspberry']
         elif System.linux: paths += ['/usr/bin/raspberry', '/usr/local/bin/raspberry', '/opt/raspberry']
         compiler = ''
@@ -556,32 +539,24 @@
                 if self.print: console(f'Found RASPI TOOLS: {self.raspi_compilers}\n    sysroot: {self.raspi_system}')
                 return
         raise EnvironmentError(f'''No Raspberry PI toolchain compilers detected! 
 Default search paths: {paths} 
 Define env RASPI_HOME with path to Raspberry tools.''')
 
 
-    def init_oclea_path(self):
-        if not System.linux: raise RuntimeError('Oclea only supported on Linux')
-        paths = []
-        self.append_env_path(paths, 'OCLEA_HOME')
-        self.append_env_path(paths, 'OCLEA_SDK')
-        if System.linux: paths += ['/usr/bin/oclea', '/usr/local/bin/oclea']
-        compiler = ''
-        if System.linux: compiler = 'x86_64-ocleasdk-linux/usr/bin/aarch64-oclea-linux/aarch64-oclea-linux-gcc'
-        for oclea_path in paths:
-            if os.path.exists(f'{oclea_path}/{compiler}'):
-                self.oclea_compilers = f'{oclea_path}/x86_64-ocleasdk-linux/usr/bin/aarch64-oclea-linux/'
-                self.oclea_system    = f'{oclea_path}/x86_64-ocleasdk-linux/usr/lib'
-                self.oclea_include_paths = [f'{oclea_path}/aarch64-oclea-linux/usr/include']
-                if self.print: console(f'Found Oclea TOOLS: {self.oclea_compilers}\n    sysroot: {self.oclea_system}')
-                return
-        raise EnvironmentError(f'''No Oclea toolchain compilers detected! 
-Default search paths: {paths} 
-Define env OCLEA_HOME with path to Oclea tools.''')
+    def set_oclea_toolchain(self, toolchain_dir):
+        """
+        Sets the oclea toolchain root directory, where
+        aarch64-oclea-linux/
+        x86_64-ocleasdk-linux/
+        directories exist.
+        """
+        if not os.path.exists(toolchain_dir):
+            raise FileNotFoundError(f'Toolchain directory not found: {toolchain_dir}')
+        self.oclea.init_oclea_path(toolchain_dir)
 
 
     def find_default_fortran_compiler(self):
         paths = []
         if System.linux:
             paths += [util.find_executable_from_system('gfortran')]
```

### Comparing `mama-0.7.7/mama/build_dependency.py` & `mama-0.7.9/mama/build_dependency.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
         self.should_rebuild = build
         if conf.list:
             self._print_list(conf, target)
         return build
 
 
     def load_artifactory_package(self, target):
+        # always load during rebuild
         # don't load anything during cleaning, because it will get cleaned anyways
         can_load = self.config.rebuild or not self.config.clean
         load_art = can_load and \
             (self.dep_source.is_pkg or os.path.exists(self.papa_package_file()) or self.is_first_time_build())
         if load_art:
             fetched, dependencies = artifactory_fetch_and_reconfigure(target)
             if fetched:
@@ -483,11 +484,11 @@
     ## Clean
     def clean(self):
         if self.config.print:
             console(f'  - Target {self.name: <16}   CLEAN  {self.config.platform_build_dir_name()}')
 
         if self.build_dir == '/' or not os.path.exists(self.build_dir):
             return
-        
+
         self.target.clean() # Customization point
         shutil.rmtree(self.build_dir, ignore_errors=True)
```

### Comparing `mama-0.7.7/mama/build_target.py` & `mama-0.7.9/mama/build_target.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         self.config = config
         self.name = name
         self.dep  = dep
         self.args = [] # user defined args for this target (must be a list)
         self.install_target = 'install'
         self.cmake_ndk_toolchain   = '' # Custom Android toolchain file for this target only
         self.cmake_raspi_toolchain = '' # Custom Raspberry toolchain file for this target only
-        self.cmake_oclea_toolchain = '' # Custom Oclea toolchain file for this target only
         self.cmake_ios_toolchain   = '' # Custom iOS toolchain file for this target only
         self.cmake_opts       = []
         self.cmake_cxxflags   = dict()
         self.cmake_cflags     = dict()
         self.cmake_ldflags    = dict()
         self.cmake_build_type = 'Debug' if config.debug else 'RelWithDebInfo'
         self.enable_exceptions = True
```

### Comparing `mama-0.7.7/mama/cmake_configure.py` & `mama-0.7.9/mama/cmake_configure.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,17 +161,15 @@
         if target.enable_cxx_build:
             add_flag('-stdlib', 'libc++')
     elif config.raspi:
         add_flag('--sysroot', config.raspi_sysroot())
         for path in config.raspi_includes():
             add_flag(f'-I {path}')
     elif config.oclea:
-        add_flag('--sysroot', config.oclea_sysroot())
-        for path in config.oclea_includes():
-            add_flag(f'-I {path}')
+        config.oclea.get_cxx_flags(add_flag)
 
     if config.flags:
         add_flag(config.flags)
 
     opt = [
         "CMAKE_POSITION_INDEPENDENT_CODE=ON",
         "CMAKE_EXPORT_COMPILE_COMMANDS=ON" # for tools like clang-tidy and .vscode intellisense
@@ -232,27 +230,15 @@
             'CMAKE_FIND_ROOT_PATH_MODE_INCLUDE=ONLY',
         ]
         if target.cmake_raspi_toolchain:
             toolchain = target.source_dir(target.cmake_raspi_toolchain)
             if config.print: console(f'Toolchain: {toolchain}')
             opt += [f'CMAKE_TOOLCHAIN_FILE="{toolchain}"']
     elif config.oclea:
-        opt += [
-            'OCLEA=TRUE',
-            'CMAKE_SYSTEM_NAME=Linux',
-            'CMAKE_SYSTEM_VERSION=1',
-            'CMAKE_SYSTEM_PROCESSOR=arm64',
-            'CMAKE_FIND_ROOT_PATH_MODE_PROGRAM=NEVER', # Use our definitions for compiler tools
-            'CMAKE_FIND_ROOT_PATH_MODE_LIBRARY=ONLY', # Search for libraries and headers in the target directories only
-            'CMAKE_FIND_ROOT_PATH_MODE_INCLUDE=ONLY',
-        ]
-        if target.cmake_oclea_toolchain:
-            toolchain = target.source_dir(target.cmake_oclea_toolchain)
-            if config.print: console(f'Toolchain: {toolchain}')
-            opt += [f'CMAKE_TOOLCHAIN_FILE="{toolchain}"']
+        opt += config.oclea.get_cmake_build_opts()
     elif config.macos:
         pass
     elif config.ios:
         opt += [
             'IOS_PLATFORM=OS',
             'CMAKE_SYSTEM_NAME=Darwin',
             'CMAKE_XCODE_EFFECTIVE_PLATFORMS=-iphoneos',
```

### Comparing `mama-0.7.7/mama/dependency_chain.py` & `mama-0.7.9/mama/dependency_chain.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/init_project.py` & `mama-0.7.9/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/main.py` & `mama-0.7.9/mama/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,17 +205,17 @@
                 if dep.from_artifactory or target.try_automatic_artifactory_fetch():
                     console(f'    Target {target.name} fetched from artifactory')
                 else:
                     target.package()
                 target.print_exports(abs_paths=True)
         return
 
-    if config.android: config.init_ndk_path()
-    if config.raspi:   config.init_raspi_path()
-    if config.oclea:   config.init_oclea_path()
+    if config.android: config.android_home()
+    if config.raspi:   config.raspi_bin()
+    if config.oclea:   config.oclea.bin()
 
     if config.verbose:
         console(f'Executing task chain for build:', Color.BLUE)
     execute_task_chain(root)
 
     if config.open:
         open_project(config, root)
```

### Comparing `mama-0.7.7/mama/msbuild.py` & `mama-0.7.9/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/package.py` & `mama-0.7.9/mama/package.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/papa_deploy.py` & `mama-0.7.9/mama/papa_deploy.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/parse_mamafile.py` & `mama-0.7.9/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/types/artifactory_pkg.py` & `mama-0.7.9/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/types/asset.py` & `mama-0.7.9/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/types/dep_source.py` & `mama-0.7.9/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/types/git.py` & `mama-0.7.9/mama/types/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,22 +203,22 @@
                     for f in files: os.chmod(os.path.join(root, f), stat.S_IWUSR)
             shutil.rmtree(dep.dep_dir)
 
 
     def clone_or_pull(self, dep: BuildDependency, wiped=False):
         if is_dir_empty(dep.src_dir):
             if not wiped and dep.config.print:
-                console(f"  - Target {dep.name: <16}   CLONE because src is missing")
+                console(f"  - Target {dep.name: <16}   CLONE because src is missing", color=Color.BLUE)
             branch = self.branch_or_tag()
             if branch: branch = f" --branch {self.branch_or_tag()}"
             execute(f"git clone --recurse-submodules --depth 1 {branch} {self.url} {dep.src_dir}", dep.config.verbose)
             self.checkout_current_branch(dep)
         else:
             if dep.config.print:
-                console(f"  - Pulling {dep.name: <16}  SCM change detected")
+                console(f"  - Pulling {dep.name: <16}  SCM change detected", color=Color.BLUE)
             self.checkout_current_branch(dep)
             execute("git submodule update --init --recursive")
             if not self.tag: # pull if not a tag
                 self.run_git(dep, "reset --hard -q")
                 self.run_git(dep, "pull")
 
 
@@ -245,12 +245,14 @@
         else:
             # don't pull if no changes to git status
             # or if we're current target of a non-update build
             # mama update target=ReCpp  -- this should git pull
             # mama build target=ReCpp   -- should NOT pull
             non_update_target = is_target and not config.update
             if non_update_target or not changed:
+                if config.verbose:
+                    console(f'    {self.name} git no changes detected and update not specified', color=Color.YELLOW)
                 return False
 
         self.clone_or_pull(dep, wiped)
         return True
```

### Comparing `mama-0.7.7/mama/types/local_source.py` & `mama-0.7.9/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/util.py` & `mama-0.7.9/mama/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import os, sys, shutil, random, pathlib, ssl, zipfile
-from typing import List
-import time
+import os, stat, shutil, zipfile
+from typing import List, Tuple
+import time, ssl, pathlib, random
 from .utils.system import System, console
 from .utils.sub_process import execute
 from urllib import request
 from datetime import datetime, timezone
 
 def is_file_modified(src, dst):
     return os.path.getmtime(src) == os.path.getmtime(dst) and\
@@ -244,59 +244,78 @@
     # report actual percent here, just incase something goes wrong
     elapsed = time.time() - start
     percent = int((transferred / size) * 100.0)
     print(f'\r    |<{"="*50}| {percent:>3}% ({get_time_str(elapsed)})')
     return local_file
 
 
-def get_zipinfo_datetime(zipmember: zipfile.ZipInfo) -> datetime:
-    zt = zipmember.date_time # tuple: year, month, day, hour, min, sec
-    return datetime(zt[0], zt[1], zt[2], zt[3], zt[4], zt[5], tzinfo=timezone.utc)
-
-
-def unzip(local_zip, extract_dir):
+def unzip(local_zip, extract_dir, pwd=None):
     """
-    Attempts to unzip an archive, throws on failure
-    Returns # of files actually extracted
+    Attempts to unzip an archive, throws on failure.
+    Only extracts the files if their current size or modified time mismatches.
+    Always sets modified time from the zipfile info.
+    Preserves symlinks. And sets the correct file permission attributes.
+    Returns # of files actually extracted.
     """
-    with zipfile.ZipFile(local_zip, "r") as zip:
-        members_to_extract: List[zipfile.ZipInfo] = []
-        extracted_filenames: List[str] = []
+    def get_zipinfo_datetime(zipmember: zipfile.ZipInfo) -> datetime:
+        zt = zipmember.date_time # tuple: year, month, day, hour, min, sec
+        return datetime(zt[0], zt[1], zt[2], zt[3], zt[4], zt[5], tzinfo=timezone.utc)
+
+    def has_file_changed(zipmember: zipfile.ZipInfo, dst_path):
+        st: os.stat_result = None
+        try:
+            st = os.stat(dst_path, follow_symlinks=False)
+            if st.st_size != zipmember.file_size:
+                return True
+            dst_mtime: datetime = datetime.fromtimestamp(st.st_mtime, timezone.utc)
+            src_mtime = get_zipinfo_datetime(zipmember)
+            if dst_mtime != src_mtime:
+                return True
+        except (OSError, ValueError):
+            return True # does not exist
+        return False
+
+    def make_symlink(zipmember: zipfile.ZipInfo, symlink_location, is_directory):
+        target = zip.read(zipmember, pwd=pwd).decode('utf-8')
+        if os.path.lexists(symlink_location):
+            os.remove(symlink_location)
+        os.symlink(target, symlink_location, target_is_directory=is_directory)
+
+    unzipped_files: List[Tuple[zipfile.ZipFile, str]] = []
 
+    with zipfile.ZipFile(local_zip, "r") as zip:
         for zipmember in zip.infolist():
-            if zipmember.is_dir():
-                continue
-            dst_path: str = path_join(extract_dir, zipmember.filename)
-            st: os.stat_result = None
-            changed = False
-            try:
-                st = os.stat(dst_path)
-                if st.st_size != zipmember.file_size:
-                    changed = True
+            dst_path = os.path.normpath(os.path.join(extract_dir, zipmember.filename))
+            mode = zipmember.external_attr >> 16
+            is_symlink = stat.S_ISLNK(mode)
+            #what = 'DIR' if zipmember.is_dir() else 'FILE'
+            #what = what + ' LINK' if is_symlink else what
+            #print(f'{what} {zipmember.filename} S_IMODE={stat.S_IMODE(mode):0o} S_IFMT={stat.S_IFMT(mode):0o}')
+            if zipmember.is_dir():  # make dirs if needed
+                if is_symlink:
+                    make_symlink(zipmember, dst_path, is_directory=True)
+                else:
+                    os.makedirs(dst_path, exist_ok=True)
+            elif has_file_changed(zipmember, dst_path):  # only extract if file appears to be modified
+                unzipped_files.append((zipmember, dst_path))
+                if is_symlink:
+                    make_symlink(zipmember, dst_path, is_directory=False)
                 else:
-                    dst_mtime: datetime = datetime.fromtimestamp(st.st_mtime, timezone.utc)
-                    src_mtime = get_zipinfo_datetime(zipmember)
-                    if dst_mtime != src_mtime:
-                        changed = True
-            except (OSError, ValueError):
-                changed = True # does not exist
-            if changed:
-                members_to_extract.append(zipmember)
-                extracted_filenames.append(dst_path)
-
-        zip.extractall(extract_dir, members=members_to_extract)
-
-        # extractall will set time.now() for the modified time, but we need to keep track of it between unpacks
-        # to avoid unnecessarily modifying files and causing full rebuilds
-        # so overwrite the modified time with the zip member time
-        for i in range(len(members_to_extract)):
-            mtime = get_zipinfo_datetime(members_to_extract[i]).timestamp()
-            os.utime(extracted_filenames[i], times=(mtime, mtime))
+                    with zip.open(zipmember, pwd=pwd) as src, open(dst_path, "wb") as dst:
+                        shutil.copyfileobj(src, dst)
+        for zipmember, dst_path in unzipped_files:
+            # set the correct permissions for files and folders
+            perm = stat.S_IMODE(zipmember.external_attr >> 16)
+            os.chmod(dst_path, perm)
+            # always set the modification date from the zipmember timestamp,
+            # this way we can avoid unnecessarily modifying files and causing full rebuilds
+            mtime = get_zipinfo_datetime(zipmember).timestamp()
+            os.utime(dst_path, times=(mtime, mtime), follow_symlinks=False)
 
-        return len(members_to_extract)
+    return len(unzipped_files)
 
 
 def try_unzip(local_file:str, build_dir:str) -> bool:
     """
     Attempts to unzip an archive, returns a tuple (success: bool, num_extracted: int)
     If (success: True, num_extracted: 0) is returned, it means none of the destination files
     were different from the zip contents, and zero extractions were performed
```

### Comparing `mama-0.7.7/mama/utils/nonblocking_io.py` & `mama-0.7.9/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/utils/sub_process.py` & `mama-0.7.9/mama/utils/sub_process.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama/utils/system.py` & `mama-0.7.9/mama/utils/system.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.7/mama.egg-info/PKG-INFO` & `mama-0.7.9/mama.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.7.7
+Version: 0.7.9
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mama-0.7.7/mama.egg-info/SOURCES.txt` & `mama-0.7.9/mama.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 mama/util.py
 mama.egg-info/PKG-INFO
 mama.egg-info/SOURCES.txt
 mama.egg-info/dependency_links.txt
 mama.egg-info/entry_points.txt
 mama.egg-info/requires.txt
 mama.egg-info/top_level.txt
+mama/platforms/__init__.py
+mama/platforms/oclea.py
 mama/types/__init__.py
 mama/types/artifactory_pkg.py
 mama/types/asset.py
 mama/types/dep_source.py
 mama/types/git.py
 mama/types/local_source.py
 mama/utils/__init__.py
```

### Comparing `mama-0.7.7/pyproject.toml` & `mama-0.7.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.7.7"
+version = "0.7.9"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
```

