# Comparing `tmp/cryptoparser-0.8.5.tar.gz` & `tmp/cryptoparser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/usr/src/dist/tmp7T8gsl/cryptoparser-0.8.5.tar", last modified: Tue Apr  4 22:31:20 2023, max compression
+gzip compressed data, was "cryptoparser-0.9.0.tar", last modified: Sat Apr 29 12:09:24 2023, max compression
```

## Comparing `cryptoparser-0.8.5.tar` & `cryptoparser-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/
--rw-r--r--   0 root         (0) root         (0)     3605 2023-04-03 22:15:11.000000 cryptoparser-0.8.5/setup.py
--rw-r--r--   0 root         (0) root         (0)     8617 2023-04-02 12:41:14.000000 cryptoparser-0.8.5/CONTRIBUTING.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser.egg-info/
--rw-rw-r--   0 root         (0) root         (0)       13 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)     3591 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1131 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)      268 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)    16726 2022-09-04 16:33:32.000000 cryptoparser-0.8.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     3591 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8141 2023-04-03 22:15:11.000000 cryptoparser-0.8.5/CHANGELOG.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser/tls/
--rw-r--r--   0 root         (0) root         (0)    16107 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/mysql.py
--rw-r--r--   0 root         (0) root         (0)     7009 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/rdp.py
--rw-r--r--   0 root         (0) root         (0)      645 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/ciphersuite.py
--rw-r--r--   0 root         (0) root         (0)     3953 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/record.py
--rw-r--r--   0 root         (0) root         (0)     3166 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/grease.py
--rw-r--r--   0 root         (0) root         (0)     5802 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/ldap.py
--rw-r--r--   0 root         (0) root         (0)    38089 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/subprotocol.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/version.py
--rw-r--r--   0 root         (0) root         (0)     1618 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/postgresql.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-04-28 17:35:12.000000 cryptoparser-0.8.5/cryptoparser/tls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      884 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/algorithm.py
--rw-r--r--   0 root         (0) root         (0)    39461 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/tls/extension.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser/httpx/
--rw-r--r--   0 root         (0) root         (0)    19581 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/httpx/header.py
--rw-r--r--   0 root         (0) root         (0)    16124 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/httpx/parse.py
--rw-r--r--   0 root         (0) root         (0)      700 2022-09-04 16:33:32.000000 cryptoparser-0.8.5/cryptoparser/httpx/version.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-04 16:33:32.000000 cryptoparser-0.8.5/cryptoparser/httpx/__init__.py
--rw-rw-r--   0 root         (0) root         (0)        0 2022-04-23 18:10:38.000000 cryptoparser-0.8.5/cryptoparser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser/common/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/utils.py
--rw-r--r--   0 root         (0) root         (0)    32485 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/parse.py
--rw-r--r--   0 root         (0) root         (0)    29870 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/base.py
--rw-rw-r--   0 root         (0) root         (0)        0 2021-04-28 17:35:12.000000 cryptoparser-0.8.5/cryptoparser/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      655 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/exception.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/x509.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/key.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/common/classes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 22:31:20.000000 cryptoparser-0.8.5/cryptoparser/ssh/
--rw-r--r--   0 root         (0) root         (0)     2201 2022-09-04 16:33:32.000000 cryptoparser-0.8.5/cryptoparser/ssh/record.py
--rw-r--r--   0 root         (0) root         (0)    20265 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/ssh/subprotocol.py
--rw-r--r--   0 root         (0) root         (0)     6215 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/ssh/version.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-04 16:33:32.000000 cryptoparser-0.8.5/cryptoparser/ssh/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33359 2023-04-03 22:09:54.000000 cryptoparser-0.8.5/cryptoparser/ssh/key.py
--rw-r--r--   0 root         (0) root         (0)      127 2023-04-04 22:28:24.000000 cryptoparser-0.8.5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      909 2023-04-02 12:41:14.000000 cryptoparser-0.8.5/README.rst
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-02 12:41:14.000000 cryptoparser-0.8.5/MANIFEST.in
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.511059 cryptoparser-0.9.0/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8322 2023-04-29 11:18:56.000000 cryptoparser-0.9.0/CHANGELOG.rst
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     8617 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    16726 2023-04-06 21:12:48.000000 cryptoparser-0.9.0/LICENSE.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       39 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/MANIFEST.in
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3263 2023-04-29 12:09:24.511059 cryptoparser-0.9.0/PKG-INFO
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      909 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/README.rst
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.504059 cryptoparser-0.9.0/cryptoparser/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2022-04-23 18:10:38.000000 cryptoparser-0.9.0/cryptoparser/__init__.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.507059 cryptoparser-0.9.0/cryptoparser/common/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2021-04-28 17:35:12.000000 cryptoparser-0.9.0/cryptoparser/common/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    29870 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/base.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1714 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/classes.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      655 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/exception.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      894 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/key.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    32485 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/parse.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1051 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/utils.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      583 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/common/x509.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.508059 cryptoparser-0.9.0/cryptoparser/httpx/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2022-09-04 16:33:32.000000 cryptoparser-0.9.0/cryptoparser/httpx/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    19581 2023-04-29 07:15:22.000000 cryptoparser-0.9.0/cryptoparser/httpx/header.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    16124 2023-04-29 07:15:22.000000 cryptoparser-0.9.0/cryptoparser/httpx/parse.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      700 2022-09-04 16:33:32.000000 cryptoparser-0.9.0/cryptoparser/httpx/version.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.509059 cryptoparser-0.9.0/cryptoparser/ssh/
+-rw-r--r--   0 coroner   (1000) coroner   (1000)        0 2022-09-04 16:33:32.000000 cryptoparser-0.9.0/cryptoparser/ssh/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    33359 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/ssh/key.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2201 2023-04-06 21:12:48.000000 cryptoparser-0.9.0/cryptoparser/ssh/record.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    20265 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/ssh/subprotocol.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     6215 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/ssh/version.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.511059 cryptoparser-0.9.0/cryptoparser/tls/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        0 2021-04-28 17:35:12.000000 cryptoparser-0.9.0/cryptoparser/tls/__init__.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      884 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/algorithm.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      645 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/ciphersuite.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    39461 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/extension.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3166 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/grease.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     5802 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/ldap.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    16107 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/mysql.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     7217 2023-04-29 07:52:48.000000 cryptoparser-0.9.0/cryptoparser/tls/openvpn.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     1618 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/postgresql.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     7009 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/rdp.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3953 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/record.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)    38089 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/subprotocol.py
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     2369 2023-04-06 21:13:01.000000 cryptoparser-0.9.0/cryptoparser/tls/version.py
+drwxr-xr-x   0 coroner   (1000) coroner   (1000)        0 2023-04-29 12:09:24.505059 cryptoparser-0.9.0/cryptoparser.egg-info/
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)     3263 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/PKG-INFO
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)     1159 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/SOURCES.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)        1 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/dependency_links.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)      268 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/requires.txt
+-rw-rw-r--   0 coroner   (1000) coroner   (1000)       13 2023-04-29 12:09:24.000000 cryptoparser-0.9.0/cryptoparser.egg-info/top_level.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)      127 2023-04-06 21:14:45.000000 cryptoparser-0.9.0/requirements.txt
+-rw-r--r--   0 coroner   (1000) coroner   (1000)       38 2023-04-29 12:09:24.512059 cryptoparser-0.9.0/setup.cfg
+-rw-r--r--   0 coroner   (1000) coroner   (1000)     3605 2023-04-29 11:22:50.000000 cryptoparser-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cryptoparser-0.8.5/setup.py` & `cryptoparser-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     test_loader = unittest.TestLoader()
     test_suite = test_loader.discover('test', pattern='test_*.py')
     return test_suite
 
 
 setup(
     name='cryptoparser',
-    version='0.8.5',
+    version='0.9.0',
     description='Fast and flexible security protocol parser and generator',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Szilárd Pfeiffer',
     author_email='coroner@pfeifferszilard.hu',
     maintainer='Szilárd Pfeiffer',
     maintainer_email='coroner@pfeifferszilard.hu',
```

### Comparing `cryptoparser-0.8.5/CONTRIBUTING.rst` & `cryptoparser-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser.egg-info/PKG-INFO` & `cryptoparser-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,22 @@
 Metadata-Version: 2.1
 Name: cryptoparser
-Version: 0.8.5
+Version: 0.9.0
 Summary: Fast and flexible security protocol parser and generator
-Home-page: UNKNOWN
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
-Project-URL: Source, https://gitlab.com/coroner/cryptoparser
-Project-URL: Documentation, https://cryptoparser.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/coroner/cryptoparser
-Project-URL: Issues, https://gitlab.com/coroner/cryptoparser/-/issues
 Project-URL: Changelog, https://cryptoparser.readthedocs.io/en/latest/changelog
-Description: **CryptoParser** is a cryptographic protocol (TLS, SSH) and security-related protocol piece (HTTP headers) parser. It
-        is neither a comprehensive nor a secure implementation of any cryptographic protocol. The goal is to support
-        testing cryptographic libraries or analysing cryptography-realted settings of application servers such as
-        `CryptoLyzer <https://cryptolyzer.readthedocs.io/>`__ does.
-        
-        Usage
-        -----
-        
-        Pip
-        ^^^
-        
-        .. code:: shell
-        
-           pip install cryptoparser
-        
-        Support
-        -------
-        
-        Python implementation
-        ^^^^^^^^^^^^^^^^^^^^^
-        
-        -  CPython (2.7, 3.3+)
-        -  PyPy (2.7, 3.5+)
-        
-        Operating systems
-        ^^^^^^^^^^^^^^^^^
-        
-        -  Linux
-        -  macOS
-        -  Windows
-        
-        License
-        -------
-        
-        The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
-        
-        A non-comprehensive, but straightforward description of MPL 2.0 can be found at
-        `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
-        
+Project-URL: Documentation, https://cryptoparser.readthedocs.io/en/latest/
+Project-URL: Issues, https://gitlab.com/coroner/cryptoparser/-/issues
+Project-URL: Source, https://gitlab.com/coroner/cryptoparser
 Keywords: ssl tls gost ja3 ldap rdp ssh hsts
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -83,9 +42,49 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: pylint
 Provides-Extra: pep8
+Provides-Extra: pylint
+License-File: LICENSE.txt
+
+**CryptoParser** is a cryptographic protocol (TLS, SSH) and security-related protocol piece (HTTP headers) parser. It
+is neither a comprehensive nor a secure implementation of any cryptographic protocol. The goal is to support
+testing cryptographic libraries or analysing cryptography-realted settings of application servers such as
+`CryptoLyzer <https://cryptolyzer.readthedocs.io/>`__ does.
+
+Usage
+-----
+
+Pip
+^^^
+
+.. code:: shell
+
+   pip install cryptoparser
+
+Support
+-------
+
+Python implementation
+^^^^^^^^^^^^^^^^^^^^^
+
+-  CPython (2.7, 3.3+)
+-  PyPy (2.7, 3.5+)
+
+Operating systems
+^^^^^^^^^^^^^^^^^
+
+-  Linux
+-  macOS
+-  Windows
+
+License
+-------
+
+The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
+
+A non-comprehensive, but straightforward description of MPL 2.0 can be found at
+`Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
```

### Comparing `cryptoparser-0.8.5/cryptoparser.egg-info/SOURCES.txt` & `cryptoparser-0.9.0/cryptoparser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,12 +31,13 @@
 cryptoparser/tls/__init__.py
 cryptoparser/tls/algorithm.py
 cryptoparser/tls/ciphersuite.py
 cryptoparser/tls/extension.py
 cryptoparser/tls/grease.py
 cryptoparser/tls/ldap.py
 cryptoparser/tls/mysql.py
+cryptoparser/tls/openvpn.py
 cryptoparser/tls/postgresql.py
 cryptoparser/tls/rdp.py
 cryptoparser/tls/record.py
 cryptoparser/tls/subprotocol.py
 cryptoparser/tls/version.py
```

### Comparing `cryptoparser-0.8.5/LICENSE.txt` & `cryptoparser-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/PKG-INFO` & `cryptoparser-0.9.0/cryptoparser.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,22 @@
 Metadata-Version: 2.1
 Name: cryptoparser
-Version: 0.8.5
+Version: 0.9.0
 Summary: Fast and flexible security protocol parser and generator
-Home-page: UNKNOWN
 Author: Szilárd Pfeiffer
 Author-email: coroner@pfeifferszilard.hu
 Maintainer: Szilárd Pfeiffer
 Maintainer-email: coroner@pfeifferszilard.hu
 License: MPL-2.0
-Project-URL: Source, https://gitlab.com/coroner/cryptoparser
-Project-URL: Documentation, https://cryptoparser.readthedocs.io/en/latest/
 Project-URL: Homepage, https://gitlab.com/coroner/cryptoparser
-Project-URL: Issues, https://gitlab.com/coroner/cryptoparser/-/issues
 Project-URL: Changelog, https://cryptoparser.readthedocs.io/en/latest/changelog
-Description: **CryptoParser** is a cryptographic protocol (TLS, SSH) and security-related protocol piece (HTTP headers) parser. It
-        is neither a comprehensive nor a secure implementation of any cryptographic protocol. The goal is to support
-        testing cryptographic libraries or analysing cryptography-realted settings of application servers such as
-        `CryptoLyzer <https://cryptolyzer.readthedocs.io/>`__ does.
-        
-        Usage
-        -----
-        
-        Pip
-        ^^^
-        
-        .. code:: shell
-        
-           pip install cryptoparser
-        
-        Support
-        -------
-        
-        Python implementation
-        ^^^^^^^^^^^^^^^^^^^^^
-        
-        -  CPython (2.7, 3.3+)
-        -  PyPy (2.7, 3.5+)
-        
-        Operating systems
-        ^^^^^^^^^^^^^^^^^
-        
-        -  Linux
-        -  macOS
-        -  Windows
-        
-        License
-        -------
-        
-        The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
-        
-        A non-comprehensive, but straightforward description of MPL 2.0 can be found at
-        `Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
-        
+Project-URL: Documentation, https://cryptoparser.readthedocs.io/en/latest/
+Project-URL: Issues, https://gitlab.com/coroner/cryptoparser/-/issues
+Project-URL: Source, https://gitlab.com/coroner/cryptoparser
 Keywords: ssl tls gost ja3 ldap rdp ssh hsts
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Framework :: tox
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
@@ -83,9 +42,49 @@
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing :: Traffic Generation
 Classifier: Topic :: Software Development :: Testing
 Description-Content-Type: text/x-rst
 Provides-Extra: test
-Provides-Extra: pylint
 Provides-Extra: pep8
+Provides-Extra: pylint
+License-File: LICENSE.txt
+
+**CryptoParser** is a cryptographic protocol (TLS, SSH) and security-related protocol piece (HTTP headers) parser. It
+is neither a comprehensive nor a secure implementation of any cryptographic protocol. The goal is to support
+testing cryptographic libraries or analysing cryptography-realted settings of application servers such as
+`CryptoLyzer <https://cryptolyzer.readthedocs.io/>`__ does.
+
+Usage
+-----
+
+Pip
+^^^
+
+.. code:: shell
+
+   pip install cryptoparser
+
+Support
+-------
+
+Python implementation
+^^^^^^^^^^^^^^^^^^^^^
+
+-  CPython (2.7, 3.3+)
+-  PyPy (2.7, 3.5+)
+
+Operating systems
+^^^^^^^^^^^^^^^^^
+
+-  Linux
+-  macOS
+-  Windows
+
+License
+-------
+
+The code is available under the terms of Mozilla Public License Version 2.0 (MPL 2.0).
+
+A non-comprehensive, but straightforward description of MPL 2.0 can be found at
+`Choose an open source license <https://choosealicense.com/licenses#mpl-2.0>`__ website.
```

### Comparing `cryptoparser-0.8.5/CHANGELOG.rst` & `cryptoparser-0.9.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+0.9.0 - 2023-04-29
+------------------
+
+-  TLS (``tls``)
+
+   -  Generic
+
+      -  protocol item classes for `OpenVPN <https://en.wikipedia.org/wiki/OpenVPN>`__ support (#62)
+
 0.8.5 - 2023-04-02
 ------------------
 
    -  Generic
 
       -  move data classes to `CryptoDataHub repository <https://gitlab.com/coroner/cryptodatahub>`__ (#67)
 
@@ -65,15 +74,15 @@
 -  update contributing to the latest version from contribution-guide.org
 
 0.7.1 - 2021-09-20
 ------------------
 
 -  TLS (``tls``)
 
-   -  protocol item classes for RDP support (#44)
+   -  protocol item classes for PostgreSQL support (#44)
 
 0.7.0 - 2021-09-02
 ------------------
 
 -  TLS (``tls``)
 
    -  Extensions (``extensions``)
```

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/mysql.py` & `cryptoparser-0.9.0/cryptoparser/tls/mysql.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/rdp.py` & `cryptoparser-0.9.0/cryptoparser/tls/rdp.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/ciphersuite.py` & `cryptoparser-0.9.0/cryptoparser/tls/ciphersuite.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/record.py` & `cryptoparser-0.9.0/cryptoparser/tls/record.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/grease.py` & `cryptoparser-0.9.0/cryptoparser/tls/grease.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/ldap.py` & `cryptoparser-0.9.0/cryptoparser/tls/ldap.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/subprotocol.py` & `cryptoparser-0.9.0/cryptoparser/tls/subprotocol.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/version.py` & `cryptoparser-0.9.0/cryptoparser/tls/version.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/postgresql.py` & `cryptoparser-0.9.0/cryptoparser/tls/postgresql.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/algorithm.py` & `cryptoparser-0.9.0/cryptoparser/tls/algorithm.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/tls/extension.py` & `cryptoparser-0.9.0/cryptoparser/tls/extension.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/httpx/header.py` & `cryptoparser-0.9.0/cryptoparser/httpx/header.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/httpx/parse.py` & `cryptoparser-0.9.0/cryptoparser/httpx/parse.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/httpx/version.py` & `cryptoparser-0.9.0/cryptoparser/httpx/version.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/utils.py` & `cryptoparser-0.9.0/cryptoparser/common/utils.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/parse.py` & `cryptoparser-0.9.0/cryptoparser/common/parse.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/base.py` & `cryptoparser-0.9.0/cryptoparser/common/base.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/exception.py` & `cryptoparser-0.9.0/cryptoparser/common/exception.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/x509.py` & `cryptoparser-0.9.0/cryptoparser/common/x509.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/key.py` & `cryptoparser-0.9.0/cryptoparser/common/key.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/common/classes.py` & `cryptoparser-0.9.0/cryptoparser/common/classes.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/ssh/record.py` & `cryptoparser-0.9.0/cryptoparser/ssh/record.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/ssh/subprotocol.py` & `cryptoparser-0.9.0/cryptoparser/ssh/subprotocol.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/ssh/version.py` & `cryptoparser-0.9.0/cryptoparser/ssh/version.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/cryptoparser/ssh/key.py` & `cryptoparser-0.9.0/cryptoparser/ssh/key.py`

 * *Files identical despite different names*

### Comparing `cryptoparser-0.8.5/README.rst` & `cryptoparser-0.9.0/README.rst`

 * *Files identical despite different names*

