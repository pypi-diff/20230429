# Comparing `tmp/chef_helper-3.tar.gz` & `tmp/chef_helper-4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chef_helper-3.tar", last modified: Sat Apr 29 14:05:41 2023, max compression
+gzip compressed data, was "chef_helper-4.tar", last modified: Sat Apr 29 14:13:32 2023, max compression
```

## Comparing `chef_helper-3.tar` & `chef_helper-4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:05:41.929628 chef_helper-3/
--rw-r--r--   0 andriiosypenko   (501) staff       (20)     1065 2023-04-23 13:09:21.000000 chef_helper-3/LICENSE
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 14:05:41.928754 chef_helper-3/PKG-INFO
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      442 2023-04-29 11:54:03.000000 chef_helper-3/README.md
-drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:05:41.910534 chef_helper-3/chef_helper.egg-info/
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 14:05:41.000000 chef_helper-3/chef_helper.egg-info/PKG-INFO
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      507 2023-04-29 14:05:41.000000 chef_helper-3/chef_helper.egg-info/SOURCES.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)        1 2023-04-29 14:05:41.000000 chef_helper-3/chef_helper.egg-info/dependency_links.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       54 2023-04-29 14:05:41.000000 chef_helper-3/chef_helper.egg-info/entry_points.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       17 2023-04-29 14:05:41.000000 chef_helper-3/chef_helper.egg-info/requires.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       10 2023-04-29 14:05:41.000000 chef_helper-3/chef_helper.egg-info/top_level.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       38 2023-04-29 14:05:41.930551 chef_helper-3/setup.cfg
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      460 2023-04-29 14:05:17.000000 chef_helper-3/setup.py
-drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:05:41.898765 chef_helper-3/venv/
-drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:05:41.926186 chef_helper-3/venv/bin/
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      643 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2html.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      765 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2html4.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)     1110 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2html5.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      842 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2latex.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      665 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2man.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      831 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2odt.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)     1769 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      650 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      686 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2s5.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      922 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2xetex.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      651 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rst2xml.py
--rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      719 2023-04-29 13:52:05.000000 chef_helper-3/venv/bin/rstpep2html.py
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:13:32.391248 chef_helper-4/
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)     1065 2023-04-23 13:09:21.000000 chef_helper-4/LICENSE
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 14:13:32.390481 chef_helper-4/PKG-INFO
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      442 2023-04-29 11:54:03.000000 chef_helper-4/README.md
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:13:32.363017 chef_helper-4/app/
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)     1089 2023-04-29 14:11:48.000000 chef_helper-4/app/client_app.py
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:13:32.369666 chef_helper-4/chef_helper.egg-info/
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 14:13:32.000000 chef_helper-4/chef_helper.egg-info/PKG-INFO
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      525 2023-04-29 14:13:32.000000 chef_helper-4/chef_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)        1 2023-04-29 14:13:32.000000 chef_helper-4/chef_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       58 2023-04-29 14:13:32.000000 chef_helper-4/chef_helper.egg-info/entry_points.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       17 2023-04-29 14:13:32.000000 chef_helper-4/chef_helper.egg-info/requires.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       14 2023-04-29 14:13:32.000000 chef_helper-4/chef_helper.egg-info/top_level.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       38 2023-04-29 14:13:32.391501 chef_helper-4/setup.cfg
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      464 2023-04-29 14:12:59.000000 chef_helper-4/setup.py
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:13:32.360328 chef_helper-4/venv/
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 14:13:32.388401 chef_helper-4/venv/bin/
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      643 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2html.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      765 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2html4.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)     1110 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2html5.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      842 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2latex.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      665 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2man.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      831 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2odt.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)     1769 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      650 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      686 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2s5.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      922 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      651 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rst2xml.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      719 2023-04-29 13:52:05.000000 chef_helper-4/venv/bin/rstpep2html.py
```

### Comparing `chef_helper-3/LICENSE` & `chef_helper-4/LICENSE`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2html.py` & `chef_helper-4/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2html4.py` & `chef_helper-4/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2html5.py` & `chef_helper-4/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2latex.py` & `chef_helper-4/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2man.py` & `chef_helper-4/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2odt.py` & `chef_helper-4/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2odt_prepstyles.py` & `chef_helper-4/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2pseudoxml.py` & `chef_helper-4/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2s5.py` & `chef_helper-4/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2xetex.py` & `chef_helper-4/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rst2xml.py` & `chef_helper-4/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `chef_helper-3/venv/bin/rstpep2html.py` & `chef_helper-4/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

