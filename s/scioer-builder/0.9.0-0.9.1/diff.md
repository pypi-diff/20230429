# Comparing `tmp/scioer-builder-0.9.0.tar.gz` & `tmp/scioer-builder-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scioer-builder-0.9.0.tar", last modified: Sun Oct 23 01:12:00 2022, max compression
+gzip compressed data, was "scioer-builder-0.9.1.tar", last modified: Sun Oct 23 01:21:37 2022, max compression
```

## Comparing `scioer-builder-0.9.0.tar` & `scioer-builder-0.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:12:00.752322 scioer-builder-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    21681 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-10-23 01:12:00.752322 scioer-builder-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4529 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:12:00.752322 scioer-builder-0.9.0/builder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/builder/__version__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    34968 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/builder/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:12:00.752322 scioer-builder-0.9.0/builder/data/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/builder/data/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/builder/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/builder/data/motd.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/builder/prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      194 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      936 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/pytype.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-23 01:11:42.000000 scioer-builder-0.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:12:00.752322 scioer-builder-0.9.0/scioer_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/scioer_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      512 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/scioer_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/scioer_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/scioer_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/scioer_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-23 01:12:00.000000 scioer-builder-0.9.0/scioer_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 01:12:00.752322 scioer-builder-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:21:37.048909 scioer-builder-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    22040 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1550 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-10-23 01:21:37.048909 scioer-builder-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4529 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:21:37.048909 scioer-builder-0.9.1/builder/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-23 01:21:36.000000 scioer-builder-0.9.1/builder/__version__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    34968 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/builder/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:21:37.048909 scioer-builder-0.9.1/builder/data/
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/builder/data/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/builder/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/builder/data/motd.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/builder/prompt.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      194 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      936 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/pytype.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-23 01:21:27.000000 scioer-builder-0.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-23 01:21:37.048909 scioer-builder-0.9.1/scioer_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5837 2022-10-23 01:21:37.000000 scioer-builder-0.9.1/scioer_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      512 2022-10-23 01:21:37.000000 scioer-builder-0.9.1/scioer_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-23 01:21:37.000000 scioer-builder-0.9.1/scioer_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-23 01:21:37.000000 scioer-builder-0.9.1/scioer_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-10-23 01:21:37.000000 scioer-builder-0.9.1/scioer_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-23 01:21:37.000000 scioer-builder-0.9.1/scioer_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-23 01:21:37.048909 scioer-builder-0.9.1/setup.cfg
```

### Comparing `scioer-builder-0.9.0/CHANGELOG.md` & `scioer-builder-0.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v0.9.1](https://github.com/sci-oer/automated-builder/releases/v0.9.1) (2022-10-23)
+
+[Full Changelog](https://github.com/sci-oer/automated-builder/compare/v0.9.0...v0.9.1)
+
+**Merged pull requests:**
+
+- fix: remove unsuported buildx platforms [\#164](https://github.com/sci-oer/automated-builder/pull/164) ([MarshallAsch](https://github.com/MarshallAsch))
+
 ## [v0.9.0](https://github.com/sci-oer/automated-builder/releases/v0.9.0) (2022-10-23)
 
 [Full Changelog](https://github.com/sci-oer/automated-builder/compare/v0.8.2...v0.9.0)
 
 **Implemented enhancements:**
 
 - Use docker heath check status instead of polling the wiki to see if the container is ready [\#153](https://github.com/sci-oer/automated-builder/issues/153)
```

### Comparing `scioer-builder-0.9.0/Dockerfile` & `scioer-builder-0.9.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/LICENSE` & `scioer-builder-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/PKG-INFO` & `scioer-builder-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scioer-builder
-Version: 0.9.0
+Version: 0.9.1
 Summary: A cli application to help build custom versions of the sci-oer course container
 Author-email: Marshall Asch <masch@uoguelph.ca>
 Project-URL: Homepage, https://github.com/sci-oer/automated-builder
 Project-URL: Bug Reports, https://github.com/sci-oer/automated-builder/issues
 Project-URL: Funding, https://github.com/sci-oer/automated-builder/blob/main/.github/FUNDING.md
 Project-URL: Documentation, https://github.com/sci-oer/automated-builder/blob/main/README.md
 Project-URL: Source, https://github.com/sci-oer/automated-builder
```

### Comparing `scioer-builder-0.9.0/README.md` & `scioer-builder-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/builder/cli.py` & `scioer-builder-0.9.1/builder/cli.py`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/builder/data/Dockerfile` & `scioer-builder-0.9.1/builder/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/builder/prompt.py` & `scioer-builder-0.9.1/builder/prompt.py`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/pyproject.toml` & `scioer-builder-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/pytype.cfg` & `scioer-builder-0.9.1/pytype.cfg`

 * *Files identical despite different names*

### Comparing `scioer-builder-0.9.0/scioer_builder.egg-info/PKG-INFO` & `scioer-builder-0.9.1/scioer_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scioer-builder
-Version: 0.9.0
+Version: 0.9.1
 Summary: A cli application to help build custom versions of the sci-oer course container
 Author-email: Marshall Asch <masch@uoguelph.ca>
 Project-URL: Homepage, https://github.com/sci-oer/automated-builder
 Project-URL: Bug Reports, https://github.com/sci-oer/automated-builder/issues
 Project-URL: Funding, https://github.com/sci-oer/automated-builder/blob/main/.github/FUNDING.md
 Project-URL: Documentation, https://github.com/sci-oer/automated-builder/blob/main/README.md
 Project-URL: Source, https://github.com/sci-oer/automated-builder
```

### Comparing `scioer-builder-0.9.0/scioer_builder.egg-info/SOURCES.txt` & `scioer-builder-0.9.1/scioer_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

