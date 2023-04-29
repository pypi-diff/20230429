# Comparing `tmp/IPFS-Toolkit-0.5.4.tar.gz` & `tmp/IPFS-Toolkit-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPFS-Toolkit-0.5.4.tar", last modified: Sun Apr 23 14:23:51 2023, max compression
+gzip compressed data, was "IPFS-Toolkit-0.5.5.tar", last modified: Sat Apr 29 06:23:00 2023, max compression
```

## Comparing `IPFS-Toolkit-0.5.4.tar` & `IPFS-Toolkit-0.5.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/IPFS_API.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/IPFS_DataTransmission.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/IPFS_LNS.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12442 2023-04-23 14:23:50.000000 IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1337 2023-04-23 14:23:51.000000 IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-04-23 14:23:51.000000 IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-04-23 14:23:51.000000 IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/requires.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      105 2023-04-23 14:23:51.000000 IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12442 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/PKG-INFO
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    18423 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfs_api.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    15082 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfs_cli.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74368 2023-04-23 14:13:07.000000 IPFS-Toolkit-0.5.4/ipfs_datatransmission.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfs_lns.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/ipfshttpclient2/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/__init__.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/__init__.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/base.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/bitswap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/block.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/bootstrap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/config.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/dag.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/dht.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/files.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/key.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/miscellaneous.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/name.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/object.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/p2p.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/pin.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/pubsub.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/repo.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6087 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/swarm.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/client/unstable.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/encoding.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/exceptions.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/filescanner.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/http.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/http_common.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/http_httpx.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/http_requests.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/multipart.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/requests_wrapper.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/utils.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/ipfshttpclient2/version.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.4/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/setup.cfg
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1499 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.4/setup.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-23 14:23:51.359877 IPFS-Toolkit-0.5.4/tests/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5235 2023-04-23 14:22:57.000000 IPFS-Toolkit-0.5.4/tests/test_with_docker.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1527 2023-04-23 13:52:09.000000 IPFS-Toolkit-0.5.4/tests/test_without_docker.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/IPFS_API.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/IPFS_DataTransmission.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/IPFS_LNS.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.474612 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1337 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/requires.txt
+-rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      105 2023-04-29 06:23:00.000000 IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/PKG-INFO
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    17995 2023-04-29 06:15:14.000000 IPFS-Toolkit-0.5.5/ipfs_api.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 05:16:35.000000 IPFS-Toolkit-0.5.5/ipfs_cli.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-23 14:44:42.000000 IPFS-Toolkit-0.5.5/ipfs_datatransmission.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfs_lns.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/ipfshttpclient2/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/__init__.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/__init__.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/base.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bitswap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/block.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bootstrap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/config.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dag.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dht.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/files.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/key.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/miscellaneous.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/name.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/object.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/p2p.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pin.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pubsub.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/repo.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6087 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/swarm.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/client/unstable.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/encoding.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/exceptions.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/filescanner.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http_common.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http_httpx.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/http_requests.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/multipart.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/requests_wrapper.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/utils.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/ipfshttpclient2/version.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.5/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/setup.cfg
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1499 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.5/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-04-29 06:23:00.478612 IPFS-Toolkit-0.5.5/tests/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-29 06:20:36.000000 IPFS-Toolkit-0.5.5/tests/test_with_docker.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-29 06:17:33.000000 IPFS-Toolkit-0.5.5/tests/test_without_docker.py
```

### Comparing `IPFS-Toolkit-0.5.4/IPFS_API.py` & `IPFS-Toolkit-0.5.5/IPFS_API.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/IPFS_DataTransmission.py` & `IPFS-Toolkit-0.5.5/IPFS_DataTransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/IPFS_LNS.py` & `IPFS-Toolkit-0.5.5/IPFS_LNS.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/PKG-INFO` & `IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.4
+Version: 0.5.5
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -117,14 +117,16 @@
 ```Python
 import ipfs_api
 ipfs_api.http_client.add("helloworld.txt")
 ipfs_api.http_client.dht.findpeer("QMHash")
 ipfs_api.http_client.swarm.peers()
 ```
 
+To check and somewhat manage the status of the IPFS daemon, see [Examples/Demo-Check-IPFS-Status.py](Examples/Demo-Check-IPFS-Status.py)
+
 ## IPFS-Datatransmission
 `import ipfs_datatransmission`
 
 A Python module for limitless, easy, private peer-to-peer data transmission other over the IPFS Network.
 
 This module has three main pairs functions for use by the user:
 - __Simple Data Transmission:__
