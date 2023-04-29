# Comparing `tmp/bird-ospf-link-db-parser-1.1.2.tar.gz` & `tmp/bird-ospf-link-db-parser-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bird-ospf-link-db-parser-1.1.2.tar", last modified: Sat Apr 29 07:43:42 2023, max compression
+gzip compressed data, was "bird-ospf-link-db-parser-1.1.3.tar", last modified: Sat Apr 29 18:54:51 2023, max compression
```

## Comparing `bird-ospf-link-db-parser-1.1.2.tar` & `bird-ospf-link-db-parser-1.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 07:43:42.661471 bird-ospf-link-db-parser-1.1.2/
--rw-rw-rw-   0        0        0     1094 2023-04-16 04:36:39.000000 bird-ospf-link-db-parser-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 07:07:22.000000 bird-ospf-link-db-parser-1.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5979 2023-04-29 07:43:42.660467 bird-ospf-link-db-parser-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     4111 2023-04-29 07:43:11.000000 bird-ospf-link-db-parser-1.1.2/README.md
--rw-rw-rw-   0        0        0     1011 2023-04-29 07:38:03.000000 bird-ospf-link-db-parser-1.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 07:43:42.661471 bird-ospf-link-db-parser-1.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-29 07:43:42.632782 bird-ospf-link-db-parser-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-29 07:43:42.651470 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/
--rw-rw-rw-   0        0        0     5979 2023-04-29 07:43:42.000000 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-29 07:43:42.000000 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 07:43:42.000000 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-29 07:43:42.000000 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      102 2023-04-29 07:43:42.000000 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-29 07:43:42.000000 bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 07:43:42.656468 bird-ospf-link-db-parser-1.1.2/src/bird_parser/
--rw-rw-rw-   0        0        0        0 2023-04-16 04:38:40.000000 bird-ospf-link-db-parser-1.1.2/src/bird_parser/__init__.py
--rw-rw-rw-   0        0        0      868 2023-04-29 07:01:45.000000 bird-ospf-link-db-parser-1.1.2/src/bird_parser/main.py
--rw-rw-rw-   0        0        0     6161 2023-04-29 06:58:21.000000 bird-ospf-link-db-parser-1.1.2/src/bird_parser/output_schema.json
--rw-rw-rw-   0        0        0     4159 2023-04-29 05:06:33.000000 bird-ospf-link-db-parser-1.1.2/src/bird_parser/parse_bird_output.py
--rw-rw-rw-   0        0        0     1644 2023-04-29 05:07:09.000000 bird-ospf-link-db-parser-1.1.2/src/bird_parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-29 07:43:42.659467 bird-ospf-link-db-parser-1.1.2/test/
--rw-rw-rw-   0        0        0     3290 2023-04-29 04:12:24.000000 bird-ospf-link-db-parser-1.1.2/test/test_comprehensive.py
--rw-rw-rw-   0        0        0     1100 2023-04-29 05:20:14.000000 bird-ospf-link-db-parser-1.1.2/test/test_live_data.py
--rw-rw-rw-   0        0        0     1736 2023-04-29 03:04:39.000000 bird-ospf-link-db-parser-1.1.2/test/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:54:51.201438 bird-ospf-link-db-parser-1.1.3/
+-rw-rw-rw-   0        0        0     1094 2023-04-16 04:36:39.000000 bird-ospf-link-db-parser-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 07:07:22.000000 bird-ospf-link-db-parser-1.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5963 2023-04-29 18:54:51.200438 bird-ospf-link-db-parser-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4095 2023-04-29 18:54:02.000000 bird-ospf-link-db-parser-1.1.3/README.md
+-rw-rw-rw-   0        0        0     1011 2023-04-29 18:54:22.000000 bird-ospf-link-db-parser-1.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 18:54:51.201438 bird-ospf-link-db-parser-1.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 18:54:51.161053 bird-ospf-link-db-parser-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 18:54:51.190439 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/
+-rw-rw-rw-   0        0        0     5963 2023-04-29 18:54:51.000000 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-29 18:54:51.000000 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 18:54:51.000000 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-29 18:54:51.000000 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      102 2023-04-29 18:54:51.000000 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-04-29 18:54:51.000000 bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 18:54:51.196437 bird-ospf-link-db-parser-1.1.3/src/bird_parser/
+-rw-rw-rw-   0        0        0        0 2023-04-16 04:38:40.000000 bird-ospf-link-db-parser-1.1.3/src/bird_parser/__init__.py
+-rw-rw-rw-   0        0        0      868 2023-04-29 07:01:45.000000 bird-ospf-link-db-parser-1.1.3/src/bird_parser/main.py
+-rw-rw-rw-   0        0        0     6161 2023-04-29 06:58:21.000000 bird-ospf-link-db-parser-1.1.3/src/bird_parser/output_schema.json
+-rw-rw-rw-   0        0        0     4159 2023-04-29 05:06:33.000000 bird-ospf-link-db-parser-1.1.3/src/bird_parser/parse_bird_output.py
+-rw-rw-rw-   0        0        0     1644 2023-04-29 05:07:09.000000 bird-ospf-link-db-parser-1.1.3/src/bird_parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-29 18:54:51.199438 bird-ospf-link-db-parser-1.1.3/test/
+-rw-rw-rw-   0        0        0     3290 2023-04-29 04:12:24.000000 bird-ospf-link-db-parser-1.1.3/test/test_comprehensive.py
+-rw-rw-rw-   0        0        0     1100 2023-04-29 05:20:14.000000 bird-ospf-link-db-parser-1.1.3/test/test_live_data.py
+-rw-rw-rw-   0        0        0     1736 2023-04-29 03:04:39.000000 bird-ospf-link-db-parser-1.1.3/test/test_simple.py
```

### Comparing `bird-ospf-link-db-parser-1.1.2/LICENSE.txt` & `bird-ospf-link-db-parser-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/PKG-INFO` & `bird-ospf-link-db-parser-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bird-ospf-link-db-parser
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parse the text output from the BIRD Routing Daemon's OSPF link database into machine readable JSON
 Author-email: Andrew Dickinson <andrew.dickinson.0216@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Andrew Dickinson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 
 
 # Bird OSFP Link Database Parser
 
 Parses the output of the BIRD Routing Daemon's `birdc show ospf state` command into a machine-readable JSON string.
 
 ```sh
-> birdc show ospf state all | parse-bird-link-db - | jq | less
+> birdc show ospf state | parse-bird-link-db - | jq | less
 {
   "areas": {
     "0.0.0.0": {
       "routers": {
         "10.68.29.50": {
           "links": {
             "router": [
@@ -117,21 +117,21 @@
 First, install the CLI via pip:
 ```shell
 pip install bird-ospf-link-db-parser
 ```
 
 then invoke the tool with the CLI command:
 ```shell
-birdc show ospf state all | parse-bird-link-db -
+birdc show ospf state | parse-bird-link-db -
 ```
 
 But you probably want to use `jq` and `less` to make this output a bit more manageable:
 ```shell
 sudo apt update && sudo apt install jq less
