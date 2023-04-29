# Comparing `tmp/pycotap-1.3.0.tar.gz` & `tmp/pycotap-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycotap-1.3.0.tar", last modified: Fri Apr 28 10:27:44 2023, max compression
+gzip compressed data, was "pycotap-1.3.1.tar", last modified: Sat Apr 29 09:56:37 2023, max compression
```

## Comparing `pycotap-1.3.0.tar` & `pycotap-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.201216 pycotap-1.3.0/
--rw-r--r--   0 remko      (501) staff       (20)     1080 2015-01-21 16:26:27.000000 pycotap-1.3.0/COPYING
--rw-r--r--   0 remko      (501) staff       (20)     1756 2023-04-28 10:27:44.201019 pycotap-1.3.0/PKG-INFO
--rw-r--r--   0 remko      (501) staff       (20)     5480 2023-04-28 10:24:45.000000 pycotap-1.3.0/README.md
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.199351 pycotap-1.3.0/pycotap/
--rw-r--r--   0 remko      (501) staff       (20)     4948 2023-04-28 10:05:29.000000 pycotap-1.3.0/pycotap/__init__.py
--rw-r--r--   0 remko      (501) staff       (20)      123 2023-04-28 09:54:31.000000 pycotap-1.3.0/pycotap/__main__.py
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.200515 pycotap-1.3.0/pycotap.egg-info/
--rw-r--r--   0 remko      (501) staff       (20)     1756 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/PKG-INFO
--rw-r--r--   0 remko      (501) staff       (20)      218 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/SOURCES.txt
--rw-r--r--   0 remko      (501) staff       (20)        1 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/dependency_links.txt
--rw-r--r--   0 remko      (501) staff       (20)        8 2023-04-28 10:27:44.000000 pycotap-1.3.0/pycotap.egg-info/top_level.txt
--rw-r--r--   0 remko      (501) staff       (20)      869 2023-04-28 10:16:29.000000 pycotap-1.3.0/pyproject.toml
--rw-r--r--   0 remko      (501) staff       (20)       38 2023-04-28 10:27:44.201273 pycotap-1.3.0/setup.cfg
--rwxr-xr-x   0 remko      (501) staff       (20)     1977 2023-04-28 10:25:08.000000 pycotap-1.3.0/setup.py
-drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-28 10:27:44.200741 pycotap-1.3.0/test/
--rw-r--r--   0 remko      (501) staff       (20)    10365 2023-04-28 10:16:27.000000 pycotap-1.3.0/test/test.py
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-29 09:56:37.293027 pycotap-1.3.1/
+-rw-r--r--   0 remko      (501) staff       (20)     1080 2015-01-20 19:49:45.000000 pycotap-1.3.1/COPYING
+-rw-r--r--   0 remko      (501) staff       (20)     1773 2023-04-29 09:56:37.292932 pycotap-1.3.1/PKG-INFO
+-rw-r--r--   0 remko      (501) staff       (20)     5504 2023-04-29 06:23:33.000000 pycotap-1.3.1/README.md
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-29 09:56:37.292257 pycotap-1.3.1/pycotap/
+-rw-r--r--   0 remko      (501) staff       (20)     4969 2023-04-29 06:04:36.000000 pycotap-1.3.1/pycotap/__init__.py
+-rw-r--r--   0 remko      (501) staff       (20)      123 2023-04-29 05:55:02.000000 pycotap-1.3.1/pycotap/__main__.py
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-29 09:56:37.292681 pycotap-1.3.1/pycotap.egg-info/
+-rw-r--r--   0 remko      (501) staff       (20)     1773 2023-04-29 09:56:37.000000 pycotap-1.3.1/pycotap.egg-info/PKG-INFO
+-rw-r--r--   0 remko      (501) staff       (20)      218 2023-04-29 09:56:37.000000 pycotap-1.3.1/pycotap.egg-info/SOURCES.txt
+-rw-r--r--   0 remko      (501) staff       (20)        1 2023-04-29 09:56:37.000000 pycotap-1.3.1/pycotap.egg-info/dependency_links.txt
+-rw-r--r--   0 remko      (501) staff       (20)        8 2023-04-29 09:56:37.000000 pycotap-1.3.1/pycotap.egg-info/top_level.txt
+-rw-r--r--   0 remko      (501) staff       (20)      935 2023-04-29 06:12:04.000000 pycotap-1.3.1/pyproject.toml
+-rw-r--r--   0 remko      (501) staff       (20)       38 2023-04-29 09:56:37.293062 pycotap-1.3.1/setup.cfg
+-rwxr-xr-x   0 remko      (501) staff       (20)     1962 2023-04-29 09:55:25.000000 pycotap-1.3.1/setup.py
+drwxr-xr-x   0 remko      (501) staff       (20)        0 2023-04-29 09:56:37.292791 pycotap-1.3.1/test/
+-rw-r--r--   0 remko      (501) staff       (20)    10331 2023-04-29 05:55:15.000000 pycotap-1.3.1/test/test.py
```

### Comparing `pycotap-1.3.0/COPYING` & `pycotap-1.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `pycotap-1.3.0/PKG-INFO` & `pycotap-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycotap
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tiny test runner that outputs TAP results to standard output.
-Home-page: https://el-tramo.be/pycotap
+Home-page: https://github.com/remko/pycotap
 Author: Remko Tronçon
-Author-email: dev@el-tramo.be
+Author-email: 08cage-calm@icloud.com
 License: MIT
 Keywords: tap unittest testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -34,8 +34,8 @@
 
 - ... is configurable: you can choose how you want the test output and test result
   diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
   attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
   flow.
 
 Documentation and examples can be found on `the pycotap page 
