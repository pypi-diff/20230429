# Comparing `tmp/alacorder-80.0.4.tar.gz` & `tmp/alacorder-80.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.0.4.tar", max compression
+gzip compressed data, was "alacorder-80.0.5.tar", max compression
```

## Comparing `alacorder-80.0.4.tar` & `alacorder-80.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.4/LICENSE
--rw-r--r--   0        0        0     6750 2023-04-29 03:07:07.203418 alacorder-80.0.4/README.md
--rw-r--r--   0        0        0      697 2023-04-29 15:42:32.152293 alacorder-80.0.4/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-04-29 14:45:34.879592 alacorder-80.0.4/src/alacorder/.DS_Store
--rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   198019 2023-04-29 15:42:47.194263 alacorder-80.0.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   198019 2023-04-29 15:42:19.631622 alacorder-80.0.4/src/alacorder/alac.py
--rw-r--r--   0        0        0     7679 1970-01-01 00:00:00.000000 alacorder-80.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.0.5/LICENSE
+-rw-r--r--   0        0        0     6821 2023-04-29 16:14:55.778453 alacorder-80.0.5/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 16:03:14.696382 alacorder-80.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-04-29 15:44:27.166659 alacorder-80.0.5/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0     1784 2023-04-21 19:12:38.269775 alacorder-80.0.5/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   198035 2023-04-29 16:02:26.019897 alacorder-80.0.5/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   198035 2023-04-29 16:02:31.026154 alacorder-80.0.5/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7750 1970-01-01 00:00:00.000000 alacorder-80.0.5/PKG-INFO
```

### Comparing `alacorder-80.0.4/LICENSE` & `alacorder-80.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.4/README.md` & `alacorder-80.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -187,236 +187,241 @@
 00000ba0: 2020 2020 2020 2020 2020 4578 706f 7274            Export
 00000bb0: 2061 6c6c 2064 6174 6120 7461 626c 6573   all data tables
 00000bc0: 2074 6f20 2e78 6c73 2f2e 786c 7378 0a20   to .xls/.xlsx. 
 00000bd0: 2070 6169 7220 2020 2020 2020 2020 2020   pair           
 00000be0: 2020 2020 2020 4372 6561 7465 2062 6c61        Create bla
 00000bf0: 6e6b 2041 4953 202f 2075 6e69 7175 6520  nk AIS / unique 
 00000c00: 7061 6972 696e 6720 7465 6d70 6c61 7465  pairing template
