# Comparing `tmp/LordNzb-2023.3.11.tar.gz` & `tmp/LordNzb-2023.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LordNzb-2023.3.11.tar", last modified: Sat Mar 11 18:58:21 2023, max compression
+gzip compressed data, was "LordNzb-2023.4.29.tar", last modified: Sat Apr 29 21:45:04 2023, max compression
```

## Comparing `LordNzb-2023.3.11.tar` & `LordNzb-2023.4.29.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-11 18:58:21.293758 LordNzb-2023.3.11/
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-11 18:58:21.291120 LordNzb-2023.3.11/LordNzb/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       30 2022-12-04 19:39:17.000000 LordNzb-2023.3.11/LordNzb/__init__.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-11 18:58:21.293139 LordNzb-2023.3.11/LordNzb/core/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     5019 2023-03-11 18:55:38.000000 LordNzb-2023.3.11/LordNzb/core/__init__.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      268 2022-11-18 17:40:40.000000 LordNzb-2023.3.11/LordNzb/core/descriptor.py
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      378 2022-10-20 13:00:08.000000 LordNzb-2023.3.11/LordNzb/core/reg.py
-drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-03-11 18:58:21.292230 LordNzb-2023.3.11/LordNzb.egg-info/
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1437 2023-03-11 18:58:21.000000 LordNzb-2023.3.11/LordNzb.egg-info/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      271 2023-03-11 18:58:21.000000 LordNzb-2023.3.11/LordNzb.egg-info/SOURCES.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-03-11 18:58:21.000000 LordNzb-2023.3.11/LordNzb.egg-info/dependency_links.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        6 2023-03-11 18:58:21.000000 LordNzb-2023.3.11/LordNzb.egg-info/requires.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)        8 2023-03-11 18:58:21.000000 LordNzb-2023.3.11/LordNzb.egg-info/top_level.txt
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1437 2023-03-11 18:58:21.293599 LordNzb-2023.3.11/PKG-INFO
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      850 2022-12-04 19:39:16.000000 LordNzb-2023.3.11/README.rst
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)      665 2023-03-11 18:35:31.000000 LordNzb-2023.3.11/pyproject.toml
--rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-03-11 18:58:21.293797 LordNzb-2023.3.11/setup.cfg
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-04-29 21:45:04.289662 LordNzb-2023.4.29/
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-04-29 21:45:04.286634 LordNzb-2023.4.29/LordNzb/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       30 2022-12-04 19:39:17.000000 LordNzb-2023.4.29/LordNzb/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1108 2023-04-29 19:45:13.000000 LordNzb-2023.4.29/LordNzb/cli.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-04-29 21:45:04.289048 LordNzb-2023.4.29/LordNzb/core/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     5045 2023-04-29 19:14:05.000000 LordNzb-2023.4.29/LordNzb/core/__init__.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      268 2022-11-18 17:40:40.000000 LordNzb-2023.4.29/LordNzb/core/descriptor.py
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      378 2022-10-20 13:00:08.000000 LordNzb-2023.4.29/LordNzb/core/reg.py
+drwxr-xr-x   0 philippkitzmuller   (501) staff       (20)        0 2023-04-29 21:45:04.287920 LordNzb-2023.4.29/LordNzb.egg-info/
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1437 2023-04-29 21:45:04.000000 LordNzb-2023.4.29/LordNzb.egg-info/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      320 2023-04-29 21:45:04.000000 LordNzb-2023.4.29/LordNzb.egg-info/SOURCES.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        1 2023-04-29 21:45:04.000000 LordNzb-2023.4.29/LordNzb.egg-info/dependency_links.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       45 2023-04-29 21:45:04.000000 LordNzb-2023.4.29/LordNzb.egg-info/entry_points.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        6 2023-04-29 21:45:04.000000 LordNzb-2023.4.29/LordNzb.egg-info/requires.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)        8 2023-04-29 21:45:04.000000 LordNzb-2023.4.29/LordNzb.egg-info/top_level.txt
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)     1437 2023-04-29 21:45:04.289440 LordNzb-2023.4.29/PKG-INFO
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      850 2022-12-04 19:39:16.000000 LordNzb-2023.4.29/README.rst
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)      688 2023-04-29 21:44:59.000000 LordNzb-2023.4.29/pyproject.toml
+-rw-r--r--   0 philippkitzmuller   (501) staff       (20)       38 2023-04-29 21:45:04.289717 LordNzb-2023.4.29/setup.cfg
```

### Comparing `LordNzb-2023.3.11/LordNzb/core/__init__.py` & `LordNzb-2023.4.29/LordNzb/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,25 +162,27 @@
     _th = ele.attrib['subject']
     _th = m_reg_Head(_th)
     if not _th is None:
         header = _th['val']
 
     # get Group
 
