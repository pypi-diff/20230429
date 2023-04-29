# Comparing `tmp/stuphos-2.0.8.tar.gz` & `tmp/stuphos-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stuphos-2.0.8.tar", last modified: Wed Nov 30 11:35:30 2022, max compression
+gzip compressed data, was "stuphos-2.0.9.tar", last modified: Mon Feb  6 17:03:12 2023, max compression
```

## Comparing `stuphos-2.0.8.tar` & `stuphos-2.0.9.tar`

### file list

```diff
@@ -1,271 +1,282 @@
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.342285 stuphos-2.0.8/
--rw-rw-r--   0 op        (1000) op        (1000)       28 2021-01-25 12:39:25.000000 stuphos-2.0.8/MANIFEST.in
--rw-rw-r--   0 op        (1000) op        (1000)    11382 2022-11-30 11:35:30.342285 stuphos-2.0.8/PKG-INFO
--rw-rw-r--   0 op        (1000) op        (1000)     6907 2022-11-30 11:31:24.000000 stuphos-2.0.8/README
--rw-rw-r--   0 op        (1000) op        (1000)       38 2022-11-30 11:35:30.342285 stuphos-2.0.8/setup.cfg
--rw-rw-r--   0 op        (1000) op        (1000)     8623 2022-11-21 16:19:21.000000 stuphos-2.0.8/setup.py
--rw-rw-r--   0 op        (1000) op        (1000)     2633 2022-02-25 14:12:42.000000 stuphos-2.0.8/skeletoncore.tar.gz
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.303284 stuphos-2.0.8/stuphmud/
--rw-rw-r--   0 op        (1000) op        (1000)        0 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)       50 2021-09-14 15:51:31.000000 stuphos-2.0.8/stuphmud/elemental.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.303284 stuphos-2.0.8/stuphmud/server/
--rw-rw-r--   0 op        (1000) op        (1000)      683 2021-01-28 13:58:49.000000 stuphos-2.0.8/stuphmud/server/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)    25778 2022-11-19 20:07:36.000000 stuphos-2.0.8/stuphmud/server/adapters.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.304284 stuphos-2.0.8/stuphmud/server/api/
--rw-rw-r--   0 op        (1000) op        (1000)     7149 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/api/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)       26 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/api/constants.py
--rw-rw-r--   0 op        (1000) op        (1000)    62523 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/api/structs.py
--rw-rw-r--   0 op        (1000) op        (1000)     4917 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/api/tests.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.304284 stuphos-2.0.8/stuphmud/server/magic/
--rw-rw-r--   0 op        (1000) op        (1000)     2136 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/magic/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)      505 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/magic/structure.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.305284 stuphos-2.0.8/stuphmud/server/player/
--rw-rw-r--   0 op        (1000) op        (1000)    14819 2022-11-14 10:49:20.000000 stuphos-2.0.8/stuphmud/server/player/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.306284 stuphos-2.0.8/stuphmud/server/player/commands/
--rw-rw-r--   0 op        (1000) op        (1000)     3618 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.307284 stuphos-2.0.8/stuphmud/server/player/commands/gc/
--rw-rw-r--   0 op        (1000) op        (1000)      114 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)    11488 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/olc.py
--rw-rw-r--   0 op        (1000) op        (1000)     9186 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/profiling.py
--rw-rw-r--   0 op        (1000) op        (1000)     6353 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/system.py
--rw-rw-r--   0 op        (1000) op        (1000)     1891 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/web_debug.py
--rw-rw-r--   0 op        (1000) op        (1000)    32671 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/wizard.py
--rw-rw-r--   0 op        (1000) op        (1000)    10636 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/gc/xdebug.py
--rw-rw-r--   0 op        (1000) op        (1000)     8263 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/commands/mime.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.308284 stuphos-2.0.8/stuphmud/server/player/db/
--rw-rw-r--   0 op        (1000) op        (1000)     8806 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     2872 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/db/hi.py
--rw-rw-r--   0 op        (1000) op        (1000)     9873 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/managedfs.py
--rw-rw-r--   0 op        (1000) op        (1000)     8126 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/playerfile.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.309284 stuphos-2.0.8/stuphmud/server/player/db/rent/
--rw-rw-r--   0 op        (1000) op        (1000)       46 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)       48 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/constants.py
--rw-rw-r--   0 op        (1000) op        (1000)     7590 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/edit.py
--rw-rw-r--   0 op        (1000) op        (1000)       13 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/equip.py
--rw-rw-r--   0 op        (1000) op        (1000)     1728 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/management.py
--rw-rw-r--   0 op        (1000) op        (1000)     2642 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/scan.py
--rw-rw-r--   0 op        (1000) op        (1000)     3530 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/db/rent/show.py
--rw-rw-r--   0 op        (1000) op        (1000)     3243 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/db/sql.py
--rw-rw-r--   0 op        (1000) op        (1000)    18861 2022-03-06 13:11:31.000000 stuphos-2.0.8/stuphmud/server/player/editor.py
--rw-rw-r--   0 op        (1000) op        (1000)      704 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/events.py
--rw-rw-r--   0 op        (1000) op        (1000)     1409 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/http.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.310284 stuphos-2.0.8/stuphmud/server/player/interfaces/
--rw-rw-r--   0 op        (1000) op        (1000)     2205 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.311284 stuphos-2.0.8/stuphmud/server/player/interfaces/code/
--rw-rw-r--   0 op        (1000) op        (1000)    16834 2022-09-19 13:10:56.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/code/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     1335 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/code/environ.py
--rw-rw-r--   0 op        (1000) op        (1000)    28093 2022-11-27 10:48:53.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/code/girl.py
--rw-rw-r--   0 op        (1000) op        (1000)     6419 2022-10-30 11:28:43.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/code/python.py
--rw-rw-r--   0 op        (1000) op        (1000)     3025 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/code/xmlrpc_python.py
--rw-rw-r--   0 op        (1000) op        (1000)     6683 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/dictcmd.py
--rw-rw-r--   0 op        (1000) op        (1000)     3913 2022-02-25 16:15:45.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/history.py
--rw-rw-r--   0 op        (1000) op        (1000)     6700 2022-10-30 11:29:44.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/standard.py
--rw-rw-r--   0 op        (1000) op        (1000)     1771 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/interfaces/threading.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.311284 stuphos-2.0.8/stuphmud/server/player/messaging/
--rw-rw-r--   0 op        (1000) op        (1000)       45 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/messaging/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)    17074 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/notebook.py
--rw-rw-r--   0 op        (1000) op        (1000)     8081 2022-03-06 11:45:42.000000 stuphos-2.0.8/stuphmud/server/player/shell.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.313284 stuphos-2.0.8/stuphmud/server/player/telnet/
--rw-rw-r--   0 op        (1000) op        (1000)      130 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     8130 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/client.py
--rw-rw-r--   0 op        (1000) op        (1000)     3454 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/comm.py
--rw-rw-r--   0 op        (1000) op        (1000)     1895 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/telnet/core.py
--rw-rw-r--   0 op        (1000) op        (1000)     1702 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/player/telnet/deploy.py
--rw-rw-r--   0 op        (1000) op        (1000)    11444 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/dispatch.py
--rw-rw-r--   0 op        (1000) op        (1000)     5139 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/ftp.py
--rw-rw-r--   0 op        (1000) op        (1000)     3806 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/http.py
--rw-rw-r--   0 op        (1000) op        (1000)     2934 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/pentacle.py
--rw-rw-r--   0 op        (1000) op        (1000)     2951 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/rexec.py
--rw-rw-r--   0 op        (1000) op        (1000)     2400 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/player/telnet/test.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.315284 stuphos-2.0.8/stuphmud/server/zones/
--rw-rw-r--   0 op        (1000) op        (1000)    19714 2022-03-17 16:40:08.000000 stuphos-2.0.8/stuphmud/server/zones/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)      176 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/zones/combat.py
--rw-rw-r--   0 op        (1000) op        (1000)    15315 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/zones/config.py
--rw-rw-r--   0 op        (1000) op        (1000)     7392 2022-09-16 12:45:21.000000 stuphos-2.0.8/stuphmud/server/zones/controller.py
--rw-rw-r--   0 op        (1000) op        (1000)    18848 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/zones/freeze.py
--rw-rw-r--   0 op        (1000) op        (1000)       83 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphmud/server/zones/physical.py
--rw-rw-r--   0 op        (1000) op        (1000)      884 2021-01-28 13:58:50.000000 stuphos-2.0.8/stuphmud/server/zones/space.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.315284 stuphos-2.0.8/stuphmud/server/zones/specials/
--rw-rw-r--   0 op        (1000) op        (1000)     8860 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/zones/specials/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.315284 stuphos-2.0.8/stuphmud/server/zones/specials/autoquest/
--rw-rw-r--   0 op        (1000) op        (1000)    35280 2022-10-25 17:56:12.000000 stuphos-2.0.8/stuphmud/server/zones/specials/autoquest/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)    10104 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/zones/specials/autoquest/slay.py
--rw-rw-r--   0 op        (1000) op        (1000)     6281 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphmud/server/zones/specials/standard.py
--rw-rw-r--   0 op        (1000) op        (1000)     1931 2021-01-28 13:58:50.000000 stuphos-2.0.8/stuphmud/server/zones/wilderness.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.316284 stuphos-2.0.8/stuphos/
--rw-rw-r--   0 op        (1000) op        (1000)      980 2022-10-30 11:01:10.000000 stuphos-2.0.8/stuphos/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.317284 stuphos-2.0.8/stuphos/db/
--rw-rw-r--   0 op        (1000) op        (1000)      835 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/db/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     6281 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/db/conf.py
--rw-rw-r--   0 op        (1000) op        (1000)    23189 2022-10-21 12:56:20.000000 stuphos-2.0.8/stuphos/db/orm.py
--rw-rw-r--   0 op        (1000) op        (1000)    12016 2022-11-17 18:23:42.000000 stuphos-2.0.8/stuphos/db/vardb.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.318284 stuphos-2.0.8/stuphos/etc/
--rw-rw-r--   0 op        (1000) op        (1000)       21 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/etc/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.320284 stuphos-2.0.8/stuphos/etc/tools/
--rw-rw-r--   0 op        (1000) op        (1000)     2365 2022-09-15 11:55:58.000000 stuphos-2.0.8/stuphos/etc/tools/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     4096 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/etc/tools/cmdln.py
--rw-rw-r--   0 op        (1000) op        (1000)    21636 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/etc/tools/collections_hack.py
--rw-rw-r--   0 op        (1000) op        (1000)     9747 2021-11-20 19:30:35.000000 stuphos-2.0.8/stuphos/etc/tools/debugging.py
--rw-rw-r--   0 op        (1000) op        (1000)     6629 2021-08-18 15:54:35.000000 stuphos-2.0.8/stuphos/etc/tools/errors.py
--rw-rw-r--   0 op        (1000) op        (1000)     1215 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/etc/tools/internet.py
--rw-rw-r--   0 op        (1000) op        (1000)     3932 2022-11-18 20:36:37.000000 stuphos-2.0.8/stuphos/etc/tools/logs.py
--rw-rw-r--   0 op        (1000) op        (1000)    13902 2022-11-22 21:13:16.000000 stuphos-2.0.8/stuphos/etc/tools/misc.py
--rw-rw-r--   0 op        (1000) op        (1000)      423 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/etc/tools/platform.py
--rw-rw-r--   0 op        (1000) op        (1000)     6596 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/etc/tools/pyg_colorizer.py
--rw-rw-r--   0 op        (1000) op        (1000)     7281 2022-11-02 10:28:48.000000 stuphos-2.0.8/stuphos/etc/tools/strings.py
--rw-rw-r--   0 op        (1000) op        (1000)      779 2022-10-30 16:16:11.000000 stuphos-2.0.8/stuphos/etc/tools/timing.py
--rw-r--r--   0 op        (1000) op        (1000)     1288 2022-11-02 16:12:43.000000 stuphos-2.0.8/stuphos/etc/tools/urls.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.320284 stuphos-2.0.8/stuphos/kernel/
--rw-rw-r--   0 op        (1000) op        (1000)     5722 2022-11-15 18:15:21.000000 stuphos-2.0.8/stuphos/kernel/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.320284 stuphos-2.0.8/stuphos/language/
--rw-rw-r--   0 op        (1000) op        (1000)      734 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/language/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.321284 stuphos-2.0.8/stuphos/language/board/
--rw-rw-r--   0 op        (1000) op        (1000)    14855 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/board/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)    32461 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/board/comm.py
--rw-rw-r--   0 op        (1000) op        (1000)    16574 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/board/specproc.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.322284 stuphos-2.0.8/stuphos/language/document/
--rw-rw-r--   0 op        (1000) op        (1000)       27 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/language/document/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     1747 2022-11-09 15:42:16.000000 stuphos-2.0.8/stuphos/language/document/interface.py
--rw-rw-r--   0 op        (1000) op        (1000)    88610 2022-11-22 21:26:30.000000 stuphos-2.0.8/stuphos/language/document/structural.py
--rw-rw-r--   0 op        (1000) op        (1000)    11669 2022-11-08 17:43:11.000000 stuphos-2.0.8/stuphos/language/document/wrlc.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.323284 stuphos-2.0.8/stuphos/language/gen/
--rw-rw-r--   0 op        (1000) op        (1000)    24614 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/gen/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     9830 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/language/gen/gs_indent_lexer.py
--rw-r--r--   0 op        (1000) op        (1000)      116 2021-06-11 12:58:16.000000 stuphos-2.0.8/stuphos/language/moo.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.323284 stuphos-2.0.8/stuphos/language/query/
--rw-rw-r--   0 op        (1000) op        (1000)    11506 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/query/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     5024 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/query/ql2.py
--rw-rw-r--   0 op        (1000) op        (1000)     9655 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/shortate.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.323284 stuphos-2.0.8/stuphos/language/vm/
--rw-rw-r--   0 op        (1000) op        (1000)      511 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/language/vm/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.323284 stuphos-2.0.8/stuphos/language/xml/
--rw-rw-r--   0 op        (1000) op        (1000)    34407 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/language/xml/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.326285 stuphos-2.0.8/stuphos/management/
--rw-rw-r--   0 op        (1000) op        (1000)     5901 2022-11-15 14:10:44.000000 stuphos-2.0.8/stuphos/management/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     8827 2022-03-16 15:52:04.000000 stuphos-2.0.8/stuphos/management/authlock.py
--rw-rw-r--   0 op        (1000) op        (1000)       55 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/management/autowiz.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.328285 stuphos-2.0.8/stuphos/management/command_messaging/
--rw-rw-r--   0 op        (1000) op        (1000)      846 2021-11-20 19:30:35.000000 stuphos-2.0.8/stuphos/management/command_messaging/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     3697 2021-11-20 19:30:35.000000 stuphos-2.0.8/stuphos/management/command_messaging/base.py
--rw-rw-r--   0 op        (1000) op        (1000)      979 2021-12-11 20:04:18.000000 stuphos-2.0.8/stuphos/management/command_messaging/deployment.py
--rw-rw-r--   0 op        (1000) op        (1000)      509 2021-01-28 13:58:50.000000 stuphos-2.0.8/stuphos/management/command_messaging/girl.py
--rw-rw-r--   0 op        (1000) op        (1000)     2286 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/management/command_messaging/python.py
--rw-rw-r--   0 op        (1000) op        (1000)     3934 2021-01-29 14:21:41.000000 stuphos-2.0.8/stuphos/management/command_messaging/resource.py
--rw-rw-r--   0 op        (1000) op        (1000)     1228 2021-01-28 13:58:43.000000 stuphos-2.0.8/stuphos/management/command_messaging/shell.py
--rw-rw-r--   0 op        (1000) op        (1000)      712 2021-01-28 13:58:42.000000 stuphos-2.0.8/stuphos/management/command_messaging/subdaemon.py
--rw-rw-r--   0 op        (1000) op        (1000)     4577 2022-04-06 23:32:10.000000 stuphos-2.0.8/stuphos/management/config.py
--rw-rw-r--   0 op        (1000) op        (1000)    14666 2021-11-20 19:30:35.000000 stuphos-2.0.8/stuphos/management/deploy.py
--rw-rw-r--   0 op        (1000) op        (1000)     2272 2022-02-22 13:20:12.000000 stuphos-2.0.8/stuphos/management/idling.py
--rw-rw-r--   0 op        (1000) op        (1000)      968 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/management/naming.py
--rw-rw-r--   0 op        (1000) op        (1000)    12939 2022-11-09 15:44:00.000000 stuphos-2.0.8/stuphos/management/packaging.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.328285 stuphos-2.0.8/stuphos/management/protocols/
--rw-rw-r--   0 op        (1000) op        (1000)      225 2021-01-28 13:58:41.000000 stuphos-2.0.8/stuphos/management/protocols/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)       58 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/management/protocols/http.py
--rw-rw-r--   0 op        (1000) op        (1000)    13141 2022-10-30 11:16:32.000000 stuphos-2.0.8/stuphos/management/reboot.py
--rw-rw-r--   0 op        (1000) op        (1000)     3867 2022-03-14 16:33:19.000000 stuphos-2.0.8/stuphos/management/services.py
--rw-rw-r--   0 op        (1000) op        (1000)     6465 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/management/shell.py
--rw-rw-r--   0 op        (1000) op        (1000)    15462 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/management/subdaemon.py
--rw-rw-r--   0 op        (1000) op        (1000)    37273 2022-11-08 18:54:26.000000 stuphos-2.0.8/stuphos/management/syslog.py
--rw-rw-r--   0 op        (1000) op        (1000)     9875 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/management/tracking.py
--rw-rw-r--   0 op        (1000) op        (1000)    14287 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/management/tracsite.py
--rw-rw-r--   0 op        (1000) op        (1000)      160 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/management/workflow.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.329285 stuphos-2.0.8/stuphos/pentacle/
--rw-rw-r--   0 op        (1000) op        (1000)      608 2021-01-28 13:58:34.000000 stuphos-2.0.8/stuphos/pentacle/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.329285 stuphos-2.0.8/stuphos/pentacle/federation/
--rw-rw-r--   0 op        (1000) op        (1000)       24 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/pentacle/federation/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)      817 2021-01-28 13:58:33.000000 stuphos-2.0.8/stuphos/pentacle/management.py
--rw-rw-r--   0 op        (1000) op        (1000)     1098 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/pentacle/native.py
--rw-rw-r--   0 op        (1000) op        (1000)     4390 2021-01-28 13:58:33.000000 stuphos-2.0.8/stuphos/pentacle/oob.py
--rw-rw-r--   0 op        (1000) op        (1000)      457 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/pentacle/partner.py
--rw-rw-r--   0 op        (1000) op        (1000)     2600 2021-12-11 20:07:45.000000 stuphos-2.0.8/stuphos/pentacle/service.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.329285 stuphos-2.0.8/stuphos/phClient/
--rw-rw-r--   0 op        (1000) op        (1000)    27752 2022-11-08 18:37:36.000000 stuphos-2.0.8/stuphos/phClient/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.331285 stuphos-2.0.8/stuphos/runtime/
--rw-rw-r--   0 op        (1000) op        (1000)     7099 2022-04-03 13:54:28.000000 stuphos-2.0.8/stuphos/runtime/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.331285 stuphos-2.0.8/stuphos/runtime/architecture/
--rw-rw-r--   0 op        (1000) op        (1000)    35594 2022-11-28 11:28:47.000000 stuphos-2.0.8/stuphos/runtime/architecture/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     5355 2022-11-22 19:48:57.000000 stuphos-2.0.8/stuphos/runtime/architecture/api.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.332285 stuphos-2.0.8/stuphos/runtime/architecture/lookup/
--rw-rw-r--   0 op        (1000) op        (1000)     2582 2022-11-08 17:16:50.000000 stuphos-2.0.8/stuphos/runtime/architecture/lookup/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)      521 2022-04-27 12:38:39.000000 stuphos-2.0.8/stuphos/runtime/architecture/routines.py
--rw-rw-r--   0 op        (1000) op        (1000)    20414 2022-03-02 19:45:52.000000 stuphos-2.0.8/stuphos/runtime/architecture/spatial.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.332285 stuphos-2.0.8/stuphos/runtime/core/
--rw-rw-r--   0 op        (1000) op        (1000)    12097 2022-11-21 16:17:52.000000 stuphos-2.0.8/stuphos/runtime/core/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     9831 2022-11-08 17:25:42.000000 stuphos-2.0.8/stuphos/runtime/events.py
--rw-rw-r--   0 op        (1000) op        (1000)     4964 2022-11-08 17:18:47.000000 stuphos-2.0.8/stuphos/runtime/facilities.py
--rw-rw-r--   0 op        (1000) op        (1000)     1972 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/runtime/misc.py
--rw-rw-r--   0 op        (1000) op        (1000)      275 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/runtime/parallel.py
--rw-rw-r--   0 op        (1000) op        (1000)     8634 2022-11-08 17:24:42.000000 stuphos-2.0.8/stuphos/runtime/plugins.py
--rw-rw-r--   0 op        (1000) op        (1000)    14165 2022-11-08 17:39:57.000000 stuphos-2.0.8/stuphos/runtime/registry.py
--rw-rw-r--   0 op        (1000) op        (1000)     4093 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/runtime/sandbox.py
--rw-rw-r--   0 op        (1000) op        (1000)     3546 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/runtime/support.py
--rw-rw-r--   0 op        (1000) op        (1000)    67622 2022-11-29 11:10:00.000000 stuphos-2.0.8/stuphos/structure.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.336285 stuphos-2.0.8/stuphos/stuphlib/
--rw-rw-r--   0 op        (1000) op        (1000)        0 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/stuphlib/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     6605 2022-11-22 22:53:03.000000 stuphos-2.0.8/stuphos/stuphlib/binary.py
--rw-rw-r--   0 op        (1000) op        (1000)     8010 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/boards.py
--rw-rw-r--   0 op        (1000) op        (1000)     2683 2022-01-20 16:18:18.000000 stuphos-2.0.8/stuphos/stuphlib/cherry.py
--rw-rw-r--   0 op        (1000) op        (1000)     6309 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/clanlib.py
--rw-rw-r--   0 op        (1000) op        (1000)    72417 2022-02-27 16:29:14.000000 stuphos-2.0.8/stuphos/stuphlib/constants.py
--rw-rw-r--   0 op        (1000) op        (1000)    18082 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/dblib.py
--rw-rw-r--   0 op        (1000) op        (1000)    26706 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/directory.py
--rw-rw-r--   0 op        (1000) op        (1000)     1688 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/etc.py
--rw-rw-r--   0 op        (1000) op        (1000)     2807 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/stuphlib/help.py
--rw-rw-r--   0 op        (1000) op        (1000)     3318 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/house.py
--rw-rw-r--   0 op        (1000) op        (1000)     4441 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/moblib.py
--rw-rw-r--   0 op        (1000) op        (1000)     7630 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/objlib.py
--rw-rw-r--   0 op        (1000) op        (1000)    19757 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/playerfile.py
--rw-rw-r--   0 op        (1000) op        (1000)     3581 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/rent.py
--rw-rw-r--   0 op        (1000) op        (1000)     4088 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/roomlib.py
--rw-rw-r--   0 op        (1000) op        (1000)     9920 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/searchlib.py
--rw-rw-r--   0 op        (1000) op        (1000)     2882 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/shplib.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.336285 stuphos-2.0.8/stuphos/stuphlib/sql/
--rw-rw-r--   0 op        (1000) op        (1000)     2091 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/sql/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)      805 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/stuphlib/sql/item.py
--rw-rw-r--   0 op        (1000) op        (1000)      316 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/stuphlib/sql/room.py
--rw-rw-r--   0 op        (1000) op        (1000)      753 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/stuphlib/sql/zone.py
--rw-rw-r--   0 op        (1000) op        (1000)    19942 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/textlib.py
--rw-rw-r--   0 op        (1000) op        (1000)    22304 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/wldlib.py
--rw-rw-r--   0 op        (1000) op        (1000)     8549 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/stuphlib/zonelib.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.337285 stuphos-2.0.8/stuphos/system/
--rw-rw-r--   0 op        (1000) op        (1000)     6292 2022-11-15 19:21:57.000000 stuphos-2.0.8/stuphos/system/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)       97 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/system/access.py
--rw-rw-r--   0 op        (1000) op        (1000)      846 2022-10-30 11:34:51.000000 stuphos-2.0.8/stuphos/system/api.py
--rw-rw-r--   0 op        (1000) op        (1000)     6582 2022-11-15 14:11:53.000000 stuphos-2.0.8/stuphos/system/cli.py
--rw-rw-r--   0 op        (1000) op        (1000)    12898 2022-11-15 19:21:41.000000 stuphos-2.0.8/stuphos/system/core.py
--rw-rw-r--   0 op        (1000) op        (1000)     4308 2022-09-15 12:29:28.000000 stuphos-2.0.8/stuphos/system/db.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.338285 stuphos-2.0.8/stuphos/system/game/
--rw-rw-r--   0 op        (1000) op        (1000)     1705 2021-11-20 19:30:35.000000 stuphos-2.0.8/stuphos/system/game/__init__.py
--rw-r--r--   0 op        (1000) op        (1000)       69 2021-06-04 15:37:50.000000 stuphos-2.0.8/stuphos/system/game/__main__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.339285 stuphos-2.0.8/stuphos/system/game/compartment/
--rw-rw-r--   0 op        (1000) op        (1000)     2893 2022-11-18 20:36:13.000000 stuphos-2.0.8/stuphos/system/game/compartment/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)    16093 2022-11-08 17:37:54.000000 stuphos-2.0.8/stuphos/system/game/compartment/cli.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.339285 stuphos-2.0.8/stuphos/system/game/compartment/format/
--rw-rw-r--   0 op        (1000) op        (1000)       29 2021-05-25 15:46:03.000000 stuphos-2.0.8/stuphos/system/game/compartment/format/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.339285 stuphos-2.0.8/stuphos/system/game/compartment/misc/
--rw-rw-r--   0 op        (1000) op        (1000)     4430 2022-08-02 14:42:29.000000 stuphos-2.0.8/stuphos/system/game/compartment/misc/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     2494 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/system/game/compartment/misc/devel.py
--rw-rw-r--   0 op        (1000) op        (1000)      136 2021-05-25 15:46:03.000000 stuphos-2.0.8/stuphos/system/game/compartment/system.py
--rw-rw-r--   0 op        (1000) op        (1000)      224 2022-10-30 11:22:49.000000 stuphos-2.0.8/stuphos/system/game/namespace.py
--rw-rw-r--   0 op        (1000) op        (1000)     9269 2022-10-30 11:21:26.000000 stuphos-2.0.8/stuphos/system/network.py
--rw-rw-r--   0 op        (1000) op        (1000)    23450 2022-11-08 18:00:36.000000 stuphos-2.0.8/stuphos/triggers.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.339285 stuphos-2.0.8/stuphos/webserver/
--rw-rw-r--   0 op        (1000) op        (1000)    27201 2022-11-08 18:33:49.000000 stuphos-2.0.8/stuphos/webserver/__init__.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.340285 stuphos-2.0.8/stuphos/webserver/project/
--rw-rw-r--   0 op        (1000) op        (1000)        0 2021-01-25 12:39:25.000000 stuphos-2.0.8/stuphos/webserver/project/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     1791 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/webserver/project/manage.py
--rw-rw-r--   0 op        (1000) op        (1000)     9825 2022-09-19 13:27:46.000000 stuphos-2.0.8/stuphos/webserver/project/settings.py
--rw-rw-r--   0 op        (1000) op        (1000)     6386 2022-11-08 17:20:04.000000 stuphos-2.0.8/stuphos/webserver/project/urls.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.341285 stuphos-2.0.8/stuphos/webserver/services/
--rw-rw-r--   0 op        (1000) op        (1000)       29 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/webserver/services/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     3378 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/webserver/services/checkpointing.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.342285 stuphos-2.0.8/stuphos/xmlrpc/
--rw-rw-r--   0 op        (1000) op        (1000)     2129 2021-09-22 14:07:40.000000 stuphos-2.0.8/stuphos/xmlrpc/__init__.py
--rw-rw-r--   0 op        (1000) op        (1000)     1272 2021-07-23 14:59:08.000000 stuphos-2.0.8/stuphos/xmlrpc/client.py
--rw-rw-r--   0 op        (1000) op        (1000)      762 2021-01-28 13:58:04.000000 stuphos-2.0.8/stuphos/xmlrpc/config.py
--rw-rw-r--   0 op        (1000) op        (1000)    28057 2022-11-08 18:30:39.000000 stuphos-2.0.8/stuphos/xmlrpc/host.py
-drwxrwxr-x   0 op        (1000) op        (1000)        0 2022-11-30 11:35:30.317284 stuphos-2.0.8/stuphos.egg-info/
--rw-rw-r--   0 op        (1000) op        (1000)    11382 2022-11-30 11:35:30.000000 stuphos-2.0.8/stuphos.egg-info/PKG-INFO
--rw-rw-r--   0 op        (1000) op        (1000)     7319 2022-11-30 11:35:30.000000 stuphos-2.0.8/stuphos.egg-info/SOURCES.txt
--rw-rw-r--   0 op        (1000) op        (1000)        1 2022-11-30 11:35:30.000000 stuphos-2.0.8/stuphos.egg-info/dependency_links.txt
--rw-rw-r--   0 op        (1000) op        (1000)       17 2022-11-30 11:35:30.000000 stuphos-2.0.8/stuphos.egg-info/top_level.txt
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.542825 stuphos-2.0.9/
+-rw-r--r--   0 Owner    (197610) None     (197121)       28 2022-12-09 19:32:54.000000 stuphos-2.0.9/MANIFEST.in
+-rw-r--r--   0 Owner    (197610) None     (197121)     8483 2023-02-06 17:03:12.542825 stuphos-2.0.9/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)     6017 2022-12-09 19:32:54.000000 stuphos-2.0.9/README
+-rw-r--r--   0 Owner    (197610) None     (197121)       38 2023-02-06 17:03:12.542825 stuphos-2.0.9/setup.cfg
+-rw-r--r--   0 Owner    (197610) None     (197121)     8625 2023-02-06 17:02:14.000000 stuphos-2.0.9/setup.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     5145 2022-12-09 19:32:54.000000 stuphos-2.0.9/setupCMR.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2633 2022-12-09 19:32:54.000000 stuphos-2.0.9/skeletoncore.tar.gz
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.308440 stuphos-2.0.9/stuphmud/
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       50 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/elemental.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.308440 stuphos-2.0.9/stuphmud/server/
+-rw-r--r--   0 Owner    (197610) None     (197121)      683 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    25778 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/adapters.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.355316 stuphos-2.0.9/stuphmud/server/api/
+-rw-r--r--   0 Owner    (197610) None     (197121)     7149 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/api/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       26 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/api/constants.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    62523 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/api/structs.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4917 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/api/tests.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.355316 stuphos-2.0.9/stuphmud/server/magic/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2136 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/magic/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      505 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/magic/structure.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.386564 stuphos-2.0.9/stuphmud/server/player/
+-rw-r--r--   0 Owner    (197610) None     (197121)    15071 2023-01-02 14:56:28.000000 stuphos-2.0.9/stuphmud/server/player/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.402193 stuphos-2.0.9/stuphmud/server/player/commands/
+-rw-r--r--   0 Owner    (197610) None     (197121)     3618 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.449067 stuphos-2.0.9/stuphmud/server/player/commands/gc/
+-rw-r--r--   0 Owner    (197610) None     (197121)      114 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    11488 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/olc.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9186 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/profiling.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6353 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/system.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1891 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/web_debug.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    32671 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/wizard.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    10636 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/gc/xdebug.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8263 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/commands/mime.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.464689 stuphos-2.0.9/stuphmud/server/player/db/
+-rw-r--r--   0 Owner    (197610) None     (197121)     8806 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2872 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/hi.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9873 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/managedfs.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8126 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/playerfile.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.511565 stuphos-2.0.9/stuphmud/server/player/db/rent/
+-rw-r--r--   0 Owner    (197610) None     (197121)       46 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       48 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/constants.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     7590 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/edit.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       13 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/equip.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1728 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/management.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2642 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/scan.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3530 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/rent/show.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3243 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/db/sql.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    18861 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/editor.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      704 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/events.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1409 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/http.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.574064 stuphos-2.0.9/stuphmud/server/player/interfaces/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2205 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.605314 stuphos-2.0.9/stuphmud/server/player/interfaces/code/
+-rw-r--r--   0 Owner    (197610) None     (197121)    16834 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/code/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1335 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/code/environ.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    28601 2023-02-01 14:16:29.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/code/girl.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6419 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/code/python.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3025 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/code/xmlrpc_python.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6683 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/dictcmd.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3913 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/history.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6700 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/standard.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1771 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/interfaces/threading.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.605314 stuphos-2.0.9/stuphmud/server/player/messaging/
+-rw-r--r--   0 Owner    (197610) None     (197121)       45 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/messaging/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    17074 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/notebook.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8081 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/shell.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.683442 stuphos-2.0.9/stuphmud/server/player/telnet/
+-rw-r--r--   0 Owner    (197610) None     (197121)      130 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8130 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/client.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3454 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/comm.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1895 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/core.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1702 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/deploy.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    11444 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/dispatch.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     5139 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/ftp.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3806 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/http.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2934 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/pentacle.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2951 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/rexec.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2400 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/player/telnet/test.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.745942 stuphos-2.0.9/stuphmud/server/zones/
+-rw-r--r--   0 Owner    (197610) None     (197121)    19714 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      176 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/combat.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    15315 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/config.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     7392 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/controller.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    18848 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/freeze.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       83 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/physical.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      884 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/space.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.761565 stuphos-2.0.9/stuphmud/server/zones/specials/
+-rw-r--r--   0 Owner    (197610) None     (197121)     8860 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.792821 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/
+-rw-r--r--   0 Owner    (197610) None     (197121)    35280 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      473 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/behaviors.npc
+-rw-r--r--   0 Owner    (197610) None     (197121)      196 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/quest-help-topics.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)     1348 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/quest-help.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)      214 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/quests.cfg
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.792821 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/senarios/
+-rw-r--r--   0 Owner    (197610) None     (197121)     3072 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/senarios/slay1.qst
+-rw-r--r--   0 Owner    (197610) None     (197121)    10104 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/slay.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6281 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/specials/standard.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1931 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphmud/server/zones/wilderness.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.808445 stuphos-2.0.9/stuphos/
+-rw-r--r--   0 Owner    (197610) None     (197121)      980 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.870942 stuphos-2.0.9/stuphos/db/
+-rw-r--r--   0 Owner    (197610) None     (197121)      835 2023-01-05 14:35:25.000000 stuphos-2.0.9/stuphos/db/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6534 2023-01-30 00:37:55.000000 stuphos-2.0.9/stuphos/db/conf.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    25020 2023-01-27 11:49:41.000000 stuphos-2.0.9/stuphos/db/orm.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    12847 2023-01-30 15:18:10.000000 stuphos-2.0.9/stuphos/db/vardb.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.870942 stuphos-2.0.9/stuphos/etc/
+-rw-r--r--   0 Owner    (197610) None     (197121)       21 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.949066 stuphos-2.0.9/stuphos/etc/tools/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2365 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4096 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/cmdln.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    21636 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/collections_hack.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9747 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/debugging.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6629 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/errors.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1215 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/internet.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3932 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/logs.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    13538 2023-01-05 14:50:39.000000 stuphos-2.0.9/stuphos/etc/tools/misc.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      423 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/platform.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6596 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/pyg_colorizer.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     7647 2023-01-05 14:50:53.000000 stuphos-2.0.9/stuphos/etc/tools/strings.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      779 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/timing.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1288 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/etc/tools/urls.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.949066 stuphos-2.0.9/stuphos/kernel/
+-rw-r--r--   0 Owner    (197610) None     (197121)     5781 2023-01-02 14:57:00.000000 stuphos-2.0.9/stuphos/kernel/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.964692 stuphos-2.0.9/stuphos/language/
+-rw-r--r--   0 Owner    (197610) None     (197121)      734 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.980319 stuphos-2.0.9/stuphos/language/board/
+-rw-r--r--   0 Owner    (197610) None     (197121)    14855 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/board/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    32461 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/board/comm.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    16574 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/board/specproc.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.011566 stuphos-2.0.9/stuphos/language/document/
+-rw-r--r--   0 Owner    (197610) None     (197121)       27 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/document/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1747 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/document/interface.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    88775 2023-01-02 14:57:00.000000 stuphos-2.0.9/stuphos/language/document/structural.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    11669 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/document/wrlc.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.011566 stuphos-2.0.9/stuphos/language/gen/
+-rw-r--r--   0 Owner    (197610) None     (197121)    24614 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/gen/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9830 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/gen/gs_indent_lexer.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      116 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/moo.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.027189 stuphos-2.0.9/stuphos/language/query/
+-rw-r--r--   0 Owner    (197610) None     (197121)    11506 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/query/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     5024 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/query/ql2.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9655 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/shortate.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.027189 stuphos-2.0.9/stuphos/language/vm/
+-rw-r--r--   0 Owner    (197610) None     (197121)      511 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/vm/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.042823 stuphos-2.0.9/stuphos/language/xml/
+-rw-r--r--   0 Owner    (197610) None     (197121)    34407 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/xml/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3503 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/language/xml/stuph.xml
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.105317 stuphos-2.0.9/stuphos/management/
+-rw-r--r--   0 Owner    (197610) None     (197121)     5993 2023-01-29 13:43:07.000000 stuphos-2.0.9/stuphos/management/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8827 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/authlock.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       55 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/autowiz.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.152191 stuphos-2.0.9/stuphos/management/command_messaging/
+-rw-r--r--   0 Owner    (197610) None     (197121)      846 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3697 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/base.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      979 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/deployment.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      509 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/girl.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2286 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/python.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3934 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/resource.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.152191 stuphos-2.0.9/stuphos/management/command_messaging/samples/
+-rw-r--r--   0 Owner    (197610) None     (197121)     1256 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/samples/penro_team_core.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1228 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/shell.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      712 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/command_messaging/subdaemon.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     5490 2023-01-30 00:48:27.000000 stuphos-2.0.9/stuphos/management/config.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    14666 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/deploy.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2272 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/idling.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      968 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/naming.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    15454 2023-02-03 13:53:44.000000 stuphos-2.0.9/stuphos/management/packaging.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.167816 stuphos-2.0.9/stuphos/management/protocols/
+-rw-r--r--   0 Owner    (197610) None     (197121)      225 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/protocols/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       58 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/protocols/http.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    13141 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/reboot.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3867 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/services.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6465 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/shell.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    15462 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/subdaemon.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    37704 2023-02-04 21:13:42.000000 stuphos-2.0.9/stuphos/management/syslog.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9875 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/tracking.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    14287 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/tracsite.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      160 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/management/workflow.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.199066 stuphos-2.0.9/stuphos/pentacle/
+-rw-r--r--   0 Owner    (197610) None     (197121)      608 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.199066 stuphos-2.0.9/stuphos/pentacle/federation/
+-rw-r--r--   0 Owner    (197610) None     (197121)       24 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/federation/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      817 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/management.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1098 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/native.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4390 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/oob.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      457 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/partner.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2600 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/pentacle/service.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.199066 stuphos-2.0.9/stuphos/phClient/
+-rw-r--r--   0 Owner    (197610) None     (197121)    27752 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/phClient/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.245940 stuphos-2.0.9/stuphos/runtime/
+-rw-r--r--   0 Owner    (197610) None     (197121)     7099 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.261568 stuphos-2.0.9/stuphos/runtime/architecture/
+-rw-r--r--   0 Owner    (197610) None     (197121)    35954 2023-01-30 15:44:46.000000 stuphos-2.0.9/stuphos/runtime/architecture/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     5355 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/architecture/api.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.261568 stuphos-2.0.9/stuphos/runtime/architecture/lookup/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2582 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/architecture/lookup/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      521 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/architecture/routines.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    20414 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/architecture/spatial.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.277191 stuphos-2.0.9/stuphos/runtime/core/
+-rw-r--r--   0 Owner    (197610) None     (197121)    12607 2023-01-02 14:57:00.000000 stuphos-2.0.9/stuphos/runtime/core/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9831 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/events.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4964 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/facilities.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1972 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/misc.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      275 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/parallel.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8634 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/plugins.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    14239 2023-01-29 12:57:00.000000 stuphos-2.0.9/stuphos/runtime/registry.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4093 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/sandbox.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3546 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/runtime/support.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    74419 2023-02-04 22:02:44.000000 stuphos-2.0.9/stuphos/structure.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.386566 stuphos-2.0.9/stuphos/stuphlib/
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6605 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/binary.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8010 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/boards.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2683 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/cherry.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6309 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/clanlib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    72417 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/constants.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    18082 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/dblib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    26706 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/directory.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1688 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/etc.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2807 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/help.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3318 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/house.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4441 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/moblib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     7630 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/objlib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    19757 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/playerfile.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3581 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/rent.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4088 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/roomlib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9920 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/searchlib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2882 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/shplib.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.402193 stuphos-2.0.9/stuphos/stuphlib/sql/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2091 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/sql/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      805 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/sql/item.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      316 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/sql/room.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      753 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/sql/zone.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    19942 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/textlib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    22304 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/wldlib.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     8549 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/stuphlib/zonelib.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.433442 stuphos-2.0.9/stuphos/system/
+-rw-r--r--   0 Owner    (197610) None     (197121)     6292 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       97 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/access.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      846 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/api.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6701 2023-01-02 14:57:00.000000 stuphos-2.0.9/stuphos/system/cli.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    13073 2023-01-02 14:57:00.000000 stuphos-2.0.9/stuphos/system/core.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     4308 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/db.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.449067 stuphos-2.0.9/stuphos/system/game/
+-rw-r--r--   0 Owner    (197610) None     (197121)     1705 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)       69 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/__main__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.464690 stuphos-2.0.9/stuphos/system/game/compartment/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2893 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/compartment/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    16093 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/compartment/cli.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.464690 stuphos-2.0.9/stuphos/system/game/compartment/format/
+-rw-r--r--   0 Owner    (197610) None     (197121)       29 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/compartment/format/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.480317 stuphos-2.0.9/stuphos/system/game/compartment/misc/
+-rw-r--r--   0 Owner    (197610) None     (197121)     4430 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/compartment/misc/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     2494 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/compartment/misc/devel.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      136 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/compartment/system.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      224 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/game/namespace.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9269 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/system/network.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    23450 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/triggers.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.480317 stuphos-2.0.9/stuphos/webserver/
+-rw-r--r--   0 Owner    (197610) None     (197121)    27391 2023-02-04 11:52:05.000000 stuphos-2.0.9/stuphos/webserver/__init__.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.495942 stuphos-2.0.9/stuphos/webserver/project/
+-rw-r--r--   0 Owner    (197610) None     (197121)        0 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/webserver/project/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      328 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/webserver/project/loadOlc.sh
+-rw-r--r--   0 Owner    (197610) None     (197121)     1791 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/webserver/project/manage.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     9987 2023-01-30 11:29:53.000000 stuphos-2.0.9/stuphos/webserver/project/settings.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     6386 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/webserver/project/urls.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.511567 stuphos-2.0.9/stuphos/webserver/services/
+-rw-r--r--   0 Owner    (197610) None     (197121)       29 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/webserver/services/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     3378 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/webserver/services/checkpointing.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:12.542825 stuphos-2.0.9/stuphos/xmlrpc/
+-rw-r--r--   0 Owner    (197610) None     (197121)     2129 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/xmlrpc/__init__.py
+-rw-r--r--   0 Owner    (197610) None     (197121)     1272 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/xmlrpc/client.py
+-rw-r--r--   0 Owner    (197610) None     (197121)      762 2022-12-09 19:32:54.000000 stuphos-2.0.9/stuphos/xmlrpc/config.py
+-rw-r--r--   0 Owner    (197610) None     (197121)    28333 2023-01-24 20:33:20.000000 stuphos-2.0.9/stuphos/xmlrpc/host.py
+drwxr-xr-x   0 Owner    (197610) None     (197121)        0 2023-02-06 17:03:11.824066 stuphos-2.0.9/stuphos.egg-info/
+-rw-r--r--   0 Owner    (197610) None     (197121)     8483 2023-02-06 17:03:09.000000 stuphos-2.0.9/stuphos.egg-info/PKG-INFO
+-rw-r--r--   0 Owner    (197610) None     (197121)     7749 2023-02-06 17:03:11.000000 stuphos-2.0.9/stuphos.egg-info/SOURCES.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)        1 2023-02-06 17:03:09.000000 stuphos-2.0.9/stuphos.egg-info/dependency_links.txt
+-rw-r--r--   0 Owner    (197610) None     (197121)       17 2023-02-06 17:03:09.000000 stuphos-2.0.9/stuphos.egg-info/top_level.txt
```

### Comparing `stuphos-2.0.8/PKG-INFO` & `stuphos-2.0.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,266 +1,15 @@
 Metadata-Version: 2.1
 Name: stuphos
