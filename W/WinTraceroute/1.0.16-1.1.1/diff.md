# Comparing `tmp/WinTraceroute-1.0.16.tar.gz` & `tmp/WinTraceroute-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.0.16.tar", last modified: Sat Apr 29 11:11:22 2023, max compression
+gzip compressed data, was "WinTraceroute-1.1.1.tar", last modified: Sat Apr 29 12:58:04 2023, max compression
```

## Comparing `WinTraceroute-1.0.16.tar` & `WinTraceroute-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/WinTraceroute.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/traceroute/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/traceroute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/traceroute/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:58:04.832564 WinTraceroute-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-29 12:57:37.000000 WinTraceroute-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-29 12:58:04.832564 WinTraceroute-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-04-29 12:57:37.000000 WinTraceroute-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:58:04.832564 WinTraceroute-1.1.1/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21345 2023-04-29 12:58:04.000000 WinTraceroute-1.1.1/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-29 12:58:04.000000 WinTraceroute-1.1.1/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:58:04.000000 WinTraceroute-1.1.1/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 12:58:04.000000 WinTraceroute-1.1.1/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 12:58:04.000000 WinTraceroute-1.1.1/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 12:58:04.000000 WinTraceroute-1.1.1/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-29 12:57:37.000000 WinTraceroute-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 12:58:04.832564 WinTraceroute-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:58:04.832564 WinTraceroute-1.1.1/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:57:37.000000 WinTraceroute-1.1.1/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-29 12:57:37.000000 WinTraceroute-1.1.1/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-04-29 12:57:37.000000 WinTraceroute-1.1.1/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.0.16/pyproject.toml` & `WinTraceroute-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.0.16"
+version = "1.1.1"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
@@ -24,24 +24,24 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.0.16"
+current_version = "1.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
-#[tool.setuptools.dynamic]
-#readme = {file = ["README.md"]}
+[tool.setuptools.dynamic]
+readme = {file = ["README.md"]}
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
```

### Comparing `WinTraceroute-1.0.16/traceroute/__main__.py` & `WinTraceroute-1.1.1/traceroute/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from signal import signal, SIGINT, SIGKILL, SIGABRT, SIGTERM
+from sys import exit
 import argparse
 from traceroute.traceroute import trace_udp, trace_icmp
 
 
 def main() -> int:
     import logging
     logging.getLogger("scapy").setLevel(logging.WARNING)
@@ -83,8 +85,23 @@
                 timeout=int(args.timeout),
                 port=int(args.port),
                 source=args.source)
         case _:
             print('Module ' + args.module + ' is not supported.')
 
 
-main()
+def term_handler(signal_received, frame) -> None:
+    print()
+    print("-- Cancelled by signal " + str(signal_received) + ".")
+    exit(-1)
+
+try:
+    # this only works on *nix
+    signal(SIGINT, term_handler)
+    #signal(SIGKILL, term_handler)
+    #signal(SIGABRT, term_handler)
+    #signal(SIGTERM, term_handler)
+except ImportError:
+    pass
+
+if __name__ == '__main__':
+    main()
```

### Comparing `WinTraceroute-1.0.16/traceroute/traceroute.py` & `WinTraceroute-1.1.1/traceroute/traceroute.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import sys, math
 from typing import Callable, Any
 from abc import ABC, abstractmethod
 from scapy.plist import SndRcvList, PacketList
 from scapy.all import IP, UDP, ICMP, sr1
 
 
+PRINT_FILE = sys.stdout
+
+
 def trace(host:str,
           IP_PACKET_SUPPLIER=Callable[[str,str,int],Any],
           DATAGRAM_SUPPLIER=Callable[[int],Any],
           min_ttl:int=1,
           max_ttl:int=30,
           num_per_fleet:int=3,
           timeout:int=5,
@@ -25,15 +28,16 @@
     times = list()
     dest_reached = False
     for ttl in range(min_ttl, max_ttl+1):
         # this is for each ttl
         ttl_responses = list()
         ttl_times = list()
         # print ttl index
-        print(' ', f_ttl_str_format.format(ttl), "\t",  sep='', end='')
+        print(' ', f_ttl_str_format.format(ttl), "\t",  sep='', end='', \
+                file=PRINT_FILE)
         for _ in range(num_per_fleet):
             # this is for each packet in the fleet (3 by default)
             packet = IP_PACKET_SUPPLIER(host, source, ttl) / \
                      DATAGRAM_SUPPLIER(port)
             response = sr1(packet, timeout=timeout, verbose=False)
             if response:
                 ttl_responses.append(response)
@@ -113,50 +117,53 @@
             sorted_responses[response_source].append(i)
         else:
             sorted_responses[response_source] = [i]
     # now print results
     is_first_line = True
     for host in sorted_responses.keys():
         if is_first_line:
-            print(firstline_pfx, end='')
+            print(firstline_pfx, end='', file=PRINT_FILE)
         else:
-            print(restlines_pfx, end='')
+            print(restlines_pfx, end='', file=PRINT_FILE)
         indices = sorted_responses[host]
         for i in range(0, fleetsize):
             if i in indices:
                 time = times[i]
                 if time == None:
-                    print(' '*(time_str_width-4) + '*   ' + '\t', end='')
+                    print(' '*(time_str_width-4) + '*   ' + '\t', end='', file=PRINT_FILE)
                 else:
-                    print(time_str_format.format(time) + '\t', end='')
+                    print(time_str_format.format(time) + '\t', end='', file=PRINT_FILE)
             else:
-                print(' '*time_str_width + '\t', end='')
-        print(host)
+                print(' '*time_str_width + '\t', end='', file=PRINT_FILE)
+        print(host, file=PRINT_FILE)
         is_first_line = False
 
 def is_dest_reached(responses:list[tuple[SndRcvList,PacketList]], dest):
     for rt in responses:
         if rt == None:
             continue
         else:
             rt_icmp = rt[ICMP]
             if rt_icmp.type == 3 or rt.src == dest:
                 return True  # Dest unreachable, port unavailable
     return False
 
 def summarize_termination(host, times, ttl, dest_reached):
-    print()
+    print(file=PRINT_FILE)
     if dest_reached:
         print("Destination '" + host + "' reached " + \
             " in RTT " + summarize_times(times, as_string=True) + " ms " + \
-            " via " + str(ttl) + " hops.")
+            " via " + str(ttl) + " hops.", \
+            file=PRINT_FILE)
     else:
-        print("Maximum TTL reached, but no '" + host + "' in sight. Aborting.")
+        print("Maximum TTL reached, but no '" + host + "' in sight. Aborting.", \
+            file=PRINT_FILE)
         print("If you wish to continue the search, consider increasing the `--maxttl`\n" + \
-            "  setting on the next try. Besides that, try a different `--module`, maybe?")
+            "  setting on the next try. Besides that, try a different `--module`, maybe?", \
+            file=PRINT_FILE)
 
 def summarize_times(times:list,
                     as_string:bool=False):
     min = times[0]
     max = times[0]
     sum = times[0]
```

