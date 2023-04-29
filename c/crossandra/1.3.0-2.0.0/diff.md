# Comparing `tmp/crossandra-1.3.0.tar.gz` & `tmp/crossandra-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossandra-1.3.0.tar", last modified: Tue Mar  7 19:50:31 2023, max compression
+gzip compressed data, was "crossandra-2.0.0.tar", last modified: Sat Apr 29 17:52:27 2023, max compression
```

## Comparing `crossandra-1.3.0.tar` & `crossandra-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 19:50:31.819134 crossandra-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-07 19:50:12.000000 crossandra-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-03-07 19:50:31.819134 crossandra-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-03-07 19:50:12.000000 crossandra-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 19:50:31.815134 crossandra-1.3.0/crossandra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-03-07 19:50:31.000000 crossandra-1.3.0/crossandra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-07 19:50:31.000000 crossandra-1.3.0/crossandra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 19:50:31.000000 crossandra-1.3.0/crossandra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-07 19:50:31.000000 crossandra-1.3.0/crossandra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-07 19:50:31.000000 crossandra-1.3.0/crossandra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-07 19:50:12.000000 crossandra-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 19:50:31.819134 crossandra-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-07 19:50:12.000000 crossandra-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 19:50:31.815134 crossandra-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 19:50:31.819134 crossandra-1.3.0/src/crossandra/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-07 19:50:12.000000 crossandra-1.3.0/src/crossandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-07 19:50:12.000000 crossandra-1.3.0/src/crossandra/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-07 19:50:12.000000 crossandra-1.3.0/src/crossandra/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-03-07 19:50:12.000000 crossandra-1.3.0/src/crossandra/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:52:27.181537 crossandra-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-29 17:52:13.000000 crossandra-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-29 17:52:27.181537 crossandra-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-29 17:52:13.000000 crossandra-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-29 17:52:13.000000 crossandra-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 17:52:27.181537 crossandra-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 17:52:13.000000 crossandra-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:52:27.177537 crossandra-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:52:27.181537 crossandra-2.0.0/src/crossandra/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-29 17:52:13.000000 crossandra-2.0.0/src/crossandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-04-29 17:52:13.000000 crossandra-2.0.0/src/crossandra/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-29 17:52:13.000000 crossandra-2.0.0/src/crossandra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-04-29 17:52:13.000000 crossandra-2.0.0/src/crossandra/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-04-29 17:52:13.000000 crossandra-2.0.0/src/crossandra/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 17:52:27.181537 crossandra-2.0.0/src/crossandra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-29 17:52:27.000000 crossandra-2.0.0/src/crossandra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-29 17:52:27.000000 crossandra-2.0.0/src/crossandra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 17:52:27.000000 crossandra-2.0.0/src/crossandra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 17:52:27.000000 crossandra-2.0.0/src/crossandra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-29 17:52:27.000000 crossandra-2.0.0/src/crossandra.egg-info/top_level.txt
```

### Comparing `crossandra-1.3.0/LICENSE` & `crossandra-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crossandra-1.3.0/pyproject.toml` & `crossandra-2.0.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 [project]
 name = "crossandra"
-version = "1.3.0"
+version = "2.0.0"
 description = "A simple tokenizer operating on enums with a decent amount of configuration"
 authors = [{ email = "trag1c <trag1cdev@yahoo.com>" }]
 license = { text = "MIT" }
 urls = { repository = "https://github.com/trag1c/crossandra" }
 readme = "README.md"
-requires-python = ">=3.9"
-dependencies = ["result ~= 0.8.0"]
+requires-python = ">=3.8"
+dependencies = ["result ~= 0.9.0"]
+
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["crossandra*"]
 
 [tool.cibuildwheel.linux]
 archs = ["auto", "aarch64"]
 
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "universal2"]
 
+[tool.ruff]
+target-version = "py38"
+
+[tool.mypy]
+exclude = ["tests/*"]
+
 [build-system]
-requires = ["setuptools", "mypy", "result ~= 0.8.0" ]
+requires = ["setuptools", "mypy", "result ~= 0.9.0"]
 build-backend = "setuptools.build_meta"
```