-<https://el-tramo.be/pycotap>`_.
+<https://github.com/remko/pycotap>`_.
```

### Comparing `pycotap-1.3.0/README.md` & `pycotap-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # pycotap: Tiny Python TAP Test Runner
 
 [![Build](https://github.com/remko/pycotap/actions/workflows/build.yml/badge.svg)](https://github.com/remko/pycotap/actions/workflows/build.yml)
+[![Coverage](https://remko.github.io/pycotap/ci/coverage/coverage.svg)](https://remko.github.io/pycotap/ci/coverage)
 [![PyPI
 version](https://badge.fury.io/py/pycotap.svg)](https://badge.fury.io/py/pycotap)
 
 `pycotap` is a simple Python test runner for `unittest` that outputs
 [Test Anything Protocol](http://testanything.org) results to standard
 output (similar to what [`tape`](https://www.npmjs.com/package/tape)
 does for JavaScript).
 
 Contrary to other TAP runners for Python, `pycotap` ...
 
-  - ... prints TAP (and *only* TAP) to standard output instead of to a
-    separate file, allowing you to pipe it directly to TAP pretty
-    printers and processors (such as the ones listed on the [`tape`
-    page](https://www.npmjs.com/package/tape#pretty-reporters)). By
-    piping it to other consumers, you can avoid the need to add specific
-    test runners to your test code. Since the TAP results are printed as
-    they come in, the consumers can directly display results while the
-    tests are run.
-  - ... only contains a TAP reporter, so no parsers, no frameworks, no
-    dependencies, ...
-  - ... is configurable: you can choose how you want the test output and
-    test result diagnostics to end up in your TAP output (as TAP
-    diagnostics, YAML blocks, or attachments). The defaults are
-    optimized for a [Jenkins](http://jenkins-ci.org) based flow.
-
-> Nice work with pycotap\! I took a "kitchen sink" approach with tappy
-> so I'm glad someone made a no dependency TAP unittest runner. :) --
-> [Matt Layman](http://www.mattlayman.com), author of
+- ... prints TAP (and *only* TAP) to standard output instead of to a
+  separate file, allowing you to pipe it directly to TAP pretty printers
+  and processors (such as the ones listed on the [`tape`
+  page](https://www.npmjs.com/package/tape#pretty-reporters)). By piping
+  it to other consumers, you can avoid the need to add specific test
+  runners to your test code. Since the TAP results are printed as they
+  come in, the consumers can directly display results while the tests
+  are run.
+- ... only contains a TAP reporter, so no parsers, no frameworks, no
+  dependencies, ...
+- ... is configurable: you can choose how you want the test output and
+  test result diagnostics to end up in your TAP output (as TAP
+  diagnostics, YAML blocks, or attachments). The defaults are optimized
+  for a [Jenkins](http://jenkins-ci.org) based flow.
+
+> Nice work with pycotap! I took a "kitchen sink" approach with tappy so
+> I'm glad someone made a no dependency TAP unittest runner. :) -- [Matt
+> Layman](http://www.mattlayman.com), author of
 > [tappy](http://tappy.readthedocs.org/en/latest/)
 
 ## Installation
 
 You can install the package directly from
 [PIP](https://pypi.python.org):
 
@@ -79,23 +80,23 @@
 [tap-dot](https://github.com/scottcorgan/tap-dot):
 
     $ python -mpycotap test_example  | faucet
     ⨯ __main__.MyTests.test_that_it_fails
     ✓ __main__.MyTests.test_that_it_passes
     ✓ __main__.MyTests.test_that_it_skips # Skipped: not finished yet
     ⨯ fail  1
-    
-    
+
+
     $ python -mpycotap test_example  | tap-dot 
     x  ..  
-    
+
       3 tests
       2 passed
       1 failed  
-    
+
       Failed Tests:   There was 1 failure
         x __main__.MyTests.test_that_it_fails
 
 ### Bring your own `__main__`
 
 You can create a `TAPTestRunner` yourself (e.g. to pass custom
 parameters), and use it to drive your own main function.
@@ -118,53 +119,52 @@
     ok 3 __main__.MyTests.test_that_it_skips # Skipped: not finished yet
     1..3
 
 ## API
 
 ### `TAPTestRunner([message_log], [test_output_log])`
 
-  - `message_log` (Optional; Default: `LogMode.LogToYAML`):  
-    What to do with test messages (e.g. assertion failure details). See
-    `LogMode` for possible values.
-  - `test_output_log` (Optional; Default: `LogMode.LogToDiagnostics`):  
-    What to do with output printed by the tests. See `LogMode` for
-    possible values.
+- `message_log` (Optional; Default: `LogMode.LogToYAML`):  
+  What to do with test messages (e.g. assertion failure details). See
+  `LogMode` for possible values.
+- `test_output_log` (Optional; Default: `LogMode.LogToDiagnostics`):  
+  What to do with output printed by the tests. See `LogMode` for
+  possible values.
 
 ### `LogMode`
 
 Enumeration of different destinations to log information. Possible
 values:
 
-  - `LogMode.LogToError`: Log all output to standard error. This means
-    no output information will end up in the TAP stream, and so will not
-    be processed by any processors.
-  - `LogMode.LogToDiagnostics`: Put output in a diagnostics message
-    after the test result. This means all output will end up in the TAP
-    stream. How this is displayed depends on the processor.
-  - `LogMode.LogToYAML`: Put output in a YAML block.
-  - `LogMode.LogToAttachment`: Put output in a downloadable attachment
-    in a YAML block. This is an extension supported by e.g.
-    [`tap4j`](http://tap4j.org).
+- `LogMode.LogToError`: Log all output to standard error. This means no
+  output information will end up in the TAP stream, and so will not be
+  processed by any processors.
+- `LogMode.LogToDiagnostics`: Put output in a diagnostics message after
+  the test result. This means all output will end up in the TAP stream.
+  How this is displayed depends on the processor.
+- `LogMode.LogToYAML`: Put output in a YAML block.
+- `LogMode.LogToAttachment`: Put output in a downloadable attachment in
+  a YAML block. This is an extension supported by e.g.
+  [`tap4j`](http://tap4j.org).
 
 ## Changelog
 
 ### 1.3.0 (2023-04-28)
 
-  - Fix problem with garbage output (thanks
-    [wjt](https://github.com/wjt))
+- Fix problem with garbage output (thanks [wjt](https://github.com/wjt))
 
 ### 1.1.0 (2015-07-29)
 
-  - Don't print message for expected failures
-  - Fix problem with unexpected success
+- Don't print message for expected failures
+- Fix problem with unexpected success
 
 ### 1.0.1 (2015-07-28)
 
-  - Fix problem with tests that cache `sys.std*` output streams
+- Fix problem with tests that cache `sys.std*` output streams
 
 ### 1.0.0 (2015-01-24)
 
-  - Initial stable version
+- Initial stable version
 
 ### 0.1.0 (2015-01-21)
 
-  - Initial version
+- Initial version
```

### Comparing `pycotap-1.3.0/pycotap/__init__.py` & `pycotap-1.3.1/pycotap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #!/usr/bin/env python
-# coding=utf-8
 
 # Copyright (c) 2015 Remko Tronçon (https://el-tramo.be)
 # Released under the MIT license
 # See COPYING for details
 
 import base64
 import sys
 import unittest
 
 if sys.hexversion >= 0x03000000:
   from io import StringIO
 else:
-  from StringIO import StringIO
+  from StringIO import StringIO  # pylint: disable=import-error
 
 
 # Log modes
 class LogMode(object):
   LogToError, LogToDiagnostics, LogToYAML, LogToAttachment = range(4)
 
 
@@ -71,16 +70,16 @@
 
   def ok(self, test, directive = None):
     self.print_result("ok", test, directive)
 
   def not_ok(self, test):
     self.print_result("not ok", test)
 
-  def startTest(self, test):
-    super(TAPTestResult, self).startTest(test)
+  # def startTest(self, test):
+  #   super(TAPTestResult, self).startTest(test)
 
   def stopTest(self, test):
     super(TAPTestResult, self).stopTest(test)
     if self.message_log == self.test_output_log:
       logs = [(self.message_log, self.message, "output")]
     else:
       logs = [
```

### Comparing `pycotap-1.3.0/pycotap.egg-info/PKG-INFO` & `pycotap-1.3.1/pycotap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pycotap
-Version: 1.3.0
+Version: 1.3.1
 Summary: A tiny test runner that outputs TAP results to standard output.
-Home-page: https://el-tramo.be/pycotap
+Home-page: https://github.com/remko/pycotap
 Author: Remko Tronçon
-Author-email: dev@el-tramo.be
+Author-email: 08cage-calm@icloud.com
 License: MIT
 Keywords: tap unittest testing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -34,8 +34,8 @@
 
 - ... is configurable: you can choose how you want the test output and test result
   diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
   attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
   flow.
 
 Documentation and examples can be found on `the pycotap page 
-<https://el-tramo.be/pycotap>`_.
+<https://github.com/remko/pycotap>`_.
```

### Comparing `pycotap-1.3.0/pyproject.toml` & `pycotap-1.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -30,7 +30,11 @@
 continuation_align_style = "valign-right"
 i18n_function_call = ["_", "N_"]
 indent_dictionary_value = true
 split_before_closing_bracket = false
 spaces_around_default_or_named_assign = true
 dedent_closing_brackets = true
 blank_line_before_nested_class_or_def = false
+
+[tool.pylint.MESSAGES_CONTROL]
+disable= "C,I,R,bad-indentation"
+
```

### Comparing `pycotap-1.3.0/setup.py` & `pycotap-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import find_packages, setup
 
 setup(
-    name="pycotap",
-    version="1.3.0",
-    packages=find_packages(),
-
-    # Metadata
-    author="Remko Tronçon",
-    author_email="dev@el-tramo.be",
-    description=
-    """A tiny test runner that outputs TAP results to standard output.""",
-    long_description="""
+  name = "pycotap",
+  version = "1.3.1",
+  packages = find_packages(),
+
+  # Metadata
+  author = "Remko Tronçon",
+  author_email = "08cage-calm@icloud.com",
+  description = """A tiny test runner that outputs TAP results to standard output.""",
+  long_description = """
 `pycotap` is a simple Python test runner for ``unittest`` that outputs 
 `Test Anything Protocol <http://testanything.org>`_ results directly to standard output.
 
 Contrary to other TAP runners for Python, ``pycotap`` ...
 
 - ... prints TAP (and *only* TAP) to standard output instead of to a separate file,
   allowing you to pipe it directly to TAP pretty printers and processors 
@@ -32,20 +31,20 @@
 
 - ... is configurable: you can choose how you want the test output and test result
   diagnostics to end up in your TAP output (as TAP diagnostics, YAML blocks, or 
   attachments). The defaults are optimized for a `Jenkins <http://jenkins-ci.org>`_ based
   flow.
 
 Documentation and examples can be found on `the pycotap page 
-<https://el-tramo.be/pycotap>`_.
+<https://github.com/remko/pycotap>`_.
 """,
-    license="MIT",
-    keywords="tap unittest testing",
-    url="https://el-tramo.be/pycotap",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers", "Topic :: Utilities",
-        "License :: OSI Approved :: MIT License",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Topic :: Software Development :: Testing"
-    ],
-    data_files=[("", ["COPYING"])])
+  license = "MIT",
+  keywords = "tap unittest testing",
+  url = "https://github.com/remko/pycotap",
+  classifiers = [
+    "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers",
+    "Topic :: Utilities", "License :: OSI Approved :: MIT License",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "Topic :: Software Development :: Testing"
+  ],
+  data_files = [("", ["COPYING"])]
+)
```

### Comparing `pycotap-1.3.0/test/test.py` & `pycotap-1.3.1/test/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-#!/usr/bin/env python
-
-# pylint: disable=C0325,E402,E501
+#!/usr/bin/env python3
 
 import os
 import re
 import sys
 import unittest
 
 sys.path.append(os.path.join(os.path.dirname(__file__), ".."))
```

