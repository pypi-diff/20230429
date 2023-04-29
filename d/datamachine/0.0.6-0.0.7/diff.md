# Comparing `tmp/datamachine-0.0.6.tar.gz` & `tmp/datamachine-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamachine-0.0.6.tar", last modified: Tue Apr 25 17:17:36 2023, max compression
+gzip compressed data, was "datamachine-0.0.7.tar", last modified: Sat Apr 29 00:18:44 2023, max compression
```

## Comparing `datamachine-0.0.6.tar` & `datamachine-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.818833 datamachine-0.0.6/
--rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      755 2023-04-25 17:17:36.819497 datamachine-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      139 2023-04-13 18:21:44.000000 datamachine-0.0.6/README.md
--rw-rw-rw-   0        0        0      652 2023-04-25 17:16:16.000000 datamachine-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      634 2023-04-25 17:17:36.825620 datamachine-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.786955 datamachine-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.805210 datamachine-0.0.6/src/datamachine/
--rw-rw-rw-   0        0        0      234 2023-04-25 17:09:05.000000 datamachine-0.0.6/src/datamachine/__init__.py
--rw-rw-rw-   0        0        0     7768 2023-04-25 17:09:10.000000 datamachine-0.0.6/src/datamachine/_modular.py
--rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.6/src/datamachine/xxx.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:17:36.818353 datamachine-0.0.6/src/datamachine.egg-info/
--rw-rw-rw-   0        0        0      755 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-25 17:17:36.000000 datamachine-0.0.6/src/datamachine.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.460610 datamachine-0.0.7/
+-rw-rw-rw-   0        0        0     1074 2023-04-13 18:31:43.000000 datamachine-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     3657 2023-04-29 00:18:44.461425 datamachine-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3041 2023-04-28 23:48:04.000000 datamachine-0.0.7/README.md
+-rw-rw-rw-   0        0        0      652 2023-04-29 00:17:55.000000 datamachine-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      599 2023-04-29 00:18:44.462449 datamachine-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.443231 datamachine-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.449320 datamachine-0.0.7/src/datamachine/
+-rw-rw-rw-   0        0        0      270 2023-04-28 14:00:39.000000 datamachine-0.0.7/src/datamachine/__init__.py
+-rw-rw-rw-   0        0        0    10918 2023-04-29 00:15:15.000000 datamachine-0.0.7/src/datamachine/_modular.py
+-rw-rw-rw-   0        0        0     5051 2023-04-16 02:31:46.000000 datamachine-0.0.7/src/datamachine/xxx.py
+drwxrwxrwx   0        0        0        0 2023-04-29 00:18:44.460610 datamachine-0.0.7/src/datamachine.egg-info/
+-rw-rw-rw-   0        0        0     3657 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 00:18:44.000000 datamachine-0.0.7/src/datamachine.egg-info/top_level.txt
```

### Comparing `datamachine-0.0.6/LICENSE` & `datamachine-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `datamachine-0.0.6/pyproject.toml` & `datamachine-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamachine"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = []
 authors = [
   { name="Dave Killough", email="dave.killough@gmail.com" },
 ]
 description = "A data machine made of modular Python notebooks"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `datamachine-0.0.6/setup.cfg` & `datamachine-0.0.7/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 616d 6163 6869 6e65 0d0a   = datamachine..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 370d  version = 0.0.7.
 00000030: 0a61 7574 686f 7220 3d20 4461 7665 204b  .author = Dave K
 00000040: 696c 6c6f 7567 680d 0a61 7574 686f 725f  illough..author_
 00000050: 656d 6169 6c20 3d20 6461 7665 2e6b 696c  email = dave.kil
 00000060: 6c6f 7567 6840 676d 6169 6c2e 636f 6d0d  lough@gmail.com.
 00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
 00000080: 2064 6174 6120 6d61 6368 696e 6520 6d61   data machine ma
 00000090: 6465 206f 6620 6d6f 6475 6c61 7220 5079  de of modular Py
@@ -12,29 +12,27 @@
 000000b0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000c0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 000000d0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 000000e0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
 000000f0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
 00000100: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
 00000110: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00000120: 742f 6461 7461 6d61 6368 696e 650d 0a70  t/datamachine..p
-00000130: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
-00000140: 0942 7567 2054 7261 636b 6572 203d 202e  .Bug Tracker = .
-00000150: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000160: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000170: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000180: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-00000190: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-000001a0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
-000001b0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-000001c0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000001d0: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-000001e0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-000001f0: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000200: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000210: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000220: 3d33 2e36 0d0a 0d0a 5b6f 7074 696f 6e73  =3.6....[options
-00000230: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-00000240: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000250: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000260: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000270: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000120: 742f 6461 7461 6d61 6368 696e 650d 0a63  t/datamachine..c
+00000130: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+00000140: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000150: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000160: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
+00000170: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000180: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+00000190: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+000001a0: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+000001b0: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+000001c0: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+000001d0: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
+000001e0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
+000001f0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
+00000200: 360d 0a0d 0a5b 6f70 7469 6f6e 732e 7061  6....[options.pa
+00000210: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
+00000220: 6572 6520 3d20 7372 630d 0a0d 0a5b 6567  ere = src....[eg
+00000230: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+00000240: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+00000250: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `datamachine-0.0.6/src/datamachine/xxx.py` & `datamachine-0.0.7/src/datamachine/xxx.py`

 * *Files identical despite different names*

