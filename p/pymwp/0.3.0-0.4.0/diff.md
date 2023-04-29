# Comparing `tmp/pymwp-0.3.0.tar.gz` & `tmp/pymwp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymwp-0.3.0.tar", last modified: Sat Apr  8 21:13:10 2023, max compression
+gzip compressed data, was "pymwp-0.4.0.tar", last modified: Sat Apr 29 20:56:47 2023, max compression
```

## Comparing `pymwp-0.3.0.tar` & `pymwp-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.935534 pymwp-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 21:12:38.000000 pymwp-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-08 21:12:38.000000 pymwp-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-08 21:13:10.935534 pymwp-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-08 21:12:38.000000 pymwp-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.927534 pymwp-0.3.0/pymwp/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18142 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11278 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/delta_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/monomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    18152 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/relation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-08 21:12:38.000000 pymwp-0.3.0/pymwp/semiring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.931534 pymwp-0.3.0/pymwp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:13:10.000000 pymwp-0.3.0/pymwp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-08 21:12:38.000000 pymwp-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:13:10.935534 pymwp-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-08 21:12:38.000000 pymwp-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.935534 pymwp-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:13:10.935534 pymwp-0.3.0/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/mocks/ast_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_delta_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_file_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_monomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-08 21:12:38.000000 pymwp-0.3.0/tests/test_relation_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 20:56:19.000000 pymwp-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 20:56:19.000000 pymwp-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-29 20:56:47.449555 pymwp-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-29 20:56:19.000000 pymwp-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.445554 pymwp-0.4.0/pymwp/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18891 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10167 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/delta_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18771 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/relation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-04-29 20:56:19.000000 pymwp-0.4.0/pymwp/semiring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/pymwp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 20:56:47.000000 pymwp-0.4.0/pymwp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-29 20:56:19.000000 pymwp-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 20:56:47.449555 pymwp-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-29 20:56:19.000000 pymwp-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 20:56:47.449555 pymwp-0.4.0/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/mocks/ast_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_delta_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_file_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_monomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-29 20:56:19.000000 pymwp-0.4.0/tests/test_relation_list.py
```

### Comparing `pymwp-0.3.0/LICENSE` & `pymwp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/PKG-INFO` & `pymwp-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
@@ -103,26 +103,26 @@
 
 1. Clone the repository
 
     ```
     git clone https://github.com/statycc/pymwp.git
     ``` 
 
