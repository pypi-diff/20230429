# Comparing `tmp/tox_backtocks-0.3.2.tar.gz` & `tmp/tox_backtocks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tox_backtocks-0.3.2.tar", max compression
+gzip compressed data, was "tox_backtocks-0.4.0.tar", max compression
```

## Comparing `tox_backtocks-0.3.2.tar` & `tox_backtocks-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0    26526 2023-03-05 18:12:43.890918 tox_backtocks-0.3.2/LICENSE
--rw-r--r--   0        0        0     2056 2023-03-15 19:25:15.686049 tox_backtocks-0.3.2/README.md
--rw-r--r--   0        0        0     1046 2023-03-15 19:25:37.611774 tox_backtocks-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2177 2023-03-15 19:22:11.199369 tox_backtocks-0.3.2/tox_backtocks/__init__.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 tox_backtocks-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-03-05 18:12:43.890918 tox_backtocks-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2056 2023-04-29 18:00:25.400295 tox_backtocks-0.4.0/README.md
+-rw-r--r--   0        0        0     1046 2023-04-29 18:19:56.626749 tox_backtocks-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1035 2023-04-29 18:19:37.066906 tox_backtocks-0.4.0/tox_backtocks/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-29 18:19:37.067906 tox_backtocks-0.4.0/tox_backtocks/backquote.py
+-rw-r--r--   0        0        0     1010 2023-04-29 18:19:37.067906 tox_backtocks-0.4.0/tox_backtocks/setenv.py
+-rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 tox_backtocks-0.4.0/PKG-INFO
```

### Comparing `tox_backtocks-0.3.2/LICENSE` & `tox_backtocks-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_backtocks-0.3.2/README.md` & `tox_backtocks-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tox_backtocks-0.3.2/pyproject.toml` & `tox_backtocks-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tox-backtocks"
-version = "0.3.2"
+version = "0.4.0"
 description = ""
 authors = ["Damien Nadé <anvil.github+tox-backtocks@livna.org>"]
 license = "LGPL-2.1-or-later"
 repository = "https://github.com/Anvil/tox-backtocks/"
 readme = "README.md"
 keywords = ["tox", "backtocks", "backticks", "backquotes"]
 documentation = "https://github.com/Anvil/tox-backtocks/"
```

### Comparing `tox_backtocks-0.3.2/tox_backtocks/__init__.py` & `tox_backtocks-0.4.0/tox_backtocks/backquote.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-"""A tox plugin that allows backquote expansion in set_env section.
-"""
+"""Functions related to backquotes detection and evaluation"""
 
-from typing import Callable, Any
 
-from tox.config.cli.parser import ToxParser
-from tox.config.sets import EnvConfigSet
-from tox.execute.api import Outcome, StdinSource
-from tox.plugin import impl
-from tox.session.state import State
-from tox.tox_env.api import ToxEnv
+from typing import Any
+from collections.abc import Callable, Iterator
 
-EvalFunc = Callable[[ToxEnv, str, str], str]
+from tox.tox_env.api import ToxEnv
+from tox.execute.api import StdinSource
+from .setenv import set_env_items
 
 
 SHELL = "bash"
 
+EvalFunc = Callable[[ToxEnv, str, str], str]
+
 
 def eval_cache_decorator(func: EvalFunc) -> EvalFunc:
     """A cache decorator for eval_backquote"""
 
     cache: dict[Any, str] = {}
 
     def _function(tox_env: ToxEnv, cmd: str, var: str) -> str:
@@ -45,28 +43,11 @@
 @eval_cache_decorator
 def eval_backquote(tox_env: ToxEnv, cmd: str, var: str) -> str:
     """Evaluate a command inside a tox environment"""
     outcome = tox_env.execute([SHELL, "-c", cmd], StdinSource.OFF, run_id=f"backtocks[{var}]")
     return outcome.out.rstrip('\r\n')
 
 
-# pylint: disable=protected-access
-
-@impl
-def tox_add_env_config(env_conf: EnvConfigSet, state: State) -> None:
-    """Post process config after parsing."""
-    # pylint: disable=unused-argument
-    set_env = env_conf["set_env"]
-    for _, value in set_env._raw.items():
-        if has_backticks(value):
-            # Add bash in order to be able to evaluate backquotes.
-            env_conf["allowlist_externals"].append(SHELL)
-            return
-
-
-@impl
-def tox_before_run_commands(tox_env: ToxEnv) -> None:
-    """Eval and replace backquotes expressions"""
-    set_env = tox_env.conf["set_env"]
-    for var, value in set_env._materialized.items():
+def set_env_backquote_items(self) -> Iterator[tuple[str, str]]:
+    for var, value in set_env_items(self):
         if cmd := has_backticks(value):
-            set_env.update({var: eval_backquote(tox_env, cmd, var)})
+            yield var, cmd
```

### Comparing `tox_backtocks-0.3.2/PKG-INFO` & `tox_backtocks-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tox-backtocks
-Version: 0.3.2
+Version: 0.4.0
 Summary: 
 Home-page: https://github.com/Anvil/tox-backtocks/
 License: LGPL-2.1-or-later
 Keywords: tox,backtocks,backticks,backquotes
 Author: Damien Nadé
 Author-email: anvil.github+tox-backtocks@livna.org
 Requires-Python: >=3.10,<4.0
```

