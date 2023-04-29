# Comparing `tmp/bird-ospf-link-db-parser-1.1.0.tar.gz` & `tmp/bird-ospf-link-db-parser-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bird-ospf-link-db-parser-1.1.0.tar", last modified: Sat Apr 29 07:21:54 2023, max compression
+gzip compressed data, was "bird-ospf-link-db-parser-1.1.1.tar", last modified: Sat Apr 29 07:28:20 2023, max compression
```

## Comparing `bird-ospf-link-db-parser-1.1.0.tar` & `bird-ospf-link-db-parser-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 07:21:54.506443 bird-ospf-link-db-parser-1.1.0/
--rw-rw-rw-   0        0        0     1094 2023-04-16 04:36:39.000000 bird-ospf-link-db-parser-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 07:07:22.000000 bird-ospf-link-db-parser-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5218 2023-04-29 07:21:54.505443 bird-ospf-link-db-parser-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3512 2023-04-29 07:19:04.000000 bird-ospf-link-db-parser-1.1.0/README.md
--rw-rw-rw-   0        0        0      830 2023-04-29 07:21:44.000000 bird-ospf-link-db-parser-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 07:21:54.506443 bird-ospf-link-db-parser-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 07:21:54.479443 bird-ospf-link-db-parser-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 07:21:54.496444 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/
--rw-rw-rw-   0        0        0     5218 2023-04-29 07:21:54.000000 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-29 07:21:54.000000 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 07:21:54.000000 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-29 07:21:54.000000 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-04-29 07:21:54.000000 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 07:21:54.000000 bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 07:21:54.501443 bird-ospf-link-db-parser-1.1.0/src/bird_parser/
--rw-rw-rw-   0        0        0        0 2023-04-16 04:38:40.000000 bird-ospf-link-db-parser-1.1.0/src/bird_parser/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-29 07:01:45.000000 bird-ospf-link-db-parser-1.1.0/src/bird_parser/main.py
--rw-rw-rw-   0        0        0     6161 2023-04-29 06:58:21.000000 bird-ospf-link-db-parser-1.1.0/src/bird_parser/output_schema.json
--rw-rw-rw-   0        0        0     4159 2023-04-29 05:06:33.000000 bird-ospf-link-db-parser-1.1.0/src/bird_parser/parse_bird_output.py
--rw-rw-rw-   0        0        0     1644 2023-04-29 05:07:09.000000 bird-ospf-link-db-parser-1.1.0/src/bird_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 07:21:54.504443 bird-ospf-link-db-parser-1.1.0/test/
--rw-rw-rw-   0        0        0     3290 2023-04-29 04:12:24.000000 bird-ospf-link-db-parser-1.1.0/test/test_comprehensive.py
--rw-rw-rw-   0        0        0     1100 2023-04-29 05:20:14.000000 bird-ospf-link-db-parser-1.1.0/test/test_live_data.py
--rw-rw-rw-   0        0        0     1736 2023-04-29 03:04:39.000000 bird-ospf-link-db-parser-1.1.0/test/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-04-29 07:28:20.294714 bird-ospf-link-db-parser-1.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-16 04:36:39.000000 bird-ospf-link-db-parser-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 07:07:22.000000 bird-ospf-link-db-parser-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5519 2023-04-29 07:28:20.293714 bird-ospf-link-db-parser-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3651 2023-04-29 07:24:56.000000 bird-ospf-link-db-parser-1.1.1/README.md
+-rw-rw-rw-   0        0        0     1011 2023-04-29 07:27:57.000000 bird-ospf-link-db-parser-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 07:28:20.294714 bird-ospf-link-db-parser-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 07:28:20.261714 bird-ospf-link-db-parser-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 07:28:20.284714 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/
+-rw-rw-rw-   0        0        0     5519 2023-04-29 07:28:20.000000 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-29 07:28:20.000000 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 07:28:20.000000 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-29 07:28:20.000000 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-04-29 07:28:20.000000 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 07:28:20.000000 bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 07:28:20.289714 bird-ospf-link-db-parser-1.1.1/src/bird_parser/
+-rw-rw-rw-   0        0        0        0 2023-04-16 04:38:40.000000 bird-ospf-link-db-parser-1.1.1/src/bird_parser/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-29 07:01:45.000000 bird-ospf-link-db-parser-1.1.1/src/bird_parser/main.py
+-rw-rw-rw-   0        0        0     6161 2023-04-29 06:58:21.000000 bird-ospf-link-db-parser-1.1.1/src/bird_parser/output_schema.json
+-rw-rw-rw-   0        0        0     4159 2023-04-29 05:06:33.000000 bird-ospf-link-db-parser-1.1.1/src/bird_parser/parse_bird_output.py
+-rw-rw-rw-   0        0        0     1644 2023-04-29 05:07:09.000000 bird-ospf-link-db-parser-1.1.1/src/bird_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 07:28:20.292714 bird-ospf-link-db-parser-1.1.1/test/
+-rw-rw-rw-   0        0        0     3290 2023-04-29 04:12:24.000000 bird-ospf-link-db-parser-1.1.1/test/test_comprehensive.py
+-rw-rw-rw-   0        0        0     1100 2023-04-29 05:20:14.000000 bird-ospf-link-db-parser-1.1.1/test/test_live_data.py
+-rw-rw-rw-   0        0        0     1736 2023-04-29 03:04:39.000000 bird-ospf-link-db-parser-1.1.1/test/test_simple.py
```

### Comparing `bird-ospf-link-db-parser-1.1.0/LICENSE.txt` & `bird-ospf-link-db-parser-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/PKG-INFO` & `bird-ospf-link-db-parser-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bird-ospf-link-db-parser
-Version: 1.1.0
-Summary: A simple Python package
+Version: 1.1.1
+Summary: Parse the text output from the BIRD Routing Daemon's OSPF link database into machine readable JSON
 Author-email: Andrew Dickinson <andrew.dickinson.0216@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Andrew Dickinson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: repository, https://github.com/Andrew-Dickinson/bird-ospf-link-db-parser
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE.txt
@@ -101,14 +102,18 @@
         ...
       }
     }
   }
 }
 ```
 
+## Output Format
+
+The output format is detailed using [JSON Schema](https://json-schema.org/) in `src/bird_parser/output_schema.json`
+
 
 ## Usage
 
 Pre-requisites: `python3` available via the shell
 
 Setup by cloning, creating a virtual env, and installing the application
 ```sh