-Version: 2.0.8
-Summary: Containerization middleware.
+Version: 2.0.9
+Summary: Online productivity container.
 Home-page: http://thetaplane.com
 Author: 
 Author-email: 
 License: None
-Description: Copyright 2009-2022 Thetaplane . com
-        ====================================
-        
-        Virtualizes python so that it is isolated and controlled in terms of resource usage per
-        registered user account, and all operations are tracked by time, generating computational
-        telemetry and executive management.
-        
-        
-        Intended Audiences
-        ==================
-        
-        * System administrators who want to support protected user multitasking without system
-          management overhead.
-        * Web administrators who want to publish a CMS site with integrated real-time networking.
-        * Physical and computational scientific research.  Python 3 users.
-        
-        
-        Legal and Operational Notes
-        ===========================
-        
-        This software makes use of cryptographic algorithms, designed to protect the user data
-        and the user, but may be restricted in jurisdictions that overrule their use.
-        
-        Please research the full law regarding data and information security.
-        
-        THERE IS ABSOLUTELY NO WARRANTY INCLUDED.
-        
-        
-        Starting
-        ========
-        
-        Unpack the skeletoncore.tar.gz directory and configure it for your application (the
-        location of the stuphos packages in your PYTHONPATH), then switch to that directory
-        and run it like this: ./runcore --headless &
-        
-        Connect to it with a web browser.
-        
-        
-        Boot Procedure
-        ==============
-        
-        An embedding core invokes the boot start and complete routines in the mud module to
-        initialize the bindings and runtime.
-        
-        These things start up in the application, opening up all components and facilities.
-        
-            * Event bridge module is constructed and initialized
-            * Registry is configured (with bridge for shutdown events)
-            * VM installed
-            * Site packages are loaded
-            * Paths for system packages are configured
-            * Environment updated
-            * XMLRPC host started
-            * System journal installed, system packages loaded
-        
-            * Management components
-                * Web Adapter Session Manager
-                * WSGI Webserver
-        
-            * Facilities:
-                * AgentSystem and Elemental Interpreter
-        
-            * Zones
-            * Commands
-            * Warmboot
-            * Engine Loop
-        
-        
-        Application & Core Architecture
-        ===============================
-        
-        The system uses a collection of components to build its application of managing objects.
-        One of the components is the 'registry' which names unique objects within the runtime,
-        and requires that it be installed during boot time (this is normally handled by the
-        boot procedure).
-        
-        Other component package implementations are configured using the 'components.pth' file
-        for service implementations, external (third-party) server package installations, and
-        developmental modules.
-        
-        
-        Supplemental
-        ============
-        
-        With an extended license, the 'ph' package contains a virtual machine computational
-        core and database querying engine.
-        
-        The 'stuphmud' package contains code previously released in ''stuphos-lite''.
-        
-        
-        Filesystem and Command-Line Configuration
-        =========================================
-        
-        Options:
-            -w --world-dir                          path
-            -z --zone-index --index                 string
-            -i --interactive                        bool
-            -a --async                              bool
-            -W --cascade --load-world               bool
-            -C --config-file --config --game-config path
-            -g --debug                              count
-            -n --no-world                           bool
-            -p --port                               integer
-            -m --mud-package --mud                  string
-            -s --supreme                            bool
-            --admin-name                            string
-            --enter-game                            bool
-            -L --data-dir --lib-dir                 path
-            -v --verbose                            count
-            --headless --no-console                 bool
-        
-        Experimental:
-            --blocking                              integer
-            --runpid                                bool
-            --timeout                               integer
-        
-            --parser-tokenize                       bool
-            --elemental-parser-debug, --parser-debug
-        
-            --no-run-engine                         bool
-        
-        Additional:
-            --reset-world                           bool
-            -Z, --full-world                        bool
-            -e, --service                           list
-        
-            --admin-script                          string
-            -x, --admin-script-args                 list
-        
-            -f, --file                              string
-        
-            -c, --admin-command                     string
-            --admin-trace                           bool
-        
-            --no-init                               bool
-        
-            --tool-package                          list
-            --agent-system                          string
-            --local, --local-filesystem             string
-        
-        
-        The configuration file has the following options:
-        
-            [MUD]
-            config-dir = .
-            components: components.pth
-            traceback-relative: yes
-            log-uncaught-traceback: yes
-            logindent = 4
-            greetings: name prompt %w means whitespace
-            greeting-delay: 1.2
-            http-redirect-url: https://thetaplane.com/
-            player-store-shelf = %(config-dir)s/.players.shelf
-            zone-config-file = .zone-modules.cfg
-            world-path = ../../lib/archive/lib/world
-            olc-world-path = ../../lib/archive/lib/world
-            zone-database: sqlite
-        
-        
-            [Management]
-            embedded-webserver: yes
-            pentacle-service: no
-            session-adapter: yes
-            system-shell: no
-            subdaemon-manager: no
-            syslog-scanner: no
-        
-        
-            [XMLRPC]
-            off: off
-            address: 0.0.0.0
-            ; certificate-path = server.pem
-        
-        
-            [Security]
-            trust-localhost: yes
-            ; trusted-domain: 10.0.0.1
-        
-        
-            [Interpreter]
-            rich-editor: yes
-            player-notebook: yes
-            wizard-gc: yes
-            checkpointing: no
-            native-traceback: yes ; no
-        
-        
-            [Environment]
-            PENTACLE_PARTNER_NAME = 'stuphos/mud'
-        
-        
-            [Syslog]
-            path.1: ..\log\syslog*
-            path.2: mattercore.run.log
-            patterns: etc\syslog-patterns.cfg
-        
-        
-            [Services]
-            facility.billing: ph.emulation.billing.BillingCore
-        
-        
-            [DjangoService]
-            port = 2180
-            database = sqlite
-            sitemap = stuphos.webserver.project.urls
-            show-debug-page = admin
-            certificate-path = server.pem
-            software: phaseware
-            log-request: yes
-            hosts:
-                <public ip address 1>
-                <hostname 1>
-                <hostname 2>
-                ...
-            media:
-                serving-path: folder-path
-            webapps:
-                person.services.web
-                ...
-        
-            [DBCore]
-            primary.type = pg-auth
-            primary.path = ../lib/db.conf ; username\npassword\n
-            primary.host = 127.0.0.1
-            primary.port = 5432
-            sqlite.type = sqlite
-            sqlite.path = sqlite:webcore.db
-            sqlite.file-path = webcore.db
-        
-        
-            [SystemComponents]
-            system-path.common: /workspace/library/packages/common
-        
-            [SystemPackages]
-            package.wrlc: op
-        
-            [Logging]
-            database: sqlite
-        
-            [Billing]
-            policy-rates-path = ../resources/rates.wmc
-        
-        
-        
-        Web Interface Guide
-        ===================
-        
-        The application is developed internally by programming principals, which require user
-        authentication.  Programming documentation should be viewable within the online interface.
-        
-        
 Platform: OS-independent
 Platform: Many
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Environment :: Other Environment
 Classifier: Environment :: Web Environment