```

### Comparing `IPFS-Toolkit-0.5.4/IPFS_Toolkit.egg-info/SOURCES.txt` & `IPFS-Toolkit-0.5.5/IPFS_Toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/PKG-INFO` & `IPFS-Toolkit-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.4
+Version: 0.5.5
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -117,14 +117,16 @@
 ```Python
 import ipfs_api
 ipfs_api.http_client.add("helloworld.txt")
 ipfs_api.http_client.dht.findpeer("QMHash")
 ipfs_api.http_client.swarm.peers()
 ```
 
+To check and somewhat manage the status of the IPFS daemon, see [Examples/Demo-Check-IPFS-Status.py](Examples/Demo-Check-IPFS-Status.py)
+
 ## IPFS-Datatransmission
 `import ipfs_datatransmission`
 
 A Python module for limitless, easy, private peer-to-peer data transmission other over the IPFS Network.
 
 This module has three main pairs functions for use by the user:
 - __Simple Data Transmission:__
```

### Comparing `IPFS-Toolkit-0.5.4/ipfs_api.py` & `IPFS-Toolkit-0.5.5/ipfs_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # This is a wrapper for the ipfshttpclient module to make it easier to interact with the Interplanetary File System (IPFS)
 # process running on the computer.
 # To use it you must have IPFS running on your computer.
 # This wrapper uses a custom updated version of the ipfshttpclient.
 
 
+import time
+from threading import Event
 import shutil
 import tempfile
 # import sys
 from subprocess import Popen, PIPE
 # import subprocess
 import os
 import os.path
@@ -26,49 +28,18 @@
 except Exception as e:
     print(str(e))
     LIBERROR = True
     http_client = None
     ipfshttpclient = None
 print_log = False
 
-autostart = True
-started = False
 # List for keeping track of subscriptions to IPFS topics, so that subscriptions can be ended
 subscriptions = list([])
 
 
-def _start():
-    try:
-        global http_client
-        global started
-        from ipfs_cli import run_command, ipfs_cmd
-        Thread(target=run_command, args=[
-               ipfs_cmd, "daemon", "--enable-pubsub-experiment"])
-
-        http_client = ipfshttpclient.connect('/ip4/127.0.0.1/tcp/5001/http')
-        started = True
-        logging.info("Started ipfs_api, connected to daemon")
-        return True
-    except Exception as e:
-        logging.warning("could not connect to daemon")
-        logging.debug(traceback.format_exc())
-        if print_log:
-            print("")
-            print("----------------------------------------------------")
-            traceback.print_exc()  # printing stack trace
-            print("----------------------------------------------------")
-            print("")
-            print(type(e))
-            if(str(e).startswith("ConnectionError: HTTPConnectionPool")):
-                print("Failed to connect to the IPFS process on this machine.")
-                print("Is IPFS running?")
-                print("Is it listening on '/ip4/127.0.0.1/tcp/5001/http'?")
-                return "IPFS not running"
-
-
 def publish(path: str):
     """Upload a file or a directory to IPFS, returning its CID.
     Args:
         path (str): the path of the file to publish
     Returns:
         str: the IPFS content ID (CID) of the published file
     """
@@ -106,23 +77,23 @@
     Returns:
         str: the content of the specified IPFS resource as text
     """
     return http_client.cat(cid)
 
 
 def pin(cid: str):
-    """Ensure the specified IPFS resource remains available on this IPFS node.    
+    """Ensure the specified IPFS resource remains available on this IPFS node.
     Args:
         cid (str): the IPFS content ID (CID) of the resource to pin
     """
     http_client.pin.add(cid)
 
 
 def unpin(cid: str):
-    """Allow a pinned IPFS resource to be garbage-collected and removed on this IPFS node.    
+    """Allow a pinned IPFS resource to be garbage-collected and removed on this IPFS node.
     Args:
         cid (str): the IPFS content ID (CID) of the resource to unpin
     """
     http_client.pin.rm(cid)
 
 
 def create_ipns_record(name: str, type: str = "rsa", size: int = 2048):
@@ -205,14 +176,30 @@
     """Returns this IPFS node's peer ID.
     Returns:
         str: the peer ID of this node
     """
     return http_client.id().get("ID")
 
 
+def is_ipfs_running():
+    """Checks whether or not the IPFS daemon is currently running.
+    Returns:
+        bool: whether or not the IPFS daemon is currently running
+    """
+    return len(my_multiaddrs()) > 0
+
+
+def my_multiaddrs():
+    """Returns this IPFS node's peer ID.
+    Returns:
+        str: the peer ID of this node
+    """
+    return http_client.id().get("Addresses")
+
+
 def list_peer_multiaddrs():
     """Returns a list of the IPFS multiaddresses of the other nodes
     this node is connected to.
     Returns:
         list(str): a list of the IPFS multiaddresses of the other nodes
         this node is connected to
     """
@@ -282,16 +269,16 @@
     to the specified peer via this connection.
     Args:
         name (str): the name of the connection (starts with /x/)
         port (int): the local TCP port number from which to forward traffic
     """
     if name[:3] != "/x/":
         name = "/x/" + name