```

### Comparing `bird-ospf-link-db-parser-1.1.0/README.md` & `bird-ospf-link-db-parser-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -95,126 +95,135 @@
 000005e0: 2020 226d 6574 7269 6322 3a20 300d 0a20    "metric": 0.. 
 000005f0: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
 00000600: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
 00000610: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
 00000620: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
 00000630: 2e2e 2e0d 0a20 2020 2020 207d 0d0a 2020  .....      }..  
 00000640: 2020 7d0d 0a20 207d 0d0a 7d0d 0a60 6060    }..  }..}..```
-00000650: 0d0a 0d0a 0d0a 2323 2055 7361 6765 0d0a  ......## Usage..
-00000660: 0d0a 5072 652d 7265 7175 6973 6974 6573  ..Pre-requisites
-00000670: 3a20 6070 7974 686f 6e33 6020 6176 6169  : `python3` avai
-00000680: 6c61 626c 6520 7669 6120 7468 6520 7368  lable via the sh
-00000690: 656c 6c0d 0a0d 0a53 6574 7570 2062 7920  ell....Setup by 
-000006a0: 636c 6f6e 696e 672c 2063 7265 6174 696e  cloning, creatin
-000006b0: 6720 6120 7669 7274 7561 6c20 656e 762c  g a virtual env,
-000006c0: 2061 6e64 2069 6e73 7461 6c6c 696e 6720   and installing 
-000006d0: 7468 6520 6170 706c 6963 6174 696f 6e0d  the application.
-000006e0: 0a60 6060 7368 0d0a 6769 7420 636c 6f6e  .```sh..git clon
-000006f0: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
-00000700: 2e63 6f6d 2f41 6e64 7265 772d 4469 636b  .com/Andrew-Dick
-00000710: 696e 736f 6e2f 6269 7264 2d6f 7370 662d  inson/bird-ospf-
-00000720: 6c69 6e6b 2d64 622d 7061 7273 6572 0d0a  link-db-parser..
-00000730: 6364 2062 6972 642d 6f73 7066 2d6c 696e  cd bird-ospf-lin
-00000740: 6b2d 6462 2d70 6172 7365 720d 0a70 7974  k-db-parser..pyt
-00000750: 686f 6e33 202d 6d20 7665 6e76 202e 7665  hon3 -m venv .ve
-00000760: 6e76 0d0a 736f 7572 6365 202e 7665 6e76  nv..source .venv
-00000770: 2f62 696e 2f61 6374 6976 6174 650d 0a70  /bin/activate..p
-00000780: 6970 2069 6e73 7461 6c6c 202d 6520 2e0d  ip install -e ..
-00000790: 0a60 6060 0d0a 0d0a 7468 656e 2069 6e76  .```....then inv
-000007a0: 6f6b 6520 7468 6520 746f 6f6c 2077 6974  oke the tool wit
-000007b0: 6820 7468 6520 434c 4920 636f 6d6d 616e  h the CLI comman
-000007c0: 643a 0d0a 6060 6073 680d 0a62 6972 6463  d:..```sh..birdc
-000007d0: 2073 686f 7720 6f73 7066 206c 696e 6b20   show ospf link 
-000007e0: 7374 6174 6520 616c 6c20 3e20 7061 7273  state all > pars
-000007f0: 652d 6269 7264 2d6c 696e 6b2d 6462 7061  e-bird-link-dbpa
-00000800: 7273 652d 6269 7264 2d6c 696e 6b2d 6462  rse-bird-link-db
-00000810: 202d 0d0a 6060 600d 0a0d 0a23 2320 5275   -..```....## Ru
-00000820: 6e6e 696e 6720 7468 6520 756e 6974 2074  nning the unit t
-00000830: 6573 7473 0d0a 0d0a 466f 6c6c 6f77 2074  ests....Follow t
-00000840: 6865 2069 6e73 7472 7563 7469 6f6e 7320  he instructions 
-00000850: 756e 6465 7220 2255 7361 6765 2220 6162  under "Usage" ab
-00000860: 6f76 652c 2074 6f20 636c 6f6e 6520 6120  ove, to clone a 
-00000870: 6c6f 6361 6c20 636f 7079 206f 6620 7468  local copy of th
-00000880: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
-00000890: 6e64 2061 6374 6976 6174 650d 0a74 6865  nd activate..the
-000008a0: 2076 6972 7475 616c 2065 6e76 6972 6f6e   virtual environ
-000008b0: 6d65 6e74 2e20 5468 656e 2069 6e73 7461  ment. Then insta
-000008c0: 6c6c 696e 6720 7468 6520 7465 7374 2064  lling the test d
-000008d0: 6570 656e 6465 6e63 6965 7320 7769 7468  ependencies with
-000008e0: 3a0d 0a60 6060 7368 0d0a 7069 7020 696e  :..```sh..pip in
-000008f0: 7374 616c 6c20 2d65 2022 2e5b 7465 7374  stall -e ".[test
-00000900: 2c64 6576 5d22 0d0a 6060 600d 0a0d 0a46  ,dev]"..```....F
-00000910: 696e 616c 6c79 2c20 696e 766f 6b65 2074  inally, invoke t
-00000920: 6865 2074 6573 7420 7375 6974 6520 7573  he test suite us
-00000930: 696e 6720 7079 7465 7374 3a0d 0a60 6060  ing pytest:..```
-00000940: 0d0a 7079 7465 7374 2074 6573 742f 0d0a  ..pytest test/..
-00000950: 6060 600d 0a0d 0a23 2320 4275 696c 6469  ```....## Buildi
-00000960: 6e67 2074 6f20 5079 5069 0d0a 0d0a 466f  ng to PyPi....Fo
-00000970: 6c6c 6f77 2074 6865 2069 6e73 7472 7563  llow the instruc
-00000980: 7469 6f6e 7320 6162 6f76 6520 746f 2063  tions above to c
-00000990: 6c6f 6e65 2061 206c 6f63 616c 2063 6f70  lone a local cop
-000009a0: 7920 6f66 2074 6869 7320 6170 706c 6963  y of this applic
-000009b0: 6174 696f 6e2c 2061 6374 6976 6174 650d  ation, activate.
-000009c0: 0a74 6865 2076 6972 7475 616c 2065 6e76  .the virtual env
-000009d0: 6972 6f6e 6d65 6e74 2c20 616e 6420 7275  ironment, and ru
-000009e0: 6e20 7468 6520 7465 7374 732e 0d0a 0d0a  n the tests.....
-000009f0: 5468 656e 2c20 6275 696c 6420 2620 7570  Then, build & up
-00000a00: 6c6f 6164 2074 6865 2061 7070 6c69 6361  load the applica
-00000a10: 7469 6f6e 2077 6974 680d 0a60 6060 0d0a  tion with..```..
-00000a20: 726d 202d 7266 2064 6973 742f 2a0d 0a70  rm -rf dist/*..p
-00000a30: 7974 686f 6e20 2d6d 2062 7569 6c64 202e  ython -m build .
-00000a40: 0d0a 7477 696e 6520 7570 6c6f 6164 2064  ..twine upload d
-00000a50: 6973 742f 2a0d 0a60 6060 0d0a 0d0a 2323  ist/*..```....##
-00000a60: 204c 6963 656e 7365 0d0a 0d0a 4469 7374   License....Dist
-00000a70: 7269 6275 7465 6420 756e 6465 7220 7468  ributed under th
-00000a80: 6520 4d49 5420 4c69 6365 6e73 652e 2053  e MIT License. S
-00000a90: 6565 2060 4c49 4345 4e53 452e 7478 7460  ee `LICENSE.txt`
-00000aa0: 2066 6f72 206d 6f72 6520 696e 666f 726d   for more inform
-00000ab0: 6174 696f 6e2e 0d0a 0d0a 2323 2043 6f6e  ation.....## Con
-00000ac0: 7472 6962 7574 696e 670d 0a0d 0a43 6f6e  tributing....Con
-00000ad0: 7472 6962 7574 696f 6e73 2061 7265 2077  tributions are w
-00000ae0: 6861 7420 6d61 6b65 2074 6865 206f 7065  hat make the ope
-00000af0: 6e20 736f 7572 6365 2063 6f6d 6d75 6e69  n source communi
-00000b00: 7479 2073 7563 6820 616e 2061 6d61 7a69  ty such an amazi
-00000b10: 6e67 2070 6c61 6365 2074 6f20 6c65 6172  ng place to lear
-00000b20: 6e2c 2069 6e73 7069 7265 2c20 616e 6420  n, inspire, and 
-00000b30: 6372 6561 7465 2e20 416e 7920 636f 6e74  create. Any cont
-00000b40: 7269 6275 7469 6f6e 7320 796f 7520 6d61  ributions you ma
-00000b50: 6b65 2061 7265 202a 2a67 7265 6174 6c79  ke are **greatly
-00000b60: 2061 7070 7265 6369 6174 6564 2a2a 2e0d   appreciated**..
-00000b70: 0a0d 0a49 6620 796f 7520 6861 7665 2061  ...If you have a
-00000b80: 2073 7567 6765 7374 696f 6e20 7468 6174   suggestion that
-00000b90: 2077 6f75 6c64 206d 616b 6520 7468 6973   would make this
-00000ba0: 2062 6574 7465 722c 2070 6c65 6173 6520   better, please 
-00000bb0: 666f 726b 2074 6865 2072 6570 6f20 616e  fork the repo an
-00000bc0: 6420 6372 6561 7465 2061 2070 756c 6c20  d create a pull 
-00000bd0: 7265 7175 6573 742e 2059 6f75 2063 616e  request. You can
-00000be0: 2061 6c73 6f20 7369 6d70 6c79 206f 7065   also simply ope
-00000bf0: 6e20 616e 2069 7373 7565 2077 6974 6820  n an issue with 
-00000c00: 7468 6520 7461 6720 2265 6e68 616e 6365  the tag "enhance
-00000c10: 6d65 6e74 222e 0d0a 446f 6e27 7420 666f  ment"...Don't fo
-00000c20: 7267 6574 2074 6f20 6769 7665 2074 6865  rget to give the
-00000c30: 2070 726f 6a65 6374 2061 2073 7461 7221   project a star!
-00000c40: 2054 6861 6e6b 7320 6167 6169 6e21 0d0a   Thanks again!..
-00000c50: 0d0a 312e 2046 6f72 6b20 7468 6520 5072  ..1. Fork the Pr
-00000c60: 6f6a 6563 740d 0a32 2e20 4372 6561 7465  oject..2. Create
-00000c70: 2079 6f75 7220 4665 6174 7572 6520 4272   your Feature Br
-00000c80: 616e 6368 2028 6067 6974 2063 6865 636b  anch (`git check
-00000c90: 6f75 7420 2d62 2066 6561 7475 7265 2f41  out -b feature/A
-00000ca0: 6d61 7a69 6e67 4665 6174 7572 6560 290d  mazingFeature`).
-00000cb0: 0a33 2e20 436f 6d6d 6974 2079 6f75 7220  .3. Commit your 
-00000cc0: 4368 616e 6765 7320 2860 6769 7420 636f  Changes (`git co
-00000cd0: 6d6d 6974 202d 6d20 2741 6464 2073 6f6d  mmit -m 'Add som
-00000ce0: 6520 416d 617a 696e 6746 6561 7475 7265  e AmazingFeature
-00000cf0: 2760 290d 0a34 2e20 5075 7368 2074 6f20  '`)..4. Push to 
-00000d00: 7468 6520 4272 616e 6368 2028 6067 6974  the Branch (`git
-00000d10: 2070 7573 6820 6f72 6967 696e 2066 6561   push origin fea
-00000d20: 7475 7265 2f41 6d61 7a69 6e67 4665 6174  ture/AmazingFeat
-00000d30: 7572 6560 290d 0a35 2e20 4f70 656e 2061  ure`)..5. Open a
-00000d40: 2050 756c 6c20 5265 7175 6573 740d 0a0d   Pull Request...
-00000d50: 0a0d 0a23 2320 4163 6b6e 6f77 6c65 6467  ...## Acknowledg
-00000d60: 6d65 6e74 730d 0a20 2a20 5b42 6573 742d  ments.. * [Best-
-00000d70: 5245 4144 4d45 2d54 656d 706c 6174 655d  README-Template]
-00000d80: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000d90: 636f 6d2f 6f74 686e 6569 6c64 7265 772f  com/othneildrew/
-00000da0: 4265 7374 2d52 4541 444d 452d 5465 6d70  Best-README-Temp
-00000db0: 6c61 7465 2f29 0d0a                      late/)..
+00000650: 0d0a 0d0a 2323 204f 7574 7075 7420 466f  ....## Output Fo
+00000660: 726d 6174 0d0a 0d0a 5468 6520 6f75 7470  rmat....The outp
+00000670: 7574 2066 6f72 6d61 7420 6973 2064 6574  ut format is det
+00000680: 6169 6c65 6420 7573 696e 6720 5b4a 534f  ailed using [JSO
+00000690: 4e20 5363 6865 6d61 5d28 6874 7470 733a  N Schema](https:
+000006a0: 2f2f 6a73 6f6e 2d73 6368 656d 612e 6f72  //json-schema.or
+000006b0: 672f 2920 696e 2060 7372 632f 6269 7264  g/) in `src/bird
+000006c0: 5f70 6172 7365 722f 6f75 7470 7574 5f73  _parser/output_s
+000006d0: 6368 656d 612e 6a73 6f6e 600d 0a0d 0a0d  chema.json`.....
+000006e0: 0a23 2320 5573 6167 650d 0a0d 0a50 7265  .## Usage....Pre
+000006f0: 2d72 6571 7569 7369 7465 733a 2060 7079  -requisites: `py
+00000700: 7468 6f6e 3360 2061 7661 696c 6162 6c65  thon3` available
+00000710: 2076 6961 2074 6865 2073 6865 6c6c 0d0a   via the shell..
+00000720: 0d0a 5365 7475 7020 6279 2063 6c6f 6e69  ..Setup by cloni
+00000730: 6e67 2c20 6372 6561 7469 6e67 2061 2076  ng, creating a v
+00000740: 6972 7475 616c 2065 6e76 2c20 616e 6420  irtual env, and 
+00000750: 696e 7374 616c 6c69 6e67 2074 6865 2061  installing the a
+00000760: 7070 6c69 6361 7469 6f6e 0d0a 6060 6073  pplication..```s
+00000770: 680d 0a67 6974 2063 6c6f 6e65 2068 7474  h..git clone htt
+00000780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000790: 416e 6472 6577 2d44 6963 6b69 6e73 6f6e  Andrew-Dickinson
+000007a0: 2f62 6972 642d 6f73 7066 2d6c 696e 6b2d  /bird-ospf-link-
+000007b0: 6462 2d70 6172 7365 720d 0a63 6420 6269  db-parser..cd bi
+000007c0: 7264 2d6f 7370 662d 6c69 6e6b 2d64 622d  rd-ospf-link-db-
+000007d0: 7061 7273 6572 0d0a 7079 7468 6f6e 3320  parser..python3 
+000007e0: 2d6d 2076 656e 7620 2e76 656e 760d 0a73  -m venv .venv..s
+000007f0: 6f75 7263 6520 2e76 656e 762f 6269 6e2f  ource .venv/bin/
+00000800: 6163 7469 7661 7465 0d0a 7069 7020 696e  activate..pip in
+00000810: 7374 616c 6c20 2d65 202e 0d0a 6060 600d  stall -e ...```.
+00000820: 0a0d 0a74 6865 6e20 696e 766f 6b65 2074  ...then invoke t
+00000830: 6865 2074 6f6f 6c20 7769 7468 2074 6865  he tool with the
+00000840: 2043 4c49 2063 6f6d 6d61 6e64 3a0d 0a60   CLI command:..`
+00000850: 6060 7368 0d0a 6269 7264 6320 7368 6f77  ``sh..birdc show
+00000860: 206f 7370 6620 6c69 6e6b 2073 7461 7465   ospf link state
+00000870: 2061 6c6c 203e 2070 6172 7365 2d62 6972   all > parse-bir
+00000880: 642d 6c69 6e6b 2d64 6270 6172 7365 2d62  d-link-dbparse-b
+00000890: 6972 642d 6c69 6e6b 2d64 6220 2d0d 0a60  ird-link-db -..`
+000008a0: 6060 0d0a 0d0a 2323 2052 756e 6e69 6e67  ``....## Running
+000008b0: 2074 6865 2075 6e69 7420 7465 7374 730d   the unit tests.
+000008c0: 0a0d 0a46 6f6c 6c6f 7720 7468 6520 696e  ...Follow the in
+000008d0: 7374 7275 6374 696f 6e73 2075 6e64 6572  structions under
+000008e0: 2022 5573 6167 6522 2061 626f 7665 2c20   "Usage" above, 
+000008f0: 746f 2063 6c6f 6e65 2061 206c 6f63 616c  to clone a local
+00000900: 2063 6f70 7920 6f66 2074 6869 7320 6170   copy of this ap
+00000910: 706c 6963 6174 696f 6e20 616e 6420 6163  plication and ac
+00000920: 7469 7661 7465 0d0a 7468 6520 7669 7274  tivate..the virt
+00000930: 7561 6c20 656e 7669 726f 6e6d 656e 742e  ual environment.
+00000940: 2054 6865 6e20 696e 7374 616c 6c69 6e67   Then installing
+00000950: 2074 6865 2074 6573 7420 6465 7065 6e64   the test depend
+00000960: 656e 6369 6573 2077 6974 683a 0d0a 6060  encies with:..``
+00000970: 6073 680d 0a70 6970 2069 6e73 7461 6c6c  `sh..pip install
+00000980: 202d 6520 222e 5b74 6573 742c 6465 765d   -e ".[test,dev]
+00000990: 220d 0a60 6060 0d0a 0d0a 4669 6e61 6c6c  "..```....Finall
+000009a0: 792c 2069 6e76 6f6b 6520 7468 6520 7465  y, invoke the te
+000009b0: 7374 2073 7569 7465 2075 7369 6e67 2070  st suite using p
+000009c0: 7974 6573 743a 0d0a 6060 600d 0a70 7974  ytest:..```..pyt
+000009d0: 6573 7420 7465 7374 2f0d 0a60 6060 0d0a  est test/..```..
+000009e0: 0d0a 2323 2042 7569 6c64 696e 6720 746f  ..## Building to
+000009f0: 2050 7950 690d 0a0d 0a46 6f6c 6c6f 7720   PyPi....Follow 
+00000a00: 7468 6520 696e 7374 7275 6374 696f 6e73  the instructions
+00000a10: 2061 626f 7665 2074 6f20 636c 6f6e 6520   above to clone 
+00000a20: 6120 6c6f 6361 6c20 636f 7079 206f 6620  a local copy of 
+00000a30: 7468 6973 2061 7070 6c69 6361 7469 6f6e  this application
+00000a40: 2c20 6163 7469 7661 7465 0d0a 7468 6520  , activate..the 
+00000a50: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00000a60: 656e 742c 2061 6e64 2072 756e 2074 6865  ent, and run the
+00000a70: 2074 6573 7473 2e0d 0a0d 0a54 6865 6e2c   tests.....Then,
+00000a80: 2062 7569 6c64 2026 2075 706c 6f61 6420   build & upload 
+00000a90: 7468 6520 6170 706c 6963 6174 696f 6e20  the application 
+00000aa0: 7769 7468 0d0a 6060 600d 0a72 6d20 2d72  with..```..rm -r
+00000ab0: 6620 6469 7374 2f2a 0d0a 7079 7468 6f6e  f dist/*..python
+00000ac0: 202d 6d20 6275 696c 6420 2e0d 0a74 7769   -m build ...twi
+00000ad0: 6e65 2075 706c 6f61 6420 6469 7374 2f2a  ne upload dist/*
+00000ae0: 0d0a 6060 600d 0a0d 0a23 2320 4c69 6365  ..```....## Lice
+00000af0: 6e73 650d 0a0d 0a44 6973 7472 6962 7574  nse....Distribut
+00000b00: 6564 2075 6e64 6572 2074 6865 204d 4954  ed under the MIT
+00000b10: 204c 6963 656e 7365 2e20 5365 6520 604c   License. See `L
+00000b20: 4943 454e 5345 2e74 7874 6020 666f 7220  ICENSE.txt` for 
+00000b30: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00000b40: 2e0d 0a0d 0a23 2320 436f 6e74 7269 6275  .....## Contribu
+00000b50: 7469 6e67 0d0a 0d0a 436f 6e74 7269 6275  ting....Contribu
+00000b60: 7469 6f6e 7320 6172 6520 7768 6174 206d  tions are what m
+00000b70: 616b 6520 7468 6520 6f70 656e 2073 6f75  ake the open sou
+00000b80: 7263 6520 636f 6d6d 756e 6974 7920 7375  rce community su
+00000b90: 6368 2061 6e20 616d 617a 696e 6720 706c  ch an amazing pl
+00000ba0: 6163 6520 746f 206c 6561 726e 2c20 696e  ace to learn, in
+00000bb0: 7370 6972 652c 2061 6e64 2063 7265 6174  spire, and creat
+00000bc0: 652e 2041 6e79 2063 6f6e 7472 6962 7574  e. Any contribut
+00000bd0: 696f 6e73 2079 6f75 206d 616b 6520 6172  ions you make ar
+00000be0: 6520 2a2a 6772 6561 746c 7920 6170 7072  e **greatly appr
+00000bf0: 6563 6961 7465 642a 2a2e 0d0a 0d0a 4966  eciated**.....If
+00000c00: 2079 6f75 2068 6176 6520 6120 7375 6767   you have a sugg
+00000c10: 6573 7469 6f6e 2074 6861 7420 776f 756c  estion that woul
+00000c20: 6420 6d61 6b65 2074 6869 7320 6265 7474  d make this bett
+00000c30: 6572 2c20 706c 6561 7365 2066 6f72 6b20  er, please fork 
+00000c40: 7468 6520 7265 706f 2061 6e64 2063 7265  the repo and cre
+00000c50: 6174 6520 6120 7075 6c6c 2072 6571 7565  ate a pull reque
+00000c60: 7374 2e20 596f 7520 6361 6e20 616c 736f  st. You can also
+00000c70: 2073 696d 706c 7920 6f70 656e 2061 6e20   simply open an 
+00000c80: 6973 7375 6520 7769 7468 2074 6865 2074  issue with the t
+00000c90: 6167 2022 656e 6861 6e63 656d 656e 7422  ag "enhancement"
+00000ca0: 2e0d 0a44 6f6e 2774 2066 6f72 6765 7420  ...Don't forget 
+00000cb0: 746f 2067 6976 6520 7468 6520 7072 6f6a  to give the proj
+00000cc0: 6563 7420 6120 7374 6172 2120 5468 616e  ect a star! Than
+00000cd0: 6b73 2061 6761 696e 210d 0a0d 0a31 2e20  ks again!....1. 
+00000ce0: 466f 726b 2074 6865 2050 726f 6a65 6374  Fork the Project
+00000cf0: 0d0a 322e 2043 7265 6174 6520 796f 7572  ..2. Create your
+00000d00: 2046 6561 7475 7265 2042 7261 6e63 6820   Feature Branch 
+00000d10: 2860 6769 7420 6368 6563 6b6f 7574 202d  (`git checkout -
+00000d20: 6220 6665 6174 7572 652f 416d 617a 696e  b feature/Amazin
+00000d30: 6746 6561 7475 7265 6029 0d0a 332e 2043  gFeature`)..3. C
+00000d40: 6f6d 6d69 7420 796f 7572 2043 6861 6e67  ommit your Chang
+00000d50: 6573 2028 6067 6974 2063 6f6d 6d69 7420  es (`git commit 
+00000d60: 2d6d 2027 4164 6420 736f 6d65 2041 6d61  -m 'Add some Ama
+00000d70: 7a69 6e67 4665 6174 7572 6527 6029 0d0a  zingFeature'`)..
+00000d80: 342e 2050 7573 6820 746f 2074 6865 2042  4. Push to the B
+00000d90: 7261 6e63 6820 2860 6769 7420 7075 7368  ranch (`git push
+00000da0: 206f 7269 6769 6e20 6665 6174 7572 652f   origin feature/
+00000db0: 416d 617a 696e 6746 6561 7475 7265 6029  AmazingFeature`)
+00000dc0: 0d0a 352e 204f 7065 6e20 6120 5075 6c6c  ..5. Open a Pull
+00000dd0: 2052 6571 7565 7374 0d0a 0d0a 0d0a 2323   Request......##
+00000de0: 2041 636b 6e6f 776c 6564 676d 656e 7473   Acknowledgments
+00000df0: 0d0a 202a 205b 4265 7374 2d52 4541 444d  .. * [Best-READM
+00000e00: 452d 5465 6d70 6c61 7465 5d28 6874 7470  E-Template](http
+00000e10: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
+00000e20: 7468 6e65 696c 6472 6577 2f42 6573 742d  thneildrew/Best-
+00000e30: 5245 4144 4d45 2d54 656d 706c 6174 652f  README-Template/
+00000e40: 290d 0a                                  )..
```

### Comparing `bird-ospf-link-db-parser-1.1.0/pyproject.toml` & `bird-ospf-link-db-parser-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 [project]
 name = "bird-ospf-link-db-parser"