@@ -300,7 +49,233 @@
 Classifier: Topic :: System :: Operating System Kernels
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals :: Telnet
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
 Description-Content-Type: text/plain
+
+Copyright 2009-2022 Thetaplane . com
+====================================
+
+Virtualizes python so that it is isolated and controlled in terms of resource usage per
+registered user account, and all operations are tracked by time, generating computational
+telemetry and executive management.
+
+
+Intended Audiences
+==================
+
+* System administrators who want to support protected user multitasking without system
+  management overhead.
+* Web administrators who want to publish a CMS site with integrated real-time networking.
+* Physical and computational scientific research.  Python 3 users.
+
+
+Legal and Operational Notes
+===========================
+
+This software makes use of cryptographic algorithms, designed to protect the user data
+and the user, but may be restricted in jurisdictions that overrule their use.
+
+Please research the full law regarding data and information security.
+
+THERE IS ABSOLUTELY NO WARRANTY INCLUDED.
+
+
+Starting
+========
+
+Unpack the skeletoncore.tar.gz directory and configure it for your application (the
+location of the stuphos packages in your PYTHONPATH), then switch to that directory
+and run it like this: ./runcore --headless &
+
+Connect to it with a web browser.
+
+
+Boot Procedure
+==============
+
+An embedding core invokes the boot start and complete routines in the mud module to
+initialize the bindings and runtime.
+
+These things start up in the application, opening up all components and facilities.
+
+    * Registry is configured
+    * Site packages are loaded
+    * Event bridge module is constructed and initialized
+    * VM, system journal installed
+    * System package paths are installed
+    * Environment updated
+    * XMLRPC host started
+    * Management components
+        * Web Adapter Session Manager
+        * WSGI Webserver
+
+    * Facilities:
+        * AgentSystem and Elemental Interpreter
+
+    * Zones
+    * Commands
+    * Warmboot
+    * Engine Loop
+
+
+Application & Core Architecture
+===============================
+
+The system uses a collection of components to build its application of managing objects.
+One of the components is the 'registry' which names unique objects within the runtime,
+and requires that it be installed during boot time (this is normally handled by the
+boot procedure).
+
+Other component package implementations are configured using the 'components.pth' file
+for service implementations, external (third-party) server package installations, and
+developmental modules.
+
+
+Supplemental
+============
+
+With an extended license, the 'ph' package contains a virtual machine computational
+core and database querying engine.
+
+The 'stuphmud' package contains code previously released in ''stuphos-lite''.
+
+
+Filesystem and Command-Line Configuration
+=========================================
+
+Options:
+    -w --world-dir                          path
+    -z --zone-index --index                 string
+    -i --interactive                        bool
+    -a --async                              bool
+    -W --cascade --load-world               bool
+    -C --config-file --config --game-config path
+    -g --debug                              count
+    -n --no-world                           bool
+    -p --port                               integer
+    -m --mud-package --mud                  string
+    -s --supreme                            bool
+    --admin-name                            string
+    --enter-game                            bool
+    -L --data-dir --lib-dir                 path
+    -v --verbose                            count
+    --headless --no-console                 bool
+
+Experimental:
+    --blocking                              integer
+    --runpid                                bool
+
+
+The configuration file has the following options:
+
+    [MUD]
+    config-dir = .
+    components: components.pth
+    traceback-relative: yes
+    log-uncaught-traceback: yes
+    logindent = 4
+    greetings: name prompt %w means whitespace
+    greeting-delay: 1.2
+    http-redirect-url: https://runphase.com:2180/
+    player-store-shelf = %(config-dir)s/.players.shelf
+    zone-config-file = .zone-modules.cfg
+    world-path = ../../lib/archive/lib/world
+    olc-world-path = ../../lib/archive/lib/world
+    zone-database: sqlite
+
+
+    [Management]
+    embedded-webserver: yes
+    pentacle-service: no
+    session-adapter: yes
+    system-shell: no
+    subdaemon-manager: no
+    syslog-scanner: no
+
+
+    [XMLRPC]
+    off: off
+    address: 0.0.0.0
+    ; certificate-path = server.pem
+
+
+    [Security]
+    trust-localhost: yes
+    ; trusted-domain: 10.0.0.1
+
+
+    [Interpreter]
+    rich-editor: yes
+    player-notebook: yes
+    wizard-gc: yes
+    checkpointing: no
+    native-traceback: yes ; no
+
+
+    [Environment]
+    PENTACLE_PARTNER_NAME = 'stuphos/mud'
+
+
+    [Syslog]
+    path.1: ..\log\syslog*
+    path.2: mattercore.run.log
+    patterns: etc\syslog-patterns.cfg
+
+
+    [Services]
+    facility.billing: ph.emulation.billing.BillingCore
+
+
+    [DjangoService]
+    port = 2180
+    database = sqlite
+    sitemap = stuphos.webserver.project.urls
+    show-debug-page = admin
+    certificate-path = server.pem
+    software: phaseware
+    log-request: yes
+    hosts:
+        <public ip address 1>
+        <hostname 1>
+        <hostname 2>
+        ...
+    media:
+        serving-path: folder-path
+    webapps:
+        person.services.web
+        ...
+
+    [DBCore]
+    primary.type = pg-auth
+    primary.path = ../lib/db.conf ; username\npassword\n
+    primary.host = 127.0.0.1
+    primary.port = 5432
+    sqlite.type = sqlite
+    sqlite.path = sqlite:webcore.db
+    sqlite.file-path = webcore.db
+
+
+    [SystemComponents]
+    system-path.common: /workspace/library/packages/common
+
+    [SystemPackages]
+    package.wrlc: op
+
+    [Logging]
+    database: sqlite
+
+    [Billing]
+    policy-rates-path = ../resources/rates.wmc
+
+
+
+Web Interface Guide
+===================
+
+The application is developed internally by programming principals, which require user
+authentication.  Programming documentation should be viewable within the online interface.
+
+
+
```

### Comparing `stuphos-2.0.8/setup.py` & `stuphos-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!python
-VERSION = '2.0.8'
+VERSION = '2.0.9'
 
 # Major Version 2 Release - python 3, primarily, cython
 
 # from op.subsystem.project.distribution import structured
 
 CMRWebsite = ''
 
