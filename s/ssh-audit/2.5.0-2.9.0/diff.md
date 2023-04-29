# Comparing `tmp/ssh-audit-2.5.0.tar.gz` & `tmp/ssh-audit-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssh-audit-2.5.0.tar", last modified: Thu Aug 26 19:58:01 2021, max compression
+gzip compressed data, was "ssh-audit-2.9.0.tar", last modified: Sat Apr 29 17:56:54 2023, max compression
```

## Comparing `ssh-audit-2.5.0.tar` & `ssh-audit-2.9.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2021-08-26 19:58:01.641002 ssh-audit-2.5.0/
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1165 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/LICENSE
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    21189 2021-08-26 19:58:01.641002 ssh-audit-2.5.0/PKG-INFO
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    17416 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/README.md
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1302 2021-08-26 19:58:01.641002 ssh-audit-2.5.0/setup.cfg
--rw-rw-r--   0 jdog      (1000) jdog      (1000)      867 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/setup.py
-drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2021-08-26 19:58:01.637002 ssh-audit-2.5.0/src/
-drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2021-08-26 19:58:01.641002 ssh-audit-2.5.0/src/ssh_audit/
--rw-rw-r--   0 jdog      (1000) jdog      (1000)        0 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/__init__.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)      269 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/__main__.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     2550 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/algorithm.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     9894 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/algorithms.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     4540 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/auditconf.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     3619 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/banner.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)      222 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/exitcodes.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1719 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/fingerprint.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     6798 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/gextest.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1383 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/globals.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    10189 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/hostkeytest.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    20095 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/kexdh.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     6784 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/outputbuffer.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    38142 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/policy.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1341 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/product.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1469 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/protocol.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     3326 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/readbuf.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     8949 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/software.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1743 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh1.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1895 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh1_crc32.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     2486 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh1_kexdb.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     5318 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh1_publickeymessage.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     4973 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh2_kex.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    20100 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh2_kexdb.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1919 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh2_kexparty.py
--rwxrwxr-x   0 jdog      (1000) jdog      (1000)    49247 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh_audit.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    14856 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/ssh_socket.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     3450 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/timeframe.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     5446 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/utils.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    13680 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/versionvulnerabilitydb.py
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     3947 2021-08-26 19:57:53.000000 ssh-audit-2.5.0/src/ssh_audit/writebuf.py
-drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2021-08-26 19:58:01.641002 ssh-audit-2.5.0/src/ssh_audit.egg-info/
--rw-rw-r--   0 jdog      (1000) jdog      (1000)    21189 2021-08-26 19:58:01.000000 ssh-audit-2.5.0/src/ssh_audit.egg-info/PKG-INFO
--rw-rw-r--   0 jdog      (1000) jdog      (1000)     1069 2021-08-26 19:58:01.000000 ssh-audit-2.5.0/src/ssh_audit.egg-info/SOURCES.txt
--rw-rw-r--   0 jdog      (1000) jdog      (1000)        1 2021-08-26 19:58:01.000000 ssh-audit-2.5.0/src/ssh_audit.egg-info/dependency_links.txt
--rw-rw-r--   0 jdog      (1000) jdog      (1000)       56 2021-08-26 19:58:01.000000 ssh-audit-2.5.0/src/ssh_audit.egg-info/entry_points.txt
--rw-rw-r--   0 jdog      (1000) jdog      (1000)       10 2021-08-26 19:58:01.000000 ssh-audit-2.5.0/src/ssh_audit.egg-info/top_level.txt
+drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2023-04-29 17:56:54.642218 ssh-audit-2.9.0/
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1165 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/LICENSE
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    23420 2023-04-29 17:56:54.642218 ssh-audit-2.9.0/PKG-INFO
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    22176 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/README.md
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1358 2023-04-29 17:56:54.642218 ssh-audit-2.9.0/setup.cfg
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)      867 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/setup.py
+drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2023-04-29 17:56:54.638218 ssh-audit-2.9.0/src/
+drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2023-04-29 17:56:54.638218 ssh-audit-2.9.0/src/ssh_audit/
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)        0 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/__init__.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)      269 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/__main__.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     2550 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/algorithm.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     9894 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/algorithms.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     4579 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/auditconf.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     3619 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/banner.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)      222 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/exitcodes.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1719 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/fingerprint.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    11149 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/gextest.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1981 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/globals.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    13307 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/hostkeytest.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    22477 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/kexdh.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     6784 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/outputbuffer.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    59702 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/policy.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1341 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/product.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1469 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/protocol.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     3326 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/readbuf.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     8949 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/software.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1743 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh1.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1895 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh1_crc32.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     2486 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh1_kexdb.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     5318 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh1_publickeymessage.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     5438 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh2_kex.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    27028 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh2_kexdb.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1919 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh2_kexparty.py
+-rwxrwxr-x   0 jdog      (1000) jdog      (1000)    62834 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh_audit.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    14884 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/ssh_socket.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     3450 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/timeframe.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     5446 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/utils.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    15843 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/versionvulnerabilitydb.py
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     3947 2023-04-29 17:56:41.000000 ssh-audit-2.9.0/src/ssh_audit/writebuf.py
+drwxrwxr-x   0 jdog      (1000) jdog      (1000)        0 2023-04-29 17:56:54.642218 ssh-audit-2.9.0/src/ssh_audit.egg-info/
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)    23420 2023-04-29 17:56:54.000000 ssh-audit-2.9.0/src/ssh_audit.egg-info/PKG-INFO
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)     1069 2023-04-29 17:56:54.000000 ssh-audit-2.9.0/src/ssh_audit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)        1 2023-04-29 17:56:54.000000 ssh-audit-2.9.0/src/ssh_audit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)       55 2023-04-29 17:56:54.000000 ssh-audit-2.9.0/src/ssh_audit.egg-info/entry_points.txt
+-rw-rw-r--   0 jdog      (1000) jdog      (1000)       10 2023-04-29 17:56:54.000000 ssh-audit-2.9.0/src/ssh_audit.egg-info/top_level.txt
```

### Comparing `ssh-audit-2.5.0/LICENSE` & `ssh-audit-2.9.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (C) 2017-2020 Joe Testa (jtesta@positronsecurity.com)
+Copyright (C) 2017-2023 Joe Testa (jtesta@positronsecurity.com)
 Copyright (C) 2017 Andris Raugulis (moo@arthepsy.eu)
 
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
```

### Comparing `ssh-audit-2.5.0/PKG-INFO` & `ssh-audit-2.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,349 +1,345 @@
-Metadata-Version: 2.1
-Name: ssh-audit
-Version: 2.5.0
-Summary: An SSH server & client configuration security auditing tool
-Home-page: https://github.com/jtesta/ssh-audit
-Author: Joe Testa
-Author-email: jtesta@positronsecurity.com
-License: UNKNOWN
-Project-URL: Source Code, https://github.com/jtesta/ssh-audit
-Project-URL: Bug Tracker, https://github.com/jtesta/ssh-audit/issues
-Description: # ssh-audit
-        [![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/LICENSE)
-        [![PyPI Downloads](https://img.shields.io/pypi/dm/ssh-audit)](https://pypi.org/project/ssh-audit/)
-        [![Docker Pulls](https://img.shields.io/docker/pulls/positronsecurity/ssh-audit)](https://hub.docker.com/r/positronsecurity/ssh-audit)
-        [![Build Status](https://github.com/jtesta/ssh-audit/actions/workflows/tox.yaml/badge.svg)](https://github.com/jtesta/ssh-audit/actions)
-        [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/CONTRIBUTING.md)
-        
-        **ssh-audit** is a tool for ssh server & client configuration auditing.
-        
-        [jtesta/ssh-audit](https://github.com/jtesta/ssh-audit/) (v2.0+) is the updated and maintained version of ssh-audit forked from [arthepsy/ssh-audit](https://github.com/arthepsy/ssh-audit) (v1.x) due to inactivity.
-        
-        - [Features](#features)
-        - [Usage](#usage)
-        - [Screenshots](#screenshots)
-            - [Server Standard Audit Example](#server-standard-audit-example)
-            - [Server Policy Audit Example](#server-policy-audit-example)
-            - [Client Standard Audit Example](#client-standard-audit-example)
-        - [Hardening Guides](#hardening-guides)
-        - [Pre-Built Packages](#pre-built-packages)
-        - [Web Front-End](#web-front-end)
-        - [ChangeLog](#changelog)
-        
-        ## Features
-        - SSH1 and SSH2 protocol server support;
-        - analyze SSH client configuration;
-        - grab banner, recognize device or software and operating system, detect compression;
-        - gather key-exchange, host-key, encryption and message authentication code algorithms;
-        - output algorithm information (available since, removed/disabled, unsafe/weak/legacy, etc);
-        - output algorithm recommendations (append or remove based on recognized software version);
-        - output security information (related issues, assigned CVE list, etc);
-        - analyze SSH version compatibility based on algorithm information;
-        - historical information from OpenSSH, Dropbear SSH and libssh;
-        - policy scans to ensure adherence to a hardened/standard configuration;
-        - runs on Linux and Windows;
-        - supports Python 3.6 - 3.9;
-        - no dependencies
-        
-        ## Usage
-        ```
-        usage: ssh-audit.py [options] <host>
-        
-           -h,  --help             print this help
-           -1,  --ssh1             force ssh version 1 only
-           -2,  --ssh2             force ssh version 2 only
-           -4,  --ipv4             enable IPv4 (order of precedence)
-           -6,  --ipv6             enable IPv6 (order of precedence)
-           -b,  --batch            batch output
-           -c,  --client-audit     starts a server on port 2222 to audit client
-                                       software config (use -p to change port;
-                                       use -t to change timeout)
-           -d,  --debug            Enable debug output.
-           -j,  --json             JSON output (use -jj to enable indents)
-           -l,  --level=<level>    minimum output level (info|warn|fail)
-           -L,  --list-policies    list all the official, built-in policies
-                --lookup=<alg1,alg2,...>    looks up an algorithm(s) without
-                                            connecting to a server
-           -m,  --manual           print the man page (Windows only)
-           -M,  --make-policy=<policy.txt>  creates a policy based on the target server
-                                            (i.e.: the target server has the ideal
-                                            configuration that other servers should
-                                            adhere to)
-           -n,  --no-colors        disable colors
-           -p,  --port=<port>      port to connect
-           -P,  --policy=<"policy name" | policy.txt>  run a policy test using the
-                                                           specified policy
-           -t,  --timeout=<secs>   timeout (in seconds) for connection and reading
-                                       (default: 5)
-           -T,  --targets=<hosts.txt>  a file containing a list of target hosts (one
-                                           per line, format HOST[:PORT])
-                --threads=<threads>    number of threads to use when scanning multiple
-                                           targets (-T/--targets) (default: 32)
-           -v,  --verbose          verbose output
-        ```
-        * if both IPv4 and IPv6 are used, order of precedence can be set by using either `-46` or `-64`.  
-        * batch flag `-b` will output sections without header and without empty lines (implies verbose flag).  
-        * verbose flag `-v` will prefix each line with section type and algorithm name.  
-        * an exit code of 0 is returned when all algorithms are considered secure (for a standard audit), or when a policy check passes (for a policy audit).
-        
-        Basic server auditing:
-        ```
-        ssh-audit localhost
-        ssh-audit 127.0.0.1
-        ssh-audit 127.0.0.1:222
-        ssh-audit ::1
-        ssh-audit [::1]:222
-        ```
-        
-        To run a standard audit against many servers (place targets into servers.txt, one on each line in the format of `HOST[:PORT]`):
-        
-        ```
-        ssh-audit -T servers.txt
-        ```
-        
-        To audit a client configuration (listens on port 2222 by default; connect using `ssh -p 2222 anything@localhost`):
-        
-        ```
-        ssh-audit -c
-        ```
-        
-        To audit a client configuration, with a listener on port 4567:
-        ```
-        ssh-audit -c -p 4567
-        ```
-        
-        To  list all official built-in policies (hint: use resulting policy names with `-P`/`--policy`):
-        ```
-        ssh-audit -L
-        ```
-        
-        To run a policy audit against a server:
-        ```
-        ssh-audit -P ["policy name" | path/to/server_policy.txt] targetserver
-        ```
-        
-        To run a policy audit against a client:
-        ```
-        ssh-audit -c -P ["policy name" | path/to/client_policy.txt]
-        ```
-        
-        To run a policy audit against many servers:
-        ```
-        ssh-audit -T servers.txt -P ["policy name" | path/to/server_policy.txt]
-        ```
-        
-        To create a policy based on a target server (which can be manually edited):
-        ```
-        ssh-audit -M new_policy.txt targetserver
-        ```
-        
-        ## Screenshots
-        
-        ### Server Standard Audit Example
-        Below is a screen shot of the standard server-auditing output when connecting to an unhardened OpenSSH v5.3 service:
-        ![screenshot](https://user-images.githubusercontent.com/2982011/64388792-317e6f80-d00e-11e9-826e-a4934769bb07.png)
-        
-        ### Server Policy Audit Example
-        Below is a screen shot of the policy auditing output when connecting to an un-hardened Ubuntu Server 20.04 machine (hint: use `-L`/`--list-policies` to see names of built-in policies to use with `-P`/`--policy`):
-        ![screenshot](https://user-images.githubusercontent.com/2982011/94370881-95178700-00c0-11eb-8705-3157a4669dc0.png)
-        
-        After applying the steps in the hardening guide (see below), the output changes to the following:
-        ![screenshot](https://user-images.githubusercontent.com/2982011/94370873-87620180-00c0-11eb-9a59-469f61a56ce1.png)
-        
-        ### Client Standard Audit Example
-        Below is a screen shot of the client-auditing output when an unhardened OpenSSH v7.2 client connects:
-        ![client_screenshot](https://user-images.githubusercontent.com/2982011/68867998-b946c100-06c4-11ea-975f-1f47e4178a74.png)
-        
-        ## Hardening Guides
-        Guides to harden server & client configuration can be found here: [https://www.ssh-audit.com/hardening_guides.html](https://www.ssh-audit.com/hardening_guides.html)
-        
-        ## Pre-Built Packages
-        Pre-built packages are available for Windows (see the releases page), on PyPI, Snap, and Homebrew.
-        
-        To install from PyPI:
-        ```
-        $ pip3 install ssh-audit
-        ```
-        
-        To install the Snap package:
-        ```
-        $ snap install ssh-audit
-        ```
-        
-        To install on Homebrew:
-        ```
-        $ brew install ssh-audit
-        ```
-        
-        To install from Dockerhub:
-        ```
-        $ docker pull positronsecurity/ssh-audit
-        ```
-        (Then run with: `docker run -it -p 2222:2222 positronsecurity/ssh-audit 10.1.1.1`)
-        
-        ## Web Front-End
-        For convenience, a web front-end on top of the command-line tool is available at [https://www.ssh-audit.com/](https://www.ssh-audit.com/).
-        
-        ## ChangeLog
-        ### v2.5.0 (2021-08-26)
-         - Fixed crash when running host key tests.
-         - Handles server connection failures more gracefully.
-         - Now prints JSON with indents when `-jj` is used (useful for debugging).
-         - Added MD5 fingerprints to verbose output.
-         - Added `-d`/`--debug` option for getting debugging output; credit [Adam Russell](https://github.com/thecliguy).
-         - Updated JSON output to include MD5 fingerprints.  Note that this results in a breaking change in the 'fingerprints' dictionary format.
-         - Updated OpenSSH 8.1 (and earlier) policies to include `rsa-sha2-512` and `rsa-sha2-256`.
-         - Added OpenSSH v8.6 & v8.7 policies.
-         - Added 3 new key exchanges: `gss-gex-sha1-eipGX3TCiQSrx573bT1o1Q==`, `gss-group1-sha1-eipGX3TCiQSrx573bT1o1Q==`, and `gss-group14-sha1-eipGX3TCiQSrx573bT1o1Q==`.
-         - Added 3 new MACs: `hmac-ripemd160-96`, `AEAD_AES_128_GCM`, and `AEAD_AES_256_GCM`.
-        
-        ### v2.4.0 (2021-02-23)
-         - Added multi-threaded scanning support.
-         - Added built-in Windows manual page (see `-m`/`--manual`); credit [Adam Russell](https://github.com/thecliguy).
-         - Added version check for OpenSSH user enumeration (CVE-2018-15473).
-         - Added deprecation note to host key types based on SHA-1.
-         - Added extra warnings for SSHv1.
-         - Added built-in hardened OpenSSH v8.5 policy.
-         - Upgraded warnings to failures for host key types based on SHA-1.
-         - Fixed crash when receiving unexpected response during host key test.
-         - Fixed hang against older Cisco devices during host key test & gex test.
-         - Fixed improper termination while scanning multiple targets when one target returns an error.
-         - Dropped support for Python 3.5 (which reached EOL in Sept. 2020).
-         - Added 1 new key exchange: `sntrup761x25519-sha512@openssh.com`.
-        
-        ### v2.3.1 (2020-10-28)
-         - Now parses public key sizes for `rsa-sha2-256-cert-v01@openssh.com` and `rsa-sha2-512-cert-v01@openssh.com` host key types.
-         - Flag `ssh-rsa-cert-v01@openssh.com` as a failure due to SHA-1 hash.
-         - Fixed bug in recommendation output which suppressed some algorithms inappropriately.
-         - Built-in policies now include CA key requirements (if certificates are in use).
-         - Lookup function (`--lookup`) now performs case-insensitive lookups of similar algorithms; credit [Adam Russell](https://github.com/thecliguy).
-         - Migrated pre-made policies from external files to internal database.
-         - Split single 3,500 line script into many files (by class).
-         - Added setup.py support; credit [Ganden Schaffner](https://github.com/gschaffner).
-         - Added 1 new cipher: `des-cbc@ssh.com`.
-        
-        ### v2.3.0 (2020-09-27)
-         - Added new policy auditing functionality to test adherence to a hardening guide/standard configuration (see `-L`/`--list-policies`, `-M`/`--make-policy` and `-P`/`--policy`).  For an in-depth tutorial, see <https://www.positronsecurity.com/blog/2020-09-27-ssh-policy-configuration-checks-with-ssh-audit/>.
-         - Created new man page (see `ssh-audit.1` file).
-         - 1024-bit moduli upgraded from warnings to failures.
-         - Many Python 2 code clean-ups, testing framework improvements, pylint & flake8 fixes, and mypy type comments; credit [Jürgen Gmach](https://github.com/jugmac00).
-         - Added feature to look up algorithms in internal database (see `--lookup`); credit [Adam Russell](https://github.com/thecliguy).
-         - Suppress recommendation of token host key types.
-         - Added check for use-after-free vulnerability in PuTTY v0.73.
-         - Added 11 new host key types: `ssh-rsa1`, `ssh-dss-sha256@ssh.com`, `ssh-gost2001`, `ssh-gost2012-256`, `ssh-gost2012-512`, `spki-sign-rsa`, `ssh-ed448`, `x509v3-ecdsa-sha2-nistp256`, `x509v3-ecdsa-sha2-nistp384`, `x509v3-ecdsa-sha2-nistp521`, `x509v3-rsa2048-sha256`.
-         - Added 8 new key exchanges: `diffie-hellman-group1-sha256`, `kexAlgoCurve25519SHA256`, `Curve25519SHA256`, `gss-group14-sha256-`, `gss-group15-sha512-`, `gss-group16-sha512-`, `gss-nistp256-sha256-`, `gss-curve25519-sha256-`.
-         - Added 5 new ciphers: `blowfish`, `AEAD_AES_128_GCM`, `AEAD_AES_256_GCM`, `crypticore128@ssh.com`, `seed-cbc@ssh.com`.
-         - Added 3 new MACs: `chacha20-poly1305@openssh.com`, `hmac-sha3-224`, `crypticore-mac@ssh.com`.
-        
-        ### v2.2.0 (2020-03-11)
-         - Marked host key type `ssh-rsa` as weak due to [practical SHA-1 collisions](https://eprint.iacr.org/2020/014.pdf).
-         - Added Windows builds.
-         - Added 10 new host key types: `ecdsa-sha2-1.3.132.0.10`, `x509v3-sign-dss`, `x509v3-sign-rsa`, `x509v3-sign-rsa-sha256@ssh.com`, `x509v3-ssh-dss`, `x509v3-ssh-rsa`, `sk-ecdsa-sha2-nistp256-cert-v01@openssh.com`, `sk-ecdsa-sha2-nistp256@openssh.com`, `sk-ssh-ed25519-cert-v01@openssh.com`, and `sk-ssh-ed25519@openssh.com`.
-         - Added 18 new key exchanges: `diffie-hellman-group14-sha256@ssh.com`, `diffie-hellman-group15-sha256@ssh.com`, `diffie-hellman-group15-sha384@ssh.com`, `diffie-hellman-group16-sha384@ssh.com`, `diffie-hellman-group16-sha512@ssh.com`, `diffie-hellman-group18-sha512@ssh.com`, `ecdh-sha2-curve25519`, `ecdh-sha2-nistb233`, `ecdh-sha2-nistb409`, `ecdh-sha2-nistk163`, `ecdh-sha2-nistk233`, `ecdh-sha2-nistk283`, `ecdh-sha2-nistk409`, `ecdh-sha2-nistp192`, `ecdh-sha2-nistp224`, `ecdh-sha2-nistt571`, `gss-gex-sha1-`, and `gss-group1-sha1-`.
-         - Added 9 new ciphers: `camellia128-cbc`, `camellia128-ctr`, `camellia192-cbc`, `camellia192-ctr`, `camellia256-cbc`, `camellia256-ctr`, `aes128-gcm`, `aes256-gcm`, and `chacha20-poly1305`.
-         - Added 2 new MACs: `aes128-gcm` and `aes256-gcm`.
-        
-        ### v2.1.1 (2019-11-26)
-         - Added 2 new host key types: `rsa-sha2-256-cert-v01@openssh.com`, `rsa-sha2-512-cert-v01@openssh.com`.
-         - Added 2 new ciphers: `des`, `3des`.
-         - Added 3 new PuTTY vulnerabilities.
-         - During client testing, client IP address is now listed in output.
-        
-        ### v2.1.0 (2019-11-14)
-         - Added client software auditing functionality (see `-c` / `--client-audit` option).
-         - Added JSON output option (see `-j` / `--json` option; credit [Andreas Jaggi](https://github.com/x-way)).
-         - Fixed crash while scanning Solaris Sun_SSH.
-         - Added 9 new key exchanges: `gss-group1-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-gex-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha1-`, `gss-group14-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha256-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group15-sha512-toWM5Slw5Ew8Mqkay+al2g==`, `diffie-hellman-group15-sha256`, `ecdh-sha2-1.3.132.0.10`, `curve448-sha512`.
-         - Added 1 new host key type: `ecdsa-sha2-1.3.132.0.10`.
-         - Added 4 new ciphers: `idea-cbc`, `serpent128-cbc`, `serpent192-cbc`, `serpent256-cbc`.
-         - Added 6 new MACs: `hmac-sha2-256-96-etm@openssh.com`, `hmac-sha2-512-96-etm@openssh.com`, `hmac-ripemd`, `hmac-sha256-96@ssh.com`, `umac-32@openssh.com`, `umac-96@openssh.com`.
-        
-        ### v2.0.0 (2019-08-29)
-         - Forked from https://github.com/arthepsy/ssh-audit (development was stalled, and developer went MIA).
-         - Added RSA host key length test.
-         - Added RSA certificate key length test.
-         - Added Diffie-Hellman modulus size test.
-         - Now outputs host key fingerprints for RSA and ED25519.
-         - Added 5 new key exchanges: `sntrup4591761x25519-sha512@tinyssh.org`, `diffie-hellman-group-exchange-sha256@ssh.com`, `diffie-hellman-group-exchange-sha512@ssh.com`, `diffie-hellman-group16-sha256`, `diffie-hellman-group17-sha512`.
-         - Added 3 new encryption algorithms: `des-cbc-ssh1`, `blowfish-ctr`, `twofish-ctr`.
-         - Added 10 new MACs: `hmac-sha2-56`, `hmac-sha2-224`, `hmac-sha2-384`, `hmac-sha3-256`, `hmac-sha3-384`, `hmac-sha3-512`, `hmac-sha256`, `hmac-sha256@ssh.com`, `hmac-sha512`, `hmac-512@ssh.com`.
-         - Added command line argument (`-t` / `--timeout`) for connection & reading timeouts.
-         - Updated CVEs for libssh & Dropbear.
-        
-        ### v1.7.0 (2016-10-26)
-         - implement options to allow specify IPv4/IPv6 usage and order of precedence
-         - implement option to specify remote port (old behavior kept for compatibility)
-         - add colors support for Microsoft Windows via optional colorama dependency
-         - fix encoding and decoding issues, add tests, do not crash on encoding errors
-         - use mypy-lang for static type checking and verify all code
-        
-        ### v1.6.0 (2016-10-14)
-         - implement algorithm recommendations section (based on recognized software)
-         - implement full libssh support (version history, algorithms, security, etc)
-         - fix SSH-1.99 banner recognition and version comparison functionality
-         - do not output empty algorithms (happens for misconfigured servers)
-         - make consistent output for Python 3.x versions
-         - add a lot more tests (conf, banner, software, SSH1/SSH2, output, etc)
-         - use Travis CI to test for multiple Python versions (2.6-3.5, pypy, pypy3)
-        
-        ### v1.5.0 (2016-09-20)
-         - create security section for related security information
-         - match and output assigned CVE list and security issues for Dropbear SSH
-         - implement full SSH1 support with fingerprint information
-         - automatically fallback to SSH1 on protocol mismatch
-         - add new options to force SSH1 or SSH2 (both allowed by default)
-         - parse banner information and convert it to specific software and OS version
-         - do not use padding in batch mode
-         - several fixes (Cisco sshd, rare hangs, error handling, etc)
-        
-        ### v1.0.20160902
-         - implement batch output option
-         - implement minimum output level option
-         - fix compatibility with Python 2.6
-        
-        ### v1.0.20160812
-         - implement SSH version compatibility feature
-         - fix wrong mac algorithm warning
-         - fix Dropbear SSH version typo
-         - parse pre-banner header
-         - better errors handling
-        
-        ### v1.0.20160803
-         - use OpenSSH 7.3 banner
-         - add new key-exchange algorithms
-        
-        ### v1.0.20160207
-         - use OpenSSH 7.2 banner
-         - additional warnings for OpenSSH 7.2 
-         - fix OpenSSH 7.0 failure messages
-         - add rijndael-cbc failure message from OpenSSH 6.7
-        
-        ### v1.0.20160105
-         - multiple additional warnings
-         - support for none algorithm
-         - better compression handling  
-         - ensure reading enough data (fixes few Linux SSH)  
-        
-        ### v1.0.20151230
-         - Dropbear SSH support  
-        
-        ### v1.0.20151223
-         - initial version  
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Security
-Classifier: Topic :: Security :: Cryptography
-Requires-Python: <4,>=3.6
-Description-Content-Type: text/markdown
+# ssh-audit
+[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/LICENSE)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/ssh-audit)](https://pypi.org/project/ssh-audit/)
+[![Docker Pulls](https://img.shields.io/docker/pulls/positronsecurity/ssh-audit)](https://hub.docker.com/r/positronsecurity/ssh-audit)
+[![Build Status](https://github.com/jtesta/ssh-audit/actions/workflows/tox.yaml/badge.svg)](https://github.com/jtesta/ssh-audit/actions)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/CONTRIBUTING.md)
+
+**ssh-audit** is a tool for ssh server & client configuration auditing.
+
+[jtesta/ssh-audit](https://github.com/jtesta/ssh-audit/) (v2.0+) is the updated and maintained version of ssh-audit forked from [arthepsy/ssh-audit](https://github.com/arthepsy/ssh-audit) (v1.x) due to inactivity.
+
+- [Features](#features)
+- [Usage](#usage)
+- [Screenshots](#screenshots)
+    - [Server Standard Audit Example](#server-standard-audit-example)
+    - [Server Policy Audit Example](#server-policy-audit-example)
+    - [Client Standard Audit Example](#client-standard-audit-example)
+- [Hardening Guides](#hardening-guides)
+- [Pre-Built Packages](#pre-built-packages)
+- [Web Front-End](#web-front-end)
+- [ChangeLog](#changelog)
+
+## Features
+- SSH1 and SSH2 protocol server support;
+- analyze SSH client configuration;
+- grab banner, recognize device or software and operating system, detect compression;
+- gather key-exchange, host-key, encryption and message authentication code algorithms;
+- output algorithm information (available since, removed/disabled, unsafe/weak/legacy, etc);
+- output algorithm recommendations (append or remove based on recognized software version);
+- output security information (related issues, assigned CVE list, etc);
+- analyze SSH version compatibility based on algorithm information;
+- historical information from OpenSSH, Dropbear SSH and libssh;
+- policy scans to ensure adherence to a hardened/standard configuration;
+- runs on Linux and Windows;
+- supports Python 3.7 - 3.11;
+- no dependencies
+
+## Usage
+```
+usage: ssh-audit.py [options] <host>
+
+   -h,  --help             print this help
+   -1,  --ssh1             force ssh version 1 only
+   -2,  --ssh2             force ssh version 2 only
+   -4,  --ipv4             enable IPv4 (order of precedence)
+   -6,  --ipv6             enable IPv6 (order of precedence)
+   -b,  --batch            batch output
+   -c,  --client-audit     starts a server on port 2222 to audit client
+                               software config (use -p to change port;
+                               use -t to change timeout)
+   -d,  --debug            Enable debug output.
+   -g,  --gex-test=<x[,y,...]>  dh gex modulus size test
+                   <min1:pref1:max1[,min2:pref2:max2,...]>
+                   <x-y[:step]>
+   -j,  --json             JSON output (use -jj to enable indents)
+   -l,  --level=<level>    minimum output level (info|warn|fail)
+   -L,  --list-policies    list all the official, built-in policies
+        --lookup=<alg1,alg2,...>    looks up an algorithm(s) without
+                                    connecting to a server
+   -m,  --manual           print the man page (Windows only)
+   -M,  --make-policy=<policy.txt>  creates a policy based on the target server
+                                    (i.e.: the target server has the ideal
+                                    configuration that other servers should
+                                    adhere to)
+   -n,  --no-colors        disable colors
+   -p,  --port=<port>      port to connect
+   -P,  --policy=<"policy name" | policy.txt>  run a policy test using the
+                                                   specified policy
+   -t,  --timeout=<secs>   timeout (in seconds) for connection and reading
+                               (default: 5)
+   -T,  --targets=<hosts.txt>  a file containing a list of target hosts (one
+                                   per line, format HOST[:PORT])
+        --threads=<threads>    number of threads to use when scanning multiple
+                                   targets (-T/--targets) (default: 32)
+   -v,  --verbose          verbose output
+```
+* if both IPv4 and IPv6 are used, order of precedence can be set by using either `-46` or `-64`.
+* batch flag `-b` will output sections without header and without empty lines (implies verbose flag).
+* verbose flag `-v` will prefix each line with section type and algorithm name.
+* an exit code of 0 is returned when all algorithms are considered secure (for a standard audit), or when a policy check passes (for a policy audit).
+
+Basic server auditing:
+```
+ssh-audit localhost
+ssh-audit 127.0.0.1
+ssh-audit 127.0.0.1:222
+ssh-audit ::1
+ssh-audit [::1]:222
+```
+
+To run a standard audit against many servers (place targets into servers.txt, one on each line in the format of `HOST[:PORT]`):
+
+```
+ssh-audit -T servers.txt
+```
+
+To audit a client configuration (listens on port 2222 by default; connect using `ssh -p 2222 anything@localhost`):
+
+```
+ssh-audit -c
+```
+
+To audit a client configuration, with a listener on port 4567:
+```
+ssh-audit -c -p 4567
+```
+
+To  list all official built-in policies (hint: use resulting policy names with `-P`/`--policy`):
+```
+ssh-audit -L
+```
+
+To run a policy audit against a server:
+```
+ssh-audit -P ["policy name" | path/to/server_policy.txt] targetserver
+```
+
+To run a policy audit against a client:
+```
+ssh-audit -c -P ["policy name" | path/to/client_policy.txt]
+```
+
+To run a policy audit against many servers:
+```
+ssh-audit -T servers.txt -P ["policy name" | path/to/server_policy.txt]
+```
+
+To create a policy based on a target server (which can be manually edited):
+```
+ssh-audit -M new_policy.txt targetserver
+```
+
+## Screenshots
+
+### Server Standard Audit Example
+Below is a screen shot of the standard server-auditing output when connecting to an unhardened OpenSSH v5.3 service:
+![screenshot](https://user-images.githubusercontent.com/2982011/64388792-317e6f80-d00e-11e9-826e-a4934769bb07.png)
+
+### Server Policy Audit Example
+Below is a screen shot of the policy auditing output when connecting to an un-hardened Ubuntu Server 20.04 machine (hint: use `-L`/`--list-policies` to see names of built-in policies to use with `-P`/`--policy`):
+![screenshot](https://user-images.githubusercontent.com/2982011/94370881-95178700-00c0-11eb-8705-3157a4669dc0.png)
+
+After applying the steps in the hardening guide (see below), the output changes to the following:
+![screenshot](https://user-images.githubusercontent.com/2982011/94370873-87620180-00c0-11eb-9a59-469f61a56ce1.png)
+
+### Client Standard Audit Example
+Below is a screen shot of the client-auditing output when an unhardened OpenSSH v7.2 client connects:
+![client_screenshot](https://user-images.githubusercontent.com/2982011/68867998-b946c100-06c4-11ea-975f-1f47e4178a74.png)
+
+## Hardening Guides
+Guides to harden server & client configuration can be found here: [https://www.ssh-audit.com/hardening_guides.html](https://www.ssh-audit.com/hardening_guides.html)
+
+## Pre-Built Packages
+Pre-built packages are available for Windows (see the releases page), PyPI, Snap, and Docker:
+
+To install from PyPI:
+```
+$ pip3 install ssh-audit
+```
+
+To install the Snap package:
+```
+$ snap install ssh-audit
+```
+
+To install from Dockerhub:
+```
+$ docker pull positronsecurity/ssh-audit
+```
+(Then run with: `docker run -it -p 2222:2222 positronsecurity/ssh-audit 10.1.1.1`)
+
+The status of various other platform packages can be found below (via Repology):
+
+<a href="https://repology.org/project/ssh-audit/versions"><img src="https://repology.org/badge/vertical-allrepos/ssh-audit.svg?columns=4" alt="Packaging status" align="center"></a>
+
+## Web Front-End
+For convenience, a web front-end on top of the command-line tool is available at [https://www.ssh-audit.com/](https://www.ssh-audit.com/).
+
+## ChangeLog
+
+### v2.9.0 (2023-04-29)
+ - Dropped support for Python 3.6, as it reached EOL at the end of 2021.
+ - Added Ubuntu Server & Client 22.04 hardening policies.
+ - Removed experimental warning tag from `sntrup761x25519-sha512@openssh.com`.
+ - Updated CVE database; credit [Alexandre Zanni](https://github.com/noraj).
+ - Added `-g` and `--gex-test` for granular GEX modulus size tests; credit [Adam Russell](https://github.com/thecliguy).
+ - Snap packages now print more user-friendly error messages when permission errors are encountered.
+ - JSON 'target' field now always includes port number; credit [tomatohater1337](https://github.com/tomatohater1337).
+ - JSON output now includes recommendations and CVE data.
+ - Mixed host key/CA key types (i.e.: RSA host keys signed with ED25519 CAs, etc.) are now properly handled.
+ - Warnings are now printed for 2048-bit moduli; partial credit [Adam Russell](https://github.com/thecliguy).
+ - SHA-1 algorithms now cause failures.
+ - CBC mode ciphers are now warnings instead of failures.
+ - Generic failure/warning messages replaced with more specific reasons (i.e.: 'using weak cipher' => 'using broken RC4 cipher').
+ - Updated built-in policies to include missing host key size information.
+ - Added built-in policies for OpenSSH 8.8, 8.9, 9.0, 9.1, 9.2, and 9.3.
+ - Added 33 new host keys: `dsa2048-sha224@libassh.org`, `dsa2048-sha256@libassh.org`, `dsa3072-sha256@libassh.org`, `ecdsa-sha2-1.3.132.0.10-cert-v01@openssh.com`, `eddsa-e382-shake256@libassh.org`, `eddsa-e521-shake256@libassh.org`, `null`, `pgp-sign-dss`, `pgp-sign-rsa`, `spki-sign-dss`, `spki-sign-rsa`, `ssh-dss-sha224@ssh.com`, `ssh-dss-sha384@ssh.com`, `ssh-dss-sha512@ssh.com`, `ssh-ed448-cert-v01@openssh.com`, `ssh-rsa-sha224@ssh.com`, `ssh-rsa-sha2-256`, `ssh-rsa-sha2-512`, `ssh-rsa-sha384@ssh.com`, `ssh-rsa-sha512@ssh.com`, `ssh-xmss-cert-v01@openssh.com`, `ssh-xmss@openssh.com`, `webauthn-sk-ecdsa-sha2-nistp256@openssh.com`, `x509v3-ecdsa-sha2-1.3.132.0.10`, `x509v3-sign-dss-sha1`, `x509v3-sign-dss-sha224@ssh.com`, `x509v3-sign-dss-sha256@ssh.com`, `x509v3-sign-dss-sha384@ssh.com`, `x509v3-sign-dss-sha512@ssh.com`, `x509v3-sign-rsa-sha1`, `x509v3-sign-rsa-sha224@ssh.com`, `x509v3-sign-rsa-sha384@ssh.com`, `x509v3-sign-rsa-sha512@ssh.com`.
+ - Added 46 new key exchanges: `diffie-hellman-group14-sha224@ssh.com`, `diffie-hellman_group17-sha512`, `diffie-hellman-group-exchange-sha224@ssh.com`, `diffie-hellman-group-exchange-sha384@ssh.com`, `ecdh-sha2-1.2.840.10045.3.1.1`, `ecdh-sha2-1.2.840.10045.3.1.7`, `ecdh-sha2-1.3.132.0.1`, `ecdh-sha2-1.3.132.0.16`, `ecdh-sha2-1.3.132.0.26`, `ecdh-sha2-1.3.132.0.27`, `ecdh-sha2-1.3.132.0.33`, `ecdh-sha2-1.3.132.0.34`, `ecdh-sha2-1.3.132.0.35`, `ecdh-sha2-1.3.132.0.36`, `ecdh-sha2-1.3.132.0.37`, `ecdh-sha2-1.3.132.0.38`, `ecdh-sha2-4MHB+NBt3AlaSRQ7MnB4cg==`, `ecdh-sha2-5pPrSUQtIaTjUSt5VZNBjg==`, `ecdh-sha2-9UzNcgwTlEnSCECZa7V1mw==`, `ecdh-sha2-D3FefCjYoJ/kfXgAyLddYA==`, `ecdh-sha2-h/SsxnLCtRBh7I9ATyeB3A==`, `ecdh-sha2-m/FtSAmrV4j/Wy6RVUaK7A==`, `ecdh-sha2-mNVwCXAoS1HGmHpLvBC94w==`, `ecdh-sha2-qCbG5Cn/jjsZ7nBeR7EnOA==`, `ecdh-sha2-qcFQaMAMGhTziMT0z+Tuzw==`, `ecdh-sha2-VqBg4QRPjxx1EXZdV0GdWQ==`, `ecdh-sha2-wiRIU8TKjMZ418sMqlqtvQ==`, `ecdh-sha2-zD/b3hu/71952ArpUG4OjQ==`, `ecmqv-sha2`, `gss-13.3.132.0.10-sha256-*`, `gss-curve25519-sha256-*`, `gss-curve448-sha512-*`, `gss-gex-sha1-*`, `gss-gex-sha256-*`, `gss-group14-sha1-*`, `gss-group14-sha256-*`, `gss-group15-sha512-*`, `gss-group16-sha512-*`, `gss-group17-sha512-*`, `gss-group18-sha512-*`, `gss-group1-sha1-*`, `gss-nistp256-sha256-*`, `gss-nistp384-sha256-*`, `gss-nistp521-sha512-*`, `m383-sha384@libassh.org`, `m511-sha512@libassh.org`.
+ - Added 28 new ciphers: `3des-cfb`, `3des-ecb`, `3des-ofb`, `blowfish-cfb`, `blowfish-ecb`, `blowfish-ofb`, `camellia128-cbc@openssh.org`, `camellia128-ctr@openssh.org`, `camellia192-cbc@openssh.org`, `camellia192-ctr@openssh.org`, `camellia256-cbc@openssh.org`, `camellia256-ctr@openssh.org`, `cast128-cfb`, `cast128-ecb`, `cast128-ofb`, `cast128-12-cbc@ssh.com`, `idea-cfb`, `idea-ecb`, `idea-ofb`, `rijndael-cbc@ssh.com`, `seed-ctr@ssh.com`, `serpent128-gcm@libassh.org`, `serpent256-gcm@libassh.org`, `twofish128-gcm@libassh.org`, `twofish256-gcm@libassh.org`, `twofish-cfb`, `twofish-ecb`, `twofish-ofb`
+ - Added 5 new MACs: `hmac-sha1-96@openssh.com`, `hmac-sha224@ssh.com`, `hmac-sha256-2@ssh.com`, `hmac-sha384@ssh.com`, `hmac-whirlpool`.
+
+### v2.5.0 (2021-08-26)
+ - Fixed crash when running host key tests.
+ - Handles server connection failures more gracefully.
+ - Now prints JSON with indents when `-jj` is used (useful for debugging).
+ - Added MD5 fingerprints to verbose output.
+ - Added `-d`/`--debug` option for getting debugging output; credit [Adam Russell](https://github.com/thecliguy).
+ - Updated JSON output to include MD5 fingerprints.  Note that this results in a breaking change in the 'fingerprints' dictionary format.
+ - Updated OpenSSH 8.1 (and earlier) policies to include `rsa-sha2-512` and `rsa-sha2-256`.
+ - Added OpenSSH v8.6 & v8.7 policies.
+ - Added 3 new key exchanges: `gss-gex-sha1-eipGX3TCiQSrx573bT1o1Q==`, `gss-group1-sha1-eipGX3TCiQSrx573bT1o1Q==`, and `gss-group14-sha1-eipGX3TCiQSrx573bT1o1Q==`.
+ - Added 3 new MACs: `hmac-ripemd160-96`, `AEAD_AES_128_GCM`, and `AEAD_AES_256_GCM`.
+
+### v2.4.0 (2021-02-23)
+ - Added multi-threaded scanning support.
+ - Added built-in Windows manual page (see `-m`/`--manual`); credit [Adam Russell](https://github.com/thecliguy).
+ - Added version check for OpenSSH user enumeration (CVE-2018-15473).
+ - Added deprecation note to host key types based on SHA-1.
+ - Added extra warnings for SSHv1.
+ - Added built-in hardened OpenSSH v8.5 policy.
+ - Upgraded warnings to failures for host key types based on SHA-1.
+ - Fixed crash when receiving unexpected response during host key test.
+ - Fixed hang against older Cisco devices during host key test & gex test.
+ - Fixed improper termination while scanning multiple targets when one target returns an error.
+ - Dropped support for Python 3.5 (which reached EOL in Sept. 2020).
+ - Added 1 new key exchange: `sntrup761x25519-sha512@openssh.com`.
+
+### v2.3.1 (2020-10-28)
+ - Now parses public key sizes for `rsa-sha2-256-cert-v01@openssh.com` and `rsa-sha2-512-cert-v01@openssh.com` host key types.
+ - Flag `ssh-rsa-cert-v01@openssh.com` as a failure due to SHA-1 hash.
+ - Fixed bug in recommendation output which suppressed some algorithms inappropriately.
+ - Built-in policies now include CA key requirements (if certificates are in use).
+ - Lookup function (`--lookup`) now performs case-insensitive lookups of similar algorithms; credit [Adam Russell](https://github.com/thecliguy).
+ - Migrated pre-made policies from external files to internal database.
+ - Split single 3,500 line script into many files (by class).
+ - Added setup.py support; credit [Ganden Schaffner](https://github.com/gschaffner).
+ - Added 1 new cipher: `des-cbc@ssh.com`.
+
+### v2.3.0 (2020-09-27)
+ - Added new policy auditing functionality to test adherence to a hardening guide/standard configuration (see `-L`/`--list-policies`, `-M`/`--make-policy` and `-P`/`--policy`).  For an in-depth tutorial, see <https://www.positronsecurity.com/blog/2020-09-27-ssh-policy-configuration-checks-with-ssh-audit/>.
+ - Created new man page (see `ssh-audit.1` file).
+ - 1024-bit moduli upgraded from warnings to failures.
+ - Many Python 2 code clean-ups, testing framework improvements, pylint & flake8 fixes, and mypy type comments; credit [Jürgen Gmach](https://github.com/jugmac00).
+ - Added feature to look up algorithms in internal database (see `--lookup`); credit [Adam Russell](https://github.com/thecliguy).
+ - Suppress recommendation of token host key types.
+ - Added check for use-after-free vulnerability in PuTTY v0.73.
+ - Added 11 new host key types: `ssh-rsa1`, `ssh-dss-sha256@ssh.com`, `ssh-gost2001`, `ssh-gost2012-256`, `ssh-gost2012-512`, `spki-sign-rsa`, `ssh-ed448`, `x509v3-ecdsa-sha2-nistp256`, `x509v3-ecdsa-sha2-nistp384`, `x509v3-ecdsa-sha2-nistp521`, `x509v3-rsa2048-sha256`.
+ - Added 8 new key exchanges: `diffie-hellman-group1-sha256`, `kexAlgoCurve25519SHA256`, `Curve25519SHA256`, `gss-group14-sha256-`, `gss-group15-sha512-`, `gss-group16-sha512-`, `gss-nistp256-sha256-`, `gss-curve25519-sha256-`.
+ - Added 5 new ciphers: `blowfish`, `AEAD_AES_128_GCM`, `AEAD_AES_256_GCM`, `crypticore128@ssh.com`, `seed-cbc@ssh.com`.
+ - Added 3 new MACs: `chacha20-poly1305@openssh.com`, `hmac-sha3-224`, `crypticore-mac@ssh.com`.
+
+### v2.2.0 (2020-03-11)
+ - Marked host key type `ssh-rsa` as weak due to [practical SHA-1 collisions](https://eprint.iacr.org/2020/014.pdf).
+ - Added Windows builds.
+ - Added 10 new host key types: `ecdsa-sha2-1.3.132.0.10`, `x509v3-sign-dss`, `x509v3-sign-rsa`, `x509v3-sign-rsa-sha256@ssh.com`, `x509v3-ssh-dss`, `x509v3-ssh-rsa`, `sk-ecdsa-sha2-nistp256-cert-v01@openssh.com`, `sk-ecdsa-sha2-nistp256@openssh.com`, `sk-ssh-ed25519-cert-v01@openssh.com`, and `sk-ssh-ed25519@openssh.com`.
+ - Added 18 new key exchanges: `diffie-hellman-group14-sha256@ssh.com`, `diffie-hellman-group15-sha256@ssh.com`, `diffie-hellman-group15-sha384@ssh.com`, `diffie-hellman-group16-sha384@ssh.com`, `diffie-hellman-group16-sha512@ssh.com`, `diffie-hellman-group18-sha512@ssh.com`, `ecdh-sha2-curve25519`, `ecdh-sha2-nistb233`, `ecdh-sha2-nistb409`, `ecdh-sha2-nistk163`, `ecdh-sha2-nistk233`, `ecdh-sha2-nistk283`, `ecdh-sha2-nistk409`, `ecdh-sha2-nistp192`, `ecdh-sha2-nistp224`, `ecdh-sha2-nistt571`, `gss-gex-sha1-`, and `gss-group1-sha1-`.
+ - Added 9 new ciphers: `camellia128-cbc`, `camellia128-ctr`, `camellia192-cbc`, `camellia192-ctr`, `camellia256-cbc`, `camellia256-ctr`, `aes128-gcm`, `aes256-gcm`, and `chacha20-poly1305`.
+ - Added 2 new MACs: `aes128-gcm` and `aes256-gcm`.
+
+### v2.1.1 (2019-11-26)
+ - Added 2 new host key types: `rsa-sha2-256-cert-v01@openssh.com`, `rsa-sha2-512-cert-v01@openssh.com`.
+ - Added 2 new ciphers: `des`, `3des`.
+ - Added 3 new PuTTY vulnerabilities.
+ - During client testing, client IP address is now listed in output.
+
+### v2.1.0 (2019-11-14)
+ - Added client software auditing functionality (see `-c` / `--client-audit` option).
+ - Added JSON output option (see `-j` / `--json` option; credit [Andreas Jaggi](https://github.com/x-way)).
+ - Fixed crash while scanning Solaris Sun_SSH.
+ - Added 9 new key exchanges: `gss-group1-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-gex-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha1-`, `gss-group14-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha256-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group15-sha512-toWM5Slw5Ew8Mqkay+al2g==`, `diffie-hellman-group15-sha256`, `ecdh-sha2-1.3.132.0.10`, `curve448-sha512`.
+ - Added 1 new host key type: `ecdsa-sha2-1.3.132.0.10`.
+ - Added 4 new ciphers: `idea-cbc`, `serpent128-cbc`, `serpent192-cbc`, `serpent256-cbc`.
+ - Added 6 new MACs: `hmac-sha2-256-96-etm@openssh.com`, `hmac-sha2-512-96-etm@openssh.com`, `hmac-ripemd`, `hmac-sha256-96@ssh.com`, `umac-32@openssh.com`, `umac-96@openssh.com`.
+
+### v2.0.0 (2019-08-29)
+ - Forked from https://github.com/arthepsy/ssh-audit (development was stalled, and developer went MIA).
+ - Added RSA host key length test.
+ - Added RSA certificate key length test.
+ - Added Diffie-Hellman modulus size test.
+ - Now outputs host key fingerprints for RSA and ED25519.
+ - Added 5 new key exchanges: `sntrup4591761x25519-sha512@tinyssh.org`, `diffie-hellman-group-exchange-sha256@ssh.com`, `diffie-hellman-group-exchange-sha512@ssh.com`, `diffie-hellman-group16-sha256`, `diffie-hellman-group17-sha512`.
+ - Added 3 new encryption algorithms: `des-cbc-ssh1`, `blowfish-ctr`, `twofish-ctr`.
+ - Added 10 new MACs: `hmac-sha2-56`, `hmac-sha2-224`, `hmac-sha2-384`, `hmac-sha3-256`, `hmac-sha3-384`, `hmac-sha3-512`, `hmac-sha256`, `hmac-sha256@ssh.com`, `hmac-sha512`, `hmac-512@ssh.com`.
+ - Added command line argument (`-t` / `--timeout`) for connection & reading timeouts.
+ - Updated CVEs for libssh & Dropbear.
+
+### v1.7.0 (2016-10-26)
+ - implement options to allow specify IPv4/IPv6 usage and order of precedence
+ - implement option to specify remote port (old behavior kept for compatibility)
+ - add colors support for Microsoft Windows via optional colorama dependency
+ - fix encoding and decoding issues, add tests, do not crash on encoding errors
+ - use mypy-lang for static type checking and verify all code
+
+### v1.6.0 (2016-10-14)
+ - implement algorithm recommendations section (based on recognized software)
+ - implement full libssh support (version history, algorithms, security, etc)
+ - fix SSH-1.99 banner recognition and version comparison functionality
+ - do not output empty algorithms (happens for misconfigured servers)
+ - make consistent output for Python 3.x versions
+ - add a lot more tests (conf, banner, software, SSH1/SSH2, output, etc)
+ - use Travis CI to test for multiple Python versions (2.6-3.5, pypy, pypy3)
+
+### v1.5.0 (2016-09-20)
+ - create security section for related security information
+ - match and output assigned CVE list and security issues for Dropbear SSH
+ - implement full SSH1 support with fingerprint information
+ - automatically fallback to SSH1 on protocol mismatch
+ - add new options to force SSH1 or SSH2 (both allowed by default)
+ - parse banner information and convert it to specific software and OS version
+ - do not use padding in batch mode
+ - several fixes (Cisco sshd, rare hangs, error handling, etc)
+
+### v1.0.20160902
+ - implement batch output option
+ - implement minimum output level option
+ - fix compatibility with Python 2.6
+
+### v1.0.20160812
+ - implement SSH version compatibility feature
+ - fix wrong mac algorithm warning
+ - fix Dropbear SSH version typo
+ - parse pre-banner header
+ - better errors handling
+
+### v1.0.20160803
+ - use OpenSSH 7.3 banner
+ - add new key-exchange algorithms
+
+### v1.0.20160207
+ - use OpenSSH 7.2 banner
+ - additional warnings for OpenSSH 7.2
+ - fix OpenSSH 7.0 failure messages
+ - add rijndael-cbc failure message from OpenSSH 6.7
+
+### v1.0.20160105
+ - multiple additional warnings
+ - support for none algorithm
+ - better compression handling
+ - ensure reading enough data (fixes few Linux SSH)
+
+### v1.0.20151230
+ - Dropbear SSH support
+
+### v1.0.20151223
+ - initial version
```

### Comparing `ssh-audit-2.5.0/setup.cfg` & `ssh-audit-2.9.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -2,40 +2,42 @@
 name = ssh-audit
 version = attr: ssh_audit.globals.VERSION
 author = Joe Testa
 author_email = jtesta@positronsecurity.com
 description = An SSH server & client configuration security auditing tool
 long_description = file: README.md
 long_description_content_type = text/markdown
-license_file = LICENSE
+license = MIT
+license_files = LICENSE
 url = https://github.com/jtesta/ssh-audit
 project_urls = 
 	Source Code = https://github.com/jtesta/ssh-audit
 	Bug Tracker = https://github.com/jtesta/ssh-audit/issues
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	Topic :: Security
 	Topic :: Security :: Cryptography
 
 [options]
 packages = find:
 package_dir = 
 	= src
-python_requires = >=3.6,<4
+python_requires = >=3.7,<4
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	ssh-audit = ssh_audit.ssh_audit:main
```

### Comparing `ssh-audit-2.5.0/setup.py` & `ssh-audit-2.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/algorithm.py` & `ssh-audit-2.9.0/src/ssh_audit/algorithm.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/algorithms.py` & `ssh-audit-2.9.0/src/ssh_audit/algorithms.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/auditconf.py` & `ssh-audit-2.9.0/src/ssh_audit/auditconf.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         self.target_file: Optional[str] = None
         self.target_list: List[str] = []
         self.threads = 32
         self.list_policies = False
         self.lookup = ''
         self.manual = False
         self.debug = False
+        self.gex_test = ''
 
     def __setattr__(self, name: str, value: Union[str, int, float, bool, Sequence[int]]) -> None:
         valid = False
         if name in ['batch', 'client_audit', 'colors', 'json', 'json_print_indent', 'list_policies', 'manual', 'make_policy', 'ssh1', 'ssh2', 'timeout_set', 'verbose', 'debug']:
             valid, value = True, bool(value)
         elif name in ['ipv4', 'ipv6']:
             valid, value = True, bool(value)
@@ -82,15 +83,15 @@
         elif name == 'host':
             valid = True
         elif name == 'timeout':
             value = Utils.parse_float(value)
             if value == -1.0:
                 raise ValueError('invalid timeout: {}'.format(value))
             valid = True
-        elif name in ['ip_version_preference', 'lookup', 'policy_file', 'policy', 'target_file', 'target_list']:
+        elif name in ['ip_version_preference', 'lookup', 'policy_file', 'policy', 'target_file', 'target_list', 'gex_test']:
             valid = True
         elif name == "threads":
             valid, num_threads = True, Utils.parse_int(value)
             if num_threads < 1:
                 raise ValueError('invalid number of threads: {}'.format(value))
             value = num_threads
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/banner.py` & `ssh-audit-2.9.0/src/ssh_audit/banner.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/fingerprint.py` & `ssh-audit-2.9.0/src/ssh_audit/fingerprint.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/globals.py` & `ssh-audit-2.9.0/src/ssh_audit/product.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
    The MIT License (MIT)
 
-   Copyright (C) 2017-2021 Joe Testa (jtesta@positronsecurity.com)
+   Copyright (C) 2017 Andris Raugulis (moo@arthepsy.eu)
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
@@ -17,11 +17,15 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
-VERSION = 'v2.5.0'
-SSH_HEADER = 'SSH-{0}-OpenSSH_8.2'  # SSH software to impersonate
-GITHUB_ISSUES_URL = 'https://github.com/jtesta/ssh-audit/issues'  # The URL to the Github issues tracker.
-WINDOWS_MAN_PAGE = ''
+
+
+class Product:  # pylint: disable=too-few-public-methods
+    OpenSSH = 'OpenSSH'
+    DropbearSSH = 'Dropbear SSH'
+    LibSSH = 'libssh'
+    TinySSH = 'TinySSH'
+    PuTTY = 'PuTTY'
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/hostkeytest.py` & `ssh-audit-2.9.0/src/ssh_audit/gextest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
    The MIT License (MIT)
 
-   Copyright (C) 2017-2021 Joe Testa (jtesta@positronsecurity.com)
+   Copyright (C) 2017-2023 Joe Testa (jtesta@positronsecurity.com)
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
@@ -17,172 +17,221 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
+import traceback
 
 # pylint: disable=unused-import
 from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
 from typing import Callable, Optional, Union, Any  # noqa: F401
 
-import traceback
-
-from ssh_audit.kexdh import KexDH, KexGroup1, KexGroup14_SHA1, KexGroup14_SHA256, KexCurve25519_SHA256, KexGroup16_SHA512, KexGroup18_SHA512, KexGroupExchange_SHA1, KexGroupExchange_SHA256, KexNISTP256, KexNISTP384, KexNISTP521
-from ssh_audit.ssh2_kex import SSH2_Kex
+from ssh_audit.kexdh import KexDHException, KexGroupExchange_SHA1, KexGroupExchange_SHA256
 from ssh_audit.ssh2_kexdb import SSH2_KexDB
+from ssh_audit.ssh2_kex import SSH2_Kex
 from ssh_audit.ssh_socket import SSH_Socket
 from ssh_audit.outputbuffer import OutputBuffer
+from ssh_audit import exitcodes
+
+
+# Performs DH group exchanges to find what moduli are supported, and checks
+# their size.
+class GEXTest:
 
+    # Creates a new connection to the server.  Returns True on success, or False.
+    @staticmethod
+    def reconnect(out: 'OutputBuffer', s: 'SSH_Socket', kex: 'SSH2_Kex', gex_alg: str) -> bool:
+        if s.is_connected():
+            return True
+
+        err = s.connect()
+        if err is not None:
+            out.v(err, write_now=True)
+            return False
+
+        _, _, err = s.get_banner()
+        if err is not None:
+            out.v(err, write_now=True)
+            s.close()
+            return False
 
-# Obtains host keys, checks their size, and derives their fingerprints.
-class HostKeyTest:
-    # Tracks the RSA host key types.  As of this writing, testing one in this family yields valid results for the rest.
-    RSA_FAMILY = ['ssh-rsa', 'rsa-sha2-256', 'rsa-sha2-512']
-
-    # Dict holding the host key types we should extract & parse.  'cert' is True to denote that a host key type handles certificates (thus requires additional parsing).  'variable_key_len' is True for host key types that can have variable sizes (True only for RSA types, as the rest are of fixed-size).  After the host key type is fully parsed, the key 'parsed' is added with a value of True.
-    HOST_KEY_TYPES = {
-        'ssh-rsa':      {'cert': False, 'variable_key_len': True},
-        'rsa-sha2-256': {'cert': False, 'variable_key_len': True},
-        'rsa-sha2-512': {'cert': False, 'variable_key_len': True},
-
-        'ssh-rsa-cert-v01@openssh.com':      {'cert': True, 'variable_key_len': True},
-        'rsa-sha2-256-cert-v01@openssh.com': {'cert': True, 'variable_key_len': True},
-        'rsa-sha2-512-cert-v01@openssh.com': {'cert': True, 'variable_key_len': True},
-
-        'ssh-ed25519':                      {'cert': False, 'variable_key_len': False},
-        'ssh-ed25519-cert-v01@openssh.com': {'cert': True, 'variable_key_len': False},
-    }
+        # Send our KEX using the specified group-exchange and most of the
+        # server's own values.
+        s.send_kexinit(key_exchanges=[gex_alg], hostkeys=kex.key_algorithms, ciphers=kex.server.encryption, macs=kex.server.mac, compressions=kex.server.compression, languages=kex.server.languages)
+
+        try:
+            # Parse the server's KEX.
+            _, payload = s.read_packet(2)
+            SSH2_Kex.parse(out, payload)
+        except KexDHException:
+            out.v("Failed to parse server's kex.  Stack trace:\n%s" % str(traceback.format_exc()), write_now=True)
+            return False
+
+        return True
 
     @staticmethod
-    def run(out: 'OutputBuffer', s: 'SSH_Socket', server_kex: 'SSH2_Kex') -> None:
-        KEX_TO_DHGROUP = {
-            'diffie-hellman-group1-sha1': KexGroup1,
-            'diffie-hellman-group14-sha1': KexGroup14_SHA1,
-            'diffie-hellman-group14-sha256': KexGroup14_SHA256,
-            'curve25519-sha256': KexCurve25519_SHA256,
-            'curve25519-sha256@libssh.org': KexCurve25519_SHA256,
-            'diffie-hellman-group16-sha512': KexGroup16_SHA512,
-            'diffie-hellman-group18-sha512': KexGroup18_SHA512,
+    def granular_modulus_size_test(out: 'OutputBuffer', s: 'SSH_Socket', kex: 'SSH2_Kex', bits_min: int, bits_pref: int, bits_max: int, modulus_dict: Dict[str, List[int]]) -> int:
+        '''
+        Tests for granular modulus sizes.
+        Builds a dictionary, where a key represents a DH algorithm name and the
+        values are the modulus sizes (in bits) that have been returned by the
+        target server.
+        Returns an exitcodes.* flag.
+        '''
+
+        retval = exitcodes.GOOD
+
+        out.d("Starting modulus_size_test...")
+        out.d("Bits Min:  " + str(bits_min))
+        out.d("Bits Pref: " + str(bits_pref))
+        out.d("Bits Max:  " + str(bits_max))
+
+        GEX_ALGS = {
             'diffie-hellman-group-exchange-sha1': KexGroupExchange_SHA1,
             'diffie-hellman-group-exchange-sha256': KexGroupExchange_SHA256,
-            'ecdh-sha2-nistp256': KexNISTP256,
-            'ecdh-sha2-nistp384': KexNISTP384,
-            'ecdh-sha2-nistp521': KexNISTP521,
-            # 'kexguess2@matt.ucc.asn.au': ???
         }
 
-        # Pick the first kex algorithm that the server supports, which we
-        # happen to support as well.
-        kex_str = None
-        kex_group = None
-        for server_kex_alg in server_kex.kex_algorithms:
-            if server_kex_alg in KEX_TO_DHGROUP:
-                kex_str = server_kex_alg
-                kex_group = KEX_TO_DHGROUP[kex_str]()
-                break
+        # Check if the server supports any of the group-exchange
+        # algorithms.  If so, test each one.
+        for gex_alg, kex_group_class in GEX_ALGS.items():
+            if gex_alg not in kex.kex_algorithms:
+                out.d('Server does not support the algorithm "' + gex_alg + '".', write_now=True)
+            else:
+                kex_group = kex_group_class(out)
+                out.d('Preparing to perform DH group exchange using ' + gex_alg + ' with min, pref and max modulus sizes of ' + str(bits_min) + ' bits, ' + str(bits_pref) + ' bits and ' + str(bits_max) + ' bits...', write_now=True)
+
+                # It has been observed that reconnecting to some SSH servers
+                # multiple times in quick succession can eventually result
+                # in a "connection reset by peer" error. It may be possible
+                # to recover from such an error by sleeping for some time
+                # before continuing to issue reconnects.
+                if GEXTest.reconnect(out, s, kex, gex_alg) is False:
+                    out.fail('Reconnect failed.')
+                    return exitcodes.FAILURE
+                try:
+                    modulus_size_returned = None
+                    kex_group.send_init_gex(s, bits_min, bits_pref, bits_max)
+                    kex_group.recv_reply(s, False)
+                    modulus_size_returned = kex_group.get_dh_modulus_size()
+                    out.d('Modulus size returned by server: ' + str(modulus_size_returned) + ' bits', write_now=True)
+                except KexDHException:
+                    out.d('[exception] ' + str(traceback.format_exc()), write_now=True)
+                finally:
+                    # The server is in a state that is not re-testable,
+                    # so there's nothing else to do with this open
+                    # connection.
+                    s.close()
+
+                if modulus_size_returned is not None:
+                    if gex_alg in modulus_dict:
+                        if modulus_size_returned not in modulus_dict[gex_alg]:
+                            modulus_dict[gex_alg].append(modulus_size_returned)
+                    else:
+                        modulus_dict[gex_alg] = [modulus_size_returned]
 
-        if kex_str is not None and kex_group is not None:
-            HostKeyTest.perform_test(out, s, server_kex, kex_str, kex_group, HostKeyTest.HOST_KEY_TYPES)
+        return retval
 
+    # Runs the DH moduli test against the specified target.
     @staticmethod
-    def perform_test(out: 'OutputBuffer', s: 'SSH_Socket', server_kex: 'SSH2_Kex', kex_str: str, kex_group: 'KexDH', host_key_types: Dict[str, Dict[str, bool]]) -> None:
-        hostkey_modulus_size = 0
-        ca_modulus_size = 0
-
-        # If the connection still exists, close it so we can test
-        # using a clean slate (otherwise it may exist in a non-testable
-        # state).
+    def run(out: 'OutputBuffer', s: 'SSH_Socket', kex: 'SSH2_Kex') -> None:
+        GEX_ALGS = {
+            'diffie-hellman-group-exchange-sha1': KexGroupExchange_SHA1,
+            'diffie-hellman-group-exchange-sha256': KexGroupExchange_SHA256,
+        }
+
+        # The previous RSA tests put the server in a state we can't
+        # test.  So we need a new connection to start with a clean
+        # slate.
         if s.is_connected():
             s.close()
 
-        # For each host key type...
-        for host_key_type in host_key_types:
-            # Skip those already handled (i.e.: those in the RSA family, as testing one tests them all).
-            if 'parsed' in host_key_types[host_key_type] and host_key_types[host_key_type]['parsed']:
-                continue
-
-            # If this host key type is supported by the server, we test it.
-            if host_key_type in server_kex.key_algorithms:
-                out.d('Preparing to obtain ' + host_key_type + ' host key...', write_now=True)
-
-                cert = host_key_types[host_key_type]['cert']
-                variable_key_len = host_key_types[host_key_type]['variable_key_len']
-
-                # If the connection is closed, re-open it and get the kex again.
-                if not s.is_connected():
-                    err = s.connect()
-                    if err is not None:
-                        out.v(err, write_now=True)
-                        return
-
-                    _, _, err = s.get_banner()
-                    if err is not None:
-                        out.v(err, write_now=True)
-                        s.close()
-                        return
+        # Check if the server supports any of the group-exchange
+        # algorithms.  If so, test each one.
+        for gex_alg, kex_group_class in GEX_ALGS.items():
+            if gex_alg in kex.kex_algorithms:
+                out.d('Preparing to perform DH group exchange using ' + gex_alg + ' with min, pref and max modulus sizes of 512 bits, 1024 bits and 1536 bits...', write_now=True)
 
-                    # Send our KEX using the specified group-exchange and most of the server's own values.
-                    s.send_kexinit(key_exchanges=[kex_str], hostkeys=[host_key_type], ciphers=server_kex.server.encryption, macs=server_kex.server.mac, compressions=server_kex.server.compression, languages=server_kex.server.languages)
+                if GEXTest.reconnect(out, s, kex, gex_alg) is False:
+                    break
 
-                    try:
-                        # Parse the server's KEX.
-                        _, payload = s.read_packet()
-                        SSH2_Kex.parse(payload)
-                    except Exception:
-                        out.v("Failed to parse server's kex.  Stack trace:\n%s" % str(traceback.format_exc()), write_now=True)
-                        return
-
-                # Do the initial DH exchange.  The server responds back
-                # with the host key and its length.  Bingo.  We also get back the host key fingerprint.
-                kex_group.send_init(s)
+                kex_group = kex_group_class(out)
+                smallest_modulus = -1
+
+                # First try a range of weak sizes.
                 try:
-                    host_key = kex_group.recv_reply(s, variable_key_len)
-                    if host_key is not None:
-                        server_kex.set_host_key(host_key_type, host_key)
-                except Exception:
-                    pass
-
-                hostkey_modulus_size = kex_group.get_hostkey_size()
-                ca_modulus_size = kex_group.get_ca_size()
-
-                # Close the socket, as the connection has
-                # been put in a state that later tests can't use.
-                s.close()
-
-                # If the host key modulus or CA modulus was successfully parsed, check to see that its a safe size.
-                if hostkey_modulus_size > 0 or ca_modulus_size > 0:
-                    # Set the hostkey size for all RSA key types since 'ssh-rsa',
-                    # 'rsa-sha2-256', etc. are all using the same host key.
-                    # Note, however, that this may change in the future.
-                    if cert is False and host_key_type in HostKeyTest.RSA_FAMILY:
-                        for rsa_type in HostKeyTest.RSA_FAMILY:
-                            server_kex.set_rsa_key_size(rsa_type, hostkey_modulus_size)
-                    elif cert is True:
-                        server_kex.set_rsa_key_size(host_key_type, hostkey_modulus_size, ca_modulus_size)
-
-                    # Keys smaller than 2048 result in a failure.  Update the database accordingly.
-                    if (cert is False) and (hostkey_modulus_size < 2048):
-                        for rsa_type in HostKeyTest.RSA_FAMILY:
-                            alg_list = SSH2_KexDB.ALGORITHMS['key'][rsa_type]
-
-                            # If no failure list exists, add an empty failure list.
-                            if len(alg_list) < 2:
-                                alg_list.append([])
-                            alg_list[1].append('using small %d-bit modulus' % hostkey_modulus_size)
-                    elif (cert is True) and ((hostkey_modulus_size < 2048) or (ca_modulus_size > 0 and ca_modulus_size < 2048)):  # pylint: disable=chained-comparison
-                        alg_list = SSH2_KexDB.ALGORITHMS['key'][host_key_type]
-                        min_modulus = min(hostkey_modulus_size, ca_modulus_size)
-                        min_modulus = min_modulus if min_modulus > 0 else max(hostkey_modulus_size, ca_modulus_size)
-
-                        # If no failure list exists, add an empty failure list.
-                        if len(alg_list) < 2:
-                            alg_list.append([])
-                        alg_list[1].append('using small %d-bit modulus' % min_modulus)
-
-                # If this host key type is in the RSA family, then mark them all as parsed (since results in one are valid for them all).
-                if host_key_type in HostKeyTest.RSA_FAMILY:
-                    for rsa_type in HostKeyTest.RSA_FAMILY:
-                        host_key_types[rsa_type]['parsed'] = True
-                else:
-                    host_key_types[host_key_type]['parsed'] = True
+                    kex_group.send_init_gex(s, 512, 1024, 1536)
+                    kex_group.recv_reply(s, False)
+
+                    # Its been observed that servers will return a group
+                    # larger than the requested max.  So just because we
+                    # got here, doesn't mean the server is vulnerable...
+                    smallest_modulus = kex_group.get_dh_modulus_size()
+                    out.d('Modulus size returned by server: ' + str(smallest_modulus) + ' bits', write_now=True)
+
+                except KexDHException:
+                    out.d('[exception] ' + str(traceback.format_exc()), write_now=True)
+                finally:
+                    s.close()
+
+                # Try an array of specific modulus sizes... one at a time.
+                reconnect_failed = False
+                for bits in [512, 768, 1024, 1536, 2048, 3072, 4096]:
+
+                    # If we found one modulus size already, but we're about
+                    # to test a larger one, don't bother.
+                    if bits >= smallest_modulus > 0:
+                        break
+
+                    out.d('Preparing to perform DH group exchange using ' + gex_alg + ' with min, pref and max modulus sizes of ' + str(bits) + ' bits...', write_now=True)
+
+                    if GEXTest.reconnect(out, s, kex, gex_alg) is False:
+                        reconnect_failed = True
+                        break
+
+                    try:
+                        kex_group.send_init_gex(s, bits, bits, bits)
+                        kex_group.recv_reply(s, False)
+                        smallest_modulus = kex_group.get_dh_modulus_size()
+                        out.d('Modulus size returned by server: ' + str(smallest_modulus) + ' bits', write_now=True)
+                    except KexDHException as e:
+                        out.d('Exception when testing DH group exchange ' + gex_alg + ' with modulus size ' + str(bits) + '.  (Hint: this is probably normal since the server does not support this modulus size.): ' + str(e), write_now=True)
+                    finally:
+                        # The server is in a state that is not re-testable,
+                        # so there's nothing else to do with this open
+                        # connection.
+                        s.close()
+
+                if smallest_modulus > 0:
+                    kex.set_dh_modulus_size(gex_alg, smallest_modulus)
+
+                    # We flag moduli smaller than 2048 as a failure.
+                    if smallest_modulus < 2048:
+                        text = 'using small %d-bit modulus' % smallest_modulus
+                        lst = SSH2_KexDB.ALGORITHMS['kex'][gex_alg]
+                        # For 'diffie-hellman-group-exchange-sha256', add
+                        # a failure reason.
+                        if len(lst) == 1:
+                            lst.append([text])
+                        # For 'diffie-hellman-group-exchange-sha1', delete
+                        # the existing failure reason (which is vague), and
+                        # insert our own.
+                        else:
+                            del lst[1]
+                            lst.insert(1, [text])
+
+                    # Moduli smaller than 3072 get flagged as a warning.
+                    elif smallest_modulus < 3072:
+                        lst = SSH2_KexDB.ALGORITHMS['kex'][gex_alg]
+
+                        # Ensure that a warning list exists for us to append to, below.
+                        while len(lst) < 3:
+                            lst.append([])
+
+                        # Ensure this is only added once.
+                        text = '2048-bit modulus only provides 112-bits of symmetric strength'
+                        if text not in lst[2]:
+                            lst[2].append(text)
+
+                if reconnect_failed:
+                    break
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/kexdh.py` & `ssh-audit-2.9.0/src/ssh_audit/kexdh.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
    The MIT License (MIT)
 
-   Copyright (C) 2017-2021 Joe Testa (jtesta@positronsecurity.com)
+   Copyright (C) 2017-2023 Joe Testa (jtesta@positronsecurity.com)
    Copyright (C) 2017 Andris Raugulis (moo@arthepsy.eu)
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
@@ -27,34 +27,41 @@
 import random
 import struct
 
 # pylint: disable=unused-import
 from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
 from typing import Callable, Optional, Union, Any  # noqa: F401
 
+from ssh_audit.outputbuffer import OutputBuffer
 from ssh_audit.protocol import Protocol
 from ssh_audit.ssh_socket import SSH_Socket
 
 
+class KexDHException(Exception):
+    pass
+
+
 class KexDH:  # pragma: nocover
-    def __init__(self, kex_name: str, hash_alg: str, g: int, p: int) -> None:
+    def __init__(self, out: 'OutputBuffer', kex_name: str, hash_alg: str, g: int, p: int) -> None:
+        self.out = out
         self.__kex_name = kex_name  # pylint: disable=unused-private-member
         self.__hash_alg = hash_alg  # pylint: disable=unused-private-member
         self.__g = 0
         self.__p = 0
         self.__q = 0
         self.__x = 0
         self.__e = 0
         self.set_params(g, p)
 
         self.__ed25519_pubkey: Optional[bytes] = None  # pylint: disable=unused-private-member
-        self.__hostkey_type: Optional[bytes] = None
+        self.__hostkey_type = ''
         self.__hostkey_e = 0  # pylint: disable=unused-private-member
         self.__hostkey_n = 0  # pylint: disable=unused-private-member
         self.__hostkey_n_len = 0  # Length of the host key modulus.
+        self.__ca_key_type = ''  # Type of CA key ('ssh-rsa', etc).
         self.__ca_n_len = 0  # Length of the CA key modulus (if hostkey is a cert).
 
     def set_params(self, g: int, p: int) -> None:
         self.__g = g
         self.__p = p
         self.__q = (self.__p - 1) // 2
         self.__x = 0
@@ -68,124 +75,150 @@
         s.write_mpint2(self.__e)
         s.send_packet()
 
     # Parse a KEXDH_REPLY or KEXDH_GEX_REPLY message from the server.  This
     # contains the host key, among other things.  Function returns the host
     # key blob (from which the fingerprint can be calculated).
     def recv_reply(self, s: 'SSH_Socket', parse_host_key_size: bool = True) -> Optional[bytes]:
+        # Reset the CA info, in case it was set from a prior invokation.
+        self.__hostkey_type = ''
+        self.__hostkey_e = 0  # pylint: disable=unused-private-member
+        self.__hostkey_n = 0  # pylint: disable=unused-private-member
+        self.__hostkey_n_len = 0
+        self.__ca_key_type = ''
+        self.__ca_n_len = 0
+
         packet_type, payload = s.read_packet(2)
 
         # Skip any & all MSG_DEBUG messages.
         while packet_type == Protocol.MSG_DEBUG:
             packet_type, payload = s.read_packet(2)
 
         if packet_type != -1 and packet_type not in [Protocol.MSG_KEXDH_REPLY, Protocol.MSG_KEXDH_GEX_REPLY]:  # pylint: disable=no-else-raise
-            # TODO: change Exception to something more specific.
-            raise Exception('Expected MSG_KEXDH_REPLY (%d) or MSG_KEXDH_GEX_REPLY (%d), but got %d instead.' % (Protocol.MSG_KEXDH_REPLY, Protocol.MSG_KEXDH_GEX_REPLY, packet_type))
+            raise KexDHException('Expected MSG_KEXDH_REPLY (%d) or MSG_KEXDH_GEX_REPLY (%d), but got %d instead.' % (Protocol.MSG_KEXDH_REPLY, Protocol.MSG_KEXDH_GEX_REPLY, packet_type))
         elif packet_type == -1:
             # A connection error occurred.  We can't parse anything, so just
             # return.  The host key modulus (and perhaps certificate modulus)
             # will remain at length 0.
+            self.out.d("KexDH.recv_reply(): received packge_type == -1.")
             return None
 
-        hostkey_len = 0  # pylint: disable=unused-variable
-        hostkey_type_len = hostkey_e_len = 0  # pylint: disable=unused-variable
-        key_id_len = principles_len = 0  # pylint: disable=unused-variable
-        critical_options_len = extensions_len = 0  # pylint: disable=unused-variable
-        nonce_len = ca_key_len = ca_key_type_len = 0  # pylint: disable=unused-variable
-        ca_key_len = ca_key_type_len = ca_key_e_len = 0  # pylint: disable=unused-variable
-
-        key_id = principles = None  # pylint: disable=unused-variable
-        critical_options = extensions = None  # pylint: disable=unused-variable
-        nonce = ca_key = ca_key_type = None  # pylint: disable=unused-variable
-        ca_key_e = ca_key_n = None  # pylint: disable=unused-variable
-
         # Get the host key blob, F, and signature.
         ptr = 0
-        hostkey, hostkey_len, ptr = KexDH.__get_bytes(payload, ptr)
+        hostkey, _, ptr = KexDH.__get_bytes(payload, ptr)
 
         # If we are not supposed to parse the host key size (i.e.: it is a type that is of fixed size such as ed25519), then stop here.
         if not parse_host_key_size:
             return hostkey
 
         _, _, ptr = KexDH.__get_bytes(payload, ptr)
         _, _, ptr = KexDH.__get_bytes(payload, ptr)
 
         # Now pick apart the host key blob.
         # Get the host key type (i.e.: 'ssh-rsa', 'ssh-ed25519', etc).
         ptr = 0
-        self.__hostkey_type, hostkey_type_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+        hostkey_type, _, ptr = KexDH.__get_bytes(hostkey, ptr)
+        self.__hostkey_type = hostkey_type.decode('ascii')
+        self.out.d("Parsing host key type: %s" % self.__hostkey_type)
 
         # If this is an RSA certificate, skip over the nonce.
-        if self.__hostkey_type.startswith(b'ssh-rsa-cert-v0'):
-            nonce, nonce_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+        if self.__hostkey_type.startswith('ssh-rsa-cert-v0'):
+            self.out.d("RSA certificate found, so skipping nonce.")
+            _, _, ptr = KexDH.__get_bytes(hostkey, ptr)  # Read & skip over the nonce.
 
         # The public key exponent.
-        hostkey_e, hostkey_e_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+        hostkey_e, _, ptr = KexDH.__get_bytes(hostkey, ptr)
         self.__hostkey_e = int(binascii.hexlify(hostkey_e), 16)  # pylint: disable=unused-private-member
 
-        # Here is the modulus size & actual modulus of the host key public key.
-        hostkey_n, self.__hostkey_n_len, ptr = KexDH.__get_bytes(hostkey, ptr)
-        self.__hostkey_n = int(binascii.hexlify(hostkey_n), 16)  # pylint: disable=unused-private-member
-
-        # If this is an RSA certificate, continue parsing to extract the CA
-        # key.
-        if self.__hostkey_type.startswith(b'ssh-rsa-cert-v0'):
-            # Skip over the serial number.
-            ptr += 8
-
-            # Get the certificate type.
-            cert_type = int(binascii.hexlify(hostkey[ptr:ptr + 4]), 16)
-            ptr += 4
+        # ED25519 moduli are fixed at 32 bytes.
+        if self.__hostkey_type == 'ssh-ed25519':
+            self.out.d("%s has a fixed host key modulus of 32." % self.__hostkey_type)
+            self.__hostkey_n_len = 32
+        else:
+            # Here is the modulus size & actual modulus of the host key public key.
+            hostkey_n, self.__hostkey_n_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+            self.__hostkey_n = int(binascii.hexlify(hostkey_n), 16)  # pylint: disable=unused-private-member
+
+        # If this is a certificate, continue parsing to extract the CA type and key length.  Even though a hostkey type might be 'ssh-ed25519-cert-v01@openssh.com', its CA may still be RSA.
+        if self.__hostkey_type.startswith('ssh-rsa-cert-v0') or self.__hostkey_type.startswith('ssh-ed25519-cert-v0'):
+            # Get the CA key type and key length.
+            self.__ca_key_type, self.__ca_n_len = self.__parse_ca_key(hostkey, self.__hostkey_type, ptr)
+            self.out.d("KexDH.__parse_ca_key(): CA key type: [%s]; CA key length: %u" % (self.__ca_key_type, self.__ca_n_len))
 
-            # Only SSH2_CERT_TYPE_HOST (2) makes sense in this context.
-            if cert_type == 2:
+        return hostkey
 
-                # Skip the key ID (this is the serial number of the
-                # certificate).
-                key_id, key_id_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+    def __parse_ca_key(self, hostkey: bytes, hostkey_type: str, ptr: int) -> Tuple[str, int]:
+        ca_key_type = ''
+        ca_key_n_len = 0
+
+        # If this is a certificate, continue parsing to extract the CA type and key length.  Even though a hostkey type might be 'ssh-ed25519-cert-v01@openssh.com', its CA may still be RSA.
+        # if hostkey_type.startswith('ssh-rsa-cert-v0') or hostkey_type.startswith('ssh-ed25519-cert-v0'):
+        self.out.d("Parsing CA for hostkey type [%s]..." % hostkey_type)
 
-                # The principles, which are... I don't know what.
-                principles, principles_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+        # Skip over the serial number.
+        ptr += 8
 
-                # Skip over the timestamp that this certificate is valid after.
-                ptr += 8
+        # Get the certificate type.
+        cert_type = int(binascii.hexlify(hostkey[ptr:ptr + 4]), 16)
+        ptr += 4
 
-                # Skip over the timestamp that this certificate is valid before.
-                ptr += 8
+        # Only SSH2_CERT_TYPE_HOST (2) makes sense in this context.
+        if cert_type == 2:
 
-                # TODO: validate the principles, and time range.
+            # Skip the key ID (this is the serial number of the
+            # certificate).
+            key_id, key_id_len, ptr = KexDH.__get_bytes(hostkey, ptr)  # pylint: disable=unused-variable
 
-                # The critical options.
-                critical_options, critical_options_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+            # The principles, which are... I don't know what.
+            principles, principles_len, ptr = KexDH.__get_bytes(hostkey, ptr)  # pylint: disable=unused-variable
 
-                # Certificate extensions.
-                extensions, extensions_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+            # Skip over the timestamp that this certificate is valid after.
+            ptr += 8
 
-                # Another nonce.
-                nonce, nonce_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+            # Skip over the timestamp that this certificate is valid before.
+            ptr += 8
 
-                # Finally, we get to the CA key.
-                ca_key, ca_key_len, ptr = KexDH.__get_bytes(hostkey, ptr)
+            # TODO: validate the principles, and time range.
 
-                # Last in the host key blob is the CA signature.  It isn't
-                # interesting to us, so we won't bother parsing any further.
-                # The CA key has the modulus, however...
-                ptr = 0
+            # The critical options.
+            critical_options, critical_options_len, ptr = KexDH.__get_bytes(hostkey, ptr)  # pylint: disable=unused-variable
 
-                # 'ssh-rsa', 'rsa-sha2-256', etc.
-                ca_key_type, ca_key_type_len, ptr = KexDH.__get_bytes(ca_key, ptr)
+            # Certificate extensions.
+            extensions, extensions_len, ptr = KexDH.__get_bytes(hostkey, ptr)  # pylint: disable=unused-variable
 
+            # Another nonce.
+            nonce, nonce_len, ptr = KexDH.__get_bytes(hostkey, ptr)  # pylint: disable=unused-variable
+
+            # Finally, we get to the CA key.
+            ca_key, ca_key_len, ptr = KexDH.__get_bytes(hostkey, ptr)  # pylint: disable=unused-variable
+
+            # Last in the host key blob is the CA signature.  It isn't
+            # interesting to us, so we won't bother parsing any further.
+            # The CA key has the modulus, however...
+            ptr = 0
+
+            # 'ssh-rsa', 'rsa-sha2-256', etc.
+            ca_key_type_bytes, ca_key_type_len, ptr = KexDH.__get_bytes(ca_key, ptr)  # pylint: disable=unused-variable
+            ca_key_type = ca_key_type_bytes.decode('ascii')
+            self.out.d("Found CA type: [%s]" % ca_key_type)
+
+            # ED25519 CA's don't explicitly include the modulus size in the public key, since its fixed at 32 in all cases.
+            if ca_key_type == 'ssh-ed25519':
+                ca_key_n_len = 32
+            else:
                 # CA's public key exponent.
-                ca_key_e, ca_key_e_len, ptr = KexDH.__get_bytes(ca_key, ptr)
+                ca_key_e, ca_key_e_len, ptr = KexDH.__get_bytes(ca_key, ptr)  # pylint: disable=unused-variable
 
                 # CA's modulus.  Bingo.
-                ca_key_n, self.__ca_n_len, ptr = KexDH.__get_bytes(ca_key, ptr)
+                ca_key_n, ca_key_n_len, ptr = KexDH.__get_bytes(ca_key, ptr)  # pylint: disable=unused-variable
 
-        return hostkey
+        else:
+            self.out.d("Certificate type %u found; this is not usually valid in the context of a host key!  Skipping it..." % cert_type)
+
+        return ca_key_type, ca_key_n_len
 
     @staticmethod
     def __get_bytes(buf: bytes, ptr: int) -> Tuple[bytes, int, int]:
         num_bytes = struct.unpack('>I', buf[ptr:ptr + 4])[0]
         ptr += 4
         return buf[ptr:ptr + num_bytes], num_bytes, ptr + num_bytes
 
@@ -198,119 +231,127 @@
         # (i.e.: 1024-bit keys have a 1032-bit modulus).  Check if this is
         # the case, and subtract 8 if so.  This simply improves readability
         # in the UI.
         if (size >> 3) % 2 != 0:
             size = size - 8
         return size
 
+    # Returns the hostkey type.
+    def get_hostkey_type(self) -> str:
+        return self.__hostkey_type
+
     # Returns the size of the hostkey, in bits.
     def get_hostkey_size(self) -> int:
         return KexDH.__adjust_key_size(self.__hostkey_n_len)
 
+    # Returns the CA type ('ssh-rsa', 'ssh-ed25519', etc).
+    def get_ca_type(self) -> str:
+        return self.__ca_key_type
+
     # Returns the size of the CA key, in bits.
     def get_ca_size(self) -> int:
         return KexDH.__adjust_key_size(self.__ca_n_len)
 
     # Returns the size of the DH modulus, in bits.
     def get_dh_modulus_size(self) -> int:
         # -2 to account for the '0b' prefix in the string.
         return len(bin(self.__p)) - 2
 
 
 class KexGroup1(KexDH):  # pragma: nocover
-    def __init__(self) -> None:
+    def __init__(self, out: 'OutputBuffer') -> None:
         # rfc2409: second oakley group
         p = int('ffffffffffffffffc90fdaa22168c234c4c6628b80dc1cd129024e088a67cc74020bbea63b139b22514a08798e3404ddef9519b3cd3a431b302b0a6df25f14374fe1356d6d51c245e485b576625e7ec6f44c42e9a637ed6b0bff5cb6f406b7edee386bfb5a899fa5ae9f24117c4b1fe649286651ece65381ffffffffffffffff', 16)
-        super(KexGroup1, self).__init__('KexGroup1', 'sha1', 2, p)
+        super(KexGroup1, self).__init__(out, 'KexGroup1', 'sha1', 2, p)
 
 
 class KexGroup14(KexDH):  # pragma: nocover
-    def __init__(self, hash_alg: str) -> None:
+    def __init__(self, out: 'OutputBuffer', hash_alg: str) -> None:
         # rfc3526: 2048-bit modp group
         p = int('ffffffffffffffffc90fdaa22168c234c4c6628b80dc1cd129024e088a67cc74020bbea63b139b22514a08798e3404ddef9519b3cd3a431b302b0a6df25f14374fe1356d6d51c245e485b576625e7ec6f44c42e9a637ed6b0bff5cb6f406b7edee386bfb5a899fa5ae9f24117c4b1fe649286651ece45b3dc2007cb8a163bf0598da48361c55d39a69163fa8fd24cf5f83655d23dca3ad961c62f356208552bb9ed529077096966d670c354e4abc9804f1746c08ca18217c32905e462e36ce3be39e772c180e86039b2783a2ec07a28fb5c55df06f4c52c9de2bcbf6955817183995497cea956ae515d2261898fa051015728e5a8aacaa68ffffffffffffffff', 16)
-        super(KexGroup14, self).__init__('KexGroup14', hash_alg, 2, p)
+        super(KexGroup14, self).__init__(out, 'KexGroup14', hash_alg, 2, p)
 
 
 class KexGroup14_SHA1(KexGroup14):
-    def __init__(self) -> None:
-        super(KexGroup14_SHA1, self).__init__('sha1')
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexGroup14_SHA1, self).__init__(out, 'sha1')
 
 
 class KexGroup14_SHA256(KexGroup14):
-    def __init__(self) -> None:
-        super(KexGroup14_SHA256, self).__init__('sha256')
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexGroup14_SHA256, self).__init__(out, 'sha256')
 
 
 class KexGroup16_SHA512(KexDH):
-    def __init__(self) -> None:
+    def __init__(self, out: 'OutputBuffer') -> None:
         # rfc3526: 4096-bit modp group
         p = int('ffffffffffffffffc90fdaa22168c234c4c6628b80dc1cd129024e088a67cc74020bbea63b139b22514a08798e3404ddef9519b3cd3a431b302b0a6df25f14374fe1356d6d51c245e485b576625e7ec6f44c42e9a637ed6b0bff5cb6f406b7edee386bfb5a899fa5ae9f24117c4b1fe649286651ece45b3dc2007cb8a163bf0598da48361c55d39a69163fa8fd24cf5f83655d23dca3ad961c62f356208552bb9ed529077096966d670c354e4abc9804f1746c08ca18217c32905e462e36ce3be39e772c180e86039b2783a2ec07a28fb5c55df06f4c52c9de2bcbf6955817183995497cea956ae515d2261898fa051015728e5a8aaac42dad33170d04507a33a85521abdf1cba64ecfb850458dbef0a8aea71575d060c7db3970f85a6e1e4c7abf5ae8cdb0933d71e8c94e04a25619dcee3d2261ad2ee6bf12ffa06d98a0864d87602733ec86a64521f2b18177b200cbbe117577a615d6c770988c0bad946e208e24fa074e5ab3143db5bfce0fd108e4b82d120a92108011a723c12a787e6d788719a10bdba5b2699c327186af4e23c1a946834b6150bda2583e9ca2ad44ce8dbbbc2db04de8ef92e8efc141fbecaa6287c59474e6bc05d99b2964fa090c3a2233ba186515be7ed1f612970cee2d7afb81bdd762170481cd0069127d5b05aa993b4ea988d8fddc186ffb7dc90a6c08f4df435c934063199ffffffffffffffff', 16)
-        super(KexGroup16_SHA512, self).__init__('KexGroup16_SHA512', 'sha512', 2, p)
+        super(KexGroup16_SHA512, self).__init__(out, 'KexGroup16_SHA512', 'sha512', 2, p)
 
 
 class KexGroup18_SHA512(KexDH):
-    def __init__(self) -> None:
+    def __init__(self, out: 'OutputBuffer') -> None:
         # rfc3526: 8192-bit modp group
         p = int('ffffffffffffffffc90fdaa22168c234c4c6628b80dc1cd129024e088a67cc74020bbea63b139b22514a08798e3404ddef9519b3cd3a431b302b0a6df25f14374fe1356d6d51c245e485b576625e7ec6f44c42e9a637ed6b0bff5cb6f406b7edee386bfb5a899fa5ae9f24117c4b1fe649286651ece45b3dc2007cb8a163bf0598da48361c55d39a69163fa8fd24cf5f83655d23dca3ad961c62f356208552bb9ed529077096966d670c354e4abc9804f1746c08ca18217c32905e462e36ce3be39e772c180e86039b2783a2ec07a28fb5c55df06f4c52c9de2bcbf6955817183995497cea956ae515d2261898fa051015728e5a8aaac42dad33170d04507a33a85521abdf1cba64ecfb850458dbef0a8aea71575d060c7db3970f85a6e1e4c7abf5ae8cdb0933d71e8c94e04a25619dcee3d2261ad2ee6bf12ffa06d98a0864d87602733ec86a64521f2b18177b200cbbe117577a615d6c770988c0bad946e208e24fa074e5ab3143db5bfce0fd108e4b82d120a92108011a723c12a787e6d788719a10bdba5b2699c327186af4e23c1a946834b6150bda2583e9ca2ad44ce8dbbbc2db04de8ef92e8efc141fbecaa6287c59474e6bc05d99b2964fa090c3a2233ba186515be7ed1f612970cee2d7afb81bdd762170481cd0069127d5b05aa993b4ea988d8fddc186ffb7dc90a6c08f4df435c93402849236c3fab4d27c7026c1d4dcb2602646dec9751e763dba37bdf8ff9406ad9e530ee5db382f413001aeb06a53ed9027d831179727b0865a8918da3edbebcf9b14ed44ce6cbaced4bb1bdb7f1447e6cc254b332051512bd7af426fb8f401378cd2bf5983ca01c64b92ecf032ea15d1721d03f482d7ce6e74fef6d55e702f46980c82b5a84031900b1c9e59e7c97fbec7e8f323a97a7e36cc88be0f1d45b7ff585ac54bd407b22b4154aacc8f6d7ebf48e1d814cc5ed20f8037e0a79715eef29be32806a1d58bb7c5da76f550aa3d8a1fbff0eb19ccb1a313d55cda56c9ec2ef29632387fe8d76e3c0468043e8f663f4860ee12bf2d5b0b7474d6e694f91e6dbe115974a3926f12fee5e438777cb6a932df8cd8bec4d073b931ba3bc832b68d9dd300741fa7bf8afc47ed2576f6936ba424663aab639c5ae4f5683423b4742bf1c978238f16cbe39d652de3fdb8befc848ad922222e04a4037c0713eb57a81a23f0c73473fc646cea306b4bcbc8862f8385ddfa9d4b7fa2c087e879683303ed5bdd3a062b3cf5b3a278a66d2a13f83f44f82ddf310ee074ab6a364597e899a0255dc164f31cc50846851df9ab48195ded7ea1b1d510bd7ee74d73faf36bc31ecfa268359046f4eb879f924009438b481c6cd7889a002ed5ee382bc9190da6fc026e479558e4475677e9aa9e3050e2765694dfc81f56e880b96e7160c980dd98edd3dfffffffffffffffff', 16)
-        super(KexGroup18_SHA512, self).__init__('KexGroup18_SHA512', 'sha512', 2, p)
+        super(KexGroup18_SHA512, self).__init__(out, 'KexGroup18_SHA512', 'sha512', 2, p)
 
 
 class KexCurve25519_SHA256(KexDH):
-    def __init__(self) -> None:
-        super(KexCurve25519_SHA256, self).__init__('KexCurve25519_SHA256', 'sha256', 0, 0)
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexCurve25519_SHA256, self).__init__(out, 'KexCurve25519_SHA256', 'sha256', 0, 0)
 
     # To start an ED25519 kex, we simply send a random 256-bit number as the
     # public key.
     def send_init(self, s: 'SSH_Socket', init_msg: int = Protocol.MSG_KEXDH_INIT) -> None:
         self.__ed25519_pubkey = os.urandom(32)
         s.write_byte(init_msg)
         s.write_string(self.__ed25519_pubkey)
         s.send_packet()
 
 
 class KexNISTP256(KexDH):
-    def __init__(self) -> None:
-        super(KexNISTP256, self).__init__('KexNISTP256', 'sha256', 0, 0)
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexNISTP256, self).__init__(out, 'KexNISTP256', 'sha256', 0, 0)
 
     # Because the server checks that the value sent here is valid (i.e.: it lies
     # on the curve, among other things), we would have to write a lot of code
     # or import an elliptic curve library in order to randomly generate a
     # valid elliptic point each time.  Hence, we will simply send a static
     # value, which is enough for us to extract the server's host key.
     def send_init(self, s: 'SSH_Socket', init_msg: int = Protocol.MSG_KEXDH_INIT) -> None:
         s.write_byte(init_msg)
         s.write_string(b'\x04\x0b\x60\x44\x9f\x8a\x11\x9e\xc7\x81\x0c\xa9\x98\xfc\xb7\x90\xaa\x6b\x26\x8c\x12\x4a\xc0\x09\xbb\xdf\xc4\x2c\x4c\x2c\x99\xb6\xe1\x71\xa0\xd4\xb3\x62\x47\x74\xb3\x39\x0c\xf2\x88\x4a\x84\x6b\x3b\x15\x77\xa5\x77\xd2\xa9\xc9\x94\xf9\xd5\x66\x19\xcd\x02\x34\xd1')
         s.send_packet()
 
 
 class KexNISTP384(KexDH):
-    def __init__(self) -> None:
-        super(KexNISTP384, self).__init__('KexNISTP384', 'sha256', 0, 0)
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexNISTP384, self).__init__(out, 'KexNISTP384', 'sha256', 0, 0)
 
     # See comment for KexNISTP256.send_init().
     def send_init(self, s: 'SSH_Socket', init_msg: int = Protocol.MSG_KEXDH_INIT) -> None:
         s.write_byte(init_msg)
         s.write_string(b'\x04\xe2\x9b\x84\xce\xa1\x39\x50\xfe\x1e\xa3\x18\x70\x1c\xe2\x7a\xe4\xb5\x6f\xdf\x93\x9f\xd4\xf4\x08\xcc\x9b\x02\x10\xa4\xca\x77\x9c\x2e\x51\x44\x1d\x50\x7a\x65\x4e\x7e\x2f\x10\x2d\x2d\x4a\x32\xc9\x8e\x18\x75\x90\x6c\x19\x10\xda\xcc\xa8\xe9\xf4\xc4\x3a\x53\x80\x35\xf4\x97\x9c\x04\x16\xf9\x5a\xdc\xcc\x05\x94\x29\xfa\xc4\xd6\x87\x4e\x13\x21\xdb\x3d\x12\xac\xbd\x20\x3b\x60\xff\xe6\x58\x42')
         s.send_packet()
 
 
 class KexNISTP521(KexDH):
-    def __init__(self) -> None:
-        super(KexNISTP521, self).__init__('KexNISTP521', 'sha256', 0, 0)
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexNISTP521, self).__init__(out, 'KexNISTP521', 'sha256', 0, 0)
 
     # See comment for KexNISTP256.send_init().
     def send_init(self, s: 'SSH_Socket', init_msg: int = Protocol.MSG_KEXDH_INIT) -> None:
         s.write_byte(init_msg)
         s.write_string(b'\x04\x01\x02\x90\x29\xe9\x8f\xa8\x04\xaf\x1c\x00\xf9\xc6\x29\xc0\x39\x74\x8e\xea\x47\x7e\x7c\xf7\x15\x6e\x43\x3b\x59\x13\x53\x43\xb0\xae\x0b\xe7\xe6\x7c\x55\x73\x52\xa5\x2a\xc1\x42\xde\xfc\xf4\x1f\x8b\x5a\x8d\xfa\xcd\x0a\x65\x77\xa8\xce\x68\xd2\xc6\x26\xb5\x3f\xee\x4b\x01\x7b\xd2\x96\x23\x69\x53\xc7\x01\xe1\x0d\x39\xe9\x87\x49\x3b\xc8\xec\xda\x0c\xf9\xca\xad\x89\x42\x36\x6f\x93\x78\x78\x31\x55\x51\x09\x51\xc0\x96\xd7\xea\x61\xbf\xc2\x44\x08\x80\x43\xed\xc6\xbb\xfb\x94\xbd\xf8\xdf\x2b\xd8\x0b\x2e\x29\x1b\x8c\xc4\x8a\x04\x2d\x3a')
         s.send_packet()
 
 
 class KexGroupExchange(KexDH):
-    def __init__(self, classname: str, hash_alg: str) -> None:
-        super(KexGroupExchange, self).__init__(classname, hash_alg, 0, 0)
+    def __init__(self, out: 'OutputBuffer', classname: str, hash_alg: str) -> None:
+        super(KexGroupExchange, self).__init__(out, classname, hash_alg, 0, 0)
 
     def send_init(self, s: 'SSH_Socket', init_msg: int = Protocol.MSG_KEXDH_GEX_REQUEST) -> None:
         self.send_init_gex(s)
 
     # The group exchange starts with sending a message to the server with
     # the minimum, maximum, and preferred number of bits are for the DH group.
     # The server responds with a generator and prime modulus that matches that,
@@ -324,16 +365,15 @@
         s.write_int(minbits)
         s.write_int(prefbits)
         s.write_int(maxbits)
         s.send_packet()
 
         packet_type, payload = s.read_packet(2)
         if packet_type not in [Protocol.MSG_KEXDH_GEX_GROUP, Protocol.MSG_DEBUG]:
-            # TODO: replace with a better exception type.
-            raise Exception('Expected MSG_KEXDH_GEX_REPLY (%d), but got %d instead.' % (Protocol.MSG_KEXDH_GEX_REPLY, packet_type))
+            raise KexDHException('Expected MSG_KEXDH_GEX_REPLY (%d), but got %d instead.' % (Protocol.MSG_KEXDH_GEX_REPLY, packet_type))
 
         # Skip any & all MSG_DEBUG messages.
         while packet_type == Protocol.MSG_DEBUG:
             packet_type, payload = s.read_packet(2)
 
         # Parse the modulus (p) and generator (g) values from the server.
         ptr = 0
@@ -352,14 +392,14 @@
         # Now that we got the generator and modulus, perform the DH exchange
         # like usual.
         super(KexGroupExchange, self).set_params(g, p)
         super(KexGroupExchange, self).send_init(s, Protocol.MSG_KEXDH_GEX_INIT)
 
 
 class KexGroupExchange_SHA1(KexGroupExchange):
-    def __init__(self) -> None:
-        super(KexGroupExchange_SHA1, self).__init__('KexGroupExchange_SHA1', 'sha1')
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexGroupExchange_SHA1, self).__init__(out, 'KexGroupExchange_SHA1', 'sha1')
 
 
 class KexGroupExchange_SHA256(KexGroupExchange):
-    def __init__(self) -> None:
-        super(KexGroupExchange_SHA256, self).__init__('KexGroupExchange_SHA256', 'sha256')
+    def __init__(self, out: 'OutputBuffer') -> None:
+        super(KexGroupExchange_SHA256, self).__init__(out, 'KexGroupExchange_SHA256', 'sha256')
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/outputbuffer.py` & `ssh-audit-2.9.0/src/ssh_audit/outputbuffer.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/product.py` & `ssh-audit-2.9.0/src/ssh_audit/protocol.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,13 +19,18 @@
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
 
 
-class Product:  # pylint: disable=too-few-public-methods
-    OpenSSH = 'OpenSSH'
-    DropbearSSH = 'Dropbear SSH'
-    LibSSH = 'libssh'
-    TinySSH = 'TinySSH'
-    PuTTY = 'PuTTY'
+class Protocol:  # pylint: disable=too-few-public-methods
+    SMSG_PUBLIC_KEY = 2
+    MSG_DEBUG = 4
+    MSG_KEXINIT = 20
+    MSG_NEWKEYS = 21
+    MSG_KEXDH_INIT = 30
+    MSG_KEXDH_REPLY = 31
+    MSG_KEXDH_GEX_REQUEST = 34
+    MSG_KEXDH_GEX_GROUP = 31
+    MSG_KEXDH_GEX_INIT = 32
+    MSG_KEXDH_GEX_REPLY = 33
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/protocol.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh1_crc32.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,20 +17,31 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
+# pylint: disable=unused-import
+from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
+from typing import Callable, Optional, Union, Any  # noqa: F401
 
 
-class Protocol:  # pylint: disable=too-few-public-methods
-    SMSG_PUBLIC_KEY = 2
-    MSG_DEBUG = 4
-    MSG_KEXINIT = 20
-    MSG_NEWKEYS = 21
-    MSG_KEXDH_INIT = 30
-    MSG_KEXDH_REPLY = 31
-    MSG_KEXDH_GEX_REQUEST = 34
-    MSG_KEXDH_GEX_GROUP = 31
-    MSG_KEXDH_GEX_INIT = 32
-    MSG_KEXDH_GEX_REPLY = 33
+class SSH1_CRC32:
+    def __init__(self) -> None:
+        self._table = [0] * 256
+        for i in range(256):
+            crc = 0
+            n = i
+            for _ in range(8):
+                x = (crc ^ n) & 1
+                crc = (crc >> 1) ^ (x * 0xedb88320)
+                n = n >> 1
+                self._table[i] = crc
+
+    def calc(self, v: bytes) -> int:
+        crc, length = 0, len(v)
+        for i in range(length):
+            n = ord(v[i:i + 1])
+            n = n ^ (crc & 0xff)
+            crc = (crc >> 8) ^ self._table[n]
+        return crc
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/readbuf.py` & `ssh-audit-2.9.0/src/ssh_audit/readbuf.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/software.py` & `ssh-audit-2.9.0/src/ssh_audit/software.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh1.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh1.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh1_crc32.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh2_kexparty.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,26 +22,29 @@
    THE SOFTWARE.
 """
 # pylint: disable=unused-import
 from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
 from typing import Callable, Optional, Union, Any  # noqa: F401
 
 
-class SSH1_CRC32:
-    def __init__(self) -> None:
-        self._table = [0] * 256
-        for i in range(256):
-            crc = 0
-            n = i
-            for _ in range(8):
-                x = (crc ^ n) & 1
-                crc = (crc >> 1) ^ (x * 0xedb88320)
-                n = n >> 1
-                self._table[i] = crc
-
-    def calc(self, v: bytes) -> int:
-        crc, length = 0, len(v)
-        for i in range(length):
-            n = ord(v[i:i + 1])
-            n = n ^ (crc & 0xff)
-            crc = (crc >> 8) ^ self._table[n]
-        return crc
+class SSH2_KexParty:
+    def __init__(self, enc: List[str], mac: List[str], compression: List[str], languages: List[str]) -> None:
+        self.__enc = enc
+        self.__mac = mac
+        self.__compression = compression
+        self.__languages = languages
+
+    @property
+    def encryption(self) -> List[str]:
+        return self.__enc
+
+    @property
+    def mac(self) -> List[str]:
+        return self.__mac
+
+    @property
+    def compression(self) -> List[str]:
+        return self.__compression
+
+    @property
+    def languages(self) -> List[str]:
+        return self.__languages
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh1_kexdb.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh1_kexdb.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh1_publickeymessage.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh1_publickeymessage.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh2_kex.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh2_kex.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,36 +18,36 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
-# pylint: disable=unused-import
-from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
-from typing import Callable, Optional, Union, Any  # noqa: F401
+from typing import Dict, List
+from typing import Union
 
-from ssh_audit.ssh2_kexparty import SSH2_KexParty
+from ssh_audit.outputbuffer import OutputBuffer
 from ssh_audit.readbuf import ReadBuf
+from ssh_audit.ssh2_kexparty import SSH2_KexParty
 from ssh_audit.writebuf import WriteBuf
 
 
 class SSH2_Kex:
-    def __init__(self, cookie: bytes, kex_algs: List[str], key_algs: List[str], cli: 'SSH2_KexParty', srv: 'SSH2_KexParty', follows: bool, unused: int = 0) -> None:
+    def __init__(self, outputbuffer: 'OutputBuffer', cookie: bytes, kex_algs: List[str], key_algs: List[str], cli: 'SSH2_KexParty', srv: 'SSH2_KexParty', follows: bool, unused: int = 0) -> None:  # pylint: disable=too-many-arguments
+        self.__outputbuffer = outputbuffer
         self.__cookie = cookie
         self.__kex_algs = kex_algs
         self.__key_algs = key_algs
         self.__client = cli
         self.__server = srv
         self.__follows = follows
         self.__unused = unused
 
-        self.__rsa_key_sizes: Dict[str, Tuple[int, int]] = {}
-        self.__dh_modulus_sizes: Dict[str, Tuple[int, int]] = {}
-        self.__host_keys: Dict[str, bytes] = {}
+        self.__dh_modulus_sizes: Dict[str, int] = {}
+        self.__host_keys: Dict[str, Dict[str, Union[bytes, str, int]]] = {}
 
     @property
     def cookie(self) -> bytes:
         return self.__cookie
 
     @property
     def kex_algorithms(self) -> List[str]:
@@ -71,30 +71,28 @@
     def follows(self) -> bool:
         return self.__follows
 
     @property
     def unused(self) -> int:
         return self.__unused
 
-    def set_rsa_key_size(self, rsa_type: str, hostkey_size: int, ca_size: int = -1) -> None:
-        self.__rsa_key_sizes[rsa_type] = (hostkey_size, ca_size)
-
-    def rsa_key_sizes(self) -> Dict[str, Tuple[int, int]]:
-        return self.__rsa_key_sizes
-
     def set_dh_modulus_size(self, gex_alg: str, modulus_size: int) -> None:
-        self.__dh_modulus_sizes[gex_alg] = (modulus_size, -1)
+        self.__dh_modulus_sizes[gex_alg] = modulus_size
 
-    def dh_modulus_sizes(self) -> Dict[str, Tuple[int, int]]:
+    def dh_modulus_sizes(self) -> Dict[str, int]:
         return self.__dh_modulus_sizes
 
-    def set_host_key(self, key_type: str, hostkey: bytes) -> None:
-        self.__host_keys[key_type] = hostkey
+    def set_host_key(self, key_type: str, raw_hostkey_bytes: bytes, hostkey_size: int, ca_key_type: str, ca_key_size: int) -> None:
+
+        if key_type not in self.__host_keys:
+            self.__host_keys[key_type] = {'raw_hostkey_bytes': raw_hostkey_bytes, 'hostkey_size': hostkey_size, 'ca_key_type': ca_key_type, 'ca_key_size': ca_key_size}
+        else:  # A host key may only have one CA signature...
+            self.__outputbuffer.d("WARNING: called SSH2_Kex.set_host_key() multiple times with the same host key type (%s)!  Existing info: %r, %r, %r; Duplicate (ignored) info: %r, %r, %r" % (key_type, self.__host_keys[key_type]['hostkey_size'], self.__host_keys[key_type]['ca_key_type'], self.__host_keys[key_type]['ca_key_size'], hostkey_size, ca_key_type, ca_key_size))
 
-    def host_keys(self) -> Dict[str, bytes]:
+    def host_keys(self) -> Dict[str, Dict[str, Union[bytes, str, int]]]:
         return self.__host_keys
 
     def write(self, wbuf: 'WriteBuf') -> None:
         wbuf.write(self.cookie)
         wbuf.write_list(self.kex_algorithms)
         wbuf.write_list(self.key_algorithms)
         wbuf.write_list(self.client.encryption)
@@ -111,15 +109,15 @@
     @property
     def payload(self) -> bytes:
         wbuf = WriteBuf()
         self.write(wbuf)
         return wbuf.write_flush()
 
     @classmethod
-    def parse(cls, payload: bytes) -> 'SSH2_Kex':
+    def parse(cls, outputbuffer: 'OutputBuffer', payload: bytes) -> 'SSH2_Kex':
         buf = ReadBuf(payload)
         cookie = buf.read(16)
         kex_algs = buf.read_list()
         key_algs = buf.read_list()
         cli_enc = buf.read_list()
         srv_enc = buf.read_list()
         cli_mac = buf.read_list()
@@ -128,9 +126,9 @@
         srv_compression = buf.read_list()
         cli_languages = buf.read_list()
         srv_languages = buf.read_list()
         follows = buf.read_bool()
         unused = buf.read_int()
         cli = SSH2_KexParty(cli_enc, cli_mac, cli_compression, cli_languages)
         srv = SSH2_KexParty(srv_enc, srv_mac, srv_compression, srv_languages)
-        kex = cls(cookie, kex_algs, key_algs, cli, srv, follows, unused)
+        kex = cls(outputbuffer, cookie, kex_algs, key_algs, cli, srv, follows, unused)
         return kex
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh2_kexdb.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh2_kexdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
    The MIT License (MIT)
 
-   Copyright (C) 2017-2021 Joe Testa (jtesta@positronsecurity.com)
+   Copyright (C) 2017-2023 Joe Testa (jtesta@positronsecurity.com)
    Copyright (C) 2017 Andris Raugulis (moo@arthepsy.eu)
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
@@ -24,257 +24,368 @@
 """
 # pylint: disable=unused-import
 from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
 from typing import Callable, Optional, Union, Any  # noqa: F401
 
 
 class SSH2_KexDB:  # pylint: disable=too-few-public-methods
-    WARN_OPENSSH74_UNSAFE = 'disabled (in client) since OpenSSH 7.4, unsafe algorithm'
-    WARN_OPENSSH72_LEGACY = 'disabled (in client) since OpenSSH 7.2, legacy algorithm'
-    FAIL_OPENSSH70_LEGACY = 'removed since OpenSSH 7.0, legacy algorithm'
-    FAIL_OPENSSH70_WEAK = 'removed (in server) and disabled (in client) since OpenSSH 7.0, weak algorithm'
-    FAIL_OPENSSH70_LOGJAM = 'disabled (in client) since OpenSSH 7.0, logjam attack'
-    INFO_OPENSSH69_CHACHA = 'default cipher since OpenSSH 6.9.'
-    FAIL_OPENSSH67_UNSAFE = 'removed (in server) since OpenSSH 6.7, unsafe algorithm'
-    FAIL_OPENSSH61_REMOVE = 'removed since OpenSSH 6.1, removed from specification'
-    FAIL_OPENSSH31_REMOVE = 'removed since OpenSSH 3.1'
-    INFO_OPENSSH82_FUTURE_DEPRECATION = 'a future deprecation notice has been issued in OpenSSH 8.2: https://www.openssh.com/txt/release-8.2'
-    FAIL_DBEAR67_DISABLED = 'disabled since Dropbear SSH 2015.67'
-    FAIL_DBEAR53_DISABLED = 'disabled since Dropbear SSH 0.53'
-    FAIL_DEPRECATED_CIPHER = 'deprecated cipher'
-    FAIL_WEAK_CIPHER = 'using weak cipher'
-    FAIL_WEAK_ALGORITHM = 'using weak/obsolete algorithm'
-    FAIL_PLAINTEXT = 'no encryption/integrity'
-    FAIL_DEPRECATED_MAC = 'deprecated MAC'
     FAIL_1024BIT_MODULUS = 'using small 1024-bit modulus'
+    FAIL_3DES = 'using broken & deprecated 3DES cipher'
+    FAIL_BLOWFISH = 'using weak & deprecated Blowfish cipher'
+    FAIL_CAST = 'using weak & deprecated CAST cipher'
+    FAIL_DES = 'using broken DES cipher'
+    FAIL_IDEA = 'using deprecated IDEA cipher'
+    FAIL_LOGJAM_ATTACK = 'vulnerable to the Logjam attack: https://en.wikipedia.org/wiki/Logjam_(computer_security)'
+    FAIL_MD5 = 'using broken MD5 hash algorithm'
+    FAIL_NSA_BACKDOORED_CURVE = 'using elliptic curves that are suspected as being backdoored by the U.S. National Security Agency'
+    FAIL_PLAINTEXT = 'no encryption/integrity'
+    FAIL_RC4 = 'using broken RC4 cipher'
+    FAIL_RIJNDAEL = 'using deprecated & non-standardized Rijndael cipher'
+    FAIL_RIPEMD = 'using deprecated RIPEMD hash algorithm'
+    FAIL_SEED = 'using deprecated SEED cipher'
+    FAIL_SERPENT = 'using deprecated Serpent cipher'
+    FAIL_SHA1 = 'using broken SHA-1 hash algorithm'
+    FAIL_SMALL_ECC_MODULUS = 'using small ECC modulus'
+    FAIL_UNKNOWN = 'using unknown algorithm'
     FAIL_UNPROVEN = 'using unproven algorithm'
-    FAIL_HASH_WEAK = 'using weak hashing algorithm'
-    WARN_CURVES_WEAK = 'using weak elliptic curves'
-    WARN_RNDSIG_KEY = 'using weak random number generator could reveal the key'
-    WARN_HASH_WEAK = 'using weak hashing algorithm'
-    WARN_CIPHER_MODE = 'using weak cipher mode'
+    FAIL_UNTRUSTED = 'using untrusted algorithm developed in secret by a government entity'
+
+    WARN_2048BIT_MODULUS = '2048-bit modulus only provides 112-bits of symmetric strength'
     WARN_BLOCK_SIZE = 'using small 64-bit block size'
-    WARN_CIPHER_WEAK = 'using weak cipher'
+    WARN_CIPHER_MODE = 'using weak cipher mode'
     WARN_ENCRYPT_AND_MAC = 'using encrypt-and-MAC mode'
+    WARN_EXPERIMENTAL = 'using experimental algorithm'
+    WARN_RNDSIG_KEY = 'using weak random number generator could reveal the key'
     WARN_TAG_SIZE = 'using small 64-bit tag size'
     WARN_TAG_SIZE_96 = 'using small 96-bit tag size'
-    WARN_EXPERIMENTAL = 'using experimental algorithm'
-    WARN_OBSOLETE = 'using obsolete algorithm'
-    WARN_UNTRUSTED = 'using untrusted algorithm'
+
+    INFO_DEFAULT_OPENSSH_CIPHER = 'default cipher since OpenSSH 6.9'
+    INFO_DEFAULT_OPENSSH_KEX = 'default key exchange since OpenSSH 6.4'
+    INFO_DEPRECATED_IN_OPENSSH88 = 'deprecated in OpenSSH 8.8: https://www.openssh.com/txt/release-8.8'
+    INFO_DISABLED_IN_DBEAR67 = 'disabled in Dropbear SSH 2015.67'
+    INFO_DISABLED_IN_OPENSSH70 = 'disabled in OpenSSH 7.0: https://www.openssh.com/txt/release-7.0'
+    INFO_NEVER_IMPLEMENTED_IN_OPENSSH = 'despite the @openssh.com tag, this was never implemented in OpenSSH'
+    INFO_REMOVED_IN_OPENSSH61 = 'removed since OpenSSH 6.1, removed from specification'
+    INFO_REMOVED_IN_OPENSSH69 = 'removed in OpenSSH 6.9: https://www.openssh.com/txt/release-6.9'
+    INFO_REMOVED_IN_OPENSSH70 = 'removed in OpenSSH 7.0: https://www.openssh.com/txt/release-7.0'
+    INFO_WITHDRAWN_PQ_ALG = 'the sntrup4591761 algorithm was withdrawn, as it may not provide strong post-quantum security'
+
 
     ALGORITHMS: Dict[str, Dict[str, List[List[Optional[str]]]]] = {
-        # Format: 'algorithm_name': [['version_first_appeared_in'], [reason_for_failure1, reason_for_failure2, ...], [warning1, warning2, ...]]
+        # Format: 'algorithm_name': [['version_first_appeared_in'], [reason_for_failure1, reason_for_failure2, ...], [warning1, warning2, ...], [info1, info2, ...]]
         'kex': {
-            'diffie-hellman-group1-sha1': [['2.3.0,d0.28,l10.2', '6.6', '6.9'], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH67_UNSAFE, FAIL_OPENSSH70_LOGJAM], [WARN_HASH_WEAK]],
-            'gss-group1-sha1-toWM5Slw5Ew8Mqkay+al2g==': [[], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH67_UNSAFE, FAIL_OPENSSH70_LOGJAM], [WARN_HASH_WEAK]],
-            'gss-gex-sha1-eipGX3TCiQSrx573bT1o1Q==': [[], [], [WARN_HASH_WEAK]],
-            'gss-gex-sha1-toWM5Slw5Ew8Mqkay+al2g==': [[], [], [WARN_HASH_WEAK]],
-            'gss-gex-sha1-': [[], [], [WARN_HASH_WEAK]],
-            'gss-group1-sha1-eipGX3TCiQSrx573bT1o1Q==': [[], [FAIL_1024BIT_MODULUS], [WARN_HASH_WEAK]],
-            'gss-group1-sha1-': [[], [FAIL_1024BIT_MODULUS], [WARN_HASH_WEAK]],
-            'gss-group14-sha1-': [[], [], [WARN_HASH_WEAK]],
-            'gss-group14-sha1-eipGX3TCiQSrx573bT1o1Q==': [[], [], [WARN_HASH_WEAK]],
-            'gss-group14-sha1-toWM5Slw5Ew8Mqkay+al2g==': [[], [], [WARN_HASH_WEAK]],
-            'gss-group14-sha256-': [[]],
-            'gss-group14-sha256-toWM5Slw5Ew8Mqkay+al2g==': [[]],
-            'gss-group15-sha512-': [[]],
-            'gss-group15-sha512-toWM5Slw5Ew8Mqkay+al2g==': [[]],
-            'gss-group16-sha512-': [[]],
-            'gss-nistp256-sha256-': [[], [WARN_CURVES_WEAK]],
-            'gss-curve25519-sha256-': [[]],
-            'diffie-hellman-group1-sha256': [[], [FAIL_1024BIT_MODULUS]],
-            'diffie-hellman-group14-sha1': [['3.9,d0.53,l10.6.0'], [], [WARN_HASH_WEAK]],
-            'diffie-hellman-group14-sha256': [['7.3,d2016.73']],
-            'diffie-hellman-group14-sha256@ssh.com': [[]],
+            'Curve25519SHA256': [[]],
+            'curve25519-sha256': [['7.4,d2018.76'], [], [], [INFO_DEFAULT_OPENSSH_KEX]],
+            'curve25519-sha256@libssh.org': [['6.4,d2013.62,l10.6.0'], [], [], [INFO_DEFAULT_OPENSSH_KEX]],
+            'curve448-sha512': [[]],
+            'diffie-hellman-group14-sha1': [['3.9,d0.53,l10.6.0'], [FAIL_SHA1], [WARN_2048BIT_MODULUS]],
+            'diffie-hellman-group14-sha224@ssh.com': [[]],
+            'diffie-hellman-group14-sha256': [['7.3,d2016.73'], [], [WARN_2048BIT_MODULUS]],
+            'diffie-hellman-group14-sha256@ssh.com': [[], [], [WARN_2048BIT_MODULUS]],
             'diffie-hellman-group15-sha256': [[]],
             'diffie-hellman-group15-sha256@ssh.com': [[]],
             'diffie-hellman-group15-sha384@ssh.com': [[]],
             'diffie-hellman-group15-sha512': [[]],
             'diffie-hellman-group16-sha256': [[]],
             'diffie-hellman-group16-sha384@ssh.com': [[]],
             'diffie-hellman-group16-sha512': [['7.3,d2016.73']],
             'diffie-hellman-group16-sha512@ssh.com': [[]],
             'diffie-hellman-group17-sha512': [[]],
+            'diffie-hellman_group17-sha512': [[]],
             'diffie-hellman-group18-sha512': [['7.3']],
             'diffie-hellman-group18-sha512@ssh.com': [[]],
-            'diffie-hellman-group-exchange-sha1': [['2.3.0', '6.6', None], [FAIL_OPENSSH67_UNSAFE], [WARN_HASH_WEAK]],
+            'diffie-hellman-group1-sha1': [['2.3.0,d0.28,l10.2', '6.6', '6.9'], [FAIL_1024BIT_MODULUS, FAIL_LOGJAM_ATTACK, FAIL_SHA1], [], [INFO_REMOVED_IN_OPENSSH69]],
+            'diffie-hellman-group1-sha256': [[], [FAIL_1024BIT_MODULUS]],
+            'diffie-hellman-group-exchange-sha1': [['2.3.0', '6.6', None], [FAIL_SHA1]],
+            'diffie-hellman-group-exchange-sha224@ssh.com': [[]],
             'diffie-hellman-group-exchange-sha256': [['4.4']],
             'diffie-hellman-group-exchange-sha256@ssh.com': [[]],
+            'diffie-hellman-group-exchange-sha384@ssh.com': [[]],
             'diffie-hellman-group-exchange-sha512@ssh.com': [[]],
-            'ecdh-sha2-curve25519': [[], []],
-            'ecdh-sha2-nistb233': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistb409': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistk163': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistk233': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistk283': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistk409': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistp192': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistp224': [[], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistp256': [['5.7,d2013.62,l10.6.0'], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistp384': [['5.7,d2013.62'], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistp521': [['5.7,d2013.62'], [WARN_CURVES_WEAK]],
-            'ecdh-sha2-nistt571': [[], [WARN_CURVES_WEAK]],
+            'ecdh-sha2-1.2.840.10045.3.1.1': [[], [FAIL_SMALL_ECC_MODULUS, FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-192 / secp192r1
+            'ecdh-sha2-1.2.840.10045.3.1.7': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-256 / secp256r1
             'ecdh-sha2-1.3.132.0.10': [[]],  # ECDH over secp256k1 (i.e.: the Bitcoin curve)
-            'curve25519-sha256@libssh.org': [['6.5,d2013.62,l10.6.0']],
-            'curve25519-sha256': [['7.4,d2018.76']],
-            'curve448-sha512': [[]],
-            'kexguess2@matt.ucc.asn.au': [['d2013.57']],
-            'rsa1024-sha1': [[], [FAIL_1024BIT_MODULUS], [WARN_HASH_WEAK]],
-            'rsa2048-sha256': [[]],
-            'sntrup4591761x25519-sha512@tinyssh.org': [['8.0', '8.4'], [], [WARN_EXPERIMENTAL]],
-            'sntrup761x25519-sha512@openssh.com': [['8.5'], [], [WARN_EXPERIMENTAL]],
-            'kexAlgoCurve25519SHA256': [[]],
-            'Curve25519SHA256': [[]],
+            'ecdh-sha2-1.3.132.0.16': [[]],  # sect283k1
+            'ecdh-sha2-1.3.132.0.1': [[], [FAIL_SMALL_ECC_MODULUS]],  # sect163k1
+            'ecdh-sha2-1.3.132.0.26': [[], [FAIL_SMALL_ECC_MODULUS]],  # sect233k1
+            'ecdh-sha2-1.3.132.0.27': [[], [FAIL_SMALL_ECC_MODULUS, FAIL_NSA_BACKDOORED_CURVE]],  # sect233r1
+            'ecdh-sha2-1.3.132.0.33': [[], [FAIL_SMALL_ECC_MODULUS, FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-224 / secp224r1
+            'ecdh-sha2-1.3.132.0.34': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-384 / secp384r1
+            'ecdh-sha2-1.3.132.0.35': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-521 / secp521r1
+            'ecdh-sha2-1.3.132.0.36': [[]],  # sect409k1
+            'ecdh-sha2-1.3.132.0.37': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # sect409r1
+            'ecdh-sha2-1.3.132.0.38': [[]],  # sect571k1
+
+            # Note: the base64 strings, according to draft 6 of RFC5656, is Base64(MD5(DER(OID))).  The final RFC5656 dropped the base64 strings in favor of plain OID concatenation, but apparently some SSH servers implement them anyway.  See: https://datatracker.ietf.org/doc/html/draft-green-secsh-ecc-06#section-9.2
+            'ecdh-sha2-4MHB+NBt3AlaSRQ7MnB4cg==': [[], [FAIL_SMALL_ECC_MODULUS]],  # sect163k1
+            'ecdh-sha2-5pPrSUQtIaTjUSt5VZNBjg==': [[], [FAIL_SMALL_ECC_MODULUS, FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-192 / secp192r1
+            'ecdh-sha2-9UzNcgwTlEnSCECZa7V1mw==': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-256 / secp256r1
+            'ecdh-sha2-curve25519': [[], []],
+            'ecdh-sha2-D3FefCjYoJ/kfXgAyLddYA==': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # sect409r1
+            'ecdh-sha2-h/SsxnLCtRBh7I9ATyeB3A==': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-521 / secp521r1
+            'ecdh-sha2-m/FtSAmrV4j/Wy6RVUaK7A==': [[]],  # sect409k1
+            'ecdh-sha2-mNVwCXAoS1HGmHpLvBC94w==': [[]],  # sect571k1
+
+            'ecdh-sha2-nistb233': [[]],  # The NIST P-curves are suspected as being backdoored; this isn't a P-curve.
+            'ecdh-sha2-nistb409': [[]],  # Not a NIST P-curve.
+            'ecdh-sha2-nistk163': [[], [FAIL_SMALL_ECC_MODULUS]],    # Not a NIST P-curve.
+            'ecdh-sha2-nistk233': [[]],  # Not a NIST P-curve.
+            'ecdh-sha2-nistk283': [[]],  # Not a NIST P-curve.
+            'ecdh-sha2-nistk409': [[]],  # Not a NIST P-curve.
+            'ecdh-sha2-nistp192': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+            'ecdh-sha2-nistp224': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+            'ecdh-sha2-nistp256': [['5.7,d2013.62,l10.6.0'], [FAIL_NSA_BACKDOORED_CURVE]],
+            'ecdh-sha2-nistp384': [['5.7,d2013.62'], [FAIL_NSA_BACKDOORED_CURVE]],
+            'ecdh-sha2-nistp521': [['5.7,d2013.62'], [FAIL_NSA_BACKDOORED_CURVE]],
+            'ecdh-sha2-nistt571': [[]],  # Not a NIST P-curve.
+            'ecdh-sha2-qCbG5Cn/jjsZ7nBeR7EnOA==': [[FAIL_SMALL_ECC_MODULUS, FAIL_NSA_BACKDOORED_CURVE]],  # sect233r1
+            'ecdh-sha2-qcFQaMAMGhTziMT0z+Tuzw==': [[], [FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-384 / secp384r1
+            'ecdh-sha2-VqBg4QRPjxx1EXZdV0GdWQ==': [[], [FAIL_SMALL_ECC_MODULUS, FAIL_NSA_BACKDOORED_CURVE]],  # NIST P-224 / secp224r1
+            'ecdh-sha2-wiRIU8TKjMZ418sMqlqtvQ==': [[]],  # sect283k1
+            'ecdh-sha2-zD/b3hu/71952ArpUG4OjQ==': [[], [FAIL_SMALL_ECC_MODULUS]],  # sect233k1
+            'ecmqv-sha2': [[], [FAIL_UNPROVEN]],
             'ext-info-c': [[]],  # Extension negotiation (RFC 8308)
             'ext-info-s': [[]],  # Extension negotiation (RFC 8308)
+
+            # The GSS kex algorithms get special wildcard handling, since they include variable base64 data after their standard prefixes.
+            'gss-13.3.132.0.10-sha256-*': [[], [FAIL_UNKNOWN]],
+            'gss-curve25519-sha256-*': [[]],
+            'gss-curve448-sha512-*': [[]],
+            'gss-gex-sha1-*': [[], [FAIL_SHA1]],
+            'gss-gex-sha256-*': [[]],
+            'gss-group14-sha1-*': [[], [FAIL_SHA1], [WARN_2048BIT_MODULUS]],
+            'gss-group14-sha256-*': [[], [], [WARN_2048BIT_MODULUS]],
+            'gss-group15-sha512-*': [[]],
+            'gss-group16-sha512-*': [[]],
+            'gss-group17-sha512-*': [[]],
+            'gss-group18-sha512-*': [[]],
+            'gss-group1-sha1-*': [[], [FAIL_1024BIT_MODULUS, FAIL_LOGJAM_ATTACK, FAIL_SHA1]],
+            'gss-nistp256-sha256-*': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+            'gss-nistp384-sha256-*': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+            'gss-nistp521-sha512-*': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+
+            'kexAlgoCurve25519SHA256': [[]],
+            'kexguess2@matt.ucc.asn.au': [['d2013.57']],
+            'm383-sha384@libassh.org': [[], [FAIL_UNPROVEN]],
+            'm511-sha512@libassh.org': [[], [FAIL_UNPROVEN]],
+            'rsa1024-sha1': [[], [FAIL_1024BIT_MODULUS, FAIL_SHA1]],
+            'rsa2048-sha256': [[], [], [WARN_2048BIT_MODULUS]],
+            'sntrup4591761x25519-sha512@tinyssh.org': [['8.0', '8.4'], [], [WARN_EXPERIMENTAL], [INFO_WITHDRAWN_PQ_ALG]],
+            'sntrup761x25519-sha512@openssh.com': [['8.5'], [], []],
         },
         'key': {
-            'ssh-rsa1': [[], [FAIL_WEAK_ALGORITHM]],
-            'rsa-sha2-256': [['7.2']],
-            'rsa-sha2-512': [['7.2']],
-            'ssh-ed25519': [['6.5,l10.7.0']],
-            'ssh-ed25519-cert-v01@openssh.com': [['6.5']],
-            'ssh-rsa': [['2.5.0,d0.28,l10.2'], [FAIL_HASH_WEAK], [], [INFO_OPENSSH82_FUTURE_DEPRECATION]],
-            'ssh-dss': [['2.1.0,d0.28,l10.2', '6.9'], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH70_WEAK], [WARN_RNDSIG_KEY]],
-            'ecdsa-sha2-nistp256': [['5.7,d2013.62,l10.6.4'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
-            'ecdsa-sha2-nistp384': [['5.7,d2013.62,l10.6.4'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
-            'ecdsa-sha2-nistp521': [['5.7,d2013.62,l10.6.4'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
+            'dsa2048-sha224@libassh.org': [[], [FAIL_UNPROVEN], [WARN_2048BIT_MODULUS]],
+            'dsa2048-sha256@libassh.org': [[], [FAIL_UNPROVEN], [WARN_2048BIT_MODULUS]],
+            'dsa3072-sha256@libassh.org': [[], [FAIL_UNPROVEN]],
+            'ecdsa-sha2-1.3.132.0.10-cert-v01@openssh.com': [[], [FAIL_UNKNOWN]],
             'ecdsa-sha2-1.3.132.0.10': [[], [], [WARN_RNDSIG_KEY]],  # ECDSA over secp256k1 (i.e.: the Bitcoin curve)
-            'x509v3-sign-dss': [[], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH70_WEAK], [WARN_RNDSIG_KEY]],
-            'x509v3-sign-rsa': [[], [FAIL_HASH_WEAK], [], [INFO_OPENSSH82_FUTURE_DEPRECATION]],
-            'x509v3-sign-rsa-sha256@ssh.com': [[]],
-            'x509v3-ssh-dss': [[], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH70_WEAK], [WARN_RNDSIG_KEY]],
-            'x509v3-ssh-rsa': [[], [FAIL_HASH_WEAK], [], [INFO_OPENSSH82_FUTURE_DEPRECATION]],
-            'ssh-rsa-cert-v00@openssh.com': [['5.4', '6.9'], [FAIL_OPENSSH70_LEGACY, FAIL_HASH_WEAK], [], [INFO_OPENSSH82_FUTURE_DEPRECATION]],
-            'ssh-dss-cert-v00@openssh.com': [['5.4', '6.9'], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH70_LEGACY], [WARN_RNDSIG_KEY]],
-            'ssh-rsa-cert-v01@openssh.com': [['5.6'], [FAIL_HASH_WEAK], [], [INFO_OPENSSH82_FUTURE_DEPRECATION]],
-            'ssh-dss-cert-v01@openssh.com': [['5.6', '6.9'], [FAIL_1024BIT_MODULUS, FAIL_OPENSSH70_WEAK], [WARN_RNDSIG_KEY]],
-            'ecdsa-sha2-nistp256-cert-v01@openssh.com': [['5.7'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
-            'ecdsa-sha2-nistp384-cert-v01@openssh.com': [['5.7'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
-            'ecdsa-sha2-nistp521-cert-v01@openssh.com': [['5.7'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
+            'ecdsa-sha2-nistp256': [['5.7,d2013.62,l10.6.4'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'ecdsa-sha2-nistp256-cert-v01@openssh.com': [['5.7'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'ecdsa-sha2-nistp384': [['5.7,d2013.62,l10.6.4'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'ecdsa-sha2-nistp384-cert-v01@openssh.com': [['5.7'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'ecdsa-sha2-nistp521': [['5.7,d2013.62,l10.6.4'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'ecdsa-sha2-nistp521-cert-v01@openssh.com': [['5.7'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'eddsa-e382-shake256@libassh.org': [[], [FAIL_UNPROVEN]],
+            'eddsa-e521-shake256@libassh.org': [[], [FAIL_UNPROVEN]],
+            'null': [[], [FAIL_PLAINTEXT]],
+            'pgp-sign-dss': [[], [FAIL_1024BIT_MODULUS]],
+            'pgp-sign-rsa': [[], [FAIL_1024BIT_MODULUS]],
+            'rsa-sha2-256': [['7.2']],
             'rsa-sha2-256-cert-v01@openssh.com': [['7.8']],
+            'rsa-sha2-512': [['7.2']],
             'rsa-sha2-512-cert-v01@openssh.com': [['7.8']],
-            'ssh-rsa-sha256@ssh.com': [[]],
-            'ssh-dss-sha256@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
-            'sk-ecdsa-sha2-nistp256-cert-v01@openssh.com': [['8.2'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
-            'sk-ecdsa-sha2-nistp256@openssh.com': [['8.2'], [WARN_CURVES_WEAK], [WARN_RNDSIG_KEY]],
+            'sk-ecdsa-sha2-nistp256-cert-v01@openssh.com': [['8.2'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
+            'sk-ecdsa-sha2-nistp256@openssh.com': [['8.2'], [FAIL_NSA_BACKDOORED_CURVE], [WARN_RNDSIG_KEY]],
             'sk-ssh-ed25519-cert-v01@openssh.com': [['8.2']],
             'sk-ssh-ed25519@openssh.com': [['8.2']],
-            'ssh-gost2001': [[], [], [WARN_UNTRUSTED]],
-            'ssh-gost2012-256': [[], [], [WARN_UNTRUSTED]],
-            'ssh-gost2012-512': [[], [], [WARN_UNTRUSTED]],
             'spi-sign-rsa': [[]],
+            'spki-sign-dss': [[], [FAIL_1024BIT_MODULUS]],
+            'spki-sign-rsa': [[], [FAIL_1024BIT_MODULUS]],
+            'ssh-dss': [['2.1.0,d0.28,l10.2', '6.9'], [FAIL_1024BIT_MODULUS], [WARN_RNDSIG_KEY], [INFO_DISABLED_IN_OPENSSH70]],
+            'ssh-dss-cert-v00@openssh.com': [['5.4', '6.9'], [FAIL_1024BIT_MODULUS], [WARN_RNDSIG_KEY], [INFO_DISABLED_IN_OPENSSH70]],
+            'ssh-dss-cert-v01@openssh.com': [['5.6', '6.9'], [FAIL_1024BIT_MODULUS], [WARN_RNDSIG_KEY]],
+            'ssh-dss-sha224@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'ssh-dss-sha256@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'ssh-dss-sha384@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'ssh-dss-sha512@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'ssh-ed25519': [['6.5,l10.7.0']],
+            'ssh-ed25519-cert-v01@openssh.com': [['6.5']],
             'ssh-ed448': [[]],
-            'x509v3-ecdsa-sha2-nistp256': [[], [WARN_CURVES_WEAK]],
-            'x509v3-ecdsa-sha2-nistp384': [[], [WARN_CURVES_WEAK]],
-            'x509v3-ecdsa-sha2-nistp521': [[], [WARN_CURVES_WEAK]],
+            'ssh-ed448-cert-v01@openssh.com': [[], [], [], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],
+            'ssh-gost2001': [[], [FAIL_UNTRUSTED]],
+            'ssh-gost2012-256': [[], [FAIL_UNTRUSTED]],
+            'ssh-gost2012-512': [[], [FAIL_UNTRUSTED]],
+            'ssh-rsa1': [[], [FAIL_SHA1]],
+            'ssh-rsa': [['2.5.0,d0.28,l10.2'], [FAIL_SHA1], [], [INFO_DEPRECATED_IN_OPENSSH88]],
+            'ssh-rsa-cert-v00@openssh.com': [['5.4', '6.9'], [FAIL_SHA1], [], [INFO_REMOVED_IN_OPENSSH70]],
+            'ssh-rsa-cert-v01@openssh.com': [['5.6'], [FAIL_SHA1], [], [INFO_DEPRECATED_IN_OPENSSH88]],
+            'ssh-rsa-sha224@ssh.com': [[]],
+            'ssh-rsa-sha2-256': [[]],
+            'ssh-rsa-sha2-512': [[]],
+            'ssh-rsa-sha256@ssh.com': [[]],
+            'ssh-rsa-sha384@ssh.com': [[]],
+            'ssh-rsa-sha512@ssh.com': [[]],
+            'ssh-xmss-cert-v01@openssh.com': [['7.7'], [WARN_EXPERIMENTAL]],
+            'ssh-xmss@openssh.com': [['7.7'], [WARN_EXPERIMENTAL]],
+            'webauthn-sk-ecdsa-sha2-nistp256@openssh.com': [['8.3'], [FAIL_NSA_BACKDOORED_CURVE]],
+            'x509v3-ecdsa-sha2-1.3.132.0.10': [[], [FAIL_UNKNOWN]],
+            'x509v3-ecdsa-sha2-nistp256': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+            'x509v3-ecdsa-sha2-nistp384': [[], [FAIL_NSA_BACKDOORED_CURVE]],
+            'x509v3-ecdsa-sha2-nistp521': [[], [FAIL_NSA_BACKDOORED_CURVE]],
             'x509v3-rsa2048-sha256': [[]],
+            'x509v3-sign-dss': [[], [FAIL_1024BIT_MODULUS], [WARN_RNDSIG_KEY]],
+            'x509v3-sign-dss-sha1': [[], [FAIL_1024BIT_MODULUS, FAIL_SHA1]],
+            'x509v3-sign-dss-sha224@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'x509v3-sign-dss-sha256@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'x509v3-sign-dss-sha384@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'x509v3-sign-dss-sha512@ssh.com': [[], [FAIL_1024BIT_MODULUS]],
+            'x509v3-sign-rsa': [[], [FAIL_SHA1]],
+            'x509v3-sign-rsa-sha1': [[], [FAIL_SHA1]],
+            'x509v3-sign-rsa-sha224@ssh.com': [[]],
+            'x509v3-sign-rsa-sha256@ssh.com': [[]],
+            'x509v3-sign-rsa-sha384@ssh.com': [[]],
+            'x509v3-sign-rsa-sha512@ssh.com': [[]],
+            'x509v3-ssh-dss': [[], [FAIL_1024BIT_MODULUS], [WARN_RNDSIG_KEY]],
+            'x509v3-ssh-rsa': [[], [FAIL_SHA1], [], [INFO_DEPRECATED_IN_OPENSSH88]],
         },
         'enc': {
-            'none': [['1.2.2,d2013.56,l10.2'], [FAIL_PLAINTEXT]],
-            'des': [[], [FAIL_WEAK_CIPHER], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            'des-cbc': [[], [FAIL_WEAK_CIPHER], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            'des-cbc@ssh.com': [[], [FAIL_WEAK_CIPHER], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            'des-cbc-ssh1': [[], [FAIL_WEAK_CIPHER], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            '3des': [[], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH74_UNSAFE, WARN_CIPHER_WEAK, WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            '3des-cbc': [['1.2.2,d0.28,l10.2', '6.6', None], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH74_UNSAFE, WARN_CIPHER_WEAK, WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            '3des-ctr': [['d0.52'], [FAIL_WEAK_CIPHER]],
-            'blowfish': [[], [FAIL_WEAK_ALGORITHM], [WARN_BLOCK_SIZE]],
-            'blowfish-cbc': [['1.2.2,d0.28,l10.2', '6.6,d0.52', '7.1,d0.52'], [FAIL_OPENSSH67_UNSAFE, FAIL_DBEAR53_DISABLED], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            'blowfish-ctr': [[], [FAIL_OPENSSH67_UNSAFE, FAIL_DBEAR53_DISABLED], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            'twofish-cbc': [['d0.28', 'd2014.66'], [FAIL_DBEAR67_DISABLED], [WARN_CIPHER_MODE]],
-            'twofish128-cbc': [['d0.47', 'd2014.66'], [FAIL_DBEAR67_DISABLED], [WARN_CIPHER_MODE]],
-            'twofish192-cbc': [[], [], [WARN_CIPHER_MODE]],
-            'twofish256-cbc': [['d0.47', 'd2014.66'], [FAIL_DBEAR67_DISABLED], [WARN_CIPHER_MODE]],
-            'twofish-ctr': [[]],
-            'twofish128-ctr': [['d2015.68']],
-            'twofish192-ctr': [[]],
-            'twofish256-ctr': [['d2015.68']],
-            'serpent128-cbc': [[], [FAIL_DEPRECATED_CIPHER], [WARN_CIPHER_MODE]],
-            'serpent192-cbc': [[], [FAIL_DEPRECATED_CIPHER], [WARN_CIPHER_MODE]],
-            'serpent256-cbc': [[], [FAIL_DEPRECATED_CIPHER], [WARN_CIPHER_MODE]],
-            'serpent128-ctr': [[], [FAIL_DEPRECATED_CIPHER]],
-            'serpent192-ctr': [[], [FAIL_DEPRECATED_CIPHER]],
-            'serpent256-ctr': [[], [FAIL_DEPRECATED_CIPHER]],
-            'idea-cbc': [[], [FAIL_DEPRECATED_CIPHER], [WARN_CIPHER_MODE]],
-            'idea-ctr': [[], [FAIL_DEPRECATED_CIPHER]],
-            'cast128-ctr': [[], [FAIL_DEPRECATED_CIPHER]],
-            'cast128-cbc': [['2.1.0', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
-            'arcfour': [['2.1.0', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_WEAK]],
-            'arcfour128': [['4.2', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_WEAK]],
-            'arcfour256': [['4.2', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_WEAK]],
-            'aes128-cbc': [['2.3.0,d0.28,l10.2', '6.6', None], [FAIL_OPENSSH67_UNSAFE], [WARN_CIPHER_MODE]],
-            'aes192-cbc': [['2.3.0,l10.2', '6.6', None], [FAIL_OPENSSH67_UNSAFE], [WARN_CIPHER_MODE]],
-            'aes256-cbc': [['2.3.0,d0.47,l10.2', '6.6', None], [FAIL_OPENSSH67_UNSAFE], [WARN_CIPHER_MODE]],
-            'rijndael128-cbc': [['2.3.0', '3.0.2'], [FAIL_OPENSSH31_REMOVE], [WARN_CIPHER_MODE]],
-            'rijndael192-cbc': [['2.3.0', '3.0.2'], [FAIL_OPENSSH31_REMOVE], [WARN_CIPHER_MODE]],
-            'rijndael256-cbc': [['2.3.0', '3.0.2'], [FAIL_OPENSSH31_REMOVE], [WARN_CIPHER_MODE]],
-            'rijndael-cbc@lysator.liu.se': [['2.3.0', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_CIPHER_MODE]],
+            '3des-cbc': [['1.2.2,d0.28,l10.2', '6.6', None], [FAIL_3DES], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            '3des-cfb': [[], [FAIL_3DES], [WARN_CIPHER_MODE]],
+            '3des-ctr': [['d0.52'], [FAIL_3DES]],
+            '3des-ecb': [[], [FAIL_3DES], [WARN_CIPHER_MODE]],
+            '3des': [[], [FAIL_3DES], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            '3des-ofb': [[], [FAIL_3DES], [WARN_CIPHER_MODE]],
+            'AEAD_AES_128_GCM': [[]],
+            'AEAD_AES_256_GCM': [[]],
+            'aes128-cbc': [['2.3.0,d0.28,l10.2', '6.6', None], [], [WARN_CIPHER_MODE]],
             'aes128-ctr': [['3.7,d0.52,l10.4.1']],
+            'aes128-gcm': [[]],
+            'aes128-gcm@openssh.com': [['6.2']],
+            'aes192-cbc': [['2.3.0,l10.2', '6.6', None], [], [WARN_CIPHER_MODE]],
             'aes192-ctr': [['3.7,l10.4.1']],
+            'aes256-cbc': [['2.3.0,d0.47,l10.2', '6.6', None], [], [WARN_CIPHER_MODE]],
             'aes256-ctr': [['3.7,d0.52,l10.4.1']],
-            'aes128-gcm': [[]],
             'aes256-gcm': [[]],
-            'AEAD_AES_128_GCM': [[]],
-            'AEAD_AES_256_GCM': [[]],
-            'aes128-gcm@openssh.com': [['6.2']],
             'aes256-gcm@openssh.com': [['6.2']],
-            'chacha20-poly1305': [[], [], [], [INFO_OPENSSH69_CHACHA]],
-            'chacha20-poly1305@openssh.com': [['6.5'], [], [], [INFO_OPENSSH69_CHACHA]],
+            'arcfour128': [['4.2', '6.6', '7.1'], [FAIL_RC4]],
+            'arcfour': [['2.1.0', '6.6', '7.1'], [FAIL_RC4]],
+            'arcfour256': [['4.2', '6.6', '7.1'], [FAIL_RC4]],
+            'blowfish-cbc': [['1.2.2,d0.28,l10.2', '6.6,d0.52', '7.1,d0.52'], [FAIL_BLOWFISH], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'blowfish-cfb': [[], [FAIL_BLOWFISH], [WARN_CIPHER_MODE]],
+            'blowfish-ctr': [[], [FAIL_BLOWFISH], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'blowfish-ecb': [[], [FAIL_BLOWFISH], [WARN_CIPHER_MODE]],
+            'blowfish': [[], [FAIL_BLOWFISH], [WARN_BLOCK_SIZE]],
+            'blowfish-ofb': [[], [FAIL_BLOWFISH], [WARN_CIPHER_MODE]],
+            'camellia128-cbc@openssh.org': [[], [], [WARN_CIPHER_MODE]],
             'camellia128-cbc': [[], [], [WARN_CIPHER_MODE]],
             'camellia128-ctr': [[]],
+            'camellia128-ctr@openssh.org': [[]],
+            'camellia192-cbc@openssh.org': [[], [], [WARN_CIPHER_MODE]],
             'camellia192-cbc': [[], [], [WARN_CIPHER_MODE]],
             'camellia192-ctr': [[]],
+            'camellia192-ctr@openssh.org': [[]],
+            'camellia256-cbc@openssh.org': [[], [], [WARN_CIPHER_MODE]],
             'camellia256-cbc': [[], [], [WARN_CIPHER_MODE]],
             'camellia256-ctr': [[]],
+            'camellia256-ctr@openssh.org': [[]],
+            'cast128-12-cbc@ssh.com': [[], [FAIL_CAST], [WARN_CIPHER_MODE]],
+            'cast128-cbc': [['2.1.0', '6.6', '7.1'], [FAIL_CAST], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'cast128-cfb': [[], [FAIL_CAST], [WARN_CIPHER_MODE]],
+            'cast128-ctr': [[], [FAIL_CAST]],
+            'cast128-ecb': [[], [FAIL_CAST], [WARN_CIPHER_MODE]],
+            'cast128-ofb': [[], [FAIL_CAST], [WARN_CIPHER_MODE]],
+            'chacha20-poly1305': [[], [], [], [INFO_DEFAULT_OPENSSH_CIPHER]],
+            'chacha20-poly1305@openssh.com': [['6.5'], [], [], [INFO_DEFAULT_OPENSSH_CIPHER]],
             'crypticore128@ssh.com': [[], [FAIL_UNPROVEN]],
-            'seed-cbc@ssh.com': [[], [], [WARN_OBSOLETE, WARN_CIPHER_MODE]],
+            'des-cbc': [[], [FAIL_DES], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'des-cbc-ssh1': [[], [FAIL_DES], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'des-cbc@ssh.com': [[], [FAIL_DES], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'des': [[], [FAIL_DES], [WARN_CIPHER_MODE, WARN_BLOCK_SIZE]],
+            'idea-cbc': [[], [FAIL_IDEA], [WARN_CIPHER_MODE]],
+            'idea-cfb': [[], [FAIL_IDEA], [WARN_CIPHER_MODE]],
+            'idea-ctr': [[], [FAIL_IDEA]],
+            'idea-ecb': [[], [FAIL_IDEA], [WARN_CIPHER_MODE]],
+            'idea-ofb': [[], [FAIL_IDEA], [WARN_CIPHER_MODE]],
+            'none': [['1.2.2,d2013.56,l10.2'], [FAIL_PLAINTEXT]],
+            'rijndael128-cbc': [['2.3.0', '7.0'], [FAIL_RIJNDAEL], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_OPENSSH70]],
+            'rijndael192-cbc': [['2.3.0', '7.0'], [FAIL_RIJNDAEL], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_OPENSSH70]],
+            'rijndael256-cbc': [['2.3.0', '7.0'], [FAIL_RIJNDAEL], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_OPENSSH70]],
+            'rijndael-cbc@lysator.liu.se': [['2.3.0', '6.6', '7.0'], [FAIL_RIJNDAEL], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_OPENSSH70]],
+            'rijndael-cbc@ssh.com': [[], [FAIL_RIJNDAEL], [WARN_CIPHER_MODE]],
+            'seed-cbc@ssh.com': [[], [FAIL_SEED], [WARN_CIPHER_MODE]],
+            'seed-ctr@ssh.com': [[], [FAIL_SEED]],
+            'serpent128-cbc': [[], [FAIL_SERPENT], [WARN_CIPHER_MODE]],
+            'serpent128-ctr': [[], [FAIL_SERPENT]],
+            'serpent128-gcm@libassh.org': [[], [FAIL_SERPENT]],
+            'serpent192-cbc': [[], [FAIL_SERPENT], [WARN_CIPHER_MODE]],
+            'serpent192-ctr': [[], [FAIL_SERPENT]],
+            'serpent256-cbc': [[], [FAIL_SERPENT], [WARN_CIPHER_MODE]],
+            'serpent256-ctr': [[], [FAIL_SERPENT]],
+            'serpent256-gcm@libassh.org': [[], [FAIL_SERPENT]],
+            'twofish128-cbc': [['d0.47', 'd2014.66'], [], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_DBEAR67]],
+            'twofish128-ctr': [['d2015.68']],
+            'twofish128-gcm@libassh.org': [[]],
+            'twofish192-cbc': [[], [], [WARN_CIPHER_MODE]],
+            'twofish192-ctr': [[]],
+            'twofish256-cbc': [['d0.47', 'd2014.66'], [], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_DBEAR67]],
+            'twofish256-ctr': [['d2015.68']],
+            'twofish256-gcm@libassh.org': [[]],
+            'twofish-cbc': [['d0.28', 'd2014.66'], [], [WARN_CIPHER_MODE], [INFO_DISABLED_IN_DBEAR67]],
+            'twofish-cfb': [[], [], [WARN_CIPHER_MODE]],
+            'twofish-ctr': [[]],
+            'twofish-ecb': [[], [], [WARN_CIPHER_MODE]],
+            'twofish-ofb': [[], [], [WARN_CIPHER_MODE]],
         },
         'mac': {
-            'none': [['d2013.56'], [FAIL_PLAINTEXT]],
-            'hmac-sha1': [['2.1.0,d0.28,l10.2'], [], [WARN_ENCRYPT_AND_MAC, WARN_HASH_WEAK]],
-            'hmac-sha1-96': [['2.5.0,d0.47', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_ENCRYPT_AND_MAC, WARN_HASH_WEAK]],
-            'hmac-sha2-56': [[], [], [WARN_TAG_SIZE, WARN_ENCRYPT_AND_MAC]],
+            'AEAD_AES_128_GCM': [[]],
+            'AEAD_AES_256_GCM': [[]],
+            'aes128-gcm': [[]],
+            'aes256-gcm': [[]],
+            'chacha20-poly1305@openssh.com': [[], [], [], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],  # Despite the @openssh.com tag, this was never shipped as a MAC in OpenSSH (only as a cipher); it is only implemented as a MAC in Syncplify.
+            'crypticore-mac@ssh.com': [[], [FAIL_UNPROVEN]],
+            'hmac-md5': [['2.1.0,d0.28', '6.6', '7.1'], [FAIL_MD5], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-md5-96': [['2.5.0', '6.6', '7.1'], [FAIL_MD5], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-md5-96-etm@openssh.com': [['6.2', '6.6', '7.1'], [FAIL_MD5]],
+            'hmac-md5-etm@openssh.com': [['6.2', '6.6', '7.1'], [FAIL_MD5]],
+            'hmac-ripemd160': [['2.5.0', '6.6', '7.1'], [FAIL_RIPEMD], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-ripemd160-96': [[], [FAIL_RIPEMD], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],
+            'hmac-ripemd160-etm@openssh.com': [['6.2', '6.6', '7.1'], [FAIL_RIPEMD]],
+            'hmac-ripemd160@openssh.com': [['2.1.0', '6.6', '7.1'], [FAIL_RIPEMD], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-ripemd': [[], [FAIL_RIPEMD], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha1': [['2.1.0,d0.28,l10.2'], [FAIL_SHA1], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha1-96': [['2.5.0,d0.47', '6.6', '7.1'], [FAIL_SHA1], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha1-96-etm@openssh.com': [['6.2', '6.6', None], [FAIL_SHA1]],
+            'hmac-sha1-96@openssh.com': [[], [FAIL_SHA1], [WARN_TAG_SIZE, WARN_ENCRYPT_AND_MAC], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],
+            'hmac-sha1-etm@openssh.com': [['6.2'], [FAIL_SHA1]],
             'hmac-sha2-224': [[], [], [WARN_TAG_SIZE, WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha224@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],
             'hmac-sha2-256': [['5.9,d2013.56,l10.7.0'], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-sha2-256-96': [['5.9', '6.0'], [FAIL_OPENSSH61_REMOVE], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha2-256-96': [['5.9', '6.0'], [], [WARN_ENCRYPT_AND_MAC], [INFO_REMOVED_IN_OPENSSH61]],
+            'hmac-sha2-256-96-etm@openssh.com': [[], [], [WARN_TAG_SIZE_96], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],  # Only ever implemented in AsyncSSH (?).
+            'hmac-sha2-256-etm@openssh.com': [['6.2']],
             'hmac-sha2-384': [[], [], [WARN_ENCRYPT_AND_MAC]],
             'hmac-sha2-512': [['5.9,d2013.56,l10.7.0'], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-sha2-512-96': [['5.9', '6.0'], [FAIL_OPENSSH61_REMOVE], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha2-512-96': [['5.9', '6.0'], [], [WARN_ENCRYPT_AND_MAC], [INFO_REMOVED_IN_OPENSSH61]],
+            'hmac-sha2-512-96-etm@openssh.com': [[], [], [WARN_TAG_SIZE_96], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],  # Only ever implemented in AsyncSSH (?).
+            'hmac-sha2-512-etm@openssh.com': [['6.2']],
+            'hmac-sha256-2@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha256-96@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],
+            'hmac-sha256@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha256': [[], [], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha2-56': [[], [], [WARN_TAG_SIZE, WARN_ENCRYPT_AND_MAC]],
             'hmac-sha3-224': [[], [], [WARN_ENCRYPT_AND_MAC]],
             'hmac-sha3-256': [[], [], [WARN_ENCRYPT_AND_MAC]],
             'hmac-sha3-384': [[], [], [WARN_ENCRYPT_AND_MAC]],
             'hmac-sha3-512': [[], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-sha256': [[], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-sha256-96@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],
-            'hmac-sha256@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-sha512': [[], [], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-sha384@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],
             'hmac-sha512@ssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-md5': [['2.1.0,d0.28', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_ENCRYPT_AND_MAC, WARN_HASH_WEAK]],
-            'hmac-md5-96': [['2.5.0', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_ENCRYPT_AND_MAC, WARN_HASH_WEAK]],
-            'hmac-ripemd': [[], [FAIL_DEPRECATED_MAC], [WARN_OPENSSH72_LEGACY, WARN_ENCRYPT_AND_MAC]],
-            'hmac-ripemd160': [['2.5.0', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_ENCRYPT_AND_MAC]],
-            'hmac-ripemd160-96': [[], [FAIL_DEPRECATED_MAC], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],
-            'hmac-ripemd160@openssh.com': [['2.1.0', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_ENCRYPT_AND_MAC]],
-            'umac-64@openssh.com': [['4.7'], [], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],
+            'hmac-sha512': [[], [], [WARN_ENCRYPT_AND_MAC]],
+            'hmac-whirlpool': [[], [], [WARN_ENCRYPT_AND_MAC]],
+            'none': [['d2013.56'], [FAIL_PLAINTEXT]],
+            'umac-128-etm@openssh.com': [['6.2']],
             'umac-128@openssh.com': [['6.2'], [], [WARN_ENCRYPT_AND_MAC]],
-            'hmac-sha1-etm@openssh.com': [['6.2'], [], [WARN_HASH_WEAK]],
-            'hmac-sha1-96-etm@openssh.com': [['6.2', '6.6', None], [FAIL_OPENSSH67_UNSAFE], [WARN_HASH_WEAK]],
-            'hmac-sha2-256-96-etm@openssh.com': [[], [], [WARN_TAG_SIZE_96]],  # Despite the @openssh.com tag, it doesn't appear that this was ever shipped with OpenSSH; it is only implemented in AsyncSSH (?).
-            'hmac-sha2-512-96-etm@openssh.com': [[], [], [WARN_TAG_SIZE_96]],  # Despite the @openssh.com tag, it doesn't appear that this was ever shipped with OpenSSH; it is only implemented in AsyncSSH (?).
-            'hmac-sha2-256-etm@openssh.com': [['6.2']],
-            'hmac-sha2-512-etm@openssh.com': [['6.2']],
-            'hmac-md5-etm@openssh.com': [['6.2', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_HASH_WEAK]],
-            'hmac-md5-96-etm@openssh.com': [['6.2', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY, WARN_HASH_WEAK]],
-            'hmac-ripemd160-etm@openssh.com': [['6.2', '6.6', '7.1'], [FAIL_OPENSSH67_UNSAFE], [WARN_OPENSSH72_LEGACY]],
-            'umac-32@openssh.com': [[], [], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],  # Despite having the @openssh.com suffix, this may never have shipped with OpenSSH (!).
+            'umac-32@openssh.com': [[], [], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],
             'umac-64-etm@openssh.com': [['6.2'], [], [WARN_TAG_SIZE]],
-            'umac-96@openssh.com': [[], [], [WARN_ENCRYPT_AND_MAC]],  # Despite having the @openssh.com suffix, this may never have shipped with OpenSSH (!).
-            'umac-128-etm@openssh.com': [['6.2']],
-            'aes128-gcm': [[]],
-            'aes256-gcm': [[]],
-            'chacha20-poly1305@openssh.com': [[]],  # Despite the @openssh.com tag, this was never shipped as a MAC in OpenSSH (only as a cipher); it is only implemented as a MAC in Syncplify.
-            'crypticore-mac@ssh.com': [[], [FAIL_UNPROVEN]],
-            'AEAD_AES_128_GCM': [[]],
-            'AEAD_AES_256_GCM': [[]],
+            'umac-64@openssh.com': [['4.7'], [], [WARN_ENCRYPT_AND_MAC, WARN_TAG_SIZE]],
+            'umac-96@openssh.com': [[], [], [WARN_ENCRYPT_AND_MAC], [INFO_NEVER_IMPLEMENTED_IN_OPENSSH]],
         }
     }
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh_audit.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh_audit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 """
    The MIT License (MIT)
 
-   Copyright (C) 2017-2021 Joe Testa (jtesta@positronsecurity.com)
+   Copyright (C) 2017-2023 Joe Testa (jtesta@positronsecurity.com)
    Copyright (C) 2017 Andris Raugulis (moo@arthepsy.eu)
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
@@ -30,16 +30,18 @@
 import os
 import re
 import sys
 import traceback
 
 # pylint: disable=unused-import
 from typing import Dict, List, Set, Sequence, Tuple, Iterable  # noqa: F401
-from typing import Callable, Optional, Union, Any  # noqa: F401
+from typing import cast, Callable, Optional, Union, Any  # noqa: F401
 
+from ssh_audit.globals import SNAP_PACKAGE
+from ssh_audit.globals import SNAP_PERMISSIONS_ERROR
 from ssh_audit.globals import VERSION
 from ssh_audit.globals import WINDOWS_MAN_PAGE
 from ssh_audit.algorithm import Algorithm
 from ssh_audit.algorithms import Algorithms
 from ssh_audit.auditconf import AuditConf
 from ssh_audit.banner import Banner
 from ssh_audit import exitcodes
@@ -55,40 +57,53 @@
 from ssh_audit.ssh1_publickeymessage import SSH1_PublicKeyMessage
 from ssh_audit.ssh2_kex import SSH2_Kex
 from ssh_audit.ssh2_kexdb import SSH2_KexDB
 from ssh_audit.ssh_socket import SSH_Socket
 from ssh_audit.utils import Utils
 from ssh_audit.versionvulnerabilitydb import VersionVulnerabilityDB
 
+
+# no_idna_workaround = False
+
 # Only import colorama under Windows.  Other OSes can natively handle terminal colors.
 if sys.platform == 'win32':
     try:
-        from colorama import init as colorama_init
-        colorama_init()
+        from colorama import just_fix_windows_console
+        just_fix_windows_console()
     except ImportError:
         pass
 
+    # This is a workaround for a Python bug that causes a crash on Windows when multiple threads are used (see https://github.com/python/cpython/issues/73474).  Importing the idna module and using it in a no-op seems to fix the issue.  Otherwise, if idna isn't available at run-time, force single threaded scans.
+    # try:
+    #     import idna  # noqa: F401
+    #
+    #     ''.encode('idna')
+    # except ImportError:
+    #     no_idna_workaround = True
+
 
-def usage(err: Optional[str] = None) -> None:
+def usage(uout: OutputBuffer, err: Optional[str] = None) -> None:
     retval = exitcodes.GOOD
-    uout = OutputBuffer()
     p = os.path.basename(sys.argv[0])
     uout.head('# {} {}, https://github.com/jtesta/ssh-audit\n'.format(p, VERSION))
     if err is not None and len(err) > 0:
-        uout.fail('\n' + err)
+        uout.fail(err + '\n')
         retval = exitcodes.UNKNOWN_ERROR
     uout.info('usage: {0} [options] <host>\n'.format(p))
     uout.info('   -h,  --help             print this help')
     uout.info('   -1,  --ssh1             force ssh version 1 only')
     uout.info('   -2,  --ssh2             force ssh version 2 only')
     uout.info('   -4,  --ipv4             enable IPv4 (order of precedence)')
     uout.info('   -6,  --ipv6             enable IPv6 (order of precedence)')
     uout.info('   -b,  --batch            batch output')
     uout.info('   -c,  --client-audit     starts a server on port 2222 to audit client\n                               software config (use -p to change port;\n                               use -t to change timeout)')
     uout.info('   -d,  --debug            debug output')
+    uout.info('   -g,  --gex-test=<x[,y,...]>  dh gex modulus size test')
+    uout.info('                   <min1:pref1:max1[,min2:pref2:max2,...]>')
+    uout.info('                   <x-y[:step]>')
     uout.info('   -j,  --json             JSON output (use -jj to enable indents)')
     uout.info('   -l,  --level=<level>    minimum output level (info|warn|fail)')
     uout.info('   -L,  --list-policies    list all the official, built-in policies')
     uout.info('        --lookup=<alg1,alg2,...>    looks up an algorithm(s) without\n                                    connecting to a server')
     uout.info('   -M,  --make-policy=<policy.txt>  creates a policy based on the target server\n                                    (i.e.: the target server has the ideal\n                                    configuration that other servers should\n                                    adhere to)')
     uout.info('   -m,  --manual           print the man page (Windows only)')
     uout.info('   -n,  --no-colors        disable colors')
@@ -99,44 +114,60 @@
     uout.info('        --threads=<threads>    number of threads to use when scanning multiple\n                                   targets (-T/--targets) (default: 32)')
     uout.info('   -v,  --verbose          verbose output')
     uout.sep()
     uout.write()
     sys.exit(retval)
 
 
-def output_algorithms(out: OutputBuffer, title: str, alg_db: Dict[str, Dict[str, List[List[Optional[str]]]]], alg_type: str, algorithms: List[str], unknown_algs: List[str], is_json_output: bool, program_retval: int, maxlen: int = 0, alg_sizes: Optional[Dict[str, Tuple[int, int]]] = None) -> int:  # pylint: disable=too-many-arguments
+def output_algorithms(out: OutputBuffer, title: str, alg_db: Dict[str, Dict[str, List[List[Optional[str]]]]], alg_type: str, algorithms: List[str], unknown_algs: List[str], is_json_output: bool, program_retval: int, maxlen: int = 0, host_keys: Optional[Dict[str, Dict[str, Union[bytes, str, int]]]] = None, dh_modulus_sizes: Optional[Dict[str, int]] = None) -> int:  # pylint: disable=too-many-arguments
     with out:
         for algorithm in algorithms:
-            program_retval = output_algorithm(out, alg_db, alg_type, algorithm, unknown_algs, program_retval, maxlen, alg_sizes)
+            program_retval = output_algorithm(out, alg_db, alg_type, algorithm, unknown_algs, program_retval, maxlen, host_keys=host_keys, dh_modulus_sizes=dh_modulus_sizes)
     if not out.is_section_empty() and not is_json_output:
         out.head('# ' + title)
         out.flush_section()
         out.sep()
 
     return program_retval
 
 
-def output_algorithm(out: OutputBuffer, alg_db: Dict[str, Dict[str, List[List[Optional[str]]]]], alg_type: str, alg_name: str, unknown_algs: List[str], program_retval: int, alg_max_len: int = 0, alg_sizes: Optional[Dict[str, Tuple[int, int]]] = None) -> int:
+def output_algorithm(out: OutputBuffer, alg_db: Dict[str, Dict[str, List[List[Optional[str]]]]], alg_type: str, alg_name: str, unknown_algs: List[str], program_retval: int, alg_max_len: int = 0, host_keys: Optional[Dict[str, Dict[str, Union[bytes, str, int]]]] = None, dh_modulus_sizes: Optional[Dict[str, int]] = None) -> int:  # pylint: disable=too-many-arguments
     prefix = '(' + alg_type + ') '
     if alg_max_len == 0:
         alg_max_len = len(alg_name)
     padding = '' if out.batch else ' ' * (alg_max_len - len(alg_name))
 
     # If this is an RSA host key or DH GEX, append the size to its name and fix
     # the padding.
     alg_name_with_size = None
-    if (alg_sizes is not None) and (alg_name in alg_sizes):
-        hostkey_size, ca_size = alg_sizes[alg_name]
-        if ca_size > 0:
-            alg_name_with_size = '%s (%d-bit cert/%d-bit CA)' % (alg_name, hostkey_size, ca_size)
+    if (dh_modulus_sizes is not None) and (alg_name in dh_modulus_sizes):
+        alg_name_with_size = '%s (%u-bit)' % (alg_name, dh_modulus_sizes[alg_name])
+        padding = padding[0:-11]
+    elif (host_keys is not None) and (alg_name in host_keys):
+        hostkey_size = cast(int, host_keys[alg_name]['hostkey_size'])
+        ca_key_type = cast(str, host_keys[alg_name]['ca_key_type'])
+        ca_key_size = cast(int, host_keys[alg_name]['ca_key_size'])
+
+        # If this is an RSA variant, just print "RSA".
+        if ca_key_type in HostKeyTest.RSA_FAMILY:
+            ca_key_type = "RSA"
+
+        if len(ca_key_type) > 0 and ca_key_size > 0:
+            alg_name_with_size = '%s (%u-bit cert/%u-bit %s CA)' % (alg_name, hostkey_size, ca_key_size, ca_key_type)
             padding = padding[0:-15]
-        else:
-            alg_name_with_size = '%s (%d-bit)' % (alg_name, hostkey_size)
+        elif alg_name in HostKeyTest.RSA_FAMILY:
+            alg_name_with_size = '%s (%u-bit)' % (alg_name, hostkey_size)
             padding = padding[0:-11]
 
+    # If this is a kex algorithm and starts with 'gss-', then normalize its name (i.e.: 'gss-gex-sha1-vz8J1E9PzLr8b1K+0remTg==' => 'gss-gex-sha1-*').  The base64 field can vary, so we'll convert it to the wildcard that our database uses and we'll just resume doing a straight match like all other algorithm names.
+    alg_name_original = alg_name
+    if alg_type == 'kex' and alg_name.startswith('gss-'):
+        last_dash = alg_name.rindex('-')
+        alg_name = "%s-*" % alg_name[0:last_dash]
+
     texts = []
     if len(alg_name.strip()) == 0:
         return program_retval
     alg_name_native = Utils.to_text(alg_name)
     if alg_name_native in alg_db[alg_type]:
         alg_desc = alg_db[alg_type][alg_name_native]
         ldesc = len(alg_desc)
@@ -154,14 +185,18 @@
                     texts.append((level, t))
         if len(texts) == 0:
             texts.append(('info', ''))
     else:
         texts.append(('warn', 'unknown algorithm'))
         unknown_algs.append(alg_name)
 
+    # For kex GSS algorithms, now that we already did the database lookup (above), restore the original algorithm name so its reported properly in the output.
+    if alg_name != alg_name_original:
+        alg_name = alg_name_original
+
     alg_name = alg_name_with_size if alg_name_with_size is not None else alg_name
     first = True
     for level, text in texts:
         if level == 'fail':
             program_retval = exitcodes.FAILURE
         elif level == 'warn' and program_retval != exitcodes.FAILURE:  # If a failure was found previously, don't downgrade to warning.
             program_retval = exitcodes.WARNING
@@ -173,15 +208,15 @@
                 f = out.good
             f(prefix + alg_name + comment)
             first = False
         else:  # pylint: disable=else-if-used
             if out.verbose:
                 f(prefix + alg_name + comment)
             elif text != '':
-                comment = (padding + ' `- [' + level + '] ' + text)
+                comment = padding + ' `- [' + level + '] ' + text
                 f(' ' * len(prefix + alg_name) + comment)
 
     return program_retval
 
 
 def output_compatibility(out: OutputBuffer, algs: Algorithms, client_audit: bool, for_server: bool = True) -> None:
 
@@ -209,18 +244,20 @@
             else:
                 tfmt = '{0} {1}-{2}'
             comp_text.append(tfmt.format(ssh_prod, v_from, v_till))
     if len(comp_text) > 0:
         out.good('(gen) compatibility: ' + ', '.join(comp_text))
 
 
-def output_security_sub(out: OutputBuffer, sub: str, software: Optional[Software], client_audit: bool, padlen: int) -> None:
+def output_security_sub(out: OutputBuffer, sub: str, software: Optional[Software], client_audit: bool, padlen: int) -> List[Dict[str, Union[str, float]]]:
+    ret: List[Dict[str, Union[str, float]]] = []
+
     secdb = VersionVulnerabilityDB.CVE if sub == 'cve' else VersionVulnerabilityDB.TXT
     if software is None or software.product not in secdb:
-        return
+        return ret
     for line in secdb[software.product]:
         vfrom: str = ''
         vtill: str = ''
         vfrom, vtill = line[0:2]
         if not software.between_versions(vfrom, vtill):
             continue
         target: int = 0
@@ -240,75 +277,82 @@
             cvss, descr = line[4:6]
 
             # Critical CVSS scores (>= 8.0) are printed as a fail, otherwise they are printed as a warning.
             out_func = out.warn
             if cvss >= 8.0:
                 out_func = out.fail
             out_func('(cve) {}{} -- (CVSSv2: {}) {}'.format(name, p, cvss, descr))
+            ret.append({'name': name, 'cvssv2': cvss, 'description': descr})
         else:
             descr = line[4]
             out.fail('(sec) {}{} -- {}'.format(name, p, descr))
 
+    return ret
+
+
+def output_security(out: OutputBuffer, banner: Optional[Banner], client_audit: bool, padlen: int, is_json_output: bool) -> List[Dict[str, Union[str, float]]]:
+    cves = []
 
-def output_security(out: OutputBuffer, banner: Optional[Banner], client_audit: bool, padlen: int, is_json_output: bool) -> None:
     with out:
         if banner is not None:
             software = Software.parse(banner)
-            output_security_sub(out, 'cve', software, client_audit, padlen)
-            output_security_sub(out, 'txt', software, client_audit, padlen)
+            cves = output_security_sub(out, 'cve', software, client_audit, padlen)
+            _ = output_security_sub(out, 'txt', software, client_audit, padlen)
             if banner.protocol[0] == 1:
                 p = '' if out.batch else ' ' * (padlen - 14)
                 out.fail('(sec) SSH v1 enabled{} -- SSH v1 can be exploited to recover plaintext passwords'.format(p))
     if not out.is_section_empty() and not is_json_output:
         out.head('# security')
         out.flush_section()
         out.sep()
 
+    return cves
+
 
 def output_fingerprints(out: OutputBuffer, algs: Algorithms, is_json_output: bool) -> None:
     with out:
-        fps = []
+        fps = {}
         if algs.ssh1kex is not None:
             name = 'ssh-rsa1'
             fp = Fingerprint(algs.ssh1kex.host_key_fingerprint_data)
             # bits = algs.ssh1kex.host_key_bits
-            fps.append((name, fp))
+            fps[name] = fp
         if algs.ssh2kex is not None:
             host_keys = algs.ssh2kex.host_keys()
             for host_key_type in algs.ssh2kex.host_keys():
                 if host_keys[host_key_type] is None:
                     continue
 
-                fp = Fingerprint(host_keys[host_key_type])
+                fp = Fingerprint(cast(bytes, host_keys[host_key_type]['raw_hostkey_bytes']))
 
                 # Workaround for Python's order-indifference in dicts.  We might get a random RSA type (ssh-rsa, rsa-sha2-256, or rsa-sha2-512), so running the tool against the same server three times may give three different host key types here.  So if we have any RSA type, we will simply hard-code it to 'ssh-rsa'.
                 if host_key_type in HostKeyTest.RSA_FAMILY:
                     host_key_type = 'ssh-rsa'
 
-                # Skip over certificate host types (or we would return invalid fingerprints).
+                # Skip over certificate host types (or we would return invalid fingerprints), and only add one fingerprint in the RSA family.
                 if '-cert-' not in host_key_type:
-                    fps.append((host_key_type, fp))
+                    fps[host_key_type] = fp
         # Similarly, the host keys can be processed in random order due to Python's order-indifference in dicts.  So we sort this list before printing; this makes automated testing possible.
-        fps = sorted(fps)
-        for fpp in fps:
-            name, fp = fpp
-            out.good('(fin) {}: {}'.format(name, fp.sha256))
+        fp_types = sorted(fps.keys())
+        for fp_type in fp_types:
+            fp = fps[fp_type]
+            out.good('(fin) {}: {}'.format(fp_type, fp.sha256))
 
             # Output the MD5 hash too if verbose mode is enabled.
             if out.verbose:
-                out.info('(fin) {}: {} -- [info] do not rely on MD5 fingerprints for server identification; it is insecure for this use case'.format(name, fp.md5))
+                out.info('(fin) {}: {} -- [info] do not rely on MD5 fingerprints for server identification; it is insecure for this use case'.format(fp_type, fp.md5))
 
     if not out.is_section_empty() and not is_json_output:
         out.head('# fingerprints')
         out.flush_section()
         out.sep()
 
 
 # Returns True if no warnings or failures encountered in configuration.
-def output_recommendations(out: OutputBuffer, algs: Algorithms, software: Optional[Software], is_json_output: bool, padlen: int = 0) -> bool:
+def output_recommendations(out: OutputBuffer, algs: Algorithms, algorithm_recommendation_suppress_list: List[str], software: Optional[Software], is_json_output: bool, padlen: int = 0) -> bool:
 
     ret = True
     # PuTTY's algorithms cannot be modified, so there's no point in issuing recommendations.
     if (software is not None) and (software.product == Product.PuTTY):
         max_vuln_version = 0.0
         max_cvssv2_severity = 0.0
         # Search the CVE database for the most recent vulnerable version and the max CVSSv2 score.
@@ -331,43 +375,43 @@
         if current_version < upgrade_to_version:
             out.head('# recommendations')
             fn('(rec) Upgrade to PuTTY v%.2f' % upgrade_to_version)
             out.sep()
             ret = False
         return ret
 
-    for_server = True
     with out:
-        software, alg_rec = algs.get_recommendations(software, for_server)
-        for sshv in range(2, 0, -1):
-            if sshv not in alg_rec:
-                continue
-            for alg_type in ['kex', 'key', 'enc', 'mac']:
-                if alg_type not in alg_rec[sshv]:
-                    continue
-                for action in ['del', 'add', 'chg']:
-                    if action not in alg_rec[sshv][alg_type]:
-                        continue
-                    for name in alg_rec[sshv][alg_type][action]:
+        recommendations = get_algorithm_recommendations(algs, algorithm_recommendation_suppress_list, software, for_server=True)
+
+        for level in recommendations:  # pylint: disable=consider-using-dict-items
+            for action in recommendations[level]:
+                for alg_type in recommendations[level][action]:
+                    for alg_name_and_notes in recommendations[level][action][alg_type]:
+                        name = alg_name_and_notes['name']
+                        notes = alg_name_and_notes['notes']
+
                         p = '' if out.batch else ' ' * (padlen - len(name))
-                        chg_additional_info = ''
+
                         if action == 'del':
                             an, sg, fn = 'remove', '-', out.warn
                             ret = False
-                            if alg_rec[sshv][alg_type][action][name] >= 10:
+                            if level == 'critical':
                                 fn = out.fail
                         elif action == 'add':
                             an, sg, fn = 'append', '+', out.good
                         elif action == 'chg':
                             an, sg, fn = 'change', '!', out.fail
                             ret = False
-                            chg_additional_info = ' (increase modulus size to 2048 bits or larger)'
-                        b = '(SSH{})'.format(sshv) if sshv == 1 else ''
-                        fm = '(rec) {0}{1}{2}-- {3} algorithm to {4}{5} {6}'
-                        fn(fm.format(sg, name, p, alg_type, an, chg_additional_info, b))
+
+                        if notes != '':
+                            notes = " (%s)" % notes
+
+                        fm = '(rec) {0}{1}{2}-- {3} algorithm to {4}{5} '
+                        fn(fm.format(sg, name, p, alg_type, an, notes))
+
     if not out.is_section_empty() and not is_json_output:
         if software is not None:
             title = '(for {})'.format(software.display(False))
         else:
             title = ''
         out.head('# algorithm recommendations {}'.format(title))
         out.flush_section(sort_section=True)  # Sort the output so that it is always stable (needed for repeatable testing).
@@ -388,21 +432,46 @@
 
     if not out.is_section_empty() and not is_json_output:
         out.head('# additional info')
         out.flush_section()
         out.sep()
 
 
+def post_process_findings(banner: Optional[Banner], algs: Algorithms) -> List[str]:
+    '''Perform post-processing on scan results before reporting them to the user.  Returns a list of algorithms that should not be recommended'''
+
+
+    algorithm_recommendation_suppress_list = []
+
+    # If the server is OpenSSH, and the diffie-hellman-group-exchange-sha256 key exchange was found with modulus size 2048, add a note regarding the bug that causes the server to support 2048-bit moduli no matter the configuration.
+    if (algs.ssh2kex is not None and 'diffie-hellman-group-exchange-sha256' in algs.ssh2kex.kex_algorithms and 'diffie-hellman-group-exchange-sha256' in algs.ssh2kex.dh_modulus_sizes() and algs.ssh2kex.dh_modulus_sizes()['diffie-hellman-group-exchange-sha256'] == 2048) and (banner is not None and banner.software is not None and banner.software.find('OpenSSH') != -1):
+
+        # Ensure a list for notes exists.
+        while len(SSH2_KexDB.ALGORITHMS['kex']['diffie-hellman-group-exchange-sha256']) < 4:
+            SSH2_KexDB.ALGORITHMS['kex']['diffie-hellman-group-exchange-sha256'].append([])
+
+        SSH2_KexDB.ALGORITHMS['kex']['diffie-hellman-group-exchange-sha256'][3].append("A bug in OpenSSH causes it to fall back to a 2048-bit modulus regardless of server configuration (https://bugzilla.mindrot.org/show_bug.cgi?id=2793)")
+
+        # Ensure that this algorithm doesn't appear in the recommendations section since the user cannot control this OpenSSH bug.
+        algorithm_recommendation_suppress_list.append('diffie-hellman-group-exchange-sha256')
+
+    return algorithm_recommendation_suppress_list
+
+
 # Returns a exitcodes.* flag to denote if any failures or warnings were encountered.
 def output(out: OutputBuffer, aconf: AuditConf, banner: Optional[Banner], header: List[str], client_host: Optional[str] = None, kex: Optional[SSH2_Kex] = None, pkm: Optional[SSH1_PublicKeyMessage] = None, print_target: bool = False) -> int:
 
     program_retval = exitcodes.GOOD
     client_audit = client_host is not None  # If set, this is a client audit.
     sshv = 1 if pkm is not None else 2
     algs = Algorithms(pkm, kex)
+
+    # Perform post-processing on the findings to make final adjustments before outputting the results.
+    algorithm_recommendation_suppress_list = post_process_findings(banner, algs)
+
     with out:
         if print_target:
             host = aconf.host
 
             # Print the port if it's not the default of 22.
             if aconf.port != 22:
 
@@ -443,45 +512,50 @@
                 cmptxt = 'disabled'
             out.good('(gen) compression: {}'.format(cmptxt))
     if not out.is_section_empty() and not aconf.json:  # Print output when it exists and JSON output isn't requested.
         out.head('# general')
         out.flush_section()
         out.sep()
     maxlen = algs.maxlen + 1
-    output_security(out, banner, client_audit, maxlen, aconf.json)
+    cves = output_security(out, banner, client_audit, maxlen, aconf.json)
     # Filled in by output_algorithms() with unidentified algs.
     unknown_algorithms: List[str] = []
+
+    # SSHv1
     if pkm is not None:
         adb = SSH1_KexDB.ALGORITHMS
         ciphers = pkm.supported_ciphers
         auths = pkm.supported_authentications
         title, atype = 'SSH1 host-key algorithms', 'key'
         program_retval = output_algorithms(out, title, adb, atype, ['ssh-rsa1'], unknown_algorithms, aconf.json, program_retval, maxlen)
         title, atype = 'SSH1 encryption algorithms (ciphers)', 'enc'
         program_retval = output_algorithms(out, title, adb, atype, ciphers, unknown_algorithms, aconf.json, program_retval, maxlen)
         title, atype = 'SSH1 authentication types', 'aut'
         program_retval = output_algorithms(out, title, adb, atype, auths, unknown_algorithms, aconf.json, program_retval, maxlen)
+
+    # SSHv2
     if kex is not None:
         adb = SSH2_KexDB.ALGORITHMS
         title, atype = 'key exchange algorithms', 'kex'
-        program_retval = output_algorithms(out, title, adb, atype, kex.kex_algorithms, unknown_algorithms, aconf.json, program_retval, maxlen, kex.dh_modulus_sizes())
+        program_retval = output_algorithms(out, title, adb, atype, kex.kex_algorithms, unknown_algorithms, aconf.json, program_retval, maxlen, dh_modulus_sizes=kex.dh_modulus_sizes())
         title, atype = 'host-key algorithms', 'key'
-        program_retval = output_algorithms(out, title, adb, atype, kex.key_algorithms, unknown_algorithms, aconf.json, program_retval, maxlen, kex.rsa_key_sizes())
+        program_retval = output_algorithms(out, title, adb, atype, kex.key_algorithms, unknown_algorithms, aconf.json, program_retval, maxlen, host_keys=kex.host_keys())
         title, atype = 'encryption algorithms (ciphers)', 'enc'
         program_retval = output_algorithms(out, title, adb, atype, kex.server.encryption, unknown_algorithms, aconf.json, program_retval, maxlen)
         title, atype = 'message authentication code algorithms', 'mac'
         program_retval = output_algorithms(out, title, adb, atype, kex.server.mac, unknown_algorithms, aconf.json, program_retval, maxlen)
+
     output_fingerprints(out, algs, aconf.json)
-    perfect_config = output_recommendations(out, algs, software, aconf.json, maxlen)
+    perfect_config = output_recommendations(out, algs, algorithm_recommendation_suppress_list, software, aconf.json, maxlen)
     output_info(out, software, client_audit, not perfect_config, aconf.json)
 
     if aconf.json:
         out.reset()
         # Build & write the JSON struct.
-        out.info(json.dumps(build_struct(aconf.host, banner, kex=kex, client_host=client_host), indent=4 if aconf.json_print_indent else None, sort_keys=True))
+        out.info(json.dumps(build_struct(aconf.host + ":" + str(aconf.port), banner, cves, kex=kex, client_host=client_host, software=software, algorithms=algs, algorithm_recommendation_suppress_list=algorithm_recommendation_suppress_list), indent=4 if aconf.json_print_indent else None, sort_keys=True))
     elif len(unknown_algorithms) > 0:  # If we encountered any unknown algorithms, ask the user to report them.
         out.warn("\n\n!!! WARNING: unknown algorithm(s) found!: %s.  Please email the full output above to the maintainer (jtesta@positronsecurity.com), or create a Github issue at <https://github.com/jtesta/ssh-audit/issues>.\n" % ','.join(unknown_algorithms))
 
     return program_retval
 
 
 def evaluate_policy(out: OutputBuffer, aconf: AuditConf, banner: Optional['Banner'], client_host: Optional[str], kex: Optional['SSH2_Kex'] = None) -> bool:
@@ -523,14 +597,63 @@
         else:
             out.fail("%sFailed!" % icon_fail)
             out.warn("\nErrors:\n%s" % error_str)
 
     return passed
 
 
+def get_algorithm_recommendations(algs: Optional[Algorithms], algorithm_recommendation_suppress_list: Optional[List[str]], software: Optional[Software], for_server: bool = True) -> Dict[str, Any]:
+    '''Returns the algorithm recommendations.'''
+    ret: Dict[str, Any] = {}
+
+    if algs is None or software is None:
+        return ret
+
+    software, alg_rec = algs.get_recommendations(software, for_server)
+    for sshv in range(2, 0, -1):
+        if sshv not in alg_rec:
+            continue
+        for alg_type in ['kex', 'key', 'enc', 'mac']:
+            if alg_type not in alg_rec[sshv]:
+                continue
+            for action in ['del', 'add', 'chg']:
+                if action not in alg_rec[sshv][alg_type]:
+                    continue
+
+                for name in alg_rec[sshv][alg_type][action]:
+
+                    # If this algorithm should be suppressed, skip it.
+                    if algorithm_recommendation_suppress_list is not None and name in algorithm_recommendation_suppress_list:
+                        continue
+
+                    level = 'informational'
+                    points = alg_rec[sshv][alg_type][action][name]
+                    if points >= 10:
+                        level = 'critical'
+                    elif points >= 1:
+                        level = 'warning'
+
+                    if level not in ret:
+                        ret[level] = {}
+
+                    if action not in ret[level]:
+                        ret[level][action] = {}
+
+                    if alg_type not in ret[level][action]:
+                        ret[level][action][alg_type] = []
+
+                    notes = ''
+                    if action == 'chg':
+                        notes = 'increase modulus size to 3072 bits or larger'
+
+                    ret[level][action][alg_type].append({'name': name, 'notes': notes})
+
+    return ret
+
+
 def list_policies(out: OutputBuffer) -> None:
     '''Prints a list of server & client policies.'''
 
     server_policy_names, client_policy_names = Policy.list_builtin_policies()
 
     if len(server_policy_names) > 0:
         out.head('\nServer policies:\n')
@@ -556,44 +679,58 @@
         source = client_host
 
     policy_data = Policy.create(source, banner, kex, aconf.client_audit)
 
     if aconf.policy_file is None:
         raise RuntimeError('Internal error: cannot write policy file since filename is None!')
 
-    # Open with mode 'x' (creates the file, or fails if it already exist).
-    succeeded = True
+    succeeded = False
+    err = ''
     try:
+        # Open with mode 'x' (creates the file, or fails if it already exist).
         with open(aconf.policy_file, 'x', encoding='utf-8') as f:
             f.write(policy_data)
+        succeeded = True
     except FileExistsError:
-        succeeded = False
+        err = "Error: file already exists: %s" % aconf.policy_file
+    except PermissionError as e:
+        # If installed as a Snap package, print a more useful message with potential work-arounds.
+        if SNAP_PACKAGE:
+            print(SNAP_PERMISSIONS_ERROR)
+            sys.exit(exitcodes.UNKNOWN_ERROR)
+        else:
+            err = "Error: insufficient permissions: %s" % str(e)
 
     if succeeded:
         print("Wrote policy to %s.  Customize as necessary, then run a policy scan with -P option." % aconf.policy_file)
     else:
-        print("Error: file already exists: %s" % aconf.policy_file)
+        print(err)
 
 
 def process_commandline(out: OutputBuffer, args: List[str], usage_cb: Callable[..., None]) -> 'AuditConf':  # pylint: disable=too-many-statements
     # pylint: disable=too-many-branches
     aconf = AuditConf()
+
+    enable_colors = not any(i in args for i in ['--no-colors', '-n'])
+    aconf.colors = enable_colors
+    out.use_colors = enable_colors
+
     try:
-        sopts = 'h1246M:p:P:jbcnvl:t:T:Lmd'
-        lopts = ['help', 'ssh1', 'ssh2', 'ipv4', 'ipv6', 'make-policy=', 'port=', 'policy=', 'json', 'batch', 'client-audit', 'no-colors', 'verbose', 'level=', 'timeout=', 'targets=', 'list-policies', 'lookup=', 'threads=', 'manual', 'debug']
+        sopts = 'h1246M:p:P:jbcnvl:t:T:Lmdg:'
+        lopts = ['help', 'ssh1', 'ssh2', 'ipv4', 'ipv6', 'make-policy=', 'port=', 'policy=', 'json', 'batch', 'client-audit', 'no-colors', 'verbose', 'level=', 'timeout=', 'targets=', 'list-policies', 'lookup=', 'threads=', 'manual', 'debug', 'gex-test=']
         opts, args = getopt.gnu_getopt(args, sopts, lopts)
     except getopt.GetoptError as err:
-        usage_cb(str(err))
+        usage_cb(out, str(err))
     aconf.ssh1, aconf.ssh2 = False, False
     host: str = ''
     oport: Optional[str] = None
     port: int = 0
     for o, a in opts:
         if o in ('-h', '--help'):
-            usage_cb()
+            usage_cb(out)
         elif o in ('-1', '--ssh1'):
             aconf.ssh1 = True
         elif o in ('-2', '--ssh2'):
             aconf.ssh2 = True
         elif o in ('-4', '--ipv4'):
             aconf.ipv4 = True
         elif o in ('-6', '--ipv6'):
@@ -601,53 +738,80 @@
         elif o in ('-p', '--port'):
             oport = a
         elif o in ('-b', '--batch'):
             aconf.batch = True
             aconf.verbose = True
         elif o in ('-c', '--client-audit'):
             aconf.client_audit = True
-        elif o in ('-n', '--no-colors'):
-            aconf.colors = False
-            out.use_colors = False
         elif o in ('-j', '--json'):
             if aconf.json:  # If specified twice, enable indent printing.
                 aconf.json_print_indent = True
             else:
                 aconf.json = True
         elif o in ('-v', '--verbose'):
             aconf.verbose = True
             out.verbose = True
         elif o in ('-l', '--level'):
             if a not in ('info', 'warn', 'fail'):
-                usage_cb('level {} is not valid'.format(a))
+                usage_cb(out, 'level {} is not valid'.format(a))
             aconf.level = a
         elif o in ('-t', '--timeout'):
             aconf.timeout = float(a)
             aconf.timeout_set = True
         elif o in ('-M', '--make-policy'):
             aconf.make_policy = True
             aconf.policy_file = a
         elif o in ('-P', '--policy'):
             aconf.policy_file = a
         elif o in ('-T', '--targets'):
             aconf.target_file = a
+
+            # If we're on Windows, and we can't use the idna workaround, force only one thread to be used (otherwise a crash would occur).
+            # if no_idna_workaround:
+            #    print("\nWARNING: the idna module was not found on this system, thus only single-threaded scanning will be done (this is a workaround for this Windows-specific crash: https://github.com/python/cpython/issues/73474).  Multi-threaded scanning can be enabled by installing the idna module (pip install idna).\n")
+            #    aconf.threads = 1
         elif o == '--threads':
             aconf.threads = int(a)
+            # if no_idna_workaround:
+            #    aconf.threads = 1
         elif o in ('-L', '--list-policies'):
             aconf.list_policies = True
         elif o == '--lookup':
             aconf.lookup = a
         elif o in ('-m', '--manual'):
             aconf.manual = True
         elif o in ('-d', '--debug'):
             aconf.debug = True
             out.debug = True
+        elif o in ('-g', '--gex-test'):
+            permitted_syntax = get_permitted_syntax_for_gex_test()
+
+            if not any(re.search(regex_str, a) for regex_str in permitted_syntax.values()):
+                usage_cb(out, '{} {} is not valid'.format(o, a))
+
+            if re.search(permitted_syntax['RANGE'], a):
+                extracted_digits = re.findall(r'\d+', a)
+                bits_left_bound = int(extracted_digits[0])
+                bits_right_bound = int(extracted_digits[1])
+
+                bits_step = 1
+                if (len(extracted_digits)) == 3:
+                    bits_step = int(extracted_digits[2])
+
+                if bits_step <= 0:
+                    usage_cb(out, '{} {} is not valid'.format(o, bits_step))
+
+                if all(x < 0 for x in (bits_left_bound, bits_right_bound)):
+                    usage_cb(out, '{} {} {} is not valid'.format(o, bits_left_bound, bits_right_bound))
+
+            aconf.gex_test = a
+
 
     if len(args) == 0 and aconf.client_audit is False and aconf.target_file is None and aconf.list_policies is False and aconf.lookup == '' and aconf.manual is False:
-        usage_cb()
+        usage_cb(out)
 
     if aconf.manual:
         return aconf
 
     if aconf.lookup != '':
         return aconf
 
@@ -657,48 +821,56 @@
 
     if aconf.client_audit is False and aconf.target_file is None:
         if oport is not None:
             host = args[0]
         else:
             host, port = Utils.parse_host_and_port(args[0])
         if not host and aconf.target_file is None:
-            usage_cb('host is empty')
+            usage_cb(out, 'host is empty')
 
     if port == 0 and oport is None:
         if aconf.client_audit:  # The default port to listen on during a client audit is 2222.
             port = 2222
         else:
             port = 22
 
     if oport is not None:
         port = Utils.parse_int(oport)
         if port <= 0 or port > 65535:
-            usage_cb('port {} is not valid'.format(oport))
+            usage_cb(out, 'port {} is not valid'.format(oport))
 
     aconf.host = host
     aconf.port = port
     if not (aconf.ssh1 or aconf.ssh2):
         aconf.ssh1, aconf.ssh2 = True, True
 
     # If a file containing a list of targets was given, read it.
     if aconf.target_file is not None:
-        with open(aconf.target_file, 'r', encoding='utf-8') as f:
-            aconf.target_list = f.readlines()
+        try:
+            with open(aconf.target_file, 'r', encoding='utf-8') as f:
+                aconf.target_list = f.readlines()
+        except PermissionError as e:
+            # If installed as a Snap package, print a more useful message with potential work-arounds.
+            if SNAP_PACKAGE:
+                print(SNAP_PERMISSIONS_ERROR)
+            else:
+                print("Error: insufficient permissions: %s" % str(e))
+            sys.exit(exitcodes.UNKNOWN_ERROR)
 
         # Strip out whitespace from each line in target file, and skip empty lines.
         aconf.target_list = [target.strip() for target in aconf.target_list if target not in ("", "\n")]
 
     # If a policy file was provided, validate it.
     if (aconf.policy_file is not None) and (aconf.make_policy is False):
 
         # First, see if this is a built-in policy name.  If not, assume a file path was provided, and try to load it from disk.
-        aconf.policy = Policy.load_builtin_policy(aconf.policy_file)
+        aconf.policy = Policy.load_builtin_policy(aconf.policy_file, json_output=aconf.json)
         if aconf.policy is None:
             try:
-                aconf.policy = Policy(policy_file=aconf.policy_file)
+                aconf.policy = Policy(policy_file=aconf.policy_file, json_output=aconf.json)
             except Exception as e:
                 out.fail("Error while loading policy file: %s: %s" % (str(e), traceback.format_exc()))
                 out.write()
                 sys.exit(exitcodes.UNKNOWN_ERROR)
 
         # If the user wants to do a client audit, but provided a server policy, terminate.
         if aconf.client_audit and aconf.policy.is_server_policy():
@@ -711,15 +883,15 @@
             out.fail("Error: server audit selected, but client policy provided.")
             out.write()
             sys.exit(exitcodes.UNKNOWN_ERROR)
 
     return aconf
 
 
-def build_struct(target_host: str, banner: Optional['Banner'], kex: Optional['SSH2_Kex'] = None, pkm: Optional['SSH1_PublicKeyMessage'] = None, client_host: Optional[str] = None) -> Any:
+def build_struct(target_host: str, banner: Optional['Banner'], cves: List[Dict[str, Union[str, float]]], kex: Optional['SSH2_Kex'] = None, pkm: Optional['SSH1_PublicKeyMessage'] = None, client_host: Optional[str] = None, software: Optional[Software] = None, algorithms: Optional[Algorithms] = None, algorithm_recommendation_suppress_list: Optional[List[str]] = None) -> Any:  # pylint: disable=too-many-arguments
 
     banner_str = ''
     banner_protocol = None
     banner_software = None
     banner_comments = None
     if banner is not None:
         banner_str = str(banner)
@@ -742,36 +914,45 @@
     else:
         res['target'] = target_host
 
     if kex is not None:
         res['compression'] = kex.server.compression
 
         res['kex'] = []
-        alg_sizes = kex.dh_modulus_sizes()
+        dh_alg_sizes = kex.dh_modulus_sizes()
         for algorithm in kex.kex_algorithms:
             entry: Any = {
                 'algorithm': algorithm,
             }
-            if algorithm in alg_sizes:
-                hostkey_size, ca_size = alg_sizes[algorithm]
+            if algorithm in dh_alg_sizes:
+                hostkey_size = dh_alg_sizes[algorithm]
                 entry['keysize'] = hostkey_size
-                if ca_size > 0:
-                    entry['casize'] = ca_size
             res['kex'].append(entry)
 
         res['key'] = []
-        alg_sizes = kex.rsa_key_sizes()
+        host_keys = kex.host_keys()
         for algorithm in kex.key_algorithms:
             entry = {
                 'algorithm': algorithm,
             }
-            if algorithm in alg_sizes:
-                hostkey_size, ca_size = alg_sizes[algorithm]
-                entry['keysize'] = hostkey_size
+            if algorithm in host_keys:
+                hostkey_info = host_keys[algorithm]
+                hostkey_size = cast(int, hostkey_info['hostkey_size'])
+
+                ca_type = ''
+                ca_size = 0
+                if 'ca_key_type' in hostkey_info:
+                    ca_type = cast(str, hostkey_info['ca_key_type'])
+                if 'ca_key_size' in hostkey_info:
+                    ca_size = cast(int, hostkey_info['ca_key_size'])
+
+                if algorithm in HostKeyTest.RSA_FAMILY or algorithm.startswith('ssh-rsa-cert-v0'):
+                    entry['keysize'] = hostkey_size
                 if ca_size > 0:
+                    entry['ca_algorithm'] = ca_type
                     entry['casize'] = ca_size
             res['key'].append(entry)
 
         res['enc'] = kex.server.encryption
         res['mac'] = kex.server.mac
         res['fingerprints'] = []
         host_keys = kex.host_keys()
@@ -783,15 +964,15 @@
                 del host_keys[host_key_type]
                 host_keys['ssh-rsa'] = val
 
         for host_key_type in sorted(host_keys):
             if host_keys[host_key_type] is None:
                 continue
 
-            fp = Fingerprint(host_keys[host_key_type])
+            fp = Fingerprint(cast(bytes, host_keys[host_key_type]['raw_hostkey_bytes']))
 
             # Skip over certificate host types (or we would return invalid fingerprints).
             if '-cert-' in host_key_type:
                 continue
 
             # Add the SHA256 and MD5 fingerprints.
             res['fingerprints'].append({
@@ -817,14 +998,20 @@
         res['enc'] = pkm_supported_ciphers
         res['aut'] = pkm_supported_authentications
         res['fingerprints'] = [{
             'type': 'ssh-rsa1',
             'fp': pkm_fp,
         }]
 
+    # Add in the CVE information.
+    res['cves'] = cves
+
+    # Add in the recommendations.
+    res['recommendations'] = get_algorithm_recommendations(algorithms, algorithm_recommendation_suppress_list, software, for_server=True)
+
     return res
 
 
 # Returns one of the exitcodes.* flags.
 def audit(out: OutputBuffer, aconf: AuditConf, sshv: Optional[int] = None, print_target: bool = False) -> int:
     program_retval = exitcodes.GOOD
     out.batch = aconf.batch
@@ -892,22 +1079,25 @@
         output(out, aconf, banner, header)
         out.fail(err)
         return exitcodes.CONNECTION_ERROR
     if sshv == 1:
         program_retval = output(out, aconf, banner, header, pkm=SSH1_PublicKeyMessage.parse(payload))
     elif sshv == 2:
         try:
-            kex = SSH2_Kex.parse(payload)
+            kex = SSH2_Kex.parse(out, payload)
         except Exception:
             out.fail("Failed to parse server's kex.  Stack trace:\n%s" % str(traceback.format_exc()))
             return exitcodes.CONNECTION_ERROR
 
         if aconf.client_audit is False:
             HostKeyTest.run(out, s, kex)
-            GEXTest.run(out, s, kex)
+            if aconf.gex_test != '':
+                return run_gex_granular_modulus_size_test(out, s, kex, aconf)
+            else:
+                GEXTest.run(out, s, kex)
 
         # This is a standard audit scan.
         if (aconf.policy is None) and (aconf.make_policy is False):
             program_retval = output(out, aconf, banner, header, client_host=s.client_host, kex=kex, print_target=print_target)
 
         # This is a policy test.
         elif (aconf.policy is not None) and (aconf.make_policy is False):
@@ -1038,14 +1228,87 @@
     if not out.use_colors:
         windows_man_page = re.sub(r'\x1b\[\d+?m', '', windows_man_page)
 
     out.info(windows_man_page)
     return retval
 
 
+def get_permitted_syntax_for_gex_test() -> Dict[str, str]:
+    syntax = {
+        'RANGE': r'^\d+-\d+(:\d+)?$',
+        'LIST_WITHOUT_MIN_PREF_MAX': r'^\d+(,\d+)*$',
+        'LIST_WITH_MIN_PREF_MAX': r'^\d+:\d+:\d+(,\d+:\d+:\d+)*$'
+    }
+    return syntax
+
+
+def run_gex_granular_modulus_size_test(out: OutputBuffer, s: 'SSH_Socket', kex: 'SSH2_Kex', aconf: AuditConf) -> int:
+    '''Extracts the user specified modulus sizes and submits them for testing against the target server.  Returns an exitcodes.* flag.'''
+
+    permitted_syntax = get_permitted_syntax_for_gex_test()
+
+    mod_dict: Dict[str, List[int]] = {}
+
+    # Range syntax.
+    if re.search(permitted_syntax['RANGE'], aconf.gex_test):
+        extracted_digits = re.findall(r'\d+', aconf.gex_test)
+        bits_left_bound = int(extracted_digits[0])
+        bits_right_bound = int(extracted_digits[1])
+
+        bits_step = 1
+        if (len(extracted_digits)) == 3:
+            bits_step = int(extracted_digits[2])
+
+        # If the left value is greater than the right value, then the sequence
+        # operates from right to left.
+        if bits_left_bound <= bits_right_bound:
+            bits_in_range_to_test = range(bits_left_bound, bits_right_bound + 1, bits_step)
+        else:
+            bits_in_range_to_test = range(bits_left_bound, bits_right_bound - 1, -abs(bits_step))
+
+        out.v("A separate test will be performed against each of the following modulus sizes: " + ", ".join([str(x) for x in bits_in_range_to_test]) + ".", write_now=True)
+
+        for i_bits in bits_in_range_to_test:
+            program_retval = GEXTest.granular_modulus_size_test(out, s, kex, i_bits, i_bits, i_bits, mod_dict)
+            if program_retval != exitcodes.GOOD:
+                return program_retval
+
+    # Two variations of list syntax.
+    if re.search(permitted_syntax['LIST_WITHOUT_MIN_PREF_MAX'], aconf.gex_test):
+        bits_in_list_to_test = aconf.gex_test.split(',')
+        out.v("A separate test will be performed against each of the following modulus sizes: " + ", ".join([str(x) for x in bits_in_list_to_test]) + ".", write_now=True)
+        for s_bits in bits_in_list_to_test:
+            program_retval = GEXTest.granular_modulus_size_test(out, s, kex, int(s_bits), int(s_bits), int(s_bits), mod_dict)
+            if program_retval != exitcodes.GOOD:
+                return program_retval
+
+    if re.search(permitted_syntax['LIST_WITH_MIN_PREF_MAX'], aconf.gex_test):
+        sets_of_min_pref_max = aconf.gex_test.split(',')
+        out.v("A separate test will be performed against each of the following sets of 'min:pref:max' modulus sizes: " + ', '.join(sets_of_min_pref_max), write_now=True)
+        for set_of_min_pref_max in sets_of_min_pref_max:
+            bits_in_list_to_test = set_of_min_pref_max.split(':')
+            program_retval = GEXTest.granular_modulus_size_test(out, s, kex, int(bits_in_list_to_test[0]), int(bits_in_list_to_test[1]), int(bits_in_list_to_test[2]), mod_dict)
+            if program_retval != exitcodes.GOOD:
+                return program_retval
+
+    if mod_dict:
+        if aconf.json:
+            json_struct = {'dh-gex-modulus-size': mod_dict}
+            out.info(json.dumps(json_struct, indent=4 if aconf.json_print_indent else None, sort_keys=True))
+        else:
+            out.head('# diffie-hellman group exchange modulus size')
+            max_key_len = len(max(mod_dict, key=len))
+
+            for key, value in mod_dict.items():
+                padding = (max_key_len - len(key)) + 1
+                out.info(key + " " * padding + '--> ' + ', '.join([str(i) for i in value]))
+
+    return program_retval
+
+
 def main() -> int:
     out = OutputBuffer()
     aconf = process_commandline(out, sys.argv[1:], usage)
 
     # If we're on Windows, but the colorama module could not be imported, print a warning if we're in verbose mode.
     if (sys.platform == 'win32') and ('colorama' not in sys.modules):
         out.v("WARNING: colorama module not found.  Colorized output will be disabled.", write_now=True)
@@ -1079,15 +1342,15 @@
 
         # Loop through each target in the list.
         target_servers = []
         for _, target in enumerate(aconf.target_list):
             host, port = Utils.parse_host_and_port(target, default_port=22)
             target_servers.append((host, port))
 
-        # A ranked list of return codes.  Those with higher indices will take precendence over lower ones.  For example, if three servers are scanned, yielding WARNING, GOOD, and UNKNOWN_ERROR, the overall result will be UNKNOWN_ERROR, since its index is the highest.  Errors have highest priority, followed by failures, then warnings.
+        # A ranked list of return codes.  Those with higher indices will take precedence over lower ones.  For example, if three servers are scanned, yielding WARNING, GOOD, and UNKNOWN_ERROR, the overall result will be UNKNOWN_ERROR, since its index is the highest.  Errors have highest priority, followed by failures, then warnings.
         ranked_return_codes = [exitcodes.GOOD, exitcodes.WARNING, exitcodes.FAILURE, exitcodes.CONNECTION_ERROR, exitcodes.UNKNOWN_ERROR]
 
         # Queue all worker threads.
         num_target_servers = len(target_servers)
         num_processed = 0
         out.v("Scanning %u targets with %s%u threads..." % (num_target_servers, '(at most) ' if aconf.threads > num_target_servers else '',  aconf.threads), write_now=True)
         with concurrent.futures.ThreadPoolExecutor(max_workers=aconf.threads) as executor:
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/ssh_socket.py` & `ssh-audit-2.9.0/src/ssh_audit/ssh_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             family = socket.AF_UNSPEC
         try:
             stype = socket.SOCK_STREAM
             r = socket.getaddrinfo(self.__host, self.__port, family, stype)
 
             # If the user has a preference for using IPv4 over IPv6 (or vice-versa), then sort the list returned by getaddrinfo() so that the preferred address type comes first.
             if len(self.__ip_version_preference) == 2:
-                r = sorted(r, key=lambda x: x[0], reverse=(self.__ip_version_preference[0] == 6))
+                r = sorted(r, key=lambda x: x[0], reverse=(self.__ip_version_preference[0] == 6))  # pylint: disable=superfluous-parens
             for af, socktype, _proto, _canonname, addr in r:
                 if socktype == socket.SOCK_STREAM:
                     yield af, addr
         except socket.error as e:
             self.__outputbuffer.fail('[exception] {}'.format(e)).write()
             sys.exit(exitcodes.CONNECTION_ERROR)
 
@@ -232,15 +232,15 @@
     # Send a KEXINIT with the lists of key exchanges, hostkeys, ciphers, MACs, compressions, and languages that we "support".
     def send_kexinit(self, key_exchanges: List[str] = ['curve25519-sha256', 'curve25519-sha256@libssh.org', 'ecdh-sha2-nistp256', 'ecdh-sha2-nistp384', 'ecdh-sha2-nistp521', 'diffie-hellman-group-exchange-sha256', 'diffie-hellman-group16-sha512', 'diffie-hellman-group18-sha512', 'diffie-hellman-group14-sha256'], hostkeys: List[str] = ['rsa-sha2-512', 'rsa-sha2-256', 'ssh-rsa', 'ecdsa-sha2-nistp256', 'ssh-ed25519'], ciphers: List[str] = ['chacha20-poly1305@openssh.com', 'aes128-ctr', 'aes192-ctr', 'aes256-ctr', 'aes128-gcm@openssh.com', 'aes256-gcm@openssh.com'], macs: List[str] = ['umac-64-etm@openssh.com', 'umac-128-etm@openssh.com', 'hmac-sha2-256-etm@openssh.com', 'hmac-sha2-512-etm@openssh.com', 'hmac-sha1-etm@openssh.com', 'umac-64@openssh.com', 'umac-128@openssh.com', 'hmac-sha2-256', 'hmac-sha2-512', 'hmac-sha1'], compressions: List[str] = ['none', 'zlib@openssh.com'], languages: List[str] = ['']) -> None:  # pylint: disable=dangerous-default-value
         '''Sends the list of supported host keys, key exchanges, ciphers, and MACs.  Emulates OpenSSH v8.2.'''
 
         self.__outputbuffer.d('KEX initialisation...', write_now=True)
 
         kexparty = SSH2_KexParty(ciphers, macs, compressions, languages)
-        kex = SSH2_Kex(os.urandom(16), key_exchanges, hostkeys, kexparty, kexparty, False, 0)
+        kex = SSH2_Kex(self.__outputbuffer, os.urandom(16), key_exchanges, hostkeys, kexparty, kexparty, False, 0)
 
         self.write_byte(Protocol.MSG_KEXINIT)
         kex.write(self)
         self.send_packet()
 
     def send_banner(self, banner: str) -> None:
         self.send(banner.encode() + b'\r\n')
@@ -321,15 +321,15 @@
     def close(self) -> None:
         self.__cleanup()
         self.reset()
         self.__state = 0
         self.__header = []
         self.__banner = None
 
-    def _close_socket(self, s: Optional[socket.socket]) -> None:  # pylint: disable=no-self-use
+    def _close_socket(self, s: Optional[socket.socket]) -> None:
         try:
             if s is not None:
                 s.shutdown(socket.SHUT_RDWR)
                 s.close()  # pragma: nocover
         except Exception:
             pass
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/timeframe.py` & `ssh-audit-2.9.0/src/ssh_audit/timeframe.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/utils.py` & `ssh-audit-2.9.0/src/ssh_audit/utils.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit/versionvulnerabilitydb.py` & `ssh-audit-2.9.0/src/ssh_audit/versionvulnerabilitydb.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     # Format: [starting_vuln_version, last_vuln_version, affected, CVE_ID, CVSSv2, description]
     #   affected: 1 = server, 2 = client, 4 = local
     #   Example:  if it affects servers, both remote & local, then affected
     #             = 1.  If it affects servers, but is a local issue only,
     #             then affected = 1 + 4 = 5.
     CVE: Dict[str, List[List[Any]]] = {
         'Dropbear SSH': [
+            ['0.0', '2020.81', 2, 'CVE-2021-36369', 7.5, 'trivial authentication attack to bypass FIDO tokens and SSH-ASKPASS'],
             ['0.0', '2018.76', 1, 'CVE-2018-15599', 5.0, 'remote users may enumerate users on the system'],
             ['0.0', '2017.74', 5, 'CVE-2017-9079', 4.7, 'local users can read certain files as root'],
             ['0.0', '2017.74', 5, 'CVE-2017-9078', 9.3, 'local users may elevate privileges to root under certain conditions'],
             ['0.0', '2016.73', 5, 'CVE-2016-7409', 2.1, 'local users can read process memory under limited conditions'],
             ['0.0', '2016.73', 1, 'CVE-2016-7408', 6.5, 'remote users can execute arbitrary code'],
             ['0.0', '2016.73', 5, 'CVE-2016-7407', 10.0, 'local users can execute arbitrary code'],
             ['0.0', '2016.73', 1, 'CVE-2016-7406', 10.0, 'remote users can execute arbitrary code'],
@@ -62,15 +63,29 @@
             ['0.4.7', '0.5.3',  1, 'CVE-2013-0176', 4.3, 'cause DoS via kex packet (null pointer dereference)'],
             ['0.4.7', '0.5.2',  1, 'CVE-2012-6063', 7.5, 'cause DoS or execute arbitrary code via sftp (double free)'],
             ['0.4.7', '0.5.2',  1, 'CVE-2012-4562', 7.5, 'cause DoS or execute arbitrary code (overflow check)'],
             ['0.4.7', '0.5.2',  1, 'CVE-2012-4561', 5.0, 'cause DoS via unspecified vectors (invalid pointer)'],
             ['0.4.7', '0.5.2',  1, 'CVE-2012-4560', 7.5, 'cause DoS or execute arbitrary code (buffer overflow)'],
             ['0.4.7', '0.5.2',  1, 'CVE-2012-4559', 6.8, 'cause DoS or execute arbitrary code (double free)']],
         'OpenSSH': [
-            ['1.0',     '7.7',     1, 'CVE-2018-15473', 5.3, 'enumerate usernames due to timing discrepencies'],
+            ['6.2',     '8.7',     5, 'CVE-2021-41617', 7.0, 'privilege escalation via supplemental groups'],
+            ['1.0',     '8.8',     2, 'CVE-2021-36368', 3.7, 'trivial authentication attack to bypass FIDO tokens and SSH-ASKPASS'],
+            ['8.2',     '8.4',     2, 'CVE-2021-28041', 7.1, 'double free via ssh-agent'],
+            ['1.0',     '8.3',     5, 'CVE-2020-15778', 7.8, 'command injection via anomalous argument transfers'],
+            ['5.7',     '8.3',     2, 'CVE-2020-14145', 5.9, 'information leak via algorithm negotiation'],
+            ['8.2',     '8.2',     2, 'CVE-2020-12062', 7.5, 'arbitrary files overwrite via scp'],
+            ['7.7',     '8.0',     7, 'CVE-2019-16905', 7.8, 'memory corruption and local code execution via pre-authentication integer overflow'],
+            ['1.0',     '7.9',     2, 'CVE-2019-6111',  5.9, 'arbitrary files overwrite via scp'],
+            ['1.0',     '7.9',     2, 'CVE-2019-6110',  6.8, 'output manipulation'],
+            ['1.0',     '7.9',     2, 'CVE-2019-6109',  6.8, 'output manipulation'],
+            ['1.0',     '7.9',     2, 'CVE-2018-20685', 5.3, 'directory permissions modification via scp'],
+            ['5.9',     '7.8',     1, 'CVE-2018-15919', 5.3, 'username enumeration via GS2'],
+            ['1.0',     '7.7',     1, 'CVE-2018-15473', 5.3, 'enumerate usernames due to timing discrepancies'],
+            ['1.2',     '6.292',   1, 'CVE-2017-15906', 5.3, 'readonly bypass via sftp'],
+            ['1.0',     '8.7',     1, 'CVE-2016-20012', 5.3, 'enumerate usernames via challenge response'],
             ['7.2',     '7.2p2',   1, 'CVE-2016-6515',  7.8, 'cause DoS via long password string (crypt CPU consumption)'],
             ['1.2.2',   '7.2',     1, 'CVE-2016-3115',  5.5, 'bypass command restrictions via crafted X11 forwarding data'],
             ['5.4',     '7.1',     1, 'CVE-2016-1907',  5.0, 'cause DoS via crafted network traffic (out of bounds read)'],
             ['5.4',     '7.1p1',   2, 'CVE-2016-0778',  4.6, 'cause DoS via requesting many forwardings (heap based buffer overflow)'],
             ['5.0',     '7.1p1',   2, 'CVE-2016-0777',  4.0, 'leak data via allowing transfer of entire buffer'],
             ['6.0',     '7.2p2',   5, 'CVE-2015-8325',  7.2, 'privilege escalation via triggering crafted environment'],
             ['6.8',     '6.9',     5, 'CVE-2015-6565',  7.2, 'cause DoS via writing to a device (terminal disruption)'],
@@ -121,14 +136,18 @@
             ['2.1',     '3.2',     1, 'CVE-2002-0575',  7.5, 'privilege escalation'],
             ['2.1',     '3.0.2p1', 2, 'CVE-2002-0083', 10.0, 'privilege escalation'],
             ['3.0',     '3.0p1',   1, 'CVE-2001-1507',  7.5, 'bypass authentication'],
             ['1.2.3',   '3.0.1p1', 5, 'CVE-2001-0872',  7.2, 'privilege escalation via crafted environment variables'],
             ['1.2.3',   '2.1.1',   1, 'CVE-2001-0361',  4.0, 'recover plaintext from ciphertext'],
             ['1.2',     '2.1',     1, 'CVE-2000-0525', 10.0, 'execute arbitrary code (improper privileges)']],
         'PuTTY': [
+            # info for CVE-2021-36367 - only PuTTY up to 0.71 is affected - see https://www.chiark.greenend.org.uk/~sgtatham/putty/wishlist/reject-trivial-auth.html
+            ['0.0', '0.71', 2, 'CVE-2021-36367', 8.1, 'trivial authentication attack to bypass FIDO tokens and SSH-ASKPASS'],
+            ['0.0', '0.74', 2, 'CVE-2021-33500', 5.0, 'denial of service of the complete windows desktop'],
+            ['0.68', '0.73', 2, 'CVE-2020-14002', 4.3, 'Observable Discrepancy which allows man-in-the-middle attackers to target initial connection attempts'],
             ['0.54', '0.73', 2, 'CVE-2020-XXXX', 5.0, 'out of bounds memory read'],
             ['0.0', '0.72', 2, 'CVE-2019-17069', 5.0, 'potential DOS by remote SSHv1 server'],
             ['0.71', '0.72', 2, 'CVE-2019-17068', 5.0, 'xterm bracketed paste mode command injection'],
             ['0.52', '0.72', 2, 'CVE-2019-17067', 7.5, 'port rebinding weakness in port forward tunnel handling'],
             ['0.0', '0.71', 2, 'CVE-2019-XXXX', 5.0, 'undefined vulnerability in obsolete SSHv1 protocol handling'],
             ['0.0', '0.71', 6, 'CVE-2019-XXXX', 5.0, 'local privilege escalation in Pageant'],
             ['0.0', '0.70', 2, 'CVE-2019-9898', 7.5, 'potential recycling of random numbers'],
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit/writebuf.py` & `ssh-audit-2.9.0/src/ssh_audit/writebuf.py`

 * *Files identical despite different names*

### Comparing `ssh-audit-2.5.0/src/ssh_audit.egg-info/PKG-INFO` & `ssh-audit-2.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,349 +1,374 @@
 Metadata-Version: 2.1
 Name: ssh-audit
-Version: 2.5.0
+Version: 2.9.0
 Summary: An SSH server & client configuration security auditing tool
 Home-page: https://github.com/jtesta/ssh-audit
 Author: Joe Testa
 Author-email: jtesta@positronsecurity.com
-License: UNKNOWN
+License: MIT
 Project-URL: Source Code, https://github.com/jtesta/ssh-audit
 Project-URL: Bug Tracker, https://github.com/jtesta/ssh-audit/issues
-Description: # ssh-audit
-        [![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/LICENSE)
-        [![PyPI Downloads](https://img.shields.io/pypi/dm/ssh-audit)](https://pypi.org/project/ssh-audit/)
-        [![Docker Pulls](https://img.shields.io/docker/pulls/positronsecurity/ssh-audit)](https://hub.docker.com/r/positronsecurity/ssh-audit)
-        [![Build Status](https://github.com/jtesta/ssh-audit/actions/workflows/tox.yaml/badge.svg)](https://github.com/jtesta/ssh-audit/actions)
-        [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/CONTRIBUTING.md)
-        
-        **ssh-audit** is a tool for ssh server & client configuration auditing.
-        
-        [jtesta/ssh-audit](https://github.com/jtesta/ssh-audit/) (v2.0+) is the updated and maintained version of ssh-audit forked from [arthepsy/ssh-audit](https://github.com/arthepsy/ssh-audit) (v1.x) due to inactivity.
-        
-        - [Features](#features)
-        - [Usage](#usage)
-        - [Screenshots](#screenshots)
-            - [Server Standard Audit Example](#server-standard-audit-example)
-            - [Server Policy Audit Example](#server-policy-audit-example)
-            - [Client Standard Audit Example](#client-standard-audit-example)
-        - [Hardening Guides](#hardening-guides)
-        - [Pre-Built Packages](#pre-built-packages)
-        - [Web Front-End](#web-front-end)
-        - [ChangeLog](#changelog)
-        
-        ## Features
-        - SSH1 and SSH2 protocol server support;
-        - analyze SSH client configuration;
-        - grab banner, recognize device or software and operating system, detect compression;
-        - gather key-exchange, host-key, encryption and message authentication code algorithms;
-        - output algorithm information (available since, removed/disabled, unsafe/weak/legacy, etc);
-        - output algorithm recommendations (append or remove based on recognized software version);
-        - output security information (related issues, assigned CVE list, etc);
-        - analyze SSH version compatibility based on algorithm information;
-        - historical information from OpenSSH, Dropbear SSH and libssh;
-        - policy scans to ensure adherence to a hardened/standard configuration;
-        - runs on Linux and Windows;
-        - supports Python 3.6 - 3.9;
-        - no dependencies
-        
-        ## Usage
-        ```
-        usage: ssh-audit.py [options] <host>
-        
-           -h,  --help             print this help
-           -1,  --ssh1             force ssh version 1 only
-           -2,  --ssh2             force ssh version 2 only
-           -4,  --ipv4             enable IPv4 (order of precedence)
-           -6,  --ipv6             enable IPv6 (order of precedence)
-           -b,  --batch            batch output
-           -c,  --client-audit     starts a server on port 2222 to audit client
-                                       software config (use -p to change port;
-                                       use -t to change timeout)
-           -d,  --debug            Enable debug output.
-           -j,  --json             JSON output (use -jj to enable indents)
-           -l,  --level=<level>    minimum output level (info|warn|fail)
-           -L,  --list-policies    list all the official, built-in policies
-                --lookup=<alg1,alg2,...>    looks up an algorithm(s) without
-                                            connecting to a server
-           -m,  --manual           print the man page (Windows only)
-           -M,  --make-policy=<policy.txt>  creates a policy based on the target server
-                                            (i.e.: the target server has the ideal
-                                            configuration that other servers should
-                                            adhere to)
-           -n,  --no-colors        disable colors
-           -p,  --port=<port>      port to connect
-           -P,  --policy=<"policy name" | policy.txt>  run a policy test using the
-                                                           specified policy
-           -t,  --timeout=<secs>   timeout (in seconds) for connection and reading
-                                       (default: 5)
-           -T,  --targets=<hosts.txt>  a file containing a list of target hosts (one
-                                           per line, format HOST[:PORT])
-                --threads=<threads>    number of threads to use when scanning multiple
-                                           targets (-T/--targets) (default: 32)
-           -v,  --verbose          verbose output
-        ```
-        * if both IPv4 and IPv6 are used, order of precedence can be set by using either `-46` or `-64`.  
-        * batch flag `-b` will output sections without header and without empty lines (implies verbose flag).  
-        * verbose flag `-v` will prefix each line with section type and algorithm name.  
-        * an exit code of 0 is returned when all algorithms are considered secure (for a standard audit), or when a policy check passes (for a policy audit).
-        
-        Basic server auditing:
-        ```
-        ssh-audit localhost
-        ssh-audit 127.0.0.1
-        ssh-audit 127.0.0.1:222
-        ssh-audit ::1
-        ssh-audit [::1]:222
-        ```
-        
-        To run a standard audit against many servers (place targets into servers.txt, one on each line in the format of `HOST[:PORT]`):
-        
-        ```
-        ssh-audit -T servers.txt
-        ```
-        
-        To audit a client configuration (listens on port 2222 by default; connect using `ssh -p 2222 anything@localhost`):
-        
-        ```
-        ssh-audit -c
-        ```
-        
-        To audit a client configuration, with a listener on port 4567:
-        ```
-        ssh-audit -c -p 4567
-        ```
-        
-        To  list all official built-in policies (hint: use resulting policy names with `-P`/`--policy`):
-        ```
-        ssh-audit -L
-        ```
-        
-        To run a policy audit against a server:
-        ```
-        ssh-audit -P ["policy name" | path/to/server_policy.txt] targetserver
-        ```
-        
-        To run a policy audit against a client:
-        ```
-        ssh-audit -c -P ["policy name" | path/to/client_policy.txt]
-        ```
-        
-        To run a policy audit against many servers:
-        ```
-        ssh-audit -T servers.txt -P ["policy name" | path/to/server_policy.txt]
-        ```
-        
-        To create a policy based on a target server (which can be manually edited):
-        ```
-        ssh-audit -M new_policy.txt targetserver
-        ```
-        
-        ## Screenshots
-        
-        ### Server Standard Audit Example
-        Below is a screen shot of the standard server-auditing output when connecting to an unhardened OpenSSH v5.3 service:
-        ![screenshot](https://user-images.githubusercontent.com/2982011/64388792-317e6f80-d00e-11e9-826e-a4934769bb07.png)
-        
-        ### Server Policy Audit Example
-        Below is a screen shot of the policy auditing output when connecting to an un-hardened Ubuntu Server 20.04 machine (hint: use `-L`/`--list-policies` to see names of built-in policies to use with `-P`/`--policy`):
-        ![screenshot](https://user-images.githubusercontent.com/2982011/94370881-95178700-00c0-11eb-8705-3157a4669dc0.png)
-        
-        After applying the steps in the hardening guide (see below), the output changes to the following:
-        ![screenshot](https://user-images.githubusercontent.com/2982011/94370873-87620180-00c0-11eb-9a59-469f61a56ce1.png)
-        
-        ### Client Standard Audit Example
-        Below is a screen shot of the client-auditing output when an unhardened OpenSSH v7.2 client connects:
-        ![client_screenshot](https://user-images.githubusercontent.com/2982011/68867998-b946c100-06c4-11ea-975f-1f47e4178a74.png)
-        
-        ## Hardening Guides
-        Guides to harden server & client configuration can be found here: [https://www.ssh-audit.com/hardening_guides.html](https://www.ssh-audit.com/hardening_guides.html)
-        
-        ## Pre-Built Packages
-        Pre-built packages are available for Windows (see the releases page), on PyPI, Snap, and Homebrew.
-        
-        To install from PyPI:
-        ```
-        $ pip3 install ssh-audit
-        ```
-        
-        To install the Snap package:
-        ```
-        $ snap install ssh-audit
-        ```
-        
-        To install on Homebrew:
-        ```
-        $ brew install ssh-audit
-        ```
-        
-        To install from Dockerhub:
-        ```
-        $ docker pull positronsecurity/ssh-audit
-        ```
-        (Then run with: `docker run -it -p 2222:2222 positronsecurity/ssh-audit 10.1.1.1`)
-        
-        ## Web Front-End
-        For convenience, a web front-end on top of the command-line tool is available at [https://www.ssh-audit.com/](https://www.ssh-audit.com/).
-        
-        ## ChangeLog
-        ### v2.5.0 (2021-08-26)
-         - Fixed crash when running host key tests.
-         - Handles server connection failures more gracefully.
-         - Now prints JSON with indents when `-jj` is used (useful for debugging).
-         - Added MD5 fingerprints to verbose output.
-         - Added `-d`/`--debug` option for getting debugging output; credit [Adam Russell](https://github.com/thecliguy).
-         - Updated JSON output to include MD5 fingerprints.  Note that this results in a breaking change in the 'fingerprints' dictionary format.
-         - Updated OpenSSH 8.1 (and earlier) policies to include `rsa-sha2-512` and `rsa-sha2-256`.
-         - Added OpenSSH v8.6 & v8.7 policies.
-         - Added 3 new key exchanges: `gss-gex-sha1-eipGX3TCiQSrx573bT1o1Q==`, `gss-group1-sha1-eipGX3TCiQSrx573bT1o1Q==`, and `gss-group14-sha1-eipGX3TCiQSrx573bT1o1Q==`.
-         - Added 3 new MACs: `hmac-ripemd160-96`, `AEAD_AES_128_GCM`, and `AEAD_AES_256_GCM`.
-        
-        ### v2.4.0 (2021-02-23)
-         - Added multi-threaded scanning support.
-         - Added built-in Windows manual page (see `-m`/`--manual`); credit [Adam Russell](https://github.com/thecliguy).
-         - Added version check for OpenSSH user enumeration (CVE-2018-15473).
-         - Added deprecation note to host key types based on SHA-1.
-         - Added extra warnings for SSHv1.
-         - Added built-in hardened OpenSSH v8.5 policy.
-         - Upgraded warnings to failures for host key types based on SHA-1.
-         - Fixed crash when receiving unexpected response during host key test.
-         - Fixed hang against older Cisco devices during host key test & gex test.
-         - Fixed improper termination while scanning multiple targets when one target returns an error.
-         - Dropped support for Python 3.5 (which reached EOL in Sept. 2020).
-         - Added 1 new key exchange: `sntrup761x25519-sha512@openssh.com`.
-        
-        ### v2.3.1 (2020-10-28)
-         - Now parses public key sizes for `rsa-sha2-256-cert-v01@openssh.com` and `rsa-sha2-512-cert-v01@openssh.com` host key types.
-         - Flag `ssh-rsa-cert-v01@openssh.com` as a failure due to SHA-1 hash.
-         - Fixed bug in recommendation output which suppressed some algorithms inappropriately.
-         - Built-in policies now include CA key requirements (if certificates are in use).
-         - Lookup function (`--lookup`) now performs case-insensitive lookups of similar algorithms; credit [Adam Russell](https://github.com/thecliguy).
-         - Migrated pre-made policies from external files to internal database.
-         - Split single 3,500 line script into many files (by class).
-         - Added setup.py support; credit [Ganden Schaffner](https://github.com/gschaffner).
-         - Added 1 new cipher: `des-cbc@ssh.com`.
-        
-        ### v2.3.0 (2020-09-27)
-         - Added new policy auditing functionality to test adherence to a hardening guide/standard configuration (see `-L`/`--list-policies`, `-M`/`--make-policy` and `-P`/`--policy`).  For an in-depth tutorial, see <https://www.positronsecurity.com/blog/2020-09-27-ssh-policy-configuration-checks-with-ssh-audit/>.
-         - Created new man page (see `ssh-audit.1` file).
-         - 1024-bit moduli upgraded from warnings to failures.
-         - Many Python 2 code clean-ups, testing framework improvements, pylint & flake8 fixes, and mypy type comments; credit [Jürgen Gmach](https://github.com/jugmac00).
-         - Added feature to look up algorithms in internal database (see `--lookup`); credit [Adam Russell](https://github.com/thecliguy).
-         - Suppress recommendation of token host key types.
-         - Added check for use-after-free vulnerability in PuTTY v0.73.
-         - Added 11 new host key types: `ssh-rsa1`, `ssh-dss-sha256@ssh.com`, `ssh-gost2001`, `ssh-gost2012-256`, `ssh-gost2012-512`, `spki-sign-rsa`, `ssh-ed448`, `x509v3-ecdsa-sha2-nistp256`, `x509v3-ecdsa-sha2-nistp384`, `x509v3-ecdsa-sha2-nistp521`, `x509v3-rsa2048-sha256`.
-         - Added 8 new key exchanges: `diffie-hellman-group1-sha256`, `kexAlgoCurve25519SHA256`, `Curve25519SHA256`, `gss-group14-sha256-`, `gss-group15-sha512-`, `gss-group16-sha512-`, `gss-nistp256-sha256-`, `gss-curve25519-sha256-`.
-         - Added 5 new ciphers: `blowfish`, `AEAD_AES_128_GCM`, `AEAD_AES_256_GCM`, `crypticore128@ssh.com`, `seed-cbc@ssh.com`.
-         - Added 3 new MACs: `chacha20-poly1305@openssh.com`, `hmac-sha3-224`, `crypticore-mac@ssh.com`.
-        
-        ### v2.2.0 (2020-03-11)
-         - Marked host key type `ssh-rsa` as weak due to [practical SHA-1 collisions](https://eprint.iacr.org/2020/014.pdf).
-         - Added Windows builds.
-         - Added 10 new host key types: `ecdsa-sha2-1.3.132.0.10`, `x509v3-sign-dss`, `x509v3-sign-rsa`, `x509v3-sign-rsa-sha256@ssh.com`, `x509v3-ssh-dss`, `x509v3-ssh-rsa`, `sk-ecdsa-sha2-nistp256-cert-v01@openssh.com`, `sk-ecdsa-sha2-nistp256@openssh.com`, `sk-ssh-ed25519-cert-v01@openssh.com`, and `sk-ssh-ed25519@openssh.com`.
-         - Added 18 new key exchanges: `diffie-hellman-group14-sha256@ssh.com`, `diffie-hellman-group15-sha256@ssh.com`, `diffie-hellman-group15-sha384@ssh.com`, `diffie-hellman-group16-sha384@ssh.com`, `diffie-hellman-group16-sha512@ssh.com`, `diffie-hellman-group18-sha512@ssh.com`, `ecdh-sha2-curve25519`, `ecdh-sha2-nistb233`, `ecdh-sha2-nistb409`, `ecdh-sha2-nistk163`, `ecdh-sha2-nistk233`, `ecdh-sha2-nistk283`, `ecdh-sha2-nistk409`, `ecdh-sha2-nistp192`, `ecdh-sha2-nistp224`, `ecdh-sha2-nistt571`, `gss-gex-sha1-`, and `gss-group1-sha1-`.
-         - Added 9 new ciphers: `camellia128-cbc`, `camellia128-ctr`, `camellia192-cbc`, `camellia192-ctr`, `camellia256-cbc`, `camellia256-ctr`, `aes128-gcm`, `aes256-gcm`, and `chacha20-poly1305`.
-         - Added 2 new MACs: `aes128-gcm` and `aes256-gcm`.
-        
-        ### v2.1.1 (2019-11-26)
-         - Added 2 new host key types: `rsa-sha2-256-cert-v01@openssh.com`, `rsa-sha2-512-cert-v01@openssh.com`.
-         - Added 2 new ciphers: `des`, `3des`.
-         - Added 3 new PuTTY vulnerabilities.
-         - During client testing, client IP address is now listed in output.
-        
-        ### v2.1.0 (2019-11-14)
-         - Added client software auditing functionality (see `-c` / `--client-audit` option).
-         - Added JSON output option (see `-j` / `--json` option; credit [Andreas Jaggi](https://github.com/x-way)).
-         - Fixed crash while scanning Solaris Sun_SSH.
-         - Added 9 new key exchanges: `gss-group1-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-gex-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha1-`, `gss-group14-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha256-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group15-sha512-toWM5Slw5Ew8Mqkay+al2g==`, `diffie-hellman-group15-sha256`, `ecdh-sha2-1.3.132.0.10`, `curve448-sha512`.
-         - Added 1 new host key type: `ecdsa-sha2-1.3.132.0.10`.
-         - Added 4 new ciphers: `idea-cbc`, `serpent128-cbc`, `serpent192-cbc`, `serpent256-cbc`.
-         - Added 6 new MACs: `hmac-sha2-256-96-etm@openssh.com`, `hmac-sha2-512-96-etm@openssh.com`, `hmac-ripemd`, `hmac-sha256-96@ssh.com`, `umac-32@openssh.com`, `umac-96@openssh.com`.
-        
-        ### v2.0.0 (2019-08-29)
-         - Forked from https://github.com/arthepsy/ssh-audit (development was stalled, and developer went MIA).
-         - Added RSA host key length test.
-         - Added RSA certificate key length test.
-         - Added Diffie-Hellman modulus size test.
-         - Now outputs host key fingerprints for RSA and ED25519.
-         - Added 5 new key exchanges: `sntrup4591761x25519-sha512@tinyssh.org`, `diffie-hellman-group-exchange-sha256@ssh.com`, `diffie-hellman-group-exchange-sha512@ssh.com`, `diffie-hellman-group16-sha256`, `diffie-hellman-group17-sha512`.
-         - Added 3 new encryption algorithms: `des-cbc-ssh1`, `blowfish-ctr`, `twofish-ctr`.
-         - Added 10 new MACs: `hmac-sha2-56`, `hmac-sha2-224`, `hmac-sha2-384`, `hmac-sha3-256`, `hmac-sha3-384`, `hmac-sha3-512`, `hmac-sha256`, `hmac-sha256@ssh.com`, `hmac-sha512`, `hmac-512@ssh.com`.
-         - Added command line argument (`-t` / `--timeout`) for connection & reading timeouts.
-         - Updated CVEs for libssh & Dropbear.
-        
-        ### v1.7.0 (2016-10-26)
-         - implement options to allow specify IPv4/IPv6 usage and order of precedence
-         - implement option to specify remote port (old behavior kept for compatibility)
-         - add colors support for Microsoft Windows via optional colorama dependency
-         - fix encoding and decoding issues, add tests, do not crash on encoding errors
-         - use mypy-lang for static type checking and verify all code
-        
-        ### v1.6.0 (2016-10-14)
-         - implement algorithm recommendations section (based on recognized software)
-         - implement full libssh support (version history, algorithms, security, etc)
-         - fix SSH-1.99 banner recognition and version comparison functionality
-         - do not output empty algorithms (happens for misconfigured servers)
-         - make consistent output for Python 3.x versions
-         - add a lot more tests (conf, banner, software, SSH1/SSH2, output, etc)
-         - use Travis CI to test for multiple Python versions (2.6-3.5, pypy, pypy3)
-        
-        ### v1.5.0 (2016-09-20)
-         - create security section for related security information
-         - match and output assigned CVE list and security issues for Dropbear SSH
-         - implement full SSH1 support with fingerprint information
-         - automatically fallback to SSH1 on protocol mismatch
-         - add new options to force SSH1 or SSH2 (both allowed by default)
-         - parse banner information and convert it to specific software and OS version
-         - do not use padding in batch mode
-         - several fixes (Cisco sshd, rare hangs, error handling, etc)
-        
-        ### v1.0.20160902
-         - implement batch output option
-         - implement minimum output level option
-         - fix compatibility with Python 2.6
-        
-        ### v1.0.20160812
-         - implement SSH version compatibility feature
-         - fix wrong mac algorithm warning
-         - fix Dropbear SSH version typo
-         - parse pre-banner header
-         - better errors handling
-        
-        ### v1.0.20160803
-         - use OpenSSH 7.3 banner
-         - add new key-exchange algorithms
-        
-        ### v1.0.20160207
-         - use OpenSSH 7.2 banner
-         - additional warnings for OpenSSH 7.2 
-         - fix OpenSSH 7.0 failure messages
-         - add rijndael-cbc failure message from OpenSSH 6.7
-        
-        ### v1.0.20160105
-         - multiple additional warnings
-         - support for none algorithm
-         - better compression handling  
-         - ensure reading enough data (fixes few Linux SSH)  
-        
-        ### v1.0.20151230
-         - Dropbear SSH support  
-        
-        ### v1.0.20151223
-         - initial version  
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: <4,>=3.6
+Requires-Python: <4,>=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ssh-audit
+[![License](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/LICENSE)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/ssh-audit)](https://pypi.org/project/ssh-audit/)
+[![Docker Pulls](https://img.shields.io/docker/pulls/positronsecurity/ssh-audit)](https://hub.docker.com/r/positronsecurity/ssh-audit)
+[![Build Status](https://github.com/jtesta/ssh-audit/actions/workflows/tox.yaml/badge.svg)](https://github.com/jtesta/ssh-audit/actions)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/jtesta/ssh-audit/blob/master/CONTRIBUTING.md)
+
+**ssh-audit** is a tool for ssh server & client configuration auditing.
+
+[jtesta/ssh-audit](https://github.com/jtesta/ssh-audit/) (v2.0+) is the updated and maintained version of ssh-audit forked from [arthepsy/ssh-audit](https://github.com/arthepsy/ssh-audit) (v1.x) due to inactivity.
+
+- [Features](#features)
+- [Usage](#usage)
+- [Screenshots](#screenshots)
+    - [Server Standard Audit Example](#server-standard-audit-example)
+    - [Server Policy Audit Example](#server-policy-audit-example)
+    - [Client Standard Audit Example](#client-standard-audit-example)
+- [Hardening Guides](#hardening-guides)
+- [Pre-Built Packages](#pre-built-packages)
+- [Web Front-End](#web-front-end)
+- [ChangeLog](#changelog)
+
+## Features
+- SSH1 and SSH2 protocol server support;
+- analyze SSH client configuration;
+- grab banner, recognize device or software and operating system, detect compression;
+- gather key-exchange, host-key, encryption and message authentication code algorithms;
+- output algorithm information (available since, removed/disabled, unsafe/weak/legacy, etc);
+- output algorithm recommendations (append or remove based on recognized software version);
+- output security information (related issues, assigned CVE list, etc);
+- analyze SSH version compatibility based on algorithm information;
+- historical information from OpenSSH, Dropbear SSH and libssh;
+- policy scans to ensure adherence to a hardened/standard configuration;
+- runs on Linux and Windows;
+- supports Python 3.7 - 3.11;
+- no dependencies
+
+## Usage
+```
+usage: ssh-audit.py [options] <host>
+
+   -h,  --help             print this help
+   -1,  --ssh1             force ssh version 1 only
+   -2,  --ssh2             force ssh version 2 only
+   -4,  --ipv4             enable IPv4 (order of precedence)
+   -6,  --ipv6             enable IPv6 (order of precedence)
+   -b,  --batch            batch output
+   -c,  --client-audit     starts a server on port 2222 to audit client
+                               software config (use -p to change port;
+                               use -t to change timeout)
+   -d,  --debug            Enable debug output.
+   -g,  --gex-test=<x[,y,...]>  dh gex modulus size test
+                   <min1:pref1:max1[,min2:pref2:max2,...]>
+                   <x-y[:step]>
+   -j,  --json             JSON output (use -jj to enable indents)
+   -l,  --level=<level>    minimum output level (info|warn|fail)
+   -L,  --list-policies    list all the official, built-in policies
+        --lookup=<alg1,alg2,...>    looks up an algorithm(s) without
+                                    connecting to a server
+   -m,  --manual           print the man page (Windows only)
+   -M,  --make-policy=<policy.txt>  creates a policy based on the target server
+                                    (i.e.: the target server has the ideal
+                                    configuration that other servers should
+                                    adhere to)
+   -n,  --no-colors        disable colors
+   -p,  --port=<port>      port to connect
+   -P,  --policy=<"policy name" | policy.txt>  run a policy test using the
+                                                   specified policy
+   -t,  --timeout=<secs>   timeout (in seconds) for connection and reading
+                               (default: 5)
+   -T,  --targets=<hosts.txt>  a file containing a list of target hosts (one
+                                   per line, format HOST[:PORT])
+        --threads=<threads>    number of threads to use when scanning multiple
+                                   targets (-T/--targets) (default: 32)
+   -v,  --verbose          verbose output
+```
+* if both IPv4 and IPv6 are used, order of precedence can be set by using either `-46` or `-64`.
+* batch flag `-b` will output sections without header and without empty lines (implies verbose flag).
+* verbose flag `-v` will prefix each line with section type and algorithm name.
+* an exit code of 0 is returned when all algorithms are considered secure (for a standard audit), or when a policy check passes (for a policy audit).
+
+Basic server auditing:
+```
+ssh-audit localhost
+ssh-audit 127.0.0.1
+ssh-audit 127.0.0.1:222
+ssh-audit ::1
+ssh-audit [::1]:222
+```
+
+To run a standard audit against many servers (place targets into servers.txt, one on each line in the format of `HOST[:PORT]`):
+
+```
+ssh-audit -T servers.txt
+```
+
+To audit a client configuration (listens on port 2222 by default; connect using `ssh -p 2222 anything@localhost`):
+
+```
+ssh-audit -c
+```
+
+To audit a client configuration, with a listener on port 4567:
+```
+ssh-audit -c -p 4567
+```
+
+To  list all official built-in policies (hint: use resulting policy names with `-P`/`--policy`):
+```
+ssh-audit -L
+```
+
+To run a policy audit against a server:
+```
+ssh-audit -P ["policy name" | path/to/server_policy.txt] targetserver
+```
+
+To run a policy audit against a client:
+```
+ssh-audit -c -P ["policy name" | path/to/client_policy.txt]
+```
+
+To run a policy audit against many servers:
+```
+ssh-audit -T servers.txt -P ["policy name" | path/to/server_policy.txt]
+```
+
+To create a policy based on a target server (which can be manually edited):
+```
+ssh-audit -M new_policy.txt targetserver
+```
+
+## Screenshots
+
+### Server Standard Audit Example
+Below is a screen shot of the standard server-auditing output when connecting to an unhardened OpenSSH v5.3 service:
+![screenshot](https://user-images.githubusercontent.com/2982011/64388792-317e6f80-d00e-11e9-826e-a4934769bb07.png)
+
+### Server Policy Audit Example
+Below is a screen shot of the policy auditing output when connecting to an un-hardened Ubuntu Server 20.04 machine (hint: use `-L`/`--list-policies` to see names of built-in policies to use with `-P`/`--policy`):
+![screenshot](https://user-images.githubusercontent.com/2982011/94370881-95178700-00c0-11eb-8705-3157a4669dc0.png)
+
+After applying the steps in the hardening guide (see below), the output changes to the following:
+![screenshot](https://user-images.githubusercontent.com/2982011/94370873-87620180-00c0-11eb-9a59-469f61a56ce1.png)
+
+### Client Standard Audit Example
+Below is a screen shot of the client-auditing output when an unhardened OpenSSH v7.2 client connects:
+![client_screenshot](https://user-images.githubusercontent.com/2982011/68867998-b946c100-06c4-11ea-975f-1f47e4178a74.png)
+
+## Hardening Guides
+Guides to harden server & client configuration can be found here: [https://www.ssh-audit.com/hardening_guides.html](https://www.ssh-audit.com/hardening_guides.html)
+
+## Pre-Built Packages
+Pre-built packages are available for Windows (see the releases page), PyPI, Snap, and Docker:
+
+To install from PyPI:
+```
+$ pip3 install ssh-audit
+```
+
+To install the Snap package:
+```
+$ snap install ssh-audit
+```
+
+To install from Dockerhub:
+```
+$ docker pull positronsecurity/ssh-audit
+```
+(Then run with: `docker run -it -p 2222:2222 positronsecurity/ssh-audit 10.1.1.1`)
+
+The status of various other platform packages can be found below (via Repology):
+
+<a href="https://repology.org/project/ssh-audit/versions"><img src="https://repology.org/badge/vertical-allrepos/ssh-audit.svg?columns=4" alt="Packaging status" align="center"></a>
+
+## Web Front-End
+For convenience, a web front-end on top of the command-line tool is available at [https://www.ssh-audit.com/](https://www.ssh-audit.com/).
+
+## ChangeLog
+
+### v2.9.0 (2023-04-29)
+ - Dropped support for Python 3.6, as it reached EOL at the end of 2021.
+ - Added Ubuntu Server & Client 22.04 hardening policies.
+ - Removed experimental warning tag from `sntrup761x25519-sha512@openssh.com`.
+ - Updated CVE database; credit [Alexandre Zanni](https://github.com/noraj).
+ - Added `-g` and `--gex-test` for granular GEX modulus size tests; credit [Adam Russell](https://github.com/thecliguy).
+ - Snap packages now print more user-friendly error messages when permission errors are encountered.
+ - JSON 'target' field now always includes port number; credit [tomatohater1337](https://github.com/tomatohater1337).
+ - JSON output now includes recommendations and CVE data.
+ - Mixed host key/CA key types (i.e.: RSA host keys signed with ED25519 CAs, etc.) are now properly handled.
+ - Warnings are now printed for 2048-bit moduli; partial credit [Adam Russell](https://github.com/thecliguy).
+ - SHA-1 algorithms now cause failures.
+ - CBC mode ciphers are now warnings instead of failures.
+ - Generic failure/warning messages replaced with more specific reasons (i.e.: 'using weak cipher' => 'using broken RC4 cipher').
+ - Updated built-in policies to include missing host key size information.
+ - Added built-in policies for OpenSSH 8.8, 8.9, 9.0, 9.1, 9.2, and 9.3.
+ - Added 33 new host keys: `dsa2048-sha224@libassh.org`, `dsa2048-sha256@libassh.org`, `dsa3072-sha256@libassh.org`, `ecdsa-sha2-1.3.132.0.10-cert-v01@openssh.com`, `eddsa-e382-shake256@libassh.org`, `eddsa-e521-shake256@libassh.org`, `null`, `pgp-sign-dss`, `pgp-sign-rsa`, `spki-sign-dss`, `spki-sign-rsa`, `ssh-dss-sha224@ssh.com`, `ssh-dss-sha384@ssh.com`, `ssh-dss-sha512@ssh.com`, `ssh-ed448-cert-v01@openssh.com`, `ssh-rsa-sha224@ssh.com`, `ssh-rsa-sha2-256`, `ssh-rsa-sha2-512`, `ssh-rsa-sha384@ssh.com`, `ssh-rsa-sha512@ssh.com`, `ssh-xmss-cert-v01@openssh.com`, `ssh-xmss@openssh.com`, `webauthn-sk-ecdsa-sha2-nistp256@openssh.com`, `x509v3-ecdsa-sha2-1.3.132.0.10`, `x509v3-sign-dss-sha1`, `x509v3-sign-dss-sha224@ssh.com`, `x509v3-sign-dss-sha256@ssh.com`, `x509v3-sign-dss-sha384@ssh.com`, `x509v3-sign-dss-sha512@ssh.com`, `x509v3-sign-rsa-sha1`, `x509v3-sign-rsa-sha224@ssh.com`, `x509v3-sign-rsa-sha384@ssh.com`, `x509v3-sign-rsa-sha512@ssh.com`.
+ - Added 46 new key exchanges: `diffie-hellman-group14-sha224@ssh.com`, `diffie-hellman_group17-sha512`, `diffie-hellman-group-exchange-sha224@ssh.com`, `diffie-hellman-group-exchange-sha384@ssh.com`, `ecdh-sha2-1.2.840.10045.3.1.1`, `ecdh-sha2-1.2.840.10045.3.1.7`, `ecdh-sha2-1.3.132.0.1`, `ecdh-sha2-1.3.132.0.16`, `ecdh-sha2-1.3.132.0.26`, `ecdh-sha2-1.3.132.0.27`, `ecdh-sha2-1.3.132.0.33`, `ecdh-sha2-1.3.132.0.34`, `ecdh-sha2-1.3.132.0.35`, `ecdh-sha2-1.3.132.0.36`, `ecdh-sha2-1.3.132.0.37`, `ecdh-sha2-1.3.132.0.38`, `ecdh-sha2-4MHB+NBt3AlaSRQ7MnB4cg==`, `ecdh-sha2-5pPrSUQtIaTjUSt5VZNBjg==`, `ecdh-sha2-9UzNcgwTlEnSCECZa7V1mw==`, `ecdh-sha2-D3FefCjYoJ/kfXgAyLddYA==`, `ecdh-sha2-h/SsxnLCtRBh7I9ATyeB3A==`, `ecdh-sha2-m/FtSAmrV4j/Wy6RVUaK7A==`, `ecdh-sha2-mNVwCXAoS1HGmHpLvBC94w==`, `ecdh-sha2-qCbG5Cn/jjsZ7nBeR7EnOA==`, `ecdh-sha2-qcFQaMAMGhTziMT0z+Tuzw==`, `ecdh-sha2-VqBg4QRPjxx1EXZdV0GdWQ==`, `ecdh-sha2-wiRIU8TKjMZ418sMqlqtvQ==`, `ecdh-sha2-zD/b3hu/71952ArpUG4OjQ==`, `ecmqv-sha2`, `gss-13.3.132.0.10-sha256-*`, `gss-curve25519-sha256-*`, `gss-curve448-sha512-*`, `gss-gex-sha1-*`, `gss-gex-sha256-*`, `gss-group14-sha1-*`, `gss-group14-sha256-*`, `gss-group15-sha512-*`, `gss-group16-sha512-*`, `gss-group17-sha512-*`, `gss-group18-sha512-*`, `gss-group1-sha1-*`, `gss-nistp256-sha256-*`, `gss-nistp384-sha256-*`, `gss-nistp521-sha512-*`, `m383-sha384@libassh.org`, `m511-sha512@libassh.org`.
+ - Added 28 new ciphers: `3des-cfb`, `3des-ecb`, `3des-ofb`, `blowfish-cfb`, `blowfish-ecb`, `blowfish-ofb`, `camellia128-cbc@openssh.org`, `camellia128-ctr@openssh.org`, `camellia192-cbc@openssh.org`, `camellia192-ctr@openssh.org`, `camellia256-cbc@openssh.org`, `camellia256-ctr@openssh.org`, `cast128-cfb`, `cast128-ecb`, `cast128-ofb`, `cast128-12-cbc@ssh.com`, `idea-cfb`, `idea-ecb`, `idea-ofb`, `rijndael-cbc@ssh.com`, `seed-ctr@ssh.com`, `serpent128-gcm@libassh.org`, `serpent256-gcm@libassh.org`, `twofish128-gcm@libassh.org`, `twofish256-gcm@libassh.org`, `twofish-cfb`, `twofish-ecb`, `twofish-ofb`
+ - Added 5 new MACs: `hmac-sha1-96@openssh.com`, `hmac-sha224@ssh.com`, `hmac-sha256-2@ssh.com`, `hmac-sha384@ssh.com`, `hmac-whirlpool`.
+
+### v2.5.0 (2021-08-26)
+ - Fixed crash when running host key tests.
+ - Handles server connection failures more gracefully.
+ - Now prints JSON with indents when `-jj` is used (useful for debugging).
+ - Added MD5 fingerprints to verbose output.
+ - Added `-d`/`--debug` option for getting debugging output; credit [Adam Russell](https://github.com/thecliguy).
+ - Updated JSON output to include MD5 fingerprints.  Note that this results in a breaking change in the 'fingerprints' dictionary format.
+ - Updated OpenSSH 8.1 (and earlier) policies to include `rsa-sha2-512` and `rsa-sha2-256`.
+ - Added OpenSSH v8.6 & v8.7 policies.
+ - Added 3 new key exchanges: `gss-gex-sha1-eipGX3TCiQSrx573bT1o1Q==`, `gss-group1-sha1-eipGX3TCiQSrx573bT1o1Q==`, and `gss-group14-sha1-eipGX3TCiQSrx573bT1o1Q==`.
+ - Added 3 new MACs: `hmac-ripemd160-96`, `AEAD_AES_128_GCM`, and `AEAD_AES_256_GCM`.
+
+### v2.4.0 (2021-02-23)
+ - Added multi-threaded scanning support.
+ - Added built-in Windows manual page (see `-m`/`--manual`); credit [Adam Russell](https://github.com/thecliguy).
+ - Added version check for OpenSSH user enumeration (CVE-2018-15473).
+ - Added deprecation note to host key types based on SHA-1.
+ - Added extra warnings for SSHv1.
+ - Added built-in hardened OpenSSH v8.5 policy.
+ - Upgraded warnings to failures for host key types based on SHA-1.
+ - Fixed crash when receiving unexpected response during host key test.
+ - Fixed hang against older Cisco devices during host key test & gex test.
+ - Fixed improper termination while scanning multiple targets when one target returns an error.
+ - Dropped support for Python 3.5 (which reached EOL in Sept. 2020).
+ - Added 1 new key exchange: `sntrup761x25519-sha512@openssh.com`.
+
+### v2.3.1 (2020-10-28)
+ - Now parses public key sizes for `rsa-sha2-256-cert-v01@openssh.com` and `rsa-sha2-512-cert-v01@openssh.com` host key types.
+ - Flag `ssh-rsa-cert-v01@openssh.com` as a failure due to SHA-1 hash.
+ - Fixed bug in recommendation output which suppressed some algorithms inappropriately.
+ - Built-in policies now include CA key requirements (if certificates are in use).
+ - Lookup function (`--lookup`) now performs case-insensitive lookups of similar algorithms; credit [Adam Russell](https://github.com/thecliguy).
+ - Migrated pre-made policies from external files to internal database.
+ - Split single 3,500 line script into many files (by class).
+ - Added setup.py support; credit [Ganden Schaffner](https://github.com/gschaffner).
+ - Added 1 new cipher: `des-cbc@ssh.com`.
+
+### v2.3.0 (2020-09-27)
+ - Added new policy auditing functionality to test adherence to a hardening guide/standard configuration (see `-L`/`--list-policies`, `-M`/`--make-policy` and `-P`/`--policy`).  For an in-depth tutorial, see <https://www.positronsecurity.com/blog/2020-09-27-ssh-policy-configuration-checks-with-ssh-audit/>.
+ - Created new man page (see `ssh-audit.1` file).
+ - 1024-bit moduli upgraded from warnings to failures.
+ - Many Python 2 code clean-ups, testing framework improvements, pylint & flake8 fixes, and mypy type comments; credit [Jürgen Gmach](https://github.com/jugmac00).
+ - Added feature to look up algorithms in internal database (see `--lookup`); credit [Adam Russell](https://github.com/thecliguy).
+ - Suppress recommendation of token host key types.
+ - Added check for use-after-free vulnerability in PuTTY v0.73.
+ - Added 11 new host key types: `ssh-rsa1`, `ssh-dss-sha256@ssh.com`, `ssh-gost2001`, `ssh-gost2012-256`, `ssh-gost2012-512`, `spki-sign-rsa`, `ssh-ed448`, `x509v3-ecdsa-sha2-nistp256`, `x509v3-ecdsa-sha2-nistp384`, `x509v3-ecdsa-sha2-nistp521`, `x509v3-rsa2048-sha256`.
+ - Added 8 new key exchanges: `diffie-hellman-group1-sha256`, `kexAlgoCurve25519SHA256`, `Curve25519SHA256`, `gss-group14-sha256-`, `gss-group15-sha512-`, `gss-group16-sha512-`, `gss-nistp256-sha256-`, `gss-curve25519-sha256-`.
+ - Added 5 new ciphers: `blowfish`, `AEAD_AES_128_GCM`, `AEAD_AES_256_GCM`, `crypticore128@ssh.com`, `seed-cbc@ssh.com`.
+ - Added 3 new MACs: `chacha20-poly1305@openssh.com`, `hmac-sha3-224`, `crypticore-mac@ssh.com`.
+
+### v2.2.0 (2020-03-11)
+ - Marked host key type `ssh-rsa` as weak due to [practical SHA-1 collisions](https://eprint.iacr.org/2020/014.pdf).
+ - Added Windows builds.
+ - Added 10 new host key types: `ecdsa-sha2-1.3.132.0.10`, `x509v3-sign-dss`, `x509v3-sign-rsa`, `x509v3-sign-rsa-sha256@ssh.com`, `x509v3-ssh-dss`, `x509v3-ssh-rsa`, `sk-ecdsa-sha2-nistp256-cert-v01@openssh.com`, `sk-ecdsa-sha2-nistp256@openssh.com`, `sk-ssh-ed25519-cert-v01@openssh.com`, and `sk-ssh-ed25519@openssh.com`.
+ - Added 18 new key exchanges: `diffie-hellman-group14-sha256@ssh.com`, `diffie-hellman-group15-sha256@ssh.com`, `diffie-hellman-group15-sha384@ssh.com`, `diffie-hellman-group16-sha384@ssh.com`, `diffie-hellman-group16-sha512@ssh.com`, `diffie-hellman-group18-sha512@ssh.com`, `ecdh-sha2-curve25519`, `ecdh-sha2-nistb233`, `ecdh-sha2-nistb409`, `ecdh-sha2-nistk163`, `ecdh-sha2-nistk233`, `ecdh-sha2-nistk283`, `ecdh-sha2-nistk409`, `ecdh-sha2-nistp192`, `ecdh-sha2-nistp224`, `ecdh-sha2-nistt571`, `gss-gex-sha1-`, and `gss-group1-sha1-`.
+ - Added 9 new ciphers: `camellia128-cbc`, `camellia128-ctr`, `camellia192-cbc`, `camellia192-ctr`, `camellia256-cbc`, `camellia256-ctr`, `aes128-gcm`, `aes256-gcm`, and `chacha20-poly1305`.
+ - Added 2 new MACs: `aes128-gcm` and `aes256-gcm`.
+
+### v2.1.1 (2019-11-26)
+ - Added 2 new host key types: `rsa-sha2-256-cert-v01@openssh.com`, `rsa-sha2-512-cert-v01@openssh.com`.
+ - Added 2 new ciphers: `des`, `3des`.
+ - Added 3 new PuTTY vulnerabilities.
+ - During client testing, client IP address is now listed in output.
+
+### v2.1.0 (2019-11-14)
+ - Added client software auditing functionality (see `-c` / `--client-audit` option).
+ - Added JSON output option (see `-j` / `--json` option; credit [Andreas Jaggi](https://github.com/x-way)).
+ - Fixed crash while scanning Solaris Sun_SSH.
+ - Added 9 new key exchanges: `gss-group1-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-gex-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha1-`, `gss-group14-sha1-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group14-sha256-toWM5Slw5Ew8Mqkay+al2g==`, `gss-group15-sha512-toWM5Slw5Ew8Mqkay+al2g==`, `diffie-hellman-group15-sha256`, `ecdh-sha2-1.3.132.0.10`, `curve448-sha512`.
+ - Added 1 new host key type: `ecdsa-sha2-1.3.132.0.10`.
+ - Added 4 new ciphers: `idea-cbc`, `serpent128-cbc`, `serpent192-cbc`, `serpent256-cbc`.
+ - Added 6 new MACs: `hmac-sha2-256-96-etm@openssh.com`, `hmac-sha2-512-96-etm@openssh.com`, `hmac-ripemd`, `hmac-sha256-96@ssh.com`, `umac-32@openssh.com`, `umac-96@openssh.com`.
+
+### v2.0.0 (2019-08-29)
+ - Forked from https://github.com/arthepsy/ssh-audit (development was stalled, and developer went MIA).
+ - Added RSA host key length test.
+ - Added RSA certificate key length test.
+ - Added Diffie-Hellman modulus size test.
+ - Now outputs host key fingerprints for RSA and ED25519.
+ - Added 5 new key exchanges: `sntrup4591761x25519-sha512@tinyssh.org`, `diffie-hellman-group-exchange-sha256@ssh.com`, `diffie-hellman-group-exchange-sha512@ssh.com`, `diffie-hellman-group16-sha256`, `diffie-hellman-group17-sha512`.
+ - Added 3 new encryption algorithms: `des-cbc-ssh1`, `blowfish-ctr`, `twofish-ctr`.
+ - Added 10 new MACs: `hmac-sha2-56`, `hmac-sha2-224`, `hmac-sha2-384`, `hmac-sha3-256`, `hmac-sha3-384`, `hmac-sha3-512`, `hmac-sha256`, `hmac-sha256@ssh.com`, `hmac-sha512`, `hmac-512@ssh.com`.
+ - Added command line argument (`-t` / `--timeout`) for connection & reading timeouts.
+ - Updated CVEs for libssh & Dropbear.
+
+### v1.7.0 (2016-10-26)
+ - implement options to allow specify IPv4/IPv6 usage and order of precedence
+ - implement option to specify remote port (old behavior kept for compatibility)
+ - add colors support for Microsoft Windows via optional colorama dependency
+ - fix encoding and decoding issues, add tests, do not crash on encoding errors
+ - use mypy-lang for static type checking and verify all code
+
+### v1.6.0 (2016-10-14)
+ - implement algorithm recommendations section (based on recognized software)
+ - implement full libssh support (version history, algorithms, security, etc)
+ - fix SSH-1.99 banner recognition and version comparison functionality
+ - do not output empty algorithms (happens for misconfigured servers)
+ - make consistent output for Python 3.x versions
+ - add a lot more tests (conf, banner, software, SSH1/SSH2, output, etc)
+ - use Travis CI to test for multiple Python versions (2.6-3.5, pypy, pypy3)
+
+### v1.5.0 (2016-09-20)
+ - create security section for related security information
+ - match and output assigned CVE list and security issues for Dropbear SSH
+ - implement full SSH1 support with fingerprint information
+ - automatically fallback to SSH1 on protocol mismatch
+ - add new options to force SSH1 or SSH2 (both allowed by default)
+ - parse banner information and convert it to specific software and OS version
+ - do not use padding in batch mode
+ - several fixes (Cisco sshd, rare hangs, error handling, etc)
+
+### v1.0.20160902
+ - implement batch output option
+ - implement minimum output level option
+ - fix compatibility with Python 2.6
+
+### v1.0.20160812
+ - implement SSH version compatibility feature
+ - fix wrong mac algorithm warning
+ - fix Dropbear SSH version typo
+ - parse pre-banner header
+ - better errors handling
+
+### v1.0.20160803
+ - use OpenSSH 7.3 banner
+ - add new key-exchange algorithms
+
+### v1.0.20160207
+ - use OpenSSH 7.2 banner
+ - additional warnings for OpenSSH 7.2
+ - fix OpenSSH 7.0 failure messages
+ - add rijndael-cbc failure message from OpenSSH 6.7
+
+### v1.0.20160105
+ - multiple additional warnings
+ - support for none algorithm
+ - better compression handling
+ - ensure reading enough data (fixes few Linux SSH)
+
+### v1.0.20151230
+ - Dropbear SSH support
+
+### v1.0.20151223
+ - initial version
```

### Comparing `ssh-audit-2.5.0/src/ssh_audit.egg-info/SOURCES.txt` & `ssh-audit-2.9.0/src/ssh_audit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

