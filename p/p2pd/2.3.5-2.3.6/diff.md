# Comparing `tmp/p2pd-2.3.5.tar.gz` & `tmp/p2pd-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/p2pd-2.3.5.tar", last modified: Thu Feb 16 03:42:35 2023, max compression
+gzip compressed data, was "p2pd-2.3.6.tar", last modified: Sat Apr 29 16:38:35 2023, max compression
```

## Comparing `p2pd-2.3.5.tar` & `p2pd-2.3.6.tar`

### file list

```diff
@@ -1,50 +1,78 @@
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-02-16 03:42:35.000000 p2pd-2.3.5/
--rw-rw-r--   0 x         (1000) x         (1000)     6189 2023-02-16 03:42:35.000000 p2pd-2.3.5/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)     4543 2023-01-29 09:34:01.000000 p2pd-2.3.5/README.md
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd/
--rw-rw-r--   0 x         (1000) x         (1000)     1196 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)     7065 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/ack_udp.py
--rw-rw-r--   0 x         (1000) x         (1000)     6437 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/address.py
--rw-rw-r--   0 x         (1000) x         (1000)    30486 2023-01-29 09:34:01.000000 p2pd-2.3.5/p2pd/base_stream.py
--rw-rw-r--   0 x         (1000) x         (1000)     8028 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/clock_skew.py
--rw-rw-r--   0 x         (1000) x         (1000)     8004 2023-01-29 09:34:05.000000 p2pd-2.3.5/p2pd/cmd_tools.py
--rw-rw-r--   0 x         (1000) x         (1000)     7896 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/daemon.py
--rw-rw-r--   0 x         (1000) x         (1000)      303 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/echo_server.py
--rw-rw-r--   0 x         (1000) x         (1000)      222 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/errors.py
--rw-rw-r--   0 x         (1000) x         (1000)     2465 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/http_client_lib.py
--rw-rw-r--   0 x         (1000) x         (1000)     5968 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/http_server_lib.py
--rw-rw-r--   0 x         (1000) x         (1000)    19527 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/interface.py
--rw-rw-r--   0 x         (1000) x         (1000)    11971 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/ip_range.py
--rw-rw-r--   0 x         (1000) x         (1000)    27256 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/nat.py
--rw-rw-r--   0 x         (1000) x         (1000)    22921 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/net.py
--rw-rw-r--   0 x         (1000) x         (1000)     4438 2023-01-07 14:17:58.000000 p2pd-2.3.5/p2pd/netiface_extra.py
--rw-rw-r--   0 x         (1000) x         (1000)    13973 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/ntp_client.py
--rw-rw-r--   0 x         (1000) x         (1000)     6624 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/p2p_addr.py
--rw-rw-r--   0 x         (1000) x         (1000)    13199 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/p2p_node.py
--rw-rw-r--   0 x         (1000) x         (1000)    26320 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/p2p_pipe.py
--rw-rw-r--   0 x         (1000) x         (1000)    15517 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/p2p_protocol.py
--rw-rw-r--   0 x         (1000) x         (1000)     2986 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/p2p_utils.py
--rw-rw-r--   0 x         (1000) x         (1000)    13146 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/rest_api.py
--rw-rw-r--   0 x         (1000) x         (1000)    32854 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/route.py
--rw-rw-r--   0 x         (1000) x         (1000)     5992 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/route_table.py
--rw-rw-r--   0 x         (1000) x         (1000)     7094 2023-02-16 03:40:14.000000 p2pd-2.3.5/p2pd/settings.py
--rw-rw-r--   0 x         (1000) x         (1000)     2885 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/signaling.py
--rw-rw-r--   0 x         (1000) x         (1000)    42083 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/stun_client.py
--rw-rw-r--   0 x         (1000) x         (1000)    40903 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/tcp_punch.py
--rw-rw-r--   0 x         (1000) x         (1000)     4366 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/test_init.py
--rw-rw-r--   0 x         (1000) x         (1000)    16867 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/turn_client.py
--rw-rw-r--   0 x         (1000) x         (1000)    13940 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/turn_defs.py
--rw-rw-r--   0 x         (1000) x         (1000)    10862 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/turn_process.py
--rw-rw-r--   0 x         (1000) x         (1000)    13894 2023-01-14 07:17:08.000000 p2pd-2.3.5/p2pd/upnp.py
--rw-rw-r--   0 x         (1000) x         (1000)    16078 2023-01-29 09:34:05.000000 p2pd-2.3.5/p2pd/utils.py
--rw-rw-r--   0 x         (1000) x         (1000)     1027 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/var_names.py
--rw-rw-r--   0 x         (1000) x         (1000)     4220 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/win_net.py
--rw-rw-r--   0 x         (1000) x         (1000)    16718 2023-01-05 09:43:21.000000 p2pd-2.3.5/p2pd/win_netifaces.py
-drwxrwxr-x   0 x         (1000) x         (1000)        0 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd.egg-info/
--rw-rw-r--   0 x         (1000) x         (1000)     6189 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd.egg-info/PKG-INFO
--rw-rw-r--   0 x         (1000) x         (1000)      912 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd.egg-info/SOURCES.txt
--rw-rw-r--   0 x         (1000) x         (1000)        1 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd.egg-info/dependency_links.txt
--rw-rw-r--   0 x         (1000) x         (1000)      103 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd.egg-info/requires.txt
--rw-rw-r--   0 x         (1000) x         (1000)        5 2023-02-16 03:42:35.000000 p2pd-2.3.5/p2pd.egg-info/top_level.txt
--rw-rw-r--   0 x         (1000) x         (1000)       38 2023-02-16 03:42:35.000000 p2pd-2.3.5/setup.cfg
--rw-rw-r--   0 x         (1000) x         (1000)     1161 2023-02-16 03:35:40.000000 p2pd-2.3.5/setup.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.299638 p2pd-2.3.6/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1570 2023-04-28 06:42:33.000000 p2pd-2.3.6/CREDITS.md
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1072 2023-04-28 06:42:33.000000 p2pd-2.3.6/LICENSE
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      106 2023-04-29 16:38:16.000000 p2pd-2.3.6/MANIFEST.in
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5084 2023-04-29 16:38:35.299638 p2pd-2.3.6/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4543 2023-04-28 06:42:33.000000 p2pd-2.3.6/README.md
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.295637 p2pd-2.3.6/p2pd/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1196 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/__init__.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7065 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/ack_udp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6437 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    30486 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/base_stream.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8028 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8004 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/cmd_tools.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7896 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      303 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/echo_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      222 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/errors.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2465 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/http_client_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5968 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/http_server_lib.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    19527 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    11971 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    27256 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    22921 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4438 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/netiface_extra.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13973 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/ntp_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     6624 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13199 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_node.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    26320 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    15517 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_protocol.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2986 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/p2p_utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13146 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/rest_api.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    32854 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5992 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7094 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/settings.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    42083 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    40903 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4366 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/test_init.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16867 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13940 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/turn_defs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    10862 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/turn_process.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    13894 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/upnp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16078 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/utils.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1027 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/var_names.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4220 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/win_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)    16718 2023-04-28 06:42:33.000000 p2pd-2.3.6/p2pd/win_netifaces.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.295637 p2pd-2.3.6/p2pd.egg-info/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5084 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/PKG-INFO
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1482 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/SOURCES.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        1 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/dependency_links.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      103 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/requires.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        5 2023-04-29 16:38:35.000000 p2pd-2.3.6/p2pd.egg-info/top_level.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      305 2023-04-28 06:42:33.000000 p2pd-2.3.6/requirements.txt
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)       38 2023-04-29 16:38:35.299638 p2pd-2.3.6/setup.cfg
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1161 2023-04-29 16:23:03.000000 p2pd-2.3.6/setup.py
+drwxr-xr-x   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)        0 2023-04-29 16:38:35.299638 p2pd-2.3.6/tests/
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1090 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_address.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     4111 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_bind.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      735 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_clock_skew.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5211 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_cmd.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5111 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_daemon.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2885 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_interface.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5161 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_ip_range.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     7449 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_nat.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2016 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_net.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2038 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_net_afs.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      394 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_p2p_addr.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     8187 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_p2p_pipe.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2759 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_p2pd_server.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     9323 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_route.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1618 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_route_table.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1406 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_rudp.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1377 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_signaling.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     1545 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_sock.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)      992 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_sorted_search.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3355 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_stun_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     5617 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_tcp_punch.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     3537 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_turn_client.py
+-rw-r--r--   0 lounge-linux-vm  (1000) lounge-linux-vm  (1000)     2823 2023-04-28 06:42:33.000000 p2pd-2.3.6/tests/test_win_netifaces.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `p2pd-2.3.5/PKG-INFO` & `p2pd-2.3.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,151 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.3.5
+Version: 2.3.6
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
-Description: # P2PD
-        
-        ``[Coverage >= 82%] [Python >= 3.6] [Mac, Win, Nix, BSD, Android]``
-        
-        **P2PD** is a new async networking library for Python. It's based on solving some of the problems with Python's existing APIs and supports P2P networking among other features.
-        
-        Let's look at some examples.
-        Start the Python REPL with await support with:
-        
-        > python3 -m asyncio
-        
-        Initialise information about your network interfaces.
-        
-        ```python
-        from p2pd import *
-        netifaces = await init_p2pd() # Same API as netifaces
-        ```
-        
-        Load default interface and load details about it's NAT.
-        
-        ```python
-        i = await Interface(netifaces=netifaces)
-        await i.load_nat()
-        ```
-        
-        Choose an external address to use for an endpoint.
-        Resolve the address of an echo server.
-        
-        ```python
-        route = await i.route().bind()
-        dest = await Address("p2pd.net", 7, route)
-        ```
-        
-        Build an async UDP pipe to the server.
-        
-        ```python
-        pipe = await pipe_open(UDP, dest, route)
-        pipe.subscribe()
-        ```
-        
-        Do some I/O on the pipe and cleanup.
-        
-        ```python
-        # UDP so may not arrive.
-        await pipe.send(b"some message", dest_tup)
-        out = await pipe.recv(timeout=2)
-        print(out)
-        ```
-        
-        ## P2P networking
-        
-        How about an example that does P2P networking?
-        
-        ```python
-        from p2pd import *
-        
-        # Put your custom protocol code here.
-        async def custom_protocol(msg, client_tup, pipe):
-            # E.G. add a ping feature to your protocol.
-            if b"PING" in msg:
-                await pipe.send(b"PONG")
-        
-        async def make_p2p_con():
-            # Initalize p2pd.
-            netifaces = await init_p2pd()
-            #
-            # Start our main node server.
-            # The node implements your protocol.
-            node = await start_p2p_node(netifaces=netifaces)
-            node.add_msg_cb(custom_protocol)
-            #
-            # Spawn a new pipe from a P2P con.
-            # Connect to our own node server.
-            pipe = await node.connect(node.addr_bytes)
-            pipe.subscribe(SUB_ALL)
-            #
-            # Test send / receive.
-            msg = b"test send"
-            await pipe.send(b"ECHO " + msg)
-            out = await pipe.recv()
-            #
-            # Cleanup.
-            assert(msg in out)
-            await pipe.close()
-            await node.close()
-        
-        # Run the coroutine.
-        # Or await make_p2p_con() if in async REPL.
-        async_test(make_p2p_con)
-        ```
-        
-        In this example the node connects to itself but it could just as easily be used to connect to another peer.
-        
-        ## Features
-        
-        **P2PD** is a new project aiming to make peer-to-peer networking
-        simple and ubiquitous. P2PD can be used either as a library or as a service.
-        As a library P2PD is written in Python 3 using asyncio for everything.
-        As a service P2PD provides a REST API on http://127.0.0.1:12333/.
-        The REST API is provided for non-Python languages.
-        
-        P2PD offers engineers the following features:
-        
-        - Multiple strategies for establishing peer-to-peer direct connections.
-        
-          - **Direct connect** = Connect to a reachable node.
-          - **Reverse connect** = Tell a node to connect to you.
-          - **TCP hole punching** = Simultaneous TCP connections.
-          - **TURN** = Use a proxy server as a last resort.
-        - **Advanced NAT detection.** P2PD can detect 7 different types of NATs and
-           5 different sub-types for a combined total of **35 unique NAT
-           configurations.** The result is better NAT bypass.
-        - **Smart TCP hole punching.** The TCP hole punching algorithm has been
-           designed to require minimal communication between peers to increase
-           the chances of success. The algorithm supports a diverse number of
-           NAT configurations for the best results possible.
-        - **Port forwarding (IPv4) and pin hole (IPv6.)** Automatically
-           handles openning ports on the router to increase reachability.
-        - **IPv6 ready from day 1.** Supports IPv4 and IPv6. Introduces a new
-           format for addresses that offers insight into a peer's
-           NIC cards, internal network, and NAT devices.
-        - **A new way to do network programming.** Focuses on NICs as the
-           starting point for building services. Introduces 'routes' as a
-           way to provide visibility into external addresses. You can build
-           services that support IPv4, IPv6, TCP, and UDP without writing
-           different code for each of them.
-        - **Language-agnostic REST API.** You can call **/p2p/open/name/addr**
-           then **/p2p/pipe/name** to turn any HTTP connection into a two-way relay
-           between a peer-to-peer connection.
-        - **Minimal dependencies.** Most of the code in P2PD uses the Python
-          standard library to improve portability and reduce packaging issues.
-        - **Built on open protocols.** P2PD uses **STUN** for address lookups,
-           **MQTT** for signaling messages, and **TURN** for last resort proxying.
-           All of these protocols have public infrastructure.
-        
-        Learn how to use the software:
-        https://p2pd.readthedocs.io/
-        
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# P2PD
+
+``[Coverage >= 82%] [Python >= 3.6] [Mac, Win, Nix, BSD, Android]``
+
+**P2PD** is a new async networking library for Python. It's based on solving some of the problems with Python's existing APIs and supports P2P networking among other features.
+
+Let's look at some examples.
+Start the Python REPL with await support with:
+
+> python3 -m asyncio
+
+Initialise information about your network interfaces.
+
+```python
+from p2pd import *
+netifaces = await init_p2pd() # Same API as netifaces
+```
+
+Load default interface and load details about it's NAT.
+
+```python
+i = await Interface(netifaces=netifaces)
+await i.load_nat()
+```
+
+Choose an external address to use for an endpoint.
+Resolve the address of an echo server.
+
+```python
+route = await i.route().bind()
+dest = await Address("p2pd.net", 7, route)
+```
+
+Build an async UDP pipe to the server.
+
+```python
+pipe = await pipe_open(UDP, dest, route)
+pipe.subscribe()
+```
+
+Do some I/O on the pipe and cleanup.
+
+```python
+# UDP so may not arrive.
+await pipe.send(b"some message", dest_tup)
+out = await pipe.recv(timeout=2)
+print(out)
+```
+
+## P2P networking
+
+How about an example that does P2P networking?
+
+```python
+from p2pd import *
+
+# Put your custom protocol code here.
+async def custom_protocol(msg, client_tup, pipe):
+    # E.G. add a ping feature to your protocol.
+    if b"PING" in msg:
+        await pipe.send(b"PONG")
+
+async def make_p2p_con():
+    # Initalize p2pd.
+    netifaces = await init_p2pd()
+    #
+    # Start our main node server.
+    # The node implements your protocol.
+    node = await start_p2p_node(netifaces=netifaces)
+    node.add_msg_cb(custom_protocol)
+    #
+    # Spawn a new pipe from a P2P con.
+    # Connect to our own node server.
+    pipe = await node.connect(node.addr_bytes)
+    pipe.subscribe(SUB_ALL)
+    #
+    # Test send / receive.
+    msg = b"test send"
+    await pipe.send(b"ECHO " + msg)
+    out = await pipe.recv()
+    #
+    # Cleanup.
+    assert(msg in out)
+    await pipe.close()
+    await node.close()
+
+# Run the coroutine.
+# Or await make_p2p_con() if in async REPL.
+async_test(make_p2p_con)
+```
+
+In this example the node connects to itself but it could just as easily be used to connect to another peer.
+
+## Features
+
+**P2PD** is a new project aiming to make peer-to-peer networking
+simple and ubiquitous. P2PD can be used either as a library or as a service.
+As a library P2PD is written in Python 3 using asyncio for everything.
+As a service P2PD provides a REST API on http://127.0.0.1:12333/.
+The REST API is provided for non-Python languages.
+
+P2PD offers engineers the following features:
+
+- Multiple strategies for establishing peer-to-peer direct connections.
+
+  - **Direct connect** = Connect to a reachable node.
+  - **Reverse connect** = Tell a node to connect to you.
+  - **TCP hole punching** = Simultaneous TCP connections.
+  - **TURN** = Use a proxy server as a last resort.
+- **Advanced NAT detection.** P2PD can detect 7 different types of NATs and
+   5 different sub-types for a combined total of **35 unique NAT
+   configurations.** The result is better NAT bypass.
+- **Smart TCP hole punching.** The TCP hole punching algorithm has been
+   designed to require minimal communication between peers to increase
+   the chances of success. The algorithm supports a diverse number of
+   NAT configurations for the best results possible.
+- **Port forwarding (IPv4) and pin hole (IPv6.)** Automatically
+   handles openning ports on the router to increase reachability.
+- **IPv6 ready from day 1.** Supports IPv4 and IPv6. Introduces a new
+   format for addresses that offers insight into a peer's
+   NIC cards, internal network, and NAT devices.
+- **A new way to do network programming.** Focuses on NICs as the
+   starting point for building services. Introduces 'routes' as a
+   way to provide visibility into external addresses. You can build
+   services that support IPv4, IPv6, TCP, and UDP without writing
+   different code for each of them.
+- **Language-agnostic REST API.** You can call **/p2p/open/name/addr**
+   then **/p2p/pipe/name** to turn any HTTP connection into a two-way relay
+   between a peer-to-peer connection.
+- **Minimal dependencies.** Most of the code in P2PD uses the Python
+  standard library to improve portability and reduce packaging issues.
+- **Built on open protocols.** P2PD uses **STUN** for address lookups,
+   **MQTT** for signaling messages, and **TURN** for last resort proxying.
+   All of these protocols have public infrastructure.
+
+Learn how to use the software:
+https://p2pd.readthedocs.io/
```