-version = "1.1.0"
+version = "1.1.1"
 authors = [{ name = "Andrew Dickinson", email = "andrew.dickinson.0216@gmail.com" }]
-description = "A simple Python package"
+description = "Parse the text output from the BIRD Routing Daemon's OSPF link database into machine readable JSON"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent"
 ]
-
-[options.packages.find]
-where = "src"
-
 dependencies = [
     "python-dotenv",
     "pytz",
     "python-dateutil",
     "jsonschema",
 ]
 
+[project.urls]
+repository = "https://github.com/Andrew-Dickinson/bird-ospf-link-db-parser"
+
 [project.optional-dependencies]
 test = [
     "pytest >= 6",
     "coverage",
     "freezegun",
 ]
 dev = [
     "build",
+    "twine"
 ]
 
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project.scripts]
-parse-bird-link-db = "bird_parser:main.main"
+parse-bird-link-db = "bird_parser:main.main"
+
+[options.packages.find]
+where = "src"
```

### Comparing `bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/PKG-INFO` & `bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: bird-ospf-link-db-parser
-Version: 1.1.0
-Summary: A simple Python package
+Version: 1.1.1
+Summary: Parse the text output from the BIRD Routing Daemon's OSPF link database into machine readable JSON
 Author-email: Andrew Dickinson <andrew.dickinson.0216@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Andrew Dickinson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -21,14 +21,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Project-URL: repository, https://github.com/Andrew-Dickinson/bird-ospf-link-db-parser
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE.txt
@@ -101,14 +102,18 @@
         ...
       }
     }
   }
 }
 ```
 
+## Output Format
+
+The output format is detailed using [JSON Schema](https://json-schema.org/) in `src/bird_parser/output_schema.json`
+
 
 ## Usage
 
 Pre-requisites: `python3` available via the shell
 
 Setup by cloning, creating a virtual env, and installing the application
 ```sh
```

### Comparing `bird-ospf-link-db-parser-1.1.0/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt` & `bird-ospf-link-db-parser-1.1.1/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/src/bird_parser/main.py` & `bird-ospf-link-db-parser-1.1.1/src/bird_parser/main.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/src/bird_parser/output_schema.json` & `bird-ospf-link-db-parser-1.1.1/src/bird_parser/output_schema.json`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/src/bird_parser/parse_bird_output.py` & `bird-ospf-link-db-parser-1.1.1/src/bird_parser/parse_bird_output.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/src/bird_parser/utils.py` & `bird-ospf-link-db-parser-1.1.1/src/bird_parser/utils.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/test/test_comprehensive.py` & `bird-ospf-link-db-parser-1.1.1/test/test_comprehensive.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/test/test_live_data.py` & `bird-ospf-link-db-parser-1.1.1/test/test_live_data.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.0/test/test_simple.py` & `bird-ospf-link-db-parser-1.1.1/test/test_simple.py`

 * *Files identical despite different names*