-    group = []
+    group = set()
 
     ns = regXMLNS.search(root.tag)
     if ns is not None:
         ns = ns.group(0)
     else:
         ns = ""
-    groups = ele.findall(".//" + ns + "group")
+    groups = root.findall(".//" + ns + "group")
 
     for g in groups:
-        group.append(g.text)
+        group.add(g.text)
+
+    group = list(group)
 
     # Date
 
     dateTime = None
     _eleDate = root.find(".//*[@date]")
     if _eleDate is not None:
         dateTime = int(_eleDate.attrib['date'])
```

### Comparing `LordNzb-2023.3.11/LordNzb.egg-info/PKG-INFO` & `LordNzb-2023.4.29/LordNzb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LordNzb
-Version: 2023.3.11
+Version: 2023.4.29
 Summary: Nzb parser Lib für python
 Author-email: lordbex <lordibex@protonmail.com>
 Maintainer-email: lordbex <lordibex@protonmail.com>
 Project-URL: homepage, https://github.com/BexWorld/LordNzb
 Project-URL: repository, https://github.com/BexWorld/LordNzb
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `LordNzb-2023.3.11/PKG-INFO` & `LordNzb-2023.4.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LordNzb
-Version: 2023.3.11
+Version: 2023.4.29
 Summary: Nzb parser Lib für python
 Author-email: lordbex <lordibex@protonmail.com>
 Maintainer-email: lordbex <lordibex@protonmail.com>
 Project-URL: homepage, https://github.com/BexWorld/LordNzb
 Project-URL: repository, https://github.com/BexWorld/LordNzb
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `LordNzb-2023.3.11/README.rst` & `LordNzb-2023.4.29/README.rst`

 * *Files identical despite different names*

### Comparing `LordNzb-2023.3.11/pyproject.toml` & `LordNzb-2023.4.29/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [project]
 name = "LordNzb"
-version = "2023.03.11"
+version = "2023.4.29"
 description = "Nzb parser Lib für python"
 readme = "README.rst"
 requires-python = ">=3.10"
 keywords = []
-authors = [
-    { email = "lordibex@protonmail.com", name = "lordbex" },
-]
-maintainers = [
-    { email = "lordibex@protonmail.com", name = "lordbex" },
-]
-classifiers = [
-    'Operating System :: OS Independent', 'Programming Language :: Python',
-    'Programming Language :: Python :: 3.10',
-    'Topic :: Software Development :: Libraries :: Python Modules'
-]
+classifiers = [ "Operating System :: OS Independent", "Programming Language :: Python", "Programming Language :: Python :: 3.10", "Topic :: Software Development :: Libraries :: Python Modules",]
+dependencies = [ "regex",]
+[[project.authors]]
+email = "lordibex@protonmail.com"
+name = "lordbex"
 
-dependencies = [
-    'regex'
-]
+[[project.maintainers]]
+email = "lordibex@protonmail.com"
+name = "lordbex"
 
 [project.urls]
 homepage = "https://github.com/BexWorld/LordNzb"
 repository = "https://github.com/BexWorld/LordNzb"
+
+[project.scripts]
+lordnzb = "LordNzb.cli:main"
```