### Comparing `p2pd-2.3.5/README.md` & `p2pd-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/__init__.py` & `p2pd-2.3.6/p2pd/__init__.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/ack_udp.py` & `p2pd-2.3.6/p2pd/ack_udp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/address.py` & `p2pd-2.3.6/p2pd/address.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/base_stream.py` & `p2pd-2.3.6/p2pd/base_stream.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/clock_skew.py` & `p2pd-2.3.6/p2pd/clock_skew.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/cmd_tools.py` & `p2pd-2.3.6/p2pd/cmd_tools.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/daemon.py` & `p2pd-2.3.6/p2pd/daemon.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/http_client_lib.py` & `p2pd-2.3.6/p2pd/http_client_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/http_server_lib.py` & `p2pd-2.3.6/p2pd/http_server_lib.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/interface.py` & `p2pd-2.3.6/p2pd/interface.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/ip_range.py` & `p2pd-2.3.6/p2pd/ip_range.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/nat.py` & `p2pd-2.3.6/p2pd/nat.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/net.py` & `p2pd-2.3.6/p2pd/net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/netiface_extra.py` & `p2pd-2.3.6/p2pd/netiface_extra.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/ntp_client.py` & `p2pd-2.3.6/p2pd/ntp_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/p2p_addr.py` & `p2pd-2.3.6/p2pd/p2p_addr.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/p2p_node.py` & `p2pd-2.3.6/p2pd/p2p_node.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/p2p_pipe.py` & `p2pd-2.3.6/p2pd/p2p_pipe.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/p2p_protocol.py` & `p2pd-2.3.6/p2pd/p2p_protocol.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/p2p_utils.py` & `p2pd-2.3.6/p2pd/p2p_utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/rest_api.py` & `p2pd-2.3.6/p2pd/rest_api.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/route.py` & `p2pd-2.3.6/p2pd/route.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/route_table.py` & `p2pd-2.3.6/p2pd/route_table.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/settings.py` & `p2pd-2.3.6/p2pd/settings.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/signaling.py` & `p2pd-2.3.6/p2pd/signaling.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/stun_client.py` & `p2pd-2.3.6/p2pd/stun_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/tcp_punch.py` & `p2pd-2.3.6/p2pd/tcp_punch.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/test_init.py` & `p2pd-2.3.6/p2pd/test_init.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/turn_client.py` & `p2pd-2.3.6/p2pd/turn_client.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/turn_defs.py` & `p2pd-2.3.6/p2pd/turn_defs.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/turn_process.py` & `p2pd-2.3.6/p2pd/turn_process.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/upnp.py` & `p2pd-2.3.6/p2pd/upnp.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/utils.py` & `p2pd-2.3.6/p2pd/utils.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/var_names.py` & `p2pd-2.3.6/p2pd/var_names.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/win_net.py` & `p2pd-2.3.6/p2pd/win_net.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd/win_netifaces.py` & `p2pd-2.3.6/p2pd/win_netifaces.py`

 * *Files identical despite different names*