-    http_client.p2p.forward(name, "/ip4/127.0.0.1/tcp/" +
-                            str(port), "/p2p/" + peerID)
+    http_client.p2p.forward(name, "/ip4/127.0.0.1/tcp/"
+                            + str(port), "/p2p/" + peerID)
 
 
 def close_all_tcp_connections(listeners_only=False):
     """Close all libp2p stream-mounting (IPFS port-forwarding) connections.
     Args:
         listeners_only (bool): if set to True, only listening connections are closed
     """
@@ -483,16 +470,29 @@
     data = urlsafe_b64encode(data)
     while data[-1] == 61 and data[-1]:
         data = data[:-1]
     data = b'u' + data
     return data
 
 
-if autostart:
-    if not LIBERROR:    # if all modules needed for the ipfs_http_client library were loaded
-        _start()
-    if not started:
-        from ipfs_cli import is_daemon_running, run_daemon
-        from ipfs_cli import *
-        print("Using IPFS CLI because our HTTP client isn't working.")
-        if not is_daemon_running():
-            run_daemon()
+def wait_till_ipfs_is_running(timeout_sec=None):
+    count = 0
+    while True:
+        try:
+            if is_ipfs_running():
+                return
+        except ipfshttpclient.exceptions.ConnectionError as error:
+            pass
+        time.sleep(1)
+        count += 1
+        if timeout_sec and count == timeout_sec:
+            raise TimeoutError()
+
+
+def try_run_ipfs():
+    from ipfs_cli import try_run_ipfs as _try_run_ipfs
+    _try_run_ipfs()
+
+
+if LIBERROR:    # if not all modules needed for the ipfs_http_client library were loaded
+    print("Falling back to IPFS CLI because our HTTP client isn't working;\nNot all modules required by the http-connection could be loaded.")
+    from ipfs_cli import *
```

### Comparing `IPFS-Toolkit-0.5.4/ipfs_cli.py` & `IPFS-Toolkit-0.5.5/ipfs_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,37 +44,26 @@
 
 ipfs_cmd = "ipfs"
 if not run_command([ipfs_cmd]):
     if bool(run_command("./ipfs")):
         ipfs_cmd = "./ipfs"
 
 
-def is_daemon_running():
-    try:
-        proc = Popen([ipfs_cmd, "swarm", "peers"], stdout=PIPE, stderr=PIPE)
-
-        proc.wait()
-        if proc.stderr.readline():
-            return False
-        else:
-            return True
-    except:
-        return
+def is_ipfs_running():
+    return len(my_multiaddrs()) > 0
 
 
-def run_daemon():
-    try:
-        proc = Popen([ipfs_cmd, "daemon", "--enable-pubsub-experiment"],
-                     stdout=PIPE, stdin=PIPE)
-        while True:
-            data = proc.stdout.read1().decode()
-            if data.strip("\n") == "Daemon is ready" or is_daemon_running():
-                return True
-    except:
-        return
+def try_run_ipfs():
+    print("Starting IPFS...")
+    proc = Popen([ipfs_cmd, "daemon", "--enable-pubsub-experiment"],
+                 stdout=PIPE, stdin=PIPE)
+    while True:
+        data = proc.stdout.read1().decode()
+        if data.strip("\n") == "Daemon is ready":
+            return True
 
 
 def download_ipfs_binary(downloading_callback=None):
     global found_ipfs
     global ipfs_cmd
     if not run_command([ipfs_cmd]):
         if bool(run_command("./ipfs")):
@@ -112,15 +101,15 @@
         # init ipfs
         if not run_command([ipfs_cmd, "id"]):
             run_command([ipfs_cmd, "init"])
         # configure ipfs
         run_command(
             [ipfs_cmd, "config", "--json Experimental.Libp2pStreamMounting", "true"])
         # run ipfs