-birdc show ospf state all | parse-bird-link-db - | jq | less
+birdc show ospf state | parse-bird-link-db - | jq | less
 ```
 
 ## Dev Setup
 
 Pre-requisites: `python3` available via the shell
 
 Setup by cloning, creating a virtual env, and installing the application
@@ -141,15 +141,15 @@
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -e .
 ```
 
 then invoke the tool with the CLI command:
 ```sh
-birdc show ospf link state all > parse-bird-link-db -
+birdc show ospf link state > parse-bird-link-db -
 ```
 
 ## Running the unit tests
 
 Follow the instructions under "Dev Setup" above, to clone a local copy of this application and activate
 the virtual environment. Then installing the test dependencies with:
 ```sh
```

### Comparing `bird-ospf-link-db-parser-1.1.2/README.md` & `bird-ospf-link-db-parser-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,253 +5,252 @@
 00000040: 4952 4420 526f 7574 696e 6720 4461 656d  IRD Routing Daem
 00000050: 6f6e 2773 2060 6269 7264 6320 7368 6f77  on's `birdc show
 00000060: 206f 7370 6620 7374 6174 6560 2063 6f6d   ospf state` com
 00000070: 6d61 6e64 2069 6e74 6f20 6120 6d61 6368  mand into a mach
 00000080: 696e 652d 7265 6164 6162 6c65 204a 534f  ine-readable JSO
 00000090: 4e20 7374 7269 6e67 2e0d 0a0d 0a60 6060  N string.....```
 000000a0: 7368 0d0a 3e20 6269 7264 6320 7368 6f77  sh..> birdc show
