# Comparing `tmp/WinTraceroute-1.0.14.tar.gz` & `tmp/WinTraceroute-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WinTraceroute-1.0.14.tar", last modified: Sat Apr 29 09:33:39 2023, max compression
+gzip compressed data, was "WinTraceroute-1.0.16.tar", last modified: Sat Apr 29 11:11:22 2023, max compression
```

## Comparing `WinTraceroute-1.0.14.tar` & `WinTraceroute-1.0.16.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-29 09:33:39.040084 WinTraceroute-1.0.14/
--rwxrwxrwx   0 root         (0) root         (0)      510 2023-04-29 09:33:39.039216 WinTraceroute-1.0.14/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-29 09:33:39.036153 WinTraceroute-1.0.14/WinTraceroute.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      510 2023-04-29 09:33:39.000000 WinTraceroute-1.0.14/WinTraceroute.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      309 2023-04-29 09:33:39.000000 WinTraceroute-1.0.14/WinTraceroute.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-29 09:33:39.000000 WinTraceroute-1.0.14/WinTraceroute.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       59 2023-04-29 09:33:39.000000 WinTraceroute-1.0.14/WinTraceroute.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       57 2023-04-29 09:33:39.000000 WinTraceroute-1.0.14/WinTraceroute.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2023-04-29 09:33:39.000000 WinTraceroute-1.0.14/WinTraceroute.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     1378 2023-04-29 09:29:05.000000 WinTraceroute-1.0.14/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-29 09:33:39.040373 WinTraceroute-1.0.14/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-29 09:33:39.038370 WinTraceroute-1.0.14/traceroute/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-04-20 11:21:37.000000 WinTraceroute-1.0.14/traceroute/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     3697 2023-04-26 13:22:09.000000 WinTraceroute-1.0.14/traceroute/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     7057 2023-04-26 13:21:32.000000 WinTraceroute-1.0.14/traceroute/traceroute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/WinTraceroute.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-29 11:11:22.000000 WinTraceroute-1.0.16/WinTraceroute.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 11:11:22.578688 WinTraceroute-1.0.16/traceroute/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/traceroute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/traceroute/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-29 11:10:50.000000 WinTraceroute-1.0.16/traceroute/traceroute.py
```

### Comparing `WinTraceroute-1.0.14/pyproject.toml` & `WinTraceroute-1.0.16/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel", "bumpver", "scapy==2.5.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "WinTraceroute"
-version = "1.0.14"
+version = "1.0.16"
 description = "A mostly *NIX-traceroute-like -- but very basic -- tracert/traceroute IPv4 alternative built on scapy."
 authors = [{ name = "Nico Rittinghaus", email = "nico@ritti.ng" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta"
@@ -24,15 +24,15 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest", "pyinstaller==5.10.1"]
 
 [project.urls]
 Homepage = "https://github.com/NiRit100/WinTraceroute"
 
 [tool.bumpver]
-current_version = "1.0.14"
+current_version = "1.0.16"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 # (BETA) tells setuptools you will be using a readme file for the long description field for your pypi profile.
```

### Comparing `WinTraceroute-1.0.14/traceroute/__main__.py` & `WinTraceroute-1.0.16/traceroute/__main__.py`

 * *Files identical despite different names*

### Comparing `WinTraceroute-1.0.14/traceroute/traceroute.py` & `WinTraceroute-1.0.16/traceroute/traceroute.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,23 +45,23 @@
             #print(" ###", response)
         # append this ttl's data to the record
         responses.append(ttl_responses)
         times.append(ttl_times)
         # print results
         summarize_ttl(ttl_responses, ttl_times,
                       restlines_pfx=(' '*(f_log10_maxttl+1))+'\t',
-                      time_str_format=f_time_str_format, 
+                      time_str_format=f_time_str_format,
                       time_str_width=f_time_str_width)
         # terminate if destination reached
         if is_dest_reached(ttl_responses, dest=host):
             dest_reached = True
             break
     # end of run -- maybe destination reached, maybe not.
     summarize_termination(host, ttl_times, ttl, dest_reached=dest_reached)
-        
+
     # return the records
     return (responses, times)
 
 def trace_udp(host:str,
               udp_length=2,
               min_ttl:int=1,
               max_ttl:int=30,
@@ -71,33 +71,33 @@
               source:str=None):
     ip_packet_supplier = \
         lambda host, source, ttl: \
             make_ip_packet(host=host, source=source, ttl=ttl)
     datagram_supplier = \
         lambda port: \
             make_udp_packet(port=port) / get_junk(udp_length)
-    trace(host, ip_packet_supplier, datagram_supplier, 
-          min_ttl=min_ttl, max_ttl=max_ttl, num_per_fleet=num_per_fleet, 
+    trace(host, ip_packet_supplier, datagram_supplier,
+          min_ttl=min_ttl, max_ttl=max_ttl, num_per_fleet=num_per_fleet,
           timeout=timeout, port=port, source=source)
-        
+
 def trace_icmp(host:str,
                min_ttl:int=1,
                max_ttl:int=30,
                num_per_fleet:int=3,
                timeout:int=5,
                port:int=33434,
                source:str=None):
     ip_packet_supplier = \
         lambda host, source, ttl: \
             make_ip_packet(host=host, source=source, ttl=ttl)
     datagram_supplier = \
         lambda port: \
             make_icmp_packet()  # ignore port on icmp
-    trace(host, ip_packet_supplier, datagram_supplier, 
-          min_ttl=min_ttl, max_ttl=max_ttl, num_per_fleet=num_per_fleet, 
+    trace(host, ip_packet_supplier, datagram_supplier,
+          min_ttl=min_ttl, max_ttl=max_ttl, num_per_fleet=num_per_fleet,
           timeout=timeout, port=port, source=source)
 
 
 def summarize_ttl(responses:list, times:list,
                   firstline_pfx:str='', restlines_pfx:str='',
                   time_str_format:str='%8.3f',
                   time_str_width:int=8):
@@ -149,37 +149,37 @@
         print("Destination '" + host + "' reached " + \
             " in RTT " + summarize_times(times, as_string=True) + " ms " + \
             " via " + str(ttl) + " hops.")
     else:
         print("Maximum TTL reached, but no '" + host + "' in sight. Aborting.")
         print("If you wish to continue the search, consider increasing the `--maxttl`\n" + \
             "  setting on the next try. Besides that, try a different `--module`, maybe?")
-                
+
 def summarize_times(times:list,
                     as_string:bool=False):
     min = times[0]
     max = times[0]
     sum = times[0]
-    
+
     if len(times) > 1:
         for t in times[1:]:
             if t < min:
                 min = t
             if t > max:
                 max = t
             sum += t
-            
+
     avg = sum / len(times)
-    
+
     if as_string:
-        return "min. %.3f, avg. %.3f, max. %.3f" % (min, avg, max) 
+        return "min. %.3f, avg. %.3f, max. %.3f" % (min, avg, max)
     else:
         return (min, avg, max)
-    
-    
+
+
 def make_ip_packet(host:str, source:str, ttl:int):
     if source != None:
         packet = IP(dst=host, src=source, ttl=ttl)
     else:
         packet = IP(dst=host, ttl=ttl)
     return packet
```