-        run_daemon()
+        try_run_ipfs()
 
 
 found_ipfs = bool(run_command([ipfs_cmd]))
 
 
 if found_ipfs:
     if not run_command([ipfs_cmd, "id"]):
@@ -168,21 +157,23 @@
 
     def _listen(self):
         if self.__listening:
             return
         self.__listening = True
         """blocks the calling thread"""
         while not self._terminate:
-            proc = Popen([ipfs_cmd, "pubsub", "sub", self.topic],
-                         stdout=PIPE, stdin=PIPE)
+            self.proc = Popen([ipfs_cmd, "pubsub", "sub", self.topic],
+                              stdout=PIPE, stdin=PIPE)
             while True:
                 data = {
                     "senderID": "",
-                    "data": proc.stdout.read1(),
+                    "data": self.proc.stdout.read1(),
                 }
+                if self._terminate:
+                    return
                 Thread(target=self.eventhandler, args=(data,)).start()
         self.__listening = False
 
     def __decode_base64_url(self, data: str):
         """Performs the URL-Safe multibase decoding required by the new pubsub function (since IFPS v0.11.0) on strings"""
         # print(data)
         data = str(data)[1:].encode()
@@ -191,20 +182,21 @@
             data += b'=' * (4 - missing_padding)
         # print(data.decode())
         # print(urlsafe_b64decode(data))
         return urlsafe_b64decode(data)
 
     def listen(self):
         self._terminate = False
-        thr = Thread(target=self._listen, args=())
+        thr = Thread(target=self._listen, args=(), name=f"ipfs_cli.pubsub_listener {self.topic}")
         thr.start()
 
     def terminate(self):
         """May let one more pubsub message through"""
         self._terminate = True
+        pubsub_publish(self.topic, "terminate".encode())
 
 
 def pubsub_subscribe(topic, eventhandler):
     """
     Listens to the specified IPFS PubSub topic, calling the eventhandler
     whenever a message is received, passing the message data and its sender
     to the evventhandler.
@@ -215,25 +207,14 @@
                             except when using an older version of IPFS < v0.11.0,
                             in which case only the message is passed as a string.
     Returns a PubsubListener object which can  be terminated with the .terminate() method (and restarted with the .listen() method)
     """
     return PubsubListener(topic, eventhandler)
 
 
-def pubsub_unsubscribe(topic, eventhandler):
-    index = 0
-    for subscription in subscriptions:
-        if(subscription[0] == topic and subscription[1] == eventhandler):
-            subscription[2].terminate()
-            break
-        index = index + 1
-    # remove the subscription from the list of subscriptions
-    subscriptions.pop(index)
-
-
 def publish(path: str):
     """
     upload a file or a directory to IPFS.
     Returns the Hash of the uploaded file.
     """
     result = run_command([ipfs_cmd, "add", "-r", path]).split("\n")
     while result[-1] == "":
@@ -328,14 +309,22 @@
 # Returns the IPFS ID of the currently running IPFS node
 
 
 def my_id():
     return json.loads(run_command([ipfs_cmd, "id"])).get("ID")
 
 
+def my_multiaddrs():
+    multi_addrs = json.loads(run_command([ipfs_cmd, "id"])).get("Addresses")
+    if multi_addrs:
+        return multi_addrs
+    else:
+        return []
+
+
 myid = my_id
 
 
 def create_tcp_listening_connection(name, port):
     run_command([ipfs_cmd, "p2p", "listen", "/x/" +
                  name, "/ip4/127.0.0.1/tcp/" + str(port)])
```

### Comparing `IPFS-Toolkit-0.5.4/ipfs_datatransmission.py` & `IPFS-Toolkit-0.5.5/ipfs_datatransmission.py`

 * *Files 0% similar despite different names*

```diff
@@ -721,15 +721,15 @@
             return
         if not timeout:
             data = self.message_queue.get()
         else:
             try:
                 data = self.message_queue.get(timeout=timeout)
             except:  # timeout reached
-                raise ConvListenTimeout("Didn't receive any data.")
+                raise ConvListenTimeout("Didn't receive any data.") from None
 
         if data:
             return data
         else:
             if PRINT_LOG_CONVERSATIONS:
                 print("Conv.listen: received nothing restarting Event Wait")
             self.listen()