@@ -147,15 +147,15 @@
         del sys.argv[0]
 
         try: from setuptools import setup, find_packages
         except ImportError: from distutils.core import setup, find_packages
 
         SETUP_CONF = \
         dict (name = "stuphos",
-              description = "Containerization middleware.",
+              description = "Online productivity container.",
               download_url = "",
 
               license = "None",
               platforms = ['OS-independent', 'Many'],
 
               include_package_data = True,
```

### Comparing `stuphos-2.0.8/skeletoncore.tar.gz` & `stuphos-2.0.9/skeletoncore.tar.gz`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/__init__.py` & `stuphos-2.0.9/stuphmud/server/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/adapters.py` & `stuphos-2.0.9/stuphmud/server/adapters.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/api/__init__.py` & `stuphos-2.0.9/stuphmud/server/api/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/api/structs.py` & `stuphos-2.0.9/stuphmud/server/api/structs.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/api/tests.py` & `stuphos-2.0.9/stuphmud/server/api/tests.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/magic/__init__.py` & `stuphos-2.0.9/stuphmud/server/magic/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/__init__.py` & `stuphos-2.0.9/stuphmud/server/player/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     # Eventually, logged in states differ from enter-game states.
 
     # Since this isn't done anywhere else during the emerge_internal_peer service call.
     # This should be moved before enterGame.  Do in enterGame.
     avatar.room = getStartRoom(avatar)
 
     # debugOn()
+    # This indirectly calls enterGame (below).
     StuphMUD.EnterGame(peer, avatar, webAdapter = webAdapter, post = post)
 
     # XXX :skip: Todo: do this by way of enterGame.
     # self.updateCharacter() # selecting 'Character' in player menu will call do-score command.
     # Done via SessionManager.onPlayerActivate
     # if webAdapter:
     #     peer.session.updateLocation()
@@ -191,29 +192,32 @@
     player = MobileAdapter(player) # System perspective
 
 
     # Enter game script: task.
     from stuphmud.elemental import PlayerScript
 
     # Todo: configure these based on webAdapter parameter.
-    script = configuration.Interpreter.enter_game_script or ENTER_GAME_SCRIPT
+    script = configuration.Interpreter.enter_game_script
+    script = script.strip() if isinstance(script, str) else ENTER_GAME_SCRIPT
     debug = configuration.Interpreter.debug_bridge or DEBUG_ENTER_GAME
 
     if debug not in ['stack', 'console']:
         debug = isYesValue(debug)
 
     # debugOn()
+    scriptComplete = bool(script)
     if script:
         if post:
             def initialize(task):
                 # From the web adapter login request.
                 task.frame.locals['post'] = task.mapping(*post.items())
         else:
             initialize = None
 
+        # todo: onComplete: scriptComplete = bool(task.stack.pop()[0])
         PlayerScript.evaluateEvent(peer, script,
                                    tracing = debug,
                                    initialize = initialize,
                                    player = player)
 
 
     # # Greeting & Enter game script: todo: move into the above evaluateEvent.
@@ -248,15 +252,16 @@
     #         session.postMessages(['javascript', str(result)])
 
 
     # This runs before the customizers, because they have to wait for the vm.
     # This means the scriptable event, too.  But also this statement is required,
     # and so far there's nothing that makes anything in enterGame rely on the
     # customization code.
-    postJavascript(peer, 'enterGame();' if script else 'enterGame(complete = true);')
+    postJavascript(peer, 'enterGame();' if scriptComplete else
+                   'enterGame(complete = true);')
 
 
 # Rudimentary Access Policy.
 TRUSTED_FILENAME = 'etc/trust.python'
 class Trust(dict):
     def __init__(self, filename = TRUSTED_FILENAME):
         self.filename = filename
@@ -324,14 +329,15 @@
     domains = getSecureDomains()
     if TRUST_ALL:
         return True
 
     return domainName.lower() in domains
 
 def isFromSecureHost(peer):
+    # debugOn()
     if getattr(peer, 'session', None) is not None:
         # Authenticated via SSL.
         if isYesValue(configuration.Security.trust_web_session_adapter):
             return True
 
     return isSecureDomain(peer.host)
```

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/__init__.py` & `stuphos-2.0.9/stuphmud/server/player/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/gc/olc.py` & `stuphos-2.0.9/stuphmud/server/player/commands/gc/olc.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/gc/profiling.py` & `stuphos-2.0.9/stuphmud/server/player/commands/gc/profiling.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/gc/system.py` & `stuphos-2.0.9/stuphmud/server/player/commands/gc/system.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/gc/web_debug.py` & `stuphos-2.0.9/stuphmud/server/player/commands/gc/web_debug.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/gc/wizard.py` & `stuphos-2.0.9/stuphmud/server/player/commands/gc/wizard.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/gc/xdebug.py` & `stuphos-2.0.9/stuphmud/server/player/commands/gc/xdebug.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/commands/mime.py` & `stuphos-2.0.9/stuphmud/server/player/commands/mime.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/__init__.py` & `stuphos-2.0.9/stuphmud/server/player/db/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/hi.py` & `stuphos-2.0.9/stuphmud/server/player/db/hi.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/managedfs.py` & `stuphos-2.0.9/stuphmud/server/player/db/managedfs.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/playerfile.py` & `stuphos-2.0.9/stuphmud/server/player/db/playerfile.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/rent/edit.py` & `stuphos-2.0.9/stuphmud/server/player/db/rent/edit.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/rent/management.py` & `stuphos-2.0.9/stuphmud/server/player/db/rent/management.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/rent/scan.py` & `stuphos-2.0.9/stuphmud/server/player/db/rent/scan.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/rent/show.py` & `stuphos-2.0.9/stuphmud/server/player/db/rent/show.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/db/sql.py` & `stuphos-2.0.9/stuphmud/server/player/db/sql.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/editor.py` & `stuphos-2.0.9/stuphmud/server/player/editor.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/events.py` & `stuphos-2.0.9/stuphmud/server/player/events.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/http.py` & `stuphos-2.0.9/stuphmud/server/player/http.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/__init__.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/code/__init__.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/code/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/code/environ.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/code/environ.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/code/girl.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/code/girl.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         TaskCreation.__init__(self, *args, **kwd)
 
         self.peer = peer
         self.completion = completion
         self.initialize = initialize
         # self.environ = environ
 
+        # debugOn()
         if peer is None:
             self.programmer = DEFAULT_PROGRAMMER
             self.user = None
         else:
             name = peer.avatar.name
             self.programmer = Programmer(name)
             self.user = findUserByName(name)
@@ -90,14 +91,16 @@
         if tracing:
             # debugOn()
             if isYesValue(configuration.Interpreter.console_operator) or tracing == 'console':
                 self.tracing = self.traceToConsole
             else:
                 self.tracing = self.debugInstructionPeer(self.peer)
 
+            if tracing == 'full-stack' and isYesValue(configuration.AgentSystem.allow_full_stack):
+                self.debugStack = 'full'
             if tracing in ['stack', 'console']:
                 self.debugStack = True
 
 
     def frameOneForPeer(self, peer, *args, **kwd):
         return Script.frameOne(self, *args, **kwd)
 
@@ -402,19 +405,21 @@
                          this = PeerAdapter(peer),
                          me = MobileAdapter(actor))
 
             task = self.evaluateCode(peer, peer.interpreter, program, scope,
                                      tracing = getGirlTracingLevel(peer))
 
             if task is not None:
+                # XXX Since using evaluateCode means automatically using a
+                # reprCompletion, this completion will fail (silently).
                 @task.onComplete
                 def completion(_, exception = None, traceback = None):
                     if exception is None:
                         try: outcome = task.stack.pop()[0]
