# Comparing `tmp/pyproject_fmt-0.9.1.tar.gz` & `tmp/pyproject_fmt-0.9.2.tar.gz`

## Comparing `pyproject_fmt-0.9.1.tar` & `pyproject_fmt-0.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/__init__.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/_version.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/py.typed
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/__init__.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/build_system.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/config.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/pep508.py
--rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/project.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/tools.py
--rw-r--r--   0        0        0     3769 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/util.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/test_cli.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/test_main.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/test_pyproject_toml_fmt.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/formatter/conftest.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/formatter/test_build_system.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/formatter/test_pep508.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/formatter/test_project.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/tests/formatter/test_tools.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/LICENSE.txt
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/README.md
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/__init__.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/_version.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/py.typed
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/__init__.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/build_system.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/config.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/pep508.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/project.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/tools.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/util.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/test_cli.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/test_main.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/test_pyproject_toml_fmt.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/formatter/conftest.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/formatter/test_build_system.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/formatter/test_pep508.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/formatter/test_project.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/tests/formatter/test_tools.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/LICENSE.txt
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/README.md
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 pyproject_fmt-0.9.2/PKG-INFO
```

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/__main__.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/cli.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/__init__.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/build_system.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/build_system.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/config.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/pep508.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/pep508.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/project.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/project.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/tools.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/tools.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/src/pyproject_fmt/formatter/util.py` & `pyproject_fmt-0.9.2/src/pyproject_fmt/formatter/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Any, Callable, Sequence
 
 from tomlkit.container import OutOfOrderTableProxy
 from tomlkit.items import (
     AbstractTable,
+    AoT,
     Array,
     Comment,
     Item,
     Key,
     String,
     Table,
     Trivia,
@@ -104,16 +105,23 @@
         )
         body.append(group)
     body.append(_ArrayItemGroup(indent=Whitespace("\n")))
 
 
 def ensure_newline_at_end(body: Table) -> None:
     content = body
-    while content.value.body and isinstance(content.value.body[-1][1], Table):
-        content = content.value.body[-1][1]
+    while True:
+        if isinstance(content, AoT) and content.value and isinstance(content[-1], (AoT, Table)):
+            content = content[-1]
+        elif isinstance(content, Table) and content.value.body and isinstance(content.value.body[-1][1], (AoT, Table)):
+            content = content.value.body[-1][1]
+        else:  # pragma: no cover
+            # coverage has a bug on python < 3.10, seeing this line as uncovered
+            # https://github.com/nedbat/coveragepy/issues/1480
+            break
     whitespace = Whitespace("\n")
     insert_body = content.value.body
     if insert_body and isinstance(insert_body[-1][1], Whitespace):
         insert_body[-1] = insert_body[-1][0], whitespace
     else:
         insert_body.append((None, whitespace))
```

### Comparing `pyproject_fmt-0.9.1/tests/test_cli.py` & `pyproject_fmt-0.9.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/tests/test_main.py` & `pyproject_fmt-0.9.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/tests/formatter/conftest.py` & `pyproject_fmt-0.9.2/tests/formatter/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/tests/formatter/test_build_system.py` & `pyproject_fmt-0.9.2/tests/formatter/test_build_system.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/tests/formatter/test_pep508.py` & `pyproject_fmt-0.9.2/tests/formatter/test_pep508.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/tests/formatter/test_project.py` & `pyproject_fmt-0.9.2/tests/formatter/test_project.py`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/LICENSE.txt` & `pyproject_fmt-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/README.md` & `pyproject_fmt-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/pyproject.toml` & `pyproject_fmt-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_fmt-0.9.1/PKG-INFO` & `pyproject_fmt-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject_fmt
-Version: 0.9.1
+Version: 0.9.2
 Summary: Format your pyproject.toml file
 Project-URL: Bug Tracker, https://github.com/tox-dev/pyproject-fmt/issues
 Project-URL: Documentation, https://github.com/tox-dev/pyproject-fmt/
 Project-URL: Source Code, https://github.com/tox-dev/pyproject-fmt
 Project-URL: Changelog, https://github.com/tox-dev/pyproject-fmt/releases
 Author-email: Bernat Gabor <gaborjbernat@gmail.com>
 License: Permission is hereby granted, free of charge, to any person obtaining a
```

