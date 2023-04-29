# Comparing `tmp/sbase-4.9.8.tar.gz` & `tmp/sbase-4.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbase-4.9.8.tar", last modified: Fri Dec 16 22:49:54 2022, max compression
+gzip compressed data, was "sbase-4.9.9.tar", last modified: Sun Dec 18 20:07:35 2022, max compression
```

## Comparing `sbase-4.9.8.tar` & `sbase-4.9.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:49:54.660009 sbase-4.9.8/
--rw-r--r--   0 michael    (501) staff       (20)    69231 2022-12-16 22:49:54.660160 sbase-4.9.8/PKG-INFO
--rwxr-xr-x   0 michael    (501) staff       (20)    67417 2022-12-07 20:00:46.000000 sbase-4.9.8/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-16 22:49:54.659911 sbase-4.9.8/sbase.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)    69231 2022-12-16 22:49:54.000000 sbase-4.9.8/sbase.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      172 2022-12-16 22:49:54.000000 sbase-4.9.8/sbase.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-16 22:49:54.000000 sbase-4.9.8/sbase.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       20 2022-12-16 22:49:54.000000 sbase-4.9.8/sbase.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-16 22:49:54.000000 sbase-4.9.8/sbase.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2022-12-16 22:49:54.660339 sbase-4.9.8/setup.cfg
--rwxr-xr-x   0 michael    (501) staff       (20)     5009 2022-12-16 22:49:17.000000 sbase-4.9.8/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:35.172971 sbase-4.9.9/
+-rw-r--r--   0 michael    (501) staff       (20)    69231 2022-12-18 20:07:35.173128 sbase-4.9.9/PKG-INFO
+-rwxr-xr-x   0 michael    (501) staff       (20)    67417 2022-12-18 20:06:19.000000 sbase-4.9.9/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2022-12-18 20:07:35.172876 sbase-4.9.9/sbase.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)    69231 2022-12-18 20:07:35.000000 sbase-4.9.9/sbase.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      172 2022-12-18 20:07:35.000000 sbase-4.9.9/sbase.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-18 20:07:35.000000 sbase-4.9.9/sbase.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       20 2022-12-18 20:07:35.000000 sbase-4.9.9/sbase.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2022-12-18 20:07:35.000000 sbase-4.9.9/sbase.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2022-12-18 20:07:35.173304 sbase-4.9.9/setup.cfg
+-rwxr-xr-x   0 michael    (501) staff       (20)     5009 2022-12-18 20:05:28.000000 sbase-4.9.9/setup.py
```

### Comparing `sbase-4.9.8/PKG-INFO` & `sbase-4.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbase
-Version: 4.9.8
+Version: 4.9.9
 Summary: A complete web automation framework for end-to-end testing.
 Home-page: https://github.com/seleniumbase/SeleniumBase
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/seleniumbase/SeleniumBase/releases
@@ -53,15 +53,15 @@
 
 **[<img src="https://img.shields.io/badge/pypi-sbase-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/sbase) is a proxy for [<img src="https://img.shields.io/badge/pypi-seleniumbase-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/seleniumbase)**
 ****
 
 <!-- SeleniumBase Docs -->
 
 
-<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_p3.png" alt="SeleniumBase" title="SeleniumBase" width="382" /></a></p>
+<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="365" /></a></p>
 
 <h3 align="center"><img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /> <b>All-in-one Test Automation Framework</b> <img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /></h3>
 
 <p align="center"><a href="https://pypi.python.org/pypi/seleniumbase" target="_blank"><img src="https://img.shields.io/pypi/v/seleniumbase.svg?color=3399EE" alt="PyPI version" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/releases" target="_blank"><img src="https://img.shields.io/github/v/release/seleniumbase/SeleniumBase.svg?color=22AAEE" alt="GitHub version" /></a> <a href="https://seleniumbase.io"><img src="https://img.shields.io/badge/docs-seleniumbase.io-11BBAA.svg" alt="SeleniumBase Docs" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/actions" target="_blank"><img src="https://github.com/seleniumbase/SeleniumBase/workflows/CI%20build/badge.svg" alt="SeleniumBase GitHub Actions" /></a> <a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://badges.gitter.im/seleniumbase/SeleniumBase.svg" alt="SeleniumBase" /></a></p>
 
 <p align="center">
 <a href="#python_installation">🏄 Start</a> |
@@ -1238,9 +1238,9 @@
 <span><a href="https://github.com/seleniumbase/SeleniumBase"><img src="https://seleniumbase.github.io/img/social/share_github.svg" title="SeleniumBase on GitHub" alt="SeleniumBase on GitHub" width="43" /></a></span>
 <span><a href="https://www.facebook.com/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_facebook.svg" title="SeleniumBase on Facebook" alt="SeleniumBase on Facebook" width="37" /></a></span>
 <span><a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_gitter.svg" title="SeleniumBase on Gitter" alt="SeleniumBase on Gitter" width="35" /></a></span>
 <span><a href="https://instagram.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_instagram.svg" title="SeleniumBase on Instagram" alt="SeleniumBase on Instagram" width="33" /></a></span>
 <span><a href="https://twitter.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_twitter.svg" title="SeleniumBase on Twitter" alt="SeleniumBase on Twitter" width="39" /></a></span>
 </div></p>
 
-<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i2.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
+<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
 <p><a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/pypi/pyversions/seleniumbase.svg?color=22AAEE&logo=python&logoColor=FEDC54" title="Supported Python Versions" /></a></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sbase Version: 4.9.8 Summary: A complete web
+Metadata-Version: 2.1 Name: sbase Version: 4.9.9 Summary: A complete web
 automation framework for end-to-end testing. Home-page: https://github.com/
 seleniumbase/SeleniumBase Author: Michael Mintz Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz License: MIT Project-URL: Changelog, https://
 github.com/seleniumbase/SeleniumBase/releases Project-URL: Download, https://
 pypi.org/project/seleniumbase/#files Project-URL: Gitter, https://gitter.im/
 seleniumbase/SeleniumBase Project-URL: Slack, https://app.slack.com/client/
 T0ABCRTNX/C01SM888REZ Project-URL: Blog, https://seleniumbase.com/ Project-URL:
```

### Comparing `sbase-4.9.8/README.md` & `sbase-4.9.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 <meta property="og:site_name" content="SeleniumBase">
 <meta property="og:title" content="SeleniumBase: Python Web Automation and E2E Testing" />
 <meta property="og:description" content="Fast, easy, and reliable Web/UI testing with Python." />
 <meta property="og:keywords" content="Python, pytest, selenium, webdriver, testing, automation, seleniumbase, framework, dashboard, recorder, reports, screenshots">
 <meta property="og:image" content="https://seleniumbase.github.io/cdn/img/mac_sb_logo_5b.png" />
 <link rel="icon" href="https://seleniumbase.github.io/img/logo3b.png" />
 
-<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_p3.png" alt="SeleniumBase" title="SeleniumBase" width="382" /></a></p>
+<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="365" /></a></p>
 
 <h3 align="center"><img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /> <b>All-in-one Test Automation Framework</b> <img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /></h3>
 
 <p align="center"><a href="https://pypi.python.org/pypi/seleniumbase" target="_blank"><img src="https://img.shields.io/pypi/v/seleniumbase.svg?color=3399EE" alt="PyPI version" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/releases" target="_blank"><img src="https://img.shields.io/github/v/release/seleniumbase/SeleniumBase.svg?color=22AAEE" alt="GitHub version" /></a> <a href="https://seleniumbase.io"><img src="https://img.shields.io/badge/docs-seleniumbase.io-11BBAA.svg" alt="SeleniumBase Docs" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/actions" target="_blank"><img src="https://github.com/seleniumbase/SeleniumBase/workflows/CI%20build/badge.svg" alt="SeleniumBase GitHub Actions" /></a> <a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://badges.gitter.im/seleniumbase/SeleniumBase.svg" alt="SeleniumBase" /></a></p>
 
 <p align="center">
 <a href="#python_installation">🏄 Start</a> |
@@ -1191,9 +1191,9 @@
 <span><a href="https://github.com/seleniumbase/SeleniumBase"><img src="https://seleniumbase.github.io/img/social/share_github.svg" title="SeleniumBase on GitHub" alt="SeleniumBase on GitHub" width="43" /></a></span>
 <span><a href="https://www.facebook.com/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_facebook.svg" title="SeleniumBase on Facebook" alt="SeleniumBase on Facebook" width="37" /></a></span>
 <span><a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_gitter.svg" title="SeleniumBase on Gitter" alt="SeleniumBase on Gitter" width="35" /></a></span>
 <span><a href="https://instagram.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_instagram.svg" title="SeleniumBase on Instagram" alt="SeleniumBase on Instagram" width="33" /></a></span>
 <span><a href="https://twitter.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_twitter.svg" title="SeleniumBase on Twitter" alt="SeleniumBase on Twitter" width="39" /></a></span>
 </div></p>
 
-<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i2.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
+<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
 <p><a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/pypi/pyversions/seleniumbase.svg?color=22AAEE&logo=python&logoColor=FEDC54" title="Supported Python Versions" /></a></p>
```

### Comparing `sbase-4.9.8/sbase.egg-info/PKG-INFO` & `sbase-4.9.9/sbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbase
-Version: 4.9.8
+Version: 4.9.9
 Summary: A complete web automation framework for end-to-end testing.
 Home-page: https://github.com/seleniumbase/SeleniumBase
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/seleniumbase/SeleniumBase/releases
@@ -53,15 +53,15 @@
 
 **[<img src="https://img.shields.io/badge/pypi-sbase-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/sbase) is a proxy for [<img src="https://img.shields.io/badge/pypi-seleniumbase-22AAEE.svg" alt="pypi" />](https://pypi.python.org/pypi/seleniumbase)**
 ****
 
 <!-- SeleniumBase Docs -->
 
 
-<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_p3.png" alt="SeleniumBase" title="SeleniumBase" width="382" /></a></p>
+<p align="center"><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="365" /></a></p>
 
 <h3 align="center"><img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /> <b>All-in-one Test Automation Framework</b> <img src="https://seleniumbase.github.io/cdn/img/python_logo.png" title="Python" width="29" /></h3>
 
 <p align="center"><a href="https://pypi.python.org/pypi/seleniumbase" target="_blank"><img src="https://img.shields.io/pypi/v/seleniumbase.svg?color=3399EE" alt="PyPI version" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/releases" target="_blank"><img src="https://img.shields.io/github/v/release/seleniumbase/SeleniumBase.svg?color=22AAEE" alt="GitHub version" /></a> <a href="https://seleniumbase.io"><img src="https://img.shields.io/badge/docs-seleniumbase.io-11BBAA.svg" alt="SeleniumBase Docs" /></a> <a href="https://github.com/seleniumbase/SeleniumBase/actions" target="_blank"><img src="https://github.com/seleniumbase/SeleniumBase/workflows/CI%20build/badge.svg" alt="SeleniumBase GitHub Actions" /></a> <a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://badges.gitter.im/seleniumbase/SeleniumBase.svg" alt="SeleniumBase" /></a></p>
 
 <p align="center">
 <a href="#python_installation">🏄 Start</a> |
@@ -1238,9 +1238,9 @@
 <span><a href="https://github.com/seleniumbase/SeleniumBase"><img src="https://seleniumbase.github.io/img/social/share_github.svg" title="SeleniumBase on GitHub" alt="SeleniumBase on GitHub" width="43" /></a></span>
 <span><a href="https://www.facebook.com/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_facebook.svg" title="SeleniumBase on Facebook" alt="SeleniumBase on Facebook" width="37" /></a></span>
 <span><a href="https://gitter.im/seleniumbase/SeleniumBase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_gitter.svg" title="SeleniumBase on Gitter" alt="SeleniumBase on Gitter" width="35" /></a></span>
 <span><a href="https://instagram.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_instagram.svg" title="SeleniumBase on Instagram" alt="SeleniumBase on Instagram" width="33" /></a></span>
 <span><a href="https://twitter.com/seleniumbase" target="_blank"><img src="https://seleniumbase.github.io/img/social/share_twitter.svg" title="SeleniumBase on Twitter" alt="SeleniumBase on Twitter" width="39" /></a></span>
 </div></p>
 
-<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i2.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
+<p><a href="https://github.com/seleniumbase/SeleniumBase/"><img src="https://seleniumbase.github.io/cdn/img/sb_logo_i3.png" alt="SeleniumBase" title="SeleniumBase" width="240" /></a></p>
 <p><a href="https://www.python.org/downloads/" target="_blank"><img src="https://img.shields.io/pypi/pyversions/seleniumbase.svg?color=22AAEE&logo=python&logoColor=FEDC54" title="Supported Python Versions" /></a></p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sbase Version: 4.9.8 Summary: A complete web
+Metadata-Version: 2.1 Name: sbase Version: 4.9.9 Summary: A complete web
 automation framework for end-to-end testing. Home-page: https://github.com/
 seleniumbase/SeleniumBase Author: Michael Mintz Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz License: MIT Project-URL: Changelog, https://
 github.com/seleniumbase/SeleniumBase/releases Project-URL: Download, https://
 pypi.org/project/seleniumbase/#files Project-URL: Gitter, https://gitter.im/
 seleniumbase/SeleniumBase Project-URL: Slack, https://app.slack.com/client/
 T0ABCRTNX/C01SM888REZ Project-URL: Blog, https://seleniumbase.com/ Project-URL:
```

### Comparing `sbase-4.9.8/setup.py` & `sbase-4.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name='sbase',
-    version='4.9.8',
+    version='4.9.9',
     description='A complete web automation framework for end-to-end testing.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/seleniumbase/SeleniumBase',
     project_urls={
         "Changelog": "https://github.com/seleniumbase/SeleniumBase/releases",
         "Download": "https://pypi.org/project/seleniumbase/#files",
@@ -104,15 +104,15 @@
         "Topic :: Software Development :: Testing",
         "Topic :: Software Development :: Testing :: Acceptance",
         "Topic :: Software Development :: Testing :: Traffic Generation",
         "Topic :: Utilities",
     ],
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",  # noqa: E501
     install_requires=[
-        'seleniumbase>=4.9.8',
+        'seleniumbase>=4.9.9',
         ],
     packages=[
         ],
     entry_points={
         'nose.plugins': [
             ],
         'pytest11': [
```