-2. Set up Python environment
+2. Set up Python environment (use [`venv`](https://docs.python.org/3/library/venv.html))
 
     install required packages
 
     ```
-    python -m pip install -q -r requirements.txt
+    python -m pip install -r requirements.txt
     ``` 
     
-    Note: for development purposes or to run tests, install dev dependencies instead: 
+    Note: for development purposes install dev dependencies instead: 
     
     ```
-    python -m pip install -q -r requirements-dev.txt
+    python -m pip install -r requirements-dev.txt
     ```
 
 3. Run the analysis
 
     From project root run:
     
     ```
```

### Comparing `pymwp-0.3.0/README.md` & `pymwp-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,26 +74,26 @@
 
 1. Clone the repository
 
     ```
     git clone https://github.com/statycc/pymwp.git
     ``` 
 
-2. Set up Python environment
+2. Set up Python environment (use [`venv`](https://docs.python.org/3/library/venv.html))
 
     install required packages
 
     ```
-    python -m pip install -q -r requirements.txt
+    python -m pip install -r requirements.txt
     ``` 
     
-    Note: for development purposes or to run tests, install dev dependencies instead: 
+    Note: for development purposes install dev dependencies instead: 
     
     ```
-    python -m pip install -q -r requirements-dev.txt
+    python -m pip install -r requirements-dev.txt
     ```
 
 3. Run the analysis
 
     From project root run:
     
     ```
```

### Comparing `pymwp-0.3.0/pymwp/__init__.py` & `pymwp-0.4.0/pymwp/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 """
 pymwp: implementation of MWP analysis on C code in Python.
 """
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __license__ = "GPLv3"
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 from pymwp.parser import Parser
 from pymwp.delta_graphs import DeltaGraph
 from pymwp.choice import Choices
+from pymwp.monomial import Monomial
+from pymwp.polynomial import Polynomial
 from pymwp.relation_list import RelationList
 from pymwp.relation import Relation
-from pymwp.polynomial import Polynomial
-from pymwp.monomial import Monomial
+from pymwp.bound import Bound
 from pymwp.result import Result
 from pymwp.analysis import Analysis
-
```

### Comparing `pymwp-0.3.0/pymwp/__main__.py` & `pymwp-0.4.0/pymwp/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     args = __parse_args(parser)
 
     if not args.input_file:
         parser.print_help()
         sys.exit(1)
 
     # setup logger
-    log_level = logging.FATAL - (0 if args.silent else 40)
-    __setup_logger(log_level, args.logfile)
+    log_level = logging.FATAL - (0 if args.silent else 30 if args.info else 40)
+    __setup_logger(log_level, args.logfile, args.no_time)
 
     # capture results
     result = Result()
 
     # get parser args then get AST
     parser_kwargs = {'use_cpp': not args.no_cpp}
     # these options apply only when use_cpp is True
@@ -53,15 +53,15 @@
     ast = Parser.parse(args.input_file, c_headers, **(parser_kwargs or {}))
     result.program.program_path = args.input_file
     result.program.n_lines = loc(args.input_file)
 
     # run analysis
     Analysis.run(
         ast=ast,
-        result=result,
+        res=result,
         file_out=args.out or default_file_out(args.input_file),
         no_save=args.no_save,
         no_eval=args.no_eval,
         fin=args.fin
     )
 
 
@@ -109,47 +109,59 @@
     )
     parser.add_argument(
         "--no_eval",
         action='store_true',
         help="skip evaluation"
     )
     parser.add_argument(
+        "--no_time",
+        action='store_true',
+        help="display log without timestamps"
+    )
+    parser.add_argument(
         "--fin",
         action='store_true',
-        help="ensure completion even on failure"
+        help="ensure analysis completion in all cases"
     )
     parser.add_argument(
         "--logfile",
         action="store",
         help="write console output to a file",
     )
     parser.add_argument(
+        '-i', "--info",
+        action='store_true',
+        help="set logging level to info"
+    )
+    parser.add_argument(
         '-s', "--silent",
         action='store_true',
-        help="disable console output"
+        help="disable all terminal output"
     )
     parser.add_argument(
         "--version",
         action="version",
         version="%(prog)s " + __version__,
     )
     return parser.parse_args(args)
 
 
 def __setup_logger(
-        level: int = logging.ERROR, log_filename: Optional[str] = None
+        level: int = logging.ERROR, log_filename: Optional[str] = None,
+        hide_time: bool = False
 ) -> None:
     """Create a configured instance of logger.
 
     Arguments:
         level: Describe the severity level of the logs to handle.
             see: https://docs.python.org/3/library/logging.html#levels
         log_filename: Write logging info to a file
     """
-    fmt = "[%(asctime)s] %(levelname)s (%(module)s): %(message)s"
+    fmt = "%(levelname)s (%(module)s): %(message)s" if hide_time else \
+        "[%(asctime)s] %(levelname)s (%(module)s): %(message)s"
     date_fmt = "%H:%M:%S"
     formatter = logging.Formatter(fmt, datefmt=date_fmt)
 
     logger = logging.getLogger(pymwp)
     logger.setLevel(level)
 
     stream_handler = logging.StreamHandler()
```

### Comparing `pymwp-0.3.0/pymwp/analysis.py` & `pymwp-0.4.0/pymwp/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 # noinspection DuplicatedCode
 import logging
-from typing import List, Tuple, Optional, Union, Dict
+from typing import List, Tuple, Optional
 
-from .file_io import save_relation
+from .file_io import save_result
 # noinspection PyPep8Naming
 from .parser import Parser as pr
-from pymwp import DeltaGraph, Monomial, Polynomial, RelationList, Result
-from pymwp.result import FUNC_RESULT
+from pymwp import DeltaGraph, Polynomial, RelationList, Result, Bound
+from pymwp.result import FuncResult
 
 logger = logging.getLogger(__name__)
 
 
 class Analysis:
     """MWP analysis implementation."""
 
     @staticmethod
-    def run(ast: pr.AST, result: Result = None, **kwargs) \
-            -> Union[Dict[str, FUNC_RESULT], FUNC_RESULT]:
+    def run(ast: pr.AST, res: Result = None, **kwargs) -> Result:
         """Run MWP analysis on specified input file.
 
         Arguments:
             ast: parsed C source code AST
-            result: (optional) result object
+            res: (optional) pre-initialized result object
 
         Returns:
-            Computed relation, list of non-infinity choices, and
-                infinite/not infinite (boolean flag)
+            A [`Result`](result.md) object.
         """
         file_out: str = kwargs['file_out'] if 'file_out' in kwargs else None
         save: bool = 'no_save' not in kwargs or kwargs['no_save'] is False
         stop_early: bool = 'fin' not in kwargs or kwargs['fin'] is False
         skip_eval: bool = 'no_eval' in kwargs and kwargs['no_eval'] is True
-        result__: Result = result or Result()
+        result: Result = res or Result()
 
         logger.debug("started analysis")
-        result__.on_start()
+        result.on_start()
         for ast_ext in [f for f in ast if pr.is_func(f)]:
-            choices = [0, 1, 2]
-            index, combinations = 0, []
-            function_name = ast_ext.decl.name
+            index, options, choices = 0, [0, 1, 2], []
+            outcome: FuncResult = FuncResult(ast_ext.decl.name).on_start()
+            function_name = outcome.name
             function_body = ast_ext.body
             args = ast_ext.decl.type.args
             variables = Analysis.find_variables(function_body, args)
-            logger.debug(f"variables of {function_name}: {variables}")
-            evaluated = False
+            logger.debug(f"{function_name} variables: {', '.join(variables)}")
+            evaluated, bound = False, None
 
             relations = RelationList.identity(variables=variables)
             total = len(function_body.block_items)
             delta_infty = False
             dg = DeltaGraph()
 
             for i, node in enumerate(function_body.block_items):
                 logger.debug(f'computing relation...{i} of {total}')
-                index, rel_list, delta_infty = Analysis \
+                index, rel_list, delta_infty_ = Analysis \
                     .compute_relation(index, node, dg)
+                delta_infty = delta_infty or delta_infty_  # cannot erase
                 if stop_early and delta_infty:
                     break
                 logger.debug(f'computing composition...{i} of {total}')
                 relations.composition(rel_list)
 
             # evaluate unless not enforcing finish and delta-infty
             if not skip_eval and not delta_infty:
-                combinations = relations.first.eval(choices, index)
+                choices = relations.first.eval(options, index)
+                if not choices.infinite:
+                    bound = Bound().calculate(
+                        relations.first.apply_choice(*choices.first))
                 evaluated = True
 
             # the evaluation is infinite when either of these conditions holds:
             infinite = delta_infty or (
                     relations.first.variables and index > 0 and
-                    evaluated and not combinations.valid)
+                    evaluated and not choices.valid)
 
             # record and display results
-            outcome = function_name,
-            if infinite and stop_early:
-                outcome += (None, None, True)
-            elif infinite:
-                outcome += (relations.first, None, True)
-            else:
-                outcome += (relations.first, combinations, False)
-            result__.add_relation(*outcome)
+            outcome.on_end()
+            outcome.vars = relations.first.variables
+            outcome.infinite = infinite
+            if not (infinite and stop_early):
+                outcome.relation = relations.first
+            if not infinite:
+                outcome.bound = bound
+                outcome.choices = choices
+            result.add_relation(outcome)
 
-        result__.on_end()
-        result__.log_result()
+        result.on_end()
+        result.log_result()
 
         if save:
-            save_relation(file_out, result__.relations)
-        return result__.get_result()
+            save_result(file_out, res)
+        return result
 
     @staticmethod
     def find_variables(
             function_body: pr.Compound, param_list: Optional[pr.ParamList]
     ) -> List[str]:
         """Finds all local variable declarations in function body and
         parameter list.
@@ -145,15 +148,16 @@
 
         logger.debug("in compute_relation")
 
         if isinstance(node, pr.Decl):
             return index, RelationList(), False
         if isinstance(node, pr.FuncCall):
             return Analysis.func_call(index)
-        if isinstance(node, pr.Assignment):
+        if isinstance(node, pr.Assignment) and \
+                isinstance(node.lvalue, pr.ID):
             if isinstance(node.rvalue, pr.BinaryOp):
                 return Analysis.binary_op(index, node)
             if isinstance(node.rvalue, pr.Constant):
                 return Analysis.constant(index, node.lvalue.name)
             if isinstance(node.rvalue, pr.UnaryOp):
                 return Analysis.unary_op(index, node)
             if isinstance(node.rvalue, pr.ID):
@@ -165,57 +169,59 @@
         if isinstance(node, pr.While):
             return Analysis.while_(index, node, dg)
         if isinstance(node, pr.For):
             return Analysis.for_(index, node, dg)
         if isinstance(node, pr.Compound):
             return Analysis.compound_(index, node, dg)
 
-        logger.debug(f"uncovered case! type: {type(node)}")
+        Analysis.unsupported(f"{type(node)}")
 
         return index, RelationList(), False
 
     @staticmethod
     def id(index: int, node: pr.Assignment) \
             -> Tuple[int, RelationList, bool]:
-        """Analyze x = y (with x != y) and y not a const
+        """Analyze x = y, where data flows between two variables.
 
         Arguments:
             index: delta index
             node: AST node representing a simple assignment
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
-        x = node.lvalue.name
-        y = node.rvalue.name
-        if x == y or isinstance(node.rvalue, pr.Constant):
+
+        # ensure we have distinct variables on both sides of x = y
+        if not isinstance(node.lvalue, pr.ID) \
+                or isinstance(node.rvalue, pr.Constant) \
+                or node.lvalue.name == node.rvalue.name:
             return index, RelationList(), False
 
         logger.debug('Computing Relation x = y')
-        vars_list = [[x], [y]]
+        x = node.lvalue.name
+        vars_list = [[x], [node.rvalue.name]]
 
         # create a vector of polynomials based on operator type
         #     x   y
         # x | o   o
         # y | m   m
         vector = [
             # because x != y
-            Polynomial([Monomial('o')]),
-            Polynomial([Monomial('m')])
+            Polynomial('o'), Polynomial('m')
         ]
 
         # build a list of unique variables
         variables = vars_list[0]
         for var in vars_list[1]:
             if var not in variables:
                 variables.append(var)
 
         # create relation list
         rel_list = RelationList.identity(variables)
-        rel_list.replace_column(vector, vars_list[0][0])
+        rel_list.replace_column(vector, x)
 
         return index + 1, rel_list, False
 
     @staticmethod
     def binary_op(index: int, node: pr.Assignment) \
             -> Tuple[int, RelationList, bool]:
         """Analyze binary operation, e.g. `x = y + z`.
@@ -223,29 +229,30 @@
         Arguments:
             index: delta index
             node: AST node representing a binary operation
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
-        logger.debug('Computing Relation (first case / binary op)')
+        logger.debug('Computing Relation (first case, binary op)')
         x, y, z = node.lvalue, node.rvalue.left, node.rvalue.right
         non_constants = tuple([v.name if hasattr(v, 'name') else None
                                for v in [x, y, z]])
 
         # create a vector of polynomials based on operator type
         index, vector = Analysis.create_vector(
             index, node.rvalue.op, non_constants)
 
         # build a list of unique variables but maintain order
         variables = list(dict.fromkeys(non_constants))
 
         # create relation list
         rel_list = RelationList.identity(variables)
-        rel_list.replace_column(vector, x.name)
+        if hasattr(x, 'name'):
+            rel_list.replace_column(vector, x.name)
 
         return index, rel_list, False
 
     @staticmethod
     def constant(index: int, variable_name: str) \
             -> Tuple[int, RelationList, bool]:
         """Analyze a constant assignment of form `x = c` where x is some
@@ -275,17 +282,19 @@
         Arguments:
             index: delta index
             node: unary operator node
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
-        logger.debug('Computing Relation (third case / unary)')
-        var_name = node.lvalue.name
-        variables = [var_name]
+        logger.debug('Computing Relation (third case: unary)')
+        variables = []
+        if hasattr(node.lvalue, 'expr') and \
+                hasattr(node.lvalue.expr, 'name'):
+            variables = [node.lvalue.expr.name]
         return index, RelationList.identity(variables), False
 
     @staticmethod
     def if_(index: int, node: pr.If, dg: DeltaGraph) \
             -> Tuple[int, RelationList, bool]:
         """Analyze an if statement.
 
@@ -380,15 +389,15 @@
         relations.fixpoint()
         relations.while_correction(dg)
         dg.fusion()
 
         exit_ = False
         if 0 in dg.graph_dict:
             if dg.graph_dict[0] == {(): {}}:
-                logger.info('delta_graphs: infinite -> Exit now')
+                logger.debug('delta_graphs: infinite -> Exit now')
                 exit_ = True
 
         return index, relations, exit_
 
     @staticmethod
     def for_(index: int, node: pr.For, dg: DeltaGraph) \
             -> Tuple[int, RelationList, bool]:
@@ -401,15 +410,17 @@
 
         Returns:
             Updated index value, relation list, and an exit flag.
         """
         logger.debug("analysing for:")
 
         relations = RelationList()
-        for child in node.stmt.block_items:
+
+        for child in node.stmt.block_items \
+                if hasattr(node, 'block_items') else [node.stmt]:
             index, rel_list, exit_ = Analysis.compute_relation(
                 index, child, dg)
             if exit_:
                 return index, rel_list, True
             relations.composition(rel_list)
 
         relations.fixpoint()
@@ -463,23 +474,28 @@
                 where `y` or `z` is `None` if constant
 
         Returns:
              Updated index, list of Polynomial vectors
         """
 
         x, y, z = variables
+        supported_op = {"+", "-", "*"}
         vector = []
 
+        if operator not in supported_op:
+            Analysis.unsupported(f'{operator} operator')
+            return index, []
+
         # when left variable does not occur on right side of assignment
         # x = … (if x not in …), i.e. when left side variable does not
         # occur on the right side of assignment, we prepend 0 to vector
         if x != y and x != z:
             vector.append(Polynomial('o'))
 
-        if operator in {"+", "-", "*"} and (y is None or z is None):
+        if operator in supported_op and (y is None or z is None):
             vector.append(Polynomial.from_scalars(index, 'm', 'm', 'm'))
 
         elif operator == '*' and y == z:
             vector.append(Polynomial.from_scalars(index, 'w', 'w', 'w'))
 
         elif operator == '*' and y != z:
             vector.append(Polynomial.from_scalars(index, 'w', 'w', 'w'))
@@ -491,13 +507,16 @@
         elif operator in {'+', '-'} and y != z:
             vector.append(Polynomial.from_scalars(index, 'm', 'p', 'w'))
             vector.append(Polynomial.from_scalars(index, 'p', 'm', 'w'))
 
         return index + 1, vector
 
     @staticmethod
-    def func_call(index: int) \
-            -> Tuple[int, RelationList, bool]:
+    def unsupported(command: any):
+        """Handle unsupported command."""
+        logger.warning(f'Unsupported syntax: {command} -> not evaluated')
+
+    @staticmethod
+    def func_call(index: int) -> Tuple[int, RelationList, bool]:
         """Function call handler stub."""
-        logger.debug('Function call detected!\nThis feature is not yet '
-                     'supported, but will be added soon')
+        Analysis.unsupported('function call')
         return index, RelationList(), False
```

### Comparing `pymwp-0.3.0/pymwp/choice.py` & `pymwp-0.4.0/pymwp/choice.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 from collections import Counter
 from functools import reduce
-from typing import Tuple, List, Set, Union
+from typing import Tuple, List, Set, Union, Optional
 
 logger = logging.getLogger(__name__)
 
 SEQ = Tuple[Tuple[int, int], ...]
 """Type hint to represent a sequence of deltas."""
 
 CHOICES = List[List[List[int]]]
@@ -33,14 +33,28 @@
         """
         self.valid = vectors or []
 
     @property
     def infinite(self):
         return len(self.valid) == 0
 
+    @property
+    def first(self) -> Optional[tuple[int]]:
+        """Gets the first valid derivation choice, if exists"""
+        # take first vector, then first choice at each index
+        return tuple([choices[0] for choices in self.valid[0]]) \
+            if not self.infinite else None
+
+    @property
+    def n_bounds(self) -> int:
+        """Number of bounds that can be generated from a choice vector"""
+        return sum([
+            reduce(lambda total, n: total * (n[0] ** n[1]), lens.items(), 1)
+            for lens in [Counter([len(x) for x in v]) for v in self.valid]])
+
     @staticmethod
     def generate(choices: List[int], index: int, inf: Set[SEQ]) -> Choices:
         """Generate the choice representation.
 
         This works in two steps: 1. simplify delta sequences 2. build
         choice vectors.
```

### Comparing `pymwp-0.3.0/pymwp/delta_graphs.py` & `pymwp-0.4.0/pymwp/delta_graphs.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/pymwp/matrix.py` & `pymwp-0.4.0/pymwp/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         AttributeError: If the matrix elements are not
             valid encoded polynomials.
 
     Returns:
         Decoded matrix of polynomials.
     """
     return [[
-        Polynomial([Monomial(
+        Polynomial(*[Monomial(
             scalar=monomial["scalar"],
             deltas=monomial["deltas"])
             for monomial in polynomial])
         for polynomial in row]
         for (i, row) in enumerate(matrix)]
```

### Comparing `pymwp-0.3.0/pymwp/monomial.py` & `pymwp-0.4.0/pymwp/monomial.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,26 +74,35 @@
         deltas = [".delta({0},{1})".format(*delta)
                   for delta in self.deltas]
         return self.scalar + ''.join(deltas)
 
     def __mul__(self, other) -> Monomial:
         return self.prod(other)
 
+    @staticmethod
+    def format(value: Union[str, Monomial, Tuple]) -> Monomial:
+        if isinstance(value, Monomial):
+            return value
+        if isinstance(value, str):
+            return Monomial(value)
+        if isinstance(value, Tuple):
+            return Monomial(*value)
+
     def contains(self, m: Monomial) -> bool:
         """check if all deltas of m are in deltas of self
 
         Arguments:
             m: a monomial to search for intersection
 
         Returns:
             False if one delta of m not in self
             True otherwise
         """
         for b in m.deltas:
-            if not (b in self.deltas):
+            if b not in self.deltas:
                 return False
         return True
 
     def inclusion(self, monomial: Monomial) -> SetInclusion:
         """gives info about inclusion of self monomial with monomial
 
         Arguments:
@@ -154,14 +163,28 @@
         # the second monomial passed in as argument
         elif monomial.deltas:
             # TODO here insert only those not contained ?
             Monomial.insert_deltas(mono_product, monomial.deltas)
 
         return mono_product
 
+    def choice_scalar(self, *choices: int) -> Optional[str]:
+        """Determine if given sequence of choices matches monomial.
+
+        Arguments:
+            choices: tuple of choices
+
+        Returns:
+            Monomial's scalar if structure matches choices and None otherwise.
+        """
+        for (i, j) in self.deltas:
+            if not i == choices[j]:
+                return None
+        return self.scalar
+
     def copy(self) -> Monomial:
         """Make a deep copy of a monomial."""
         return Monomial(self.scalar, self.deltas[:])
 
     def show(self) -> None:
         """Display scalar and the list of deltas."""
         print(str(self))
```

### Comparing `pymwp-0.3.0/pymwp/parser.py` & `pymwp-0.4.0/pymwp/parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/pymwp/polynomial.py` & `pymwp-0.4.0/pymwp/polynomial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 # flake8: noqa: W605
 
 from __future__ import annotations
 
 import logging
 from typing import Optional, List, Tuple, Union
+from typing import TypeVar
 
 from .constants import Comparison, SetInclusion
-from .monomial import Monomial
+from .monomial import Monomial, DELTA
 from .semiring import ZERO_MWP, sum_mwp
 
 logger = logging.getLogger(__name__)
 
+DELTAS = TypeVar('DELTAS', bound=DELTA)
+
 
 class Polynomial:
     """
     A polynomial is an ordered list of ordered [`Monomials`](monomial.md).
 
     For polynomials, I introduce a total order on the monomials. This
     eases the computation of the sum: if we want to add a monomial to an
@@ -28,17 +31,17 @@
 
     This is extended to products (which we consider ordered!) by
     letting $\\prod_k\\delta(i_k,j_k) < \\prod_l\\delta(m_l,n_l)$
     iff $\\delta(i_1,j_1) < \\delta(m_1,n_1)$.
     """
 
     def __init__(
-            self,
-            monomials: Optional[Union[str, List[Monomial], Monomial]] = None,
-            *args: Optional[Monomial]):
+            self, *monomials:
+            Optional[Union[str, Monomial, Tuple[str, DELTAS]]]
+    ):
         """Create a polynomial.
 
         Example:
 
         Create polynomial with 0-monomial
 
         ```python
@@ -49,33 +52,33 @@
 
         ```python
         poly = Polynomial('w')               # shorthand
 
         poly = Polynomial(Monomial('w'))     # longer, equivalent
         ```
 
-        Create polynomial with two monomials and deltas
+        Create polynomial with two monomials and lists of deltas
 
         ```python
-        poly = Polynomial(Monomial('m', (0, 1)), Monomial('w', (1, 1)))
+        # shorthand:
+        poly = Polynomial(('m', (0, 1)), ('w', (0, 0), (1, 1))) 
+
+        # equivalent:
+        poly = Polynomial(Monomial('m', (0, 1)), Monomial('w', (0, 0), (1, 1)))
         ```
 
         Arguments:
-            monomials: list of monomials
+            monomials: arbitrary number of monomials
         """
-        if monomials is not None and isinstance(monomials, str):
-            self.list = [Monomial(monomials)]
-        elif monomials is not None and isinstance(monomials, Monomial):
-            self.list = [monomials] + list(args if args else [])
-        else:
-            self.list = monomials or [Monomial(ZERO_MWP)]
+        m_list = [Monomial.format(v) for v in monomials]
+        self.list = m_list if len(m_list) > 0 else [Monomial(ZERO_MWP)]
 
     def __str__(self):
         values = ''.join(['+' + str(m) for m in self.list]) or ('+' + ZERO_MWP)
-        return "  " + values
+        return " " + values
 
     def __eq__(self, other):
         return self.equal(other)
 
     def __add__(self, other):
         return self.add(other)
 
@@ -87,20 +90,20 @@
         """List of monomial deltas whose scalar is infinity."""
         return [tuple(mono.deltas) for mono in
                 [m for m in self.list if m.scalar == 'i']]
 
     @staticmethod
     def inclusion(list_monom: list, mono: Monomial, i: int = 0) \
             -> Tuple[bool, int]:
-        """filter list_monom regarding to mono inclusion and return info
+        """filter list_monom regarding mono inclusion and return info.
 
-        remove all monomials of list_monom that are included in mono.
+        Remove all monomials of list_monom that are included in mono.
 
         return CONTAINS if one of monomials of list_monom contains mono
-        (regarding to Monomial.inclusion def).
+        (regarding Monomial.inclusion def).
 
         Arguments:
             list_monom: a list of monomials
             mono: a monomial we want to add
             i: the position index where to add mono
 
         Returns:
@@ -116,28 +119,28 @@
                 # We will then add mono so we can remove m
                 list_monom.remove(m)
                 # If removed monom is before i (where we want to insert mono)
                 if j < i:
                     i = i - 1  # shift left position
                 continue
             elif incl == SetInclusion.INCLUDED:
-                #  We don't want to add mono, inform with CONTAINS
+                # We don't want to add mono, inform with CONTAINS
                 return False, i
             j = j + 1
         # No inclusion
         return True, i
 
     def add(self, polynomial: Polynomial) -> Polynomial:
         """Add two polynomials
 
         - If both lists are empty the result is empty.
         - If one list is empty, the result will be the other list
         of polynomials.
 
-        Otherwise the operation will zip the two lists together
+        Otherwise, the operation will zip the two lists together
         and return a new polynomial of sorted monomials.
 
         Arguments:
             polynomial: Polynomial to add to self
 
         Returns:
             New, sorted polynomial that is a sum of the
@@ -193,15 +196,15 @@
             # when both list heads are the same
             # recompute scalar and move to next element
             else:
                 new_list[i].scalar = sum_mwp(mono1.scalar, mono2.scalar)
                 j = j + 1
 
         sorted_monomials = Polynomial.sort_monomials(new_list)
-        return Polynomial(sorted_monomials).remove_zeros()
+        return Polynomial(*sorted_monomials).remove_zeros()
 
     def times(self, polynomial: Polynomial) -> Polynomial:
         """Multiply two polynomials.
 
         Here we assume at least self is a sorted polynomial,
         and the result of this operation will be sorted.
 
@@ -292,15 +295,15 @@
                         index_list.insert(j, smallest)
                         inserted = True
                         break
                 if not inserted:
                     index_list.append(smallest)
             # 7. repeat until done
 
-        return Polynomial(result).remove_zeros()
+        return Polynomial(*result).remove_zeros()
 
     def equal(self, polynomial: Polynomial) -> bool:
         """Determine if two polynomials are equal.
 
         This method will compare current polynomial (self) to
         another polynomial provided as argument. Result of
         true means both polynomials have an equal number of
@@ -327,20 +330,42 @@
         # if False is in list it means some comparison of
         # deltas was determined not to be equal; do length
         # comparison last because it is almost never False
         return False not in same and len(p1) == len(p2)
 
     def copy(self) -> Polynomial:
         """Make a deep copy of polynomial."""
-        return Polynomial([m.copy() for m in self.list])
+        return Polynomial(*[m.copy() for m in self.list])
 
     def show(self) -> None:
         """Display polynomial."""
         print(str(self))
 
+    @property
+    def some_infty(self) -> bool:
+        """True if some monomial yields an infinity choice."""
+        for mono in self.list:
+            if mono.scalar == 'i':
+                return True
+        return False
+
+    def choice_scalar(self, *choices: int) -> Optional[str]:
+        """For given sequence of choices, determine corresponding scalar.
+
+        Arguments:
+            choices: tuple of choices
+
+        Returns:
+            Scalar value matching choices or None.
+        """
+        for mono in self.list:
+            scalar = mono.choice_scalar(*choices)
+            if scalar:
+                return scalar
+
     @staticmethod
     def compare(delta_list1: list, delta_list2: list) -> Comparison:
         """
         Compare 2 lists of deltas.
 
         We compare the initial segment up to the size of the shortest one.
         If the initial segments match, then the result is determined based
@@ -512,8 +537,8 @@
 
         Returns:
              Generated polynomial
          """
 
         monomials = [Monomial(scalar, [(number, index)])
                      for number, scalar in enumerate(scalars)]
-        return Polynomial(monomials)
+        return Polynomial(*monomials)
```

### Comparing `pymwp-0.3.0/pymwp/relation.py` & `pymwp-0.4.0/pymwp/relation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # flake8: noqa: W605
 
 from __future__ import annotations
 
 import logging
-from typing import Optional, Tuple, List
+from typing import Optional, Tuple, List, Dict
 
+from pymwp import Choices, DeltaGraph, Polynomial
 from . import matrix as matrix_utils
-from .choice import Choices
-from .delta_graphs import DeltaGraph
 
 logger = logging.getLogger(__name__)
 
 
 class Relation:
     """
     A relation is made of a list of variables and a 2D-matrix:
@@ -21,15 +20,15 @@
 
     - Matrix holds [`Polynomials`](polynomial.md#pymwp.polynomial)
     and represents the current state of the analysis.
 
     """
 
     def __init__(self, variables: Optional[List[str]] = None,
-                 matrix: Optional[List[List]] = None):
+                 matrix: Optional[List[List[Polynomial]]] = None):
         """Create a relation.
 
         When constructing a relation, provide a list of variables
         and an initial matrix.
 
         If matrix is not provided, the relation matrix will be initialized to
         zero matrix of size matching the number of variables.
@@ -52,15 +51,15 @@
         #  X2  |  0  0  0
         ```
 
         Arguments:
             variables: program variables
             matrix: relation matrix
         """
-        self.variables = [v for v in (variables or []) if v]
+        self.variables = [str(v) for v in (variables or []) if v]
         self.matrix = matrix or matrix_utils \
             .init_matrix(len(self.variables))
 
     @staticmethod
     def identity(variables: List) -> Relation:
         """Create an identity relation.
 
@@ -93,28 +92,37 @@
         matrix = matrix_utils.identity_matrix(len(variables))
         return Relation(variables, matrix)
 
     @property
     def is_empty(self):
         return not self.variables or not self.matrix
 
+    @property
+    def matrix_size(self):
+        return 0 if not self.variables else len(self.variables)
+
     def __str__(self):
-        right_pad = len(max(self.variables, key=len)) \
-            if self.variables else 0
-        return '\n'.join(
-            [var.ljust(right_pad) + '  |' + ''.join(poly) for var, poly in
-             [(var, [str(self.matrix[i][j]) for j in range(len(self.matrix))])
-              for i, var in enumerate(self.variables)]])
+        return Relation.relation_str(self.variables, self.matrix)
 
     def __add__(self, other):
         return self.sum(other)
 
     def __mul__(self, other):
         return self.composition(other)
 
+    @staticmethod
+    def relation_str(variables: List[str], matrix: List[List[any]]):
+        """Formatted string of variables and matrix."""
+        right_pad = len(max(variables, key=len)) if variables else 0
+        return '\n'.join(
+            [var.ljust(right_pad) + ' | ' + (' '.join(poly)).strip()
+             for var, poly in
+             [(var, [str(matrix[i][j]) for j in range(len(matrix))])
+              for i, var in enumerate(variables)]])
+
     def replace_column(self, vector: List, variable: str) -> Relation:
         """Replace identity matrix column by a vector.
 
         Arguments:
             vector: vector by which a matrix column will be replaced.
             variable: program variable, column replacement
                 will occur at the index of this variable.
@@ -122,19 +130,18 @@
         Raises:
               ValueError: if variable is not found in this relation.
 
         Returns:
             new relation after applying the column replacement.
         """
         new_relation = Relation.identity(self.variables)
-        j = self.variables.index(variable)
-
-        for idx, value in enumerate(vector):
-            new_relation.matrix[idx][j] = value
-
+        if variable in self.variables:
+            j = self.variables.index(variable)
+            for idx, value in enumerate(vector):
+                new_relation.matrix[idx][j] = value
         return new_relation
 
     def while_correction(self, dg: DeltaGraph) -> None:
         """Replace invalid scalars in a matrix by $\\infty$.
 
         Following the computation of fixpoint for a while loop node, this
         method checks the resulting matrix and replaces all invalid scalars
@@ -263,20 +270,50 @@
             prev_fix.matrix = fix.matrix
             current = current * self
             fix = fix + current
             if fix.equal(prev_fix):
                 logger.debug(f"fixpoint done {fix_vars}")
                 return fix
 
+    def apply_choice(self, *choices: int) -> SimpleRelation:
+        """Get the matrix corresponding to provided sequence of choices.
+
+        Arguments:
+            choices: tuple of choices
+
+        Returns:
+            New relation with simple-values matrix of scalars.
+        """
+        new_mat = [[self.matrix[i][j].choice_scalar(*choices)
+                    for j in range(self.matrix_size)]
+                   for i in range(self.matrix_size)]
+        return SimpleRelation(self.variables.copy(), matrix=new_mat)
+
+    def infty_vars(self) -> Dict[str, List[str]]:
+        """Identify all variable pairs that for some choices, can raise
+        infinity result.
+
+        Returns:
+            Dictionary of potentially infinite dependencies, where
+            the key is source variable and value is list of targets;
+            All entries are non-empty.
+        """
+        vars_ = self.variables
+        return dict([(x, y) for x, y in [
+            (src, [tgt for tgt, p in zip(vars_, polys) if p.some_infty])
+            for src, polys in zip(vars_, self.matrix)] if len(y) != 0])
+
+    def infty_pairs(self) -> str:
+        """List of potential infinity dependencies."""
+        fmt = [f'{s} ➔ {", ".join(t)}' for s, t in self.infty_vars().items()]
+        return ' ‖ '.join(fmt)
+
     def to_dict(self) -> dict:
         """Get dictionary representation of a relation."""
-        return {
-            "variables": self.variables,
-            "matrix": matrix_utils.encode(self.matrix)
-        }
+        return {"matrix": matrix_utils.encode(self.matrix)}
 
     def show(self):
         """Display relation."""
         print(str(self))
 
     @staticmethod
     def homogenisation(r1: Relation, r2: Relation) \
@@ -348,7 +385,16 @@
         # get all choices leading to infinity
         for row in self.matrix:
             for poly in row:
                 infinity_deltas.update(poly.eval)
 
         # generate valid choices
         return Choices.generate(choices, index, infinity_deltas)
+
+
+class SimpleRelation(Relation):
+    """Specialized instance of relation, where matrix contains only
+       scalar values, no Polynomials."""
+
+    def __init__(self, variables: Optional[List[str]] = None,
+                 matrix: Optional[List[List[str]]] = None):
+        super().__init__(variables, matrix)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pymwp-0.3.0/pymwp/relation_list.py` & `pymwp-0.4.0/pymwp/relation_list.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/pymwp/semiring.py` & `pymwp-0.4.0/pymwp/semiring.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/pymwp.egg-info/PKG-INFO` & `pymwp-0.4.0/pymwp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymwp
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementation of MWP analysis on C code in Python.
 Home-page: https://github.com/statycc/pymwp
 Author: Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller
 Author-email: nrusch@augusta.edu
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/statycc/pymwp/issues
 Project-URL: Documentation, https://statycc.github.io/pymwp/
@@ -103,26 +103,26 @@
 
 1. Clone the repository
 
     ```
     git clone https://github.com/statycc/pymwp.git
     ``` 
 
-2. Set up Python environment
+2. Set up Python environment (use [`venv`](https://docs.python.org/3/library/venv.html))
 
     install required packages
 
     ```
-    python -m pip install -q -r requirements.txt
+    python -m pip install -r requirements.txt
     ``` 
     
-    Note: for development purposes or to run tests, install dev dependencies instead: 
+    Note: for development purposes install dev dependencies instead: 
     
     ```
-    python -m pip install -q -r requirements-dev.txt
+    python -m pip install -r requirements-dev.txt
     ```
 
 3. Run the analysis
 
     From project root run:
     
     ```
```

### Comparing `pymwp-0.3.0/pymwp.egg-info/SOURCES.txt` & `pymwp-0.4.0/pymwp.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 pymwp/__init__.py
 pymwp/__main__.py
 pymwp/analysis.py
+pymwp/bound.py
 pymwp/choice.py
 pymwp/constants.py
 pymwp/delta_graphs.py
 pymwp/file_io.py
 pymwp/matrix.py
 pymwp/monomial.py
 pymwp/parser.py
@@ -22,14 +23,15 @@
 pymwp.egg-info/SOURCES.txt
 pymwp.egg-info/dependency_links.txt
 pymwp.egg-info/entry_points.txt
 pymwp.egg-info/requires.txt
 pymwp.egg-info/top_level.txt
 tests/__init__.py
 tests/test_analysis.py
+tests/test_bound.py
 tests/test_choices.py
 tests/test_compare.py
 tests/test_delta_graph.py
 tests/test_file_io.py
 tests/test_matrix.py
 tests/test_monomial.py
 tests/test_parser.py
```

### Comparing `pymwp-0.3.0/setup.py` & `pymwp-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 __title__ = "pymwp"
 __author__ = "Clément Aubert, Thomas Rubiano, Neea Rusch, Thomas Seiller"
 __desc__ = "Implementation of MWP analysis on C code in Python."
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name=__title__,
     version=__version__,
```

### Comparing `pymwp-0.3.0/tests/mocks/ast_mocks.py` & `pymwp-0.4.0/tests/mocks/ast_mocks.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/tests/test_analysis.py` & `pymwp-0.4.0/tests/test_analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,33 @@
     INFINITE_2C, INFINITE_8C, NOT_INFINITE_2C, NOT_INFINITE_3C, \
     IF_WO_BRACES, IF_WITH_BRACES, VARIABLE_IGNORED, BRACES_ISSUES, \
     PARAMS, FUNCTION_CALL, EMPTY
 
 
 def test_analyze_infinite2():
     """Check analysis result for infinite/infinite_2.c"""
-    relation, combinations, infty = Analysis.run(INFINITE_2C, no_save=True)
+    foo = Analysis.run(INFINITE_2C, no_save=True).get_func()
+    relation, combinations = foo.relation, foo.choices
 
-    assert infty  # result should be infinite
+    assert foo.infinite  # result should be infinite
     assert combinations is None  # no combinations since it is infinite
     assert relation is None  # no relation since infinite
 
 
 def test_analyze_infinite_8():
     """Check analysis result for infinite/infinite_8.c"""
-    _, _, infty = Analysis.run(INFINITE_8C, no_save=True)
-    assert infty
+    assert Analysis.run(INFINITE_8C, no_save=True).get_func().infinite
 
 
 def test_analyze_non_infinite_2():
     """Check analysis result for not_infinite/notinfinite_2.c"""
-    relation, combinations, infty = Analysis.run(NOT_INFINITE_2C, no_save=True)
+    foo = Analysis.run(NOT_INFINITE_2C, no_save=True).get_func()
+    relation, combinations = foo.relation, foo.choices
 
-    assert not infty
+    assert not foo.infinite
 
     # match expected choices and variables
     assert set(relation.variables) == {'X0', 'X1'}
     assert combinations.is_valid(0, 0)
     assert combinations.is_valid(0, 1)
     assert combinations.is_valid(0, 2)
     assert combinations.is_valid(1, 0)
@@ -42,32 +43,37 @@
     assert str(relation.matrix[0][0].list[0]) == 'w.delta(0,0)'
     assert str(relation.matrix[0][0].list[1]) == 'w.delta(1,0)'
     assert str(relation.matrix[0][0].list[2]) == 'w.delta(2,0)'
 
 
 def test_analyze_non_infinite_3():
     """Check analysis result for not_infinite/notinfinite_3.c"""
-    _, combinations, infty = Analysis.run(NOT_INFINITE_3C, no_save=True)
-
-    assert not infty
-    assert len(combinations.valid) == 1
-    assert combinations.valid[0] == [[0, 1, 2], [0, 1, 2], [2]]
+    foo = Analysis.run(NOT_INFINITE_3C, no_save=True).get_func()
+    assert not foo.infinite
+    assert len(foo.choices.valid) == 1
+    assert foo.choices.valid[0] == [[0, 1, 2], [0, 1, 2], [2]]
 
 
 def test_analyze_infinite_to_completion():
     """Check analysis completion for infinite program"""
-    matrix, _, _ = Analysis.run(INFINITE_2C, no_save=True, fin=True)
-    assert matrix
+    relation = Analysis.run(INFINITE_2C, no_save=True, fin=True) \
+        .get_func().relation
+    assert relation
+    assert relation.matrix
+    assert not relation.is_empty
 
 
 def test_analyze_if_braces_do_not_matter():
     """If...else block with single-statement, with or without curly braces,
      should give the same analysis result."""
-    rel_with, choices_with = Analysis.run(IF_WITH_BRACES, no_save=True)[:2]
-    rel_wo, choices_wo = Analysis.run(IF_WO_BRACES, no_save=True)[:2]
+    res1 = Analysis.run(IF_WITH_BRACES, no_save=True).get_func()
+    rel_with, choices_with = res1.relation, res1.choices
+    res2 = Analysis.run(IF_WO_BRACES, no_save=True).get_func()
+    rel_wo, choices_wo = res2.relation, res2.choices
+
     all_valid_choices = [
         [0, 0, 0], [0, 0, 1], [0, 0, 2], [0, 1, 0], [0, 1, 1],
         [0, 1, 2], [0, 2, 0], [0, 2, 1], [0, 2, 2], [1, 0, 0],
         [1, 0, 1], [1, 0, 2], [1, 1, 0], [1, 1, 1], [1, 1, 2],
         [1, 2, 0], [1, 2, 1], [1, 2, 2], [2, 0, 0], [2, 0, 1],
         [2, 0, 2], [2, 1, 0], [2, 1, 1], [2, 1, 2], [2, 2, 0],
         [2, 2, 1], [2, 2, 2]]
@@ -79,15 +85,16 @@
     for choice in all_valid_choices:
         assert choices_with.is_valid(*choice) and choices_wo.is_valid(*choice)
 
 
 def test_analyze_variable_ignore():
     """Analysis picks up variable on left of assignment,
     see issue #11: https://github.com/statycc/pymwp/issues/11 """
-    relation, combinations = Analysis.run(VARIABLE_IGNORED, no_save=True)[:2]
+    result = Analysis.run(VARIABLE_IGNORED, no_save=True).get_func()
+    relation, combinations = result.relation, result.choices
     non_infinity_choices = [[0, 0], [0, 1], [0, 2],
                             [1, 0], [1, 1], [1, 2],
                             [2, 0], [2, 1], [2, 2]]
 
     for choice in non_infinity_choices:
         assert combinations.is_valid(*choice)
     assert set(relation.variables) == {'X2', 'X3', 'X1', 'X4'}
@@ -111,41 +118,38 @@
         relation.show()
         raise
 
 
 def test_extra_braces_are_ignored():
     """Analysis ignores superfluous braces in C program,
     see issue: #25: https://github.com/statycc/pymwp/issues/25"""
-    relation, combinations = Analysis.run(BRACES_ISSUES, no_save=True)[
-                             :2]
-
+    result = Analysis.run(BRACES_ISSUES, no_save=True).get_func()
+    relation, combinations = result.relation, result.choices
     assert set(relation.variables) == {'x', 'y'}
     assert relation.matrix[0][0] == Polynomial('m')
     assert relation.matrix[0][1] == Polynomial('o')
     assert relation.matrix[1][0] == Polynomial('m')
     assert relation.matrix[1][1] == Polynomial('m')
 
 
 def test_analysis_identifies_function_params():
     """Analysis will identify variables from function declaration
     issue #51: https://github.com/statycc/pymwp/issues/51
     """
-    relation = Analysis.run(PARAMS, no_save=True)[0]
-
+    relation = Analysis.run(PARAMS, no_save=True).get_func().relation
     assert set(relation.variables) == {'x1', 'x2', 'x3'}
 
 
 def test_analysis_returns_all_functions():
     """If input file contains multiple functions result contains
     evaluation of each function (example 5a)
     """
-    result = Analysis.run(FUNCTION_CALL, no_save=True)
-    _, _, f_infty = result['f']
-    foo, _, _ = result['foo']
+    f = Analysis.run(FUNCTION_CALL, no_save=True).get_func('f')
+    foo = Analysis.run(FUNCTION_CALL, no_save=True).get_func('foo')
 
-    assert not f_infty
-    assert set(foo.variables) == {'X1', 'X2'}
+    assert not f.infinite
+    assert set(foo.relation.variables) == {'X1', 'X2'}
 
 
 def test_analysis_handles_empty_program():
-    relation = Analysis.run(EMPTY, no_save=True)
-    assert relation == {}
+    result = Analysis.run(EMPTY, no_save=True)
+    assert result.relations == {}
```

### Comparing `pymwp-0.3.0/tests/test_choices.py` & `pymwp-0.4.0/tests/test_choices.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,26 @@
     inf = {((0, 0), (0, 1)),
            ((0, 0), (1, 1), (3, 2)),
            ((1, 0), (1, 1), (3, 2)),
            ((2, 0), (1, 1), (3, 2)),
            ((3, 0), (1, 1), (3, 2))}
     result = Choices.generate(choices, index, inf)
 
-    assert not result.infinite
     assert len(result.valid) == 4
     assert [[1, 2, 3], [0, 2, 3], [0, 1, 2, 3]] in result.valid  # !(0,0) (1,1)
     assert [[1, 2, 3], [0, 1, 2, 3], [0, 1, 2]] in result.valid  # !(0,0) (3,2)
     assert [[0, 1, 2, 3], [2, 3], [0, 1, 2, 3]] in result.valid  # !(0,1) (1,1)
     assert [[0, 1, 2, 3], [1, 2, 3], [0, 1, 2]] in result.valid  # !(0,1) (3,2)
 
 
 def test_infinite_eval():
     index, choices = 4, [0, 1, 2]
     infinite = {((0, 3),), ((1, 3),), ((2, 3),)}
     result = Choices.generate(choices, index, infinite)
-    assert result.infinite
+    assert len(result.valid) == 0
 
 
 def test_is_valid_returns_correct_result():
     index, choices = 2, [0, 1, 2]
     infinite = {((0, 1),), ((1, 0), (2, 1))}
     obj = Choices.generate(choices, index, infinite)
 
@@ -55,7 +54,28 @@
                 ((2, 0), (1, 1), (1, 2))}
     result = Choices.generate(choices, index, infinite)
 
     assert [[2], [0, 1, 2], [0, 2]] in result.valid
     assert [[2], [0, 1], [0, 2]] not in result.valid
     assert [[2], [0, 2], [0, 2]] not in result.valid
     assert [[2], [0], [0, 1, 2]] in result.valid
+
+
+def test_first_choice():
+    choices = [0, 1, 2]
+
+    # all choice except [0, 1, 0] -> first choice is (1, 0, 1)
+    infty1 = {((0, 0),), ((1, 1),), ((0, 2),)}
+    # only allow (2, 2)
+    infty2 = {((0, 0),), ((1, 0),), ((0, 1),), ((1, 1),)}
+
+    assert Choices.generate(choices, 3, infty1).first == (1, 0, 1)
+    assert Choices.generate(choices, 2, infty2).first == (2, 2)
+
+
+def test_choice_counter():
+    """test bounds count"""
+    choice1 = Choices([[[0, 1, 2], [0, 1, 2], [2]]])
+    choice2 = Choices([[[0, 1, 2], [0, 1], [0, 1, 2], [0, 1, 2], [0, 2], [0]]])
+
+    assert choice1.n_bounds == 9
+    assert choice2.n_bounds == 108
```

### Comparing `pymwp-0.3.0/tests/test_compare.py` & `pymwp-0.4.0/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/tests/test_delta_graph.py` & `pymwp-0.4.0/tests/test_delta_graph.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/tests/test_matrix.py` & `pymwp-0.4.0/tests/test_matrix.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     assert matrix[2][2] == m
 
 
 def test_resize_modifies_matrix_size():
     """Resizing matrix changes matrix size correctly, it preserves the
     polynomials from the input matrix, and when enlarging, the newly added
     positions are filled with identity matrix values."""
-    poly = Polynomial([Monomial('m')])
+    poly = Polynomial(Monomial('m'))
     before_resize = init_matrix(2, poly)
     after_resize = resize(before_resize, 5)
 
     # correctly changes matrix dimensions
     assert len(before_resize) == len(before_resize[0]) == 2
     assert len(after_resize) == len(after_resize[0]) == 5
 
@@ -54,33 +54,33 @@
     assert after_resize[2][2] == m
     assert after_resize[3][3] == m
     assert after_resize[4][4] == m
 
 
 def test_matrix_sum():
     """Matrix sum should add two matrices element-wise."""
-    expected = Polynomial([Monomial('m', [(0, 0)]), Monomial('w', [(1, 1)])])
+    expected = Polynomial(Monomial('m', [(0, 0)]), Monomial('w', [(1, 1)]))
 
-    mat_a = init_matrix(2, Polynomial([Monomial('m', [(0, 0)])]))
-    mat_b = init_matrix(2, Polynomial([Monomial('w', [(1, 1)])]))
+    mat_a = init_matrix(2, Polynomial(Monomial('m', (0, 0))))
+    mat_b = init_matrix(2, Polynomial(Monomial('w', (1, 1))))
     result = matrix_sum(mat_a, mat_b)
 
     assert result[0][0] == expected
     assert result[0][1] == expected
     assert result[1][0] == expected
     assert result[1][1] == expected
 
 
 def test_matrix_prod():
     """Matrix product test -- here we check using an elaborate test case
     that the product is what it should be, at each position."""
-    p1 = Polynomial([Monomial('p', [(0, 1)]), Monomial('w', [(1, 1)])])
-    p2 = Polynomial([Monomial('m', [(0, 1)]), Monomial('w', [(1, 1)])])
-    p3 = Polynomial([Monomial('m', [(0, 2)]), Monomial('w', [(1, 2)])])
-    p4 = Polynomial([Monomial('p', [(0, 2)]), Monomial('w', [(1, 2)])])
+    p1 = Polynomial(Monomial('p', [(0, 1)]), Monomial('w', [(1, 1)]))
+    p2 = Polynomial(Monomial('m', [(0, 1)]), Monomial('w', [(1, 1)]))
+    p3 = Polynomial(Monomial('m', [(0, 2)]), Monomial('w', [(1, 2)]))
+    p4 = Polynomial(Monomial('p', [(0, 2)]), Monomial('w', [(1, 2)]))
 
     #          m p3 o
     #          o m  o
     #          o p4 m
     # m o p1
     # o m p2
     # o o o
@@ -105,15 +105,15 @@
         print("Should be :")
         print((m * p3) + (o * m) + (p1 * p4))
         raise
 
 
 def test_encode():
     """Encoding converts matrix of polynomials to a list of dictionaries."""
-    p = Polynomial([Monomial('m', [(0, 1)])])
+    p = Polynomial(Monomial('m', [(0, 1)]))
     mat = init_matrix(2, p)
     encoded = encode(mat)
     expected = [
         [[{'scalar': 'm', 'deltas': [(0, 1)]}],
          [{'scalar': 'm', 'deltas': [(0, 1)]}]],
         [[{'scalar': 'm', 'deltas': [(0, 1)]}],
          [{'scalar': 'm', 'deltas': [(0, 1)]}]]
@@ -128,39 +128,38 @@
         [[{'scalar': 'm', 'deltas': [(0, 1)]}],
          [{'scalar': 'm', 'deltas': [(0, 1)]}]],
         [[{'scalar': 'm', 'deltas': [(0, 1)]}],
          [{'scalar': 'm', 'deltas': [(0, 1)]}]]
     ]
 
     decoded = decode(sample)
-    expected = init_matrix(2, Polynomial([Monomial('m', [(0, 1)])]))
+    expected = init_matrix(2, Polynomial(Monomial('m', (0, 1))))
 
     assert decoded == expected
 
 
 def test_matrix_equals():
     """Two polynomial matrices are equal when their monomials match exactly."""
-    p1 = Polynomial([Monomial('m', [(0, 1), (1, 1)])])
-    p2 = Polynomial([Monomial('m', [(0, 1), (1, 1)])])
-    p3 = Polynomial([Monomial('m', [(0, 0)])])
-    p4 = Polynomial([Monomial('m', [(0, 0)])])
-    p5 = Polynomial([Monomial('m', [(1, 1), (2, 2)])])
-    p6 = Polynomial([Monomial('m', [(1, 1), (2, 2)])])
+    p1 = Polynomial(Monomial('m', [(0, 1), (1, 1)]))
+    p2 = Polynomial(Monomial('m', [(0, 1), (1, 1)]))
+    p3 = Polynomial(Monomial('m', [(0, 0)]))
+    p4 = Polynomial(Monomial('m', [(0, 0)]))
+    p5 = Polynomial(Monomial('m', [(1, 1), (2, 2)]))
+    p6 = Polynomial(Monomial('m', [(1, 1), (2, 2)]))
 
     m1 = [[o, p1, o], [p3, o, o], [o, o, p5]]
     m2 = [[o, p2, o], [p4, o, o], [o, o, p6]]
 
     assert equals(m1, m2) is True
 
 
 def test_matrix_not_equals():
     """Two matrices where monomials differ by deltas are not equal."""
-    p1 = Polynomial([Monomial('m', [(0, 1)])])
-    p2 = Polynomial([Monomial('m', [(1, 1)])])
-
+    p1 = Polynomial(Monomial('m', [(0, 1)]))
+    p2 = Polynomial(Monomial('m', [(1, 1)]))
     m1 = [[o, o, o], [o, o, o], [o, o, p1]]
     m2 = [[o, o, o], [o, o, o], [o, o, p2]]
 
     assert equals(m1, m2) is False
 
 
 def test_matrix_size_not_equals():
```

### Comparing `pymwp-0.3.0/tests/test_monomial.py` & `pymwp-0.4.0/tests/test_monomial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from pytest import raises
 from pymwp import Monomial
 from pymwp.constants import SetInclusion
 
 """Unit test Monomial class methods."""
 
 
 def test_create_monomial_without_deltas():
```

### Comparing `pymwp-0.3.0/tests/test_parser.py` & `pymwp-0.4.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/tests/test_polynomial.py` & `pymwp-0.4.0/tests/test_polynomial.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,65 @@
 from pymwp.semiring import ZERO_MWP
 from pymwp import Polynomial, Monomial
 
 
 def test_polynomial_copy():
     """Copying a polynomial returns different reference but of identical
     content."""
-    p = Polynomial([Monomial('m', [(0, 0), (1, 1)])])
+    p = Polynomial(Monomial('m', [(0, 0), (1, 1)]))
     poly_copy = p.copy()
 
     assert poly_copy == p  # their data is identical
     assert poly_copy is not p  # different reference
 
 
 def test_poly_decl_equivalence():
     """
     Both syntax define the same polynomial; the list
     brackets are superfluous.
     """
-    p1 = Polynomial([Monomial('m', [(0, 0), (1, 1)])])
+    p1 = Polynomial(Monomial('m', [(0, 0), (1, 1)]))
     p2 = Polynomial(Monomial('m', (0, 0), (1, 1)))
 
     assert len(p1.list) == len(p2.list) == 1
     assert len(p1.list[0].scalar) == len(p2.list[0].scalar)
     assert len(p1.list[0].deltas) == len(p2.list[0].deltas)
 
 
+def test_poly_decl_shorthand():
+    """Equivalent declarations."""
+    p1 = Polynomial(Monomial('m', (0, 1)),
+                    Monomial('w', (0, 0), (1, 1), (2, 2)))
+    p2 = Polynomial(('m', (0, 1)), ('w', (0, 0), (1, 1), (2, 2)))
+
+    assert len(p1.list) == len(p2.list) == 2
+    assert len(p1.list[0].scalar) == len(p2.list[0].scalar)
+    assert len(p1.list[1].scalar) == len(p2.list[1].scalar)
+    assert len(p1.list[0].deltas) == len(p2.list[0].deltas)
+    assert len(p1.list[1].deltas) == len(p2.list[1].deltas)
+
+
 def test_poly_decl_equivalence_multi():
     """Both syntax define the same polynomial; many monomials."""
-    p1 = Polynomial([
+    p1 = Polynomial(
         Monomial('i', [(0, 0), (1, 1)]), Monomial('i'),
-        Monomial('w', [(1, 0), (2, 1), (0, 2)])
-    ])
+        Monomial('w', [(1, 0), (2, 1), (0, 2)]))
     p2 = Polynomial(Monomial('i', (0, 0), (1, 1)), Monomial('i'),
                     Monomial('w', (1, 0), (2, 1), (0, 2)))
 
     assert len(p1.list) == len(p2.list) == 3
     for i in range(len(p1.list)):
         assert len(p1.list[i].scalar) == len(p2.list[i].scalar)
         assert len(p1.list[i].deltas) == len(p2.list[i].deltas)
 
 
 def test_polynomial_times_empty():
     """Multiplying two polynomials where one is 0-monomial, results in 0."""
     z = Polynomial(ZERO_MWP)
-    p = Polynomial([Monomial('m', [(0, 0), (1, 1)])])
+    p = Polynomial(Monomial('m', [(0, 0), (1, 1)]))
 
     assert (p * z) == Polynomial(ZERO_MWP)
 
 
 def test_contains_filter():
     """Contains correctly identifies when a monomial is contained by
     another."""
@@ -65,89 +77,81 @@
 
 
 def test_polynomial_add_by_non_empty():
     """Adding two polynomials with monomials with deltas, returns expected
     result."""
     mono1 = Monomial('m', [(2, 2)])
     mono2 = Monomial('m', [(0, 0), (1, 1)])
-    m = Polynomial([mono1])
-    p = Polynomial([mono2])
+    m = Polynomial(mono1)
+    p = Polynomial(mono2)
     c = p + m
     expected = Polynomial(
-        [Monomial('m', [(0, 0), (1, 1)]), Monomial('m', [(2, 2)])])
+        Monomial('m', [(0, 0), (1, 1)]), Monomial('m', [(2, 2)]))
 
     assert c == expected
 
 
 def test_polynomial_add_simpl():
     """Result of polynomial add is simplified."""
     mono1 = Monomial('m', [(0, 1), (0, 2), (0, 3)])
     mono2 = Monomial('w', [(0, 2), (0, 3), (0, 4)])
     mono3 = Monomial('p', [(0, 2), (0, 3), (0, 5)])
-    m = Polynomial(Polynomial.sort_monomials([mono1, mono2, mono3]))
-    print(m)
+    m = Polynomial(*Polynomial.sort_monomials([mono1, mono2, mono3]))
     mono0 = Monomial('w', [(0, 2), (0, 3)])
-    p = Polynomial([mono0])
+    p = Polynomial(mono0)
     c = p.add(m)
-    expected = Polynomial([mono0, mono3])
+    expected = Polynomial(mono0, mono3)
 
     assert c == expected
 
 
 def test_polynomial_times_by_non_empty():
     """Multiplying two polynomials with monomials with deltas gives expected
      result."""
-    p1 = Polynomial([Monomial('m', [(2, 2)])])
-    p2 = Polynomial([Monomial('m', [(0, 0), (1, 1)])])
-    expected = Polynomial([Monomial('m', [(0, 0), (1, 1), (2, 2)])])
+    p1 = Polynomial(Monomial('m', [(2, 2)]))
+    p2 = Polynomial(Monomial('m', [(0, 0), (1, 1)]))
+    expected = Polynomial(Monomial('m', [(0, 0), (1, 1), (2, 2)]))
 
     assert (p1 * p2) == expected
 
 
 def test_polynomial_times_by_non_empty2():
     mono1 = Monomial('m', [(2, 2)])
     mono12 = Monomial('m', [(1, 1)])
     mono2 = Monomial('m', [(0, 0)])
     mono22 = Monomial('m', [(3, 3)])
-    m = Polynomial([mono1, mono12])
-    p = Polynomial([mono2, mono22])
+    m = Polynomial(mono1, mono12)
+    p = Polynomial(mono2, mono22)
     c = p * m
-    expected = Polynomial([
+    expected = Polynomial(
         Monomial('m', [(0, 0), (1, 1)]),
         Monomial('m', [(0, 0), (2, 2)]),
         Monomial('m', [(1, 1), (3, 3)]),
-        Monomial('m', [(2, 2), (3, 3)])])
-    try:
-        assert c == expected
-    except AssertionError:
-        print("expected:")
-        print(expected)
-        print("prod:")
-        print(c)
-        raise
+        Monomial('m', [(2, 2), (3, 3)]))
+    assert c == expected
 
 
 def test_polynomial_equals_empty_are_equal():
     """Two default polynomials are equal."""
     p1 = Polynomial()
     p2 = Polynomial()
     assert p1.equal(p2) is True
 
 
 def test_polynomial_equals_same_returns_true():
     """equal returns true when two polynomials are the same."""
-    p1 = Polynomial([Monomial('m', [(0, 0), (1, 1), (2, 2)])])
-    p2 = Polynomial([Monomial('m', [(0, 0), (1, 1), (2, 2)])])
+    p1 = Polynomial(Monomial('m', [(0, 0), (1, 1), (2, 2)]))
+    p2 = Polynomial(Monomial('m', [(0, 0), (1, 1), (2, 2)]))
     assert p1.equal(p2) is True
 
 
 def test_polynomial_equals_different_returns_false():
     """equal returns false when two polynomials are different."""
-    p1 = Polynomial([Monomial('m', [(0, 0), (1, 1), (2, 2)])])
-    p2 = Polynomial([Monomial('m', [(1, 1), (3, 3)])])
+    p1 = Polynomial(Monomial('m', [(0, 0), (1, 1), (2, 2)]))
+    p2 = Polynomial(Monomial('m', [(1, 1), (3, 3)]))
 
     assert p1.equal(p2) is False
 
 
 def test_polynomial_sort_1():
     """Sorting monomials with deltas gives expected order."""
     m1 = Monomial('m', [(0, 1), (1, 6)])
@@ -179,42 +183,51 @@
 def test_polynomial_remove_zeros_with_deltas():
     """Adding two polynomials where one contains 0-monomial and another
     contains non-0 monomial -AND- some deltas, after addition, only the
     non-zero monomial remains in the result.
 
     see: https://github.com/statycc/pymwp/issues/16
     """
-    zero = Polynomial([Monomial('o')])
-    poly = Polynomial([Monomial('m', [(0, 0), (1, 1)])])
+    zero = Polynomial(Monomial('o'))
+    poly = Polynomial(Monomial('m', [(0, 0), (1, 1)]))
     after_add = zero + poly
 
     assert len(after_add.list) == 1
     assert 'm' == after_add.list[0].scalar
 
 
 def test_polynomial_remove_zeros_no_deltas():
     """Adding two polynomials where one contains 0-monomial and another
     contains non-0 monomial without deltas, after addition, only the
     non-zero monomial remains in the result."""
-    zero = Polynomial([Monomial('o')])
-    poly = Polynomial([Monomial('w')])
+    zero = Polynomial(Monomial('o'))
+    poly = Polynomial(Monomial('w'))
     after_add = zero + poly
 
     assert len(after_add.list) == 1
     assert 'w' == after_add.list[0].scalar
 
 
 def test_polynomial_remove_zeros_empty():
     """For a polynomial that contains only 0-monomials, only one 0-monomial
     remains after removing zeros."""
-    poly = Polynomial([Monomial('o'), Monomial('o'), Monomial('o')])
+    poly = Polynomial(Monomial('o'), Monomial('o'), Monomial('o'))
     poly.remove_zeros()
 
     assert len(poly.list) == 1
     assert poly.list[0].scalar == 'o'
 
 
 def test_polynomial_init_shorthand_syntax():
     """Shorthand syntax gives equivalent polynomial as the longer syntax."""
-    assert Polynomial('m') == Polynomial([Monomial('m')])
-    assert Polynomial('w') == Polynomial([Monomial('w')])
-    assert Polynomial('p') == Polynomial([Monomial('p')])
+    assert Polynomial('m') == Polynomial(Monomial('m'))
+    assert Polynomial('w') == Polynomial(Monomial('w'))
+    assert Polynomial('p') == Polynomial(Monomial('p'))
+
+
+def test_finds_infty_scalar():
+    p1 = Polynomial('m', 'w', 'p', 'p', 'm', 'i', 'p')
+    p2 = Polynomial(('m', (0, 0), (1, 1)), ('w', (1, 0), (0, 1)),
+                    ('p', (1, 0), (2, 1)), 'w')
+
+    assert p1.some_infty is True
+    assert p2.some_infty is False
```

### Comparing `pymwp-0.3.0/tests/test_relation.py` & `pymwp-0.4.0/tests/test_relation.py`

 * *Files identical despite different names*

### Comparing `pymwp-0.3.0/tests/test_relation_list.py` & `pymwp-0.4.0/tests/test_relation_list.py`

 * *Files identical despite different names*