-                        except IndexError: pass # Shouldn't happen
+                        except IndexError: pass # Shouldn't happen (see above)
                         else: task.handleVerbOutcome(outcome, command, argstr)
 
                 # Consider this command handled.
                 return True
 
     @classmethod
     def evaluateWebCommand(self, peer, interpreter, scope, completion,
@@ -426,22 +431,25 @@
         code = configuration.Interpreter.web_command_task or WEB_COMMAND_TASK
 
         try: program = Girl(Girl.Module, code + '\n')
         except GrammaticalError as e:
             print(f'{code}:')
             print(e.report())
         else:
+            # debugOn()
             if not isinstance(params, dict):
                 params = dict()
 
             params.update(environ)
             scope.update(session = sessionAdapter,
                          script = script,
                          syntax = syntax)
 
+            scope['instance$'] = sessionAdapter
+
             def paramsInit(task, frame):
                 scope['parameters'] = task.Environment(task.memory, params)
 
             return self.evaluateCode(peer, peer.interpreter, program, scope,
                                      tracing = getGirlTracingLevel(peer),
                                      initialize = paramsInit)
 
@@ -454,22 +462,24 @@
         except GrammaticalError as e:
             print(f'{code}:')
             print(e.report())
         else:
             task = self.evaluateCode(peer, peer.interpreter, program, scope,
                                      tracing = tracing, **environ)
 
-            @task.onComplete
-            def eventComplete(_, exception = None, traceback = None):
-                # debugOn()
-                if exception is not None:
-                    # Uncaught error.
-                    peer.sendTraceback(exception)
+            if task is not None:
+                @task.onComplete
+                def eventComplete(_, exception = None, traceback = None):
+                    # debugOn()
+                    if exception is not None:
+                        # Uncaught error.
+                        peer.sendTraceback(task, exception, traceback)
+                        # return True
 
-            return True
+                return True
 
 
     @classmethod
     def evaluateMethodCall(self, request, path, name, *args):
         # RPC.  See phsite.network.adapter.commands.doCallMethod alternatively.
         # todo: finish:
         #   instantiate self for task class
```

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/code/python.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/code/python.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/code/xmlrpc_python.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/code/xmlrpc_python.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/dictcmd.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/dictcmd.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/history.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/history.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/standard.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/standard.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/interfaces/threading.py` & `stuphos-2.0.9/stuphmud/server/player/interfaces/threading.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/notebook.py` & `stuphos-2.0.9/stuphmud/server/player/notebook.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/shell.py` & `stuphos-2.0.9/stuphmud/server/player/shell.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/client.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/client.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/comm.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/comm.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/core.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/core.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/deploy.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/deploy.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/dispatch.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/dispatch.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/ftp.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/ftp.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/http.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/http.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/pentacle.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/pentacle.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/rexec.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/rexec.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/player/telnet/test.py` & `stuphos-2.0.9/stuphmud/server/player/telnet/test.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/__init__.py` & `stuphos-2.0.9/stuphmud/server/zones/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/config.py` & `stuphos-2.0.9/stuphmud/server/zones/config.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/controller.py` & `stuphos-2.0.9/stuphmud/server/zones/controller.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/freeze.py` & `stuphos-2.0.9/stuphmud/server/zones/freeze.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/space.py` & `stuphos-2.0.9/stuphmud/server/zones/space.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/specials/__init__.py` & `stuphos-2.0.9/stuphmud/server/zones/specials/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/specials/autoquest/__init__.py` & `stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/specials/autoquest/slay.py` & `stuphos-2.0.9/stuphmud/server/zones/specials/autoquest/slay.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/specials/standard.py` & `stuphos-2.0.9/stuphmud/server/zones/specials/standard.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphmud/server/zones/wilderness.py` & `stuphos-2.0.9/stuphmud/server/zones/wilderness.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/__init__.py` & `stuphos-2.0.9/stuphos/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/db/__init__.py` & `stuphos-2.0.9/stuphos/db/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/db/conf.py` & `stuphos-2.0.9/stuphos/db/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,17 +128,31 @@
 	    self.hub.processConnection = None if name is None else self.getConnection(name)
 
 	@property
 	def hub(self):
 	    from sqlobject import sqlhub
 	    return sqlhub
 
+
+	class ConnectionDescriptor:
+		def __init__(self, connectString):
+			self.connectString = connectString
+
+		def __call__(self):
+			return self.connectString
+
+
 	def getConnection(self, name):
-	    from sqlobject import connectionForURI
-	    return connectionForURI(self[name].connectionString)
+		if isinstance(name, self.ConnectionDescriptor):
+			connect = name()
+		else:
+			connect = self[name].connectionString
+
+		from sqlobject import connectionForURI
+		return connectionForURI(connect)
 
 	def getDjangoDatabaseConfig(self, name):
 	   	return self[name].djangoDatabaseConfig
 
 	@contextmanager
 	def hubThread(self, name):
 		hub = self.hub
```

### Comparing `stuphos-2.0.8/stuphos/db/orm.py` & `stuphos-2.0.9/stuphos/db/orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -762,14 +762,15 @@
     pass
 
 try:
     class DatabaseConfiguration(SQLObject):
         name = StringCol()
         path = StringCol()
         hard = IntCol()
+        flags = IntCol()
 
 except ValueError: # Already in registry.
     pass
 
 
 try:
     class BillableAccount(SQLObject):
@@ -794,14 +795,78 @@
         superior = StringCol()
         inferior = StringCol()
 
 except ValueError: # Already in registry.
     pass
 
 
+try:
+    class InvoiceAccount(SQLObject):
+        name = StringCol()
+        type = StringCol()
+        debitCompute = FloatCol(default = 0.0)
+        debitContent = FloatCol(default = 0.0)
+
+except ValueError: # Already in registry.
+    pass
+
+try:
+    class InvoiceChargePath(SQLObject):
+        # External girl_library activity node storing accounted name.
+        pathIdExternal = IntCol()
+
+except ValueError: # Already in registry.
+    pass
+
+try:
+    # debugOn()
+    class InvoiceCharge(SQLObject):
+        account = ForeignKey('InvoiceAccount')
+        creation = DateTimeCol()
+        paid = StringCol(default = None) # XXX What I want is a NULLABLE DateTimeCol
+        type = IntCol()
+        charge = FloatCol()
+        path = ForeignKey('InvoiceChargePath', default = None)
+        memo = StringCol()
+        runId = FloatCol()
+
+except ValueError: # Already in registry.
+    pass
+
+try:
+    class InvoiceBillpoint(SQLObject):
+        account = ForeignKey('InvoiceAccount')
+        charge = ForeignKey('InvoiceCharge')
+
+        creation = DateTimeCol()
+        name = StringCol()
+
+        debitCompute = FloatCol()
+        debitContent = FloatCol()
+
+        debitComputeChargeUSD = FloatCol(default = -1.0)
+        debitContentChargeUSD = FloatCol(default = -1.0)
+
+        debitChargeTotalUSD = FloatCol(default = -1.0)
+        feeMarkup = FloatCol(default = 1.0)
+
+except ValueError: # Already in registry.
+    pass
+
+try:
+    class InvoiceQuotaObject(SQLObject):
+        account = ForeignKey('InvoiceAccount')
+        type = StringCol()
+        hard = IntCol()
+        exceeded = IntCol()
+
+except ValueError: # Already in registry.
+    pass
+
+
 # from sqlobject import JSONCol
 from sqlobject import BoolCol
 
 class VariableDBNativeTool:
     # imported dynamically from conf because sqlite is broken.
     def __init__(self, core, vardb):
         self._core = core
@@ -884,7 +949,13 @@
 def selectTableSql(cursor, table):
     cursor.execute('select %s from %s' % (', '.join(table.FIELDS), table.name))
 
     def toModel(row):
         return table.FieldsClass(**dict(list(zip(table.FIELDS, row))))
 
     return list(map(toModel, cursor))
+
+def createSQLObjectTable(table):
+    from sqlobject.dberrors import OperationalError
+    try: table.createTable()
+    except OperationalError:
+        pass
```

### Comparing `stuphos-2.0.8/stuphos/db/vardb.py` & `stuphos-2.0.9/stuphos/db/vardb.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,16 +31,20 @@
 
 def createSqlTable(table):
 	from sqlobject.dberrors import OperationalError
 	try: table.createTable()
 	except OperationalError:
 		pass
 
+# Database Flags.
+DBFLAG_NOACCOUNT = (1 << 0)
 
-class VariableDB(writeprotected, AutoMemoryMapping, representable):
+
+# class VariableDB(writeprotected, AutoMemoryMapping, representable):
+class VariableDB(writeprotected, representable):
 	# _preserve_memory_binding = True
 	_memoryObjectManaged = True
 
 	@classmethod
 	def _Select(self, name):
 		with database():
 			yield from orm.DatabaseConfiguration.selectBy(name = name)
@@ -52,24 +56,25 @@
 				yield db.name
 
 	@classmethod
 	def _Open(self, name, **cfg):
 		for dbConf in self._Select(name):
 			# Note: relies on wrlc
 			handle = sqlite.pathOpen(io.here(dbConf.path))
-			return self(name, dbConf.hard, handle, **cfg)
+			return self(name, dbConf.hard, dbConf.flags, handle, **cfg)
 
 		raise NameError(name)
 
 	@classmethod
-	def _Create(self, name, path, hard):
+	def _Create(self, name, path, hard, flags = 0):
 		for dbConf in self._Select(name):
 			raise NameError(name)
 
-		return orm.DatabaseConfiguration(name = name, path = path, hard = hard)
+		return orm.DatabaseConfiguration(name = name, path = path,
+										 hard = hard, flags = flags)
 
 	class _Namespace(writeprotected, representable):
 		def __init__(self, object):
 			self._object = object
 
 		def __getattr__(self, name):
 			try: return object.__getattribute__(self, name)
@@ -77,24 +82,26 @@
 				try: return self._object[name]
 				except KeyError:
 					raise AttributeError(name)
 
 
 	# __public_members__ = ['name', 'tables']
 
-	def __init__(self, name, hard, db, **cfg):
-		AutoMemoryMapping.__init__(self)
+	def __init__(self, name, hard, flags, db, **cfg):
+		# AutoMemoryMapping.__init__(self)
+		self._tables = dict()
 		self._name = name
 		self._hard = hard
+		self._flags = flags or 0
 		self._db = db
 
 		self._setAttribute('tables', self._Namespace(self))
 		for (name, t) in cfg.items():
 			t._set_database(self)
-			dict.__setitem__(self, name, t)
+			self._tables[name] = t
 
 	@property
 	def name(self):
 		return self._name
 
 	@property
 	def path(self):
@@ -102,27 +109,39 @@
 		vmCurrentTask().checkAccess(r, 'read')
 
 		for dbConf in self._Select(self._name):
 			return dbConf.path
 
 		raise NameError(self._name)
 
+	@property
+	def sqliteConnectURI(self):
+		path = io.path(self.path)
+		return sqlite.sqliteURIFromPath(str(path if path.absolute else io.here(path)))
+
+	@property
+	def noAccount(self):
+		return self._flags & DBFLAG_NOACCOUNT
+
 
 	def __setitem__(self, item, value):
 		raise NotImplementedError('Operation not permitted')
 
+	def __getitem__(self, name):
+		return self._tables[name]
+
 	def __getattr__(self, name):
 		try: return object.__getattribute__(self, name)
 		except AttributeError as e:
 			try: return self[name]
 			except KeyError:
 				raise e
 
 	def _calculateSize(self):
-		return sum(table.size for table in self.values())
+		return sum(table.size for table in self._tables.values())
 
 	@property
 	def size(self):
 		try: return self._size
 		except AttributeError:
 			self._size = size = self._calculateSize()
 			return size
@@ -178,36 +197,41 @@
 			# print string.call('newClassObject', name, (sqlite.Object,), **cfg)
 			# from sqlite.module.classregistry import registry
 			# registry(db.name)
 
 			assert isinstance(db, VariableDB)
 			self._database = db
 
+			noAcct = db.noAccount
+
 			class sqlmeta:
 				registry = db.name
 				lazyUpdate = True
 
 			cfg = dict(self._definition, sqlmeta = sqlmeta)
 
 			# XXX When calling from the native interface, the cfg will have objects
 			# of class VariableDBNativeTool._Column which would make this code wrong.
 			# But when built from the structural 'table' function defined below, it
 			# builds the _columnClass for the type per column name, out of the Open
 			# call connecting database, which is the right level for sqlobject.
 			self._tableClass = buildSqlObject(self.name, db.name, cfg)
 
-			self._accountingTable = buildSqlObject \
-				('%s_acct' % self.name, db.name,
-				 self._accounting_definition(sqlmeta))
+			if not noAcct:
+				self._accountingTable = buildSqlObject \
+					('%s_acct' % self.name, db.name,
+					 self._accounting_definition(sqlmeta))
 
 			self._tableClass._connection = db._db
-			self._accountingTable._connection = db._db
+			if not noAcct:
+				self._accountingTable._connection = db._db
 
 			createSqlTable(self._tableClass)
-			createSqlTable(self._accountingTable)
+			if not noAcct:
+				createSqlTable(self._accountingTable)
 
 		def _calculateSize(self):
 			return sum(row.size for row in self._accountingTable.select())
 
 		@property
 		def size(self):
 			try: return self._size
@@ -337,31 +361,43 @@
 					return f'<{self._table._name} {self._values}>'
 
 				return f'<{self._table._name} {self._row}>'
 
 			def __getattr__(self, name):
 				try: return object.__getattribute__(self, name)
 				except AttributeError as e:
-					return self.getValue(name)
+					try: return self.getValue(name)
+					except KeyError:
+						raise e
 
 			def getValue(self, name):
 				if self._row is None:
-					try: return self._values[name]
-					except KeyError:
-						raise e
+					return self._values[name]
 
 				if any(name == n for (n, c) in self._table._definition):
 					return getattr(self._row, name)
 
 
 			def _getColumnValues(self):
 				v = self._values
 				return [v[n] for (n, c) in self._table._definition]
 
+			def _saveNoAccount(self):
+				if self._row is None:
+					self._row = self._table._tableClass(**self._values) # insert
+
+				else:
+					self._row.sync()
+
+				return self
+
 			def save(self):
+				if self._table._database.noAccount:
+					return self._saveNoAccount()
+
 				def sizeOf(v):
 					if isinstance(v, str):
 						return len(v)
 
 					return 4 # or 8?
 
 				def insertAcct(size):
@@ -419,14 +455,15 @@
 		core.newToolConfig(package = VariableDBNativeTool(core, self),
 						   path = path)
 
 
 # def table(name, **cfg):
 #     return newClass(name, (sqlite.Object,) **value)
 
+# used?
 vardb = VariableDB._Open
 createdb = VariableDB._Create
 
 # table = VariableDB.Table
 
 # vardb('basic', house = table('house', id = table.integer, guests = table.list)) \
 #     .objects.house(id = 0, guests = [0]).sync()
```

### Comparing `stuphos-2.0.8/stuphos/etc/tools/__init__.py` & `stuphos-2.0.9/stuphos/etc/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/cmdln.py` & `stuphos-2.0.9/stuphos/etc/tools/cmdln.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/collections_hack.py` & `stuphos-2.0.9/stuphos/etc/tools/collections_hack.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/debugging.py` & `stuphos-2.0.9/stuphos/etc/tools/debugging.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/errors.py` & `stuphos-2.0.9/stuphos/etc/tools/errors.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/internet.py` & `stuphos-2.0.9/stuphos/etc/tools/internet.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/logs.py` & `stuphos-2.0.9/stuphos/etc/tools/logs.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/misc.py` & `stuphos-2.0.9/stuphos/etc/tools/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,29 +201,14 @@
             a = n
 
         try: setattr(submod, a, getattr(base, n))
         except AttributeError: pass
 
     return submod
 
-def isYesValue(value):
-    if value is True:
-        return True
-    if isinstance(value, str):
-        return value.lower() in ['yes', 'true', '1', 'on']
-
-    return bool(value)
-
-def isNoValue(value):
-    if value is False:
-        return True
-    if isinstance(value, str):
-        return value.lower() in ['no', 'false', '0', 'off']
-
-    return not bool(value)
 
 def xorString(s, k):
     if not k:
         return s
 
     def forever():
         o = list(map(ord, k))
```

### Comparing `stuphos-2.0.8/stuphos/etc/tools/pyg_colorizer.py` & `stuphos-2.0.9/stuphos/etc/tools/pyg_colorizer.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/strings.py` & `stuphos-2.0.9/stuphos/etc/tools/strings.py`

 * *Files 7% similar despite different names*

```diff
@@ -299,7 +299,24 @@
         return '\n'.join(function(*args, **kwd))
 
     return nl
 
 def indent(string, tab = '    ', level = 1):
     tab *= level
     return tab + ('\n' + tab).join(string.split('\n'))
+
+
+def isYesValue(value):
+    if value is True:
+        return True
+    if isinstance(value, str):
+        return value.lower() in ['yes', 'true', '1', 'on']
+
+    return bool(value)
+
+def isNoValue(value):
+    if value is False:
+        return True
+    if isinstance(value, str):
+        return value.lower() in ['no', 'false', '0', 'off']
+
+    return not bool(value)
```

### Comparing `stuphos-2.0.8/stuphos/etc/tools/timing.py` & `stuphos-2.0.9/stuphos/etc/tools/timing.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/etc/tools/urls.py` & `stuphos-2.0.9/stuphos/etc/tools/urls.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/kernel/__init__.py` & `stuphos-2.0.9/stuphos/kernel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 
 
 	from ph.emulation.machine.heartbeat import Heartbeat
 
 	from ph.emulation.operation.application import Processor
 	from ph.emulation.operation.application import Subroutine
 	from ph.emulation.operation.application import Generator
+	from ph.emulation.operation.application import FastLocals
 
 
 	try: from ph.emulation.machine.parallel import pool
 	except ImportError: pass
 
 
 from ph.emulation.security import RelationNetwork
```

### Comparing `stuphos-2.0.8/stuphos/language/__init__.py` & `stuphos-2.0.9/stuphos/language/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/board/__init__.py` & `stuphos-2.0.9/stuphos/language/board/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/board/comm.py` & `stuphos-2.0.9/stuphos/language/board/comm.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/board/specproc.py` & `stuphos-2.0.9/stuphos/language/board/specproc.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/document/interface.py` & `stuphos-2.0.9/stuphos/language/document/interface.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/document/structural.py` & `stuphos-2.0.9/stuphos/language/document/structural.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,16 +242,16 @@
 #    name[type(arg1, arg2, kwd1 = value)]
 #    name[type(tags, for, this, type)]
 #
 
 # $ -> %?
 # name(type$sub@param=value@param=value)
 TYPE_PATTERN = r'^([^()]*)' + \
-               r'(?:\(([^()]*)' + \
-               r'(?:\$([^()]*))\))$'
+               r'(?:\(([^$()]*)' + \
+               r'(?:\$?([^()]*))\))$'
 
 TYPE_PATTERN = re.compile(TYPE_PATTERN)
 TYPE_PATTERN_MATCH = TYPE_PATTERN.match
 
 def parseTypeDecl(decl):
     try: m = TYPE_PATTERN_MATCH(decl)
     except TypeError as e:
@@ -259,15 +259,22 @@
         #   XXX this may be because the YAML produced a numeral-typed key.
         raise TypeError('%s: %r' % (e.message, decl))
 
     if m is None:
         return (decl, '', '')
         raise SyntaxError(decl)
 
-    return m.groups()
+    (name, typeName, subtype) = m.groups()
+    if not subtype:
+        subtype = typeName
+        typeName = '' # default
+
+    return (name, typeName, subtype)
+
+    # return m.groups()
 
 # Todo: general tree visitation.
 # XXX This is kind of a mess because it should be all integrated into building/loading alog.
 def flatten(x, buildingClass = None):
     # Err, toplevel..
     if buildingClass is None:
         buildingClass = StructuredEncoding.ClassMap.Building
```

### Comparing `stuphos-2.0.8/stuphos/language/document/wrlc.py` & `stuphos-2.0.9/stuphos/language/document/wrlc.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/gen/__init__.py` & `stuphos-2.0.9/stuphos/language/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/gen/gs_indent_lexer.py` & `stuphos-2.0.9/stuphos/language/gen/gs_indent_lexer.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/query/__init__.py` & `stuphos-2.0.9/stuphos/language/query/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/query/ql2.py` & `stuphos-2.0.9/stuphos/language/query/ql2.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/shortate.py` & `stuphos-2.0.9/stuphos/language/shortate.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/language/xml/__init__.py` & `stuphos-2.0.9/stuphos/language/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/__init__.py` & `stuphos-2.0.9/stuphos/management/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     def loadEmbeddedWebserver(self, conf):
         from stuphos.runtime.architecture.api import LookupObject
         webServiceClass = LookupObject(self.section.get('webserver-object', 'stuphos.webserver.DjangoService'))
 
         try: webServiceClass.get(create = True) # CreateFacility(webServiceClass)
         except OSError as e:
             logOperation(f'[webserver] {e}')
+            # from stuphos import logException
+            # logException(traceback = True)
 
         # todo: catch error: [Errno 112] Address already in use
         # OSError: [Errno 98] Address already in use
 
 
     # Some lesser features.
     def loadSystemShell(self, conf):
```

### Comparing `stuphos-2.0.8/stuphos/management/authlock.py` & `stuphos-2.0.9/stuphos/management/authlock.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/__init__.py` & `stuphos-2.0.9/stuphos/management/command_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/base.py` & `stuphos-2.0.9/stuphos/management/command_messaging/base.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/deployment.py` & `stuphos-2.0.9/stuphos/management/command_messaging/deployment.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/python.py` & `stuphos-2.0.9/stuphos/management/command_messaging/python.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/resource.py` & `stuphos-2.0.9/stuphos/management/command_messaging/resource.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/shell.py` & `stuphos-2.0.9/stuphos/management/command_messaging/shell.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/command_messaging/subdaemon.py` & `stuphos-2.0.9/stuphos/management/command_messaging/subdaemon.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/config.py` & `stuphos-2.0.9/stuphos/management/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,19 @@
 from configparser import ConfigParser, DEFAULTSECT, NoOptionError, NoSectionError
 
 def loadConfig(filename, defaults = None):
     config = ConfigParser(defaults = defaults)
     config.read([filename])
     return Configuration(config, filename)
 
+def loadConfigFromString(string, defaults = None, name = None):
+    config = ConfigParser(defaults = defaults)
+    config.read_string(string, source = name)
+    return Configuration(config, name)
+
 class Configuration:
     class Section:
         def __init__(self, config, section = None, **vars):
             if section is not None and type(section) is not str:
                 raise TypeError(type(section).__name__)
 
             self.config = config
@@ -61,14 +66,18 @@
         def __repr__(self):
             return "<Section '%s:%s'>" % (self.config.filename, self.section)
 
         @property
         def data(self):
             return dict((n, self.get(n)) for n in self.options())
 
+        def setOption(self, name, value):
+            return self.config._config.set(self.section, name, value)
+
+
     class _addressor:
         # todo: rewrite this with attributable.
         class _section:
             def __init__(self, addressor, name):
                 self._addressor = addressor
                 self._section = name
 
@@ -118,14 +127,34 @@
         return "<Configuration '%s'>" % self.filename
 
     @property
     def addressor(self):
         return self._addressor(self)
 
 
+    def loadSetOption(self, options):
+        for opt in options:
+            (section, name, value) = self.parseSetOption(opt)
+            if section and name and value:
+                self.getSection(section).setOption(name, value)
+
+    def parseSetOption(self, opt):
+        try: (name, value) = opt.split('=', maxsplit = 1)
+        except ValueError as e:
+            raise ValueError(opt) from e
+
+        try: (section, name) = name.split(':', maxsplit = 1)
+        except ValueError as e:
+            raise ValueError(name) from e
+
+        yield section
+        yield name
+        yield value
+
+
 # Package Support.
 class PackageManager:
     def __init__(self, site_path = None, *components):
         if site_path is None:
             raise ValueError('Unsupported Site Path')
 
         self.site_path = site_path
```

### Comparing `stuphos-2.0.8/stuphos/management/deploy.py` & `stuphos-2.0.9/stuphos/management/deploy.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/idling.py` & `stuphos-2.0.9/stuphos/management/idling.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/naming.py` & `stuphos-2.0.9/stuphos/management/naming.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/packaging.py` & `stuphos-2.0.9/stuphos/management/packaging.py`

 * *Files 15% similar despite different names*

```diff
@@ -313,20 +313,53 @@
         print('addmodule ' + str(args))
     def addStructure(self, *args, **kwd):
         print('addstructure ' + str(args))
     def addMedia(self, *args, **kwd):
         print('addmedia ' + str(args))
 
 
-def packageUnpackTo(structure, dest_dir, mount_point = None):
+class fsUnpackCore(fsPackageCore):
+    def getLocalPath(self, path, name, ensure = False):
+        nparts = len(self.path.parts)
+        local = self.path
+        for p in path.split('/') + [name]:
+            local = local(p)
+            if len(local.parts) < nparts:
+                raise ValueError(f'{path}/{name}')
+
+        if ensure:
+            local.folder.ensure()
+
+        return local
+
+    def addFolder(self, path, name):
+        # print('folder', self.getLocalPath(path, name, ensure = False))
+        self.getLocalPath(path, name, ensure = False).ensure()
+
+    def addModule(self, path, name, content):
+        # print('module', self.getLocalPath(path, name, ensure = True))
+        self.getLocalPath(path, name, ensure = True).write(content)
+
+    def addStructure(self, path, name, content, content_type = None):
+        # print('structure', self.getLocalPath(f'{path}/interfaces', name, ensure = True))
+        self.getLocalPath(f'{path}/interfaces', name, ensure = True) \
+            .write(content)
+
+    def addMedia(self, path, name, content, content_type = None):
+        # print('media', self.getLocalPath(f'{path}/media', name, ensure = True))
+        self.getLocalPath(f'{path}/media', name, ensure = True) \
+            .write(content)
+
+
+def packageUnpackTo(structure, dest_dir, mount_point = None, fsUnpackClass = fsPackageCore):
     if isinstance(structure, str):
         from stuphos.language.document.interface import document
         structure = document(structure)
 
-    core = fsPackageCore(dest_dir)
+    core = fsUnpackClass(dest_dir)
     uploadStructure(core, mount_point or '', structure)
 
 def packageStreamUnpackTo(input, output, mount_point = None):
     '''
     --admin-script=ph.interpreter.mental.library.extensions.packageStreamUnpackTo \
     -x bin.package -x bin
 
@@ -396,14 +429,62 @@
 
         if cmd == 'upload':
             return p.upload(rest)
         elif cmd == 'package':
             return p.package(rest)
 
 
+def restricted(self, *args):
+    r = self
+
+    for a in args:
+        if isinstance(a, str) and not isinstance(a, io.path):
+            a = io.path(a)
+
+        for p in a.parts:
+            if p == '..':
+                if len(r) > len(self):
+                    r = r.folder
+
+            elif p != '.':
+                r = r(p)
+
+    return r
+
+ContentIsFolder = object()
+
+from collections import namedtuple
+
+updateFSOpTuple = namedtuple('UpdateFSOp', 'base path content type')
+updateFSTypeTuple = namedtuple('UpdateFSType', 'name commit')
+
+def updateFSTree(base, files):
+    base = io.path(base)
+    for (name, content) in files:
+        path = restricted(base, name)
+
+        if content is ContentIsFolder:
+            def op(base, path, content):
+                def buildFolder():
+                    path.ensure()
+
+                return ('folder', buildFolder)
+
+        else:
+            def op(base, path, content):
+                def writeFileContent():
+                    path.ensure(folder_only = True)
+                    path.write(content)
+
+                return ('file', writeFileContent)
+
+        yield updateFSOpTuple(base, path, content, \
+               updateFSTypeTuple(*op(base, path, content)))
+
+
 # @apply
 # class defaultIgnore:
 #     def __contains__(self, object):
 #         return object in ['.git']
 
 defaultIgnore = ['.git']
```

### Comparing `stuphos-2.0.8/stuphos/management/reboot.py` & `stuphos-2.0.9/stuphos/management/reboot.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/services.py` & `stuphos-2.0.9/stuphos/management/services.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/shell.py` & `stuphos-2.0.9/stuphos/management/shell.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/subdaemon.py` & `stuphos-2.0.9/stuphos/management/subdaemon.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/syslog.py` & `stuphos-2.0.9/stuphos/management/syslog.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 unifying them within the mud whole.
 
 ---
 Implementation:
         
 """
 
-from stuphos.etc.tools.strings import compactify
+from stuphos.etc.tools.strings import compactify, safeAttr
 from stuphos.runtime.architecture.api import NoAccessException
 
 import re, errno, pickle, traceback,pprint
 from os import popen
 
 try: import readline as rl
 except ImportError: rl = None
@@ -914,14 +914,16 @@
                     return True
             else:
                 def hasAccess(source):
                     if isinstance(source, str):
                         return True
 
                     # Otherwise, it's a CodeSource.
+
+                    # checkAccess may be None.
                     return agentCore.principalHasAccess \
                         (checkAccess, list(source), 'read')
 
 
         for (f, pos) in self.iterateTracebackData(traceback):
             p = f.procedure
 
@@ -1055,37 +1057,44 @@
                 source = None
 
             if source is not None:
                 (lnr, source, code) = source
                 if hasAccess(source):
                     r = dict(sourceFormatted = formatSource(source),
                              source = source, lineNr = lnr, name = name,
+                             sourceAttr = safeAttr(str(source)),
+                             nameAttr = safeAttr(str(name)),
                              position = pos)
 
                     if code:
                         r['code'] = code
 
                     yield r
 
                 else:
                     yield dict(sourceFormatted = formatSource(source),
-                               source = source, name = name)
+                               source = source, name = name,
+                               sourceAttr = safeAttr(str(source)),
+                               nameAttr = safeAttr(str(name)))
 
             else:
                 try: source = p.getSourceMap().source
                 except AttributeError: source = None
 
                 r = dict()
 
                 if source:
                     r['sourceFormatted'] = formatSource(source)
                     r['source'] = source
                     r['name'] = name
                     r['position'] = name
 
+                    r['sourceAttr'] = safeAttr(str(source))
+                    r['nameAttr'] = safeAttr(str(name))
+
                 try: (start, g) = p.lineGroup(pos)
                 except (TypeError, AttributeError):
                     # No line source info found -- render one instruction string.
                     try: s = p.instructionsString(pos-1, pos, suppress_name = True)
                     except AttributeError:
                         s = '<unknown procedure>'
                 else:
```

### Comparing `stuphos-2.0.8/stuphos/management/tracking.py` & `stuphos-2.0.9/stuphos/management/tracking.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/management/tracsite.py` & `stuphos-2.0.9/stuphos/management/tracsite.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/pentacle/__init__.py` & `stuphos-2.0.9/stuphos/pentacle/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/pentacle/management.py` & `stuphos-2.0.9/stuphos/pentacle/management.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/pentacle/native.py` & `stuphos-2.0.9/stuphos/pentacle/native.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/pentacle/oob.py` & `stuphos-2.0.9/stuphos/pentacle/oob.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/pentacle/service.py` & `stuphos-2.0.9/stuphos/pentacle/service.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/phClient/__init__.py` & `stuphos-2.0.9/stuphos/phClient/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/__init__.py` & `stuphos-2.0.9/stuphos/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/architecture/__init__.py` & `stuphos-2.0.9/stuphos/runtime/architecture/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -696,15 +696,17 @@
     # Do not dereference ._object when passing/returning.
     pass
 
 _transparent = Transparent
 _translucent = Translucent
 
 class ExceptionType(Translucent):
-    pass
+    @classmethod
+    def _fromMessage(self, message):
+        return self._object(message)
 
 class baseExceptionValue(Translucent):
     _type = None
 
     def __init__(self, value, type = None):
         Translucent.__init__(self, value)
         if type is not None:
@@ -733,23 +735,29 @@
             t = self._type
             if t is not None:
                 if name in getattr(t, '_methods', []):
                     m = getattr(t, name)
                     return lambda *args, **kwd: \
                         m(self._object, *args, **kwd)
 
+            # print(f'[evalue$attr] {t}: {self}: {name}')
+            # debugOn()
+
             raise e
 
 
 class safeNative(writeprotected):
+    # XXX Not pickle-friendly.
     def __init__(self, callable, name = None):
         # self.__call__ = callable
         self._callable = callable
         self._name = name
+
     def __call__(self, *args, **kwd):
+        # XXX This isn't (?) called because __getattr__ intercepts it.
         return self.__dict__['_callable'](*args, **kwd)
 
     def __getattr__(self, name):
         return getattr(self.__dict__['_callable'], name)
 
     # I don't know why I resort to this translation.  What am I hiding?
     # def __getattr__(self, name):
@@ -866,17 +874,19 @@
 BypassReturn = Continuation
 
 class YieldFrame(OuterFrame):
     pass
 
 
 class Interrupt(InterpreterState):
-    pass
+    _uncatchable = True
 class Timeout(Interrupt):
-    pass
+    _uncatchable = False
+class TimeoutQuotaExceeded(Timeout):
+    _uncatchable = True
 
 
 class Interface(writeprotected, Object):
     # Revealed to the GIRL object runtime, proxies the local subroutine def
     # through the vm invocation instruction.
     class _Meta(Object._Meta):
         Attributes = [('procedure', lambda i: repr(i._procedure))]
```

### Comparing `stuphos-2.0.8/stuphos/runtime/architecture/api.py` & `stuphos-2.0.9/stuphos/runtime/architecture/api.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/architecture/lookup/__init__.py` & `stuphos-2.0.9/stuphos/runtime/architecture/lookup/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/architecture/routines.py` & `stuphos-2.0.9/stuphos/runtime/architecture/routines.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/architecture/spatial.py` & `stuphos-2.0.9/stuphos/runtime/architecture/spatial.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/core/__init__.py` & `stuphos-2.0.9/stuphos/runtime/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,19 +101,25 @@
     return getRegistryObject(CONFIG_OBJECT_NAME,
                              create = _createMUDConfig)
 
 def deleteConfig():
     # del runtime[mudConfig]
     return deleteRegistryObject(CONFIG_OBJECT_NAME)
 
-def reloadConfigFile(filename):
+def reloadConfigFile(filename, setOptions = False):
     global CONFIG_FILE
     CONFIG_FILE = filename
     deleteConfig()
 
+    # debugOn()
+    if setOptions is not False:
+        # Load immediately and override with core cmdline opts.
+        getConfigObject().loadSetOption(setOptions)
+
+
 def getConfig(name, section = 'MUD'):
     try: return getConfigObject().get(name, section = section)
     except RegistryNotInstalled: pass
 def getSection(section = 'MUD'):
     try: return getConfigObject().getSection(section)
     except RegistryNotInstalled: pass
 
@@ -370,34 +376,41 @@
     installCommands()
 
 
 def installSystemConfig():
     from os import getenv
     config = getenv('STUPHOS_CONFIG')
     if config:
-        reloadConfigFile(config)
+        # Load --set-option from command line for initial config.
+        reloadConfigFile(config, setOptions = core.cmdln['options'].set_option)
 
 
 # Event Bridge.
-def bootStart():
+def bootStart(configFile, setOptions):
     # Note: this function must return the bridge, or
     # the rest of the extension is not installed.
 
     # todo: import more of management
     # import mud.tools.debug
 
 
+    # Least configurable:
     installSystemConfig()
 
     bridge = installBridge()
 
+
     from stuphos.runtime.registry import getRegistry
     thisModule = getMudModule()
     getRegistry(create = thisModule.on) # Binding passed for shutdown-game registration.
 
+    if configFile:
+        # Note: this is necessary in order to activate 'configuration' builtin.
+        reloadConfigFile(configFile, setOptions = setOptions)
+
 
     installSite()
 
 
     try:
         installServices(thisModule)
         installWorld()
```

### Comparing `stuphos-2.0.8/stuphos/runtime/events.py` & `stuphos-2.0.9/stuphos/runtime/events.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/facilities.py` & `stuphos-2.0.9/stuphos/runtime/facilities.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/misc.py` & `stuphos-2.0.9/stuphos/runtime/misc.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/plugins.py` & `stuphos-2.0.9/stuphos/runtime/plugins.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/registry.py` & `stuphos-2.0.9/stuphos/runtime/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,26 @@
                if name.startswith('_') \
                   else Access.Node(None, name, self._callCreate)
 
     def __getitem__(self, node):
         if isinstance(node, self.Node):
             node = node._buildName()
 
-        assert isinstance(node, str)
+        if not isinstance(node, str):
+            raise ValueError(node)
+
         return getObject(node)
 
     def __delitem__(self, node):
         if isinstance(node, self.Node):
             node = node._buildName()
 
-        assert isinstance(node, str)
+        if not isinstance(node, str):
+            raise ValueError(node)
+
         return delObject(node)
 
     def _callCreate(self, node, create = None, *args, **kwd):
         return getObject(node._buildName(),
                          create = lambda:create(*args, **kwd))
 
     def _doesNotExistError(self, name):
```

### Comparing `stuphos-2.0.8/stuphos/runtime/sandbox.py` & `stuphos-2.0.9/stuphos/runtime/sandbox.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/runtime/support.py` & `stuphos-2.0.9/stuphos/runtime/support.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/structure.py` & `stuphos-2.0.9/stuphos/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 
 # XXX :skip: upgrade this to use lang.document.structural
 # from op.runtime.structural.document import Submapping, Core
 from stuphos.language.document.structural import Submapping, Core
 
 from stuphos.runtime import Object
 from stuphos.runtime.architecture.api import writeprotected, extension, NoAccessException
-from stuphos.etc.tools.strings import renderTemplate
+from stuphos.etc.tools.strings import renderTemplate # This can also come from rt.arch.api
 from stuphos.etc.tools.logs import tracebackString, exceptionHeader
 from stuphos.etc.tools import isYesValue
 from stuphos.kernel import Subroutine, grammar, Girl, Script, executeGirl, newModuleTask
 from stuphos.kernel import vmNewMapping, AutoMemoryMapping, AutoMemorySequence, Processor
 from stuphos.kernel import vmNewSequence, vmCurrentTask, BypassReturn, MemorySequence
 from stuphos.kernel import MemoryMapping, Instance, protectedMemoryLoad
-from stuphos.kernel import constrainStructureMemory, TaskCreation
+from stuphos.kernel import constrainStructureMemory, TaskCreation, findUserByName
+
 from stuphos import getConfig
 
 from queue import Queue
 import json, re
 
 
 class MarshalizedObject(writeprotected, extension):
@@ -65,33 +66,30 @@
 
     @onComplete
     def complete(_, exception = None, **kwd):
         # print(f'[TriggerTask.result.complete] e: {exception}')
 
         if exception:
             (etype, value, tb) = exception
-
-            c.errorState = True # Signal error state while bypassing Uncaught.
             s.resumeTask(c, c.machine, exception = value)
 
-            return True # Error handled: passed to outcome-receiver.
-
         else:
             # try: value = task.stack.pop()[0]
             try: value = task.stack[-1]
             except IndexError: value = None
 
             value = convertTaskValue(c, value)
             s.resumeTask(c, c.machine, value = value)
 
     raise BypassReturn
 
 def getPrimaryIdentity(user):
-    for default in user.default_players.all():
-        return default.player.player_name
+    if user.is_authenticated:
+        for default in user.default_players.all():
+            return default.player.player_name
 
 
 class Emulation(Script):
     # todo: override exception-handling, storing exception on task.
     # Then, read flag on (rendering) task completion handler
     # to know what to do (push q reponse) with it.
 
@@ -132,14 +130,19 @@
     def createTask(self, environ):
         return self.taskClass.Load(environ = environ, user = self.user)
 
     def preInitTask(self, task, *args, **kwd):
         # debugOn()
         if self.audit in ['debug', 'trace', 'stack']:
             if self.operator is not None:
+                # This sends stylized html traces to the session, but since
+                # we don't have a peer object, only operator name, we need
+                # to interface with debugInstructionPeer at an operator level.
+                # self.tracing = self.debugInstructionPeer(self.peer)
+
                 task.tracing = task.debugInstructionOperator # (self.operator)
                 task.debugStack = self.audit == 'stack'
                 task.operator = self.operator
 
         elif self.audit is True:
             task.tracing = task.__class__.auditInstruction
 
@@ -275,14 +278,15 @@
             raise ValueError(f'Must be > 0 and <= {self.TIMEOUT_MAX}')
 
 
     def _activate(self, procedure, *args, **kwd):
         # Operate TaskCreation API now.
         environ = kwd.pop('environ', dict())
         locals = kwd.pop('locals', None)
+        forceLocals = kwd.pop('forceLocals', None)
         progr = kwd.pop('programmer', None)
         user = kwd.pop('user', None)
 
         operator = kwd.pop('operator', None)
         audit = kwd.pop('audit', None)
         trace = kwd.pop('trace', None)
         account = kwd.pop('account', None)
@@ -302,15 +306,16 @@
 
         create = dict(taskClass = Emulation, environ = environ,
                       operator = operator, audit = audit, trace = trace,
                       account = account, traceback = traceback,
                       initialize = init, name = name, timeout = timeout,
                       finishingScript = finishingScript,
                       programmer = progr, user = user,
-                      procedure = procedure, locals = locals)
+                      procedure = procedure, locals = locals,
+                      forceLocals = forceLocals)
 
         task = EmulatedCodeTaskCreation.Create(self, **create)
 
         return self._TaskClass(task, procedure)
 
 
     def _activateInline(self, procedure, *args, **kwd):
@@ -439,14 +444,16 @@
 
         return self._activate(*args, **kwd)
 
     def call(self, *args, **kwd): # spawn
         progr = vmCurrentTask().findProgrammer()
         return self._activate(self._module, *args,
                               **dict(environ = kwd,
+                                     user = None if progr is None else \
+                                        findUserByName(progr.principal),
                                      programmer = progr))
 
     def callForResult(self, *args, **kwd):
         return self.call(*args, **kwd).result()
     __call__ = callForResult
 
 
@@ -483,15 +490,15 @@
 inline = Inline._Build
 
 class View(writeprotected, Object):
     def register(self): # What is this used for?
         raise NotImplementedError
     def _render(self, request = None):
         raise NotImplementedError
-    def _debugging(self, task, etype, value, tb, traceback): # *args, **kwd
+    def _debugging(self, request, task, etype, value, tb, traceback): # *args, **kwd
         # Specifically, there was a bug during execution of the context trigger,
         # so this is a good place to generate a report page with task traceback.
 
         raise etype(value).with_traceback(tb) # there was a python bug
 
 
 class NodePath(writeprotected, list):
@@ -524,15 +531,15 @@
     @property
     def string(self):
         return '/'.join(self)
 
 # @runtime.available(runtime.System.Journal)
 # def debugging(log, self, etype, value, tb):
 
-def debugging500(self, task, etype, value, tb, traceback):
+def debugging500(self, request, task, etype, value, tb, traceback):
     # import pdb; pdb.set_trace()
 
     # todo: generate html-ready (FO) tracebacks
 
     if isinstance(value, Processor.UncaughtError):
         etype = value.etype
         tb = value.tb
@@ -547,15 +554,16 @@
         # to the initiator (and the programmer) the things that we need
         # to.  If the site debug page is disabled, then the initiator
         # will basicaly get a 'didn't work' message.
 
         raise value.with_traceback(tb)
 
     if self.debug and traceback:
-        vtb = '\n'.join(task._task.formatTraceback(traceback))
+        primaryIdentity = getPrimaryIdentity(request.user)
+        vtb = '\n'.join(task._task.formatTraceback(traceback, checkAccess = primaryIdentity))
     else:
         vtb = ''
 
 
     if isYesValue(getConfig('native-traceback', 'Interpreter')):
         # But we're mostly interested in python exception.
         tb = '%s:\n%s\n' % (exceptionHeader(etype, value),
@@ -584,15 +592,15 @@
     class _Meta(Object._Meta):
         Attributes = ['_path']
 
     __repr__ = Object.__repr__
 
     DEFAULT_TIMEOUT = None
 
-    def __init__(self, template, context, environment = None,
+    def __init__(self, template, context: Trigger, environment = None,
                  source = None, debug = False, path = '',
                  timeout = None, security = None):
 
         self._template = template
         self.context = context
         self.environment = environment
         self.source = source
@@ -660,14 +668,58 @@
                 return g
 
         @property
         def userAgent(self):
             return self._request.META['HTTP_USER_AGENT']
 
 
+        @property
+        def user(self):
+            return self._User(self._request.user, request = self._request)
+
+        @property
+        def session(self):
+            return # :security:
+            return self._request.session
+
+        @property
+        def body(self):
+            return self._request.body
+
+        # provide access to persistant storage.
+
+
+        def _sessionKey(self, name, task = None):
+            if task is None:
+                task = vmCurrentTask()
+
+            identity = task.findProgrammer()
+            if identity is not None:
+                identity = identity.principal
+
+            return f'stuphos$request:{identity or ""}:{name}'
+
+        def sessionGet(self, name):
+            task = vmCurrentTask()
+            return protectedMemoryLoad(task, self._request.session \
+                [self._sessionKey(name, task)])
+
+            # return protectedMemoryLoad(vmCurrentTask(), self._request.session \
+            #     ['stuphos$request:' + name])
+
+        def _sessionSet(self, name, value):
+            # self._request.session['stuphos$request:' + name] = str.__str__(value)
+            self._request.session[self._sessionKey(name)] = str.__str__(value)
+
+        def _sessionClear(self, *names):
+            for n in names:
+                try: del self._request.session[self._sessionKey(n)]
+                except KeyError: pass
+
+
         class _User(writeprotected, Object):
             def __init__(self, user, request = None):
                 self._user = user
                 self._request = request
 
             def __repr__(self):
                 if self._user is None:
@@ -695,27 +747,30 @@
             @property
             def primaryIdentity(self):
                 # User (Adapter) objects are passed to code running with other user permissions,
                 # so we hide this.  For now, only current programmers can access their primary
                 # identity.
                 from stuphos.kernel import vmCurrentTask
                 name = self._primaryIdentity
-                lowerName = name.lower()
+                if name is not None:
+                    lowerName = name.lower()
 
-                progr = vmCurrentTask().findProgrammer()
-                if progr is not None:
-                    if progr.principal.lower() == lowerName:
-                        return name
+                    progr = vmCurrentTask().findProgrammer()
+                    if progr is not None:
+                        if progr.principal.lower() == lowerName:
+                            return name
 
             @property
             def securityContext(self):
                 # Note: requiring a login permission here complicates serving user-to-user
                 # views, but we can't assume that the requesting user wants to give all
                 # control to any other arbitrary user (besides the system) simply because
                 # they're viewing the resource.  What is needed is user-specified ACL.
+                # debugOn()
+
                 from stuphos.kernel import securityContext, Programmer, vmCurrentTask
                 principal = self._primaryIdentity
 
                 try: vmCurrentTask().checkAccess(['system:user:context', principal], 'impersonate')
                 except NoAccessException as e:
                     print(f'[http$request$user$context] {e}')
                     return
@@ -735,45 +790,31 @@
 
                 if core is not None and core.principalHasAccess(principal, resource, op):
                     return True
 
                 raise NoAccessException(Programmer(principal), resource, op)
 
 
-        @property
-        def user(self):
-            return self._User(self._request.user, request = self._request)
-
-        @property
-        def session(self):
-            return # :security:
-            return self._request.session
-
-        @property
-        def body(self):
-            return self._request.body
-
-        # provide access to persistant storage.
-
     def _securityCheck(self, core, progr, subresource):
         sec = self.security
 
         if sec in ['allow', 'allow all', 'allow-all']:
             return True
 
         def checkAccess(path):
             # We have to manually build the check because the task
             # has no programmer frames (security context) yet.
             if isinstance(path, str):
                 path = path.split('/')
 
             if core is not None:
-                if progr is not None:
-                    if core.principalHasAccess(progr.principal.lower(), path, 'read'):
-                        return True
+                if core.principalHasAccess(None if progr is None else
+                                           progr.principal.lower(),
+                                           path, 'read'):
+                    return True
 
             raise NoAccessException(progr if progr is None else progr.principal.lower(),
                                     path, 'read')
 
         if sec in [None, 'default', 'path']:
             if self.context:
                 return checkAccess(self.context._path + self._path) # + subresource
@@ -785,26 +826,32 @@
 
         #     return checkAccess(path)
 
         raise NotImplementedError(f'view.security = {sec}')
 
     def _render(self, request = None, response = None, account = None,
                 path = None, requestAdapter = None, programmer = None,
-                query = None, core = None, context = None):
+                query = None, core = None, context = None, initiatingUser = None):
 
-        from stuphos.kernel import EmptyStackError
         from phsite.network.adapter.commands import CoreRequest
         from world import heartbeat as vm # XXX Todo: runtime.System.Engine
 
-        if isinstance(request, CoreRequest):
-            user = request._user
-        elif request is not None:
-            user = request.user
+        # Use initiatingUser if set, otherwise use programmer user or request.user
+        # if that's not set.
+        if initiatingUser is None:
+            # Note: this user setting will be overridden below if programmer is set.
+            if isinstance(request, CoreRequest):
+                user = request._user
+            elif request is not None:
+                # Common external page requests (unless interface owner is specified).
+                user = request.user
+            else:
+                user = None
         else:
-            user = None
+            user = initiatingUser
 
         progr = programmer
         # debugOn()
         # If progr.principal is '', then the interface doesn't have an owner.
         if programmer is None:
             # from phsite.network.models import DefaultPlayer
             from phsite.network.embedded.olc import WebProgrammer
@@ -818,14 +865,20 @@
             # debugOn()
     
             if user is not None and user.is_authenticated:
                 for d in user.default_players.all():
                     progr = WebProgrammer(d.player.player_name)
                     break
 
+        elif initiatingUser is None:
+            # Use interface owner.
+            from stuphos.kernel import findUserByName
+            user = findUserByName(programmer.principal)
+
+
         # Raises NoAccessException.
         self._securityCheck(core, progr, path)
 
         if self.debug in ['debug', 'trace', 'stack']:
             audit = str.__str__(self.debug)
         else: # what if self.debug is True?
             audit = None
@@ -853,44 +906,71 @@
             else:
                 requestAdapter = self._RequestAdapter(request, query = query)
 
         locals = dict(request = requestAdapter)
 
         # locals['source'] = self.source
 
-        protected = None # [None]
+        protected = None
+        protectedCont = [None]
         environ = None
+        outputLocals = [None]
 
         def initializeTask(task):
-            o = task.frame.locals
+            nonlocal protected, environ
+            outputLocals[0] = o = task.frame.locals
 
             # Convert source document into memory-safe structure.
             # Note: this is actually an (opaqued) containerAccessor.
             e = constrainStructureMemory(task, self.environment)
             o['environment'] = e
             o['container'] = e
 
             # Store memory-safe mapping for response local.
             # p = protected[0] = task.memory.Mapping(task.memory, **response)
             # task.frame.locals['response'] = p
 
-            nonlocal protected, environ
             with vm.threadContext(task = task):
-                protected = task.memory.Mapping(task.memory, **response)
+                protected = protectedCont[0] = task.memory.Mapping(task.memory, **response)
                 o['response'] = protected
 
                 task.environ = environ = task.shared_mapping(*contextObject.items())
                 environ['context'] = environ
                 environ['view'] = task.sequence(self.path)
 
                 if isinstance(path, NodePath) or path is None:
                     o['path'] = path
                 else:
                     o['path'] = task.sequence(path)
 
+
+        task = (isYesValue(configuration.AgentSystem.superior_enabled) and \
+                self._activateContextSuperior or self._activateContext) \
+            (vm, q, response, protectedCont, context,
+             path, locals, progr,
+             user, initializeTask,
+             audit, report, account,
+             outputLocals)
+
+
+        (success, result) = q.get() # *
+        if success:
+            return result
+
+        # debugOn()
+        return self._debugging(request, task, *result) # response or raise
+
+
+    def _activateContext(self, vm, q, response, protectedCont, context,
+                         path, locals, progr,
+                         user, initializeTask,
+                         audit, report, account,
+                         outputLocals):
+
+        # debugOn()
         task = self.context._activate(self.context._module,
                                       name = f'view({path})',
                                       locals = locals,
                                       programmer = progr,
                                       traceback = report,
                                       account = account,
                                       initialize = initializeTask,
@@ -904,67 +984,164 @@
         def completeViewRequest(task, exception = None, traceback = None):
             # import game
             # game.syslog('view-request-context: %r' % ctxtdct)
 
             # print 'view-request-context: %r' % (exception,)
 
             if response is not None:
-                # response.update(protected[0])
-                response.update(protected)
+                response.update(protectedCont[0])
 
             if exception is not None:
                 # Introspect into the ph runtime with debugging view.
                 q.put((False, exception + (traceback,)))
             else:
+                try: result = self._completeView_render(vm, task, outputLocals)
+                except:
+                    from sys import exc_info
+                    q.put((False, exc_info() + (traceback,)))
+                else:
+                    q.put((True, result))
+
+        return task
+
+    _activateContextServe = _activateContext
+
+
+    def _completeView_render(self, vm, task, outputLocals):
+        from stuphos.kernel import EmptyStackError
+
+        try: responseValue = task.stack.pop()[0]
+        except EmptyStackError:
+            # Treat like returning None, for now.
+            responseValue = None
+
+        if isinstance(responseValue, (str, bytes)):
+            return dict(content = responseValue)
+        elif isinstance(responseValue, dict):
+            return responseValue
+        elif responseValue is not None: # and responseValue != (None,):
+            raise TypeError(type(responseValue))
+        else:
+            # By default, this requires a permission because django templates are
+            # unsafe.  When that situation is remedied, grant to group:public.
+            # debugOn()
+            task.checkAccess(['system:network:template', 'django'], 'render',
+                             publicAccess = True)
+
+            # Re-acquire unicode/basestring type for renderTemplate call.
+
+            with vm.threadContext(task = task):
+                # environ might be a MemoryMapping which generates a
+                # memory.sequence when its items method is called.
+                items = task.environ.items()
+
                 # debugOn()
+                try: context = dict.__getitem__(outputLocals[0], 'context')
+                except KeyError:
+                    context = dict()
 
-                try:
-                    try: responseValue = task.stack.pop()[0]
-                    except EmptyStackError:
-                        # Treat like returning None, for now.
-                        responseValue = None
-
-                    if isinstance(responseValue, (str, bytes)):
-                        q.put((True, dict(content = responseValue)))
-                    elif isinstance(responseValue, dict):
-                        q.put((True, responseValue))
-                    elif responseValue is not None: # and responseValue != (None,):
-                        raise TypeError(type(responseValue))
-                    else:
-                        # Re-acquire unicode/basestring type for renderTemplate call.
+                # for (key, value) in context.items():
+                #     if isinstance(value, str):
+                #         context[key] = str.__str__(value)
+
+            for (key, value) in items:
+                if isinstance(key, bytes):
+                    # del ctxtdct[key] # The bytes key.
+                    context[key.decode('ascii')] = value
+                else:
+                    context[key] = value
 
-                        with vm.threadContext(task = task):
-                            # environ might be a MemoryMapping which generates a
-                            # memory.sequence when its items method is called.
-                            items = environ.items()
-
-                        for (key, value) in items:
-                            if isinstance(key, bytes):
-                                # del ctxtdct[key] # The bytes key.
-                                context[key.decode('ascii')] = value
-                            else:
-                                context[key] = value
-
-                        # todo: do as billable
-                        # debugOn()
-                        # from code import InteractiveConsole as    
-                        # IC(locals = dict(context = context,
-                        #                  environ = environ)).interact()
+            # todo: do as billable
+            # debugOn()
+            # from code import InteractiveConsole as    
+            # IC(locals = dict(context = context,
+            #                  environ = environ)).interact()
 
-                        q.put((True, self.renderTemplate(**context)))
+            # debugOn()
+            return self.renderTemplate(**context)
 
-                except:
-                    from sys import exc_info
-                    q.put((False, exc_info() + (traceback,)))
 
-        (success, result) = q.get() # *
-        if success:
-            return result
+    def activateContextInferior(self, name, locals):
+        task = vmCurrentTask()
+        progr = task.findProgrammer()
+        user = task.user
+
+        task = self.context._activate(self.context._module,
+                                      name = str.__str__(name),
+                                      locals = locals,
+                                      programmer = progr,
+                                      # initialize = initializeTask,
+                                      user = user
+                                      )
 
-        return self._debugging(task, *result) # response or raise
+        @task._onComplete
+        def completeViewRequest(task, exception = None, traceback = None):
+            if not task.stack:
+                task.stack.push(None)
+
+        return task
+
+    def _activateContextSuperior \
+        (self, vm, q, response, protectedCont, context,
+         path, locals, progr,
+         user, initializeTask,
+         audit, report, account,
+         outputLocals):
+
+        page: EmulatedView
+
+        core = runtime[runtime.Agent.System]
+        if core is None:
+            raise RuntimeError('Agent System is not installed!')
+
+
+        try: page = core[configuration.AgentSystem.page_superior or 'www/superior/page']
+        except Exception as e:
+            # from stuphos import logException
+            # logException(traceback = True)
+
+            return self._activateContextServe \
+                (vm, q, response, protectedCont, context,
+                 path, locals, progr,
+                 user, initializeTask,
+                 audit, report, account,
+                 outputLocals)
+
+
+        '''
+        interfaces/www/superior::
+            page(view):
+                context(trigger)::
+                    ns = locals().copy()
+                    del$('view$client', ns)
+
+                    return view$client.activateContextInferior \
+                        ('view(%r)' % path, ns).result()
+
+        '''
+
+        localsClient = locals.copy()
+        localsClient['view$client'] = self
+
+        task = page._activateContextServe \
+                (vm, q, response, protectedCont, context,
+                 path, localsClient, progr,
+                 user, initializeTask,
+                 audit, report, account,
+                 outputLocals)
+
+        @task._onComplete
+        def updateContext(_, *error, **kwd):
+            # debugOn()
+            if 'context' in localsClient:
+                context.update(localsClient['context'])
+
+        return task
+
+    # _activateContext = _activateContextSuperior
 
 
     class _DeepView(NodePath):
         def __init__(self, view, path):
             NodePath.__init__(self, path)
             self._view = view
 
@@ -1046,31 +1223,38 @@
             if new in self:
                 # Recursion detected.
                 return True
 
             self.add(new)
 
     def _render(self, request = None, **kwd):
+        # XXX Fails to detect recursion.
         from ph.interpreter.mental.library.views import renderWM
 
         # Recursion control.
-        graph = kwd.pop('aliasGraph', None)
-        if graph is None:
-            graph = self._recursionGraph(self.path)
+        receivingContext = kwd.pop('context', None) # Providing clean initial graph point.
+
+        if isinstance(receivingContext, dict):
+            recursion = receivingContext.pop('aliasGraph', None)
+            if recursion is None:
+                recursion = self._recursionGraph(self.path)
+            else:
+                if recursion(self.path):
+                    raise RecursionError('Alias recursion detected!')
+
+            ctx = dict(aliasGraph = recursion)
+
         else:
-            if graph(self.path):
-                raise RecursionError('Alias recursion detected!')
+            ctx = dict()
+
 
         kwd.pop('path', None) # Already passed as positional argument.
         kwd.pop('programmer', None) # Passed later as positional arg.
         kwd.pop('account', None) # Not permitted by renderView.
         kwd.pop('core', None) # Already passed as positional argument.
-        kwd.pop('context', None) # Providing clean initial graph point.
-
-        ctx = dict(aliasGraph = graph)
 
         # request.path = self.path
 
         # debugOn()
 
         path = self.path
 
@@ -1327,17 +1511,24 @@
 
         return value
 
     def __getattr__(self, name):
         try: return object.__getattribute__(self, name)
         except AttributeError as e:
             try: return self[name]
-            except KeyError:
+            except (KeyError, TypeError):
                 raise e
 
+    def __iter__(self):
+        # debugOn()
+        if isinstance(self._object, (list, tuple)):
+            return iter(self._object)
+        elif isinstance(self._object, dict):
+            return iter(self._object.items())
+
 
 class Factory(Submapping):
     from .db.vardb import db, table
 
     def trigger(self, name, value, **kwd):
         from stuphos.language.document.interface import getContextEnvironment
 
@@ -1354,15 +1545,15 @@
         # debugOn()
         env = containerAccessor(kwd['container'])
 
         # For relative dotlevel path lookups.
         path = getContextEnvironment('document', default = None)
         return Trigger(code, synchronous, env, path = path)
 
-    task = let = evaluation = code = box = trigger
+    task = let = evaluation = code = trigger
 
     def emulation(self, name, value, **kwd):
         return None
 
         # Todo: Pass a procedure/module and emulate a buffered version of those instructions.
         if isinstance(value, grammar.Node):
             pass # validated, but compile todo
@@ -1834,14 +2025,15 @@
             return proc.setEnvironment(*args, **kwd)
 
 
         @property
         def _activation(self):
             from ph.emulation.operation.application import Invocation
             proc = self._module.getSubroutine(self._name)
+            # debugOn()
             return Invocation(proc.main_program, proc.name, proc.start_position)
 
         def __repr__(self):
             return f'<method$interface {repr(self._name)}>'
 
 
     def method(self, name, value, **kwd):
@@ -1850,22 +2042,27 @@
         # something to mark it and get passed to the class constructor,
         # but, a method definition really has no use alone.
         module = buildMethodFromStructure(name, value, **kwd)
 
         # print('[structure.method]')
         # print(indent(module))
 
-        from stuphos.kernel import Girl
+        from stuphos.kernel import Girl, FastLocals
         module = Girl(Girl.Module, module)
 
+        env = dict(container = containerAccessor(kwd['container']))
+
         try: task = vmCurrentTask()
         except AttributeError:
             task = None
 
-        env = dict(container = containerAccessor(kwd['container']))
+        else:
+            env = FastLocals(task.memory, env, module._variableNames,
+                             module._variableIndices)
+            # print(f'[method$locals] {id(env)}')
 
         # print(f'[method def] {", ".join(kwd.keys())}')
         from stuphos.language.document.interface import getContextEnvironment
 
         try: path = getContextEnvironment('document')
         except KeyError: pass
         else:
```

### Comparing `stuphos-2.0.8/stuphos/stuphlib/binary.py` & `stuphos-2.0.9/stuphos/stuphlib/binary.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/boards.py` & `stuphos-2.0.9/stuphos/stuphlib/boards.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/cherry.py` & `stuphos-2.0.9/stuphos/stuphlib/cherry.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/clanlib.py` & `stuphos-2.0.9/stuphos/stuphlib/clanlib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/constants.py` & `stuphos-2.0.9/stuphos/stuphlib/constants.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/dblib.py` & `stuphos-2.0.9/stuphos/stuphlib/dblib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/directory.py` & `stuphos-2.0.9/stuphos/stuphlib/directory.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/etc.py` & `stuphos-2.0.9/stuphos/stuphlib/etc.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/help.py` & `stuphos-2.0.9/stuphos/stuphlib/help.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/house.py` & `stuphos-2.0.9/stuphos/stuphlib/house.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/moblib.py` & `stuphos-2.0.9/stuphos/stuphlib/moblib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/objlib.py` & `stuphos-2.0.9/stuphos/stuphlib/objlib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/playerfile.py` & `stuphos-2.0.9/stuphos/stuphlib/playerfile.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/rent.py` & `stuphos-2.0.9/stuphos/stuphlib/rent.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/roomlib.py` & `stuphos-2.0.9/stuphos/stuphlib/roomlib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/searchlib.py` & `stuphos-2.0.9/stuphos/stuphlib/searchlib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/shplib.py` & `stuphos-2.0.9/stuphos/stuphlib/shplib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/sql/__init__.py` & `stuphos-2.0.9/stuphos/stuphlib/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/sql/item.py` & `stuphos-2.0.9/stuphos/stuphlib/sql/item.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/sql/zone.py` & `stuphos-2.0.9/stuphos/stuphlib/sql/zone.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/textlib.py` & `stuphos-2.0.9/stuphos/stuphlib/textlib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/wldlib.py` & `stuphos-2.0.9/stuphos/stuphlib/wldlib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/stuphlib/zonelib.py` & `stuphos-2.0.9/stuphos/stuphlib/zonelib.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/__init__.py` & `stuphos-2.0.9/stuphos/system/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/api.py` & `stuphos-2.0.9/stuphos/system/api.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/cli.py` & `stuphos-2.0.9/stuphos/system/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Compartmental Command-line Bootstrap Interface.
 from optparse import OptionParser
 import sys, os
 
+try: import pdb
+except ImportError: pass
+
 def parseCmdln(argv = None):
     parser = OptionParser()
 
     parser.add_option('-C', '--config-file', '--config', '--game-config')
     parser.add_option('-g', '--debug', action = 'count', default = 0)
     parser.add_option('-p', '--port', type = int)
     parser.add_option('-v', '--verbose', action = 'count', default = 0)
@@ -18,14 +21,15 @@
     parser.add_option('-n', '--no-world', action = 'store_true')
     parser.add_option('-W', '--cascade', '--load-world', action = 'store_true')
 
     parser.add_option('-i', '--interactive', action = 'store_true')
     parser.add_option('-a', '--asynchronous', '--async', action = 'store_true')
     parser.add_option('-m', '--mud-package', '--mud')
     parser.add_option('-e', '--service', action = 'append', default = [], dest = 'services')
+    parser.add_option('-S', '--set-option', action = 'append', default = [])
 
     parser.add_option('-s', '--supreme', action = 'store_true')
     parser.add_option('--enter-game', action = 'store_true')
 
     parser.add_option('--admin-name')
 
     # These are different than admin-name:
```

### Comparing `stuphos-2.0.8/stuphos/system/core.py` & `stuphos-2.0.9/stuphos/system/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,22 @@
         self.boot()
 
 # Application.
 def freeClient(network, port):
     print('Opening Loopback Connection:', port)
     network.openConnection(('localhost', port))
 
+def parseArgvToKwd(args):
+    kwd = dict()
+    for a in args:
+        (name, value) = a.split('=', 1)
+        kwd[name] = value
+
+    return kwd
+
 class Core(Heartbeat):
     class Pulse(Heartbeat.Task):
         # This could go in system.heartbeat
         from time import time as getTimeInSeconds, sleep
         getTimeInSeconds = staticmethod(getTimeInSeconds)
         sleep = staticmethod(sleep)
 
@@ -190,14 +198,16 @@
         if isYesValue(configuration.Interpreter.emhw): # or options.emhw:
             EnableEMHW()
 
         if not options.headless:
             def ehwm(console):
                 # Console might be None. (?)
                 if console is not None:
+                    console.state = 'Playing' # 'Shell'
+
                     if options.admin_command:
                         # todo: do this after enter game?
                         console.input = options.admin_command
                         # if options.single_command_exit:
                         #     console.input = 'exit'
 
                     StuphMUD.GreetPlayer(console)
@@ -232,49 +242,47 @@
                                 tracing = options.admin_trace,
                                 tokenize = options.parser_tokenize)
 
 
         if options.admin_script:
             from stuphos.runtime.architecture.lookup import LookupObject
             adminScript = LookupObject(options.admin_script)
-            adminScript(*options.admin_script_args)
+            adminScript(**parseArgvToKwd(options.admin_script_args))
 
 
         # The engine will be run another way.  Just return Core.
         if not options.no_run_engine:
             if options.debug > 1:
-                runcall(self.run)
+                runcall(self.run) # Todo: ShutdownGame
             elif options.asynchronous:
                 from _thread import start_new_thread as nth
-                nth(self.run, ())
+                nth(self.run, ()) # Todo: ShutdownGame
             else:
                 try: self.run(optimisticTermination = not bool(options.file))
                 except KeyboardInterrupt:
                     print()
 
                 StuphMUD.ShutdownGame()
+                # system.core.unreachable = True
 
     @property
     def blockingQueue(self):
         return self.cmdln['options'].blocking
 
     def resetWorldOption(self, options):
         if isYesValue(configuration.World.reset_on_boot):
             return True
 
         return options.reset_world
 
     def bootMudStart(self, options, stuphlib, worldModule):
         # Initialize MUD Package.
         import stuphos
-        if options.config_file:
-            # Note: this is necessary in order to activate 'configuration' builtin.
-            stuphos.reloadConfigFile(options.config_file)
 
-        stuphos.bootStart() # runtime.
+        stuphos.bootStart(options.config_file, options.set_option) # runtime.
 
         # Complete MUD Boot Cycle.
         self.bootStartTime = getSystemTime()
         if not options.no_world:
             self.event.call(self.bootWorld, options, stuphlib, worldModule)
 
         self.event += self.worldResetStart
```

### Comparing `stuphos-2.0.8/stuphos/system/db.py` & `stuphos-2.0.9/stuphos/system/db.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/game/__init__.py` & `stuphos-2.0.9/stuphos/system/game/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/game/compartment/__init__.py` & `stuphos-2.0.9/stuphos/system/game/compartment/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/game/compartment/cli.py` & `stuphos-2.0.9/stuphos/system/game/compartment/cli.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/game/compartment/misc/__init__.py` & `stuphos-2.0.9/stuphos/system/game/compartment/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/game/compartment/misc/devel.py` & `stuphos-2.0.9/stuphos/system/game/compartment/misc/devel.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/system/network.py` & `stuphos-2.0.9/stuphos/system/network.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/triggers.py` & `stuphos-2.0.9/stuphos/triggers.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/webserver/__init__.py` & `stuphos-2.0.9/stuphos/webserver/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,18 @@
 
     class ServerHandler(ServerHandler):
         def __init__(self, stdin, stdout, stderr, environ, software, **kwd):
                      # multithread = True, multiprocess = False):
             ServerHandler.__init__(self, stdin, stdout, stderr, environ, **kwd)
             self.server_software = software
 
+        def setup_environ(self):
+            ServerHandler.setup_environ(self)
+            self.environ['stuphos.streaming.handler'] = self
+
     def handle(self):
         """Copy of WSGIRequestHandler, but with different ServerHandler"""
 
         # [HTTP 192.168.43.1:52786] ConnectionResetError: [Errno 104] Connection reset by peer [<ssl.SSLSocket fd=15, family=AddressFamily.AF_INET, type=SocketKind.SOCK_STREAM, proto=0, laddr=('192.168.43.192', 2180)>]
         #   [socketserver.py:654] process_request_thread
         #     self.finish_request(request, client_address)
         #   [socketserver.py:364] finish_request
@@ -248,14 +252,15 @@
             return
 
         handler = self.ServerHandler(
             self.rfile, self.wfile, self.get_stderr(), self.get_environ(),
             self.server.software
         )
         handler.request_handler = self      # backpointer for logging
+        # self.handler = handler # for streaming
         handler.run(self.server.get_app())
 
 class LoggingWSGIRequestHandler(EmbeddedRequestHandler):
     'Disables logging of WSGI messages (conditionally).'
 
     def log_message(self, format, *args):
         from stuphos import getConfig
```

### Comparing `stuphos-2.0.8/stuphos/webserver/project/manage.py` & `stuphos-2.0.9/stuphos/webserver/project/manage.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/webserver/project/settings.py` & `stuphos-2.0.9/stuphos/webserver/project/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 gettext = (lambda text: text)
 CMS_TEMPLATES = (
     # ('page_base.html', gettext('StuphMUD Site Default')),
     # ('cms_base.html',  gettext('StuphCMS Base Page')),
 )
 
 LOGIN_URL = '/accounts/login'
-LOGIN_REDIRECT_URL = '/' # menu
+LOGIN_REDIRECT_URL = '/' # menu.  "after login where to redirect (?)"
 
 STATIC_ROOT = 'web/cms/media' # in lib: directory with cms -> package static dir
 STATIC_URL = '/media/'
 
 SEKIZAI_IGNORE_VALIDATION = True
 SEKIZAI_VARNAME = 'my_sekizai_VarName'
 
@@ -156,16 +156,18 @@
                 'django.template.context_processors.request',
                 'django.contrib.auth.context_processors.auth',
                 'django.contrib.messages.context_processors.messages',
             ],
 
             'loaders': ['django.template.loaders.filesystem.Loader',
                         'django.template.loaders.app_directories.Loader',
-                        #'ph.components.library.TemplateLoader'
-                        ]
+                        ] + (['ph.interpreter.mental.library.loader.TemplateLoader']
+                             if isYesValue(getConfig('virtual-templates', 'AgentSystem'))
+                             else [])
+
         },
     },
 
     # {
     #     'BACKEND': 'person.features.girl.LibraryTemplates'
     # }
 ]
```

### Comparing `stuphos-2.0.8/stuphos/webserver/project/urls.py` & `stuphos-2.0.9/stuphos/webserver/project/urls.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/webserver/services/checkpointing.py` & `stuphos-2.0.9/stuphos/webserver/services/checkpointing.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/xmlrpc/__init__.py` & `stuphos-2.0.9/stuphos/xmlrpc/__init__.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/xmlrpc/client.py` & `stuphos-2.0.9/stuphos/xmlrpc/client.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/xmlrpc/config.py` & `stuphos-2.0.9/stuphos/xmlrpc/config.py`

 * *Files identical despite different names*

### Comparing `stuphos-2.0.8/stuphos/xmlrpc/host.py` & `stuphos-2.0.9/stuphos/xmlrpc/host.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 import sys
 import json
 
 from stuphos import enqueueHeartbeatTask, logException
 from stuphos.etc import nth, reraiseSystemException, getSystemExceptionString
 from stuphos.etc.tools.timing import getCurrentTime as now
 
-ALLOWED_PORT_ORIGINS = [8000, 2180, None]
+ALLOWED_PORT_ORIGINS = [#8000,
+                        2180, None, 443]
 
 # CSRF Access Control.
 def getOriginAccess(request, origin):
     # Todo: Obviously, this is seriously unfinished:
     # This should come from an access table defined via mud-control.
     if origin and urlparse(origin).port in ALLOWED_PORT_ORIGINS:
         # note: this is no longer good enough for firefox/chrome
@@ -45,14 +46,16 @@
         finally:
             sys.stderr = stderr
 
 class Deferrable:
     # For GETs (handled but undispatched).
     deferred = False
 
+    billableIdentity = None
+
     def handleAccessControl(self):
         # https://developer.mozilla.org/En/HTTP_Access_Control
         allowOrigin = getOriginAccess(self, getattr(self, 'origin', None))
         if allowOrigin:
             #print 'Sending header', allowOrigin
             self.send_header('Access-Control-Allow-Origin', allowOrigin)
 
@@ -84,14 +87,23 @@
         try: self.wfile.flush()
         except AttributeError as e:
             if str(e) != "'NoneType' object has no attribute 'sendall'":
                 raise e
 
         self.connection.shutdown(1)
 
+        identity = getattr(self, 'billableIdentity', None)
+        if identity is not None:
+            self.chargeUserContent(identity, response)
+
+
+    def chargeUserContent(self, identity, response):
+        pass
+
+
     def finish(self):
         if not self.deferred:
             if not self.wfile.closed:
                 self.wfile.flush()
             self.wfile.close()
             self.rfile.close()
```

### Comparing `stuphos-2.0.8/stuphos.egg-info/PKG-INFO` & `stuphos-2.0.9/stuphos.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,266 +1,15 @@
 Metadata-Version: 2.1
 Name: stuphos
-Version: 2.0.8
-Summary: Containerization middleware.
+Version: 2.0.9
+Summary: Online productivity container.
 Home-page: http://thetaplane.com
 Author: 
 Author-email: 
 License: None
-Description: Copyright 2009-2022 Thetaplane . com
-        ====================================
-        
-        Virtualizes python so that it is isolated and controlled in terms of resource usage per
-        registered user account, and all operations are tracked by time, generating computational
-        telemetry and executive management.
-        
-        
-        Intended Audiences
-        ==================
-        
-        * System administrators who want to support protected user multitasking without system
-          management overhead.
-        * Web administrators who want to publish a CMS site with integrated real-time networking.
-        * Physical and computational scientific research.  Python 3 users.
-        
-        
-        Legal and Operational Notes
-        ===========================
-        
-        This software makes use of cryptographic algorithms, designed to protect the user data
-        and the user, but may be restricted in jurisdictions that overrule their use.
-        
-        Please research the full law regarding data and information security.
-        
-        THERE IS ABSOLUTELY NO WARRANTY INCLUDED.
-        
-        
-        Starting
-        ========
-        
-        Unpack the skeletoncore.tar.gz directory and configure it for your application (the
-        location of the stuphos packages in your PYTHONPATH), then switch to that directory
-        and run it like this: ./runcore --headless &
-        
-        Connect to it with a web browser.
-        
-        
-        Boot Procedure
-        ==============
-        
-        An embedding core invokes the boot start and complete routines in the mud module to
-        initialize the bindings and runtime.
-        
-        These things start up in the application, opening up all components and facilities.
-        
-            * Event bridge module is constructed and initialized
-            * Registry is configured (with bridge for shutdown events)
-            * VM installed
-            * Site packages are loaded
-            * Paths for system packages are configured
-            * Environment updated
-            * XMLRPC host started
-            * System journal installed, system packages loaded
-        
-            * Management components
-                * Web Adapter Session Manager
-                * WSGI Webserver
-        
-            * Facilities:
-                * AgentSystem and Elemental Interpreter
-        
-            * Zones
-            * Commands
-            * Warmboot
-            * Engine Loop
-        
-        
-        Application & Core Architecture
-        ===============================
-        
-        The system uses a collection of components to build its application of managing objects.
-        One of the components is the 'registry' which names unique objects within the runtime,
-        and requires that it be installed during boot time (this is normally handled by the
-        boot procedure).
-        
-        Other component package implementations are configured using the 'components.pth' file
-        for service implementations, external (third-party) server package installations, and
-        developmental modules.
-        
-        
-        Supplemental
-        ============
-        
-        With an extended license, the 'ph' package contains a virtual machine computational
-        core and database querying engine.
-        
-        The 'stuphmud' package contains code previously released in ''stuphos-lite''.
-        
-        
-        Filesystem and Command-Line Configuration
-        =========================================
-        
-        Options:
-            -w --world-dir                          path
-            -z --zone-index --index                 string
-            -i --interactive                        bool
-            -a --async                              bool
-            -W --cascade --load-world               bool
-            -C --config-file --config --game-config path
-            -g --debug                              count
-            -n --no-world                           bool
-            -p --port                               integer
-            -m --mud-package --mud                  string
-            -s --supreme                            bool
-            --admin-name                            string
-            --enter-game                            bool
-            -L --data-dir --lib-dir                 path
-            -v --verbose                            count
-            --headless --no-console                 bool
-        
-        Experimental:
-            --blocking                              integer
-            --runpid                                bool
-            --timeout                               integer
-        
-            --parser-tokenize                       bool
-            --elemental-parser-debug, --parser-debug
-        
-            --no-run-engine                         bool
-        
-        Additional:
-            --reset-world                           bool
-            -Z, --full-world                        bool
-            -e, --service                           list
-        
-            --admin-script                          string
-            -x, --admin-script-args                 list
-        
-            -f, --file                              string
-        
-            -c, --admin-command                     string
-            --admin-trace                           bool
-        
-            --no-init                               bool
-        
-            --tool-package                          list
-            --agent-system                          string
-            --local, --local-filesystem             string
-        
-        
-        The configuration file has the following options:
-        
-            [MUD]
-            config-dir = .
-            components: components.pth
-            traceback-relative: yes
-            log-uncaught-traceback: yes
-            logindent = 4
-            greetings: name prompt %w means whitespace
-            greeting-delay: 1.2
-            http-redirect-url: https://thetaplane.com/
-            player-store-shelf = %(config-dir)s/.players.shelf
-            zone-config-file = .zone-modules.cfg
-            world-path = ../../lib/archive/lib/world
-            olc-world-path = ../../lib/archive/lib/world
-            zone-database: sqlite
-        
-        
-            [Management]
-            embedded-webserver: yes
-            pentacle-service: no
-            session-adapter: yes
-            system-shell: no
-            subdaemon-manager: no
-            syslog-scanner: no
-        
-        
-            [XMLRPC]
-            off: off
-            address: 0.0.0.0
-            ; certificate-path = server.pem
-        
-        
-            [Security]
-            trust-localhost: yes
-            ; trusted-domain: 10.0.0.1
-        
-        
-            [Interpreter]
-            rich-editor: yes
-            player-notebook: yes
-            wizard-gc: yes
-            checkpointing: no
-            native-traceback: yes ; no
-        
-        
-            [Environment]
-            PENTACLE_PARTNER_NAME = 'stuphos/mud'
-        
-        
-            [Syslog]
-            path.1: ..\log\syslog*
-            path.2: mattercore.run.log
-            patterns: etc\syslog-patterns.cfg
-        
-        
-            [Services]
-            facility.billing: ph.emulation.billing.BillingCore
-        
-        
-            [DjangoService]
-            port = 2180
-            database = sqlite
-            sitemap = stuphos.webserver.project.urls
-            show-debug-page = admin
-            certificate-path = server.pem
-            software: phaseware
-            log-request: yes
-            hosts:
-                <public ip address 1>
-                <hostname 1>
-                <hostname 2>
-                ...
-            media:
-                serving-path: folder-path
-            webapps:
-                person.services.web
-                ...
-        
-            [DBCore]
-            primary.type = pg-auth
-            primary.path = ../lib/db.conf ; username\npassword\n
-            primary.host = 127.0.0.1
-            primary.port = 5432
-            sqlite.type = sqlite
-            sqlite.path = sqlite:webcore.db
-            sqlite.file-path = webcore.db
-        
-        
-            [SystemComponents]
-            system-path.common: /workspace/library/packages/common
-        
-            [SystemPackages]
-            package.wrlc: op
-        
-            [Logging]
-            database: sqlite
-        
-            [Billing]
-            policy-rates-path = ../resources/rates.wmc
-        
-        
-        
-        Web Interface Guide
-        ===================
-        
-        The application is developed internally by programming principals, which require user
-        authentication.  Programming documentation should be viewable within the online interface.
-        
-        
 Platform: OS-independent
 Platform: Many
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Environment :: Other Environment
 Classifier: Environment :: Web Environment
@@ -300,7 +49,233 @@
 Classifier: Topic :: System :: Operating System Kernels
 Classifier: Topic :: System :: Operating System
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals :: Telnet
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: XML
 Description-Content-Type: text/plain
+
+Copyright 2009-2022 Thetaplane . com
+====================================
+
+Virtualizes python so that it is isolated and controlled in terms of resource usage per
+registered user account, and all operations are tracked by time, generating computational
+telemetry and executive management.
+
+
+Intended Audiences
+==================
+
+* System administrators who want to support protected user multitasking without system
+  management overhead.
+* Web administrators who want to publish a CMS site with integrated real-time networking.
+* Physical and computational scientific research.  Python 3 users.
+
+
+Legal and Operational Notes
+===========================
+
+This software makes use of cryptographic algorithms, designed to protect the user data
+and the user, but may be restricted in jurisdictions that overrule their use.
+
+Please research the full law regarding data and information security.
+
+THERE IS ABSOLUTELY NO WARRANTY INCLUDED.
+
+
+Starting
+========
+
+Unpack the skeletoncore.tar.gz directory and configure it for your application (the
+location of the stuphos packages in your PYTHONPATH), then switch to that directory
+and run it like this: ./runcore --headless &
+
+Connect to it with a web browser.
+
+
+Boot Procedure
+==============
+
+An embedding core invokes the boot start and complete routines in the mud module to
+initialize the bindings and runtime.
+
+These things start up in the application, opening up all components and facilities.
+
+    * Registry is configured
+    * Site packages are loaded
+    * Event bridge module is constructed and initialized
+    * VM, system journal installed
+    * System package paths are installed
+    * Environment updated
+    * XMLRPC host started
+    * Management components
+        * Web Adapter Session Manager
+        * WSGI Webserver
+
+    * Facilities:
+        * AgentSystem and Elemental Interpreter
+
+    * Zones
+    * Commands
+    * Warmboot
+    * Engine Loop
+
+
+Application & Core Architecture
+===============================
+
+The system uses a collection of components to build its application of managing objects.
+One of the components is the 'registry' which names unique objects within the runtime,
+and requires that it be installed during boot time (this is normally handled by the
+boot procedure).
+
+Other component package implementations are configured using the 'components.pth' file
+for service implementations, external (third-party) server package installations, and
+developmental modules.
+
+
+Supplemental
+============
+
+With an extended license, the 'ph' package contains a virtual machine computational
+core and database querying engine.
+
+The 'stuphmud' package contains code previously released in ''stuphos-lite''.
+
+
+Filesystem and Command-Line Configuration
+=========================================
+
+Options:
+    -w --world-dir                          path
+    -z --zone-index --index                 string
+    -i --interactive                        bool
+    -a --async                              bool
+    -W --cascade --load-world               bool
+    -C --config-file --config --game-config path
+    -g --debug                              count
+    -n --no-world                           bool
+    -p --port                               integer
+    -m --mud-package --mud                  string
+    -s --supreme                            bool
+    --admin-name                            string
+    --enter-game                            bool
+    -L --data-dir --lib-dir                 path
+    -v --verbose                            count
+    --headless --no-console                 bool
+
+Experimental:
+    --blocking                              integer
+    --runpid                                bool
+
+
+The configuration file has the following options:
+
+    [MUD]
+    config-dir = .
+    components: components.pth
+    traceback-relative: yes
+    log-uncaught-traceback: yes
+    logindent = 4
+    greetings: name prompt %w means whitespace
+    greeting-delay: 1.2
+    http-redirect-url: https://runphase.com:2180/
+    player-store-shelf = %(config-dir)s/.players.shelf
+    zone-config-file = .zone-modules.cfg
+    world-path = ../../lib/archive/lib/world
+    olc-world-path = ../../lib/archive/lib/world
+    zone-database: sqlite
+
+
+    [Management]
+    embedded-webserver: yes
+    pentacle-service: no
+    session-adapter: yes
+    system-shell: no
+    subdaemon-manager: no
+    syslog-scanner: no
+
+
+    [XMLRPC]
+    off: off
+    address: 0.0.0.0
+    ; certificate-path = server.pem
+
+
+    [Security]
+    trust-localhost: yes
+    ; trusted-domain: 10.0.0.1
+
+
+    [Interpreter]
+    rich-editor: yes
+    player-notebook: yes
+    wizard-gc: yes
+    checkpointing: no
+    native-traceback: yes ; no
+
+
+    [Environment]
+    PENTACLE_PARTNER_NAME = 'stuphos/mud'
+
+
+    [Syslog]
+    path.1: ..\log\syslog*
+    path.2: mattercore.run.log
+    patterns: etc\syslog-patterns.cfg
+
+
+    [Services]
+    facility.billing: ph.emulation.billing.BillingCore
+
+
+    [DjangoService]
+    port = 2180
+    database = sqlite
+    sitemap = stuphos.webserver.project.urls
+    show-debug-page = admin
+    certificate-path = server.pem
+    software: phaseware
+    log-request: yes
+    hosts:
+        <public ip address 1>
+        <hostname 1>
+        <hostname 2>
+        ...
+    media:
+        serving-path: folder-path
+    webapps:
+        person.services.web
+        ...
+
+    [DBCore]
+    primary.type = pg-auth
+    primary.path = ../lib/db.conf ; username\npassword\n
+    primary.host = 127.0.0.1
+    primary.port = 5432
+    sqlite.type = sqlite
+    sqlite.path = sqlite:webcore.db
+    sqlite.file-path = webcore.db
+
+
+    [SystemComponents]
+    system-path.common: /workspace/library/packages/common
+
+    [SystemPackages]
+    package.wrlc: op
+
+    [Logging]
+    database: sqlite
+
+    [Billing]
+    policy-rates-path = ../resources/rates.wmc
+
+
+
+Web Interface Guide
+===================
+
+The application is developed internally by programming principals, which require user
+authentication.  Programming documentation should be viewable within the online interface.
+
+
+
```

### Comparing `stuphos-2.0.8/stuphos.egg-info/SOURCES.txt` & `stuphos-2.0.9/stuphos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MANIFEST.in
 README
 setup.py
+setupCMR.py
 skeletoncore.tar.gz
 stuphmud/__init__.py
 stuphmud/elemental.py
 stuphmud/server/__init__.py
 stuphmud/server/adapters.py
 stuphmud/server/api/__init__.py
 stuphmud/server/api/constants.py
@@ -68,15 +69,20 @@
 stuphmud/server/zones/freeze.py
 stuphmud/server/zones/physical.py
 stuphmud/server/zones/space.py
 stuphmud/server/zones/wilderness.py
 stuphmud/server/zones/specials/__init__.py
 stuphmud/server/zones/specials/standard.py
 stuphmud/server/zones/specials/autoquest/__init__.py
+stuphmud/server/zones/specials/autoquest/behaviors.npc
+stuphmud/server/zones/specials/autoquest/quest-help-topics.txt
+stuphmud/server/zones/specials/autoquest/quest-help.txt
+stuphmud/server/zones/specials/autoquest/quests.cfg
 stuphmud/server/zones/specials/autoquest/slay.py
+stuphmud/server/zones/specials/autoquest/senarios/slay1.qst
 stuphos/__init__.py
 stuphos/structure.py
 stuphos/triggers.py
 stuphos.egg-info/PKG-INFO
 stuphos.egg-info/SOURCES.txt
 stuphos.egg-info/dependency_links.txt
 stuphos.egg-info/top_level.txt
@@ -111,14 +117,15 @@
 stuphos/language/document/wrlc.py
 stuphos/language/gen/__init__.py
 stuphos/language/gen/gs_indent_lexer.py
 stuphos/language/query/__init__.py
 stuphos/language/query/ql2.py
 stuphos/language/vm/__init__.py
 stuphos/language/xml/__init__.py
+stuphos/language/xml/stuph.xml
 stuphos/management/__init__.py
 stuphos/management/authlock.py
 stuphos/management/autowiz.py
 stuphos/management/config.py
 stuphos/management/deploy.py
 stuphos/management/idling.py
 stuphos/management/naming.py
@@ -135,14 +142,15 @@
 stuphos/management/command_messaging/base.py
 stuphos/management/command_messaging/deployment.py
 stuphos/management/command_messaging/girl.py
 stuphos/management/command_messaging/python.py
 stuphos/management/command_messaging/resource.py
 stuphos/management/command_messaging/shell.py
 stuphos/management/command_messaging/subdaemon.py
+stuphos/management/command_messaging/samples/penro_team_core.py
 stuphos/management/protocols/__init__.py
 stuphos/management/protocols/http.py
 stuphos/pentacle/__init__.py
 stuphos/pentacle/management.py
 stuphos/pentacle/native.py
 stuphos/pentacle/oob.py
 stuphos/pentacle/partner.py
@@ -203,14 +211,15 @@
 stuphos/system/game/compartment/cli.py
 stuphos/system/game/compartment/system.py
 stuphos/system/game/compartment/format/__init__.py
 stuphos/system/game/compartment/misc/__init__.py
 stuphos/system/game/compartment/misc/devel.py
 stuphos/webserver/__init__.py
 stuphos/webserver/project/__init__.py
+stuphos/webserver/project/loadOlc.sh
 stuphos/webserver/project/manage.py
 stuphos/webserver/project/settings.py
 stuphos/webserver/project/urls.py
 stuphos/webserver/services/__init__.py
 stuphos/webserver/services/checkpointing.py
 stuphos/xmlrpc/__init__.py
 stuphos/xmlrpc/client.py
```

