# Comparing `tmp/pytest-sqlalchemy-session-0.1.10b1.tar.gz` & `tmp/pytest-sqlalchemy-session-0.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sqlalchemy-session-0.1.10b1.tar", last modified: Wed Apr 19 19:33:33 2023, max compression
+gzip compressed data, was "pytest-sqlalchemy-session-0.2.0b1.tar", last modified: Sat Apr 29 11:03:46 2023, max compression
```

## Comparing `pytest-sqlalchemy-session-0.1.10b1.tar` & `pytest-sqlalchemy-session-0.2.0b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:33:33.112866 pytest-sqlalchemy-session-0.1.10b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 19:33:33.112866 pytest-sqlalchemy-session-0.1.10b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:33:33.112866 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-19 19:33:33.000000 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-19 19:33:33.000000 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:33:33.000000 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-19 19:33:33.000000 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 19:33:33.000000 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-19 19:33:33.000000 pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:33:33.112866 pytest-sqlalchemy-session-0.1.10b1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-19 19:33:33.112866 pytest-sqlalchemy-session-0.1.10b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:33:33.112866 pytest-sqlalchemy-session-0.1.10b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/tests/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-19 19:33:23.000000 pytest-sqlalchemy-session-0.1.10b1/tests/test_sqlalchemy_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-29 11:03:46.000000 pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-29 11:03:46.625712 pytest-sqlalchemy-session-0.2.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:03:46.621713 pytest-sqlalchemy-session-0.2.0b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/tests/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-29 11:03:38.000000 pytest-sqlalchemy-session-0.2.0b1/tests/test_strict_mode.py
```

### Comparing `pytest-sqlalchemy-session-0.1.10b1/LICENSE` & `pytest-sqlalchemy-session-0.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-session-0.1.10b1/PKG-INFO` & `pytest-sqlalchemy-session-0.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.1.10b1
+Version: 0.2.0b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.1.10b1/pyproject.toml` & `pytest-sqlalchemy-session-0.2.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pytest-sqlalchemy-session'
-version = "0.1.10-beta1"
+version = "0.2.0-beta1"
 authors = [
     {name = "Stanislav Shkitin", email = "stanislav.shkitin@yandex.ru"},
 ]
 license = {text = "MIT"}
 description = "A pytest plugin for preserving test isolation that use SQLAlchemy."
 keywords = ["pytest", "sqlalchemy", "transaction"]
 readme = "README.md"
@@ -38,16 +38,7 @@
 dependencies = {file = ["requirements/base.txt"]}
 
 [tool.setuptools]
 py-modules = ["pytest_sqlalchemy_session"]
 
 [project.entry-points.pytest11]
 pytest-sqlalchemy-session = "pytest_sqlalchemy_session.plugin"
-
-[tool.cibuildwheel]
-build = "cp3[89]* cp310* cp311*"
-
-[tool.cibuildwheel.macos]
-archs = "x86_64 universal2"
-
-[tool.cibuildwheel.linux]
-archs = "auto aarch64"
```

### Comparing `pytest-sqlalchemy-session-0.1.10b1/pytest_sqlalchemy_session.egg-info/PKG-INFO` & `pytest-sqlalchemy-session-0.2.0b1/pytest_sqlalchemy_session.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-sqlalchemy-session
-Version: 0.1.10b1
+Version: 0.2.0b1
 Summary: A pytest plugin for preserving test isolation that use SQLAlchemy.
 Author-email: Stanislav Shkitin <stanislav.shkitin@yandex.ru>
 License: MIT
 Keywords: pytest,sqlalchemy,transaction
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-sqlalchemy-session-0.1.10b1/setup.cfg` & `pytest-sqlalchemy-session-0.2.0b1/setup.cfg`

 * *Files identical despite different names*

