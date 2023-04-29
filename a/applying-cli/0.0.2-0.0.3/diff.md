# Comparing `tmp/applying-cli-0.0.2.tar.gz` & `tmp/applying-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/john/PycharmProjects/apl-cli/dist/.tmp-bz23lb_t/applying-cli-0.0.2.tar", last modified: Sat Apr 29 05:08:02 2023, max compression
+gzip compressed data, was "/home/john/PycharmProjects/apl-cli/dist/.tmp-rsedk79z/applying-cli-0.0.3.tar", last modified: Sat Apr 29 05:32:23 2023, max compression
```

## Comparing `applying-cli-0.0.2.tar` & `applying-cli-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:08:02.000000 applying-cli-0.0.2/
--rw-r--r--   0 john      (1000) john      (1000)     1069 2023-04-29 04:32:34.000000 applying-cli-0.0.2/LICENSE.txt
--rw-r--r--   0 john      (1000) john      (1000)      483 2023-04-29 05:08:02.000000 applying-cli-0.0.2/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-29 04:23:54.000000 applying-cli-0.0.2/README.md
--rw-r--r--   0 john      (1000) john      (1000)       85 2023-04-29 04:34:14.000000 applying-cli-0.0.2/pyproject.toml
--rw-r--r--   0 john      (1000) john      (1000)      605 2023-04-29 05:08:02.000000 applying-cli-0.0.2/setup.cfg
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying/
--rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-29 04:15:55.000000 applying-cli-0.0.2/src/applying/__init__.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying/cloudformation/
--rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-29 05:03:23.000000 applying-cli-0.0.2/src/applying/cloudformation/__init__.py
--rw-r--r--   0 john      (1000) john      (1000)       64 2023-04-29 05:04:29.000000 applying-cli-0.0.2/src/applying/cloudformation/project.py
-drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying_cli.egg-info/
--rw-r--r--   0 john      (1000) john      (1000)      483 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying_cli.egg-info/PKG-INFO
--rw-r--r--   0 john      (1000) john      (1000)      310 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying_cli.egg-info/SOURCES.txt
--rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying_cli.egg-info/dependency_links.txt
--rw-r--r--   0 john      (1000) john      (1000)        9 2023-04-29 05:08:02.000000 applying-cli-0.0.2/src/applying_cli.egg-info/top_level.txt
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:32:23.000000 applying-cli-0.0.3/
+-rw-r--r--   0 john      (1000) john      (1000)     1069 2023-04-29 04:32:34.000000 applying-cli-0.0.3/LICENSE.txt
+-rw-r--r--   0 john      (1000) john      (1000)      483 2023-04-29 05:32:23.000000 applying-cli-0.0.3/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-29 04:23:54.000000 applying-cli-0.0.3/README.md
+-rw-r--r--   0 john      (1000) john      (1000)       85 2023-04-29 04:34:14.000000 applying-cli-0.0.3/pyproject.toml
+-rw-r--r--   0 john      (1000) john      (1000)      605 2023-04-29 05:32:23.000000 applying-cli-0.0.3/setup.cfg
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying/
+-rw-r--r--   0 john      (1000) john      (1000)        0 2023-04-29 04:15:55.000000 applying-cli-0.0.3/src/applying/__init__.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying/cloudformation/
+-rw-r--r--   0 john      (1000) john      (1000)       18 2023-04-29 05:23:05.000000 applying-cli-0.0.3/src/applying/cloudformation/__init__.py
+-rw-r--r--   0 john      (1000) john      (1000)       64 2023-04-29 05:04:29.000000 applying-cli-0.0.3/src/applying/cloudformation/project.py
+drwxr-xr-x   0 john      (1000) john      (1000)        0 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying_cli.egg-info/
+-rw-r--r--   0 john      (1000) john      (1000)      483 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying_cli.egg-info/PKG-INFO
+-rw-r--r--   0 john      (1000) john      (1000)      310 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 john      (1000) john      (1000)        1 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 john      (1000) john      (1000)        9 2023-04-29 05:32:23.000000 applying-cli-0.0.3/src/applying_cli.egg-info/top_level.txt
```

### Comparing `applying-cli-0.0.2/LICENSE.txt` & `applying-cli-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `applying-cli-0.0.2/setup.cfg` & `applying-cli-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = applying-cli
-version = 0.0.2
+version = 0.0.3
 author = john velasquez
 author_email = javv.92@gmail.com
 description = Command Line Interface for Applying projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.google.com
 project_urls =
```