### Comparing `p2pd-2.3.5/p2pd.egg-info/PKG-INFO` & `p2pd-2.3.6/p2pd.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,151 @@
 Metadata-Version: 2.1
 Name: p2pd
-Version: 2.3.5
+Version: 2.3.6
 Summary: Asynchronous P2P networking library and service
 Home-page: http://github.com/robertsdotpm/p2pd
 Author: Matthew Roberts
 Author-email: matthew@roberts.pm
 License: public domain
-Description: # P2PD
-        
-        ``[Coverage >= 82%] [Python >= 3.6] [Mac, Win, Nix, BSD, Android]``
-        
-        **P2PD** is a new async networking library for Python. It's based on solving some of the problems with Python's existing APIs and supports P2P networking among other features.
-        
-        Let's look at some examples.
-        Start the Python REPL with await support with:
-        
-        > python3 -m asyncio
-        
-        Initialise information about your network interfaces.
-        
-        ```python
-        from p2pd import *
-        netifaces = await init_p2pd() # Same API as netifaces
-        ```
-        
-        Load default interface and load details about it's NAT.
-        
-        ```python
-        i = await Interface(netifaces=netifaces)
-        await i.load_nat()
-        ```
-        
-        Choose an external address to use for an endpoint.
-        Resolve the address of an echo server.
-        
-        ```python
-        route = await i.route().bind()
-        dest = await Address("p2pd.net", 7, route)
-        ```
-        
-        Build an async UDP pipe to the server.
-        
-        ```python
-        pipe = await pipe_open(UDP, dest, route)
-        pipe.subscribe()
-        ```
-        
-        Do some I/O on the pipe and cleanup.
-        
-        ```python
-        # UDP so may not arrive.
-        await pipe.send(b"some message", dest_tup)
-        out = await pipe.recv(timeout=2)
-        print(out)
-        ```
-        
-        ## P2P networking
-        
-        How about an example that does P2P networking?
-        
-        ```python
-        from p2pd import *
-        
-        # Put your custom protocol code here.
-        async def custom_protocol(msg, client_tup, pipe):
-            # E.G. add a ping feature to your protocol.
-            if b"PING" in msg:
-                await pipe.send(b"PONG")
-        
-        async def make_p2p_con():
-            # Initalize p2pd.
-            netifaces = await init_p2pd()
-            #
-            # Start our main node server.
-            # The node implements your protocol.
-            node = await start_p2p_node(netifaces=netifaces)
-            node.add_msg_cb(custom_protocol)
-            #
-            # Spawn a new pipe from a P2P con.
-            # Connect to our own node server.
-            pipe = await node.connect(node.addr_bytes)
-            pipe.subscribe(SUB_ALL)
-            #
-            # Test send / receive.
-            msg = b"test send"
-            await pipe.send(b"ECHO " + msg)
-            out = await pipe.recv()
-            #
-            # Cleanup.
-            assert(msg in out)
-            await pipe.close()
-            await node.close()
-        
-        # Run the coroutine.
-        # Or await make_p2p_con() if in async REPL.
-        async_test(make_p2p_con)
-        ```
-        
-        In this example the node connects to itself but it could just as easily be used to connect to another peer.
-        
-        ## Features
-        
-        **P2PD** is a new project aiming to make peer-to-peer networking
-        simple and ubiquitous. P2PD can be used either as a library or as a service.
-        As a library P2PD is written in Python 3 using asyncio for everything.
-        As a service P2PD provides a REST API on http://127.0.0.1:12333/.
-        The REST API is provided for non-Python languages.
-        
-        P2PD offers engineers the following features:
-        
-        - Multiple strategies for establishing peer-to-peer direct connections.
-        
-          - **Direct connect** = Connect to a reachable node.
-          - **Reverse connect** = Tell a node to connect to you.
-          - **TCP hole punching** = Simultaneous TCP connections.
-          - **TURN** = Use a proxy server as a last resort.
-        - **Advanced NAT detection.** P2PD can detect 7 different types of NATs and
-           5 different sub-types for a combined total of **35 unique NAT
-           configurations.** The result is better NAT bypass.
-        - **Smart TCP hole punching.** The TCP hole punching algorithm has been
-           designed to require minimal communication between peers to increase
-           the chances of success. The algorithm supports a diverse number of
-           NAT configurations for the best results possible.
-        - **Port forwarding (IPv4) and pin hole (IPv6.)** Automatically
-           handles openning ports on the router to increase reachability.
-        - **IPv6 ready from day 1.** Supports IPv4 and IPv6. Introduces a new
-           format for addresses that offers insight into a peer's
-           NIC cards, internal network, and NAT devices.
-        - **A new way to do network programming.** Focuses on NICs as the
-           starting point for building services. Introduces 'routes' as a
-           way to provide visibility into external addresses. You can build
-           services that support IPv4, IPv6, TCP, and UDP without writing
-           different code for each of them.
-        - **Language-agnostic REST API.** You can call **/p2p/open/name/addr**
-           then **/p2p/pipe/name** to turn any HTTP connection into a two-way relay
-           between a peer-to-peer connection.
-        - **Minimal dependencies.** Most of the code in P2PD uses the Python
-          standard library to improve portability and reduce packaging issues.
-        - **Built on open protocols.** P2PD uses **STUN** for address lookups,
-           **MQTT** for signaling messages, and **TURN** for last resort proxying.
-           All of these protocols have public infrastructure.
-        
-        Learn how to use the software:
-        https://p2pd.readthedocs.io/
-        
 Keywords: NAT traversal,TCP hole punching,simultaneous open,UPnP,STUN,TURN,SIP,DHCP,add IP to interface,NATPMP,P2P,Peer-to-peer networking library,python
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# P2PD
+
+``[Coverage >= 82%] [Python >= 3.6] [Mac, Win, Nix, BSD, Android]``
+
+**P2PD** is a new async networking library for Python. It's based on solving some of the problems with Python's existing APIs and supports P2P networking among other features.
+
+Let's look at some examples.
+Start the Python REPL with await support with:
+
+> python3 -m asyncio
+
+Initialise information about your network interfaces.
+
+```python
+from p2pd import *
+netifaces = await init_p2pd() # Same API as netifaces
+```
+
+Load default interface and load details about it's NAT.
+
+```python
+i = await Interface(netifaces=netifaces)
+await i.load_nat()
+```
+
+Choose an external address to use for an endpoint.
+Resolve the address of an echo server.
+
+```python
+route = await i.route().bind()
+dest = await Address("p2pd.net", 7, route)
+```
+
+Build an async UDP pipe to the server.
+
+```python
+pipe = await pipe_open(UDP, dest, route)
+pipe.subscribe()
+```
+
+Do some I/O on the pipe and cleanup.
+
+```python
+# UDP so may not arrive.
+await pipe.send(b"some message", dest_tup)
+out = await pipe.recv(timeout=2)
+print(out)
+```
+
+## P2P networking
+
+How about an example that does P2P networking?
+
+```python
+from p2pd import *
+
+# Put your custom protocol code here.
+async def custom_protocol(msg, client_tup, pipe):
+    # E.G. add a ping feature to your protocol.
+    if b"PING" in msg:
+        await pipe.send(b"PONG")
+
+async def make_p2p_con():
+    # Initalize p2pd.
+    netifaces = await init_p2pd()
+    #
+    # Start our main node server.
+    # The node implements your protocol.
+    node = await start_p2p_node(netifaces=netifaces)
+    node.add_msg_cb(custom_protocol)
+    #
+    # Spawn a new pipe from a P2P con.
+    # Connect to our own node server.
+    pipe = await node.connect(node.addr_bytes)
+    pipe.subscribe(SUB_ALL)
+    #
+    # Test send / receive.
+    msg = b"test send"
+    await pipe.send(b"ECHO " + msg)
+    out = await pipe.recv()
+    #
+    # Cleanup.
+    assert(msg in out)
+    await pipe.close()
+    await node.close()
+
+# Run the coroutine.
+# Or await make_p2p_con() if in async REPL.
+async_test(make_p2p_con)
+```
+
+In this example the node connects to itself but it could just as easily be used to connect to another peer.
+
+## Features
+
+**P2PD** is a new project aiming to make peer-to-peer networking
+simple and ubiquitous. P2PD can be used either as a library or as a service.
+As a library P2PD is written in Python 3 using asyncio for everything.
+As a service P2PD provides a REST API on http://127.0.0.1:12333/.
+The REST API is provided for non-Python languages.
+
+P2PD offers engineers the following features:
+
+- Multiple strategies for establishing peer-to-peer direct connections.
+
+  - **Direct connect** = Connect to a reachable node.
+  - **Reverse connect** = Tell a node to connect to you.
+  - **TCP hole punching** = Simultaneous TCP connections.
+  - **TURN** = Use a proxy server as a last resort.
+- **Advanced NAT detection.** P2PD can detect 7 different types of NATs and
+   5 different sub-types for a combined total of **35 unique NAT
+   configurations.** The result is better NAT bypass.
+- **Smart TCP hole punching.** The TCP hole punching algorithm has been
+   designed to require minimal communication between peers to increase
+   the chances of success. The algorithm supports a diverse number of
+   NAT configurations for the best results possible.
+- **Port forwarding (IPv4) and pin hole (IPv6.)** Automatically
+   handles openning ports on the router to increase reachability.
+- **IPv6 ready from day 1.** Supports IPv4 and IPv6. Introduces a new
+   format for addresses that offers insight into a peer's
+   NIC cards, internal network, and NAT devices.
+- **A new way to do network programming.** Focuses on NICs as the
+   starting point for building services. Introduces 'routes' as a
+   way to provide visibility into external addresses. You can build
+   services that support IPv4, IPv6, TCP, and UDP without writing
+   different code for each of them.
+- **Language-agnostic REST API.** You can call **/p2p/open/name/addr**
+   then **/p2p/pipe/name** to turn any HTTP connection into a two-way relay
+   between a peer-to-peer connection.
+- **Minimal dependencies.** Most of the code in P2PD uses the Python
+  standard library to improve portability and reduce packaging issues.
+- **Built on open protocols.** P2PD uses **STUN** for address lookups,
+   **MQTT** for signaling messages, and **TURN** for last resort proxying.
+   All of these protocols have public infrastructure.
+
+Learn how to use the software:
+https://p2pd.readthedocs.io/
```

### Comparing `p2pd-2.3.5/setup.py` & `p2pd-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     install_reqs = f.read().splitlines()
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
-    version='2.3.5',
+    version='2.3.6',
     name='p2pd',
     description='Asynchronous P2P networking library and service',
     keywords=('NAT traversal, TCP hole punching, simultaneous open, UPnP, STUN, TURN, SIP, DHCP, add IP to interface, NATPMP, P2P, Peer-to-peer networking library, python'),
     long_description_content_type="text/markdown",
     long_description=long_description,
     url='http://github.com/robertsdotpm/p2pd',
     author='Matthew Roberts',
```