-00000c10: 0a20 2073 6574 7469 6e67 7320 2020 2020  .  settings     
-00000c20: 2020 2020 2020 2020 4372 6561 7465 2061          Create a
-00000c30: 6e64 2065 7870 6f72 7420 7365 7474 696e  nd export settin
-00000c40: 6773 2074 6162 6c65 0a20 2073 7461 7274  gs table.  start
-00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c60: 4c61 756e 6368 2067 7261 7068 6963 616c  Launch graphical
-00000c70: 2075 7365 7220 696e 7465 7266 6163 650a   user interface.
-00000c80: 2020 7461 626c 6520 2020 2020 2020 2020    table         
-00000c90: 2020 2020 2020 2045 7870 6f72 7420 6461         Export da
-00000ca0: 7461 2074 6162 6c65 7320 6672 6f6d 2061  ta tables from a
-00000cb0: 7263 6869 7665 206f 7220 6469 7265 6374  rchive or direct
-00000cc0: 6f72 790a 2020 7672 722d 7061 6972 7320  ory.  vrr-pairs 
-00000cd0: 2020 2020 2020 2020 2020 2043 7265 6174             Creat
-00000ce0: 6520 766f 7469 6e67 2072 6967 6874 7320  e voting rights 
-00000cf0: 7375 6d6d 6172 7920 6672 6f6d 2069 6e70  summary from inp
-00000d00: 7574 2063 6173 6573 2061 6e64 2070 6169  ut cases and pai
-00000d10: 7273 0a20 2077 6974 6e65 7373 6573 2020  rs.  witnesses  
-00000d20: 2020 2020 2020 2020 2020 4372 6561 7465            Create
-00000d30: 2061 6e64 2065 7870 6f72 7420 7769 746e   and export witn
-00000d40: 6573 7365 7320 7461 626c 650a 6060 600a  esses table.```.
-00000d50: 0a23 2320 4665 7463 6820 6361 7365 7320  .## Fetch cases 
-00000d60: 696e 2062 756c 6b20 6672 6f6d 2041 6c61  in bulk from Ala
-00000d70: 636f 7572 742e 636f 6d20 0a0a 5461 6b65  court.com ..Take
-00000d80: 2061 2073 7072 6561 6473 6865 6574 206f   a spreadsheet o
-00000d90: 6620 6e61 6d65 7320 616e 642f 6f72 206f  f names and/or o
-00000da0: 7468 6572 2073 6561 7263 6820 7061 7261  ther search para
-00000db0: 6d65 7465 7273 2061 6e64 2064 6f77 6e6c  meters and downl
-00000dc0: 6f61 6420 6361 7365 2050 4446 7320 6672  oad case PDFs fr
-00000dd0: 6f6d 2041 6c61 636f 7572 7420 696e 2062  om Alacourt in b
-00000de0: 756c 6b2e 2044 6f77 6e6c 6f61 6420 7468  ulk. Download th
-00000df0: 6f75 7361 6e64 7320 6f66 2050 4446 7320  ousands of PDFs 
-00000e00: 696e 206a 7573 7420 686f 7572 7320 6279  in just hours by
-00000e10: 206c 6561 7669 6e67 2079 6f75 7220 636f   leaving your co
-00000e20: 6d70 7574 6572 2075 6e61 7474 656e 6465  mputer unattende
-00000e30: 642e 2028 476f 6f67 6c65 2043 6872 6f6d  d. (Google Chrom
-00000e40: 6520 6973 2072 6571 7569 7265 6420 746f  e is required to
-00000e50: 2075 7365 2074 6865 2060 6665 7463 6860   use the `fetch`
-00000e60: 2066 6561 7475 7265 2e29 0a0a 6060 600a   feature.)..```.
-00000e70: 5573 6167 653a 2070 7974 686f 6e20 2d6d  Usage: python -m
-00000e80: 2061 6c61 636f 7264 6572 2066 6574 6368   alacorder fetch
-00000e90: 205b 4f50 5449 4f4e 535d 0a0a 2020 4665   [OPTIONS]..  Fe
-00000ea0: 7463 6820 6361 7365 7320 6672 6f6d 2041  tch cases from A
-00000eb0: 6c61 636f 7572 742e 636f 6d0a 0a4f 7074  lacourt.com..Opt
-00000ec0: 696f 6e73 3a0a 2020 2d69 6e2c 202d 2d69  ions:.  -in, --i
-00000ed0: 6e70 7574 2d70 6174 6820 5041 5448 2020  nput-path PATH  
-00000ee0: 2020 5061 7468 2074 6f20 7175 6572 7920    Path to query 
-00000ef0: 7461 626c 652f 7370 7265 6164 7368 6565  table/spreadshee
-00000f00: 7420 282e 786c 732c 202e 786c 7378 290a  t (.xls, .xlsx).
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 2020 2020 2020 5b72 6571              [req
-00000f30: 7569 7265 645d 0a20 202d 6f75 742c 202d  uired].  -out, -
-00000f40: 2d6f 7574 7075 742d 7061 7468 2050 4154  -output-path PAT
-00000f50: 4820 2044 6573 6972 6564 2050 4446 206f  H  Desired PDF o
-00000f60: 7574 7075 7420 6469 7265 6374 6f72 7920  utput directory 
-00000f70: 205b 7265 7175 6972 6564 5d0a 2020 2d63   [required].  -c
-00000f80: 2c20 2d2d 6375 7374 6f6d 6572 2d69 6420  , --customer-id 
-00000f90: 5445 5854 2020 2020 4375 7374 6f6d 6572  TEXT    Customer
-00000fa0: 2049 4420 6f6e 2041 6c61 636f 7572 742e   ID on Alacourt.
-00000fb0: 636f 6d20 205b 7265 7175 6972 6564 5d0a  com  [required].
-00000fc0: 2020 2d75 2c20 2d2d 7573 6572 2d69 6420    -u, --user-id 
-00000fd0: 5445 5854 2020 2020 2020 2020 5573 6572  TEXT        User
-00000fe0: 2049 4420 6f6e 2041 6c61 636f 7572 742e   ID on Alacourt.
-00000ff0: 636f 6d20 205b 7265 7175 6972 6564 5d0a  com  [required].
-00001000: 2020 2d70 2c20 2d2d 7061 7373 776f 7264    -p, --password
-00001010: 2054 4558 5420 2020 2020 2020 5061 7373   TEXT       Pass
-00001020: 776f 7264 206f 6e20 416c 6163 6f75 7274  word on Alacourt
-00001030: 2e63 6f6d 2020 5b72 6571 7569 7265 645d  .com  [required]
-00001040: 0a20 202d 6d61 782c 202d 2d6d 6178 2049  .  -max, --max I
-00001050: 4e54 4547 4552 2020 2020 2020 204d 6178  NTEGER       Max
-00001060: 696d 756d 2071 7565 7269 6573 2074 6f20  imum queries to 
-00001070: 636f 6e64 7563 7420 6f6e 2041 6c61 636f  conduct on Alaco
-00001080: 7572 742e 636f 6d0a 2020 2d73 6b69 702c  urt.com.  -skip,
-00001090: 202d 2d73 6b69 7020 494e 5445 4745 5220   --skip INTEGER 
-000010a0: 2020 2020 536b 6970 2065 6e74 7269 6573      Skip entries
-000010b0: 2061 7420 746f 7020 6f66 2071 7565 7279   at top of query
-000010c0: 2066 696c 650a 2020 2d6e 2c20 2d2d 6e6f   file.  -n, --no
-000010d0: 2d6d 6172 6b20 2020 2020 2020 2020 2020  -mark           
-000010e0: 2020 446f 206e 6f74 2075 7064 6174 6520    Do not update 
-000010f0: 7175 6572 7920 7465 6d70 6c61 7465 2061  query template a
-00001100: 6674 6572 2063 6f6d 706c 6574 696f 6e0a  fter completion.
-00001110: 2020 2d2d 6465 6275 6720 2020 2020 2020    --debug       
-00001120: 2020 2020 2020 2020 2020 2020 5072 696e              Prin
-00001130: 7420 6465 7461 696c 6564 2072 756e 7469  t detailed runti
-00001140: 6d65 2069 6e66 6f72 6d61 7469 6f6e 2074  me information t
-00001150: 6f20 636f 6e73 6f6c 650a 2020 2d68 2c20  o console.  -h, 
-00001160: 2d2d 6865 6c70 2020 2020 2020 2020 2020  --help          
-00001170: 2020 2020 2020 5368 6f77 2074 6869 7320        Show this 
-00001180: 6d65 7373 6167 6520 616e 6420 6578 6974  message and exit
-00001190: 2e0a 6060 600a 0a0a 2320 2a2a 576f 726b  ..```...# **Work
-000011a0: 696e 6720 7769 7468 2063 6173 6520 6461  ing with case da
-000011b0: 7461 2069 6e20 5079 7468 6f6e 2a2a 0a0a  ta in Python**..
-000011c0: 0a23 2323 204f 7574 206f 6620 7468 6520  .### Out of the 
-000011d0: 626f 782c 2041 6c61 636f 7264 6572 2065  box, Alacorder e
-000011e0: 7870 6f72 7473 2074 6f20 602e 786c 7378  xports to `.xlsx
-000011f0: 602c 2060 2e78 6c73 602c 2060 2e63 7376  `, `.xls`, `.csv
-00001200: 602c 2060 2e6a 736f 6e60 2c20 616e 6420  `, `.json`, and 
-00001210: 602e 7061 7271 7565 7460 2e20 4275 7420  `.parquet`. But 
-00001220: 796f 7520 6361 6e20 7573 6520 6070 6f6c  you can use `pol
-00001230: 6172 7360 2061 6e64 206f 7468 6572 2070  ars` and other p
-00001240: 7974 686f 6e20 6c69 6272 6172 6965 7320  ython libraries 
-00001250: 746f 2063 7265 6174 6520 796f 7572 206f  to create your o
-00001260: 776e 2064 6174 6120 636f 6c6c 6563 7469  wn data collecti
-00001270: 6f6e 2077 6f72 6b66 6c6f 7773 2061 6e64  on workflows and
-00001280: 2063 7573 746f 6d69 7a65 2041 6c61 636f   customize Alaco
-00001290: 7264 6572 2065 7870 6f72 7473 2e20 0a0a  rder exports. ..
-000012a0: 2a2a 2a54 6865 2073 6e69 7070 6574 2062  ***The snippet b
-000012b0: 656c 6f77 2070 7269 6e74 7320 7468 6520  elow prints the 
-000012c0: 6665 6520 7368 6565 7473 2066 726f 6d20  fee sheets from 
-000012d0: 6120 6469 7265 6374 6f72 7920 6f66 2063  a directory of c
-000012e0: 6173 6520 5044 4673 2061 7320 6974 2072  ase PDFs as it r
-000012f0: 6561 6473 2074 6865 6d2e 2a2a 2a0a 0a0a  eads them.***...
-00001300: 6060 6070 7974 686f 6e0a 6672 6f6d 2061  ```python.from a
-00001310: 6c61 636f 7264 6572 2069 6d70 6f72 7420  lacorder import 
-00001320: 616c 6163 0a69 6d70 6f72 7420 706f 6c61  alac.import pola
-00001330: 7273 2061 7320 706c 0a0a 7175 6575 6520  rs as pl..queue 
-00001340: 3d20 616c 6163 2e67 6574 5f70 6174 6873  = alac.get_paths
-00001350: 2822 2f55 7365 7273 2f63 7269 6d73 6f6e  ("/Users/crimson
-00001360: 2f44 6573 6b74 6f70 2f54 7574 7769 6c65  /Desktop/Tutwile
-00001370: 722f 2229 2023 202d 3e20 5b73 7472 5d0a  r/") # -> [str].
-00001380: 0a72 6f77 7320 3d20 5b5d 0a0a 666f 7220  .rows = []..for 
-00001390: 692c 2070 6174 6820 696e 2065 6e75 6d65  i, path in enume
-000013a0: 7261 7465 2871 7565 7565 293a 0a20 2020  rate(queue):.   
-000013b0: 2074 6578 7420 3d20 616c 6163 2e65 7874   text = alac.ext
-000013c0: 7261 6374 5f74 6578 7428 7061 7468 290a  ract_text(path).
-000013d0: 2020 2020 636e 756d 203d 2061 6c61 632e      cnum = alac.
-000013e0: 6765 7443 6173 654e 756d 6265 7228 7465  getCaseNumber(te
-000013f0: 7874 290a 2020 2020 6374 7920 3d20 616c  xt).    cty = al
-00001400: 6163 2e67 6574 436f 756e 7479 2874 6578  ac.getCounty(tex
-00001410: 7429 0a20 2020 2074 6261 6c20 3d20 616c  t).    tbal = al
-00001420: 6163 2e67 6574 546f 7461 6c42 616c 616e  ac.getTotalBalan
-00001430: 6365 2874 6578 7429 0a20 2020 2070 7472  ce(text).    ptr
-00001440: 203d 2061 6c61 632e 6765 7450 6179 6d65   = alac.getPayme
-00001450: 6e74 546f 5265 7374 6f72 6528 7465 7874  ntToRestore(text
-00001460: 2920 2320 692e 652e 2076 6f74 696e 6720  ) # i.e. voting 
-00001470: 7269 6768 7473 0a20 2020 2072 6f77 7320  rights.    rows 
-00001480: 2b3d 205b 5b63 6e75 6d2c 2063 7479 2c20  += [[cnum, cty, 
-00001490: 7462 616c 2c20 7074 725d 5d0a 0a63 6173  tbal, ptr]]..cas
-000014a0: 6573 203d 2070 6c2e 4461 7461 4672 616d  es = pl.DataFram
-000014b0: 6528 726f 7773 290a 0a63 6173 6573 2e77  e(rows)..cases.w
-000014c0: 7269 7465 5f65 7863 656c 2822 2f55 7365  rite_excel("/Use
-000014d0: 7273 2f63 7269 6d73 6f6e 2f44 6573 6b74  rs/crimson/Deskt
-000014e0: 6f70 2f54 7574 7769 6c65 722f 7375 6d6d  op/Tutwiler/summ
-000014f0: 6172 792e 786c 7378 2229 0a0a 6060 600a  ary.xlsx")..```.
-00001500: 0a23 2320 4578 7465 6e64 696e 6720 416c  .## Extending Al
-00001510: 6163 6f72 6465 7220 7769 7468 2060 706f  acorder with `po
-00001520: 6c61 7273 6020 616e 6420 6f74 6865 7220  lars` and other 
-00001530: 746f 6f6c 730a 0a41 6c61 636f 7264 6572  tools..Alacorder
-00001540: 2072 756e 7320 6f6e 205b 6070 6f6c 6172   runs on [`polar
-00001550: 7360 5d28 6874 7470 733a 2f2f 6769 7468  s`](https://gith
-00001560: 7562 2e63 6f6d 2f70 6f6c 612d 7273 2f70  ub.com/pola-rs/p
-00001570: 6f6c 6172 7329 2c20 6120 7079 7468 6f6e  olars), a python
-00001580: 206c 6962 7261 7279 2079 6f75 2063 616e   library you can
-00001590: 2075 7365 2074 6f20 776f 726b 2077 6974   use to work wit
-000015a0: 6820 616e 6420 616e 616c 797a 6520 7461  h and analyze ta
-000015b0: 6275 6c61 7220 6461 7461 2e20 6070 6f6c  bular data. `pol
-000015c0: 6172 7360 2063 616e 2072 6561 6420 6672  ars` can read fr
-000015d0: 6f6d 2061 6e64 2077 7269 7465 2074 6f20  om and write to 
-000015e0: 616c 6c20 6d61 6a6f 7220 6461 7461 2073  all major data s
-000015f0: 746f 7261 6765 2066 6f72 6d61 7473 2e20  torage formats. 
-00001600: 4974 2063 616e 2063 6f6e 6e65 6374 2074  It can connect t
-00001610: 6f20 6120 7769 6465 2076 6172 6965 7479  o a wide variety
-00001620: 206f 6620 7365 7276 6963 6573 2074 6f20   of services to 
-00001630: 7072 6f76 6964 6520 666f 7220 6561 7379  provide for easy
-00001640: 2069 6d70 6f72 7420 616e 6420 6578 706f   import and expo
-00001650: 7274 2e0a 0a60 6060 7079 7468 6f6e 0a69  rt...```python.i
-00001660: 6d70 6f72 7420 706f 6c61 7273 2061 7320  mport polars as 
-00001670: 706c 0a63 6f6e 7465 6e74 7320 3d20 706c  pl.contents = pl
-00001680: 2e72 6561 645f 6a73 6f6e 2822 2f70 6174  .read_json("/pat
-00001690: 682f 746f 2f61 7263 6869 7665 2e6a 736f  h/to/archive.jso
-000016a0: 6e22 290a 6060 600a 0a49 6620 796f 7520  n").```..If you 
-000016b0: 776f 756c 6420 6c69 6b65 2074 6f20 7669  would like to vi
-000016c0: 7375 616c 697a 6520 6461 7461 2077 6974  sualize data wit
-000016d0: 686f 7574 2065 7870 6f72 7469 6e67 2074  hout exporting t
-000016e0: 6f20 4578 6365 6c20 6f72 2061 6e6f 7468  o Excel or anoth
-000016f0: 6572 2066 6f72 6d61 742c 2063 7265 6174  er format, creat
-00001700: 6520 6120 606a 7570 7974 6572 206e 6f74  e a `jupyter not
-00001710: 6562 6f6f 6b60 2061 6e64 2069 6e73 7461  ebook` and insta
-00001720: 6c6c 2074 6f6f 6c73 206c 696b 6520 606d  ll tools like `m
-00001730: 6174 706c 6f74 6c69 6260 2c20 6074 6162  atplotlib`, `tab
-00001740: 756c 6174 6560 2c20 616e 6420 6069 7461  ulate`, and `ita
-00001750: 626c 6573 6020 746f 2067 6574 2073 7461  bles` to get sta
-00001760: 7274 6564 2e20 5b4a 7570 7974 6572 204e  rted. [Jupyter N
-00001770: 6f74 6562 6f6f 6b5d 2868 7474 7073 3a2f  otebook](https:/
-00001780: 2f64 6f63 732e 6a75 7079 7465 722e 6f72  /docs.jupyter.or
-00001790: 672f 656e 2f6c 6174 6573 742f 7374 6172  g/en/latest/star
-000017a0: 742f 696e 6465 782e 6874 6d6c 2920 6973  t/index.html) is
-000017b0: 2061 2050 7974 686f 6e20 7072 6f6a 6563   a Python projec
-000017c0: 7420 796f 7520 6361 6e20 7573 6520 746f  t you can use to
-000017d0: 2063 7265 6174 6520 696e 7465 7261 6374   create interact
-000017e0: 6976 6520 6e6f 7465 626f 6f6b 7320 666f  ive notebooks fo
-000017f0: 7220 6461 7461 2061 6e61 6c79 7369 7320  r data analysis 
-00001800: 616e 6420 6f74 6865 7220 7075 7270 6f73  and other purpos
-00001810: 6573 2e20 4974 2063 616e 2062 6520 696e  es. It can be in
-00001820: 7374 616c 6c65 6420 7573 696e 6720 6070  stalled using `p
-00001830: 6970 2069 6e73 7461 6c6c 206a 7570 7974  ip install jupyt
-00001840: 6572 6020 6f72 2060 7069 7033 2069 6e73  er` or `pip3 ins
-00001850: 7461 6c6c 206a 7570 7974 6572 6020 616e  tall jupyter` an
-00001860: 6420 6c61 756e 6368 6564 2075 7369 6e67  d launched using
-00001870: 2060 6a75 7079 7465 7220 6e6f 7465 626f   `jupyter notebo
-00001880: 6f6b 602e 2059 6f75 7220 6465 7669 6365  ok`. Your device
-00001890: 206d 6179 2061 6c72 6561 6479 2062 6520   may already be 
-000018a0: 6571 7569 7070 6564 2074 6f20 7669 6577  equipped to view
-000018b0: 2060 2e69 7079 6e62 6020 6e6f 7465 626f   `.ipynb` notebo
-000018c0: 6f6b 732e 200a 0a23 2320 2a2a 5265 736f  oks. ..## **Reso
-000018d0: 7572 6365 732a 2a0a 2a20 5b60 706f 6c61  urces**.* [`pola
-000018e0: 7273 6020 7573 6572 2067 7569 6465 5d28  rs` user guide](
-000018f0: 6874 7470 733a 2f2f 706f 6c61 2d72 732e  https://pola-rs.
-00001900: 6769 7468 7562 2e69 6f2f 706f 6c61 7273  github.io/polars
-00001910: 2d62 6f6f 6b2f 7573 6572 2d67 7569 6465  -book/user-guide
-00001920: 2f69 6e64 6578 2e68 746d 6c29 0a2a 205b  /index.html).* [
-00001930: 7265 6765 7820 6368 6561 7420 7368 6565  regex cheat shee
-00001940: 745d 2868 7474 7073 3a2f 2f77 7777 2e72  t](https://www.r
-00001950: 6578 6567 672e 636f 6d2f 7265 6765 782d  exegg.com/regex-
-00001960: 7175 6963 6b73 7461 7274 2e68 746d 6c29  quickstart.html)
-00001970: 0a2a 205b 416e 6163 6f6e 6461 2028 7475  .* [Anaconda (tu
-00001980: 746f 7269 616c 7320 6f6e 2070 7974 686f  torials on pytho
-00001990: 6e20 6461 7461 2061 6e61 6c79 7369 7329  n data analysis)
-000019a0: 5d28 6874 7470 733a 2f2f 7777 772e 616e  ](https://www.an
-000019b0: 6163 6f6e 6461 2e63 6f6d 2f6f 7065 6e2d  aconda.com/open-
-000019c0: 736f 7572 6365 290a 2a20 5b54 6865 2050  source).* [The P
-000019d0: 7974 686f 6e20 5475 746f 7269 616c 5d28  ython Tutorial](
-000019e0: 6874 7470 733a 2f2f 646f 6373 2e70 7974  https://docs.pyt
-000019f0: 686f 6e2e 6f72 672f 332f 7475 746f 7269  hon.org/3/tutori
-00001a00: 616c 2f29 0a2a 205b 4a75 7079 7465 7220  al/).* [Jupyter 
-00001a10: 4e6f 7465 626f 6f6b 2069 6e74 726f 6475  Notebook introdu
-00001a20: 6374 696f 6e5d 2868 7474 7073 3a2f 2f72  ction](https://r
-00001a30: 6561 6c70 7974 686f 6e2e 636f 6d2f 6a75  ealpython.com/ju
-00001a40: 7079 7465 722d 6e6f 7465 626f 6f6b 2d69  pyter-notebook-i
-00001a50: 6e74 726f 6475 6374 696f 6e2f 290a       ntroduction/).
+00000c10: 0a20 2072 656e 616d 6520 2020 2020 2020  .  rename       
+00000c20: 2020 2020 2020 2020 5265 6e61 6d65 2063          Rename c
+00000c30: 6173 6573 2069 6e20 696e 7075 7420 6469  ases in input di
+00000c40: 7265 6374 6f72 7920 746f 2063 6173 6520  rectory to case 
+00000c50: 6e75 6d62 6572 730a 2020 7365 7474 696e  numbers.  settin
+00000c60: 6773 2020 2020 2020 2020 2020 2020 2043  gs             C
+00000c70: 7265 6174 6520 616e 6420 6578 706f 7274  reate and export
+00000c80: 2073 6574 7469 6e67 7320 7461 626c 650a   settings table.
+00000c90: 2020 7374 6172 7420 2020 2020 2020 2020    start         
+00000ca0: 2020 2020 2020 204c 6175 6e63 6820 6772         Launch gr
+00000cb0: 6170 6869 6361 6c20 7573 6572 2069 6e74  aphical user int
+00000cc0: 6572 6661 6365 0a20 2074 6162 6c65 2020  erface.  table  
+00000cd0: 2020 2020 2020 2020 2020 2020 2020 4578                Ex
+00000ce0: 706f 7274 2064 6174 6120 7461 626c 6573  port data tables
+00000cf0: 2066 726f 6d20 6172 6368 6976 6520 6f72   from archive or
+00000d00: 2064 6972 6563 746f 7279 0a20 2076 7272   directory.  vrr
+00000d10: 2d70 6169 7273 2020 2020 2020 2020 2020  -pairs          
+00000d20: 2020 4372 6561 7465 2076 6f74 696e 6720    Create voting 
+00000d30: 7269 6768 7473 2073 756d 6d61 7279 2066  rights summary f
+00000d40: 726f 6d20 696e 7075 7420 6361 7365 7320  rom input cases 
+00000d50: 616e 6420 7061 6972 730a 2020 7769 746e  and pairs.  witn
+00000d60: 6573 7365 7320 2020 2020 2020 2020 2020  esses           
+00000d70: 2043 7265 6174 6520 616e 6420 6578 706f   Create and expo
+00000d80: 7274 2077 6974 6e65 7373 6573 2074 6162  rt witnesses tab
+00000d90: 6c65 0a60 6060 0a0a 2323 2046 6574 6368  le.```..## Fetch
+00000da0: 2063 6173 6573 2069 6e20 6275 6c6b 2066   cases in bulk f
+00000db0: 726f 6d20 416c 6163 6f75 7274 2e63 6f6d  rom Alacourt.com
+00000dc0: 200a 0a54 616b 6520 6120 7370 7265 6164   ..Take a spread
+00000dd0: 7368 6565 7420 6f66 206e 616d 6573 2061  sheet of names a
+00000de0: 6e64 2f6f 7220 6f74 6865 7220 7365 6172  nd/or other sear
+00000df0: 6368 2070 6172 616d 6574 6572 7320 616e  ch parameters an
+00000e00: 6420 646f 776e 6c6f 6164 2063 6173 6520  d download case 
+00000e10: 5044 4673 2066 726f 6d20 416c 6163 6f75  PDFs from Alacou
+00000e20: 7274 2069 6e20 6275 6c6b 2e20 446f 776e  rt in bulk. Down
+00000e30: 6c6f 6164 2074 686f 7573 616e 6473 206f  load thousands o
+00000e40: 6620 5044 4673 2069 6e20 6a75 7374 2068  f PDFs in just h
+00000e50: 6f75 7273 2062 7920 6c65 6176 696e 6720  ours by leaving 
+00000e60: 796f 7572 2063 6f6d 7075 7465 7220 756e  your computer un
+00000e70: 6174 7465 6e64 6564 2e20 2847 6f6f 676c  attended. (Googl
+00000e80: 6520 4368 726f 6d65 2069 7320 7265 7175  e Chrome is requ
+00000e90: 6972 6564 2074 6f20 7573 6520 7468 6520  ired to use the 
+00000ea0: 6066 6574 6368 6020 6665 6174 7572 652e  `fetch` feature.
+00000eb0: 290a 0a60 6060 0a55 7361 6765 3a20 7079  )..```.Usage: py
+00000ec0: 7468 6f6e 202d 6d20 616c 6163 6f72 6465  thon -m alacorde
+00000ed0: 7220 6665 7463 6820 5b4f 5054 494f 4e53  r fetch [OPTIONS
+00000ee0: 5d0a 0a20 2046 6574 6368 2063 6173 6573  ]..  Fetch cases
+00000ef0: 2066 726f 6d20 416c 6163 6f75 7274 2e63   from Alacourt.c
+00000f00: 6f6d 0a0a 4f70 7469 6f6e 733a 0a20 202d  om..Options:.  -
+00000f10: 696e 2c20 2d2d 696e 7075 742d 7061 7468  in, --input-path
+00000f20: 2050 4154 4820 2020 2050 6174 6820 746f   PATH    Path to
+00000f30: 2071 7565 7279 2074 6162 6c65 2f73 7072   query table/spr
+00000f40: 6561 6473 6865 6574 2028 2e78 6c73 2c20  eadsheet (.xls, 
+00000f50: 2e78 6c73 7829 0a20 2020 2020 2020 2020  .xlsx).         
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 205b 7265 7175 6972 6564 5d0a 2020     [required].  
+00000f80: 2d6f 7574 2c20 2d2d 6f75 7470 7574 2d70  -out, --output-p
+00000f90: 6174 6820 5041 5448 2020 4465 7369 7265  ath PATH  Desire
+00000fa0: 6420 5044 4620 6f75 7470 7574 2064 6972  d PDF output dir
+00000fb0: 6563 746f 7279 2020 5b72 6571 7569 7265  ectory  [require
+00000fc0: 645d 0a20 202d 632c 202d 2d63 7573 746f  d].  -c, --custo
+00000fd0: 6d65 722d 6964 2054 4558 5420 2020 2043  mer-id TEXT    C
+00000fe0: 7573 746f 6d65 7220 4944 206f 6e20 416c  ustomer ID on Al
+00000ff0: 6163 6f75 7274 2e63 6f6d 2020 5b72 6571  acourt.com  [req
+00001000: 7569 7265 645d 0a20 202d 752c 202d 2d75  uired].  -u, --u
+00001010: 7365 722d 6964 2054 4558 5420 2020 2020  ser-id TEXT     
+00001020: 2020 2055 7365 7220 4944 206f 6e20 416c     User ID on Al
+00001030: 6163 6f75 7274 2e63 6f6d 2020 5b72 6571  acourt.com  [req
+00001040: 7569 7265 645d 0a20 202d 702c 202d 2d70  uired].  -p, --p
+00001050: 6173 7377 6f72 6420 5445 5854 2020 2020  assword TEXT    
+00001060: 2020 2050 6173 7377 6f72 6420 6f6e 2041     Password on A
+00001070: 6c61 636f 7572 742e 636f 6d20 205b 7265  lacourt.com  [re
+00001080: 7175 6972 6564 5d0a 2020 2d6d 6178 2c20  quired].  -max, 
+00001090: 2d2d 6d61 7820 494e 5445 4745 5220 2020  --max INTEGER   
+000010a0: 2020 2020 4d61 7869 6d75 6d20 7175 6572      Maximum quer
+000010b0: 6965 7320 746f 2063 6f6e 6475 6374 206f  ies to conduct o
+000010c0: 6e20 416c 6163 6f75 7274 2e63 6f6d 0a20  n Alacourt.com. 
+000010d0: 202d 736b 6970 2c20 2d2d 736b 6970 2049   -skip, --skip I
+000010e0: 4e54 4547 4552 2020 2020 2053 6b69 7020  NTEGER     Skip 
+000010f0: 656e 7472 6965 7320 6174 2074 6f70 206f  entries at top o
+00001100: 6620 7175 6572 7920 6669 6c65 0a20 202d  f query file.  -
+00001110: 6e2c 202d 2d6e 6f2d 6d61 726b 2020 2020  n, --no-mark    
+00001120: 2020 2020 2020 2020 2044 6f20 6e6f 7420           Do not 
+00001130: 7570 6461 7465 2071 7565 7279 2074 656d  update query tem
+00001140: 706c 6174 6520 6166 7465 7220 636f 6d70  plate after comp
+00001150: 6c65 7469 6f6e 0a20 202d 2d64 6562 7567  letion.  --debug
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 2050 7269 6e74 2064 6574 6169 6c65     Print detaile
+00001180: 6420 7275 6e74 696d 6520 696e 666f 726d  d runtime inform
+00001190: 6174 696f 6e20 746f 2063 6f6e 736f 6c65  ation to console
+000011a0: 0a20 202d 682c 202d 2d68 656c 7020 2020  .  -h, --help   
+000011b0: 2020 2020 2020 2020 2020 2020 2053 686f               Sho
+000011c0: 7720 7468 6973 206d 6573 7361 6765 2061  w this message a
+000011d0: 6e64 2065 7869 742e 0a60 6060 0a0a 0a23  nd exit..```...#
+000011e0: 202a 2a57 6f72 6b69 6e67 2077 6974 6820   **Working with 
+000011f0: 6361 7365 2064 6174 6120 696e 2050 7974  case data in Pyt
+00001200: 686f 6e2a 2a0a 0a0a 2323 2320 4f75 7420  hon**...### Out 
+00001210: 6f66 2074 6865 2062 6f78 2c20 416c 6163  of the box, Alac
+00001220: 6f72 6465 7220 6578 706f 7274 7320 746f  order exports to
+00001230: 2060 2e78 6c73 7860 2c20 602e 786c 7360   `.xlsx`, `.xls`
+00001240: 2c20 602e 6373 7660 2c20 602e 6a73 6f6e  , `.csv`, `.json
+00001250: 602c 2061 6e64 2060 2e70 6172 7175 6574  `, and `.parquet
+00001260: 602e 2042 7574 2079 6f75 2063 616e 2075  `. But you can u
+00001270: 7365 2060 706f 6c61 7273 6020 616e 6420  se `polars` and 
+00001280: 6f74 6865 7220 7079 7468 6f6e 206c 6962  other python lib
+00001290: 7261 7269 6573 2074 6f20 6372 6561 7465  raries to create
+000012a0: 2079 6f75 7220 6f77 6e20 6461 7461 2063   your own data c
+000012b0: 6f6c 6c65 6374 696f 6e20 776f 726b 666c  ollection workfl
+000012c0: 6f77 7320 616e 6420 6375 7374 6f6d 697a  ows and customiz
+000012d0: 6520 416c 6163 6f72 6465 7220 6578 706f  e Alacorder expo
+000012e0: 7274 732e 200a 0a2a 2a2a 5468 6520 736e  rts. ..***The sn
+000012f0: 6970 7065 7420 6265 6c6f 7720 7072 696e  ippet below prin
+00001300: 7473 2074 6865 2066 6565 2073 6865 6574  ts the fee sheet
+00001310: 7320 6672 6f6d 2061 2064 6972 6563 746f  s from a directo
+00001320: 7279 206f 6620 6361 7365 2050 4446 7320  ry of case PDFs 
+00001330: 6173 2069 7420 7265 6164 7320 7468 656d  as it reads them
+00001340: 2e2a 2a2a 0a0a 0a60 6060 7079 7468 6f6e  .***...```python
+00001350: 0a66 726f 6d20 616c 6163 6f72 6465 7220  .from alacorder 
+00001360: 696d 706f 7274 2061 6c61 630a 696d 706f  import alac.impo
+00001370: 7274 2070 6f6c 6172 7320 6173 2070 6c0a  rt polars as pl.
+00001380: 0a71 7565 7565 203d 2061 6c61 632e 6765  .queue = alac.ge
+00001390: 745f 7061 7468 7328 222f 5573 6572 732f  t_paths("/Users/
+000013a0: 6372 696d 736f 6e2f 4465 736b 746f 702f  crimson/Desktop/
+000013b0: 5475 7477 696c 6572 2f22 2920 2320 2d3e  Tutwiler/") # ->
+000013c0: 205b 7374 725d 0a0a 726f 7773 203d 205b   [str]..rows = [
+000013d0: 5d0a 0a66 6f72 2069 2c20 7061 7468 2069  ]..for i, path i
+000013e0: 6e20 656e 756d 6572 6174 6528 7175 6575  n enumerate(queu
+000013f0: 6529 3a0a 2020 2020 7465 7874 203d 2061  e):.    text = a
+00001400: 6c61 632e 6578 7472 6163 745f 7465 7874  lac.extract_text
+00001410: 2870 6174 6829 0a20 2020 2063 6e75 6d20  (path).    cnum 
+00001420: 3d20 616c 6163 2e67 6574 4361 7365 4e75  = alac.getCaseNu
+00001430: 6d62 6572 2874 6578 7429 0a20 2020 2063  mber(text).    c
+00001440: 7479 203d 2061 6c61 632e 6765 7443 6f75  ty = alac.getCou
+00001450: 6e74 7928 7465 7874 290a 2020 2020 7462  nty(text).    tb
+00001460: 616c 203d 2061 6c61 632e 6765 7454 6f74  al = alac.getTot
+00001470: 616c 4261 6c61 6e63 6528 7465 7874 290a  alBalance(text).
+00001480: 2020 2020 7074 7220 3d20 616c 6163 2e67      ptr = alac.g
+00001490: 6574 5061 796d 656e 7454 6f52 6573 746f  etPaymentToResto
+000014a0: 7265 2874 6578 7429 2023 2069 2e65 2e20  re(text) # i.e. 
+000014b0: 766f 7469 6e67 2072 6967 6874 730a 2020  voting rights.  
+000014c0: 2020 726f 7773 202b 3d20 5b5b 636e 756d    rows += [[cnum
+000014d0: 2c20 6374 792c 2074 6261 6c2c 2070 7472  , cty, tbal, ptr
+000014e0: 5d5d 0a0a 6361 7365 7320 3d20 706c 2e44  ]]..cases = pl.D
+000014f0: 6174 6146 7261 6d65 2872 6f77 7329 0a0a  ataFrame(rows)..
+00001500: 6361 7365 732e 7772 6974 655f 6578 6365  cases.write_exce
+00001510: 6c28 222f 5573 6572 732f 6372 696d 736f  l("/Users/crimso
+00001520: 6e2f 4465 736b 746f 702f 5475 7477 696c  n/Desktop/Tutwil
+00001530: 6572 2f73 756d 6d61 7279 2e78 6c73 7822  er/summary.xlsx"
+00001540: 290a 0a60 6060 0a0a 2323 2045 7874 656e  )..```..## Exten
+00001550: 6469 6e67 2041 6c61 636f 7264 6572 2077  ding Alacorder w
+00001560: 6974 6820 6070 6f6c 6172 7360 2061 6e64  ith `polars` and
+00001570: 206f 7468 6572 2074 6f6f 6c73 0a0a 416c   other tools..Al
+00001580: 6163 6f72 6465 7220 7275 6e73 206f 6e20  acorder runs on 
+00001590: 5b60 706f 6c61 7273 605d 2868 7474 7073  [`polars`](https
+000015a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 706f  ://github.com/po
+000015b0: 6c61 2d72 732f 706f 6c61 7273 292c 2061  la-rs/polars), a
+000015c0: 2070 7974 686f 6e20 6c69 6272 6172 7920   python library 
+000015d0: 796f 7520 6361 6e20 7573 6520 746f 2077  you can use to w
+000015e0: 6f72 6b20 7769 7468 2061 6e64 2061 6e61  ork with and ana
+000015f0: 6c79 7a65 2074 6162 756c 6172 2064 6174  lyze tabular dat
+00001600: 612e 2060 706f 6c61 7273 6020 6361 6e20  a. `polars` can 
+00001610: 7265 6164 2066 726f 6d20 616e 6420 7772  read from and wr
+00001620: 6974 6520 746f 2061 6c6c 206d 616a 6f72  ite to all major
+00001630: 2064 6174 6120 7374 6f72 6167 6520 666f   data storage fo
+00001640: 726d 6174 732e 2049 7420 6361 6e20 636f  rmats. It can co
+00001650: 6e6e 6563 7420 746f 2061 2077 6964 6520  nnect to a wide 
+00001660: 7661 7269 6574 7920 6f66 2073 6572 7669  variety of servi
+00001670: 6365 7320 746f 2070 726f 7669 6465 2066  ces to provide f
+00001680: 6f72 2065 6173 7920 696d 706f 7274 2061  or easy import a
+00001690: 6e64 2065 7870 6f72 742e 0a0a 6060 6070  nd export...```p
+000016a0: 7974 686f 6e0a 696d 706f 7274 2070 6f6c  ython.import pol
+000016b0: 6172 7320 6173 2070 6c0a 636f 6e74 656e  ars as pl.conten
+000016c0: 7473 203d 2070 6c2e 7265 6164 5f6a 736f  ts = pl.read_jso
+000016d0: 6e28 222f 7061 7468 2f74 6f2f 6172 6368  n("/path/to/arch
+000016e0: 6976 652e 6a73 6f6e 2229 0a60 6060 0a0a  ive.json").```..
+000016f0: 4966 2079 6f75 2077 6f75 6c64 206c 696b  If you would lik
+00001700: 6520 746f 2076 6973 7561 6c69 7a65 2064  e to visualize d
+00001710: 6174 6120 7769 7468 6f75 7420 6578 706f  ata without expo
+00001720: 7274 696e 6720 746f 2045 7863 656c 206f  rting to Excel o
+00001730: 7220 616e 6f74 6865 7220 666f 726d 6174  r another format
+00001740: 2c20 6372 6561 7465 2061 2060 6a75 7079  , create a `jupy
+00001750: 7465 7220 6e6f 7465 626f 6f6b 6020 616e  ter notebook` an
+00001760: 6420 696e 7374 616c 6c20 746f 6f6c 7320  d install tools 
+00001770: 6c69 6b65 2060 6d61 7470 6c6f 746c 6962  like `matplotlib
+00001780: 602c 2060 7461 6275 6c61 7465 602c 2061  `, `tabulate`, a
+00001790: 6e64 2060 6974 6162 6c65 7360 2074 6f20  nd `itables` to 
+000017a0: 6765 7420 7374 6172 7465 642e 205b 4a75  get started. [Ju
+000017b0: 7079 7465 7220 4e6f 7465 626f 6f6b 5d28  pyter Notebook](
+000017c0: 6874 7470 733a 2f2f 646f 6373 2e6a 7570  https://docs.jup
+000017d0: 7974 6572 2e6f 7267 2f65 6e2f 6c61 7465  yter.org/en/late
+000017e0: 7374 2f73 7461 7274 2f69 6e64 6578 2e68  st/start/index.h
+000017f0: 746d 6c29 2069 7320 6120 5079 7468 6f6e  tml) is a Python
+00001800: 2070 726f 6a65 6374 2079 6f75 2063 616e   project you can
+00001810: 2075 7365 2074 6f20 6372 6561 7465 2069   use to create i
+00001820: 6e74 6572 6163 7469 7665 206e 6f74 6562  nteractive noteb
+00001830: 6f6f 6b73 2066 6f72 2064 6174 6120 616e  ooks for data an
+00001840: 616c 7973 6973 2061 6e64 206f 7468 6572  alysis and other
+00001850: 2070 7572 706f 7365 732e 2049 7420 6361   purposes. It ca
+00001860: 6e20 6265 2069 6e73 7461 6c6c 6564 2075  n be installed u
+00001870: 7369 6e67 2060 7069 7020 696e 7374 616c  sing `pip instal
+00001880: 6c20 6a75 7079 7465 7260 206f 7220 6070  l jupyter` or `p
+00001890: 6970 3320 696e 7374 616c 6c20 6a75 7079  ip3 install jupy
+000018a0: 7465 7260 2061 6e64 206c 6175 6e63 6865  ter` and launche
+000018b0: 6420 7573 696e 6720 606a 7570 7974 6572  d using `jupyter
+000018c0: 206e 6f74 6562 6f6f 6b60 2e20 596f 7572   notebook`. Your
+000018d0: 2064 6576 6963 6520 6d61 7920 616c 7265   device may alre
+000018e0: 6164 7920 6265 2065 7175 6970 7065 6420  ady be equipped 
+000018f0: 746f 2076 6965 7720 602e 6970 796e 6260  to view `.ipynb`
+00001900: 206e 6f74 6562 6f6f 6b73 2e20 0a0a 2323   notebooks. ..##
+00001910: 202a 2a52 6573 6f75 7263 6573 2a2a 0a2a   **Resources**.*
+00001920: 205b 6070 6f6c 6172 7360 2075 7365 7220   [`polars` user 
+00001930: 6775 6964 655d 2868 7474 7073 3a2f 2f70  guide](https://p
+00001940: 6f6c 612d 7273 2e67 6974 6875 622e 696f  ola-rs.github.io
+00001950: 2f70 6f6c 6172 732d 626f 6f6b 2f75 7365  /polars-book/use
+00001960: 722d 6775 6964 652f 696e 6465 782e 6874  r-guide/index.ht
+00001970: 6d6c 290a 2a20 5b72 6567 6578 2063 6865  ml).* [regex che
+00001980: 6174 2073 6865 6574 5d28 6874 7470 733a  at sheet](https:
+00001990: 2f2f 7777 772e 7265 7865 6767 2e63 6f6d  //www.rexegg.com
+000019a0: 2f72 6567 6578 2d71 7569 636b 7374 6172  /regex-quickstar
+000019b0: 742e 6874 6d6c 290a 2a20 5b41 6e61 636f  t.html).* [Anaco
+000019c0: 6e64 6120 2874 7574 6f72 6961 6c73 206f  nda (tutorials o
+000019d0: 6e20 7079 7468 6f6e 2064 6174 6120 616e  n python data an
+000019e0: 616c 7973 6973 295d 2868 7474 7073 3a2f  alysis)](https:/
+000019f0: 2f77 7777 2e61 6e61 636f 6e64 612e 636f  /www.anaconda.co
+00001a00: 6d2f 6f70 656e 2d73 6f75 7263 6529 0a2a  m/open-source).*
+00001a10: 205b 5468 6520 5079 7468 6f6e 2054 7574   [The Python Tut
+00001a20: 6f72 6961 6c5d 2868 7474 7073 3a2f 2f64  orial](https://d
+00001a30: 6f63 732e 7079 7468 6f6e 2e6f 7267 2f33  ocs.python.org/3
+00001a40: 2f74 7574 6f72 6961 6c2f 290a 2a20 5b4a  /tutorial/).* [J
+00001a50: 7570 7974 6572 204e 6f74 6562 6f6f 6b20  upyter Notebook 
+00001a60: 696e 7472 6f64 7563 7469 6f6e 5d28 6874  introduction](ht
+00001a70: 7470 733a 2f2f 7265 616c 7079 7468 6f6e  tps://realpython
+00001a80: 2e63 6f6d 2f6a 7570 7974 6572 2d6e 6f74  .com/jupyter-not
+00001a90: 6562 6f6f 6b2d 696e 7472 6f64 7563 7469  ebook-introducti
+00001aa0: 6f6e 2f29 0a                             on/).
```

### Comparing `alacorder-80.0.4/pyproject.toml` & `alacorder-80.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.0.4"
+version = "80.0.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.0.4/src/alacorder/.DS_Store` & `alacorder-80.0.5/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.4/src/alacorder/__init__.py` & `alacorder-80.0.5/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.0.4/src/alacorder/__main__.py` & `alacorder-80.0.5/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.4"
+version = "80.0.5"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3663,16 +3663,16 @@
         ],
         [
             sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
             sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
             sg.Radio("Financial History", "TABLE", key="TB-HISTORY", default=False),
         ],
         [
-            sg.Radio("Disposition", "TABLE", key="TB-DISPOSITION", default=False),
-            sg.Radio("Filing", "TABLE", key="TB-FILING", default=False),
+            sg.Radio("Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False),
+            sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
```

### Comparing `alacorder-80.0.4/src/alacorder/alac.py` & `alacorder-80.0.5/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Dependencies: python 3.9+, brotli 1.0.9, click 8.1.3, polars 0.17.6, PyMuPDF 1.21.1, PySimpleGUI 4.60.4, selenium 4.8.3, tqdm 4.65.0, xlsx2csv 0.8.1, XlsxWriter 3.0.9
 
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.0.4"
+version = "80.0.5"
 
 autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -3663,16 +3663,16 @@
         ],
         [
             sg.Radio("Attorneys", "TABLE", key="TB-ATTORNEYS", default=False),
             sg.Radio("Settings", "TABLE", key="TB-SETTINGS", default=False),
             sg.Radio("Financial History", "TABLE", key="TB-HISTORY", default=False),
         ],
         [
-            sg.Radio("Disposition", "TABLE", key="TB-DISPOSITION", default=False),
-            sg.Radio("Filing", "TABLE", key="TB-FILING", default=False),
+            sg.Radio("Disposition Charges", "TABLE", key="TB-DISPOSITION", default=False),
+            sg.Radio("Filing Charges", "TABLE", key="TB-FILING", default=False),
         ],
         [
             sg.Text("Max cases: "),
             sg.Input(key="TB-COUNT", default_text="0", size=[5, 1]),
             sg.Checkbox("Allow Overwrite", key="TB-OVERWRITE", default=True),
         ],
         [
```

### Comparing `alacorder-80.0.4/PKG-INFO` & `alacorder-80.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.0.4
+Version: 80.0.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -74,14 +74,15 @@
   conv-pairs           Create convictions summary from input cases and pairs
   fees                 Create and export fees table
   fetch                Fetch cases from Alacourt.com
   financial-history    Create and export financial history table
   images               Create and export images table
   multi                Export all data tables to .xls/.xlsx
   pair                 Create blank AIS / unique pairing template
+  rename               Rename cases in input directory to case numbers
   settings             Create and export settings table
   start                Launch graphical user interface
   table                Export data tables from archive or directory
   vrr-pairs            Create voting rights summary from input cases and pairs
   witnesses            Create and export witnesses table
 ```
```

