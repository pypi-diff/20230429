# Comparing `tmp/awc_cli-1.0.2-py2.py3-none-any.whl.zip` & `tmp/awc_cli-1.0.3-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 21726 bytes, number of entries: 18
--rw-r--r--  2.0 unx      122 b- defN 23-Apr-16 00:41 awc_cli/__init__.py
+Zip file size: 21827 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      122 b- defN 23-Apr-29 18:40 awc_cli/__init__.py
 -rw-r--r--  2.0 unx      508 b- defN 23-Apr-15 23:24 awc_cli/__main__.py
 -rw-r--r--  2.0 unx      423 b- defN 23-Apr-15 23:09 awc_cli/config.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 17:08 awc_cli/py.typed
--rw-r--r--  2.0 unx     2506 b- defN 23-Apr-15 22:20 awc_cli/repl.py
+-rw-r--r--  2.0 unx     2799 b- defN 23-Apr-29 18:40 awc_cli/repl.py
 -rw-r--r--  2.0 unx     1790 b- defN 23-Apr-15 23:14 awc_cli/util.py
 -rw-r--r--  2.0 unx      490 b- defN 23-Apr-15 21:10 awc_cli/cmd/__init__.py
 -rw-r--r--  2.0 unx     4004 b- defN 23-Apr-16 00:42 awc_cli/cmd/admin_cmds.py
 -rw-r--r--  2.0 unx      290 b- defN 23-Apr-15 23:23 awc_cli/cmd/cmds.py
 -rw-r--r--  2.0 unx     3326 b- defN 23-Apr-15 23:23 awc_cli/cmd/mgr.py
 -rw-r--r--  2.0 unx     2335 b- defN 23-Apr-15 23:15 awc_cli/cmd/user_cmds.py
--rw-------  2.0 unx    35115 b- defN 23-Apr-16 00:43 awc_cli-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1092 b- defN 23-Apr-16 00:43 awc_cli-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-16 00:43 awc_cli-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-16 00:43 awc_cli-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-16 00:43 awc_cli-1.0.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.0.2.dist-info/zip-safe
--rw-rw-r--  2.0 unx     1397 b- defN 23-Apr-16 00:43 awc_cli-1.0.2.dist-info/RECORD
-18 files, 53563 bytes uncompressed, 19454 bytes compressed:  63.7%
+-rw-------  2.0 unx    35115 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1092 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-15 23:07 awc_cli-1.0.3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     1397 b- defN 23-Apr-29 18:41 awc_cli-1.0.3.dist-info/RECORD
+18 files, 53856 bytes uncompressed, 19555 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -27,29 +27,29 @@
 
 Filename: awc_cli/cmd/mgr.py
 Comment: 
 
 Filename: awc_cli/cmd/user_cmds.py
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/LICENSE
+Filename: awc_cli-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/METADATA
+Filename: awc_cli-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/WHEEL
+Filename: awc_cli-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/entry_points.txt
+Filename: awc_cli-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/top_level.txt
+Filename: awc_cli-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/zip-safe
+Filename: awc_cli-1.0.3.dist-info/zip-safe
 Comment: 
 
-Filename: awc_cli-1.0.2.dist-info/RECORD
+Filename: awc_cli-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## awc_cli/__init__.py

```diff
@@ -1,7 +1,7 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """awc_cli"""
 
 from typing import Final
 
-__version__: Final[str] = "1.0.2"
+__version__: Final[str] = "1.0.3"
```

## awc_cli/repl.py

```diff
@@ -35,47 +35,25 @@
         msg = f"resource not found : {e.value!r}"
     except Exception as e:
         msg = f"{e.__class__.__name__} -- {e}"
     finally:
         return 0 if msg is None else err(msg)
 
 
-def repl(api: awc.Awc) -> int:
-    """the repl main"""
-
-    last: int = 0
-    user: typing.Optional[str]
+def repl_shell(user: str, api: awc.Awc) -> int:
+    """main repl shell"""
 
     try:
         import readline
 
         del readline
     except Exception:
         pass
 
-    try:
-        user = awc.api.whoami(api)
-    except awc.exc.APIRequestFailedError:
-        if awc.api.applied(api):
-            if (user := accept_application(api)) is None:
-                return err("please wait for your application to get accepted")
-        else:
-            print("please apply")
-
-            try:
-                awc.api.apply(
-                    api,
-                    (user := awc_input("username")),
-                    awc_input("why do you want to apply"),
-                )
-            except EOFError:
-                return 2
-
-            if accept_application(api, user) is None:
-                return err("cannot accept your application, wait for your acceptance")
+    last: int = 0
 
     print("type `help` for help, press CTRL + D or type `.exit` to exit")
 
     while True:
         try:
             print()
             cmd: Command = Command(
@@ -90,7 +68,40 @@
         if (cfn := CMGR.get((cname := cmd.next()))) is None:
             last = err(f"{cname} -- command not found")
             continue
 
         last = run_cmd_fn(cfn, api, cmd)
 
     return last
+
+
+def repl(api: awc.Awc) -> int:
+    """the repl main"""
+
+    user: typing.Optional[str]
+
+    try:
+        user = awc.api.whoami(api)
+    except awc.exc.APIRequestFailedError:
+        if awc_input("do you want to apply [Y/n]").lower().startswith("n"):
+            print("not applying, some functions might not work")
+            return repl_shell("#", api)
+
+        if awc.api.applied(api):
+            if (user := accept_application(api)) is None:
+                return err("please wait for your application to get accepted")
+        else:
+            print("please apply")
+
+            try:
+                awc.api.apply(
+                    api,
+                    (user := awc_input("username")),
+                    awc_input("why do you want to apply"),
+                )
+            except EOFError:
+                return 2
+
+            if accept_application(api, user) is None:
+                return err("cannot accept your application, wait for your acceptance")
+
+    return repl_shell(user, api)
```