-000000b0: 206f 7370 6620 7374 6174 6520 616c 6c20   ospf state all 
-000000c0: 7c20 7061 7273 652d 6269 7264 2d6c 696e  | parse-bird-lin
-000000d0: 6b2d 6462 202d 207c 206a 7120 7c20 6c65  k-db - | jq | le
-000000e0: 7373 0d0a 7b0d 0a20 2022 6172 6561 7322  ss..{..  "areas"
-000000f0: 3a20 7b0d 0a20 2020 2022 302e 302e 302e  : {..    "0.0.0.
-00000100: 3022 3a20 7b0d 0a20 2020 2020 2022 726f  0": {..      "ro
-00000110: 7574 6572 7322 3a20 7b0d 0a20 2020 2020  uters": {..     
-00000120: 2020 2022 3130 2e36 382e 3239 2e35 3022     "10.68.29.50"
-00000130: 3a20 7b0d 0a20 2020 2020 2020 2020 2022  : {..          "
-00000140: 6c69 6e6b 7322 3a20 7b0d 0a20 2020 2020  links": {..     
-00000150: 2020 2020 2020 2022 726f 7574 6572 223a         "router":
-00000160: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00000170: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00000180: 2020 2020 2022 6964 223a 2022 3130 2e36       "id": "10.6
-00000190: 392e 372e 3331 222c 0d0a 2020 2020 2020  9.7.31",..      
-000001a0: 2020 2020 2020 2020 2020 226d 6574 7269            "metri
-000001b0: 6322 3a20 3130 0d0a 2020 2020 2020 2020  c": 10..        
-000001c0: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
-000001d0: 2020 2020 205d 2c0d 0a20 2020 2020 2020       ],..       
-000001e0: 2020 2020 2022 7374 7562 6e65 7422 3a20       "stubnet": 
-000001f0: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
-00000200: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-00000210: 2020 2020 2269 6422 3a20 2231 302e 3639      "id": "10.69
-00000220: 2e32 392e 3530 2f33 3222 2c0d 0a20 2020  .29.50/32",..   
-00000230: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
-00000240: 7472 6963 223a 2030 0d0a 2020 2020 2020  tric": 0..      
-00000250: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
-00000260: 2020 2020 2020 2020 2020 7b0d 0a20 2020            {..   
-00000270: 2020 2020 2020 2020 2020 2020 2022 6964               "id
-00000280: 223a 2022 3130 2e36 382e 3239 2e35 302f  ": "10.68.29.50/
-00000290: 3332 222c 0d0a 2020 2020 2020 2020 2020  32",..          
-000002a0: 2020 2020 2020 226d 6574 7269 6322 3a20        "metric": 
-000002b0: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
-000002c0: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
-000002d0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-000002e0: 2265 7874 6572 6e61 6c22 3a20 5b0d 0a20  "external": [.. 
-000002f0: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
-00000300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000310: 2269 6422 3a20 2231 302e 3730 2e31 3734  "id": "10.70.174
-00000320: 2e30 2f32 3422 2c0d 0a20 2020 2020 2020  .0/24",..       
-00000330: 2020 2020 2020 2020 2022 6d65 7472 6963           "metric
-00000340: 223a 2032 300d 0a20 2020 2020 2020 2020  ": 20..         
-00000350: 2020 2020 207d 0d0a 2020 2020 2020 2020       }..        
-00000360: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-00000370: 207d 0d0a 2020 2020 2020 2020 7d2c 0d0a   }..        },..
-00000380: 2020 2020 2020 2020 2231 302e 3638 2e37          "10.68.7
-00000390: 332e 3132 3522 3a20 7b0d 0a20 2020 2020  3.125": {..     
-000003a0: 2020 2020 2022 6c69 6e6b 7322 3a20 7b0d       "links": {.
-000003b0: 0a20 2020 2020 2020 2020 2020 2022 726f  .            "ro
-000003c0: 7574 6572 223a 205b 0d0a 2020 2020 2020  uter": [..      
-000003d0: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
-000003e0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-000003f0: 2022 3130 2e36 392e 3733 2e32 3522 2c0d   "10.69.73.25",.
-00000400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000410: 2022 6d65 7472 6963 223a 2031 300d 0a20   "metric": 10.. 
-00000420: 2020 2020 2020 2020 2020 2020 207d 2c0d               },.
-00000430: 0a20 2020 2020 2020 2020 2020 2020 207b  .              {
-00000440: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000450: 2020 2269 6422 3a20 2231 302e 3639 2e35    "id": "10.69.5
-00000460: 322e 3833 222c 0d0a 2020 2020 2020 2020  2.83",..        
-00000470: 2020 2020 2020 2020 226d 6574 7269 6322          "metric"
-00000480: 3a20 3330 0d0a 2020 2020 2020 2020 2020  : 30..          
-00000490: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-000004a0: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-000004b0: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-000004c0: 3130 2e36 392e 3733 2e32 3522 2c0d 0a20  10.69.73.25",.. 
-000004d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000004e0: 6d65 7472 6963 223a 2033 300d 0a20 2020  metric": 30..   
-000004f0: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
-00000500: 2020 2020 2020 2020 2020 5d2c 0d0a 2020            ],..  
-00000510: 2020 2020 2020 2020 2020 2273 7475 626e            "stubn
-00000520: 6574 223a 205b 0d0a 2020 2020 2020 2020  et": [..        
-00000530: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
-00000540: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-00000550: 3130 2e36 392e 3733 2e31 3235 2f33 3222  10.69.73.125/32"
-00000560: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000570: 2020 2022 6d65 7472 6963 223a 2030 0d0a     "metric": 0..
-00000580: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-00000590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000005a0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-000005b0: 2020 2022 6964 223a 2022 3130 2e36 382e     "id": "10.68.
-000005c0: 3733 2e31 3235 2f33 3222 2c0d 0a20 2020  73.125/32",..   
-000005d0: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
-000005e0: 7472 6963 223a 2030 0d0a 2020 2020 2020  tric": 0..      
-000005f0: 2020 2020 2020 2020 7d0d 0a20 2020 2020          }..     
-00000600: 2020 2020 2020 205d 0d0a 2020 2020 2020         ]..      
-00000610: 2020 2020 7d0d 0a20 2020 2020 2020 207d      }..        }
-00000620: 2c0d 0a20 2020 2020 2020 202e 2e2e 0d0a  ,..        .....
-00000630: 2020 2020 2020 7d0d 0a20 2020 207d 0d0a        }..    }..
-00000640: 2020 7d0d 0a7d 0d0a 6060 600d 0a0d 0a23    }..}..```....#
-00000650: 2320 4f75 7470 7574 2046 6f72 6d61 740d  # Output Format.
-00000660: 0a0d 0a54 6865 206f 7574 7075 7420 666f  ...The output fo
-00000670: 726d 6174 2069 7320 6465 7461 696c 6564  rmat is detailed
-00000680: 2075 7369 6e67 205b 4a53 4f4e 2053 6368   using [JSON Sch
-00000690: 656d 615d 2868 7474 7073 3a2f 2f6a 736f  ema](https://jso
-000006a0: 6e2d 7363 6865 6d61 2e6f 7267 2f29 2069  n-schema.org/) i
-000006b0: 6e20 6073 7263 2f62 6972 645f 7061 7273  n `src/bird_pars
-000006c0: 6572 2f6f 7574 7075 745f 7363 6865 6d61  er/output_schema
-000006d0: 2e6a 736f 6e60 0d0a 0d0a 2323 2055 7361  .json`....## Usa
-000006e0: 6765 0d0a 0d0a 5072 652d 7265 7175 6973  ge....Pre-requis
-000006f0: 6974 6573 3a20 6070 7974 686f 6e33 6020  ites: `python3` 
-00000700: 6176 6169 6c61 626c 6520 7669 6120 7468  available via th
-00000710: 6520 7368 656c 6c0d 0a0d 0a46 6972 7374  e shell....First
-00000720: 2c20 696e 7374 616c 6c20 7468 6520 434c  , install the CL
-00000730: 4920 7669 6120 7069 703a 0d0a 6060 6073  I via pip:..```s
-00000740: 6865 6c6c 0d0a 7069 7020 696e 7374 616c  hell..pip instal
-00000750: 6c20 6269 7264 2d6f 7370 662d 6c69 6e6b  l bird-ospf-link
-00000760: 2d64 622d 7061 7273 6572 0d0a 6060 600d  -db-parser..```.
-00000770: 0a0d 0a74 6865 6e20 696e 766f 6b65 2074  ...then invoke t
-00000780: 6865 2074 6f6f 6c20 7769 7468 2074 6865  he tool with the
-00000790: 2043 4c49 2063 6f6d 6d61 6e64 3a0d 0a60   CLI command:..`
-000007a0: 6060 7368 656c 6c0d 0a62 6972 6463 2073  ``shell..birdc s
-000007b0: 686f 7720 6f73 7066 2073 7461 7465 2061  how ospf state a
-000007c0: 6c6c 207c 2070 6172 7365 2d62 6972 642d  ll | parse-bird-
-000007d0: 6c69 6e6b 2d64 6220 2d0d 0a60 6060 0d0a  link-db -..```..
-000007e0: 0d0a 4275 7420 796f 7520 7072 6f62 6162  ..But you probab
-000007f0: 6c79 2077 616e 7420 746f 2075 7365 2060  ly want to use `
-00000800: 6a71 6020 616e 6420 606c 6573 7360 2074  jq` and `less` t
-00000810: 6f20 6d61 6b65 2074 6869 7320 6f75 7470  o make this outp
-00000820: 7574 2061 2062 6974 206d 6f72 6520 6d61  ut a bit more ma
-00000830: 6e61 6765 6162 6c65 3a0d 0a60 6060 7368  nageable:..```sh
-00000840: 656c 6c0d 0a73 7564 6f20 6170 7420 7570  ell..sudo apt up
-00000850: 6461 7465 2026 2620 7375 646f 2061 7074  date && sudo apt
-00000860: 2069 6e73 7461 6c6c 206a 7120 6c65 7373   install jq less
-00000870: 0d0a 6269 7264 6320 7368 6f77 206f 7370  ..birdc show osp
-00000880: 6620 7374 6174 6520 616c 6c20 7c20 7061  f state all | pa
-00000890: 7273 652d 6269 7264 2d6c 696e 6b2d 6462  rse-bird-link-db
-000008a0: 202d 207c 206a 7120 7c20 6c65 7373 0d0a   - | jq | less..
-000008b0: 6060 600d 0a0d 0a23 2320 4465 7620 5365  ```....## Dev Se
-000008c0: 7475 700d 0a0d 0a50 7265 2d72 6571 7569  tup....Pre-requi
-000008d0: 7369 7465 733a 2060 7079 7468 6f6e 3360  sites: `python3`
-000008e0: 2061 7661 696c 6162 6c65 2076 6961 2074   available via t
-000008f0: 6865 2073 6865 6c6c 0d0a 0d0a 5365 7475  he shell....Setu
-00000900: 7020 6279 2063 6c6f 6e69 6e67 2c20 6372  p by cloning, cr
-00000910: 6561 7469 6e67 2061 2076 6972 7475 616c  eating a virtual
-00000920: 2065 6e76 2c20 616e 6420 696e 7374 616c   env, and instal
-00000930: 6c69 6e67 2074 6865 2061 7070 6c69 6361  ling the applica
-00000940: 7469 6f6e 0d0a 6060 6073 680d 0a67 6974  tion..```sh..git
-00000950: 2063 6c6f 6e65 2068 7474 7073 3a2f 2f67   clone https://g
-00000960: 6974 6875 622e 636f 6d2f 416e 6472 6577  ithub.com/Andrew
-00000970: 2d44 6963 6b69 6e73 6f6e 2f62 6972 642d  -Dickinson/bird-
-00000980: 6f73 7066 2d6c 696e 6b2d 6462 2d70 6172  ospf-link-db-par
-00000990: 7365 720d 0a63 6420 6269 7264 2d6f 7370  ser..cd bird-osp
-000009a0: 662d 6c69 6e6b 2d64 622d 7061 7273 6572  f-link-db-parser
-000009b0: 0d0a 7079 7468 6f6e 3320 2d6d 2076 656e  ..python3 -m ven
-000009c0: 7620 2e76 656e 760d 0a73 6f75 7263 6520  v .venv..source 
-000009d0: 2e76 656e 762f 6269 6e2f 6163 7469 7661  .venv/bin/activa
-000009e0: 7465 0d0a 7069 7020 696e 7374 616c 6c20  te..pip install 
-000009f0: 2d65 202e 0d0a 6060 600d 0a0d 0a74 6865  -e ...```....the
-00000a00: 6e20 696e 766f 6b65 2074 6865 2074 6f6f  n invoke the too
-00000a10: 6c20 7769 7468 2074 6865 2043 4c49 2063  l with the CLI c
-00000a20: 6f6d 6d61 6e64 3a0d 0a60 6060 7368 0d0a  ommand:..```sh..
-00000a30: 6269 7264 6320 7368 6f77 206f 7370 6620  birdc show ospf 
-00000a40: 6c69 6e6b 2073 7461 7465 2061 6c6c 203e  link state all >
-00000a50: 2070 6172 7365 2d62 6972 642d 6c69 6e6b   parse-bird-link
-00000a60: 2d64 6220 2d0d 0a60 6060 0d0a 0d0a 2323  -db -..```....##
-00000a70: 2052 756e 6e69 6e67 2074 6865 2075 6e69   Running the uni
-00000a80: 7420 7465 7374 730d 0a0d 0a46 6f6c 6c6f  t tests....Follo
-00000a90: 7720 7468 6520 696e 7374 7275 6374 696f  w the instructio
-00000aa0: 6e73 2075 6e64 6572 2022 4465 7620 5365  ns under "Dev Se
-00000ab0: 7475 7022 2061 626f 7665 2c20 746f 2063  tup" above, to c
-00000ac0: 6c6f 6e65 2061 206c 6f63 616c 2063 6f70  lone a local cop
-00000ad0: 7920 6f66 2074 6869 7320 6170 706c 6963  y of this applic
-00000ae0: 6174 696f 6e20 616e 6420 6163 7469 7661  ation and activa
-00000af0: 7465 0d0a 7468 6520 7669 7274 7561 6c20  te..the virtual 
-00000b00: 656e 7669 726f 6e6d 656e 742e 2054 6865  environment. The
-00000b10: 6e20 696e 7374 616c 6c69 6e67 2074 6865  n installing the
-00000b20: 2074 6573 7420 6465 7065 6e64 656e 6369   test dependenci
-00000b30: 6573 2077 6974 683a 0d0a 6060 6073 680d  es with:..```sh.
-00000b40: 0a70 6970 2069 6e73 7461 6c6c 202d 6520  .pip install -e 
-00000b50: 222e 5b74 6573 742c 6465 765d 220d 0a60  ".[test,dev]"..`
-00000b60: 6060 0d0a 0d0a 4669 6e61 6c6c 792c 2069  ``....Finally, i
-00000b70: 6e76 6f6b 6520 7468 6520 7465 7374 2073  nvoke the test s
-00000b80: 7569 7465 2075 7369 6e67 2070 7974 6573  uite using pytes
-00000b90: 743a 0d0a 6060 600d 0a70 7974 6573 7420  t:..```..pytest 
-00000ba0: 7465 7374 2f0d 0a60 6060 0d0a 0d0a 2323  test/..```....##
-00000bb0: 2042 7569 6c64 696e 6720 746f 2050 7950   Building to PyP
-00000bc0: 690d 0a0d 0a46 6f6c 6c6f 7720 7468 6520  i....Follow the 
-00000bd0: 696e 7374 7275 6374 696f 6e73 2061 626f  instructions abo
-00000be0: 7665 2074 6f20 636c 6f6e 6520 6120 6c6f  ve to clone a lo
-00000bf0: 6361 6c20 636f 7079 206f 6620 7468 6973  cal copy of this
-00000c00: 2061 7070 6c69 6361 7469 6f6e 2c20 6163   application, ac
-00000c10: 7469 7661 7465 0d0a 7468 6520 7669 7274  tivate..the virt
-00000c20: 7561 6c20 656e 7669 726f 6e6d 656e 742c  ual environment,
-00000c30: 2061 6e64 2072 756e 2074 6865 2074 6573   and run the tes
-00000c40: 7473 2e0d 0a0d 0a54 6865 6e2c 2062 7569  ts.....Then, bui
-00000c50: 6c64 2026 2075 706c 6f61 6420 7468 6520  ld & upload the 
-00000c60: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
-00000c70: 0d0a 6060 600d 0a72 6d20 2d72 6620 6469  ..```..rm -rf di
-00000c80: 7374 2f2a 0d0a 7079 7468 6f6e 202d 6d20  st/*..python -m 
-00000c90: 6275 696c 6420 2e0d 0a74 7769 6e65 2075  build ...twine u
-00000ca0: 706c 6f61 6420 6469 7374 2f2a 0d0a 6060  pload dist/*..``
-00000cb0: 600d 0a0d 0a23 2320 4c69 6365 6e73 650d  `....## License.
-00000cc0: 0a0d 0a44 6973 7472 6962 7574 6564 2075  ...Distributed u
-00000cd0: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
-00000ce0: 656e 7365 2e20 5365 6520 604c 4943 454e  ense. See `LICEN
-00000cf0: 5345 2e74 7874 6020 666f 7220 6d6f 7265  SE.txt` for more
-00000d00: 2069 6e66 6f72 6d61 7469 6f6e 2e0d 0a0d   information....
-00000d10: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
-00000d20: 0d0a 0d0a 436f 6e74 7269 6275 7469 6f6e  ....Contribution
-00000d30: 7320 6172 6520 7768 6174 206d 616b 6520  s are what make 
-00000d40: 7468 6520 6f70 656e 2073 6f75 7263 6520  the open source 
-00000d50: 636f 6d6d 756e 6974 7920 7375 6368 2061  community such a
-00000d60: 6e20 616d 617a 696e 6720 706c 6163 6520  n amazing place 
-00000d70: 746f 206c 6561 726e 2c20 696e 7370 6972  to learn, inspir
-00000d80: 652c 2061 6e64 2063 7265 6174 652e 2041  e, and create. A
-00000d90: 6e79 2063 6f6e 7472 6962 7574 696f 6e73  ny contributions
-00000da0: 2079 6f75 206d 616b 6520 6172 6520 2a2a   you make are **
-00000db0: 6772 6561 746c 7920 6170 7072 6563 6961  greatly apprecia
-00000dc0: 7465 642a 2a2e 0d0a 0d0a 4966 2079 6f75  ted**.....If you
-00000dd0: 2068 6176 6520 6120 7375 6767 6573 7469   have a suggesti
-00000de0: 6f6e 2074 6861 7420 776f 756c 6420 6d61  on that would ma
-00000df0: 6b65 2074 6869 7320 6265 7474 6572 2c20  ke this better, 
-00000e00: 706c 6561 7365 2066 6f72 6b20 7468 6520  please fork the 
-00000e10: 7265 706f 2061 6e64 2063 7265 6174 6520  repo and create 
-00000e20: 6120 7075 6c6c 2072 6571 7565 7374 2e20  a pull request. 
-00000e30: 596f 7520 6361 6e20 616c 736f 2073 696d  You can also sim
-00000e40: 706c 7920 6f70 656e 2061 6e20 6973 7375  ply open an issu
-00000e50: 6520 7769 7468 2074 6865 2074 6167 2022  e with the tag "
-00000e60: 656e 6861 6e63 656d 656e 7422 2e0d 0a44  enhancement"...D
-00000e70: 6f6e 2774 2066 6f72 6765 7420 746f 2067  on't forget to g
-00000e80: 6976 6520 7468 6520 7072 6f6a 6563 7420  ive the project 
-00000e90: 6120 7374 6172 2120 5468 616e 6b73 2061  a star! Thanks a
-00000ea0: 6761 696e 210d 0a0d 0a31 2e20 466f 726b  gain!....1. Fork
-00000eb0: 2074 6865 2050 726f 6a65 6374 0d0a 322e   the Project..2.
-00000ec0: 2043 7265 6174 6520 796f 7572 2046 6561   Create your Fea
-00000ed0: 7475 7265 2042 7261 6e63 6820 2860 6769  ture Branch (`gi
-00000ee0: 7420 6368 6563 6b6f 7574 202d 6220 6665  t checkout -b fe
-00000ef0: 6174 7572 652f 416d 617a 696e 6746 6561  ature/AmazingFea
-00000f00: 7475 7265 6029 0d0a 332e 2043 6f6d 6d69  ture`)..3. Commi
-00000f10: 7420 796f 7572 2043 6861 6e67 6573 2028  t your Changes (
-00000f20: 6067 6974 2063 6f6d 6d69 7420 2d6d 2027  `git commit -m '
-00000f30: 4164 6420 736f 6d65 2041 6d61 7a69 6e67  Add some Amazing
-00000f40: 4665 6174 7572 6527 6029 0d0a 342e 2050  Feature'`)..4. P
-00000f50: 7573 6820 746f 2074 6865 2042 7261 6e63  ush to the Branc
-00000f60: 6820 2860 6769 7420 7075 7368 206f 7269  h (`git push ori
-00000f70: 6769 6e20 6665 6174 7572 652f 416d 617a  gin feature/Amaz
-00000f80: 696e 6746 6561 7475 7265 6029 0d0a 352e  ingFeature`)..5.
-00000f90: 204f 7065 6e20 6120 5075 6c6c 2052 6571   Open a Pull Req
-00000fa0: 7565 7374 0d0a 0d0a 0d0a 2323 2041 636b  uest......## Ack
-00000fb0: 6e6f 776c 6564 676d 656e 7473 0d0a 202a  nowledgments.. *
-00000fc0: 205b 4265 7374 2d52 4541 444d 452d 5465   [Best-README-Te
-00000fd0: 6d70 6c61 7465 5d28 6874 7470 733a 2f2f  mplate](https://
-00000fe0: 6769 7468 7562 2e63 6f6d 2f6f 7468 6e65  github.com/othne
-00000ff0: 696c 6472 6577 2f42 6573 742d 5245 4144  ildrew/Best-READ
-00001000: 4d45 2d54 656d 706c 6174 652f 290d 0a    ME-Template/)..
+000000b0: 206f 7370 6620 7374 6174 6520 7c20 7061   ospf state | pa
+000000c0: 7273 652d 6269 7264 2d6c 696e 6b2d 6462  rse-bird-link-db
+000000d0: 202d 207c 206a 7120 7c20 6c65 7373 0d0a   - | jq | less..
+000000e0: 7b0d 0a20 2022 6172 6561 7322 3a20 7b0d  {..  "areas": {.
+000000f0: 0a20 2020 2022 302e 302e 302e 3022 3a20  .    "0.0.0.0": 
+00000100: 7b0d 0a20 2020 2020 2022 726f 7574 6572  {..      "router
+00000110: 7322 3a20 7b0d 0a20 2020 2020 2020 2022  s": {..        "
+00000120: 3130 2e36 382e 3239 2e35 3022 3a20 7b0d  10.68.29.50": {.
+00000130: 0a20 2020 2020 2020 2020 2022 6c69 6e6b  .          "link
+00000140: 7322 3a20 7b0d 0a20 2020 2020 2020 2020  s": {..         
+00000150: 2020 2022 726f 7574 6572 223a 205b 0d0a     "router": [..
+00000160: 2020 2020 2020 2020 2020 2020 2020 7b0d                {.
+00000170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000180: 2022 6964 223a 2022 3130 2e36 392e 372e   "id": "10.69.7.
+00000190: 3331 222c 0d0a 2020 2020 2020 2020 2020  31",..          
+000001a0: 2020 2020 2020 226d 6574 7269 6322 3a20        "metric": 
+000001b0: 3130 0d0a 2020 2020 2020 2020 2020 2020  10..            
+000001c0: 2020 7d0d 0a20 2020 2020 2020 2020 2020    }..           
+000001d0: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+000001e0: 2022 7374 7562 6e65 7422 3a20 5b0d 0a20   "stubnet": [.. 
+000001f0: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
+00000200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000210: 2269 6422 3a20 2231 302e 3639 2e32 392e  "id": "10.69.29.
+00000220: 3530 2f33 3222 2c0d 0a20 2020 2020 2020  50/32",..       
+00000230: 2020 2020 2020 2020 2022 6d65 7472 6963           "metric
+00000240: 223a 2030 0d0a 2020 2020 2020 2020 2020  ": 0..          
+00000250: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
+00000260: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+00000270: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00000280: 3130 2e36 382e 3239 2e35 302f 3332 222c  10.68.29.50/32",
+00000290: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000002a0: 2020 226d 6574 7269 6322 3a20 300d 0a20    "metric": 0.. 
+000002b0: 2020 2020 2020 2020 2020 2020 207d 0d0a               }..
+000002c0: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
+000002d0: 2020 2020 2020 2020 2020 2020 2265 7874              "ext
+000002e0: 6572 6e61 6c22 3a20 5b0d 0a20 2020 2020  ernal": [..     
+000002f0: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
+00000300: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00000310: 3a20 2231 302e 3730 2e31 3734 2e30 2f32  : "10.70.174.0/2
+00000320: 3422 2c0d 0a20 2020 2020 2020 2020 2020  4",..           
+00000330: 2020 2020 2022 6d65 7472 6963 223a 2032       "metric": 2
+00000340: 300d 0a20 2020 2020 2020 2020 2020 2020  0..             
+00000350: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00000360: 5d0d 0a20 2020 2020 2020 2020 207d 0d0a  ]..          }..
+00000370: 2020 2020 2020 2020 7d2c 0d0a 2020 2020          },..    
+00000380: 2020 2020 2231 302e 3638 2e37 332e 3132      "10.68.73.12
+00000390: 3522 3a20 7b0d 0a20 2020 2020 2020 2020  5": {..         
+000003a0: 2022 6c69 6e6b 7322 3a20 7b0d 0a20 2020   "links": {..   
+000003b0: 2020 2020 2020 2020 2022 726f 7574 6572           "router
+000003c0: 223a 205b 0d0a 2020 2020 2020 2020 2020  ": [..          
+000003d0: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
+000003e0: 2020 2020 2020 2022 6964 223a 2022 3130         "id": "10
+000003f0: 2e36 392e 3733 2e32 3522 2c0d 0a20 2020  .69.73.25",..   
+00000400: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
+00000410: 7472 6963 223a 2031 300d 0a20 2020 2020  tric": 10..     
+00000420: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
+00000430: 2020 2020 2020 2020 2020 207b 0d0a 2020             {..  
+00000440: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00000450: 6422 3a20 2231 302e 3639 2e35 322e 3833  d": "10.69.52.83
+00000460: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00000470: 2020 2020 226d 6574 7269 6322 3a20 3330      "metric": 30
+00000480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000490: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+000004a0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+000004b0: 2020 2020 2022 6964 223a 2022 3130 2e36       "id": "10.6
+000004c0: 392e 3733 2e32 3522 2c0d 0a20 2020 2020  9.73.25",..     
+000004d0: 2020 2020 2020 2020 2020 2022 6d65 7472             "metr
+000004e0: 6963 223a 2033 300d 0a20 2020 2020 2020  ic": 30..       
+000004f0: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00000500: 2020 2020 2020 5d2c 0d0a 2020 2020 2020        ],..      
+00000510: 2020 2020 2020 2273 7475 626e 6574 223a        "stubnet":
+00000520: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+00000530: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00000540: 2020 2020 2022 6964 223a 2022 3130 2e36       "id": "10.6
+00000550: 392e 3733 2e31 3235 2f33 3222 2c0d 0a20  9.73.125/32",.. 
+00000560: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000570: 6d65 7472 6963 223a 2030 0d0a 2020 2020  metric": 0..    
+00000580: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+00000590: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000005b0: 6964 223a 2022 3130 2e36 382e 3733 2e31  id": "10.68.73.1
+000005c0: 3235 2f33 3222 2c0d 0a20 2020 2020 2020  25/32",..       
+000005d0: 2020 2020 2020 2020 2022 6d65 7472 6963           "metric
+000005e0: 223a 2030 0d0a 2020 2020 2020 2020 2020  ": 0..          
+000005f0: 2020 2020 7d0d 0a20 2020 2020 2020 2020      }..         
+00000600: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
+00000610: 7d0d 0a20 2020 2020 2020 207d 2c0d 0a20  }..        },.. 
+00000620: 2020 2020 2020 202e 2e2e 0d0a 2020 2020         .....    
+00000630: 2020 7d0d 0a20 2020 207d 0d0a 2020 7d0d    }..    }..  }.
+00000640: 0a7d 0d0a 6060 600d 0a0d 0a23 2320 4f75  .}..```....## Ou
+00000650: 7470 7574 2046 6f72 6d61 740d 0a0d 0a54  tput Format....T
+00000660: 6865 206f 7574 7075 7420 666f 726d 6174  he output format
+00000670: 2069 7320 6465 7461 696c 6564 2075 7369   is detailed usi
+00000680: 6e67 205b 4a53 4f4e 2053 6368 656d 615d  ng [JSON Schema]
+00000690: 2868 7474 7073 3a2f 2f6a 736f 6e2d 7363  (https://json-sc
+000006a0: 6865 6d61 2e6f 7267 2f29 2069 6e20 6073  hema.org/) in `s
+000006b0: 7263 2f62 6972 645f 7061 7273 6572 2f6f  rc/bird_parser/o
+000006c0: 7574 7075 745f 7363 6865 6d61 2e6a 736f  utput_schema.jso
+000006d0: 6e60 0d0a 0d0a 2323 2055 7361 6765 0d0a  n`....## Usage..
+000006e0: 0d0a 5072 652d 7265 7175 6973 6974 6573  ..Pre-requisites
+000006f0: 3a20 6070 7974 686f 6e33 6020 6176 6169  : `python3` avai
+00000700: 6c61 626c 6520 7669 6120 7468 6520 7368  lable via the sh
+00000710: 656c 6c0d 0a0d 0a46 6972 7374 2c20 696e  ell....First, in
+00000720: 7374 616c 6c20 7468 6520 434c 4920 7669  stall the CLI vi
+00000730: 6120 7069 703a 0d0a 6060 6073 6865 6c6c  a pip:..```shell
+00000740: 0d0a 7069 7020 696e 7374 616c 6c20 6269  ..pip install bi
+00000750: 7264 2d6f 7370 662d 6c69 6e6b 2d64 622d  rd-ospf-link-db-
+00000760: 7061 7273 6572 0d0a 6060 600d 0a0d 0a74  parser..```....t
+00000770: 6865 6e20 696e 766f 6b65 2074 6865 2074  hen invoke the t
+00000780: 6f6f 6c20 7769 7468 2074 6865 2043 4c49  ool with the CLI
+00000790: 2063 6f6d 6d61 6e64 3a0d 0a60 6060 7368   command:..```sh
+000007a0: 656c 6c0d 0a62 6972 6463 2073 686f 7720  ell..birdc show 
+000007b0: 6f73 7066 2073 7461 7465 207c 2070 6172  ospf state | par
+000007c0: 7365 2d62 6972 642d 6c69 6e6b 2d64 6220  se-bird-link-db 
+000007d0: 2d0d 0a60 6060 0d0a 0d0a 4275 7420 796f  -..```....But yo
+000007e0: 7520 7072 6f62 6162 6c79 2077 616e 7420  u probably want 
+000007f0: 746f 2075 7365 2060 6a71 6020 616e 6420  to use `jq` and 
+00000800: 606c 6573 7360 2074 6f20 6d61 6b65 2074  `less` to make t
+00000810: 6869 7320 6f75 7470 7574 2061 2062 6974  his output a bit
+00000820: 206d 6f72 6520 6d61 6e61 6765 6162 6c65   more manageable
+00000830: 3a0d 0a60 6060 7368 656c 6c0d 0a73 7564  :..```shell..sud
+00000840: 6f20 6170 7420 7570 6461 7465 2026 2620  o apt update && 
+00000850: 7375 646f 2061 7074 2069 6e73 7461 6c6c  sudo apt install
+00000860: 206a 7120 6c65 7373 0d0a 6269 7264 6320   jq less..birdc 
+00000870: 7368 6f77 206f 7370 6620 7374 6174 6520  show ospf state 
+00000880: 7c20 7061 7273 652d 6269 7264 2d6c 696e  | parse-bird-lin
+00000890: 6b2d 6462 202d 207c 206a 7120 7c20 6c65  k-db - | jq | le
+000008a0: 7373 0d0a 6060 600d 0a0d 0a23 2320 4465  ss..```....## De
+000008b0: 7620 5365 7475 700d 0a0d 0a50 7265 2d72  v Setup....Pre-r
+000008c0: 6571 7569 7369 7465 733a 2060 7079 7468  equisites: `pyth
+000008d0: 6f6e 3360 2061 7661 696c 6162 6c65 2076  on3` available v
+000008e0: 6961 2074 6865 2073 6865 6c6c 0d0a 0d0a  ia the shell....
+000008f0: 5365 7475 7020 6279 2063 6c6f 6e69 6e67  Setup by cloning
+00000900: 2c20 6372 6561 7469 6e67 2061 2076 6972  , creating a vir
+00000910: 7475 616c 2065 6e76 2c20 616e 6420 696e  tual env, and in
+00000920: 7374 616c 6c69 6e67 2074 6865 2061 7070  stalling the app
+00000930: 6c69 6361 7469 6f6e 0d0a 6060 6073 680d  lication..```sh.
+00000940: 0a67 6974 2063 6c6f 6e65 2068 7474 7073  .git clone https
+00000950: 3a2f 2f67 6974 6875 622e 636f 6d2f 416e  ://github.com/An
+00000960: 6472 6577 2d44 6963 6b69 6e73 6f6e 2f62  drew-Dickinson/b
+00000970: 6972 642d 6f73 7066 2d6c 696e 6b2d 6462  ird-ospf-link-db
+00000980: 2d70 6172 7365 720d 0a63 6420 6269 7264  -parser..cd bird
+00000990: 2d6f 7370 662d 6c69 6e6b 2d64 622d 7061  -ospf-link-db-pa
+000009a0: 7273 6572 0d0a 7079 7468 6f6e 3320 2d6d  rser..python3 -m
+000009b0: 2076 656e 7620 2e76 656e 760d 0a73 6f75   venv .venv..sou
+000009c0: 7263 6520 2e76 656e 762f 6269 6e2f 6163  rce .venv/bin/ac
+000009d0: 7469 7661 7465 0d0a 7069 7020 696e 7374  tivate..pip inst
+000009e0: 616c 6c20 2d65 202e 0d0a 6060 600d 0a0d  all -e ...```...
+000009f0: 0a74 6865 6e20 696e 766f 6b65 2074 6865  .then invoke the
+00000a00: 2074 6f6f 6c20 7769 7468 2074 6865 2043   tool with the C
+00000a10: 4c49 2063 6f6d 6d61 6e64 3a0d 0a60 6060  LI command:..```
+00000a20: 7368 0d0a 6269 7264 6320 7368 6f77 206f  sh..birdc show o
+00000a30: 7370 6620 6c69 6e6b 2073 7461 7465 203e  spf link state >
+00000a40: 2070 6172 7365 2d62 6972 642d 6c69 6e6b   parse-bird-link
+00000a50: 2d64 6220 2d0d 0a60 6060 0d0a 0d0a 2323  -db -..```....##
+00000a60: 2052 756e 6e69 6e67 2074 6865 2075 6e69   Running the uni
+00000a70: 7420 7465 7374 730d 0a0d 0a46 6f6c 6c6f  t tests....Follo
+00000a80: 7720 7468 6520 696e 7374 7275 6374 696f  w the instructio
+00000a90: 6e73 2075 6e64 6572 2022 4465 7620 5365  ns under "Dev Se
+00000aa0: 7475 7022 2061 626f 7665 2c20 746f 2063  tup" above, to c
+00000ab0: 6c6f 6e65 2061 206c 6f63 616c 2063 6f70  lone a local cop
+00000ac0: 7920 6f66 2074 6869 7320 6170 706c 6963  y of this applic
+00000ad0: 6174 696f 6e20 616e 6420 6163 7469 7661  ation and activa
+00000ae0: 7465 0d0a 7468 6520 7669 7274 7561 6c20  te..the virtual 
+00000af0: 656e 7669 726f 6e6d 656e 742e 2054 6865  environment. The
+00000b00: 6e20 696e 7374 616c 6c69 6e67 2074 6865  n installing the
+00000b10: 2074 6573 7420 6465 7065 6e64 656e 6369   test dependenci
+00000b20: 6573 2077 6974 683a 0d0a 6060 6073 680d  es with:..```sh.
+00000b30: 0a70 6970 2069 6e73 7461 6c6c 202d 6520  .pip install -e 
+00000b40: 222e 5b74 6573 742c 6465 765d 220d 0a60  ".[test,dev]"..`
+00000b50: 6060 0d0a 0d0a 4669 6e61 6c6c 792c 2069  ``....Finally, i
+00000b60: 6e76 6f6b 6520 7468 6520 7465 7374 2073  nvoke the test s
+00000b70: 7569 7465 2075 7369 6e67 2070 7974 6573  uite using pytes
+00000b80: 743a 0d0a 6060 600d 0a70 7974 6573 7420  t:..```..pytest 
+00000b90: 7465 7374 2f0d 0a60 6060 0d0a 0d0a 2323  test/..```....##
+00000ba0: 2042 7569 6c64 696e 6720 746f 2050 7950   Building to PyP
+00000bb0: 690d 0a0d 0a46 6f6c 6c6f 7720 7468 6520  i....Follow the 
+00000bc0: 696e 7374 7275 6374 696f 6e73 2061 626f  instructions abo
+00000bd0: 7665 2074 6f20 636c 6f6e 6520 6120 6c6f  ve to clone a lo
+00000be0: 6361 6c20 636f 7079 206f 6620 7468 6973  cal copy of this
+00000bf0: 2061 7070 6c69 6361 7469 6f6e 2c20 6163   application, ac
+00000c00: 7469 7661 7465 0d0a 7468 6520 7669 7274  tivate..the virt
+00000c10: 7561 6c20 656e 7669 726f 6e6d 656e 742c  ual environment,
+00000c20: 2061 6e64 2072 756e 2074 6865 2074 6573   and run the tes
+00000c30: 7473 2e0d 0a0d 0a54 6865 6e2c 2062 7569  ts.....Then, bui
+00000c40: 6c64 2026 2075 706c 6f61 6420 7468 6520  ld & upload the 
+00000c50: 6170 706c 6963 6174 696f 6e20 7769 7468  application with
+00000c60: 0d0a 6060 600d 0a72 6d20 2d72 6620 6469  ..```..rm -rf di
+00000c70: 7374 2f2a 0d0a 7079 7468 6f6e 202d 6d20  st/*..python -m 
+00000c80: 6275 696c 6420 2e0d 0a74 7769 6e65 2075  build ...twine u
+00000c90: 706c 6f61 6420 6469 7374 2f2a 0d0a 6060  pload dist/*..``
+00000ca0: 600d 0a0d 0a23 2320 4c69 6365 6e73 650d  `....## License.
+00000cb0: 0a0d 0a44 6973 7472 6962 7574 6564 2075  ...Distributed u
+00000cc0: 6e64 6572 2074 6865 204d 4954 204c 6963  nder the MIT Lic
+00000cd0: 656e 7365 2e20 5365 6520 604c 4943 454e  ense. See `LICEN
+00000ce0: 5345 2e74 7874 6020 666f 7220 6d6f 7265  SE.txt` for more
+00000cf0: 2069 6e66 6f72 6d61 7469 6f6e 2e0d 0a0d   information....
+00000d00: 0a23 2320 436f 6e74 7269 6275 7469 6e67  .## Contributing
+00000d10: 0d0a 0d0a 436f 6e74 7269 6275 7469 6f6e  ....Contribution
+00000d20: 7320 6172 6520 7768 6174 206d 616b 6520  s are what make 
+00000d30: 7468 6520 6f70 656e 2073 6f75 7263 6520  the open source 
+00000d40: 636f 6d6d 756e 6974 7920 7375 6368 2061  community such a
+00000d50: 6e20 616d 617a 696e 6720 706c 6163 6520  n amazing place 
+00000d60: 746f 206c 6561 726e 2c20 696e 7370 6972  to learn, inspir
+00000d70: 652c 2061 6e64 2063 7265 6174 652e 2041  e, and create. A
+00000d80: 6e79 2063 6f6e 7472 6962 7574 696f 6e73  ny contributions
+00000d90: 2079 6f75 206d 616b 6520 6172 6520 2a2a   you make are **
+00000da0: 6772 6561 746c 7920 6170 7072 6563 6961  greatly apprecia
+00000db0: 7465 642a 2a2e 0d0a 0d0a 4966 2079 6f75  ted**.....If you
+00000dc0: 2068 6176 6520 6120 7375 6767 6573 7469   have a suggesti
+00000dd0: 6f6e 2074 6861 7420 776f 756c 6420 6d61  on that would ma
+00000de0: 6b65 2074 6869 7320 6265 7474 6572 2c20  ke this better, 
+00000df0: 706c 6561 7365 2066 6f72 6b20 7468 6520  please fork the 
+00000e00: 7265 706f 2061 6e64 2063 7265 6174 6520  repo and create 
+00000e10: 6120 7075 6c6c 2072 6571 7565 7374 2e20  a pull request. 
+00000e20: 596f 7520 6361 6e20 616c 736f 2073 696d  You can also sim
+00000e30: 706c 7920 6f70 656e 2061 6e20 6973 7375  ply open an issu
+00000e40: 6520 7769 7468 2074 6865 2074 6167 2022  e with the tag "
+00000e50: 656e 6861 6e63 656d 656e 7422 2e0d 0a44  enhancement"...D
+00000e60: 6f6e 2774 2066 6f72 6765 7420 746f 2067  on't forget to g
+00000e70: 6976 6520 7468 6520 7072 6f6a 6563 7420  ive the project 
+00000e80: 6120 7374 6172 2120 5468 616e 6b73 2061  a star! Thanks a
+00000e90: 6761 696e 210d 0a0d 0a31 2e20 466f 726b  gain!....1. Fork
+00000ea0: 2074 6865 2050 726f 6a65 6374 0d0a 322e   the Project..2.
+00000eb0: 2043 7265 6174 6520 796f 7572 2046 6561   Create your Fea
+00000ec0: 7475 7265 2042 7261 6e63 6820 2860 6769  ture Branch (`gi
+00000ed0: 7420 6368 6563 6b6f 7574 202d 6220 6665  t checkout -b fe
+00000ee0: 6174 7572 652f 416d 617a 696e 6746 6561  ature/AmazingFea
+00000ef0: 7475 7265 6029 0d0a 332e 2043 6f6d 6d69  ture`)..3. Commi
+00000f00: 7420 796f 7572 2043 6861 6e67 6573 2028  t your Changes (
+00000f10: 6067 6974 2063 6f6d 6d69 7420 2d6d 2027  `git commit -m '
+00000f20: 4164 6420 736f 6d65 2041 6d61 7a69 6e67  Add some Amazing
+00000f30: 4665 6174 7572 6527 6029 0d0a 342e 2050  Feature'`)..4. P
+00000f40: 7573 6820 746f 2074 6865 2042 7261 6e63  ush to the Branc
+00000f50: 6820 2860 6769 7420 7075 7368 206f 7269  h (`git push ori
+00000f60: 6769 6e20 6665 6174 7572 652f 416d 617a  gin feature/Amaz
+00000f70: 696e 6746 6561 7475 7265 6029 0d0a 352e  ingFeature`)..5.
+00000f80: 204f 7065 6e20 6120 5075 6c6c 2052 6571   Open a Pull Req
+00000f90: 7565 7374 0d0a 0d0a 0d0a 2323 2041 636b  uest......## Ack
+00000fa0: 6e6f 776c 6564 676d 656e 7473 0d0a 202a  nowledgments.. *
+00000fb0: 205b 4265 7374 2d52 4541 444d 452d 5465   [Best-README-Te
+00000fc0: 6d70 6c61 7465 5d28 6874 7470 733a 2f2f  mplate](https://
+00000fd0: 6769 7468 7562 2e63 6f6d 2f6f 7468 6e65  github.com/othne
+00000fe0: 696c 6472 6577 2f42 6573 742d 5245 4144  ildrew/Best-READ
+00000ff0: 4d45 2d54 656d 706c 6174 652f 290d 0a    ME-Template/)..
```

### Comparing `bird-ospf-link-db-parser-1.1.2/pyproject.toml` & `bird-ospf-link-db-parser-1.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bird-ospf-link-db-parser"
-version = "1.1.2"
+version = "1.1.3"
 authors = [{ name = "Andrew Dickinson", email = "andrew.dickinson.0216@gmail.com" }]
 description = "Parse the text output from the BIRD Routing Daemon's OSPF link database into machine readable JSON"
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

### Comparing `bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/PKG-INFO` & `bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bird-ospf-link-db-parser
-Version: 1.1.2
+Version: 1.1.3
 Summary: Parse the text output from the BIRD Routing Daemon's OSPF link database into machine readable JSON
 Author-email: Andrew Dickinson <andrew.dickinson.0216@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Andrew Dickinson
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,15 +36,15 @@
 
 
 # Bird OSFP Link Database Parser
 
 Parses the output of the BIRD Routing Daemon's `birdc show ospf state` command into a machine-readable JSON string.
 
 ```sh
-> birdc show ospf state all | parse-bird-link-db - | jq | less
+> birdc show ospf state | parse-bird-link-db - | jq | less
 {
   "areas": {
     "0.0.0.0": {
       "routers": {
         "10.68.29.50": {
           "links": {
             "router": [
@@ -117,21 +117,21 @@
 First, install the CLI via pip:
 ```shell
 pip install bird-ospf-link-db-parser
 ```
 
 then invoke the tool with the CLI command:
 ```shell
-birdc show ospf state all | parse-bird-link-db -
+birdc show ospf state | parse-bird-link-db -
 ```
 
 But you probably want to use `jq` and `less` to make this output a bit more manageable:
 ```shell
 sudo apt update && sudo apt install jq less
-birdc show ospf state all | parse-bird-link-db - | jq | less
+birdc show ospf state | parse-bird-link-db - | jq | less
 ```
 
 ## Dev Setup
 
 Pre-requisites: `python3` available via the shell
 
 Setup by cloning, creating a virtual env, and installing the application
@@ -141,15 +141,15 @@
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -e .
 ```
 
 then invoke the tool with the CLI command:
 ```sh
-birdc show ospf link state all > parse-bird-link-db -
+birdc show ospf link state > parse-bird-link-db -
 ```
 
 ## Running the unit tests
 
 Follow the instructions under "Dev Setup" above, to clone a local copy of this application and activate
 the virtual environment. Then installing the test dependencies with:
 ```sh
```

### Comparing `bird-ospf-link-db-parser-1.1.2/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt` & `bird-ospf-link-db-parser-1.1.3/src/bird_ospf_link_db_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/src/bird_parser/main.py` & `bird-ospf-link-db-parser-1.1.3/src/bird_parser/main.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/src/bird_parser/output_schema.json` & `bird-ospf-link-db-parser-1.1.3/src/bird_parser/output_schema.json`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/src/bird_parser/parse_bird_output.py` & `bird-ospf-link-db-parser-1.1.3/src/bird_parser/parse_bird_output.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/src/bird_parser/utils.py` & `bird-ospf-link-db-parser-1.1.3/src/bird_parser/utils.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/test/test_comprehensive.py` & `bird-ospf-link-db-parser-1.1.3/test/test_comprehensive.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/test/test_live_data.py` & `bird-ospf-link-db-parser-1.1.3/test/test_live_data.py`

 * *Files identical despite different names*

### Comparing `bird-ospf-link-db-parser-1.1.2/test/test_simple.py` & `bird-ospf-link-db-parser-1.1.3/test/test_simple.py`

 * *Files identical despite different names*