@@ -780,18 +780,18 @@
                     timeout = min(_no_coms_timeout, _abs_timeout)
                 try:
                     data = self._file_queue.get(timeout=timeout)
                     break
                 except QueueEmpty:  # qeue timeout reached
                     # check if any of the user's timeouts were reached
                     if abs_timeout and (datetime.utcnow() - start_time).total_seconds() > abs_timeout:
-                        raise ConvListenTimeout("Didn't receive any files.")
+                        raise ConvListenTimeout("Didn't receive any files.") from None
                     elif (datetime.utcnow() - self._last_coms_time).total_seconds() > no_coms_timeout:
                         raise CommunicationTimeout(
-                            "Communication timeout reached while waiting for file.")
+                            "Communication timeout reached while waiting for file.") from None
         if data:
             return data
         else:
             if PRINT_LOG_CONVERSATIONS:
                 print("Conv.FileListen: received nothign restarting Event Wait")
             self.listen_for_file(timeout)
```

### Comparing `IPFS-Toolkit-0.5.4/ipfs_lns.py` & `IPFS-Toolkit-0.5.5/ipfs_lns.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/__init__.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/__init__.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/base.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/base.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/bitswap.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bitswap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/block.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/block.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/bootstrap.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/bootstrap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/config.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/config.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/dag.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dag.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/dht.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/dht.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/files.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/files.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/key.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/key.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/miscellaneous.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/name.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/name.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/object.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/object.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/p2p.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/p2p.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/pin.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pin.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/pubsub.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/pubsub.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/repo.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/repo.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/swarm.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/swarm.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/client/unstable.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/client/unstable.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/encoding.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/encoding.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/exceptions.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/exceptions.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/filescanner.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/filescanner.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/http.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/http.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/http_common.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/http_common.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/http_httpx.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/http_httpx.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/http_requests.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/http_requests.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/multipart.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/multipart.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/requests_wrapper.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/utils.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/utils.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/ipfshttpclient2/version.py` & `IPFS-Toolkit-0.5.5/ipfshttpclient2/version.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/setup.py` & `IPFS-Toolkit-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.4/tests/test_with_docker.py` & `IPFS-Toolkit-0.5.5/tests/test_with_docker.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,32 +28,37 @@
 import threading
 
 # time in seconds to wait for file to transmit before calling test a failure
 FILE_SEND_TIMEOUT = 20
 
 TEST_CLI = False
 
+
 # if you do not have any other important brenthydrive docker containers,
 # you can set this to true to automatically remove unpurged docker containers
 # after failed tests
-DELETE_ALL_BRENTHY_DOCKERS = True
-
+DELETE_ALL_IPFS_DOCKERS = True
+REBUILD_DOCKER = True
 
 if os.path.exists("testfile"):
     file_path = "testfile"
 else:
     file_path = input("Enter filepath for test transmission file (~10MB): ")
 
-if DELETE_ALL_BRENTHY_DOCKERS:
+if DELETE_ALL_IPFS_DOCKERS:
     try:
         os.system("docker stop $(docker ps --filter 'ancestor=emendir/ipfs-toolkit' -aq)  >/dev/null 2>&1; docker rm $(docker ps --filter 'ancestor=emendir/ipfs-toolkit' -aq)  >/dev/null 2>&1")
     except:
         pass
 
 
+if REBUILD_DOCKER:
+    from build_docker import build_docker
+    build_docker(verbose=False)
+
 if True:
     sys.path.insert(0, "..")
     if TEST_CLI:
         import ipfs_cli as ipfs_api
     else:
         import ipfs_api
     import ipfs_datatransmission
```

### Comparing `IPFS-Toolkit-0.5.4/tests/test_without_docker.py` & `IPFS-Toolkit-0.5.5/tests/test_without_docker.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,23 @@
     received_msg = bytearray()
 
     def on_pubsub_received(data):
         nonlocal received_msg
         received_msg = data["data"]
     sub = ipfs_api.pubsub_subscribe("autotest", on_pubsub_received)
     ipfs_api.pubsub_publish("autotest", "Hello there!".encode())
-    time.sleep(3)
+    time.sleep(5)
     success = received_msg.decode() == "Hello there!"
+
     print(mark(success), "PubSub communication")
     term_start = datetime.utcnow()
     sub.terminate()
     term_end = datetime.utcnow()
     term_dur = (term_end - term_start).total_seconds()
+    time.sleep(30)
     success = len(threading.enumerate()) == 1
     print(mark(success), f"PubSub thread cleanup {term_dur}s")
     if not success:
         [print(x) for x in threading.enumerate()]
 
 
 if __name__ == "__main__":
```