## Comparing `awc_cli-1.0.2.dist-info/LICENSE` & `awc_cli-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `awc_cli-1.0.2.dist-info/METADATA` & `awc_cli-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awc-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: cli for https://server.ari-web.xyz/
 Home-page: https://ari-web.xyz/gh/awc-cli
 Author: Ari Archer
 Author-email: ari.web.xyz@gmail.com
 License: GPLv3+
 Keywords: http,comments,api,https,awc
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `awc_cli-1.0.2.dist-info/RECORD` & `awc_cli-1.0.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-awc_cli/__init__.py,sha256=gfy2ZX_BeITlFYWLbr1r3Ade9yM4cqQ2onQDrsT5h1s,122
+awc_cli/__init__.py,sha256=EFfETku-Xl2gUIrozi9FooRnx9-4fqxw-1vyPvoxx74,122
 awc_cli/__main__.py,sha256=4yHZMkIHuTIIDs61cc1graPrMLDf52djTpUrIydnBHI,508
 awc_cli/config.py,sha256=LOb3rgb14ui92pGUmnk63JEiOoTO3VOxF9xFtvzN-Ic,423
 awc_cli/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-awc_cli/repl.py,sha256=W9u9tFpLX5K2Nw-_DfPyTPglUHzdvLs0DGYriJb6I4o,2506
+awc_cli/repl.py,sha256=PXZZfqVa9x9Y6DTkIcPNqm1cKAWVQA34JMeu99LntP8,2799
 awc_cli/util.py,sha256=vxJ0DwU9Bwk87H4MfgBg7rkhMWd-aO_xskib4Uxq7To,1790
 awc_cli/cmd/__init__.py,sha256=jwBEdqk3lhwYnMuhY8Srkoo__3FYKd3q9DEv8BpEmeA,490
 awc_cli/cmd/admin_cmds.py,sha256=3QifXHPwg0aU_ynpyL2w-0gxpm3EchP4aVjXGx8QH9k,4004
 awc_cli/cmd/cmds.py,sha256=dn2mhqcABK0qrdvNNz5PRQ9F5wNXW52nia2Ju6_n9Cw,290
 awc_cli/cmd/mgr.py,sha256=FUA5hl2UqKqoR6bKYwZCJTRg6_9163Lh3n17Rol2w7E,3326
 awc_cli/cmd/user_cmds.py,sha256=iytxNKB7aui4diTDybPnVUWF4ygltr2clqePR2K8v8A,2335
-awc_cli-1.0.2.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
-awc_cli-1.0.2.dist-info/METADATA,sha256=u7P8uTtAYaUHjOgnNPtFaAnN1E-SlRCKxxmuwSE2AZg,1092
-awc_cli-1.0.2.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-awc_cli-1.0.2.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
-awc_cli-1.0.2.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
-awc_cli-1.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-awc_cli-1.0.2.dist-info/RECORD,,
+awc_cli-1.0.3.dist-info/LICENSE,sha256=oo1Q3PR860k723dU4IFQHEp-dmJy49c3F_OdbhlHj88,35115
+awc_cli-1.0.3.dist-info/METADATA,sha256=WIa_q0qlJW4bSGqO2lzs71eqjvRdxqXkexMCym_80sE,1092
+awc_cli-1.0.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+awc_cli-1.0.3.dist-info/entry_points.txt,sha256=Bpjz7jmU8iLTFkxixEbvx_03RogoHocK_zDoVsGR8R0,46
+awc_cli-1.0.3.dist-info/top_level.txt,sha256=4NIrO2nFlQFYzCa0gD1_twziYc8me452Za3vtcFWans,8
+awc_cli-1.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+awc_cli-1.0.3.dist-info/RECORD,,
```

