# Comparing `tmp/pyHanko-0.8.0.tar.gz` & `tmp/pyHanko-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyHanko-0.8.0.tar", last modified: Mon Aug 23 20:51:40 2021, max compression
+gzip compressed data, was "pyHanko-0.9.0.tar", last modified: Sat Oct 30 23:34:59 2021, max compression
```

## Comparing `pyHanko-0.8.0.tar` & `pyHanko-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,73 @@
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.681292 pyHanko-0.8.0/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1076 2021-02-06 19:48:30.000000 pyHanko-0.8.0/LICENSE
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5508 2021-08-23 20:51:40.681292 pyHanko-0.8.0/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3880 2021-07-25 14:15:11.000000 pyHanko-0.8.0/README.md
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.677959 pyHanko-0.8.0/pyHanko.egg-info/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5508 2021-08-23 20:51:40.000000 pyHanko-0.8.0/pyHanko.egg-info/PKG-INFO
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1541 2021-08-23 20:51:40.000000 pyHanko-0.8.0/pyHanko.egg-info/SOURCES.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2021-08-23 20:51:40.000000 pyHanko-0.8.0/pyHanko.egg-info/dependency_links.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)       53 2021-08-23 20:51:40.000000 pyHanko-0.8.0/pyHanko.egg-info/entry_points.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)      320 2021-08-23 20:51:40.000000 pyHanko-0.8.0/pyHanko.egg-info/requires.txt
--rw-r--r--   0 matthias  (1000) matthias  (1000)        8 2021-08-23 20:51:40.000000 pyHanko-0.8.0/pyHanko.egg-info/top_level.txt
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.677959 pyHanko-0.8.0/pyhanko/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       98 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      121 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/__main__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    51209 2021-08-23 20:46:44.000000 pyHanko-0.8.0/pyhanko/cli.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    16943 2021-08-23 20:03:33.000000 pyHanko-0.8.0/pyhanko/config.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.677959 pyHanko-0.8.0/pyhanko/pdf_utils/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/pdf_utils/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3543 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/pdf_utils/_saslprep.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3368 2021-04-17 16:00:31.000000 pyHanko-0.8.0/pyhanko/pdf_utils/barcodes.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8908 2021-08-22 16:11:03.000000 pyHanko-0.8.0/pyhanko/pdf_utils/config_utils.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8095 2021-06-30 23:15:30.000000 pyHanko-0.8.0/pyhanko/pdf_utils/content.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)   100734 2021-08-20 09:42:56.000000 pyHanko-0.8.0/pyhanko/pdf_utils/crypt.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17191 2021-07-23 22:04:57.000000 pyHanko-0.8.0/pyhanko/pdf_utils/embed.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9376 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/pdf_utils/filters.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.677959 pyHanko-0.8.0/pyhanko/pdf_utils/font/
--rw-r--r--   0 matthias  (1000) matthias  (1000)      240 2021-06-16 21:31:05.000000 pyHanko-0.8.0/pyhanko/pdf_utils/font/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     3749 2021-06-16 21:45:38.000000 pyHanko-0.8.0/pyhanko/pdf_utils/font/api.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1779 2021-06-16 21:18:31.000000 pyHanko-0.8.0/pyhanko/pdf_utils/font/basic.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    28967 2021-07-19 18:56:35.000000 pyHanko-0.8.0/pyhanko/pdf_utils/font/opentype.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    58268 2021-07-30 20:33:02.000000 pyHanko-0.8.0/pyhanko/pdf_utils/generic.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     6855 2021-06-14 17:26:46.000000 pyHanko-0.8.0/pyhanko/pdf_utils/images.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     9909 2021-08-20 10:05:35.000000 pyHanko-0.8.0/pyhanko/pdf_utils/incremental_writer.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    16683 2021-08-22 15:34:31.000000 pyHanko-0.8.0/pyhanko/pdf_utils/layout.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12108 2021-08-19 21:16:25.000000 pyHanko-0.8.0/pyhanko/pdf_utils/misc.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      977 2021-04-17 15:58:54.000000 pyHanko-0.8.0/pyhanko/pdf_utils/qr.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    61140 2021-08-20 10:28:06.000000 pyHanko-0.8.0/pyhanko/pdf_utils/reader.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5961 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/pdf_utils/rw_common.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     8141 2021-06-16 21:31:05.000000 pyHanko-0.8.0/pyhanko/pdf_utils/text.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    53964 2021-08-20 10:05:35.000000 pyHanko-0.8.0/pyhanko/pdf_utils/writer.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.681292 pyHanko-0.8.0/pyhanko/sign/
--rw-r--r--   0 matthias  (1000) matthias  (1000)       22 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/sign/__init__.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.681292 pyHanko-0.8.0/pyhanko/sign/ades/
--rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/sign/ades/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2930 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/sign/ades/api.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)      485 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/sign/ades/asn1_util.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5040 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/sign/ades/cades_asn1.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1844 2021-04-03 11:08:44.000000 pyHanko-0.8.0/pyhanko/sign/beid.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    85176 2021-07-30 20:51:44.000000 pyHanko-0.8.0/pyhanko/sign/diff_analysis.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    52955 2021-08-22 14:53:38.000000 pyHanko-0.8.0/pyhanko/sign/fields.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    34324 2021-08-22 22:00:07.000000 pyHanko-0.8.0/pyhanko/sign/general.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    12220 2021-08-05 22:00:34.000000 pyHanko-0.8.0/pyhanko/sign/pkcs11.py
-drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-08-23 20:51:40.681292 pyHanko-0.8.0/pyhanko/sign/signers/
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1102 2021-07-05 23:24:36.000000 pyHanko-0.8.0/pyhanko/sign/signers/__init__.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    17059 2021-07-05 23:24:36.000000 pyHanko-0.8.0/pyhanko/sign/signers/cms_embedder.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     1665 2021-07-24 13:23:19.000000 pyHanko-0.8.0/pyhanko/sign/signers/constants.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)     5934 2021-07-21 20:58:18.000000 pyHanko-0.8.0/pyhanko/sign/signers/functions.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    14574 2021-07-05 23:24:36.000000 pyHanko-0.8.0/pyhanko/sign/signers/pdf_byterange.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    35785 2021-08-23 20:03:33.000000 pyHanko-0.8.0/pyhanko/sign/signers/pdf_cms.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    75542 2021-08-20 09:17:31.000000 pyHanko-0.8.0/pyhanko/sign/signers/pdf_signer.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    15439 2021-08-20 09:17:31.000000 pyHanko-0.8.0/pyhanko/sign/timestamps.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    95271 2021-08-22 22:03:12.000000 pyHanko-0.8.0/pyhanko/sign/validation.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)    29821 2021-08-22 15:34:31.000000 pyHanko-0.8.0/pyhanko/stamp.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)       51 2021-08-23 20:36:25.000000 pyHanko-0.8.0/pyhanko/version.py
--rw-r--r--   0 matthias  (1000) matthias  (1000)       38 2021-08-23 20:51:40.681292 pyHanko-0.8.0/setup.cfg
--rw-r--r--   0 matthias  (1000) matthias  (1000)     2647 2021-08-23 20:40:49.000000 pyHanko-0.8.0/setup.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.310082 pyHanko-0.9.0/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1076 2021-02-06 19:48:30.000000 pyHanko-0.9.0/LICENSE
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5748 2021-10-30 23:34:59.310082 pyHanko-0.9.0/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4061 2021-10-30 23:34:32.000000 pyHanko-0.9.0/README.md
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.303415 pyHanko-0.9.0/pyHanko.egg-info/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5748 2021-10-30 23:34:59.000000 pyHanko-0.9.0/pyHanko.egg-info/PKG-INFO
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1773 2021-10-30 23:34:59.000000 pyHanko-0.9.0/pyHanko.egg-info/SOURCES.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        1 2021-10-30 23:34:59.000000 pyHanko-0.9.0/pyHanko.egg-info/dependency_links.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       53 2021-10-30 23:34:59.000000 pyHanko-0.9.0/pyHanko.egg-info/entry_points.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      349 2021-10-30 23:34:59.000000 pyHanko-0.9.0/pyHanko.egg-info/requires.txt
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        8 2021-10-30 23:34:59.000000 pyHanko-0.9.0/pyHanko.egg-info/top_level.txt
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.303415 pyHanko-0.9.0/pyhanko/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       98 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      121 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/__main__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    53089 2021-10-23 10:09:03.000000 pyHanko-0.9.0/pyhanko/cli.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    19547 2021-10-06 20:44:30.000000 pyHanko-0.9.0/pyhanko/config.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.306748 pyHanko-0.9.0/pyhanko/pdf_utils/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3543 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/_saslprep.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3368 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/barcodes.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8909 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/config_utils.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8107 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/content.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)   100743 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/crypt.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17191 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/embed.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9375 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/filters.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.306748 pyHanko-0.9.0/pyhanko/pdf_utils/font/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      240 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/font/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3748 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/font/api.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1780 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/font/basic.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    29504 2021-10-05 22:00:41.000000 pyHanko-0.9.0/pyhanko/pdf_utils/font/opentype.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    58692 2021-10-26 20:05:07.000000 pyHanko-0.9.0/pyhanko/pdf_utils/generic.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6854 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/images.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     9907 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/incremental_writer.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    16683 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/layout.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    12108 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/misc.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      977 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/qr.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    61509 2021-10-30 16:09:21.000000 pyHanko-0.9.0/pyhanko/pdf_utils/reader.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     6172 2021-10-30 15:39:27.000000 pyHanko-0.9.0/pyhanko/pdf_utils/rw_common.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8132 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/text.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    54738 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/pdf_utils/writer.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.306748 pyHanko-0.9.0/pyhanko/sign/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       22 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/__init__.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.306748 pyHanko-0.9.0/pyhanko/sign/ades/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)        0 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/ades/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3444 2021-10-23 10:09:03.000000 pyHanko-0.9.0/pyhanko/sign/ades/api.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      485 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/ades/asn1_util.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5041 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/ades/cades_asn1.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     4568 2021-10-30 08:51:35.000000 pyHanko-0.9.0/pyhanko/sign/attributes.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1900 2021-10-29 21:06:08.000000 pyHanko-0.9.0/pyhanko/sign/beid.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    87032 2021-10-30 16:08:58.000000 pyHanko-0.9.0/pyhanko/sign/diff_analysis.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    53239 2021-10-30 16:53:48.000000 pyHanko-0.9.0/pyhanko/sign/fields.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    34581 2021-10-23 10:09:03.000000 pyHanko-0.9.0/pyhanko/sign/general.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    18724 2021-10-29 21:06:08.000000 pyHanko-0.9.0/pyhanko/sign/pkcs11.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.310082 pyHanko-0.9.0/pyhanko/sign/signers/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1155 2021-10-23 10:09:03.000000 pyHanko-0.9.0/pyhanko/sign/signers/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    17071 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/signers/cms_embedder.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     1664 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/signers/constants.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     8365 2021-10-23 10:09:03.000000 pyHanko-0.9.0/pyhanko/sign/signers/functions.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    14548 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/sign/signers/pdf_byterange.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    53841 2021-10-30 09:38:49.000000 pyHanko-0.9.0/pyhanko/sign/signers/pdf_cms.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    91982 2021-10-30 09:54:59.000000 pyHanko-0.9.0/pyhanko/sign/signers/pdf_signer.py
+drwxr-xr-x   0 matthias  (1000) matthias  (1000)        0 2021-10-30 23:34:59.310082 pyHanko-0.9.0/pyhanko/sign/timestamps/
+-rw-r--r--   0 matthias  (1000) matthias  (1000)      320 2021-10-25 22:22:43.000000 pyHanko-0.9.0/pyhanko/sign/timestamps/__init__.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     3256 2021-10-23 10:09:03.000000 pyHanko-0.9.0/pyhanko/sign/timestamps/aiohttp_client.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     7274 2021-10-25 22:19:59.000000 pyHanko-0.9.0/pyhanko/sign/timestamps/api.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2617 2021-10-24 21:20:58.000000 pyHanko-0.9.0/pyhanko/sign/timestamps/common_utils.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     5404 2021-10-24 21:31:54.000000 pyHanko-0.9.0/pyhanko/sign/timestamps/dummy_client.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2138 2021-10-25 22:22:43.000000 pyHanko-0.9.0/pyhanko/sign/timestamps/requests_client.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)   110079 2021-10-30 09:47:26.000000 pyHanko-0.9.0/pyhanko/sign/validation.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)    29774 2021-09-12 21:23:10.000000 pyHanko-0.9.0/pyhanko/stamp.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       51 2021-10-30 23:34:32.000000 pyHanko-0.9.0/pyhanko/version.py
+-rw-r--r--   0 matthias  (1000) matthias  (1000)       38 2021-10-30 23:34:59.310082 pyHanko-0.9.0/setup.cfg
+-rw-r--r--   0 matthias  (1000) matthias  (1000)     2759 2021-10-30 22:42:48.000000 pyHanko-0.9.0/setup.py
```

### Comparing `pyHanko-0.8.0/LICENSE` & `pyHanko-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyHanko-0.8.0/PKG-INFO` & `pyHanko-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHanko
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools for stamping and signing PDF files
 Home-page: https://github.com/MatthiasValvekens/pyHanko
 Author: Matthias Valvekens
 Author-email: dev@mvalvekens.be
 License: MIT
 Description: ![pyHanko](docs/images/pyhanko-logo.svg)
         
@@ -29,37 +29,41 @@
         ```bash
            pip install 'pyHanko[pkcs11,image-support,opentype]'
         ```
         
         This `pip` invocation includes the optional dependencies required for PKCS#11, image handling and
         OpenType/TrueType support.
         
+        PyHanko requires Python 3.7 or later. Python 3.10 support is currently incubating (and included in the standard CI test suite).
+        
         
         ### Overview
         The code in this repository functions both as a library and as a command-line tool.
         It's nowhere near complete, but here is a short overview of the features.
         Note that not all of these are necessarily exposed through the CLI.
         
          - Stamping
             - Simple text-based stamps
             - QR stamps
             - Font can be monospaced, or embedded from a TTF/OTF font (requires `[opentype]` optional deps)
          - Document preparation 
             - Add empty signature fields to existing PDFs
             - Add seed values to signature fields, with or without constraints
          - Signing
+            * Option to use async signing API
             - Signatures can be invisible, or with an appearance based on the stamping tools
             - LTV-enabled signatures are supported
                 - PAdES baseline profiles B-B, B-T, B-LT and B-LTA are all supported.
                 - Adobe-style revocation info embedding is also supported.
             - RFC 3161 timestamp server support
             - Support for multiple signatures (all modifications are executed using incremental updates to 
               preserve cryptographic integrity)
-            - Supports both RSA & ECDSA
+            - Supports RSA, DSA and ECDSA
               - RSA padding modes: PKCS#1 v1.5 and RSASSA-PSS
+              - DSA
               - ECDSA curves: anything supported by the `cryptography` library, 
                 see [here](https://cryptography.io/en/latest/hazmat/primitives/asymmetric/ec/#elliptic-curves).
             - PKCS#11 support
                 - Available both from the library and through the CLI
                 - Extra convenience wrapper for Belgian eID cards
             - "Interrupted signing" mode for ease of integration with remote and/or interactive signing
               processes.
@@ -112,7 +116,8 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: extra_pubkey_algs
 Provides-Extra: opentype
 Provides-Extra: image-support
 Provides-Extra: pkcs11
+Provides-Extra: async_http
```

### Comparing `pyHanko-0.8.0/README.md` & `pyHanko-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,37 +21,41 @@
 ```bash
    pip install 'pyHanko[pkcs11,image-support,opentype]'
 ```
 
 This `pip` invocation includes the optional dependencies required for PKCS#11, image handling and
 OpenType/TrueType support.
 
+PyHanko requires Python 3.7 or later. Python 3.10 support is currently incubating (and included in the standard CI test suite).
+
 
 ### Overview
 The code in this repository functions both as a library and as a command-line tool.
 It's nowhere near complete, but here is a short overview of the features.
 Note that not all of these are necessarily exposed through the CLI.
 
  - Stamping
     - Simple text-based stamps
     - QR stamps
     - Font can be monospaced, or embedded from a TTF/OTF font (requires `[opentype]` optional deps)
  - Document preparation 
     - Add empty signature fields to existing PDFs
     - Add seed values to signature fields, with or without constraints
  - Signing
+    * Option to use async signing API
     - Signatures can be invisible, or with an appearance based on the stamping tools
     - LTV-enabled signatures are supported
         - PAdES baseline profiles B-B, B-T, B-LT and B-LTA are all supported.
         - Adobe-style revocation info embedding is also supported.
     - RFC 3161 timestamp server support
     - Support for multiple signatures (all modifications are executed using incremental updates to 
       preserve cryptographic integrity)
-    - Supports both RSA & ECDSA
+    - Supports RSA, DSA and ECDSA
       - RSA padding modes: PKCS#1 v1.5 and RSASSA-PSS
+      - DSA
       - ECDSA curves: anything supported by the `cryptography` library, 
         see [here](https://cryptography.io/en/latest/hazmat/primitives/asymmetric/ec/#elliptic-curves).
     - PKCS#11 support
         - Available both from the library and through the CLI
         - Extra convenience wrapper for Belgian eID cards
     - "Interrupted signing" mode for ease of integration with remote and/or interactive signing
       processes.
```

### Comparing `pyHanko-0.8.0/pyHanko.egg-info/PKG-INFO` & `pyHanko-0.9.0/pyHanko.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyHanko
-Version: 0.8.0
+Version: 0.9.0
 Summary: Tools for stamping and signing PDF files
 Home-page: https://github.com/MatthiasValvekens/pyHanko
 Author: Matthias Valvekens
 Author-email: dev@mvalvekens.be
 License: MIT
 Description: ![pyHanko](docs/images/pyhanko-logo.svg)
         
@@ -29,37 +29,41 @@
         ```bash
            pip install 'pyHanko[pkcs11,image-support,opentype]'
         ```
         
         This `pip` invocation includes the optional dependencies required for PKCS#11, image handling and
         OpenType/TrueType support.
         
+        PyHanko requires Python 3.7 or later. Python 3.10 support is currently incubating (and included in the standard CI test suite).
+        
         
         ### Overview
         The code in this repository functions both as a library and as a command-line tool.
         It's nowhere near complete, but here is a short overview of the features.
         Note that not all of these are necessarily exposed through the CLI.
         
          - Stamping
             - Simple text-based stamps
             - QR stamps
             - Font can be monospaced, or embedded from a TTF/OTF font (requires `[opentype]` optional deps)
          - Document preparation 
             - Add empty signature fields to existing PDFs
             - Add seed values to signature fields, with or without constraints
          - Signing
+            * Option to use async signing API
             - Signatures can be invisible, or with an appearance based on the stamping tools
             - LTV-enabled signatures are supported
                 - PAdES baseline profiles B-B, B-T, B-LT and B-LTA are all supported.
                 - Adobe-style revocation info embedding is also supported.
             - RFC 3161 timestamp server support
             - Support for multiple signatures (all modifications are executed using incremental updates to 
               preserve cryptographic integrity)
-            - Supports both RSA & ECDSA
+            - Supports RSA, DSA and ECDSA
               - RSA padding modes: PKCS#1 v1.5 and RSASSA-PSS
+              - DSA
               - ECDSA curves: anything supported by the `cryptography` library, 
                 see [here](https://cryptography.io/en/latest/hazmat/primitives/asymmetric/ec/#elliptic-curves).
             - PKCS#11 support
                 - Available both from the library and through the CLI
                 - Extra convenience wrapper for Belgian eID cards
             - "Interrupted signing" mode for ease of integration with remote and/or interactive signing
               processes.
@@ -112,7 +116,8 @@
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: extra_pubkey_algs
 Provides-Extra: opentype
 Provides-Extra: image-support
 Provides-Extra: pkcs11
+Provides-Extra: async_http
```

### Comparing `pyHanko-0.8.0/pyHanko.egg-info/SOURCES.txt` & `pyHanko-0.9.0/pyHanko.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,25 +32,31 @@
 pyhanko/pdf_utils/text.py
 pyhanko/pdf_utils/writer.py
 pyhanko/pdf_utils/font/__init__.py
 pyhanko/pdf_utils/font/api.py
 pyhanko/pdf_utils/font/basic.py
 pyhanko/pdf_utils/font/opentype.py
 pyhanko/sign/__init__.py
+pyhanko/sign/attributes.py
 pyhanko/sign/beid.py
 pyhanko/sign/diff_analysis.py
 pyhanko/sign/fields.py
 pyhanko/sign/general.py
 pyhanko/sign/pkcs11.py
-pyhanko/sign/timestamps.py
 pyhanko/sign/validation.py
 pyhanko/sign/ades/__init__.py
 pyhanko/sign/ades/api.py
 pyhanko/sign/ades/asn1_util.py
 pyhanko/sign/ades/cades_asn1.py
 pyhanko/sign/signers/__init__.py
 pyhanko/sign/signers/cms_embedder.py
 pyhanko/sign/signers/constants.py
 pyhanko/sign/signers/functions.py
 pyhanko/sign/signers/pdf_byterange.py
 pyhanko/sign/signers/pdf_cms.py
-pyhanko/sign/signers/pdf_signer.py
+pyhanko/sign/signers/pdf_signer.py
+pyhanko/sign/timestamps/__init__.py
+pyhanko/sign/timestamps/aiohttp_client.py
+pyhanko/sign/timestamps/api.py
+pyhanko/sign/timestamps/common_utils.py
+pyhanko/sign/timestamps/dummy_client.py
+pyhanko/sign/timestamps/requests_client.py
```

### Comparing `pyHanko-0.8.0/pyhanko/cli.py` & `pyHanko-0.9.0/pyhanko/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,49 @@
+import asyncio
+import getpass
+import logging
 import sys
 from contextlib import contextmanager
 from datetime import datetime
 from enum import Enum, auto
 
 import click
-import logging
-import getpass
-
 import tzlocal
-from asn1crypto import pem, cms
-
-from pyhanko.pdf_utils.layout import LayoutError
+from asn1crypto import cms, pem
 from pyhanko_certvalidator import ValidationContext
+
+from pyhanko import __version__
 from pyhanko.config import (
-    init_validation_context_kwargs, parse_cli_config,
-    CLIConfig, LogConfig, StdLogOutput, parse_logging_config,
-    PKCS11SignatureConfig, PKCS12SignatureConfig, PemDerSignatureConfig
+    CLIConfig,
+    LogConfig,
+    PemDerSignatureConfig,
+    PKCS11SignatureConfig,
+    PKCS12SignatureConfig,
+    StdLogOutput,
+    init_validation_context_kwargs,
+    parse_cli_config,
+    parse_logging_config,
 )
-from pyhanko.pdf_utils import misc
+from pyhanko.pdf_utils import crypt, misc
 from pyhanko.pdf_utils.config_utils import ConfigurationError
-
-from pyhanko.sign import signers, validation, fields
+from pyhanko.pdf_utils.incremental_writer import IncrementalPdfFileWriter
+from pyhanko.pdf_utils.layout import LayoutError
+from pyhanko.pdf_utils.reader import PdfFileReader
+from pyhanko.pdf_utils.writer import copy_into_new_writer
+from pyhanko.sign import fields, signers, validation
 from pyhanko.sign.general import (
-    SigningError, SignatureValidationError, load_certs_from_pemder
+    SignatureValidationError,
+    SigningError,
+    load_certs_from_pemder,
 )
 from pyhanko.sign.signers import DEFAULT_SIGNER_KEY_USAGE
+from pyhanko.sign.signers.pdf_cms import PdfCMSSignedAttributes
 from pyhanko.sign.timestamps import HTTPTimeStamper
-from pyhanko.pdf_utils.reader import PdfFileReader
-from pyhanko.pdf_utils.writer import copy_into_new_writer
-from pyhanko.pdf_utils.incremental_writer import IncrementalPdfFileWriter
-from pyhanko.pdf_utils import crypt
-from pyhanko.sign.validation import (
-    RevocationInfoValidationType
-)
-from pyhanko.stamp import QRStampStyle, text_stamp_file, qr_stamp_file
-from pyhanko import __version__
+from pyhanko.sign.validation import RevocationInfoValidationType
+from pyhanko.stamp import QRStampStyle, qr_stamp_file, text_stamp_file
 
 __all__ = ['cli']
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -152,22 +157,27 @@
 
     if verbose:
         # override the root logger's logging level, but preserve the output
         root_logger_config = log_config[None]
         log_config[None] = LogConfig(
             level=logging.DEBUG, output=root_logger_config.output
         )
-    elif 'fontTools.subset' not in log_config:
-        # the fontTools subsetter has a very noisy INFO log, so
-        # set that one to WARNING by default
-        log_config['fontTools.subset'] = LogConfig(
-            level=logging.WARNING,
-            # use the root logger's output settings to populate the default
-            output=log_config[None].output
-        )
+    else:
+        # use the root logger's output settings to populate the default
+        log_output = log_config[None].output
+        # Revinfo fetch logs -> filter by default
+        log_config['pyhanko_certvalidator.fetchers'] = LogConfig(
+            level=logging.WARNING, output=log_output
+        )
+        if 'fontTools.subset' not in log_config:
+            # the fontTools subsetter has a very noisy INFO log, so
+            # set that one to WARNING by default
+            log_config['fontTools.subset'] = LogConfig(
+                level=logging.WARNING, output=log_output
+            )
 
     logging_setup(log_config)
 
     if verbose:
         logging.debug("Running with --verbose")
     if config_text is not None:
         logging.debug(f'Finished reading configuration from {config}.')
@@ -359,47 +369,48 @@
             _, _, sig_bytes = pem.unarmor(sig_bytes)
         content_info = cms.ContentInfo.load(sig_bytes)
         if content_info['content_type'].native != 'signed_data':
             raise click.ClickException("CMS content type is not signedData")
     except ValueError as e:
         raise click.ClickException("Could not parse CMS object") from e
 
-    return validation.validate_detached_cms(
+    validation_coro = validation.async_validate_detached_cms(
         infile, signed_data=content_info['content'],
         signer_validation_context=validation_context,
         key_usage_settings=key_usage_settings
     )
+    return asyncio.run(validation_coro)
 
 
 def _signature_status_str(status_callback, pretty_print, executive_summary):
     try:
         status = status_callback()
         if executive_summary and not pretty_print:
-            return 'VALID' if status.bottom_line else 'INVALID'
+            return ('VALID' if status.bottom_line else 'INVALID', status.bottom_line)
         elif pretty_print:
-            return status.pretty_print_details()
+            return (status.pretty_print_details(), status.bottom_line)
         else:
-            return status.summary()
+            return (status.summary(), status.bottom_line)
     except validation.ValidationInfoReadingError as e:
         msg = (
             'An error occurred while parsing the revocation information '
             'for this signature: ' + str(e)
         )
         logger.error(msg)
         if pretty_print:
-            return msg
+            return (msg, False)
         else:
-            return 'REVINFO_FAILURE'
+            return ('REVINFO_FAILURE', False)
     except SignatureValidationError as e:
         msg = 'An error occurred while validating this signature: ' + str(e)
         logger.error(msg, exc_info=e)
         if pretty_print:
-            return msg
+            return (msg, False)
         else:
-            return 'INVALID'
+            return ('INVALID', False)
 
 
 # TODO add an option to do LTV, but guess the profile
 @signing.command(name='validate', help='validate signatures')
 @click.argument('infile', type=click.File('rb'))
 @click.option('--executive-summary',
               help='only print final judgment on signature validity',
@@ -464,22 +475,25 @@
     key_usage_settings = _get_key_usage_settings(ctx, validation_context)
     vc_kwargs = _prepare_vc(
         vc_kwargs, soft_revocation_check=soft_revocation_check,
         force_revinfo=force_revinfo
     )
     with pyhanko_exception_manager():
         if detached is not None:
-            status_str = _signature_status_str(
+            (status_str, signature_ok) = _signature_status_str(
                 status_callback=lambda: _validate_detached(
                     infile, detached, ValidationContext(**vc_kwargs),
                     key_usage_settings
                 ),
                 pretty_print=pretty_print, executive_summary=executive_summary
             )
-            print(status_str)
+            if signature_ok:
+                print(status_str)
+            else:
+                raise click.ClickException(status_str)
             return
 
         r = PdfFileReader(infile)
         sh = r.security_handler
         if isinstance(sh, crypt.StandardSecurityHandler):
             if password is None:
                 password = getpass.getpass(prompt='File password: ')
@@ -488,17 +502,18 @@
                 raise click.ClickException("Password didn't match.")
         elif sh is not None:
             raise click.ClickException(
                 "The CLI supports only password-based encryption when "
                 "validating (for now)"
             )
 
+        all_signatures_ok = True
         for ix, embedded_sig in enumerate(r.embedded_regular_signatures):
             fingerprint: str = embedded_sig.signer_cert.sha256.hex()
-            status_str = _signature_status_str(
+            (status_str, signature_ok) = _signature_status_str(
                 status_callback=lambda: _signature_status(
                     ltv_profile=ltv_profile, force_revinfo=force_revinfo,
                     vc_kwargs=vc_kwargs, key_usage_settings=key_usage_settings,
                     embedded_sig=embedded_sig
                 ),
                 pretty_print=pretty_print, executive_summary=executive_summary
             )
@@ -509,14 +524,18 @@
                 line = '=' * len(header)
                 print(line)
                 print(header)
                 print(line)
                 print('\n\n' + status_str)
             else:
                 print('%s:%s:%s' % (name, fingerprint, status_str))
+            all_signatures_ok &= signature_ok
+
+        if not all_signatures_ok:
+            raise click.ClickException("Validation failed")
 
 
 @signing.command(name='list', help='list signature fields')
 @click.argument('infile', type=click.File('rb'))
 @click.option('--skip-status', help='do not print status', required=False,
               type=bool, is_flag=True, default=False, show_default=True)
 def list_sigfields(infile, skip_status):
@@ -741,28 +760,38 @@
     if stamp_url is not None:
         text_params = {'url': stamp_url}
     return text_params
 
 
 def detached_sig(signer: signers.Signer, infile_path, outfile,
                  timestamp_url, use_pem):
+    coro = async_detached_sig(
+        signer, infile_path, outfile, timestamp_url, use_pem
+    )
+    return asyncio.run(coro)
+
+
+async def async_detached_sig(signer: signers.Signer, infile_path, outfile,
+                             timestamp_url, use_pem):
 
     with pyhanko_exception_manager():
         if timestamp_url is not None:
             timestamper = HTTPTimeStamper(timestamp_url)
             timestamp = None
         else:
             timestamper = None
-            # in this case, embed the signing time as an unsigned attr
+            # in this case, embed the signing time as a signed attr
             timestamp = datetime.now(tz=tzlocal.get_localzone())
 
         with open(infile_path, 'rb') as inf:
-            signature = signer.sign_general_data(
+            signature = await signer.async_sign_general_data(
                 inf, signers.DEFAULT_MD, timestamper=timestamper,
-                timestamp=timestamp
+                signed_attr_settings=PdfCMSSignedAttributes(
+                    signing_time=timestamp
+                )
             )
 
         output_bytes = signature.dump()
         if use_pem:
             output_bytes = pem.armor('PKCS7', output_bytes)
 
         # outfile is managed by Click
@@ -993,26 +1022,30 @@
 @click.argument('outfile', type=click.File('wb'))
 @click.option('--lib', help='path to PKCS#11 module',
               type=readable_file, required=False)
 @click.option('--token-label', help='PKCS#11 token label', type=str,
               required=False)
 @click.option('--cert-label', help='certificate label', type=str,
               required=False)
+@click.option('--raw-mechanism',
+              help='invoke raw PKCS#11 mechanism',
+              type=bool, is_flag=True, required=False)
 @click.option('--key-label', help='key label', type=str, required=False)
 @click.option('--slot-no', help='specify PKCS#11 slot to use',
               required=False, type=int, default=None)
 @click.option('--skip-user-pin', type=bool, show_default=True,
               default=False, required=False, is_flag=True,
               help='do not prompt for PIN (e.g. if the token has a PIN pad)')
 @click.option('--p11-setup', type=str, required=False,
               help='name of preconfigured PKCS#11 profile (overrides all '
                    'other options)')
 @click.pass_context
 def addsig_pkcs11(ctx, infile, outfile, lib, token_label,
-                  cert_label, key_label, slot_no, skip_user_pin, p11_setup):
+                  cert_label, key_label, slot_no, skip_user_pin, p11_setup,
+                  raw_mechanism):
     from pyhanko.sign import pkcs11
     timestamp_url = ctx.obj[Ctx.TIMESTAMP_URL]
 
     if p11_setup:
         cli_config: CLIConfig = ctx.obj.get(Ctx.CLI_CONFIG, None)
         if cli_config is None:
             raise click.ClickException(
@@ -1029,33 +1062,45 @@
             raise click.ClickException(
                 "The parameters --lib, --token-label and --cert-label "
                 "are required."
             )
         pkcs11_config = PKCS11SignatureConfig(
             module_path=lib, cert_label=cert_label, key_label=key_label,
             slot_no=slot_no, token_label=token_label,
-            prompt_pin=not skip_user_pin
+            prompt_pin=not skip_user_pin, raw_mechanism=raw_mechanism
         )
 
-    with pkcs11.PKCS11SigningContext(pkcs11_config) as signer:
+    pin = pkcs11_config.user_pin
+    if pin is None and pkcs11_config.prompt_pin:  # pragma: nocover
+        pin = getpass.getpass(prompt='PKCS#11 user PIN: ')
+    with pkcs11.PKCS11SigningContext(pkcs11_config, user_pin=pin) as signer:
         _sign_pkcs11(ctx, signer, infile, outfile, timestamp_url)
 
 
 @click.argument('infile', type=readable_file)
 @click.argument('outfile', type=click.File('wb'))
 @click.option('--lib', help='path to libbeidpkcs11 library file',
-              type=readable_file, required=True)
+              type=readable_file, required=False)
 @click.option('--use-auth-cert', type=bool, show_default=True,
               default=False, required=False, is_flag=True,
               help='use Authentication cert instead')
 @click.option('--slot-no', help='specify PKCS#11 slot to use', 
               required=False, type=int, default=None)
 @click.pass_context
 def addsig_beid(ctx, infile, outfile, lib, use_auth_cert, slot_no):
     from pyhanko.sign import beid
+    if not lib:
+        cli_config: CLIConfig = ctx.obj.get(Ctx.CLI_CONFIG, None)
+        if cli_config is None or cli_config.beid_module_path is None:
+            raise click.ClickException(
+                "The --lib option is mandatory unless beid-module-path is "
+                "provided in the configuration file."
+            )
+        lib = cli_config.beid_module_path
+
     timestamp_url = ctx.obj[Ctx.TIMESTAMP_URL]
     session = beid.open_beid_session(lib, slot_no=slot_no)
     with session:
         signer = beid.BEIDSigner(session, use_auth_cert=use_auth_cert)
         _sign_pkcs11(ctx, signer, infile, outfile, timestamp_url)
```

### Comparing `pyHanko-0.8.0/pyhanko/config.py` & `pyHanko-0.9.0/pyhanko/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
+import binascii
 import enum
 import logging
-from datetime import timedelta
-from typing import Dict, Optional, Union, List, Iterable
 from dataclasses import dataclass
+from datetime import timedelta
+from typing import Dict, Iterable, List, Optional, Union
 
 import yaml
 from asn1crypto import x509
+from pyhanko_certvalidator import ValidationContext
 
 from pyhanko.pdf_utils import config_utils
-from pyhanko_certvalidator import ValidationContext
-from pyhanko.pdf_utils.config_utils import (
-    check_config_keys, ConfigurationError
-)
+from pyhanko.pdf_utils.config_utils import ConfigurationError, check_config_keys
 from pyhanko.pdf_utils.misc import get_and_apply
-
-from pyhanko.sign import load_certs_from_pemder, SimpleSigner
-from pyhanko.sign.general import KeyUsageConstraints
+from pyhanko.sign import SimpleSigner, load_certs_from_pemder
+from pyhanko.sign.general import KeyUsageConstraints, load_cert_from_pemder
 from pyhanko.sign.signers import DEFAULT_SIGNING_STAMP_STYLE
 from pyhanko.stamp import QRStampStyle, TextStampStyle
 
 
 class StdLogOutput(enum.Enum):
     STDERR = enum.auto()
     STDOUT = enum.auto()
@@ -60,14 +58,15 @@
     default_stamp_style: str
     time_tolerance: timedelta
     retroactive_revinfo: bool
     log_config: Dict[Optional[str], LogConfig]
     pemder_setups: Dict[str, dict]
     pkcs12_setups: Dict[str, dict]
     pkcs11_setups: Dict[str, dict]
+    beid_module_path: Optional[str]
 
     # TODO graceful error handling for syntax & type issues?
 
     def _get_validation_settings_raw(self, name=None):
         name = name or self.default_validation_context
         try:
             return self.validation_contexts[name]
@@ -378,27 +377,47 @@
     This class is used to load PKCS#11 setup information from YAML
     configuration.
     """
 
     module_path: str
     """Path to the PKCS#11 module shared object."""
 
-    token_label: str
-    """PKCS#11 token name"""
-
-    cert_label: str
+    cert_label: Optional[str] = None
     """PKCS#11 label of the signer's certificate."""
 
+    cert_id: Optional[bytes] = None
+    """PKCS#11 ID of the signer's certificate."""
+
+    signing_certificate: Optional[x509.Certificate] = None
+    """
+    The signer's certificate. If present, :attr:`cert_id` and
+    :attr:`cert_label` will not be used to obtain the signer's certificate
+    from the PKCS#11 token.
+
+    .. note::
+        This can be useful in case the signer's certificate is not available on
+        the token, or if you would like to present a different certificate than
+        the one provided on the token.
+    """
+
+    token_label: Optional[str] = None
+    """PKCS#11 token name"""
+
     other_certs: List[x509.Certificate] = None
     """Other relevant certificates."""
 
     key_label: Optional[str] = None
     """
-    PKCS#11 label of the signer's private key, if different from
-    :attr:`cert_label`.
+    PKCS#11 label of the signer's private key. Defaults to :attr:`cert_label`
+    if the latter is specified and :attr:`key_id` is not.
+    """
+
+    key_id: Optional[bytes] = None
+    """
+    PKCS#11 key ID.
     """
 
     slot_no: Optional[int] = None
     """
     Slot number of the PKCS#11 slot to use.
     """
 
@@ -439,34 +458,82 @@
     """
 
     prefer_pss: bool = False
     """
     Prefer PSS to PKCS#1 v1.5 padding when creating RSA signatures.
     """
 
+    raw_mechanism: bool = False
+    """
+    Invoke the raw variant of the PKCS#11 signing operation.
+
+    .. note::
+        This is currently only supported for ECDSA signatures.
+    """
+
     @classmethod
     def process_entries(cls, config_dict):
         super().process_entries(config_dict)
         other_certs = config_dict.get('other_certs', ())
         if isinstance(other_certs, str):
             other_certs = (other_certs,)
         config_dict['other_certs'] = list(load_certs_from_pemder(other_certs))
 
+        if 'token_label' not in config_dict and 'slot_no' not in config_dict:
+            raise ConfigurationError(
+                "Either 'slot_no' or 'token_label' must be provided in "
+                "PKCS#11 setup"
+            )
+
+        cert_file = config_dict.get('signing_certificate', None)
+        if cert_file is not None:
+            config_dict['signing_certificate'] \
+                = load_cert_from_pemder(cert_file)
+
+        if 'key_id' in config_dict:
+            config_dict['key_id'] \
+                = _process_pkcs11_id_value(config_dict['key_id'])
+        elif 'key_label' not in config_dict and 'cert_label' not in config_dict:
+            raise ConfigurationError(
+                "Either 'key_id', 'key_label' or 'cert_label' must be provided "
+                "in PKCS#11 setup"
+            )
+
+        if 'cert_id' in config_dict:
+            config_dict['cert_id'] \
+                = _process_pkcs11_id_value(config_dict['cert_id'])
+        elif 'cert_label' not in config_dict \
+                and 'signing_certificate' not in config_dict:
+            raise ConfigurationError(
+                "Either 'cert_id', 'cert_label' or 'signing_certificate' "
+                "must be provided in PKCS#11 setup"
+            )
+
+
+def _process_pkcs11_id_value(x: Union[str, int]):
+    if isinstance(x, int):
+        return bytes([x])
+    else:
+        return binascii.unhexlify(x)
+
 
 DEFAULT_VALIDATION_CONTEXT = DEFAULT_STAMP_STYLE = 'default'
 DEFAULT_TIME_TOLERANCE = 10
 STAMP_STYLE_TYPES = {
     'qr': QRStampStyle,
     'text': TextStampStyle,
 }
 
 
-def parse_cli_config(yaml_str):
+def parse_cli_config(yaml_str) -> CLIConfig:
     config_dict = yaml.safe_load(yaml_str) or {}
+    return CLIConfig(**process_config_dict(config_dict))
+
 
+def process_config_dict(config_dict: dict) -> dict:
     # validation context config
     vcs = {DEFAULT_VALIDATION_CONTEXT: {}}
     try:
         vc_specs = config_dict['validation-contexts']
         vcs.update(vc_specs)
     except KeyError:
         pass
@@ -481,17 +548,19 @@
     except KeyError:
         pass
 
     # logging config
     log_config_spec = config_dict.get('logging', {})
     log_config = parse_logging_config(log_config_spec)
 
+    # TODO type check!
     pkcs11_setups = config_dict.get('pkcs11-setups', {})
     pkcs12_setups = config_dict.get('pkcs12-setups', {})
     pemder_setups = config_dict.get('pemder-setups', {})
+    beid_module_path = config_dict.get('beid-module-path', None)
 
     # some misc settings
     default_vc = config_dict.get(
         'default-validation-context', DEFAULT_VALIDATION_CONTEXT
     )
     default_stamp_style = config_dict.get(
         'default-stamp-style', DEFAULT_STAMP_STYLE
@@ -502,14 +571,15 @@
     if not isinstance(time_tolerance_seconds, int):
         raise ConfigurationError(
             "time-tolerance parameter must be specified in seconds"
         )
 
     time_tolerance = timedelta(seconds=time_tolerance_seconds)
     retroactive_revinfo = bool(config_dict.get('retroactive-revinfo', False))
-    return CLIConfig(
+    return dict(
         validation_contexts=vcs, default_validation_context=default_vc,
         time_tolerance=time_tolerance, retroactive_revinfo=retroactive_revinfo,
         stamp_styles=stamp_configs, default_stamp_style=default_stamp_style,
         log_config=log_config, pkcs11_setups=pkcs11_setups,
-        pkcs12_setups=pkcs12_setups, pemder_setups=pemder_setups
+        pkcs12_setups=pkcs12_setups, pemder_setups=pemder_setups,
+        beid_module_path=beid_module_path
     )
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/_saslprep.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/_saslprep.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 
 """An implementation of RFC4013 SASLprep."""
 
 __all__ = ['saslprep']
 
 import stringprep
-
 import unicodedata
+
 # RFC4013 section 2.3 prohibited output.
 _PROHIBITED = (
     # A strict reading of RFC 4013 requires table c12 here, but
     # characters from it are mapped to SPACE in the Map step. Can
     # normalization reintroduce them somehow?
     stringprep.in_table_c12,
     stringprep.in_table_c21_c22,
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/barcodes.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/barcodes.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
         "pyhanko.pdf_utils.barcodes requires pyHanko to be installed with "
         "the [image-support] option. You can install missing "
         "dependencies by running "
         "\"pip install 'pyHanko[image-support]'\".", e
     )
 
 from pyhanko.pdf_utils.content import PdfContent
-from pyhanko.pdf_utils.misc import rd
 from pyhanko.pdf_utils.layout import BoxConstraints
+from pyhanko.pdf_utils.misc import rd
 
 __all__ = ['BarcodeBox', 'PdfStreamBarcodeWriter']
 
 
 def barcode_colour_to_pdf(colour) -> bytes:
     # TODO there has to be an index of common colour names somewhere, use
     #  that instead.
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/config_utils.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/config_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 .. note::
     On naming conventions: this module converts hyphens in key names to
     underscores as a matter of course.
 """
 
 import dataclasses
 import re
-from typing import Type, Optional, Union
-from asn1crypto.core import ObjectIdentifier, BitString
+from typing import Optional, Type, Union
+
+from asn1crypto.core import BitString, ObjectIdentifier
 
 __all__ = [
     'ConfigurationError', 'ConfigurableMixin', 'check_config_keys',
     'OID_REGEX', 'process_oid', 'process_oids', 'process_bit_string_flags'
 ]
 
 _noneType = type(None)
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/content.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import binascii
 import uuid
 from enum import Enum
+
 from .generic import (
-    pdf_name, DictionaryObject, NameObject,
-    PdfObject, StreamObject,
+    DictionaryObject,
+    NameObject,
+    PdfObject,
+    StreamObject,
+    pdf_name,
 )
 from .layout import BoxConstraints
 from .reader import PdfFileReader
 
-
 __all__ = [
     'ResourceType', 'ResourceManagementError',
     'PdfResources', 'PdfContent', 'RawContent', 'ImportedPdfPage'
 ]
 
 # TODO have the merge_resources helper in incremental_writer rely on some
 #  of the idioms established here
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/crypt.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/crypt.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,31 +49,33 @@
   :attr:`~.generic.StreamObject.encoded_data` attribute of
   an "implicitly encrypted" stream will therefore contain decrypted data ready
   to be decoded in the usual way.
 
 As long as you don't require access to encoded object data and/or raw encrypted
 object data, this distiction should be irrelevant to you as an API user.
 """
-import logging
 import abc
-import struct
-import secrets
 import enum
+import logging
+import secrets
+import struct
 from dataclasses import dataclass
-from hashlib import md5, sha256, sha384, sha512, sha1
-from typing import Dict, Type, Optional, Tuple, Union, List, Set, Callable
+from hashlib import md5, sha1, sha256, sha384, sha512
+from typing import Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
-from asn1crypto import x509, cms, algos
-from asn1crypto.keys import PublicKeyAlgorithm, PrivateKeyInfo
+from asn1crypto import algos, cms, x509
+from asn1crypto.keys import PrivateKeyInfo, PublicKeyAlgorithm
 from cryptography.hazmat.primitives import padding, serialization
 from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
-from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey, \
-    RSAPrivateKey
-from cryptography.hazmat.primitives.serialization import pkcs12
+from cryptography.hazmat.primitives.asymmetric.rsa import (
+    RSAPrivateKey,
+    RSAPublicKey,
+)
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.primitives.serialization import pkcs12
 
 from . import generic, misc
 
 __all__ = [
     'SecurityHandler', 'StandardSecurityHandler', 'PubKeySecurityHandler',
     'AuthResult', 'AuthStatus',
     'SecurityHandlerVersion', 'StandardSecuritySettingsRevision',
@@ -2243,16 +2245,16 @@
             with open(pfx_file, 'rb') as f:
                 pfx_bytes = f.read()
             (private_key, cert, other_certs) = pkcs12.load_key_and_certificates(
                 pfx_bytes, passphrase
             )
 
             from ..sign.general import (
+                _translate_pyca_cryptography_cert_to_asn1,
                 _translate_pyca_cryptography_key_to_asn1,
-                _translate_pyca_cryptography_cert_to_asn1
             )
             cert = _translate_pyca_cryptography_cert_to_asn1(cert)
             private_key = _translate_pyca_cryptography_key_to_asn1(private_key)
         except (IOError, ValueError, TypeError) as e:  # pragma: nocover
             logger.error(f'Could not open PKCS#12 file {pfx_file}.', exc_info=e)
             return None
 
@@ -2335,14 +2337,15 @@
     # and AES-CBC (128, 192, 256 bits)
     cipher_name = algo.encryption_cipher
 
     with_iv = {'aes': _aes_cbc_decrypt}
     try:
         # noinspection PyUnresolvedReferences
         from oscrypto import symmetric
+
         # The spec mandates that we support these, but pyca/cryptography
         # doesn't offer implementations.
         # (DES and 3DES have fortunately gone out of style, but some libraries
         #  still rely on RC2)
         with_iv.update({
             'des': symmetric.des_cbc_pkcs5_decrypt,
             'tripledes': symmetric.tripledes_cbc_pkcs5_decrypt,
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/embed.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 .. versionadded:: 0.7.0
 """
 
 import hashlib
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional, List
+from typing import List, Optional
 
 from asn1crypto import x509
 
-from . import generic, writer, misc, crypt
+from . import crypt, generic, misc, writer
 from .generic import pdf_name, pdf_string
 
 __all__ = [
     'embed_file', 'EmbeddedFileObject', 'EmbeddedFileParams',
     'FileSpec', 'RelatedFileSpec', 'wrap_encrypted_payload'
 ]
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/filters.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 for the original license of the PyPDF2 project.
 
 Note that not all decoders specified in the standard are supported.
 In particular ``/Crypt`` and ``/LZWDecode`` are missing.
 """
 import binascii
 import re
-
-from .misc import PdfReadError, PdfStreamError, Singleton
-from io import BytesIO
 import struct
-
 import zlib
+from io import BytesIO
+
+from .misc import PdfReadError, PdfStreamError, Singleton
 
 __all__ = [
     'Decoder', 'ASCII85Decode', 'ASCIIHexDecode', 'FlateDecode',
     'get_generic_decoder'
 ]
 
 decompress = zlib.decompress
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/font/api.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/font/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from dataclasses import dataclass, field
-from typing import Optional, Dict
+from typing import Dict, Optional
 
 from pyhanko.pdf_utils import generic
 
 __all__ = [
     'ShapeResult', 'FontEngine', 'FontSubsetCollection', 'FontEngineFactory'
 ]
 
 from pyhanko.pdf_utils.writer import BasePdfFileWriter
 
-
 ALPHABET = 'ABCDEFGHIJKLMNOPQRSTUVWXYZ'
 
 
 def generate_subset_prefix():
     import random
     return ''.join(ALPHABET[random.randint(0, 25)] for _ in range(6))
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/font/basic.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/font/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyhanko.pdf_utils import generic
-from .api import FontEngine, ShapeResult, FontEngineFactory
+
 from ..writer import BasePdfFileWriter
+from .api import FontEngine, FontEngineFactory, ShapeResult
 
 pdf_name = generic.NameObject
 
 
 class SimpleFontEngine(FontEngine):
     """
     Simplistic font engine that effectively only works with PDF standard fonts,
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/font/opentype.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/font/opentype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Basic support for OpenType/TrueType font handling & subsetting.
 
 This module relies on `fontTools <https://pypi.org/project/fonttools/>`_ for
 OTF parsing and subsetting, and on HarfBuzz (via ``uharfbuzz``) for shaping.
 """
 import logging
+from binascii import hexlify
 from dataclasses import dataclass
 from io import BytesIO
-from binascii import hexlify
 
 from pyhanko.pdf_utils import generic
 from pyhanko.pdf_utils.font.api import (
-    ShapeResult, FontEngine, FontEngineFactory
+    FontEngine,
+    FontEngineFactory,
+    ShapeResult,
 )
 from pyhanko.pdf_utils.misc import peek
 from pyhanko.pdf_utils.writer import BasePdfFileWriter
 
 try:
     import uharfbuzz as hb
-    from fontTools import ttLib, subset
+    from fontTools import subset, ttLib
 except ImportError as import_err:  # pragma: nocover
     raise ImportError(
         "pyhanko.pdf_utils.font.opentype requires pyHanko to be installed with "
         "the [opentype] option. You can install missing "
         "dependencies by running \"pip install 'pyHanko[opentype]'\".",
         import_err
     )
@@ -176,15 +178,15 @@
                                    vertical, obj_stream=None):
 
     # take the Identity-* encoding to inherit from the /Encoding
     # entry specified in our CIDSystemInfo dict
     encoding = 'Identity-V' if vertical else 'Identity-H'
 
     cidfont_obj.embed(writer, obj_stream=obj_stream)
-    cidfont_ref = writer.add_object(cidfont_obj)
+    cidfont_ref = writer.add_object(cidfont_obj, obj_stream=obj_stream)
     type0 = generic.DictionaryObject({
         pdf_name('/Type'): pdf_name('/Font'),
         pdf_name('/Subtype'): pdf_name('/Type0'),
         pdf_name('/DescendantFonts'): generic.ArrayObject([cidfont_ref]),
         pdf_name('/Encoding'): pdf_name('/' + encoding),
         pdf_name('/BaseFont'): pdf_name(f'/{cidfont_obj.name}-{encoding}'),
     })
@@ -289,16 +291,15 @@
 
 def _read_ps_name(tt: ttLib.TTFont) -> str:
     ps_name = None
     try:
         name_table = tt['name']
         # extract PostScript name from the font's name table
         nr = next(nr for nr in name_table.names if nr.nameID == 6)
-        if nr.encodingIsUnicodeCompatible():
-            ps_name = nr.string.decode('utf-16be')
+        ps_name = nr.toUnicode()
     except StopIteration:  # pragma: nocover
         pass
 
     if ps_name is None:
         raise NotImplementedError(
             "Could not deduce PostScript name for font; only "
             "unicode-compatible encodings in the name table are supported"
@@ -389,15 +390,15 @@
         if writing_direction is not None and \
                 writing_direction not in ('ltr', 'rtl', 'ttb', 'btt'):
             raise ValueError(
                 "Writing direction must be one of 'ltr', 'rtl', 'ttb' or 'btt'."
             )
         self.writing_direction = writing_direction
         self.bcp47_lang_code = bcp47_lang_code
-        self.__subset_created = False
+        self._subset_created = self._write_prepared = False
 
     @property
     def _reverse_cmap(self):
         if self.__reverse_cmap is None:
             self.__reverse_cmap = self.tt['cmap'].buildReversed()
         return self.__reverse_cmap
 
@@ -544,14 +545,15 @@
             'currentdict\n'
             '/CMap defineresource\n'
             'pop\nend\nend'
         )
         stream = generic.StreamObject(
             stream_data=(header + body + footer).encode('ascii')
         )
+        stream.compress()
         return stream
 
     def _extract_subset(self, options=None):
         options = options or subset.Options(layout_closure=False)
         if not self.is_cff_font:
             # Have to retain GIDs in the Type2 (non-CFF) case, since we don't
             # have a predefined character set available (i.e. the ROS ordering
@@ -579,30 +581,33 @@
 
         .. danger::
             Due to the way ``fontTools`` handles subsetting, this is a
             destructive operation. The in-memory representation of the original
             font will be overwritten by the generated subset.
         """
 
-        if not self.__subset_created:
+        if self._write_prepared:
+            return
+        if not self._subset_created:
             self._extract_subset()
-            self.__subset_created = True
+            self._subset_created = True
         writer = self.writer
         obj_stream = self.obj_stream
         by_cid = iter(sorted(self._glyphs.values(), key=lambda t: t[0]))
         type0 = _build_type0_font_from_cidfont(
             writer=writer, cidfont_obj=self.cidfont_obj,
             widths_by_cid_iter=by_cid, obj_stream=obj_stream,
             vertical=False
         )
         type0['/ToUnicode'] = writer.add_object(
             self._format_tounicode_cmap()
         )
         # use our preallocated font ref
         writer.add_object(type0, obj_stream, idnum=self._font_ref.idnum)
+        self._write_prepared = True
 
     def as_resource(self) -> generic.IndirectObject:
         return self._font_ref
 
 
 class CIDFont(generic.DictionaryObject):
     def __init__(self, tt: ttLib.TTFont, subtype, registry, ordering,
@@ -739,17 +744,19 @@
                 map(generic.NumberObject, bbox)
             ),
             # FIXME I'm setting the Serif and Symbolic flags here, but
             #  is there any way we can read/infer those from the TTF metadata?
             pdf_name('/Flags'): generic.NumberObject(0b110),
             pdf_name('/StemV'): generic.NumberObject(stemv),
             pdf_name('/ItalicAngle'): generic.FloatObject(
-                tt['post'].italicAngle
+                getattr(tt['post'], 'italicAngle', 0)
             ),
-            pdf_name('/CapHeight'): generic.NumberObject(os2.sCapHeight)
+            pdf_name('/CapHeight'): generic.NumberObject(
+                getattr(os2, 'sCapHeight', 750)
+            )
         })
 
 
 @dataclass(frozen=True)
 class GlyphAccumulatorFactory(FontEngineFactory):
     """
     Stateless callable helper class to instantiate :class:`.GlyphAccumulator`
@@ -780,17 +787,26 @@
 
     writing_direction: str = None
     """
     Writing direction, one of 'ltr', 'rtl', 'ttb' or 'btt'.
     Will be guessed by HarfBuzz if not specified.
     """
 
+    create_objstream_if_needed: bool = True
+    """
+    Create an object stream to hold this glyph accumulator's assets if no
+    object stream is passed in, and the writer supports object streams.
+    """
+
     def create_font_engine(self, writer: 'BasePdfFileWriter',
                            obj_stream=None) -> GlyphAccumulator:
         fh = open(self.font_file, 'rb')
+        if obj_stream is None and writer.stream_xrefs and \
+                self.create_objstream_if_needed:
+            obj_stream = writer.prepare_object_stream()
         return GlyphAccumulator(
             writer=writer, font_handle=fh,
             font_size=self.font_size, ot_script_tag=self.ot_script_tag,
             ot_language_tag=self.ot_language_tag,
             writing_direction=self.writing_direction,
             obj_stream=obj_stream
         )
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/generic.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 """
 Implementation of PDF object types and other generic functionality.
 The internals were imported from PyPDF2, with modifications.
 
 See :ref:`here <pypdf2-license>` for the original license
 of the PyPDF2 project.
 """
+import binascii
+import codecs
+import decimal
+import logging
 import os
 import re
-import binascii
+from dataclasses import dataclass, field
 from datetime import datetime, timedelta, timezone
 from io import BytesIO
-from typing import Iterator, Tuple, Optional, Union, Callable, Any
-from dataclasses import dataclass, field
+from typing import Any, Callable, Iterator, Optional, Tuple, Union
 
+from . import filters
 from .misc import (
-    read_non_whitespace, skip_over_comment, read_until_regex,
-    is_regular_character
-)
-from .misc import (
-    PdfStreamError, PdfReadError, IndirectObjectExpected, PdfWriteError
+    IndirectObjectExpected,
+    PdfReadError,
+    PdfStreamError,
+    PdfWriteError,
+    is_regular_character,
+    read_non_whitespace,
+    read_until_regex,
+    skip_over_comment,
 )
-import logging
-from . import filters
-import decimal
-import codecs
 
 __all__ = [
     'Dereferenceable', 'Reference', 'TrailerReference',
     'PdfObject', 'IndirectObject', 'NullObject', 'BooleanObject', 'FloatObject',
     'NumberObject', 'ByteStringObject', 'TextStringObject', 'NameObject',
     'ArrayObject', 'DictionaryObject', 'StreamObject',
     'read_object', 'pdf_name', 'pdf_string', 'pdf_date'
@@ -845,23 +848,35 @@
                     f"Byte (0x{hex(cur_byte)}) must be escaped in a PDF name"
                 )
             result.write(
                 bytes((cur_byte,))
             )
     except StopIteration:
         pass
+    name_bytes = result.getvalue()
     # NOTE: we assume UTF-8, but the PDF spec actually doesn't prescribe
     #  a character encoding for names, they're just byte sequences.
     #  This doesn't matter in 99.99% of cases (since names are not supposed
     #  to contain renderable text, and are typically 7-bit ASCII anyhow),
     #  but it's not 100% correct. I don't see a way to fix this without causing
     #  massive non-obvious API breakage (since NameObject inherits from 'str' as
     #  in PyPDF2), i.e. the correctness benefit is vastly outweighed by the
     #  risks (for now)
-    return NameObject(result.getvalue().decode('utf8'))
+    encodings_to_try = ('utf8', 'latin1')
+    # latin1 should never trigger decoding errors, since Python's implementation
+    # maps even unassigned values to corresponding unicode codepoints
+    name_str = None
+    for enc in encodings_to_try:
+        try:
+            name_str = name_bytes.decode(enc)
+            break
+        except ValueError:
+            pass
+    assert name_str is not None
+    return NameObject(name_str)
 
 
 class NameObject(str, PdfObject):
     """
     PDF name object. These are valid Python strings, but names and strings
     are treated differently in the PDF specification, so proper care is
     required.
@@ -1527,27 +1542,27 @@
 
 ASN_DT_FORMAT = "D:%Y%m%d%H%M%S"
 
 
 def pdf_date(dt: datetime) -> TextStringObject:
     """
     Convert a datetime object into a PDF string.
-    This funciton supports both timezone-aware and naive datetimes.
+    This function supports both timezone-aware and naive datetime objects.
 
     :param dt:
         The datetime object to convert.
     :return:
         A :class:`TextStringObject` representing the datetime passed in.
     """
 
     base_dt = dt.strftime(ASN_DT_FORMAT)
     utc_offset_string = ''
     if dt.tzinfo is not None:
-        # compute UTC off set string
-        tz_seconds = dt.utcoffset().seconds
+        # compute UTC offset string
+        tz_seconds = dt.utcoffset().total_seconds()
         if not tz_seconds:
             utc_offset_string = 'Z'
         else:
             sign = '+'
             if tz_seconds < 0:
                 sign = '-'
                 tz_seconds = abs(tz_seconds)
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/images.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,20 @@
     Currently there is no support for CMYK images or (direct) support for
     embedding JPEG-encoded image data as such, but these features may be added
     later.
 
 """
 
 import uuid
-
 from typing import Union
 
-from .layout import BoxConstraints
-from .generic import pdf_name
-from .content import ResourceType, PdfResources, PdfContent
 from . import generic
+from .content import PdfContent, PdfResources, ResourceType
+from .generic import pdf_name
+from .layout import BoxConstraints
 from .writer import BasePdfFileWriter
 
 try:
     from PIL import Image
     from PIL.ImagePalette import ImagePalette
 except ImportError as e:  # pragma: nocover
     raise ImportError(
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/incremental_writer.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/incremental_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 Utility for writing incremental updates to existing PDF files.
 """
 
 import os
-from typing import Union, Optional
+from typing import Optional, Union
 
 from . import generic, misc
 from .crypt import EnvelopeKeyDecrypter
-
-from .reader import PdfFileReader, parse_catalog_version
 from .generic import pdf_name
+from .reader import PdfFileReader, parse_catalog_version
 from .writer import BasePdfFileWriter
 
-
 __all__ = ['IncrementalPdfFileWriter']
 
 
 class IncrementalPdfFileWriter(BasePdfFileWriter):
     """Class to incrementally update existing files.
 
     This :class:`~.writer.BasePdfFileWriter` subclass encapsulates a
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/layout.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/layout.py`

 * *Files identical despite different names*

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/misc.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     'assert_writable_and_random_access', 'prepare_rw_output_stream',
     'finalise_output',
     'DEFAULT_CHUNK_SIZE', 'chunked_write', 'chunked_digest', 'chunk_stream',
     'ConsList', 'Singleton', 'rd'
 ]
 
 from io import BytesIO
-
-from typing import Callable, TypeVar, Generator, Iterable
-
+from typing import Callable, Generator, Iterable, TypeVar
 
 DEFAULT_CHUNK_SIZE = 4096
 """
 Default chunk size for stream I/O.
 """
 
 rd = lambda x: round(x, 4)
@@ -71,15 +69,15 @@
             tok = stream.read(1)
             if tok.isspace() or not tok:
                 break
             yield tok
     return b''.join(_build())
 
 
-PDF_WHITESPACE = b' \n\r\t\x00'
+PDF_WHITESPACE = b' \n\r\t\f\x00'
 PDF_DELIMITERS = b'()<>[]{}/%'
 
 
 def is_regular_character(byte_value: int):
     return byte_value not in PDF_WHITESPACE and byte_value not in PDF_DELIMITERS
 
 
@@ -180,15 +178,15 @@
 
 def get_courier():
     """
     :return:
         A resource dictionary representing the standard Courier font
         (or one of its metric equivalents).
     """
-    from .generic import pdf_name, DictionaryObject
+    from .generic import DictionaryObject, pdf_name
     return DictionaryObject({
         pdf_name('/Type'): pdf_name('/Font'),
         pdf_name('/Subtype'): pdf_name('/Type1'),
         pdf_name('/BaseFont'): pdf_name('/Courier')
     })
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/qr.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/qr.py`

 * *Files identical despite different names*

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/reader.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 The implementation was tweaked with the express purpose of facilitating
 historical inspection and auditing of PDF files with multiple revisions
 through incremental updates.
 This comes at a cost, and future iterations of this module may offer more
 flexibility in terms of the level of detail with which file size is scrutinised.
 """
 
-import struct
+import logging
 import os
 import re
+import struct
 from collections import defaultdict
 from io import BytesIO
 from itertools import chain
-from typing import Set, List, Optional, Union, Tuple
+from typing import List, Optional, Set, Tuple, Union
 
 from . import generic, misc
-from .misc import PdfReadError
 from .crypt import (
-    SecurityHandler, StandardSecurityHandler,
-    EnvelopeKeyDecrypter, PubKeySecurityHandler,
+    EnvelopeKeyDecrypter,
+    PubKeySecurityHandler,
+    SecurityHandler,
+    StandardSecurityHandler,
 )
-
-import logging
-
+from .misc import PdfReadError
 from .rw_common import PdfHandler
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = ['PdfFileReader', 'HistoricalResolver', 'parse_catalog_version']
 
@@ -1536,23 +1536,29 @@
                 if child_ref is not None:
                     yield child_ref
 
                 yield from _collect_struct_tree_refs(child)
 
         pages_ref = self.root.raw_get('/Pages')
         page_tree_nodes = set()
-        page_tree_nodes.update(
-            _collect_page_tree_refs(pages_obj=pages_ref.get_object())
-        )
+        for ref in _collect_page_tree_refs(pages_obj=pages_ref.get_object()):
+            if ref in page_tree_nodes:
+                raise misc.PdfReadError(
+                    "Circular reference in page tree in mapping stage"
+                )
+            page_tree_nodes.add(ref)
         struct_tree_nodes = set()
         try:
             struct_tree_root_ref = self.root.raw_get('/StructTreeRoot')
-            struct_tree_nodes.update(
-                _collect_struct_tree_refs(struct_tree_root_ref.get_object())
-            )
+            for ref in _collect_struct_tree_refs(struct_tree_root_ref.get_object()):
+                if ref in struct_tree_nodes:
+                    raise misc.PdfReadError(
+                        "Circular reference in structure tree in mapping stage"
+                    )
+                struct_tree_nodes.add(ref)
         except KeyError:
             pass
         _compute_paths_to_refs(
             self.trailer_view, misc.ConsList.empty(), misc.ConsList.empty(),
             is_page_tree=False, page_tree_objs=page_tree_nodes,
             is_struct_tree=False, struct_tree_objs=struct_tree_nodes
         )
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/rw_common.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/rw_common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utilities common to reading and writing PDF files."""
 from typing import Tuple
 
-from . import generic
+from . import generic, misc
 
 __all__ = ['PdfHandler']
 
 
 class PdfHandler:
     """Abstract class providing a general interface for quering objects
     in PDF readers and writers alike."""
@@ -73,39 +73,43 @@
 
         page_count = page_tree_root['/Count']
         if page_ix < 0:
             page_ix = page_count + page_ix
         if not (0 <= page_ix < page_count):
             raise ValueError('Page index out of range')
 
-        def _recurse(first_page_ix, pages_obj_ref, last_rsrc_dict):
+        def _recurse(first_page_ix, pages_obj_ref, last_rsrc_dict, refs_seen):
             pages_obj = pages_obj_ref.get_object()
             kids = pages_obj['/Kids']
             try:
                 last_rsrc_dict = pages_obj.raw_get('/Resources')
             except KeyError:
                 pass
 
             cur_page_ix = first_page_ix
             for kid_index, kid_ref in enumerate(kids):
-                # If this is not the case, the child node cannot possibly have
-                # a valid /Parent entry either, so let's assume that nobody
-                # screws up their PDF generator THAT badly
+                if not isinstance(kid_ref, generic.IndirectObject):
+                    raise misc.PdfReadError(
+                        "Page tree node children must be indirect objects"
+                    )
                 assert isinstance(kid_ref, generic.IndirectObject)
+                if kid_ref.reference in refs_seen:
+                    raise misc.PdfReadError("Circular reference in page tree")
 
                 kid = kid_ref.get_object()
 
                 node_type = kid['/Type']
                 if node_type == '/Pages':
                     # recurse into this branch if the page we need
                     # is part of it
                     desc_count = kid['/Count']
                     if cur_page_ix <= page_ix < cur_page_ix + desc_count:
                         return _recurse(
-                            cur_page_ix, kid_ref, last_rsrc_dict
+                            cur_page_ix, kid_ref, last_rsrc_dict,
+                            refs_seen | {kid_ref.reference}
                         )
                     cur_page_ix += desc_count
                 elif node_type == '/Page':
                     if cur_page_ix == page_ix:
                         if retrieve_parent:
                             return (
                                 pages_obj_ref, kid_index, last_rsrc_dict
@@ -117,15 +121,15 @@
                                 pass
                             return kid_ref, last_rsrc_dict
                     else:
                         cur_page_ix += 1
             # This means the PDF is not standards-compliant
             raise ValueError('Page not found')
 
-        return _recurse(0, page_tree_root_ref, root_resources)
+        return _recurse(0, page_tree_root_ref, root_resources, set())
 
     def find_page_container(self, page_ix):
         """
         Retrieve the node in the page tree containing the
         page with index ``page_ix``, along with the necessary objects
         to modify it in an incremental update scenario.
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/text.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Utilities related to text rendering & layout."""
 
 from dataclasses import dataclass, field
 
-from pyhanko.pdf_utils.font import SimpleFontEngineFactory, FontEngineFactory
-from pyhanko.pdf_utils.generic import (
-    pdf_name,
-)
-from pyhanko.pdf_utils.content import ResourceType, PdfResources, PdfContent
 from pyhanko.pdf_utils import layout
 from pyhanko.pdf_utils.config_utils import ConfigurableMixin, ConfigurationError
+from pyhanko.pdf_utils.content import PdfContent, PdfResources, ResourceType
+from pyhanko.pdf_utils.font import FontEngineFactory, SimpleFontEngineFactory
+from pyhanko.pdf_utils.generic import pdf_name
 
 
 @dataclass(frozen=True)
 class TextStyle(ConfigurableMixin):
     """Container for basic test styling settings."""
 
     font: FontEngineFactory \
```

### Comparing `pyHanko-0.8.0/pyhanko/pdf_utils/writer.py` & `pyHanko-0.9.0/pyhanko/pdf_utils/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 
 """
 Utilities for writing PDF files.
 Contains code from the PyPDF2 project; see :ref:`here <pypdf2-license>`
 for the original license.
 """
 
+import enum
 import os
 import struct
-import enum
 from dataclasses import dataclass
 from io import BytesIO
-from typing import List, Union, Optional, Tuple, Iterable
+from typing import Iterable, List, Optional, Tuple, Union
 
 from asn1crypto import x509
 
-from pyhanko.pdf_utils import generic, content
+from pyhanko import __version__
+from pyhanko.pdf_utils import content, generic
 from pyhanko.pdf_utils.crypt import (
-    SecurityHandler, StandardSecurityHandler,
     PubKeySecurityHandler,
+    SecurityHandler,
+    StandardSecurityHandler,
 )
 from pyhanko.pdf_utils.generic import pdf_name, pdf_string
 from pyhanko.pdf_utils.misc import (
-    peek, PdfReadError, instance_test,
+    PdfReadError,
     PdfWriteError,
+    instance_test,
+    peek,
 )
 from pyhanko.pdf_utils.rw_common import PdfHandler
-from pyhanko import __version__
-
 
 __all__ = [
     'ObjectStream', 'BasePdfFileWriter',
     'PageObject', 'PdfFileWriter', 'init_xobject_dictionary',
     'copy_into_new_writer', 'DeveloperExtension', 'DevExtensionMultivalued'
 ]
 
@@ -52,23 +54,25 @@
     .. warning::
         Object streams can only be used in files with a cross-reference
         stream, as opposed to a classical XRef table.
         In particular, this means that incremental updates to files with a
         legacy XRef table cannot contain object streams either.
         See § 7.5.7 in ISO 32000-1 for further details.
 
-    .. warning::
-        The usefulness of object streams is somewhat stymied by the fact that
-        PDF stream objects cannot be embedded into object streams for
-        syntactical reasons.
+    .. danger::
+        Use :meth:`.BasePdfFileWriter.prepare_object_stream` to create instances
+        of object streams. The `__init__` function is internal API.
+
     """
 
-    def __init__(self, compress=True):
+    def __init__(self, writer: 'BasePdfFileWriter', compress=True):
         self._obj_refs = {}
         self.compress = compress
+        self.writer = writer
+        self._ref = None
 
     def add_object(self, idnum: int, obj: generic.PdfObject):
         """
         Add an object to an object stream.
         Note that objects in object streams always have their generation number
         set to `0` by definition.
 
@@ -84,14 +88,31 @@
         if isinstance(obj, OBJSTREAM_FORBIDDEN):
             raise TypeError(
                 'Stream objects and bare references cannot be embedded into '
                 'object streams.'
             )  # pragma: nocover
         self._obj_refs[idnum] = obj
 
+    def register_and_emit(self):
+        """
+        Internal method to flush an object stream as part of the file
+        writing process.
+        """
+        stream_ref = self._ref
+        objects = self._obj_refs
+        if objects and stream_ref is None:
+            # first, register the object stream object
+            #  (will get written later)
+            stream_ref = self._ref \
+                = self.writer.add_object(self.as_pdf_object())
+        # loop over all objects in the stream, and prepare
+        # the data to put in the XRef table
+        for ix, (idnum, obj) in enumerate(objects.items()):
+            yield idnum, (stream_ref.idnum, ix)
+
     def as_pdf_object(self) -> generic.StreamObject:
         """
         Render the object stream to a PDF stream object
 
         :return: An instance of :class:`~.generic.StreamObject`.
         """
         stream_header = BytesIO()
@@ -244,14 +265,18 @@
 def _contiguous_xref_chunks(position_dict):
     """
     Helper method to divide the XRef table (or stream) into contiguous chunks.
     """
     previous_idnum = None
     current_chunk = []
 
+    if not position_dict.keys():
+        # return immediately, there are no objects
+        return
+
     # iterate over keys in object ID order
     key_iter = sorted(position_dict.keys(), key=lambda t: t[1])
     (_, first_idnum), key_iter = peek(key_iter)
     for ix in key_iter:
         generation, idnum = ix
 
         # the idnum jumped, so yield the current chunk
@@ -284,15 +309,20 @@
         stream.write(header.encode('ascii'))
 
     def write_subsection(chunk):
         for position, generation in chunk:
             entry = "%010d %05d n \n" % (position, generation)
             stream.write(entry.encode('ascii'))
 
-    first_idnum, subsection = next(subsections)
+    try:
+        first_idnum, subsection = next(subsections)
+    except StopIteration:
+        # no updates, just write '0 0' and be done with it
+        stream.write(b'0 0\n')
+        return xref_location
     # TODO support deleting objects
     # case distinction: in contrast with the above we have to ensure that
     # everything is written in one chunk when *not* doing incremental updates.
     # In particular, this applies to the null object
     null_obj_ref = b'0000000000 65535 f \n'
     if first_idnum == 1:
         # integrate the null object into the first subsection
@@ -722,35 +752,30 @@
         :return:
             An :class:`.ObjectStream` object.
         """
         if not self.stream_xrefs:  # pragma: no cover
             raise PdfWriteError(
                 'Object streams require Xref streams to be enabled.'
             )
-        stream = ObjectStream(compress=compress)
+        stream = ObjectStream(self, compress=compress)
         self.object_streams.append(stream)
         return stream
 
     def _write_header(self, stream):
         pass
 
     def _assign_security_handler(self, sh: SecurityHandler):
         self.security_handler = sh
         self._encrypt = self.add_object(sh.as_pdf_object())
 
     def _write_objects(self, stream, object_position_dict):
         # deal with objects in object streams first
         for obj_stream in self.object_streams:
-            # first, register the object stream object
-            #  (will get written later)
-            stream_ref = self.add_object(obj_stream.as_pdf_object())
-            # loop over all objects in the stream, and prepare
-            # the data to put in the XRef table
-            for ix, (idnum, obj) in enumerate(obj_stream._obj_refs.items()):
-                object_position_dict[(0, idnum)] = (stream_ref.idnum, ix)
+            for idnum, pos_record in obj_stream.register_and_emit():
+                object_position_dict[(0, idnum)] = pos_record
 
         for ix in sorted(self.objects.keys()):
             generation, idnum = ix
             obj = self.objects[ix]
             object_position_dict[ix] = stream.tell()
             stream.write(('%d %d obj\n' % (idnum, generation)).encode('ascii'))
             if self.security_handler is not None \
@@ -1396,15 +1421,16 @@
 
     :param input_handler:
         :class:`.PdfHandler` to source objects from.
     :return:
         New :class:`.PdfFileWriter` containing all objects from the input
         handler.
     """
-    w = PdfFileWriter(init_page_tree=False)
+    # TODO try to be more clever with object streams
+    w = PdfFileWriter(init_page_tree=False, stream_xrefs=False)
     input_root_ref = input_handler.root_ref
     output_root_ref = w.root_ref
     # call _import_object in such a way that we translate the input handler's
     # root to the new writer's root.
     # From a technical PoV this doesn't matter, but it makes the output file
     # somewhat "cleaner" (i.e. it doesn't leave an orphaned document catalog
     # cluttering up the file)
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/ades/api.py` & `pyHanko-0.9.0/pyhanko/sign/ades/api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import enum
 from dataclasses import dataclass
-
 from typing import Optional
 
+from pyhanko.sign.timestamps import TimeStamper
+
+from ..attributes import CMSAttributeProvider, TSTProvider
 from .cades_asn1 import (
-    CommitmentTypeIndication, SignaturePolicyIdentifier,
-    CommitmentTypeIdentifier
+    CommitmentTypeIdentifier,
+    CommitmentTypeIndication,
+    SignaturePolicyIdentifier,
 )
-from pyhanko.sign.general import simple_cms_attribute
-from pyhanko.sign.timestamps import TimeStamper
 
 __all__ = ['GenericCommitment', 'CAdESSignedAttrSpec']
 
 
 # TODO add semantics explanations from the standard
 
 @enum.unique
@@ -62,22 +63,41 @@
         Right now, pyHanko does not "understand" signature policies, so the
         signature policy identifier will be taken at face value and embedded
         without paying any heed to the actual rules of the signature policy.
         It is the API user's responsibility to make sure that all relevant
         provisions of the signature policy are adhered to.
     """
 
-    def extra_signed_attributes(self, message_digest, md_algorithm,
-                                timestamper: TimeStamper = None, dry_run=False):
+    def prepare_providers(self, message_digest, md_algorithm,
+                          timestamper: Optional[TimeStamper] = None):
+
         if self.timestamp_content and timestamper is not None:
-            if dry_run:
-                ts_token = timestamper.dummy_response(md_algorithm)
-            else:
-                ts_token = timestamper.timestamp(message_digest, md_algorithm)
-            yield simple_cms_attribute('content_time_stamp', ts_token)
-        if self.signature_policy_identifier is not None:
-            yield simple_cms_attribute(
-                'signature_policy_identifier', self.signature_policy_identifier
+            yield TSTProvider(
+                digest_algorithm=md_algorithm,
+                data_to_ts=message_digest,
+                timestamper=timestamper, attr_type='content_time_stamp'
             )
+        if self.signature_policy_identifier is not None:
+            yield SigPolicyIDProvider(self.signature_policy_identifier)
         if self.commitment_type is not None:
-            yield simple_cms_attribute('commitment_type', self.commitment_type)
+            yield CommitmentTypeProvider(self.commitment_type)
+
+
+class CommitmentTypeProvider(CMSAttributeProvider):
+    attribute_type = 'commitment_type'
+
+    def __init__(self, commitment_type: CommitmentTypeIndication):
+        self.commitment_type = commitment_type
+
+    async def build_attr_value(self, dry_run=False) -> CommitmentTypeIndication:
+        return self.commitment_type
+
+
+class SigPolicyIDProvider(CMSAttributeProvider):
+    attribute_type = 'signature_policy_identifier'
+
+    def __init__(self, policy_id: SignaturePolicyIdentifier):
+        self.policy_id = policy_id
 
+    async def build_attr_value(self, dry_run=False) \
+            -> SignaturePolicyIdentifier:
+        return self.policy_id
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/ades/cades_asn1.py` & `pyHanko-0.9.0/pyhanko/sign/ades/cades_asn1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from asn1crypto import core, cms, algos
+from asn1crypto import algos, cms, core
+
 from .asn1_util import register_cms_attribute
 
 """
 ASN.1 type definitions from the CAdES specification.
 
 All definitions are as used in ETSI EN 319 122-1 V1.1.0.
 See also RFC 5126.
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/beid.py` & `pyHanko-0.9.0/pyhanko/sign/beid.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 Sign PDF files using a Belgian eID card.
 
 This module defines a very thin convenience wrapper around
 :mod:`.pyhanko.sign.pkcs11` to set up a PKCS#11 session with an eID card and
 read the appropriate certificates on the device.
 """
 
-from . import pkcs11 as sign_pkcs11
 from pkcs11 import Session
 
+from . import pkcs11 as sign_pkcs11
+
 __all__ = ['open_beid_session', 'BEIDSigner']
 
 
 def open_beid_session(lib_location, slot_no=None) -> Session:
     """
     Open a PKCS#11 session
 
@@ -40,13 +41,14 @@
     the (trustless) certificate list with the relevant certificates stored
     on the card.
     This includes the government's (self-signed) root certificate and the
     certificate of the appropriate intermediate CA.
     """
 
     def __init__(self, pkcs11_session: Session, use_auth_cert: bool = False,
-                 bulk_fetch: bool = False):
+                 bulk_fetch: bool = False, embed_roots=True):
         super().__init__(
             pkcs11_session=pkcs11_session,
             cert_label='Authentication' if use_auth_cert else 'Signature',
-            other_certs_to_pull=('Root', 'CA'), bulk_fetch=bulk_fetch
+            other_certs_to_pull=('Root', 'CA'), bulk_fetch=bulk_fetch,
+            embed_roots=embed_roots
         )
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/diff_analysis.py` & `pyHanko-0.9.0/pyhanko/sign/diff_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,32 +49,42 @@
 * Rules should be entirely stateless.
   "Clearing" a reference by yielding it does not imply that the revision
   cannot be vetoed by that same rule further down the road (this is why
   the first point is important).
 
 """
 
-import re
 import logging
+import re
 from collections import defaultdict
 from dataclasses import dataclass
 from enum import unique
 from io import BytesIO
 from typing import (
-    Iterable, Optional, Set, Tuple, Generator, TypeVar, Dict,
-    List, Callable, Union, Iterator
+    Callable,
+    Dict,
+    Generator,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
 )
 
-from pyhanko.pdf_utils.generic import Reference, PdfObject
+from pyhanko.pdf_utils import generic, misc
+from pyhanko.pdf_utils.generic import PdfObject, Reference
 from pyhanko.pdf_utils.misc import OrderedEnum
 from pyhanko.pdf_utils.reader import (
-    HistoricalResolver, PdfFileReader,
+    HistoricalResolver,
+    PdfFileReader,
     RawPdfPath,
 )
-from pyhanko.pdf_utils import generic, misc
 from pyhanko.sign.fields import FieldMDPSpec, MDPPerm
 
 __all__ = [
     'ModificationLevel', 'SuspiciousModification',
     'QualifiedWhitelistRule', 'WhitelistRule', 'qualify', 'ReferenceUpdate',
     'DocInfoRule', 'DSSCompareRule', 'MetadataUpdateRule',
     'CatalogModificationRule', 'ObjectStreamRule', 'XrefStreamRule',
@@ -341,41 +351,72 @@
         path = RawPdfPath('/Info')
         yield from map(
             ReferenceUpdate.curry_ref(paths_checked=path),
             _safe_whitelist(old, old_info, new_info)
         )
 
 
+def _assert_stream_refs(der_obj_type, arr, err_cls, is_vri):
+    arr = arr.get_object()
+    all_stream_arr = isinstance(arr, generic.ArrayObject) and all(
+        isinstance(obj, generic.IndirectObject)
+        and isinstance(obj.get_object(), generic.StreamObject)
+        for obj in arr
+    )
+    if not all_stream_arr:
+        raise err_cls(
+            f"Expected contents of '{der_obj_type}' in "
+            f"{'VRI' if is_vri else 'DSS'} to be an array of stream references."
+        )
+
+
 def _validate_dss_substructure(old: HistoricalResolver, new: HistoricalResolver,
-                               new_dict, der_stream_keys, is_vri):
+                               old_dict, new_dict, der_stream_keys, is_vri,
+                               path: RawPdfPath):
     for der_obj_type in der_stream_keys:
+        as_update = ReferenceUpdate.curry_ref(paths_checked=path + der_obj_type)
         try:
             value = new_dict.raw_get(der_obj_type)
         except KeyError:
             continue
-        if not isinstance(value.get_object(), generic.ArrayObject):
-            raise SuspiciousModification(
-                f"Expected array at {'VRI' if is_vri else 'DSS'} "
-                f"key {der_obj_type}."
-            )
+        _assert_stream_refs(der_obj_type, value, SuspiciousModification, is_vri)
+        if isinstance(value, generic.IndirectObject):
+            new_ref = value.reference
+            try:
+                old_value = old_dict.raw_get(der_obj_type)
+                if isinstance(old_value, generic.IndirectObject):
+                    yield from map(
+                        as_update,
+                        _safe_whitelist(old, old_value.reference, new_ref)
+                    )
+                _assert_stream_refs(
+                    der_obj_type, old_value, misc.PdfReadError, is_vri
+                )
+                # We don't enforce the contents of the new array vs. the old one
+                # deleting info is allowed by PAdES, and this check can get
+                # pretty expensive.
+            except KeyError:
+                pass
 
-        yield from map(ReferenceUpdate, new.collect_dependencies(
+        yield from map(as_update, new.collect_dependencies(
             value, since_revision=old.revision + 1
         ))
 
 
 class DSSCompareRule(WhitelistRule):
     """
     Rule that allows changes to the document security store (DSS).
 
     This rule will validate the structure of the DSS quite rigidly, and
     will raise :class:`.SuspiciousModification` whenever it encounters
     structural problems with the DSS.
-    Similarly, modifications that remove items from the DSS also count as
-    suspicious.
+    Similarly, modifications that remove structural items from the DSS
+    also count as suspicious. However, merely removing individual OCSP
+    responses, CRLs or certificates when they become irrelevant is permitted.
+    This is also allowed by PAdES.
     """
 
     def apply(self, old: HistoricalResolver, new: HistoricalResolver)\
             -> Iterable[ReferenceUpdate]:
         # TODO refactor these into less ad-hoc rules
 
         dss_path = RawPdfPath('/Root', '/DSS')
@@ -400,15 +441,16 @@
 
         if not (dss_keys <= dss_expected_keys):
             raise SuspiciousModification(
                 f"Unexpected keys in DSS: {dss_keys - dss_expected_keys}."
             )
 
         yield from _validate_dss_substructure(
-            old, new, new_dss, dss_der_stream_keys, is_vri=False
+            old, new, old_dss, new_dss, dss_der_stream_keys, is_vri=False,
+            path=RawPdfPath('/Root', '/DSS')
         )
 
         # check that the /VRI dictionary still contains all old keys, unchanged.
         vri_path = RawPdfPath('/Root', '/DSS', '/VRI')
         old_vri, new_vri = yield from misc.map_with_return(
             _compare_key_refs(
                 '/VRI', old, old_dss, new_dss,
@@ -466,15 +508,17 @@
             new_vri_value_keys = new_vri_dict.keys()
             if not (new_vri_value_keys <= vri_expected_keys):
                 raise SuspiciousModification(
                     "Unexpected keys in VRI dictionary: "
                     f"{new_vri_value_keys - vri_expected_keys}."
                 )
             yield from _validate_dss_substructure(
-                old, new, new_vri_dict, vri_der_stream_keys, is_vri=True
+                old, new, generic.DictionaryObject(),
+                new_vri_dict, vri_der_stream_keys, is_vri=True,
+                path=RawPdfPath('/Root', '/DSS', '/VRI', key)
             )
 
             # /TS is also a DER stream
             try:
                 ts_ref = new_vri_dict.get_value_as_reference(
                     '/TS', optional=True
                 )
@@ -879,15 +923,16 @@
         new_page_root = context.new.root['/Pages']
 
         yield from qualify(
             ModificationLevel.LTA_UPDATES,
             _walk_page_tree_annots(
                 old_page_root, new_page_root,
                 field_ref_reverse, context.old,
-                valid_when_locked=True
+                valid_when_locked=True,
+                refs_seen=set()
             )
         )
 
 
 class BaseFieldModificationRule(FieldMDPRule):
     """
     Base class that implements some boilerplate to validate modifications
@@ -1357,16 +1402,16 @@
         metadata_stream = metadata_ref.get_object()
 
         if not isinstance(metadata_stream, generic.StreamObject):
             raise SuspiciousModification(
                 "/Metadata should be a reference to a stream object"
             )
 
-        from xml.sax.handler import ContentHandler
         from xml.sax import make_parser
+        from xml.sax.handler import ContentHandler
 
         parser = make_parser()
         parser.setContentHandler(ContentHandler())
         try:
             parser.parse(BytesIO(metadata_stream.data))
         except Exception as e:
             raise SuspiciousModification(
@@ -1606,15 +1651,15 @@
         return annots, annots_ref
     except KeyError:
         raise
 
 
 def _walk_page_tree_annots(old_page_root, new_page_root,
                            field_name_dict, old: HistoricalResolver,
-                           valid_when_locked):
+                           valid_when_locked, refs_seen):
     def get_kids(page_root, exc):
         try:
             return _arr_to_refs(page_root['/Kids'], exc)
         except KeyError:
             raise exc("No /Kids in /Pages entry")
 
     old_kids = get_kids(old_page_root, misc.PdfReadError)
@@ -1623,24 +1668,28 @@
     # /Kids should only contain indirect refs, so direct comparison is
     # appropriate (__eq__ ignores the attached PDF handler)
     if old_kids != new_kids:
         raise SuspiciousModification(
             "Unexpected change to page tree structure."
         )
     for new_kid_ref, old_kid_ref in zip(new_kids, old_kids):
+        if old_kid_ref in refs_seen:
+            raise misc.PdfReadError(
+                "Circular reference in page tree during annotation analysis"
+            )
         new_kid = new_kid_ref.get_object()
         old_kid = old_kid_ref.get_object()
         try:
             node_type = old_kid['/Type']
         except (KeyError, TypeError) as e:  # pragma: nocover
             raise misc.PdfReadError from e
         if node_type == '/Pages':
             yield from _walk_page_tree_annots(
                 old_kid, new_kid, field_name_dict, old,
-                valid_when_locked
+                valid_when_locked, refs_seen | {old_kid_ref},
             )
         elif node_type == '/Page':
             try:
                 new_annots, new_annots_ref = _extract_annots_from_page(
                     new_kid, SuspiciousModification
                 )
             except KeyError:
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/fields.py` & `pyHanko-0.9.0/pyhanko/sign/fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """
 Utilities to deal with signature form fields and their properties in PDF files.
 """
 
 import logging
 from dataclasses import dataclass
-from enum import Flag, Enum, unique
-from typing import List, Optional, Union, Set
+from enum import Enum, Flag, unique
+from typing import List, Optional, Set, Union
 
 from asn1crypto import x509
 from asn1crypto.x509 import KeyUsage
-
-from pyhanko.pdf_utils.content import RawContent
-from pyhanko.pdf_utils.layout import BoxConstraints
 from pyhanko_certvalidator import InvalidCertificateError
 from pyhanko_certvalidator.path import ValidationPath
 
 from pyhanko.pdf_utils import generic
+from pyhanko.pdf_utils.content import RawContent
 from pyhanko.pdf_utils.generic import pdf_name, pdf_string
-from pyhanko.pdf_utils.misc import OrderedEnum, PdfWriteError, get_and_apply
+from pyhanko.pdf_utils.layout import BoxConstraints
+from pyhanko.pdf_utils.misc import (
+    OrderedEnum,
+    PdfReadError,
+    PdfWriteError,
+    get_and_apply,
+)
 from pyhanko.pdf_utils.rw_common import PdfHandler
 from pyhanko.pdf_utils.writer import BasePdfFileWriter
 from pyhanko.sign.general import (
-    UnacceptableSignerError, SigningError,
     KeyUsageConstraints,
+    SigningError,
+    UnacceptableSignerError,
 )
 
 __all__ = [
     'SigFieldSpec', 'SigSeedValFlags', 'SigCertConstraints',
     'SigSeedValueSpec', 'SigCertConstraintFlags', 'SigSeedSubFilter',
     'SeedValueDictVersion', 'SeedLockDocument', 'SigCertKeyUsage',
     'MDPPerm', 'FieldMDPAction', 'FieldMDPSpec',
@@ -1297,15 +1302,17 @@
         form = root['/AcroForm']
 
         try:
             fields = form['/Fields']
         except KeyError:
             raise ValueError('/AcroForm has no /Fields')
 
-        candidates = enumerate_sig_fields_in(fields, with_name=sig_field_name)
+        candidates = enumerate_sig_fields_in(
+            fields, with_name=sig_field_name, refs_seen=set()
+        )
         sig_field_ref = None
         try:
             field_name, value, sig_field_ref = next(candidates)
             if value is not None:
                 raise SigningError(
                     'Signature field with name %s appears to be filled already.'
                     % sig_field_name
@@ -1367,33 +1374,35 @@
     """
 
     try:
         fields = handler.root['/AcroForm']['/Fields']
     except KeyError:
         return
 
-    yield from enumerate_sig_fields_in(fields, filled_status)
+    yield from enumerate_sig_fields_in(fields, filled_status, refs_seen=set())
 
 
 def enumerate_sig_fields_in(field_list, filled_status=None, with_name=None,
-                            parent_name="", parents=None):
+                            parent_name="", parents=None, *, refs_seen):
     if not isinstance(field_list, generic.ArrayObject):
         logger.warning(
             f"Values of type {type(field_list)} are not valid as field "
             f"lists, must be array objects -- skipping."
         )
         return
 
     parents = parents or ()
     for field_ref in field_list:
         if not isinstance(field_ref, generic.IndirectObject):
             logger.warning(
                 "Entries in field list must be indirect references -- skipping."
             )
             continue
+        if field_ref.reference in refs_seen:
+            raise PdfReadError("Circular reference in form tree")
 
         field = field_ref.get_object()
         if not isinstance(field, generic.DictionaryObject):
             logger.warning(
                 "Entries in field list must be dictionary objects, not "
                 f"{type(field)} -- skipping."
             )
@@ -1437,15 +1446,16 @@
             )
 
         # if necessary, descend into the field hierarchy
         if with_name is None or (child_requested and not explicitly_requested):
             try:
                 yield from enumerate_sig_fields_in(
                     field['/Kids'], parent_name=fq_name, parents=current_path,
-                    with_name=with_name, filled_status=filled_status
+                    with_name=with_name, filled_status=filled_status,
+                    refs_seen=refs_seen | {field_ref.reference}
                 )
             except KeyError:
                 continue
 
 
 def append_signature_field(pdf_out: BasePdfFileWriter,
                            sig_field_spec: SigFieldSpec):
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/general.py` & `pyHanko-0.9.0/pyhanko/sign/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,45 +2,50 @@
 General tools related to Cryptographic Message Syntax (CMS) signatures,
 not necessarily to the extent implemented in the PDF specification.
 
 CMS is defined in :rfc:`5652`. To parse CMS messages, pyHanko relies heavily on
 `asn1crypto <https://github.com/wbond/asn1crypto>`_.
 """
 
+import hashlib
 import logging
 from dataclasses import dataclass
-from typing import ClassVar, Set, Optional, Tuple, Union
-
-import hashlib
+from typing import ClassVar, Optional, Set, Tuple, Union
 
-from asn1crypto import x509, cms, tsp, algos, pem, keys
+from asn1crypto import algos, cms, keys, pem, tsp, x509
 
 # noinspection PyProtectedMember
 from cryptography.exceptions import InvalidSignature
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric import padding
+from cryptography.hazmat.primitives.asymmetric.dsa import DSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.ec import (
-    EllipticCurvePublicKey, ECDSA
+    ECDSA,
+    EllipticCurvePublicKey,
 )
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.hazmat.primitives.asymmetric.utils import Prehashed
-
-from pyhanko.pdf_utils.config_utils import ConfigurableMixin, \
-    process_bit_string_flags, process_oids
-from pyhanko_certvalidator.path import ValidationPath
-
 from pyhanko_certvalidator import CertificateValidator
-from pyhanko_certvalidator.registry import (
-    CertificateStore, SimpleCertificateStore
-)
 from pyhanko_certvalidator.errors import (
-    RevokedError, PathValidationError, InvalidCertificateError,
-    PathBuildingError
+    InvalidCertificateError,
+    PathBuildingError,
+    PathValidationError,
+    RevokedError,
+)
+from pyhanko_certvalidator.path import ValidationPath
+from pyhanko_certvalidator.registry import (
+    CertificateStore,
+    SimpleCertificateStore,
 )
-from cryptography.hazmat.primitives import serialization, hashes
-from cryptography.hazmat.primitives.asymmetric import padding
 
+from pyhanko.pdf_utils.config_utils import (
+    ConfigurableMixin,
+    process_bit_string_flags,
+    process_oids,
+)
 
 __all__ = [
     'SignatureStatus', 'simple_cms_attribute',
     'find_cms_attribute', 'find_unique_cms_attribute',
     'extract_message_digest', 'validate_sig_integrity',
     'CertificateStore', 'SimpleCertificateStore',
     'KeyUsageConstraints',
@@ -340,16 +345,16 @@
         """
         if self.intact and self.valid:
             return 'INTACT:' + ','.join(self.summary_fields())
         else:
             return 'INVALID'
 
     @classmethod
-    def validate_cert_usage(cls, validator: CertificateValidator,
-                            key_usage_settings: KeyUsageConstraints = None):
+    async def validate_cert_usage(cls, validator: CertificateValidator,
+                                  key_usage_settings: KeyUsageConstraints = None):
         key_usage_settings = key_usage_settings or KeyUsageConstraints()
         key_usage_settings = KeyUsageConstraints(
             key_usage=(
                 cls.key_usage if key_usage_settings.key_usage is None
                 else key_usage_settings.key_usage
             ),
             extd_key_usage=(
@@ -361,15 +366,15 @@
 
         revoked = trusted = False
         path = None
 
         try:
             # validate usage without going through pyhanko_certvalidator
             key_usage_settings.validate(cert)
-            path = validator.validate_usage(key_usage=set())
+            path = await validator.async_validate_usage(key_usage=set())
             trusted = True
         except InvalidCertificateError as e:
             # TODO accumulate these somewhere
             logger.warning(e)
         except RevokedError:
             revoked = True
         except (PathValidationError, PathBuildingError) as e:
@@ -821,14 +826,17 @@
     elif sig_algo == 'rsassa_pss':
         assert isinstance(pub_key, RSAPublicKey)
         pss_padding, hash_algo = _process_pss_params(
             signature_algorithm['parameters'], md_algorithm,
             prehashed=prehashed
         )
         pub_key.verify(signature, signed_data, pss_padding, hash_algo)
+    elif sig_algo == 'dsa':
+        assert isinstance(pub_key, DSAPublicKey)
+        pub_key.verify(signature, signed_data, verify_md)
     elif sig_algo == 'ecdsa':
         assert isinstance(pub_key, EllipticCurvePublicKey)
         pub_key.verify(signature, signed_data, ECDSA(verify_md))
     else:  # pragma: nocover
         raise SignatureValidationError(
             f"Signature mechanism {sig_algo} is not supported."
         )
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/__init__.py` & `pyHanko-0.9.0/pyhanko/sign/signers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 """
 This package houses the part of pyHanko that produces digital signatures.
 It contains modules for creating ``SignedData`` CMS objects, embedding them
 in PDF files, and for handling PDF-specific document signing needs.
 """
 
-from .pdf_cms import Signer, SimpleSigner, ExternalSigner
-from .pdf_byterange import (
-    PdfByteRangeDigest, PdfSignedData, SignatureObject, DocumentTimestamp,
-)
-from .pdf_signer import PdfSignatureMetadata, PdfTimeStamper, PdfSigner
-from .functions import sign_pdf, embed_payload_with_cms
-
 # reexport this for backwards compatibility
 from pyhanko.sign.general import load_certs_from_pemder
 
 from .constants import (
-    DEFAULT_MD, DEFAULT_SIGNING_STAMP_STYLE, DEFAULT_SIG_SUBFILTER,
-    DEFAULT_SIGNER_KEY_USAGE
+    DEFAULT_MD,
+    DEFAULT_SIG_SUBFILTER,
+    DEFAULT_SIGNER_KEY_USAGE,
+    DEFAULT_SIGNING_STAMP_STYLE,
 )
-
+from .functions import async_sign_pdf, embed_payload_with_cms, sign_pdf
+from .pdf_byterange import (
+    DocumentTimestamp,
+    PdfByteRangeDigest,
+    PdfSignedData,
+    SignatureObject,
+)
+from .pdf_cms import ExternalSigner, Signer, SimpleSigner
+from .pdf_signer import PdfSignatureMetadata, PdfSigner, PdfTimeStamper
 
 __all__ = [
     'PdfSignatureMetadata', 'Signer', 'SimpleSigner', 'ExternalSigner',
     'PdfSigner', 'PdfTimeStamper',
     'PdfByteRangeDigest', 'PdfSignedData',
     'SignatureObject', 'DocumentTimestamp',
-    'sign_pdf', 'load_certs_from_pemder',
+    'sign_pdf', 'async_sign_pdf', 'load_certs_from_pemder',
     'DEFAULT_MD', 'DEFAULT_SIGNING_STAMP_STYLE', 'DEFAULT_SIG_SUBFILTER',
     'DEFAULT_SIGNER_KEY_USAGE'
 ]
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/cms_embedder.py` & `pyHanko-0.9.0/pyhanko/sign/signers/cms_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 This module describes and implements the low-level :class:`.PdfCMSEmbedder`
 protocol for embedding CMS payloads into PDF signature objects.
 """
 
 from dataclasses import dataclass
 from datetime import datetime
+from typing import IO, Optional
 
+from pyhanko.pdf_utils import generic, misc
+from pyhanko.pdf_utils.generic import pdf_name
+from pyhanko.pdf_utils.layout import BoxConstraints
 from pyhanko.pdf_utils.writer import BasePdfFileWriter
-from typing import Optional, IO
 from pyhanko.sign.fields import (
-    MDPPerm, SigFieldSpec, enumerate_sig_fields,
-    prepare_sig_field, ensure_sig_flags,
     FieldMDPSpec,
+    MDPPerm,
+    SigFieldSpec,
+    ensure_sig_flags,
+    enumerate_sig_fields,
+    prepare_sig_field,
 )
-from pyhanko.pdf_utils import generic, misc
-from pyhanko.pdf_utils.generic import pdf_name
-from pyhanko.pdf_utils.layout import BoxConstraints
 from pyhanko.sign.general import SigningError
 from pyhanko.stamp import BaseStampStyle, TextStampStyle
 
 from .pdf_byterange import PdfSignedData
 
 __all__ = [
     'PdfCMSEmbedder', 'SigMDPSetup', 'SigObjSetup',
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/constants.py` & `pyHanko-0.9.0/pyhanko/sign/signers/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 This module defines constants & defaults used by pyHanko when creating digital
 signatures.
 """
 from pyhanko.pdf_utils import generic
-from pyhanko.sign.fields import SigSeedSubFilter
-from pyhanko.stamp import TextStampStyle, STAMP_ART_CONTENT
 from pyhanko.pdf_utils.writer import DeveloperExtension, DevExtensionMultivalued
-
+from pyhanko.sign.fields import SigSeedSubFilter
+from pyhanko.stamp import STAMP_ART_CONTENT, TextStampStyle
 
 __all__ = [
     'DEFAULT_MD', 'DEFAULT_SIG_SUBFILTER', 'DEFAULT_SIGNER_KEY_USAGE',
     'SIG_DETAILS_DEFAULT_TEMPLATE', 'DEFAULT_SIGNING_STAMP_STYLE'
 ]
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/functions.py` & `pyHanko-0.9.0/pyhanko/sign/signers/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 This module defines pyHanko's high-level API entry points.
 """
 
-import tzlocal
 from datetime import datetime
 from typing import Optional
 
+import tzlocal
 from asn1crypto import cms
 
 from pyhanko.pdf_utils import embed
 from pyhanko.pdf_utils.writer import BasePdfFileWriter
 from pyhanko.sign.fields import SigFieldSpec
 from pyhanko.sign.general import SigningError
 from pyhanko.sign.timestamps import TimeStamper
 
 from .pdf_cms import Signer
 from .pdf_signer import PdfSignatureMetadata, PdfSigner
 
-
-__all__ = ['sign_pdf', 'embed_payload_with_cms']
+__all__ = ['sign_pdf', 'async_sign_pdf', 'embed_payload_with_cms']
 
 
 def sign_pdf(pdf_out: BasePdfFileWriter,
              signature_meta: PdfSignatureMetadata, signer: Signer,
              timestamper: TimeStamper = None,
              new_field_spec: Optional[SigFieldSpec] = None,
              existing_fields_only=False, bytes_reserved=None, in_place=False,
@@ -75,14 +74,72 @@
     )
     return signer.sign_pdf(
         pdf_out, existing_fields_only=existing_fields_only,
         bytes_reserved=bytes_reserved, in_place=in_place, output=output
     )
 
 
+async def async_sign_pdf(pdf_out: BasePdfFileWriter,
+                         signature_meta: PdfSignatureMetadata, signer: Signer,
+                         timestamper: TimeStamper = None,
+                         new_field_spec: Optional[SigFieldSpec] = None,
+                         existing_fields_only=False, bytes_reserved=None,
+                         in_place=False, output=None):
+    """
+    Thin convenience wrapper around :meth:`.PdfSigner.async_sign_pdf`.
+
+    :param pdf_out:
+        An :class:`.IncrementalPdfFileWriter`.
+    :param bytes_reserved:
+        Bytes to reserve for the CMS object in the PDF file.
+        If not specified, make an estimate based on a dummy signature.
+    :param signature_meta:
+        The specification of the signature to add.
+    :param signer:
+        :class:`.Signer` object to use to produce the signature object.
+    :param timestamper:
+        :class:`.TimeStamper` object to use to produce any time stamp tokens
+        that might be required.
+    :param in_place:
+        Sign the input in-place. If ``False``, write output to a
+        :class:`.BytesIO` object.
+    :param existing_fields_only:
+        If ``True``, never create a new empty signature field to contain
+        the signature.
+        If ``False``, a new field may be created if no field matching
+        :attr:`~.PdfSignatureMetadata.field_name` exists.
+    :param new_field_spec:
+        If a new field is to be created, this parameter allows the caller
+        to specify the field's properties in the form of a
+        :class:`.SigFieldSpec`. This parameter is only meaningful if
+        ``existing_fields_only`` is ``False``.
+    :param output:
+        Write the output to the specified output stream.
+        If ``None``, write to a new :class:`.BytesIO` object.
+        Default is ``None``.
+    :return:
+        The output stream containing the signed output.
+    """
+
+    if new_field_spec is not None and existing_fields_only:
+        raise SigningError(
+            "Specifying a signature field spec is not meaningful when "
+            "existing_fields_only=True."
+        )
+
+    signer = PdfSigner(
+        signature_meta, signer, timestamper=timestamper,
+        new_field_spec=new_field_spec
+    )
+    return await signer.async_sign_pdf(
+        pdf_out, existing_fields_only=existing_fields_only,
+        bytes_reserved=bytes_reserved, in_place=in_place, output=output
+    )
+
+
 def embed_payload_with_cms(pdf_writer: BasePdfFileWriter,
                            file_spec_string: str,
                            payload: embed.EmbeddedFileObject,
                            cms_obj: cms.ContentInfo, extension='.sig',
                            file_name: Optional[str] = None,
                            file_spec_kwargs=None, cms_file_spec_kwargs=None):
     """
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/pdf_byterange.py` & `pyHanko-0.9.0/pyhanko/sign/signers/pdf_byterange.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 This module contains the low-level building blocks for dealing with bookkeeping
 around ``/ByteRange`` digests in PDF files.
 """
 
-from dataclasses import dataclass
-from io import BytesIO
 import binascii
-from cryptography.hazmat.primitives import hashes
+from dataclasses import dataclass
 from datetime import datetime
+from io import BytesIO
+from typing import IO, Optional, Union
+
 from asn1crypto import cms
-from typing import Optional, Union, IO
-from pyhanko.pdf_utils import generic
-from pyhanko.pdf_utils import misc
-from pyhanko.pdf_utils.generic import pdf_name, pdf_date, pdf_string
-from pyhanko.pdf_utils.writer import BasePdfFileWriter
+from cryptography.hazmat.primitives import hashes
+
+from pyhanko.pdf_utils import generic, misc
+from pyhanko.pdf_utils.generic import pdf_date, pdf_name, pdf_string
 from pyhanko.pdf_utils.incremental_writer import IncrementalPdfFileWriter
+from pyhanko.pdf_utils.writer import BasePdfFileWriter
 from pyhanko.sign.general import SigningError, get_pyca_cryptography_hash
-from . import constants
+
 from ..fields import SigSeedSubFilter
+from . import constants
 
 __all__ = [
     # Serialisable object used to track placeholder locations,
     # part of PdfCMSEmbedder / PdfSigner protocol
     'PreparedByteRangeDigest',
     # PDF-level signature containers
     'PdfByteRangeDigest', 'PdfSignedData', 'SignatureObject',
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/pdf_cms.py` & `pyHanko-0.9.0/pyhanko/sign/signers/pdf_cms.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,208 @@
 """
 This module defines utility classes to format CMS objects for use in PDF
 signatures.
 """
-
+import asyncio
 import logging
+import warnings
 from dataclasses import dataclass
-from typing import Optional, Union, IO
 from datetime import datetime
-from cryptography.hazmat.primitives import serialization, hashes
-from cryptography.hazmat.primitives.asymmetric.ec import \
-    EllipticCurvePrivateKey, ECDSA
+from typing import IO, Iterable, List, Optional, Union
+
+from asn1crypto import algos, cms, core, keys
+from asn1crypto import pdf as asn1_pdf
+from asn1crypto import x509
+from asn1crypto.algos import SignedDigestAlgorithm
+from cryptography.hazmat.primitives import hashes, serialization
+from cryptography.hazmat.primitives.asymmetric.dsa import DSAPrivateKey
+from cryptography.hazmat.primitives.asymmetric.ec import (
+    ECDSA,
+    EllipticCurvePrivateKey,
+)
 from cryptography.hazmat.primitives.asymmetric.padding import PKCS1v15
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 from cryptography.hazmat.primitives.serialization import pkcs12
-from asn1crypto import x509, cms, core, keys, algos, pdf as asn1_pdf
-from asn1crypto.algos import SignedDigestAlgorithm
+from pyhanko_certvalidator._asyncio_compat import to_thread
+
+from pyhanko.pdf_utils import misc
+from pyhanko.sign import attributes
+from pyhanko.sign.ades.api import CAdESSignedAttrSpec
+from pyhanko.sign.attributes import CMSAttributeProvider
 from pyhanko.sign.general import (
-    CertificateStore, SimpleCertificateStore,
-    SigningError, optimal_pss_params, simple_cms_attribute,
-    get_pyca_cryptography_hash, as_signing_certificate_v2,
-    load_private_key_from_pemder, load_cert_from_pemder,
-    load_certs_from_pemder, _process_pss_params,
+    CertificateStore,
+    SigningError,
+    SimpleCertificateStore,
+    _process_pss_params,
     _translate_pyca_cryptography_cert_to_asn1,
-    _translate_pyca_cryptography_key_to_asn1
+    _translate_pyca_cryptography_key_to_asn1,
+    get_pyca_cryptography_hash,
+    load_cert_from_pemder,
+    load_certs_from_pemder,
+    load_private_key_from_pemder,
+    optimal_pss_params,
+    simple_cms_attribute,
 )
-from pyhanko.pdf_utils import misc
-from pyhanko.sign.ades.api import CAdESSignedAttrSpec
+from pyhanko.sign.timestamps import TimeStamper
+
+from . import constants
 
 __all__ = [
-    'Signer', 'SimpleSigner', 'ExternalSigner',
-    'PdfCMSSignedAttributes'
+    'Signer', 'SimpleSigner', 'ExternalSigner', 'PdfCMSSignedAttributes',
+    'format_attributes', 'format_signed_attributes',
+    'asyncify_signer', 'select_suitable_signing_md'
 ]
 
 logger = logging.getLogger(__name__)
 
 
+@dataclass(frozen=True)
+class PdfCMSSignedAttributes:
+    """
+    .. versionadded:: 0.7.0
+
+    Serialisable container class describing input for various signed attributes
+    in a CMS object for a PDF signature.
+    """
+
+    signing_time: Optional[datetime] = None
+    """
+    Timestamp for the ``signingTime`` attribute. Will be ignored in a PAdES
+    context.
+    """
+
+    adobe_revinfo_attr: Optional[asn1_pdf.RevocationInfoArchival] = None
+    """
+    Adobe-style signed revocation info attribute.
+    """
+
+    cades_signed_attrs: Optional[CAdESSignedAttrSpec] = None
+    """
+    Optional settings for CAdES-style signed attributes.
+    """
+
+
+def _ensure_content_type(encap_content_info):
+
+    encap_content_info = encap_content_info or {'content_type': 'data'}
+    if isinstance(encap_content_info, core.Sequence):
+        # could be cms.ContentInfo or cms.EncapsulatedContentInfo depending
+        # on circumstances, so let's just stick to Sequence
+        content_type = encap_content_info['content_type'].native
+    else:
+        content_type = encap_content_info.get('content_type', 'data')
+
+    return encap_content_info, content_type
+
+
+def _cms_version(content_type: Union[str, core.ObjectIdentifier]):
+    if isinstance(content_type, core.ObjectIdentifier):
+        content_type = content_type.native
+
+    return 'v1' if content_type == 'data' else 'v3'
+
+
+def _prepare_encap_content(input_data: Union[IO, bytes,
+                                             cms.ContentInfo,
+                                             cms.EncapsulatedContentInfo],
+                           digest_algorithm: str, detached=True,
+                           chunk_size=misc.DEFAULT_CHUNK_SIZE,
+                           max_read=None):
+
+    h = hashes.Hash(get_pyca_cryptography_hash(digest_algorithm))
+    encap_content_info = None
+    if isinstance(input_data,
+                  (cms.ContentInfo, cms.EncapsulatedContentInfo)):
+        h.update(bytes(input_data['content']))
+        if detached:
+            encap_content_info = {
+                'content_type': input_data['content_type']
+            }
+        else:
+            encap_content_info = input_data
+    elif isinstance(input_data, bytes):
+        h.update(input_data)
+        if not detached:
+            # use dicts instead of Asn1Value objects, to leave asn1crypto
+            # to decide whether to use cms.ContentInfo or
+            # cms.EncapsulatedContentInfo (for backwards compat with PCKS#7)
+            encap_content_info = {
+                'content_type': 'data', 'content': input_data
+            }
+    elif not detached:
+        # input stream is a buffer, and we're in 'enveloping' mode
+        # read the entire thing into memory, since we need to embed
+        # it anyway
+        input_bytes = input_data.read(max_read)
+        h.update(input_bytes)
+        # see above
+        encap_content_info = {
+            'content_type': 'data',
+            'content': input_bytes
+        }
+    else:
+        temp_buf = bytearray(chunk_size)
+        misc.chunked_digest(temp_buf, input_data, h, max_read=max_read)
+    digest_bytes = h.finalize()
+    return encap_content_info, digest_bytes
+
+
+async def format_attributes(attr_provs: List[CMSAttributeProvider],
+                            other_attrs: Iterable[cms.CMSAttributes] = (),
+                            dry_run: bool = False) -> cms.CMSAttributes:
+    """
+    Format CMS attributes obtained from attribute providers.
+
+    :param attr_provs:
+        List of attribute providers.
+    :param other_attrs:
+        Other (predetermined) attributes to include.
+    :param dry_run:
+        Whether to invoke the attribute providers in dry-run mode or not.
+    :return:
+        A :class:`cms.CMSAttributes` value.
+    """
+
+    attrs = list(other_attrs)
+    jobs = [prov.get_attribute(dry_run=dry_run) for prov in attr_provs]
+    for attr_coro in asyncio.as_completed(jobs):
+        attr = await attr_coro
+        if attr is not None:
+            attrs.append(attr)
+
+    return cms.CMSAttributes(attrs)
+
+
+async def format_signed_attributes(data_digest: bytes,
+                                   attr_provs: List[CMSAttributeProvider],
+                                   content_type='data',
+                                   dry_run=False) -> cms.CMSAttributes:
+    """
+    Format signed attributes for a CMS ``SignerInfo`` value.
+
+    :param data_digest:
+        The byte string to put in the ``messageDigest`` attribute.
+    :param attr_provs:
+        List of attribute providers to source attributes from.
+    :param content_type:
+        The content type of the data being signed (default is ``data``).
+    :param dry_run:
+        Whether to invoke the attribute providers in dry-run mode or not.
+    :return:
+        A :class:`cms.CMSAttributes` value representing the signed attributes.
+    """
+    attrs = [
+        simple_cms_attribute('content_type', content_type),
+        simple_cms_attribute('message_digest', data_digest),
+    ]
+    return await format_attributes(
+        attr_provs, dry_run=dry_run, other_attrs=attrs
+    )
+
+
 class Signer:
     """
     Abstract signer object that is agnostic as to where the cryptographic
     operations actually happen.
 
     As of now, pyHanko provides two implementations:
 
@@ -48,14 +212,38 @@
       capable of interfacing with a PKCS11 device
       (see also :class:`~pyhanko.sign.beid.BEIDSigner`).
 
     :param prefer_pss:
         When signing using an RSA key, prefer PSS padding to legacy PKCS#1 v1.5
         padding. Default is ``False``. This option has no effect on non-RSA
         signatures.
+    :param embed_roots:
+        .. versionadded:: 0.9.0
+
+        Option that controls whether or not additional self-signed certificates
+        should be embedded into the CMS payload. The default is ``True``.
+
+        .. note::
+            The signer's certificate is always embedded, even if it is
+            self-signed.
+
+        .. note::
+            Trust roots are configured by the validator, so embedding them
+            typically does nothing in a typical validation process.
+            Therefore they can be safely omitted in most cases.
+            Nonetheless, embedding the roots can be useful for documentation
+            purposes.
+
+        .. warning::
+            To be precise, if this flag is ``False``, a certificate will be
+            dropped if (a) it is not the signer's, (b) it is self-issued and
+            (c) its subject and authority key identifiers match (or either is
+            missing). In other words, we never validate the actual
+            self-signature. This heuristic is sufficiently accurate
+            for most applications.
     """
 
     signing_cert: x509.Certificate
     """
     The certificate that will be used to create the signature.
     """
 
@@ -67,16 +255,17 @@
     """
 
     signature_mechanism: SignedDigestAlgorithm = None
     """
     The (cryptographic) signature mechanism to use.
     """
 
-    def __init__(self, prefer_pss=False):
+    def __init__(self, prefer_pss=False, embed_roots=True):
         self.prefer_pss = prefer_pss
+        self.embed_roots = embed_roots
 
     def get_signature_mechanism(self, digest_algorithm):
         """
         Get the signature mechanism for this signer to use.
         If :attr:`signature_mechanism` is set, it will be used.
         Otherwise, this method will attempt to put together a default
         based on mechanism used in the signer's certificate.
@@ -106,14 +295,23 @@
             # The correspondence with the digestAlgorithm field in CMS is
             # verified separately.
             if digest_algorithm is None:
                 raise ValueError(
                     "Digest algorithm required for ECDSA"
                 )
             mech = digest_algorithm + '_ecdsa'
+        elif algo == 'dsa':
+            if digest_algorithm is None:
+                raise ValueError("Digest algorithm required for DSA")
+            # Note: DSA isn't specified with sha384 and sha512, but we
+            # don't check that here; let's allow the error to percolate
+            # further down for now.
+            # TODO (but maybe it's worth revisiting the issue of checking
+            #  signature <> hash algorithm combinations in greater generality)
+            mech = digest_algorithm + '_dsa'
         elif algo == 'rsa':
             if self.prefer_pss:
                 mech = 'rsassa_pss'
                 if digest_algorithm is None:
                     raise ValueError(
                         "Digest algorithm required for RSASSA-PSS"
                     )
@@ -128,36 +326,14 @@
             )
 
         sda_kwargs = {'algorithm': mech}
         if params is not None:
             sda_kwargs['parameters'] = params
         return SignedDigestAlgorithm(sda_kwargs)
 
-    def sign_raw(self, data: bytes, digest_algorithm: str, dry_run=False) \
-            -> bytes:
-        """
-        Compute the raw cryptographic signature of the data provided, hashed
-        using the digest algorithm provided.
-
-        :param data:
-            Data to sign.
-        :param digest_algorithm:
-            Digest algorithm to use.
-
-            .. warning::
-                If :attr:`signature_mechanism` also specifies a digest, they
-                should match.
-        :param dry_run:
-            Do not actually create a signature, but merely output placeholder
-            bytes that would suffice to contain an actual signature.
-        :return:
-            Signature bytes.
-        """
-        raise NotImplementedError
-
     @property
     def subject_name(self):
         """
         :return:
             The subject's common name as a string, extracted from
             :attr:`signing_cert`.
         """
@@ -176,222 +352,497 @@
         Format Adobe-style revocation information for inclusion into a CMS
         object.
 
         :param ocsp_responses:
             A list of OCSP responses to include.
         :param crls:
             A list of CRLs to include.
-        :return:
-            A CMS attribute containing the relevant data.
         """
 
         revinfo_dict = {}
         if ocsp_responses:
             revinfo_dict['ocsp'] = ocsp_responses
 
         if crls:
             revinfo_dict['crl'] = crls
 
         if revinfo_dict:
-            revinfo = asn1_pdf.RevocationInfoArchival(revinfo_dict)
-            return simple_cms_attribute(
-                'adobe_revocation_info_archival', revinfo
+            return asn1_pdf.RevocationInfoArchival(revinfo_dict)
+
+    def _signed_attr_providers(self, data_digest: bytes, digest_algorithm: str,
+                               attr_settings: PdfCMSSignedAttributes,
+                               timestamper=None, use_pades=False):
+        """
+        Prepare "standard" signed attribute providers. Internal API.
+        """
+        yield attributes.SigningCertificateV2Provider(
+            signing_cert=self.signing_cert
+        )
+        if not use_pades:
+            signing_time = attr_settings.signing_time
+            if signing_time is not None:
+                # NOTE: PAdES actually forbids this!
+                yield attributes.SigningTimeProvider(timestamp=signing_time)
+            if attr_settings.adobe_revinfo_attr is not None:
+                yield attributes.AdobeRevinfoProvider(
+                    value=attr_settings.adobe_revinfo_attr
+                )
+
+            # TODO not sure if PAdES allows this, need to check.
+            #  It *should*, but perhaps the version of CMS it is based on is too
+            #  old, or it might not allow undefined signed attributes.
+            # In the meantime, we only add this attribute to non-PAdES sigs
+            yield attributes.CMSAlgorithmProtectionProvider(
+                digest_algo=digest_algorithm,
+                signature_algo=self.get_signature_mechanism(digest_algorithm)
             )
+        cades_meta = attr_settings.cades_signed_attrs
+        # apply CAdES-specific attributes regardless of use_pades
+        if cades_meta is not None:
+            yield from cades_meta.prepare_providers(
+                message_digest=data_digest,
+                md_algorithm=digest_algorithm,
+                timestamper=timestamper
+            )
+
+    def _unsigned_attr_providers(self, digest_algorithm, signature: bytes,
+                                 timestamper: Optional[TimeStamper] = None):
+        """
+        Prepare "standard" unsigned attribute providers. Internal API.
+        """
+        if timestamper is not None:
+            # the timestamp server needs to cross-sign our signature
+            yield attributes.TSTProvider(
+                digest_algorithm=digest_algorithm, data_to_ts=signature,
+                timestamper=timestamper
+            )
+
+    def signer_info(self, digest_algorithm: str, signed_attrs, signature):
+        """
+        Format the ``SignerInfo`` entry for a CMS signature.
 
-    def signed_attrs(self, data_digest: bytes, digest_algorithm: str,
-                     timestamp: datetime = None, content_type='data',
-                     revocation_info=None, use_pades=False,
-                     cades_meta: CAdESSignedAttrSpec = None,
-                     timestamper=None, dry_run=False):
+        :param digest_algorithm:
+            Digest algorithm to use.
+        :param signed_attrs:
+            Signed attributes (see :meth:`signed_attrs`).
+        :param signature:
+            The raw signature to embed (see :meth:`sign_raw`).
+        :return:
+            An :class:`.asn1crypto.cms.SignerInfo` object.
+        """
+        digest_algorithm_obj = algos.DigestAlgorithm(
+            {'algorithm': digest_algorithm}
+        )
+
+        signing_cert = self.signing_cert
+        # build the signer info object that goes into the PKCS7 signature
+        # (see RFC 2315 § 9.2)
+        sig_info = cms.SignerInfo({
+            'version': 'v1',
+            'sid': cms.SignerIdentifier({
+                'issuer_and_serial_number': cms.IssuerAndSerialNumber({
+                    'issuer': signing_cert.issuer,
+                    'serial_number': signing_cert.serial_number,
+                })
+            }),
+            'digest_algorithm': digest_algorithm_obj,
+            'signature_algorithm': self.get_signature_mechanism(
+                digest_algorithm
+            ),
+            'signed_attrs': signed_attrs,
+            'signature': signature
+        })
+        return sig_info
+
+    def _package_signature(self, *, digest_algorithm: str,
+                           cms_version, signed_attrs: cms.CMSAttributes,
+                           signature: bytes, unsigned_attrs: cms.CMSAttributes,
+                           encap_content_info) -> cms.ContentInfo:
+
+        encap_content_info = encap_content_info or {'content_type': 'data'}
+        digest_algorithm_obj = algos.DigestAlgorithm(
+            {'algorithm': digest_algorithm}
+        )
+        sig_info = self.signer_info(digest_algorithm, signed_attrs, signature)
+
+        if unsigned_attrs is not None:
+            sig_info['unsigned_attrs'] = unsigned_attrs
+
+        # Note: we do not add the TS certs at this point
+        if self.embed_roots:
+            certs = set(self.cert_registry)
+        else:
+            # asn1crypto's heuristic is good enough for now, we won't check the
+            # actual signatures. CAs that make use of self-issued certificates
+            # for things like key rollover probably also use SKI/AKI to
+            # distinguish between different certs, which will be picked up by
+            # asn1crypto either way.
+            certs = {
+                cert for cert in self.cert_registry
+                if cert.self_signed == 'no'
+            }
+        certs.add(self.signing_cert)
+        # this is the SignedData object for our message (see RFC 2315 § 9.1)
+        signed_data = {
+            'version': cms_version,
+            'digest_algorithms': cms.DigestAlgorithms((digest_algorithm_obj,)),
+            'encap_content_info': encap_content_info,
+            'certificates': certs,
+            'signer_infos': [sig_info]
+        }
+
+        return cms.ContentInfo({
+            'content_type': cms.ContentType('signed_data'),
+            'content': cms.SignedData(signed_data)
+        })
+
+    def _check_digest_algorithm(self, digest_algorithm: str):
+
+        implied_hash_algo = None
+        try:
+            if self.signature_mechanism is not None:
+                implied_hash_algo = self.signature_mechanism.hash_algo
+        except ValueError:
+            # this is OK, just use the specified message digest
+            pass
+        if implied_hash_algo is not None \
+                and implied_hash_algo != digest_algorithm:
+            raise SigningError(
+                f"Selected signature mechanism specifies message digest "
+                f"{implied_hash_algo}, but {digest_algorithm} "
+                f"was requested."
+            )
+
+    async def async_sign_raw(self, data: bytes, digest_algorithm: str,
+                             dry_run=False) -> bytes:
+        """
+        Compute the raw cryptographic signature of the data provided, hashed
+        using the digest algorithm provided.
+
+        :param data:
+            Data to sign.
+        :param digest_algorithm:
+            Digest algorithm to use.
+
+            .. warning::
+                If :attr:`signature_mechanism` also specifies a digest, they
+                should match.
+        :param dry_run:
+            Do not actually create a signature, but merely output placeholder
+            bytes that would suffice to contain an actual signature.
+        :return:
+            Signature bytes.
+        """
+        raise NotImplementedError
+
+    async def unsigned_attrs(self, digest_algorithm, signature: bytes,
+                             timestamper=None, dry_run=False) \
+            -> Optional[cms.CMSAttributes]:
+        """
+        .. versionchanged:: 0.9.0
+            Made asynchronous _(breaking change)_
+
+        Compute the unsigned attributes to embed into the CMS object.
+        This function is called after signing the hash of the signed attributes
+        (see :meth:`signed_attrs`).
+
+        By default, this method only handles timestamp requests, but other
+        functionality may be added by subclasses
+
+        If this method returns ``None``, no unsigned attributes will be
+        embedded.
+
+        :param digest_algorithm:
+            Digest algorithm used to hash the signed attributes.
+        :param signature:
+            Signature of the signed attribute hash.
+        :param timestamper:
+            Timestamp supplier to use.
+        :param dry_run:
+            Flag indicating "dry run" mode. If ``True``, only the approximate
+            size of the output matters, so cryptographic
+            operations can be replaced by placeholders.
+        :return:
+            The unsigned attributes to add, or ``None``.
+        """
+        provs = self._unsigned_attr_providers(
+            digest_algorithm=digest_algorithm, signature=signature,
+            timestamper=timestamper
+        )
+        return await format_attributes(list(provs), dry_run=dry_run)
+
+    async def signed_attrs(self, data_digest: bytes,
+                           digest_algorithm: str,
+                           attr_settings: PdfCMSSignedAttributes = None,
+                           content_type='data', use_pades=False,
+                           timestamper=None, dry_run=False):
         """
         .. versionchanged:: 0.4.0
             Added positional ``digest_algorithm`` parameter _(breaking change)_.
         .. versionchanged:: 0.5.0
             Added ``dry_run``, ``timestamper`` and ``cades_meta`` parameters.
+        .. versionchanged:: 0.9.0
+            Made asynchronous, grouped some parameters under ``attr_settings``
+            _(breaking change)_
 
         Format the signed attributes for a CMS signature.
 
         :param data_digest:
             Raw digest of the data to be signed.
         :param digest_algorithm:
             .. versionadded:: 0.4.0
 
             Name of the digest algorithm used to compute the digest.
-        :param timestamp:
-            Current timestamp (ignored when ``use_pades`` is ``True``).
-        :param revocation_info:
-            Revocation information to embed; this should be the output
-            of a call to :meth:`.Signer.format_revinfo` or ``None``
-            (ignored when ``use_pades`` is ``True``).
         :param use_pades:
             Respect PAdES requirements.
         :param dry_run:
             .. versionadded:: 0.5.0
 
             Flag indicating "dry run" mode. If ``True``, only the approximate
             size of the output matters, so cryptographic
             operations can be replaced by placeholders.
+        :param attr_settings:
+            :class:`.PdfCMSSignedAttributes` object describing the attributes
+            to be added.
         :param timestamper:
             .. versionadded:: 0.5.0
 
             Timestamper to use when creating timestamp tokens.
-        :param cades_meta:
-            .. versionadded:: 0.5.0
-
-            Specification for CAdES-specific attributes.
         :param content_type:
             CMS content type of the encapsulated data. Default is `data`.
 
             .. danger::
                 This parameter is internal API, and non-default values must not
                 be used to produce PDF signatures.
         :return:
             An :class:`.asn1crypto.cms.CMSAttributes` object.
         """
 
-        attrs = [
-            simple_cms_attribute('content_type', content_type),
-            simple_cms_attribute('message_digest', data_digest),
-            # required by PAdES
-            simple_cms_attribute(
-                'signing_certificate_v2',
-                as_signing_certificate_v2(self.signing_cert)
-            )
-        ]
+        attr_settings = attr_settings or PdfCMSSignedAttributes()
 
-        # the following attributes are only meaningful in non-PAdES signatures
-        #  (i.e. old school PKCS7 with Adobe-style revocation info)
-        if not use_pades:
-            if timestamp is not None:
-                # NOTE: PAdES actually forbids this!
-                st = simple_cms_attribute(
-                    'signing_time',
-                    cms.Time({'utc_time': core.UTCTime(timestamp)})
-                )
-                attrs.append(st)
+        provs = self._signed_attr_providers(
+            data_digest=data_digest, digest_algorithm=digest_algorithm,
+            use_pades=use_pades, attr_settings=attr_settings,
+            timestamper=timestamper
+        )
 
-            # this is not allowed under PAdES, should use DSS instead
-            if revocation_info:
-                attrs.append(revocation_info)
+        return await format_signed_attributes(
+            data_digest, attr_provs=list(provs),
+            content_type=content_type, dry_run=dry_run
+        )
 
-            # TODO not sure if PAdES allows this, need to check.
-            #  It *should*, but perhaps the version of CMS it is based on is too
-            #  old, or it might not allow undefined signed attributes.
-            # In the meantime, we only add this attribute to non-PAdES sigs
-            algid_protection = cms.CMSAlgorithmProtection({
-                'digest_algorithm': algos.DigestAlgorithm(
-                    {'algorithm': digest_algorithm}
-                ),
-                'signature_algorithm':
-                    self.get_signature_mechanism(digest_algorithm)
-            })
-            attrs.append(
-                simple_cms_attribute(
-                    'cms_algorithm_protection', algid_protection
-                )
-            )
+    async def async_sign(self, data_digest: bytes, digest_algorithm: str,
+                         dry_run=False, use_pades=False, timestamper=None,
+                         signed_attr_settings: PdfCMSSignedAttributes = None,
+                         encap_content_info=None) -> cms.ContentInfo:
 
-        # apply CAdES-specific attributes regardless of use_pades
-        if cades_meta is not None:
-            cades_attrs = cades_meta.extra_signed_attributes(
-                data_digest, digest_algorithm, timestamper=timestamper,
-                dry_run=dry_run
-            )
-            attrs.extend(cades_attrs)
+        """
+        .. versionadded:: 0.9.0
 
-        return cms.CMSAttributes(attrs)
+        Produce a detached CMS signature from a raw data digest.
 
-    def unsigned_attrs(self, digest_algorithm, signature: bytes,
-                       timestamper=None, dry_run=False) \
-            -> Optional[cms.CMSAttributes]:
+        :param data_digest:
+            Digest of the actual content being signed.
+        :param digest_algorithm:
+            Digest algorithm to use. This should be the same digest method
+            as the one used to hash the (external) content.
+        :param dry_run:
+            If ``True``, the actual signing step will be replaced with
+            a placeholder.
+
+            In a PDF signing context, this is necessary to estimate the size
+            of the signature container before computing the actual digest of
+            the document.
+        :param signed_attr_settings:
+            :class:`.PdfCMSSignedAttributes` object describing the attributes
+            to be added.
+        :param use_pades:
+            Respect PAdES requirements.
+        :param timestamper:
+            :class:`~.timestamps.TimeStamper` used to obtain a trusted timestamp
+            token that can be embedded into the signature container.
+
+            .. note::
+                If ``dry_run`` is true, the timestamper's
+                :meth:`~.timestamps.TimeStamper.dummy_response` method will be
+                called to obtain a placeholder token.
+                Note that with a standard :class:`~.timestamps.HTTPTimeStamper`,
+                this might still hit the timestamping server (in order to
+                produce a realistic size estimate), but the dummy response will
+                be cached.
+        :param encap_content_info:
+            Data to encapsulate in the CMS object.
+
+            .. danger::
+                This parameter is internal API, and must not be used to produce
+                PDF signatures.
+        :return:
+            An :class:`~.asn1crypto.cms.ContentInfo` object.
         """
-        Compute the unsigned attributes to embed into the CMS object.
-        This function is called after signing the hash of the signed attributes
-        (see :meth:`signed_attrs`).
 
-        By default, this method only handles timestamp requests, but other
-        functionality may be added by subclasses
+        encap_content_info, content_type \
+            = _ensure_content_type(encap_content_info)
+        signed_attrs = await self.signed_attrs(
+            data_digest, digest_algorithm, attr_settings=signed_attr_settings,
+            use_pades=use_pades, timestamper=timestamper,
+            dry_run=dry_run, content_type=content_type
+        )
+        return await self.async_sign_prescribed_attributes(
+            digest_algorithm, signed_attrs,
+            cms_version=_cms_version(content_type),
+            dry_run=dry_run, timestamper=timestamper,
+            encap_content_info=encap_content_info
+        )
 
-        If this method returns ``None``, no unsigned attributes will be
-        embedded.
+    async def async_sign_prescribed_attributes(self, digest_algorithm: str,
+                                               signed_attrs: cms.CMSAttributes,
+                                               cms_version='v1',
+                                               dry_run=False, timestamper=None,
+                                               encap_content_info=None) \
+            -> cms.ContentInfo:
+        """
+        .. versionadded:: 0.9.0
+
+        Start the CMS signing process with the prescribed set of signed
+        attributes.
 
         :param digest_algorithm:
-            Digest algorithm used to hash the signed attributes.
-        :param signature:
-            Signature of the signed attribute hash.
-        :param timestamper:
-            Timestamp supplier to use.
+            Digest algorithm to use. This should be the same digest method
+            as the one used to hash the (external) content.
+        :param signed_attrs:
+            CMS attributes to sign.
         :param dry_run:
-            Flag indicating "dry run" mode. If ``True``, only the approximate
-            size of the output matters, so cryptographic
-            operations can be replaced by placeholders.
+            If ``True``, the actual signing step will be replaced with
+            a placeholder.
+
+            In a PDF signing context, this is necessary to estimate the size
+            of the signature container before computing the actual digest of
+            the document.
+        :param timestamper:
+            :class:`~.timestamps.TimeStamper` used to obtain a trusted timestamp
+            token that can be embedded into the signature container.
+
+            .. note::
+                If ``dry_run`` is true, the timestamper's
+                :meth:`~.timestamps.TimeStamper.dummy_response` method will be
+                called to obtain a placeholder token.
+                Note that with a standard :class:`~.timestamps.HTTPTimeStamper`,
+                this might still hit the timestamping server (in order to
+                produce a realistic size estimate), but the dummy response will
+                be cached.
+        :param cms_version:
+            CMS version to use.
+        :param encap_content_info:
+            Data to encapsulate in the CMS object.
+
+            .. danger::
+                This parameter is internal API, and must not be used to produce
+                PDF signatures.
         :return:
-            The unsigned attributes to add, or ``None``.
+            An :class:`~.asn1crypto.cms.ContentInfo` object.
         """
 
-        if timestamper is not None:
-            # the timestamp server needs to cross-sign our signature
+        digest_algorithm = digest_algorithm.lower()
+        self._check_digest_algorithm(digest_algorithm)
 
-            md_spec = get_pyca_cryptography_hash(digest_algorithm)
-            md = hashes.Hash(md_spec)
-            md.update(signature)
-            if dry_run:
-                ts_token = timestamper.dummy_response(digest_algorithm)
-            else:
-                ts_token = timestamper.timestamp(
-                    md.finalize(), digest_algorithm
-                )
-            return cms.CMSAttributes(
-                [simple_cms_attribute('signature_time_stamp_token', ts_token)]
-            )
+        signature = await self.async_sign_raw(
+            signed_attrs.dump(), digest_algorithm.lower(), dry_run
+        )
+        unsigned_attrs = await self.unsigned_attrs(
+            digest_algorithm, signature, timestamper=timestamper,
+            dry_run=dry_run
+        )
+        return self._package_signature(
+            digest_algorithm=digest_algorithm, cms_version=cms_version,
+            signed_attrs=signed_attrs, signature=signature,
+            unsigned_attrs=unsigned_attrs, encap_content_info=encap_content_info
+        )
 
-    def signer_info(self, digest_algorithm: str, signed_attrs, signature):
+    async def async_sign_general_data(
+            self,
+            input_data: Union[IO, bytes,
+                              cms.ContentInfo,
+                              cms.EncapsulatedContentInfo],
+            digest_algorithm: str, detached=True,
+            use_cades=False, timestamper=None,
+            chunk_size=misc.DEFAULT_CHUNK_SIZE,
+            signed_attr_settings:
+            PdfCMSSignedAttributes = None,
+            max_read=None) -> cms.ContentInfo:
         """
-        Format the ``SignerInfo`` entry for a CMS signature.
+        .. versionadded:: 0.9.0
+
+        Produce a CMS signature for an arbitrary data stream
+        (not necessarily PDF data).
+
+        :param input_data:
+            The input data to sign. This can be either a :class:`bytes` object
+            a file-type object, a :class:`cms.ContentInfo` object or
+            a :class:`cms.EncapsulatedContentInfo` object.
+
+            .. warning::
+                ``asn1crypto`` mandates :class:`cms.ContentInfo` for CMS v1
+                signatures. In practical terms, this means that you need to
+                use :class:`cms.ContentInfo` if the content type is ``data``,
+                and :class:`cms.EncapsulatedContentInfo` otherwise.
 
+            .. warning::
+                We currently only support CMS v1 and v3 signatures.
+                This is only a concern if you need attribute certificate
+                support, in which case you can override the CMS version number
+                yourself (this will not invalidate any signatures).
         :param digest_algorithm:
-            Digest algorithm to use.
-        :param signed_attrs:
-            Signed attributes (see :meth:`signed_attrs`).
-        :param signature:
-            The raw signature to embed (see :meth:`sign_raw`).
+            The name of the digest algorithm to use.
+        :param detached:
+            If ``True``, create a CMS detached signature (i.e. an object where
+            the encapsulated content is not embedded in the signature object
+            itself). This is the default. If ``False``, the content to be
+            signed will be embedded as encapsulated content.
+        :param signed_attr_settings:
+            :class:`.PdfCMSSignedAttributes` object describing the attributes
+            to be added.
+        :param use_cades:
+            Construct a CAdES-style CMS object.
+        :param timestamper:
+            :class:`.PdfTimeStamper` to use to create a signature timestamp
+
+            .. note::
+                If you want to create a *content* timestamp (as opposed to
+                a *signature* timestamp), see :class:`.CAdESSignedAttrSpec`.
+        :param chunk_size:
+            Chunk size to use when consuming input data.
+        :param max_read:
+            Maximal number of bytes to read from the input stream.
         :return:
-            An :class:`.asn1crypto.cms.SignerInfo` object.
+            A CMS ContentInfo object of type signedData.
         """
-        digest_algorithm_obj = algos.DigestAlgorithm(
-            {'algorithm': digest_algorithm}
-        )
 
-        signing_cert = self.signing_cert
-        # build the signer info object that goes into the PKCS7 signature
-        # (see RFC 2315 § 9.2)
-        sig_info = cms.SignerInfo({
-            'version': 'v1',
-            'sid': cms.SignerIdentifier({
-                'issuer_and_serial_number': cms.IssuerAndSerialNumber({
-                    'issuer': signing_cert.issuer,
-                    'serial_number': signing_cert.serial_number,
-                })
-            }),
-            'digest_algorithm': digest_algorithm_obj,
-            'signature_algorithm': self.get_signature_mechanism(
-                digest_algorithm
-            ),
-            'signed_attrs': signed_attrs,
-            'signature': signature
-        })
-        return sig_info
+        encap_content_info, digest_bytes = _prepare_encap_content(
+            input_data=input_data, digest_algorithm=digest_algorithm,
+            detached=detached, chunk_size=chunk_size, max_read=max_read
+        )
+        return await self.async_sign(
+            data_digest=digest_bytes, digest_algorithm=digest_algorithm,
+            use_pades=use_cades,
+            timestamper=timestamper, encap_content_info=encap_content_info,
+            signed_attr_settings=signed_attr_settings
+        )
 
     def sign(self, data_digest: bytes, digest_algorithm: str,
              timestamp: datetime = None, dry_run=False,
              revocation_info=None, use_pades=False, timestamper=None,
              cades_signed_attr_meta: CAdESSignedAttrSpec = None,
              encap_content_info=None) -> cms.ContentInfo:
 
         """
+        .. deprecated:: 0.9.0
+            Use :meth:`async_sign` instead.
+            The implementation of this method will invoke :meth:`async_sign`
+            using ``asyncio.run()``.
+
         Produce a detached CMS signature from a raw data digest.
 
         :param data_digest:
             Digest of the actual content being signed.
         :param digest_algorithm:
             Digest algorithm to use. This should be the same digest method
             as the one used to hash the (external) content.
@@ -437,49 +888,44 @@
 
             .. danger::
                 This parameter is internal API, and must not be used to produce
                 PDF signatures.
         :return:
             An :class:`~.asn1crypto.cms.ContentInfo` object.
         """
-
-        encap_content_info = encap_content_info or {'content_type': 'data'}
-        if isinstance(encap_content_info, core.Sequence):
-            # could be cms.ContentInfo or cms.EncapsulatedContentInfo depending
-            # on circumstances, so let's just stick to Sequence
-            content_type = encap_content_info['content_type'].native
-        else:
-            content_type = encap_content_info.get('content_type', 'data')
-
-        # the piece of data we'll actually sign is a DER-encoded version of the
-        # signed attributes of our message
-        signed_attrs = self.signed_attrs(
-            data_digest, digest_algorithm, timestamp,
-            revocation_info=revocation_info, use_pades=use_pades,
-            timestamper=timestamper, cades_meta=cades_signed_attr_meta,
-            dry_run=dry_run, content_type=content_type
+        warnings.warn(
+            "'Signer.sign' is deprecated, use 'Signer.async_sign' instead",
+            DeprecationWarning
         )
-        if isinstance(content_type, core.ObjectIdentifier):
-            content_type = content_type.native
-
-        cms_version = 'v1' if content_type == 'data' else 'v3'
-        return self.sign_prescribed_attributes(
-            digest_algorithm, signed_attrs,
-            cms_version=cms_version, dry_run=dry_run, timestamper=timestamper,
+        signed_attr_settings = PdfCMSSignedAttributes(
+            signing_time=timestamp, adobe_revinfo_attr=revocation_info,
+            cades_signed_attrs=cades_signed_attr_meta
+        )
+        sign_coro = self.async_sign(
+            data_digest=data_digest, digest_algorithm=digest_algorithm,
+            dry_run=dry_run, use_pades=use_pades, timestamper=timestamper,
+            signed_attr_settings=signed_attr_settings,
             encap_content_info=encap_content_info
         )
+        return asyncio.run(sign_coro)
 
     def sign_prescribed_attributes(self, digest_algorithm: str,
                                    signed_attrs: cms.CMSAttributes,
                                    cms_version='v1',
                                    dry_run=False, timestamper=None,
                                    encap_content_info=None) -> cms.ContentInfo:
         """
         .. versionadded: 0.7.0
 
+        .. deprecated:: 0.9.0
+            Use :meth:`async_sign_prescribed_attributes` instead.
+            The implementation of this method will invoke
+            :meth:`async_sign_prescribed_attributes` using
+            ``asyncio.run()``.
+
         Start the CMS signing process with the prescribed set of signed
         attributes.
 
         :param digest_algorithm:
             Digest algorithm to use. This should be the same digest method
             as the one used to hash the (external) content.
         :param signed_attrs:
@@ -510,80 +956,47 @@
 
             .. danger::
                 This parameter is internal API, and must not be used to produce
                 PDF signatures.
         :return:
             An :class:`~.asn1crypto.cms.ContentInfo` object.
         """
-
-        encap_content_info = encap_content_info or {'content_type': 'data'}
-        digest_algorithm = digest_algorithm.lower()
-        digest_algorithm_obj = algos.DigestAlgorithm(
-            {'algorithm': digest_algorithm}
-        )
-        implied_hash_algo = None
-        try:
-            if self.signature_mechanism is not None:
-                implied_hash_algo = self.signature_mechanism.hash_algo
-        except ValueError:
-            # this is OK, just use the specified message digest
-            pass
-        if implied_hash_algo is not None \
-                and implied_hash_algo != digest_algorithm:
-            raise SigningError(
-                f"Selected signature mechanism specifies message digest "
-                f"{implied_hash_algo}, but {digest_algorithm} "
-                f"was requested."
-            )
-
-        signature = self.sign_raw(
-            signed_attrs.dump(), digest_algorithm.lower(), dry_run
+        warnings.warn(
+            "'Signer.sign_prescribed_attributes' is deprecated, use "
+            "'Signer.async_sign_prescribed_attributes' instead",
+            DeprecationWarning
         )
-
-        sig_info = self.signer_info(digest_algorithm, signed_attrs, signature)
-
-        unsigned_attrs = self.unsigned_attrs(
-            digest_algorithm, signature, timestamper=timestamper,
-            dry_run=dry_run
+        sign_coro = self.async_sign_prescribed_attributes(
+            digest_algorithm=digest_algorithm,
+            signed_attrs=signed_attrs,
+            cms_version=cms_version, dry_run=dry_run, timestamper=timestamper,
+            encap_content_info=encap_content_info
         )
-        if unsigned_attrs is not None:
-            sig_info['unsigned_attrs'] = unsigned_attrs
-
-        # do not add the TS certs at this point
-        certs = set(self.cert_registry)
-        certs.add(self.signing_cert)
-        # this is the SignedData object for our message (see RFC 2315 § 9.1)
-        signed_data = {
-            'version': cms_version,
-            'digest_algorithms': cms.DigestAlgorithms((digest_algorithm_obj,)),
-            'encap_content_info': encap_content_info,
-            'certificates': certs,
-            'signer_infos': [sig_info]
-        }
-
-        # time to pack up
-        return cms.ContentInfo({
-            'content_type': cms.ContentType('signed_data'),
-            'content': cms.SignedData(signed_data)
-        })
+        return asyncio.run(sign_coro)
 
     def sign_general_data(self, input_data: Union[IO, bytes,
                                                   cms.ContentInfo,
                                                   cms.EncapsulatedContentInfo],
                           digest_algorithm: str, detached=True,
                           timestamp: datetime = None,
                           use_cades=False, timestamper=None,
                           cades_signed_attr_meta: CAdESSignedAttrSpec = None,
                           chunk_size=misc.DEFAULT_CHUNK_SIZE,
                           max_read=None) -> cms.ContentInfo:
         """
+        .. versionadded:: 0.7.0
+
+        .. deprecated:: 0.9.0
+            Use :meth:`async_sign_general_data` instead.
+            The implementation of this method will invoke
+            :meth:`async_sign_general_data` using ``asyncio.run()``.
+
         Produce a CMS signature for an arbitrary data stream
         (not necessarily PDF data).
 
-        .. versionadded:: 0.7.0
 
         :param input_data:
             The input data to sign. This can be either a :class:`bytes` object
             a file-type object, a :class:`cms.ContentInfo` object or
             a :class:`cms.EncapsulatedContentInfo` object.
 
             .. warning::
@@ -626,56 +1039,50 @@
         :param chunk_size:
             Chunk size to use when consuming input data.
         :param max_read:
             Maximal number of bytes to read from the input stream.
         :return:
             A CMS ContentInfo object of type signedData.
         """
-        h = hashes.Hash(get_pyca_cryptography_hash(digest_algorithm))
-        encap_content_info = None
-        if isinstance(input_data,
-                      (cms.ContentInfo, cms.EncapsulatedContentInfo)):
-            h.update(bytes(input_data['content']))
-            if detached:
-                encap_content_info = {
-                    'content_type': input_data['content_type']
-                }
-            else:
-                encap_content_info = input_data
-        elif isinstance(input_data, bytes):
-            h.update(input_data)
-            if not detached:
-                # use dicts instead of Asn1Value objects, to leave asn1crypto
-                # to decide whether to use cms.ContentInfo or
-                # cms.EncapsulatedContentInfo (for backwards compat with PCKS#7)
-                encap_content_info = {
-                    'content_type': 'data', 'content': input_data
-                }
-        elif not detached:
-            # input stream is a buffer, and we're in 'enveloping' mode
-            # read the entire thing into memory, since we need to embed
-            # it anyway
-            input_bytes = input_data.read(max_read)
-            h.update(input_bytes)
-            # see above
-            encap_content_info = {
-                'content_type': 'data',
-                'content': input_bytes
-            }
-        else:
-            temp_buf = bytearray(chunk_size)
-            misc.chunked_digest(temp_buf, input_data, h, max_read=max_read)
-        digest_bytes = h.finalize()
+        warnings.warn(
+            "'Signer.sign_general_data' is deprecated, use "
+            "'Signer.async_sign_general_data' instead",
+            DeprecationWarning
+        )
+        signed_attr_settings = PdfCMSSignedAttributes(
+            signing_time=timestamp, cades_signed_attrs=cades_signed_attr_meta
+        )
+        sign_coro = self.async_sign_general_data(
+            input_data=input_data, digest_algorithm=digest_algorithm,
+            detached=detached, use_cades=use_cades,
+            timestamper=timestamper, chunk_size=chunk_size,
+            signed_attr_settings=signed_attr_settings,
+            max_read=max_read
+        )
+        return asyncio.run(sign_coro)
 
-        return self.sign(
-            data_digest=digest_bytes, digest_algorithm=digest_algorithm,
-            timestamp=timestamp, use_pades=use_cades,
-            timestamper=timestamper, encap_content_info=encap_content_info,
-            cades_signed_attr_meta=cades_signed_attr_meta
+
+def asyncify_signer(signer_cls):
+    """
+    Decorator to turn a legacy :class:`Signer` subclass into one that works
+    with the new async API.
+    """
+
+    async def async_sign_raw(self, data: bytes, digest_algorithm: str,
+                             dry_run=False) -> bytes:
+        coro = to_thread(
+            lambda: signer_cls.sign_raw(
+                self, data=data, digest_algorithm=digest_algorithm,
+                dry_run=dry_run
+            )
         )
+        return await coro
+
+    signer_cls.async_sign_raw = async_sign_raw
+    return signer_cls
 
 
 class SimpleSigner(Signer):
     """
     Simple signer implementation where the key material is available in local
     memory.
     """
@@ -685,46 +1092,61 @@
     Private key associated with the certificate in :attr:`signing_cert`.
     """
 
     def __init__(self, signing_cert: x509.Certificate,
                  signing_key: keys.PrivateKeyInfo,
                  cert_registry: CertificateStore,
                  signature_mechanism: SignedDigestAlgorithm = None,
-                 prefer_pss=False):
+                 prefer_pss=False, embed_roots=True):
         self.signing_cert = signing_cert
         self.signing_key = signing_key
         self.cert_registry = cert_registry
         self.signature_mechanism = signature_mechanism
-        super().__init__(prefer_pss=prefer_pss)
+        super().__init__(prefer_pss=prefer_pss, embed_roots=embed_roots)
+
+    async def async_sign_raw(self, data: bytes, digest_algorithm: str,
+                             dry_run=False) -> bytes:
+        return self.sign_raw(data, digest_algorithm)
 
-    def sign_raw(self, data: bytes, digest_algorithm: str, dry_run=False) \
-            -> bytes:
+    def sign_raw(self, data: bytes, digest_algorithm: str) -> bytes:
+        """
+        Synchronous raw signature implementation.
 
+        :param data:
+            Data to be signed.
+        :param digest_algorithm:
+            Digest algorithm to use.
+        :return:
+            Raw signature encoded according to the conventions of the
+            signing algorithm used.
+        """
         signature_mechanism = self.get_signature_mechanism(digest_algorithm)
         mechanism = signature_mechanism.signature_algo
         priv_key = serialization.load_der_private_key(
             self.signing_key.dump(), password=None
         )
 
         if mechanism == 'rsassa_pkcs1v15':
             padding = PKCS1v15()
             hash_algo = get_pyca_cryptography_hash(digest_algorithm)
             assert isinstance(priv_key, RSAPrivateKey)
             return priv_key.sign(data, padding, hash_algo)
         elif mechanism == 'rsassa_pss':
             params = signature_mechanism['parameters']
-            padding, hash_algo = _process_pss_params(
-                params, digest_algorithm
-            )
+            padding, hash_algo = _process_pss_params(params, digest_algorithm)
             assert isinstance(priv_key, RSAPrivateKey)
             return priv_key.sign(data, padding, hash_algo)
         elif mechanism == 'ecdsa':
             hash_algo = get_pyca_cryptography_hash(digest_algorithm)
             assert isinstance(priv_key, EllipticCurvePrivateKey)
             return priv_key.sign(data, signature_algorithm=ECDSA(hash_algo))
+        elif mechanism == 'dsa':
+            hash_algo = get_pyca_cryptography_hash(digest_algorithm)
+            assert isinstance(priv_key, DSAPrivateKey)
+            return priv_key.sign(data, hash_algo)
         else:  # pragma: nocover
             raise SigningError(
                 f"The signature mechanism {mechanism} "
                 "is unsupported by this signer."
             )
 
     @classmethod
@@ -862,23 +1284,24 @@
     Intended for use with :ref:`interrupted-signing`.
     """
 
     def __init__(self, signing_cert: x509.Certificate,
                  cert_registry: CertificateStore,
                  signature_value: bytes,
                  signature_mechanism: SignedDigestAlgorithm = None,
-                 prefer_pss=False):
+                 prefer_pss=False, embed_roots=True):
         self.signing_cert = signing_cert
         self.cert_registry = cert_registry
         self.signature_mechanism = signature_mechanism
         self._signature_value = signature_value
-        super().__init__(prefer_pss=prefer_pss)
+        super().__init__(prefer_pss=prefer_pss, embed_roots=embed_roots)
 
-    def sign_raw(self, data: bytes, digest_algorithm: str, dry_run=False) \
-            -> bytes:
+    async def async_sign_raw(self,
+                             data: bytes, digest_algorithm: str,
+                             dry_run=False) -> bytes:
         """
         Return a fixed signature value.
         """
         return self._signature_value
 
 
 # TODO consider deprecating the current signed_attrs kwargs in favour of this
@@ -904,7 +1327,37 @@
     Adobe-style signed revocation info attribute.
     """
 
     cades_signed_attrs: Optional[CAdESSignedAttrSpec] = None
     """
     Optional settings for CAdES-style signed attributes.
     """
+
+
+RSA_THRESHOLDS = [(2048, 'sha256'), (3072, 'sha384')]
+ECC_THRESHOLDS = [(256, 'sha256'), (384, 'sha384')]
+
+
+def select_suitable_signing_md(key: keys.PublicKeyInfo) -> str:
+    """
+    Choose a reasonable default signing message digest given the properties of
+    (the public part of) a key.
+
+    The fallback value is :const:`constants.DEFAULT_MD`.
+
+    :param key:
+        A :class:`keys.PublicKeyInfo` object.
+    :return:
+        The name of a message digest algorithm.
+    """
+
+    def _with_thresholds(key_size, thresholds):
+        for sz, md in thresholds:
+            if key_size <= sz:
+                return md
+        return 'sha512'
+
+    if key.algorithm == 'rsa':
+        return _with_thresholds(key.bit_size, RSA_THRESHOLDS)
+    elif key.algorithm == 'ec':
+        return _with_thresholds(key.bit_size, ECC_THRESHOLDS)
+    return constants.DEFAULT_MD
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/signers/pdf_signer.py` & `pyHanko-0.9.0/pyhanko/sign/signers/pdf_signer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,61 @@
 """
 This module implements support for PDF-specific signing functionality.
 """
+import asyncio
 import enum
 import logging
 import uuid
-import tzlocal
-from datetime import datetime
+import warnings
 from dataclasses import dataclass, field
-from typing import Set, Optional, List, Union, IO, Tuple
+from datetime import datetime
+from typing import IO, List, Optional, Set, Tuple, Union
 
-from asn1crypto import cms, ocsp, crl
+import tzlocal
+from asn1crypto import cms, crl, ocsp
+from asn1crypto import pdf as asn1_pdf
 from cryptography.hazmat.primitives import hashes
-
-from pyhanko.sign.fields import (
-    SigSeedSubFilter, MDPPerm, SigFieldSpec, FieldMDPSpec, SigSeedValueSpec,
-    SeedLockDocument, SigSeedValFlags
-)
-from pyhanko_certvalidator import ValidationContext, CertificateValidator
+from pyhanko_certvalidator import CertificateValidator, ValidationContext
+from pyhanko_certvalidator.errors import PathBuildingError, PathValidationError
 from pyhanko_certvalidator.path import ValidationPath
-from pyhanko_certvalidator.errors import PathValidationError, PathBuildingError
 
 from pyhanko.pdf_utils import generic, misc
 from pyhanko.pdf_utils.generic import pdf_name
-from pyhanko.pdf_utils.writer import BasePdfFileWriter
 from pyhanko.pdf_utils.incremental_writer import IncrementalPdfFileWriter
 from pyhanko.pdf_utils.reader import PdfFileReader
-from pyhanko.stamp import BaseStampStyle
-
+from pyhanko.pdf_utils.writer import BasePdfFileWriter
+from pyhanko.sign.ades.api import CAdESSignedAttrSpec
+from pyhanko.sign.fields import (
+    FieldMDPSpec,
+    MDPPerm,
+    SeedLockDocument,
+    SigFieldSpec,
+    SigSeedSubFilter,
+    SigSeedValFlags,
+    SigSeedValueSpec,
+    enumerate_sig_fields,
+)
 from pyhanko.sign.general import SigningError, get_pyca_cryptography_hash
 from pyhanko.sign.timestamps import TimeStamper
-from pyhanko.sign.ades.api import CAdESSignedAttrSpec
+from pyhanko.stamp import BaseStampStyle
 
 from . import constants
-from .pdf_cms import Signer, PdfCMSSignedAttributes
 from .cms_embedder import (
-    PdfCMSEmbedder, SigObjSetup, SigMDPSetup, SigIOSetup, SigAppearanceSetup,
+    PdfCMSEmbedder,
+    SigAppearanceSetup,
+    SigIOSetup,
+    SigMDPSetup,
+    SigObjSetup,
 )
 from .pdf_byterange import (
-    DocumentTimestamp, PreparedByteRangeDigest, SignatureObject
+    DocumentTimestamp,
+    PreparedByteRangeDigest,
+    SignatureObject,
 )
+from .pdf_cms import PdfCMSSignedAttributes, Signer, select_suitable_signing_md
 
 __all__ = [
     'PdfSignatureMetadata', 'DSSContentSettings',
     'TimestampDSSContentSettings', 'GeneralDSSContentSettings',
     'SigDSSPlacementPreference', 'PdfTimeStamper',
     'PdfSigner', 'PdfSigningSession', 'PdfTBSDocument',
     'PdfPostSignatureDocument',
@@ -247,17 +260,16 @@
     """
 
     md_algorithm: str = None
     """
     The name of the digest algorithm to use.
     It should be supported by `pyca/cryptography`.
 
-    If ``None``, this will ordinarily default to the value of
-    :const:`constants.DEFAULT_MD`, unless a seed value dictionary and/or a prior
-    certification signature happen to be available.
+    If ``None``, :func:`.select_suitable_signing_md` will be invoked to generate
+    a suitable default, unless a seed value dictionary happens to be available.
     """
 
     location: str = None
     """
     Location of signing.
     """
 
@@ -387,17 +399,19 @@
     """
     .. versionadded:: 0.8.0
 
     When estimating the size of a signature container,
     do not add safety margins.
     
     .. note::
-        This should be OK if the entire signature object is produced by pyHanko.
-        However, if it includes unsigned attributes such as document timestamps,
-        the size of the signature is not entirely predictable.
+        This should be OK if the entire CMS object is produced by pyHanko, and
+        the signing scheme produces signatures of a fixed size.
+        However, if the signature container includes unsigned attributes such
+        as signature timestamps, the size of the signature is never entirely
+        predictable.
     """
 
 
 def _ensure_esic_ext(pdf_writer: BasePdfFileWriter):
     """
     Helper function to ensure that the output PDF is at least PDF 1.7, and that
     the relevant ESIC extension for PAdES is enabled if the version lower than
@@ -440,15 +454,93 @@
                       bytes_reserved=None, validation_paths=None,
                       timestamper: Optional[TimeStamper] = None, *,
                       in_place=False, output=None,
                       dss_settings: TimestampDSSContentSettings =
                       TimestampDSSContentSettings(),
                       chunk_size=misc.DEFAULT_CHUNK_SIZE,
                       tight_size_estimates: bool = False):
-        """Timestamp the contents of ``pdf_out``.
+        """
+        .. versionchanged:: 0.9.0
+            Wrapper around :meth:`async_timestamp_pdf`.
+
+        Timestamp the contents of ``pdf_out``.
+        Note that ``pdf_out`` should not be written to after this operation.
+
+        :param pdf_out:
+            An :class:`.IncrementalPdfFileWriter`.
+        :param md_algorithm:
+            The hash algorithm to use when computing message digests.
+        :param validation_context:
+            The :class:`.pyhanko_certvalidator.ValidationContext`
+            against which the TSA response should be validated.
+            This validation context will also be used to update the DSS.
+        :param bytes_reserved:
+            Bytes to reserve for the CMS object in the PDF file.
+            If not specified, make an estimate based on a dummy signature.
+
+            .. warning::
+                Since the CMS object is written to the output file as a
+                hexadecimal string, you should request **twice** the (estimated)
+                number of bytes in the DER-encoded version of the CMS object.
+        :param validation_paths:
+            If the validation path(s) for the TSA's certificate are already
+            known, you can pass them using this parameter to avoid having to
+            run the validation logic again.
+        :param timestamper:
+            Override the default :class:`.TimeStamper` associated with this
+            :class:`.PdfTimeStamper`.
+        :param output:
+            Write the output to the specified output stream.
+            If ``None``, write to a new :class:`.BytesIO` object.
+            Default is ``None``.
+        :param in_place:
+            Sign the original input stream in-place.
+            This parameter overrides ``output``.
+        :param chunk_size:
+            Size of the internal buffer (in bytes) used to feed data to the
+            message digest function if the input stream does not support
+            ``memoryview``.
+        :param dss_settings:
+            DSS output settings. See :class:`.TimestampDSSContentSettings`.
+        :param tight_size_estimates:
+            When estimating the size of a document timestamp container,
+            do not add safety margins.
+
+            .. note::
+                External TSAs cannot be relied upon to always produce the
+                exact same output length, which makes this option risky to use.
+        :return:
+            The output stream containing the signed output.
+        """
+        result = asyncio.run(
+            self.async_timestamp_pdf(
+                pdf_out, md_algorithm, validation_context=validation_context,
+                bytes_reserved=bytes_reserved,
+                validation_paths=validation_paths, timestamper=timestamper,
+                in_place=in_place, output=output, chunk_size=chunk_size,
+                dss_settings=dss_settings,
+                tight_size_estimates=tight_size_estimates
+            )
+        )
+        return result
+
+    async def async_timestamp_pdf(self, pdf_out: IncrementalPdfFileWriter,
+                                  md_algorithm, validation_context=None,
+                                  bytes_reserved=None, validation_paths=None,
+                                  timestamper: Optional[TimeStamper] = None, *,
+                                  in_place=False, output=None,
+                                  dss_settings: TimestampDSSContentSettings =
+                                  TimestampDSSContentSettings(),
+                                  chunk_size=misc.DEFAULT_CHUNK_SIZE,
+                                  tight_size_estimates: bool = False,
+                                  embed_roots: bool = True):
+        """
+        .. versionadded:: 0.9.0
+
+        Timestamp the contents of ``pdf_out``.
         Note that ``pdf_out`` should not be written to after this operation.
 
         :param pdf_out:
             An :class:`.IncrementalPdfFileWriter`.
         :param md_algorithm:
             The hash algorithm to use when computing message digests.
         :param validation_context:
@@ -486,39 +578,50 @@
         :param tight_size_estimates:
             When estimating the size of a document timestamp container,
             do not add safety margins.
 
             .. note::
                 External TSAs cannot be relied upon to always produce the
                 exact same output length, which makes this option risky to use.
+        :param embed_roots:
+            Option that controls whether the root certificate of each validation
+            path should be embedded into the DSS. The default is ``True``.
+
+            .. note::
+                Trust roots are configured by the validator, so embedding them
+                typically does nothing in a typical validation process.
+                Therefore they can be safely omitted in most cases.
+                Nonetheless, embedding the roots can be useful for documentation
+                purposes.
         :return:
             The output stream containing the signed output.
         """
 
         _ensure_esic_ext(pdf_out)
         from pyhanko.sign import validation
         timestamper = timestamper or self.default_timestamper
         if validation_context is not None:
-            ts_validation_paths \
-                = timestamper.validation_paths(validation_context)
+            paths_coro = timestamper.validation_paths(validation_context)
             if validation_paths is None:
-                validation_paths = list(ts_validation_paths)
-            else:
-                validation_paths.extend(ts_validation_paths)
+                validation_paths = []
+            async for path in paths_coro:
+                validation_paths.append(path)
             dss_settings.assert_viable()
             if dss_settings.update_before_ts:
                 # NOTE: we have to disable VRI in this scenario
                 validation.DocumentSecurityStore.supply_dss_in_writer(
                     pdf_out, sig_contents=None, paths=validation_paths,
-                    validation_context=validation_context
+                    validation_context=validation_context,
+                    embed_roots=embed_roots
                 )
 
         field_name = self.field_name
         if bytes_reserved is None:
-            test_signature_cms = timestamper.dummy_response(md_algorithm)
+            test_signature_cms = \
+                await timestamper.async_dummy_response(md_algorithm)
             test_len = len(test_signature_cms.dump()) * 2
             if tight_size_estimates:
                 bytes_reserved = test_len
             else:
                 # see sign_pdf comments
                 bytes_reserved = test_len + 2 * (test_len // 4)
 
@@ -537,36 +640,80 @@
 
         sig_io = SigIOSetup(
             md_algorithm=md_algorithm,
             in_place=in_place, output=output, chunk_size=chunk_size
         )
         prep_digest: PreparedByteRangeDigest
         prep_digest, res_output = cms_writer.send(sig_io)
-        timestamp_cms = timestamper.timestamp(
+        timestamp_cms = await timestamper.async_timestamp(
             prep_digest.document_digest, md_algorithm
         )
         sig_contents = cms_writer.send(timestamp_cms)
 
         # update the DSS if necessary
         if validation_context is not None and not dss_settings.update_before_ts:
             if not dss_settings.include_vri:
                 sig_contents = None
             validation.DocumentSecurityStore.add_dss(
                 output_stream=res_output, sig_contents=sig_contents,
                 paths=validation_paths, validation_context=validation_context,
-                force_write=not dss_settings.skip_if_unneeded
+                force_write=not dss_settings.skip_if_unneeded,
+                embed_roots=embed_roots
             )
 
         return misc.finalise_output(output, res_output)
 
     def update_archival_timestamp_chain(
             self, reader: PdfFileReader, validation_context, in_place=True,
             output=None, chunk_size=misc.DEFAULT_CHUNK_SIZE,
             default_md_algorithm=constants.DEFAULT_MD):
         """
+        .. versionchanged:: 0.9.0
+            Wrapper around :meth:`async_update_archival_timestamp_chain`.
+
+        Validate the last timestamp in the timestamp chain on a PDF file, and
+        write an updated version to an output stream.
+
+        :param reader:
+            A :class:`PdfReader` encapsulating the input file.
+        :param validation_context:
+            :class:`.pyhanko_certvalidator.ValidationContext` object to validate
+            the last timestamp.
+        :param output:
+            Write the output to the specified output stream.
+            If ``None``, write to a new :class:`.BytesIO` object.
+            Default is ``None``.
+        :param in_place:
+            Sign the original input stream in-place.
+            This parameter overrides ``output``.
+        :param chunk_size:
+            Size of the internal buffer (in bytes) used to feed data to the
+            message digest function if the input stream does not support
+            ``memoryview``.
+        :param default_md_algorithm:
+            Message digest to use if there are no preceding timestamps in the
+            file.
+        :return:
+            The output stream containing the signed output.
+        """
+        coro = self.async_update_archival_timestamp_chain(
+            reader=reader, validation_context=validation_context,
+            in_place=in_place, output=output, chunk_size=chunk_size,
+            default_md_algorithm=default_md_algorithm
+        )
+        return asyncio.run(coro)
+
+    async def async_update_archival_timestamp_chain(
+            self, reader: PdfFileReader, validation_context, in_place=True,
+            output=None, chunk_size=misc.DEFAULT_CHUNK_SIZE,
+            default_md_algorithm=constants.DEFAULT_MD,
+            embed_roots: bool = True):
+        """
+        .. versionadded:: 0.9.0
+
         Validate the last timestamp in the timestamp chain on a PDF file, and
         write an updated version to an output stream.
 
         :param reader:
             A :class:`PdfReader` encapsulating the input file.
         :param validation_context:
             :class:`.pyhanko_certvalidator.ValidationContext` object to validate
@@ -581,26 +728,38 @@
         :param chunk_size:
             Size of the internal buffer (in bytes) used to feed data to the
             message digest function if the input stream does not support
             ``memoryview``.
         :param default_md_algorithm:
             Message digest to use if there are no preceding timestamps in the
             file.
+        :param embed_roots:
+            Option that controls whether the root certificate of each validation
+            path should be embedded into the DSS. The default is ``True``.
+
+            .. note::
+                Trust roots are configured by the validator, so embedding them
+                typically does nothing in a typical validation process.
+                Therefore they can be safely omitted in most cases.
+                Nonetheless, embedding the roots can be useful for documentation
+                purposes.
         :return:
             The output stream containing the signed output.
         """
+
         # TODO expose DSS fine-tuning here as well
 
         # In principle, we only have to validate that the last timestamp token
         # in the current chain is valid.
         # TODO: add an option to validate the entire timestamp chain
         #  plus all signatures
         from pyhanko.sign.validation import (
-            _establish_timestamp_trust, DocumentSecurityStore,
-            get_timestamp_chain
+            DocumentSecurityStore,
+            _establish_timestamp_trust,
+            get_timestamp_chain,
         )
 
         timestamps = get_timestamp_chain(reader)
         try:
             last_timestamp = next(timestamps)
         except StopIteration:
             logger.warning(
@@ -617,15 +776,15 @@
             last_timestamp.compute_digest()
             last_timestamp.compute_tst_digest()
 
             tst_token = last_timestamp.signed_data
             expected_imprint = last_timestamp.external_digest
 
             # run validation logic
-            tst_status = _establish_timestamp_trust(
+            tst_status = await _establish_timestamp_trust(
                 tst_token, validation_context, expected_imprint
             )
 
             md_algorithm = tst_status.md_algorithm
 
         # Prepare output
         if in_place:
@@ -639,23 +798,33 @@
 
         pdf_out = IncrementalPdfFileWriter(output)
         if last_timestamp is not None:
             # update the DSS
             DocumentSecurityStore.supply_dss_in_writer(
                 pdf_out, last_timestamp.pkcs7_content,
                 paths=(tst_status.validation_path,),
-                validation_context=validation_context
+                validation_context=validation_context,
+                embed_roots=embed_roots
             )
 
         # append a new timestamp
-        return self.timestamp_pdf(
-            pdf_out, md_algorithm, validation_context, in_place=True
+        return await self.async_timestamp_pdf(
+            pdf_out, md_algorithm, validation_context, in_place=True,
+            embed_roots=embed_roots
         )
 
 
+def _signatures_exist(handler):
+    try:
+        next(enumerate_sig_fields(handler, filled_status=True))
+        return True
+    except StopIteration:
+        return False
+
+
 class PdfSigner:
     """
     .. versionchanged: 0.7.0
         This class is no longer a subclass of :class:`.PdfTimeStamper`.
 
     Class to handle PDF signatures in general.
 
@@ -676,15 +845,16 @@
         to specify the field's properties in the form of a
         :class:`.SigFieldSpec`. This parameter is only meaningful if
         ``existing_fields_only`` is ``False``.
     """
     _ignore_sv = False
 
     def __init__(self, signature_meta: PdfSignatureMetadata,
-                 signer: Signer, *, timestamper: TimeStamper = None,
+                 signer: Signer, *,
+                 timestamper: TimeStamper = None,
                  stamp_style: Optional[BaseStampStyle] = None,
                  new_field_spec: Optional[SigFieldSpec] = None):
         self.signature_meta = signature_meta
         if new_field_spec is not None and \
                 new_field_spec.sig_field_name != signature_meta.field_name:
             raise SigningError(
                 "Field names specified in SigFieldSpec and "
@@ -716,65 +886,63 @@
         :return:
             The name of the message digest algorithm, or ``None``.
         """
         return self.signature_meta.md_algorithm or self.signer_hash_algo
 
     def _enforce_certification_constraints(self, reader: PdfFileReader):
         # TODO we really should take into account the /DocMDP constraints
-        #  of _all_ previous signatures
+        #  of _all_ previous signatures, i.e. also approval signatures with
+        #  locking instructions etc.
+        if self.signature_meta.certify and _signatures_exist(reader):
+            raise SigningError(
+                "Certification signatures must be the first signature "
+                "in a given document."
+            )
 
         from pyhanko.sign.validation import read_certification_data
         cd = read_certification_data(reader)
         # if there is no author signature, we don't have to do anything
         if cd is None:
             return
-        if self.signature_meta.certify:
-            raise SigningError(
-                "Document already contains a certification signature"
-            )
         if cd.permission == MDPPerm.NO_CHANGES:
             raise SigningError("Author signature forbids all changes")
-        return cd.digest_method
 
     def _retrieve_seed_value_spec(self, sig_field) \
             -> Optional[SigSeedValueSpec]:
         # for testing & debugging
         if self._ignore_sv:
             return None
         sv_dict = sig_field.get('/SV')
         if sv_dict is None:
             return None
         return SigSeedValueSpec.from_pdf_object(sv_dict)
 
-    def _select_md_algorithm(self, sv_spec: Optional[SigSeedValueSpec],
-                             author_sig_md_algorithm: Optional[str]) -> str:
+    def _select_md_algorithm(self, sv_spec: Optional[SigSeedValueSpec]) -> str:
 
         signature_meta = self.signature_meta
 
         # priority order for the message digest algorithm
         #  (1) If signature_meta specifies a message digest algorithm, use it
         #      (it has been cleared by the SV dictionary checker already)
         #  (2) Use the first algorithm specified in the seed value dictionary,
         #      if a suggestion is present
-        #  (3) If there is a certification signature, use the digest method
-        #      specified there.
-        #  (4) fall back to DEFAULT_MD
+        #  (3) fall back to select_suitable_signing_md()
         if sv_spec is not None and sv_spec.digest_methods:
             sv_md_algorithm = sv_spec.digest_methods[0]
         else:
             sv_md_algorithm = None
 
         if self.default_md_for_signer is not None:
             md_algorithm = self.default_md_for_signer
         elif sv_md_algorithm is not None:
             md_algorithm = sv_md_algorithm
-        elif author_sig_md_algorithm is not None:
-            md_algorithm = author_sig_md_algorithm
         else:
-            md_algorithm = constants.DEFAULT_MD
+            md_algorithm = select_suitable_signing_md(
+                self.signer.signing_cert.public_key
+            )
 
         # TODO fall back to more useful default for weak_hash_algos
         weak_hash_algos = (
             signature_meta.validation_context.weak_hash_algos
             if signature_meta.validation_context is not None
             else ()
         )
@@ -827,34 +995,23 @@
         sig_field_ref = next(cms_writer)
 
         sig_field = sig_field_ref.get_object()
 
         # Fetch seed values (if present) to prepare for signing
         sv_spec = self._retrieve_seed_value_spec(sig_field)
 
-        # look up the certification signature's MD (if present), as a fallback
-        # if the settings don't specify one
-        author_sig_md_algorithm = None
+        # Check DocMDP settings to see if we're allowed to add a signature
         if isinstance(pdf_out, IncrementalPdfFileWriter):
-            author_sig_md_algorithm = self._enforce_certification_constraints(
-                pdf_out.prev
-            )
+            self._enforce_certification_constraints(pdf_out.prev)
 
-        md_algorithm = self._select_md_algorithm(
-            sv_spec, author_sig_md_algorithm
-        )
+        md_algorithm = self._select_md_algorithm(sv_spec)
         ts_required = sv_spec is not None and sv_spec.timestamp_required
         if ts_required and timestamper is None:
             timestamper = sv_spec.build_timestamper()
 
-        if timestamper is not None:
-            # this might hit the TS server, but the response is cached
-            # and it collects the certificates we need to verify the TS response
-            timestamper.dummy_response(md_algorithm)
-
         # subfilter: try signature_meta and SV dict, fall back
         #  to /adbe.pkcs7.detached by default
         subfilter = signature_meta.subfilter
         if subfilter is None:
             if sv_spec is not None and sv_spec.subfilters:
                 subfilter = sv_spec.subfilters[0]
             else:
@@ -870,14 +1027,17 @@
     def digest_doc_for_signing(self, pdf_out: BasePdfFileWriter,
                                existing_fields_only=False, bytes_reserved=None,
                                *, appearance_text_params=None,
                                in_place=False, output=None,
                                chunk_size=misc.DEFAULT_CHUNK_SIZE)\
             -> Tuple[PreparedByteRangeDigest, 'PdfTBSDocument', IO]:
         """
+        .. deprecated:: 0.9.0
+            Use :meth:`async_digest_doc_for_signing` instead.
+
         Set up all stages of the signing process up to and including the point
         where the signature placeholder is allocated, and the document's
         ``/ByteRange`` digest is computed.
 
         See :meth:`sign_pdf` for a less granular, more high-level approach.
 
         .. note::
@@ -918,18 +1078,99 @@
             message digest function if the input stream does not support
             ``memoryview``.
         :return:
             A tuple containing a :class:`.PreparedByteRangeDigest` object,
             a :class:`.PdfTBSDocument` object and an output handle to which the
             document in its current state has been written.
         """
+        warnings.warn(
+            "'digest_doc_for_signing' is deprecated, use "
+            "'async_digest_doc_for_signing' instead",
+            DeprecationWarning
+        )
+        result = asyncio.run(
+            self.async_digest_doc_for_signing(
+                pdf_out, existing_fields_only=existing_fields_only,
+                bytes_reserved=bytes_reserved,
+                appearance_text_params=appearance_text_params,
+                in_place=in_place, output=output, chunk_size=chunk_size
+            )
+        )
+        return result
+
+    async def async_digest_doc_for_signing(self, pdf_out: BasePdfFileWriter,
+                                           existing_fields_only=False,
+                                           bytes_reserved=None,
+                                           *, appearance_text_params=None,
+                                           in_place=False, output=None,
+                                           chunk_size=misc.DEFAULT_CHUNK_SIZE) \
+            -> Tuple[PreparedByteRangeDigest, 'PdfTBSDocument', IO]:
+        """
+        .. versionadded:: 0.9.0
+
+        Set up all stages of the signing process up to and including the point
+        where the signature placeholder is allocated, and the document's
+        ``/ByteRange`` digest is computed.
+
+        See :meth:`sign_pdf` for a less granular, more high-level approach.
+
+        .. note::
+            This method is useful in remote signing scenarios, where you might
+            want to free up resources while waiting for the remote signer to
+            respond. The :class:`.PreparedByteRangeDigest` object returned
+            allows you to keep track of the required state to fill the
+            signature container at some later point in time.
+
+        :param pdf_out:
+            A PDF file writer (usually an :class:`.IncrementalPdfFileWriter`)
+            containing the data to sign.
+        :param existing_fields_only:
+            If ``True``, never create a new empty signature field to contain
+            the signature.
+            If ``False``, a new field may be created if no field matching
+            :attr:`~.PdfSignatureMetadata.field_name` exists.
+        :param bytes_reserved:
+            Bytes to reserve for the CMS object in the PDF file.
+            If not specified, make an estimate based on a dummy signature.
+
+            .. warning::
+                Since the CMS object is written to the output file as a
+                hexadecimal string, you should request **twice** the (estimated)
+                number of bytes in the DER-encoded version of the CMS object.
+        :param appearance_text_params:
+            Dictionary with text parameters that will be passed to the
+            signature appearance constructor (if applicable).
+        :param output:
+            Write the output to the specified output stream.
+            If ``None``, write to a new :class:`.BytesIO` object.
+            Default is ``None``.
+        :param in_place:
+            Sign the original input stream in-place.
+            This parameter overrides ``output``.
+        :param chunk_size:
+            Size of the internal buffer (in bytes) used to feed data to the
+            message digest function if the input stream does not support
+            ``memoryview``.
+        :return:
+            A tuple containing a :class:`.PreparedByteRangeDigest` object,
+            a :class:`.PdfTBSDocument` object and an output handle to which the
+            document in its current state has been written.
+        """
         signing_session = self.init_signing_session(
             pdf_out, existing_fields_only=existing_fields_only,
         )
-        validation_info = signing_session.perform_presign_validation(pdf_out)
+        validation_info \
+            = await signing_session.perform_presign_validation(pdf_out)
+        if bytes_reserved is None:
+            estimation = signing_session.estimate_signature_container_size(
+                validation_info=validation_info,
+                tight=self.signature_meta.tight_size_estimates
+            )
+            bytes_reserved = await estimation
+
         tbs_document = signing_session.prepare_tbs_document(
             validation_info=validation_info,
             bytes_reserved=bytes_reserved,
             appearance_text_params=appearance_text_params
         )
         prepared_br_digest, res_output = tbs_document.digest_tbs_document(
             in_place=in_place, chunk_size=chunk_size, output=output
@@ -940,14 +1181,17 @@
         )
 
     def sign_pdf(self, pdf_out: BasePdfFileWriter,
                  existing_fields_only=False, bytes_reserved=None, *,
                  appearance_text_params=None, in_place=False,
                  output=None, chunk_size=misc.DEFAULT_CHUNK_SIZE):
         """
+        .. versionchanged:: 0.9.0
+            Wrapper around :meth:`async_sign_pdf`.
+
         Sign a PDF file using the provided output writer.
 
         :param pdf_out:
             A PDF file writer (usually an :class:`.IncrementalPdfFileWriter`)
             containing the data to sign.
         :param existing_fields_only:
             If ``True``, never create a new empty signature field to contain
@@ -970,40 +1214,94 @@
         :param chunk_size:
             Size of the internal buffer (in bytes) used to feed data to the
             message digest function if the input stream does not support
             ``memoryview``.
         :return:
             The output stream containing the signed data.
         """
+        result = asyncio.run(
+            self.async_sign_pdf(
+                pdf_out, existing_fields_only=existing_fields_only,
+                bytes_reserved=bytes_reserved,
+                appearance_text_params=appearance_text_params,
+                in_place=in_place, output=output, chunk_size=chunk_size
+            )
+        )
+        return result
+
+    async def async_sign_pdf(self, pdf_out: BasePdfFileWriter,
+                             existing_fields_only=False, bytes_reserved=None, *,
+                             appearance_text_params=None, in_place=False,
+                             output=None, chunk_size=misc.DEFAULT_CHUNK_SIZE):
+        """
+        .. versionadded:: 0.9.0
+
+        Sign a PDF file using the provided output writer.
+
+        :param pdf_out:
+            A PDF file writer (usually an :class:`.IncrementalPdfFileWriter`)
+            containing the data to sign.
+        :param existing_fields_only:
+            If ``True``, never create a new empty signature field to contain
+            the signature.
+            If ``False``, a new field may be created if no field matching
+            :attr:`~.PdfSignatureMetadata.field_name` exists.
+        :param bytes_reserved:
+            Bytes to reserve for the CMS object in the PDF file.
+            If not specified, make an estimate based on a dummy signature.
+        :param appearance_text_params:
+            Dictionary with text parameters that will be passed to the
+            signature appearance constructor (if applicable).
+        :param output:
+            Write the output to the specified output stream.
+            If ``None``, write to a new :class:`.BytesIO` object.
+            Default is ``None``.
+        :param in_place:
+            Sign the original input stream in-place.
+            This parameter overrides ``output``.
+        :param chunk_size:
+            Size of the internal buffer (in bytes) used to feed data to the
+            message digest function if the input stream does not support
+            ``memoryview``.
+        :return:
+            The output stream containing the signed data.
+        """
+
         signing_session = self.init_signing_session(
             pdf_out, existing_fields_only=existing_fields_only,
         )
-        validation_info = signing_session.perform_presign_validation(pdf_out)
+        validation_info = \
+            await signing_session.perform_presign_validation(pdf_out)
+        if bytes_reserved is None:
+            estimation = signing_session.estimate_signature_container_size(
+                validation_info, tight=self.signature_meta.tight_size_estimates
+            )
+            bytes_reserved = await estimation
         tbs_document = signing_session.prepare_tbs_document(
             validation_info=validation_info,
             bytes_reserved=bytes_reserved,
             appearance_text_params=appearance_text_params
         )
         prepared_br_digest, res_output = tbs_document.digest_tbs_document(
             in_place=in_place, chunk_size=chunk_size, output=output
         )
 
-        post_signing_doc = tbs_document.perform_signature(
+        post_signing_doc = await tbs_document.perform_signature(
             document_digest=prepared_br_digest.document_digest,
             pdf_cms_signed_attrs=PdfCMSSignedAttributes(
                 signing_time=signing_session.system_time,
                 adobe_revinfo_attr=(
                     None if validation_info is None else
                     validation_info.adobe_revinfo_attr
                 ),
                 cades_signed_attrs=self.signature_meta.cades_signed_attr_spec
             )
         )
 
-        post_signing_doc.post_signature_processing(
+        await post_signing_doc.post_signature_processing(
             res_output, chunk_size=chunk_size
         )
         # we put the finalisation step after the DSS manipulations, since
         # otherwise we'd also run into issues with non-seekable output buffers
         return misc.finalise_output(output, res_output)
 
 
@@ -1028,15 +1326,15 @@
     """
 
     ts_validation_paths: Optional[List[ValidationPath]] = None
     """
     List of validation paths relevant for embedded timestamps.
     """
 
-    adobe_revinfo_attr: Optional[cms.CMSAttribute] = None
+    adobe_revinfo_attr: Optional[asn1_pdf.RevocationInfoArchival] = None
     """
     Preformatted revocation info attribute to include, if requested by the
     settings.
     """
 
     ocsps_to_embed: List[ocsp.OCSPResponse] = None
     """
@@ -1072,16 +1370,16 @@
         self.timestamper = timestamper
         self.subfilter = subfilter
         self.use_pades = subfilter == SigSeedSubFilter.PADES
         self.system_time = \
             system_time or datetime.now(tz=tzlocal.get_localzone())
         self.sv_spec = sv_spec
 
-    def perform_presign_validation(self,
-                                   pdf_out: Optional[BasePdfFileWriter] = None)\
+    async def perform_presign_validation(
+            self, pdf_out: Optional[BasePdfFileWriter] = None)\
             -> Optional[PreSignValidationStatus]:
         """
         Perform certificate validation checks for the signer's certificate,
         including any necessary revocation checks.
 
         This function will also attempt to validate & collect revocation
         information for the relevant TSA (by requesting a dummy timestamp).
@@ -1104,107 +1402,112 @@
         if signature_meta.embed_validation_info:
             if validation_context is None:
                 raise SigningError(
                     'A validation context must be provided if '
                     'validation/revocation info is to be embedded into the '
                     'signature.'
                 )
-            elif not validation_context._allow_fetching:
+            elif not validation_context.fetching_allowed:
                 logger.warning(
                     "Validation/revocation info will be embedded, but "
                     "fetching is not allowed. This may give rise to unexpected "
                     "results."
                 )
         validation_context = signature_meta.validation_context
         # if there's no validation context, bail early
         if validation_context is None:
             return None
 
-        signer_path = self._perform_presign_signer_validation(
+        signer_path = await self._perform_presign_signer_validation(
             validation_context, signature_meta.signer_key_usage
         )
         validation_paths.append(signer_path)
 
         # If LTA:
         # if the original document already included a document timestamp,
         # we need to collect revocation information for it, to preserve
         # the integrity of the timestamp chain
         if signature_meta.use_pades_lta \
                 and isinstance(pdf_out, IncrementalPdfFileWriter):
-            prev_tsa_path = self._perform_prev_ts_validation(
+            prev_tsa_path = await self._perform_prev_ts_validation(
                 validation_context, pdf_out.prev
             )
             if prev_tsa_path is not None:
                 validation_paths.append(prev_tsa_path)
 
         timestamper = self.timestamper
         # Finally, fetch validation information for the TSA that we're going to
         # use for our own TS
-        ts_validation_paths = None
+        ts_paths = None
         if timestamper is not None:
-            ts_validation_paths = list(
-                timestamper.validation_paths(validation_context)
-            )
-            validation_paths.extend(ts_validation_paths)
+            ts_paths = timestamper.validation_paths(validation_context)
+            async for ts_path in ts_paths:
+                validation_paths.append(ts_path)
 
         # do we need adobe-style revocation info?
         if signature_meta.embed_validation_info and not self.use_pades:
             assert validation_context is not None  # checked earlier
             revinfo = Signer.format_revinfo(
                 ocsp_responses=validation_context.ocsps,
                 crls=validation_context.crls
             )
         else:
             # PAdES prescribes another mechanism for embedding revocation info
             revinfo = None
         return PreSignValidationStatus(
             validation_paths=validation_paths,
-            signer_path=signer_path, ts_validation_paths=ts_validation_paths,
+            signer_path=signer_path,
+            ts_validation_paths=ts_paths,
             adobe_revinfo_attr=revinfo,
             ocsps_to_embed=validation_context.ocsps,
             crls_to_embed=validation_context.crls
         )
 
-    def _perform_presign_signer_validation(self, validation_context, key_usage):
+    async def _perform_presign_signer_validation(self, validation_context,
+                                                 key_usage):
 
         signer = self.pdf_signer.signer
         # validate cert
         # (this also keeps track of any validation data automagically)
         validator = CertificateValidator(
             signer.signing_cert, intermediate_certs=signer.cert_registry,
             validation_context=validation_context
         )
         try:
-            signer_cert_validation_path = validator.validate_usage(key_usage)
+            signer_cert_validation_path = \
+                await validator.async_validate_usage(key_usage)
         except (PathBuildingError, PathValidationError) as e:
             raise SigningError(
                 "The signer's certificate could not be validated", e
             )
         return signer_cert_validation_path
 
-    def _perform_prev_ts_validation(self, validation_context, prev_reader):
+    async def _perform_prev_ts_validation(self, validation_context,
+                                          prev_reader):
         signer = self.pdf_signer.signer
         from pyhanko.sign.validation import get_timestamp_chain
+
         # try to grab the most recent document timestamp
         last_ts = None
         try:
             last_ts = next(get_timestamp_chain(prev_reader))
         except StopIteration:
             pass
         last_ts_validation_path = None
         if last_ts is not None:
             ts_validator = CertificateValidator(
                 last_ts.signer_cert,
                 intermediate_certs=signer.cert_registry,
                 validation_context=validation_context
             )
             try:
-                last_ts_validation_path = ts_validator.validate_usage(
+                validate_coro = ts_validator.async_validate_usage(
                     set(), extended_key_usage={"time_stamping"}
                 )
+                last_ts_validation_path = await validate_coro
             except (PathBuildingError, PathValidationError) as e:
                 raise SigningError(
                     "Requested a PAdES-LTA signature on an existing "
                     "document, but the most recent timestamp "
                     "could not be validated.", e
                 )
         return last_ts_validation_path
@@ -1413,26 +1716,61 @@
                     "Reason \"%s\" is not a valid reason for signing, "
                     "please choose one of the following: %s." % (
                         reason_given,
                         ", ".join("\"%s\"" % s for s in sv_spec.reasons)
                     )
                 )
 
+    async def estimate_signature_container_size(
+            self, validation_info: PreSignValidationStatus, tight=False):
+        md_algorithm = self.md_algorithm
+        signature_meta = self.pdf_signer.signature_meta
+        signer = self.pdf_signer.signer
+        # estimate bytes_reserved by creating a fake CMS object
+        md_spec = get_pyca_cryptography_hash(md_algorithm)
+        test_md = hashes.Hash(md_spec).finalize()
+        signed_attrs = PdfCMSSignedAttributes(
+            signing_time=self.system_time,
+            adobe_revinfo_attr=(
+                None if validation_info is None else
+                validation_info.adobe_revinfo_attr
+            ),
+            cades_signed_attrs=signature_meta.cades_signed_attr_spec
+        )
+        test_signature_cms = await signer.async_sign(
+            test_md, md_algorithm, use_pades=self.use_pades,
+            dry_run=True, timestamper=self.timestamper,
+            signed_attr_settings=signed_attrs
+        )
+
+        # Note: multiply by 2 to account for the fact that this byte dump
+        # will be embedded into the resulting PDF as a hexadecimal
+        # string
+        test_len = len(test_signature_cms.dump()) * 2
+
+        if tight:
+            bytes_reserved = test_len
+        else:
+            # External actors such as timestamping servers can't be relied on to
+            # always return exactly the same response, so we build in a 50%
+            # error margin (+ ensure that bytes_reserved is even)
+            bytes_reserved = test_len + 2 * (test_len // 4)
+        return bytes_reserved
+
     def prepare_tbs_document(self, validation_info: PreSignValidationStatus,
-                             bytes_reserved=None, appearance_text_params=None) \
+                             bytes_reserved, appearance_text_params=None) \
             -> 'PdfTBSDocument':
         """
         Set up the signature appearance (if necessary) and signature dictionary
         in the PDF file, to put the document in its final pre-signing state.
 
         :param validation_info:
             Validation information collected prior to signing.
         :param bytes_reserved:
-            Bytes to reserve for the signature container. If ``None``,
-            an estimate will be computed.
+            Bytes to reserve for the signature container.
         :param appearance_text_params:
             Optional text parameters for the signature appearance content.
         :return:
             A :class:`.PdfTBSDocument` describing the document in its final
             pre-signing state.
         """
 
@@ -1441,14 +1779,16 @@
         if self.sv_spec is not None:
             # process the field's seed value constraints
             self._enforce_seed_value_constraints(
                 None if validation_info is None else
                 validation_info.signer_path
             )
 
+        signer = pdf_signer.signer
+        embed_roots = signer.embed_roots
         # take care of DSS updates, if they have to happen now
         dss_settings = signature_meta.dss_settings
         if self.use_pades and validation_info is not None:
             # Check consistency of settings
             dss_settings.assert_viable()
             if dss_settings.placement \
                     == SigDSSPlacementPreference.TOGETHER_WITH_SIGNATURE:
@@ -1457,44 +1797,19 @@
                 # source info directly from the validation_info object
                 # for consistency
                 # NOTE: we have to disable VRI in this scenario
                 validation.DocumentSecurityStore.supply_dss_in_writer(
                     pdf_out, sig_contents=None,
                     paths=validation_info.validation_paths,
                     ocsps=validation_info.ocsps_to_embed,
-                    crls=validation_info.crls_to_embed
+                    crls=validation_info.crls_to_embed,
+                    embed_roots=embed_roots
                 )
 
-        signer = pdf_signer.signer
         md_algorithm = self.md_algorithm
-        if bytes_reserved is None:
-            # estimate bytes_reserved by creating a fake CMS object
-            md_spec = get_pyca_cryptography_hash(md_algorithm)
-            test_md = hashes.Hash(md_spec).finalize()
-            test_signature_cms = signer.sign(
-                test_md, md_algorithm,
-                timestamp=self.system_time, use_pades=self.use_pades,
-                dry_run=True, timestamper=self.timestamper,
-                revocation_info=(
-                    None if validation_info is None else
-                    validation_info.adobe_revinfo_attr
-                ),
-                cades_signed_attr_meta=signature_meta.cades_signed_attr_spec
-            )
-            # Note: multiply by 2 to account for the fact that this byte dump
-            # will be embedded into the resulting PDF as a hexadecimal
-            # string
-            test_len = len(test_signature_cms.dump()) * 2
-            if signature_meta.tight_size_estimates:
-                bytes_reserved = test_len
-            else:
-                # External actors such as timestamping servers can't be relied
-                # on to always return exactly the same response, so we build in
-                # a 50% error margin (+ ensure that bytes_reserved is even)
-                bytes_reserved = test_len + 2 * (test_len // 4)
 
         sig_mdp_setup = self._apply_locking_rules()
 
         # Prepare instructions to the CMS writer to set up the
         # (PDF) signature object and its appearance
         system_time = self.system_time
         name_specified = signature_meta.name
@@ -1533,15 +1848,16 @@
                 #  of MD, and forcing our signers to use the same one to handle
                 #  might be overly restrictive (esp. for things like EdDSA where
                 #  the MD is essentially fixed)
                 timestamp_md_algorithm=md_algorithm,
                 timestamper=doc_timestamper,
                 timestamp_field_name=signature_meta.timestamp_field_name,
                 dss_settings=signature_meta.dss_settings,
-                tight_size_estimates=signature_meta.tight_size_estimates
+                tight_size_estimates=signature_meta.tight_size_estimates,
+                embed_roots=embed_roots
             )
         return PdfTBSDocument(
             cms_writer=self.cms_writer, signer=pdf_signer.signer,
             md_algorithm=md_algorithm, timestamper=self.timestamper,
             use_pades=self.use_pades,
             post_sign_instructions=post_signing_instr,
             validation_context=validation_context
@@ -1596,14 +1912,34 @@
     do not add safety margins.
 
     .. note::
         External TSAs cannot be relied upon to always produce the
         exact same output length, which makes this option risky to use.
     """
 
+    embed_roots: bool = True
+    """
+    .. versionadded:: 0.9.0
+
+    Option that controls whether the root certificate of each validation
+    path should be embedded into the DSS. The default is ``True``.
+
+    .. note::
+        Trust roots are configured by the validator, so embedding them
+        typically does nothing in a typical validation process.
+        Therefore they can be safely omitted in most cases.
+        Nonetheless, embedding the roots can be useful for documentation
+        purposes.
+
+    .. note::
+        This setting is not part of :class:`.DSSContentSettings` because
+        its value is taken from the corresponding property on the
+        :class:`.Signer` involved, not from the initial configuration.
+    """
+
 
 class PdfTBSDocument:
     """
     .. versionadded:: 0.7.0
 
     A PDF document in its final pre-signing state.
 
@@ -1659,16 +1995,16 @@
 
         # pass in I/O parameters, get back a hash
         return self.cms_writer.send(SigIOSetup(
             md_algorithm=self.md_algorithm,
             in_place=in_place, chunk_size=chunk_size, output=output
         ))
 
-    def perform_signature(self, document_digest: bytes,
-                          pdf_cms_signed_attrs: PdfCMSSignedAttributes) \
+    async def perform_signature(self, document_digest: bytes,
+                                pdf_cms_signed_attrs: PdfCMSSignedAttributes) \
             -> 'PdfPostSignatureDocument':
         """
         Perform the relevant cryptographic signing operations on the document
         digest, and write the resulting CMS object to the appropriate location
         in the output stream.
 
         .. warning::
@@ -1679,21 +2015,19 @@
             Digest of the document, as computed over the relevant
             ``/ByteRange``.
         :param pdf_cms_signed_attrs:
             Description of the signed attributes to include.
         :return:
             A :class:`.PdfPostSignatureDocument` object.
         """
-        # Tell the signer to construct a CMS object
-        signature_cms = self.signer.sign(
+        signer = self.signer
+        signature_cms = await signer.async_sign(
             document_digest, self.md_algorithm,
-            timestamp=pdf_cms_signed_attrs.signing_time,
             use_pades=self.use_pades, timestamper=self.timestamper,
-            revocation_info=pdf_cms_signed_attrs.adobe_revinfo_attr,
-            cades_signed_attr_meta=pdf_cms_signed_attrs.cades_signed_attrs
+            signed_attr_settings=pdf_cms_signed_attrs
         )
         # ... and feed it to the CMS writer
         sig_contents = self.cms_writer.send(signature_cms)
         return PdfPostSignatureDocument(
             sig_contents, post_sign_instr=self.post_sign_instructions,
             validation_context=self.validation_context
         )
@@ -1768,24 +2102,70 @@
             This is mainly intended for TSA certificate validation, but it can
             also contain additional validation data to embed in the DSS.
         :param chunk_size:
             Size of the internal buffer (in bytes) used to feed data to the
             message digest function if the input stream does not support
             ``memoryview``.
         """
+        asyncio.run(
+            cls.async_finish_signing(
+                output, prepared_digest, signature_cms,
+                post_sign_instr=post_sign_instr,
+                validation_context=validation_context,
+                chunk_size=chunk_size
+            )
+        )
+
+    @classmethod
+    async def async_finish_signing(cls, output: IO,
+                                   prepared_digest: PreparedByteRangeDigest,
+                                   signature_cms: Union[bytes, cms.ContentInfo],
+                                   post_sign_instr:
+                                   Optional[PostSignInstructions] = None,
+                                   validation_context:
+                                   Optional[ValidationContext] = None,
+                                   chunk_size=misc.DEFAULT_CHUNK_SIZE):
+        """
+        Finish signing after obtaining a CMS object from an external source, and
+        perform any required post-signature processing.
+
+        This is a class method; it doesn't require a :class:`.PdfTBSDocument`
+        instance. Contrast with :meth:`perform_signature`.
+
+        :param output:
+            Output stream housing the document in its final pre-signing state.
+        :param prepared_digest:
+            The prepared digest returned by a prior call to
+            :meth:`digest_tbs_document`.
+        :param signature_cms:
+            CMS object to embed in the signature dictionary.
+        :param post_sign_instr:
+            Instructions for post-signing processing (DSS updates and document
+            timestamps).
+        :param validation_context:
+            Validation context to use in post-signing operations.
+            This is mainly intended for TSA certificate validation, but it can
+            also contain additional validation data to embed in the DSS.
+        :param chunk_size:
+            Size of the internal buffer (in bytes) used to feed data to the
+            message digest function if the input stream does not support
+            ``memoryview``.
+        """
         # TODO at this point, the output stream no longer needs to be readable,
         #  just seekable, unless there's a timestamp requirement.
         #  Might want to factor that out for speed at some point.
         rw_output = misc.prepare_rw_output_stream(output)
         post_sign = cls.resume_signing(
             rw_output, prepared_digest=prepared_digest,
             signature_cms=signature_cms, post_sign_instr=post_sign_instr,
             validation_context=validation_context,
         )
-        post_sign.post_signature_processing(rw_output, chunk_size=chunk_size)
+        await post_sign.post_signature_processing(
+            rw_output, chunk_size=chunk_size
+        )
 
 
 class PdfPostSignatureDocument:
     """
     .. versionadded:: 0.7.0
 
     Represents the final phase of the PDF signing process
@@ -1794,44 +2174,47 @@
     def __init__(self, sig_contents: bytes,
                  post_sign_instr: Optional[PostSignInstructions] = None,
                  validation_context: Optional[ValidationContext] = None):
         self.sig_contents = sig_contents
         self.post_sign_instructions = post_sign_instr
         self.validation_context = validation_context
 
-    def post_signature_processing(self, output: IO,
-                                  chunk_size=misc.DEFAULT_CHUNK_SIZE):
+    async def post_signature_processing(self, output: IO,
+                                        chunk_size=misc.DEFAULT_CHUNK_SIZE):
         """
         Handle DSS updates and LTA timestamps, if applicable.
 
         :param output:
             I/O buffer containing the signed document. Must support
             reading, writing and seeking.
         :param chunk_size:
             Chunk size to use for I/O operations that do not support the buffer
             protocol.
         """
+
         instr = self.post_sign_instructions
         if instr is None:
             return
 
         validation_context = self.validation_context
         validation_info = instr.validation_info
         dss_settings = instr.dss_settings
 
         from pyhanko.sign import validation
+
         # If we're resuming a signing operation, the (new) validation context
         # might not have all relevant OCSP responses / CRLs available.
         # Hence why we also pass in the data from the pre-signing check.
         # The DSS handling code will deal with deduplication.
         dss_op_kwargs = dict(
             paths=validation_info.validation_paths,
             validation_context=validation_context,
             ocsps=validation_info.ocsps_to_embed,
-            crls=validation_info.crls_to_embed
+            crls=validation_info.crls_to_embed,
+            embed_roots=instr.embed_roots
         )
         if dss_settings.include_vri:
             dss_op_kwargs['sig_contents'] = self.sig_contents
         else:
             dss_op_kwargs['sig_contents'] = None
 
         timestamper = instr.timestamper
@@ -1855,15 +2238,16 @@
             pdf_timestamper = PdfTimeStamper(
                 timestamper, field_name=instr.timestamp_field_name
             )
             if dss_placement == SigDSSPlacementPreference.TOGETHER_WITH_NEXT_TS:
                 validation.DocumentSecurityStore.supply_dss_in_writer(
                     w, **dss_op_kwargs
                 )
-            pdf_timestamper.timestamp_pdf(
+            await pdf_timestamper.async_timestamp_pdf(
                 w, instr.timestamp_md_algorithm or constants.DEFAULT_MD,
                 validation_context,
                 validation_paths=validation_info.validation_paths,
                 in_place=True, timestamper=timestamper, chunk_size=chunk_size,
                 dss_settings=dss_settings.get_settings_for_ts(),
-                tight_size_estimates=instr.tight_size_estimates
+                tight_size_estimates=instr.tight_size_estimates,
+                embed_roots=instr.embed_roots
             )
```

### Comparing `pyHanko-0.8.0/pyhanko/sign/validation.py` & `pyHanko-0.9.0/pyhanko/sign/validation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,88 @@
+import asyncio
 import hashlib
-import os
 import logging
+import os
+import warnings
 from collections import namedtuple
-from dataclasses import dataclass, field as data_field
+from dataclasses import dataclass
+from dataclasses import field as data_field
 from datetime import datetime
 from enum import Enum, unique
-from typing import TypeVar, Type, Optional, Union, Iterator, IO
+from typing import IO, Iterator, Optional, Type, TypeVar, Union
 
-from asn1crypto import (
-    cms, tsp, ocsp as asn1_ocsp, pdf as asn1_pdf, crl as asn1_crl, x509, keys,
-    core
-)
+from asn1crypto import cms, core
+from asn1crypto import crl as asn1_crl
+from asn1crypto import keys
+from asn1crypto import ocsp as asn1_ocsp
+from asn1crypto import pdf as asn1_pdf
+from asn1crypto import tsp, x509
 from asn1crypto.x509 import Certificate
 from cryptography.hazmat.primitives import hashes
-
-from pyhanko_certvalidator import ValidationContext, CertificateValidator
+from pyhanko_certvalidator import CertificateValidator, ValidationContext
 from pyhanko_certvalidator.path import ValidationPath
 
 from pyhanko.pdf_utils import generic, misc
 from pyhanko.pdf_utils.generic import pdf_name
 from pyhanko.pdf_utils.incremental_writer import IncrementalPdfFileWriter
-from pyhanko.pdf_utils.misc import OrderedEnum, get_and_apply, \
-    DEFAULT_CHUNK_SIZE
+from pyhanko.pdf_utils.misc import (
+    DEFAULT_CHUNK_SIZE,
+    OrderedEnum,
+    get_and_apply,
+)
 from pyhanko.pdf_utils.reader import (
-    PdfFileReader, XRefCache, process_data_at_eof,
+    PdfFileReader,
+    XRefCache,
+    process_data_at_eof,
 )
 from pyhanko.pdf_utils.rw_common import PdfHandler
+
 from .diff_analysis import (
-    SuspiciousModification, ModificationLevel, DEFAULT_DIFF_POLICY, DiffPolicy,
+    DEFAULT_DIFF_POLICY,
+    DiffPolicy,
     DiffResult,
+    ModificationLevel,
+    SuspiciousModification,
 )
 from .fields import (
-    MDPPerm, FieldMDPSpec, SeedLockDocument, SigSeedValueSpec,
-    SigSeedValFlags, SigSeedSubFilter
+    FieldMDPSpec,
+    MDPPerm,
+    SeedLockDocument,
+    SigSeedSubFilter,
+    SigSeedValFlags,
+    SigSeedValueSpec,
 )
 from .general import (
-    SignatureStatus, find_unique_cms_attribute,
-    UnacceptableSignerError, KeyUsageConstraints,
+    DEFAULT_WEAK_HASH_ALGORITHMS,
+    KeyUsageConstraints,
+    MultivaluedAttributeError,
+    NonexistentAttributeError,
+    SignatureStatus,
     SignatureValidationError,
-    validate_sig_integrity, DEFAULT_WEAK_HASH_ALGORITHMS,
-    get_pyca_cryptography_hash, extract_message_digest, match_issuer_serial,
-    MultivaluedAttributeError, NonexistentAttributeError
+    UnacceptableSignerError,
+    extract_message_digest,
+    find_unique_cms_attribute,
+    get_pyca_cryptography_hash,
+    match_issuer_serial,
+    validate_sig_integrity,
 )
 from .timestamps import TimestampSignatureStatus
 
 __all__ = [
     'SignatureCoverageLevel', 'PdfSignatureStatus', 'DocumentTimestampStatus',
     'StandardCMSSignatureStatus', 'ModificationInfo',
     'EmbeddedPdfSignature', 'DocMDPInfo',
     'RevocationInfoValidationType', 'VRI', 'DocumentSecurityStore',
     'apply_adobe_revocation_info', 'get_timestamp_chain',
-    'read_certification_data', 'validate_pdf_ltv_signature',
-    'validate_pdf_signature', 'validate_cms_signature',
-    'validate_detached_cms', 'validate_pdf_timestamp',
+    'read_certification_data',
+    'validate_pdf_ltv_signature', 'async_validate_pdf_ltv_signature',
+    'validate_pdf_signature', 'async_validate_pdf_signature',
+    'validate_cms_signature', 'async_validate_cms_signature',
+    'validate_detached_cms', 'async_validate_detached_cms',
+    'validate_pdf_timestamp', 'async_validate_pdf_timestamp',
     'collect_validation_info',
     'add_validation_info',
     'ValidationInfoReadingError', 'SigSeedValueValidationError'
 ]
 
 from ..pdf_utils.writer import BasePdfFileWriter
 
@@ -179,21 +205,23 @@
 
     signer_info = _extract_signer_info(signed_data)
     cert, other_certs = partition_certs(certs, signer_info)
 
     return signer_info, cert, other_certs
 
 
-def _validate_cms_signature(signed_data: cms.SignedData,
-                            status_cls: Type[StatusType] = SignatureStatus,
-                            raw_digest: bytes = None,
-                            validation_context: ValidationContext = None,
-                            status_kwargs: dict = None,
-                            key_usage_settings: KeyUsageConstraints = None,
-                            encap_data_invalid=False):
+async def _validate_cms_signature(signed_data: cms.SignedData,
+                                  status_cls:
+                                  Type[StatusType] = SignatureStatus,
+                                  raw_digest: bytes = None,
+                                  validation_context: ValidationContext = None,
+                                  status_kwargs: dict = None,
+                                  key_usage_settings:
+                                  KeyUsageConstraints = None,
+                                  encap_data_invalid=False):
     """
     Validate CMS and PKCS#7 signatures.
     """
     signer_info, cert, other_certs = _extract_signer_info_and_certs(signed_data)
 
     weak_hash_algos = None
     if validation_context is not None:
@@ -230,15 +258,15 @@
     trusted = revoked = False
     path = None
     if valid:
         validator = CertificateValidator(
             cert, intermediate_certs=other_certs,
             validation_context=validation_context
         )
-        trusted, revoked, path = status_cls.validate_cert_usage(
+        trusted, revoked, path = await status_cls.validate_cert_usage(
             validator, key_usage_settings=key_usage_settings
         )
 
     status_kwargs = status_kwargs or {}
     status_kwargs.update(
         intact=intact, valid=valid, signing_cert=cert,
         md_algorithm=md_algorithm, pkcs7_signature_mechanism=mechanism,
@@ -252,19 +280,22 @@
                            status_cls: Type[StatusType] = SignatureStatus,
                            raw_digest: bytes = None,
                            validation_context: ValidationContext = None,
                            status_kwargs: dict = None,
                            key_usage_settings: KeyUsageConstraints = None,
                            encap_data_invalid=False):
     """
-    Validate a CMS signature (i.e. a ``SignedData`` object).
+    .. deprecated:: 0.9.0
+        Use :func:`async_validate_cms_signature` instead.
 
     .. versionchanged:: 0.7.0
         Now handles both detached and enveloping signatures.
 
+    Validate a CMS signature (i.e. a ``SignedData`` object).
+
     :param signed_data:
         The :class:`.asn1crypto.cms.SignedData` object to validate.
     :param status_cls:
         Status class to use for the validation result.
     :param raw_digest:
         Raw digest, computed from context.
     :param validation_context:
@@ -282,43 +313,95 @@
         imprint).
 
         This option is considered internal API, the semantics of which may
         change without notice in the future.
     :return:
         A :class:`.SignatureStatus` object (or an instance of a proper subclass)
     """
-    status_kwargs = _validate_cms_signature(
+
+    warnings.warn(
+        "'validate_cms_signature' is deprecated, use "
+        "'async_validate_cms_signature' instead",
+        DeprecationWarning
+    )
+
+    coro = async_validate_cms_signature(
+        signed_data=signed_data, status_cls=status_cls, raw_digest=raw_digest,
+        validation_context=validation_context, status_kwargs=status_kwargs,
+        key_usage_settings=key_usage_settings,
+        encap_data_invalid=encap_data_invalid
+    )
+    return asyncio.run(coro)
+
+
+async def async_validate_cms_signature(
+                           signed_data: cms.SignedData,
+                           status_cls: Type[StatusType] = SignatureStatus,
+                           raw_digest: bytes = None,
+                           validation_context: ValidationContext = None,
+                           status_kwargs: dict = None,
+                           key_usage_settings: KeyUsageConstraints = None,
+                           encap_data_invalid=False):
+    """
+    Validate a CMS signature (i.e. a ``SignedData`` object).
+
+    :param signed_data:
+        The :class:`.asn1crypto.cms.SignedData` object to validate.
+    :param status_cls:
+        Status class to use for the validation result.
+    :param raw_digest:
+        Raw digest, computed from context.
+    :param validation_context:
+        Validation context to validate the signer's certificate.
+    :param status_kwargs:
+        Other keyword arguments to pass to the ``status_class`` when reporting
+        validation results.
+    :param key_usage_settings:
+        A :class:`.KeyUsageConstraints` object specifying which key usage
+        extensions must or must not be present in the signer's certificate.
+    :param encap_data_invalid:
+        If ``True``, the encapsulated data inside the CMS is invalid,
+        but the remaining validation logic still has to be run (e.g. a
+        timestamp token, which requires validation of the embedded message
+        imprint).
+
+        This option is considered internal API, the semantics of which may
+        change without notice in the future.
+    :return:
+        A :class:`.SignatureStatus` object (or an instance of a proper subclass)
+    """
+    status_kwargs = await _validate_cms_signature(
         signed_data, status_cls, raw_digest, validation_context,
         status_kwargs, key_usage_settings, encap_data_invalid
     )
     return status_cls(**status_kwargs)
 
 
-def collect_timing_info(signer_info: cms.SignerInfo,
-                        ts_validation_context: ValidationContext):
+async def collect_timing_info(signer_info: cms.SignerInfo,
+                              ts_validation_context: ValidationContext):
 
     status_kwargs = {}
 
     # timestamp-related validation
     signer_reported_dt = _extract_self_reported_ts(signer_info)
     if signer_reported_dt is not None:
         status_kwargs['signer_reported_dt'] = signer_reported_dt
 
     tst_signed_data = _extract_tst_data(signer_info, signed=False)
     if tst_signed_data is not None:
-        tst_validity_kwargs = _validate_timestamp(
+        tst_validity_kwargs = await _validate_timestamp(
             tst_signed_data, ts_validation_context,
             _compute_tst_digest(signer_info),
         )
         tst_validity = TimestampSignatureStatus(**tst_validity_kwargs)
         status_kwargs['timestamp_validity'] = tst_validity
 
     content_tst_signed_data = _extract_tst_data(signer_info, signed=True)
     if content_tst_signed_data is not None:
-        content_tst_validity_kwargs = _validate_timestamp(
+        content_tst_validity_kwargs = await _validate_timestamp(
             content_tst_signed_data, ts_validation_context,
             expected_tst_imprint=extract_message_digest(signer_info)
         )
         content_tst_validity = TimestampSignatureStatus(
             **content_tst_validity_kwargs
         )
         status_kwargs['content_timestamp_validity'] = content_tst_validity
@@ -476,14 +559,17 @@
                           signed_data: cms.SignedData,
                           signer_validation_context: ValidationContext = None,
                           ts_validation_context: ValidationContext = None,
                           key_usage_settings: KeyUsageConstraints = None,
                           chunk_size=DEFAULT_CHUNK_SIZE,
                           max_read=None) -> StandardCMSSignatureStatus:
     """
+    .. deprecated:: 0.9.0
+        Use :func:`async_validate_detached_cms` instead.
+
     .. versionadded: 0.7.0
 
     Validate a detached CMS signature.
 
     :param input_data:
         The input data to sign. This can be either a :class:`bytes` object,
         a file-like object or a :class:`cms.ContentInfo` /
@@ -505,33 +591,93 @@
         Chunk size to use when consuming input data.
     :param max_read:
         Maximal number of bytes to read from the input stream.
     :return:
         A description of the signature's status.
     """
 
+    warnings.warn(
+        "'validate_detached_cms' is deprecated, use "
+        "'async_validate_detached_cms' instead",
+        DeprecationWarning
+    )
+
+    coro = async_validate_detached_cms(
+        input_data=input_data,
+        signed_data=signed_data,
+        signer_validation_context=signer_validation_context,
+        ts_validation_context=ts_validation_context,
+        key_usage_settings=key_usage_settings,
+        chunk_size=chunk_size,
+        max_read=max_read
+    )
+    return asyncio.run(coro)
+
+
+async def async_validate_detached_cms(
+        input_data: Union[bytes, IO,
+                          cms.ContentInfo, cms.EncapsulatedContentInfo],
+        signed_data: cms.SignedData,
+        signer_validation_context: ValidationContext = None,
+        ts_validation_context: ValidationContext = None,
+        key_usage_settings: KeyUsageConstraints = None,
+        chunk_size=DEFAULT_CHUNK_SIZE,
+        max_read=None
+    ) -> StandardCMSSignatureStatus:
+    """
+    .. versionadded: 0.9.0
+
+    Validate a detached CMS signature.
+
+    :param input_data:
+        The input data to sign. This can be either a :class:`bytes` object,
+        a file-like object or a :class:`cms.ContentInfo` /
+        :class:`cms.EncapsulatedContentInfo` object.
+
+        If a CMS content info object is passed in, the `content` field
+        will be extracted.
+    :param signed_data:
+        The :class:`cms.SignedData` object containing the signature to verify.
+    :param signer_validation_context:
+        Validation context to use to verify the signer certificate's trust.
+    :param ts_validation_context:
+        Validation context to use to verify the TSA certificate's trust, if
+        a timestamp token is present.
+        By default, the same validation context as that of the signer is used.
+    :param key_usage_settings:
+        Key usage parameters for the signer.
+    :param chunk_size:
+        Chunk size to use when consuming input data.
+    :param max_read:
+        Maximal number of bytes to read from the input stream.
+    :return:
+        A description of the signature's status.
+    """
+
     if ts_validation_context is None:
         ts_validation_context = signer_validation_context
     signer_info = _extract_signer_info(signed_data)
     digest_algorithm = signer_info['digest_algorithm']['algorithm'].native
     h = hashes.Hash(get_pyca_cryptography_hash(digest_algorithm))
     if isinstance(input_data, bytes):
         h.update(input_data)
     elif isinstance(input_data, (cms.ContentInfo, cms.EncapsulatedContentInfo)):
         h.update(bytes(input_data['content']))
     else:
         temp_buf = bytearray(chunk_size)
         misc.chunked_digest(temp_buf, input_data, h, max_read=max_read)
     digest_bytes = h.finalize()
 
-    return validate_cms_signature(
+    status_kwargs = \
+        await collect_timing_info(signer_info, ts_validation_context)
+    return await async_validate_cms_signature(
         signed_data, status_cls=StandardCMSSignatureStatus,
         raw_digest=digest_bytes,
         validation_context=signer_validation_context,
-        status_kwargs=collect_timing_info(signer_info, ts_validation_context),
+        status_kwargs=status_kwargs,
         key_usage_settings=key_usage_settings
     )
 
 
 @unique
 class SignatureCoverageLevel(OrderedEnum):
     """
@@ -1409,14 +1555,56 @@
         A :class:`.KeyUsageConstraints` object specifying which key usage
         extensions must or must not be present in the signer's certificate.
     :param skip_diff:
         If ``True``, skip the difference analysis step entirely.
     :return:
         The status of the PDF signature in question.
     """
+    coro = async_validate_pdf_signature(
+        embedded_sig=embedded_sig,
+        signer_validation_context=signer_validation_context,
+        ts_validation_context=ts_validation_context,
+        diff_policy=diff_policy, key_usage_settings=key_usage_settings,
+        skip_diff=skip_diff
+    )
+    return asyncio.run(coro)
+
+
+async def async_validate_pdf_signature(
+                           embedded_sig: EmbeddedPdfSignature,
+                           signer_validation_context: ValidationContext = None,
+                           ts_validation_context: ValidationContext = None,
+                           diff_policy: DiffPolicy = None,
+                           key_usage_settings: KeyUsageConstraints = None,
+                           skip_diff: bool = False) -> PdfSignatureStatus:
+    """
+    .. versionadded:: 0.9.0
+
+    Validate a PDF signature.
+
+    :param embedded_sig:
+        Embedded signature to evaluate.
+    :param signer_validation_context:
+        Validation context to use to validate the signature's chain of trust.
+    :param ts_validation_context:
+        Validation context to use to validate the timestamp's chain of trust
+        (defaults to ``signer_validation_context``).
+    :param diff_policy:
+        Policy to evaluate potential incremental updates that were appended
+        to the signed revision of the document.
+        Defaults to
+        :const:`~pyhanko.sign.diff_analysis.DEFAULT_DIFF_POLICY`.
+    :param key_usage_settings:
+        A :class:`.KeyUsageConstraints` object specifying which key usage
+        extensions must or must not be present in the signer's certificate.
+    :param skip_diff:
+        If ``True``, skip the difference analysis step entirely.
+    :return:
+        The status of the PDF signature in question.
+    """
 
     sig_object = embedded_sig.sig_object
     if embedded_sig.sig_object_type != '/Sig':
         raise SignatureValidationError("Signature object type must be /Sig")
 
     # check whether the subfilter type is one we support
     subfilter_str = sig_object.get('/SubFilter', None)
@@ -1430,24 +1618,25 @@
         ts_validation_context = signer_validation_context
 
     embedded_sig.compute_integrity_info(
         diff_policy=diff_policy, skip_diff=skip_diff
     )
     status_kwargs = embedded_sig.summarise_integrity_info()
 
-    status_kwargs.update(
-        collect_timing_info(embedded_sig.signer_info, ts_validation_context)
+    ts_status_kwargs = await collect_timing_info(
+        embedded_sig.signer_info, ts_validation_context
     )
+    status_kwargs.update(ts_status_kwargs)
     if 'signer_reported_dt' not in status_kwargs:
         # maybe the PDF signature dictionary declares /M
         signer_reported_dt = embedded_sig.self_reported_timestamp
         if signer_reported_dt is not None:
             status_kwargs['signer_reported_dt'] = signer_reported_dt
 
-    status_kwargs = _validate_cms_signature(
+    status_kwargs = await _validate_cms_signature(
         embedded_sig.signed_data, status_cls=PdfSignatureStatus,
         raw_digest=embedded_sig.external_digest,
         validation_context=signer_validation_context,
         status_kwargs=status_kwargs, key_usage_settings=key_usage_settings
     )
     tst_validity = status_kwargs.get('timestamp_validity', None)
     timestamp_found = (
@@ -1459,14 +1648,49 @@
 
 
 def validate_pdf_timestamp(embedded_sig: EmbeddedPdfSignature,
                            validation_context: ValidationContext = None,
                            diff_policy: DiffPolicy = None,
                            skip_diff: bool = False) -> DocumentTimestampStatus:
     """
+    .. versionchanged:: 0.9.0
+        Wrapper around :func:`async_validate_pdf_timestamp`.
+
+    Validate a PDF document timestamp.
+
+    :param embedded_sig:
+        Embedded signature to evaluate.
+    :param validation_context:
+        Validation context to use to validate the timestamp's chain of trust.
+    :param diff_policy:
+        Policy to evaluate potential incremental updates that were appended
+        to the signed revision of the document.
+        Defaults to
+        :const:`~pyhanko.sign.diff_analysis.DEFAULT_DIFF_POLICY`.
+    :param skip_diff:
+        If ``True``, skip the difference analysis step entirely.
+    :return:
+        The status of the PDF timestamp in question.
+    """
+    coro = async_validate_pdf_timestamp(
+        embedded_sig=embedded_sig,
+        validation_context=validation_context,
+        diff_policy=diff_policy, skip_diff=skip_diff
+    )
+    return asyncio.run(coro)
+
+
+async def async_validate_pdf_timestamp(
+                           embedded_sig: EmbeddedPdfSignature,
+                           validation_context: ValidationContext = None,
+                           diff_policy: DiffPolicy = None,
+                           skip_diff: bool = False) -> DocumentTimestampStatus:
+    """
+    .. versionadded:: 0.9.0
+
     Validate a PDF document timestamp.
 
     :param embedded_sig:
         Embedded signature to evaluate.
     :param validation_context:
         Validation context to use to validate the timestamp's chain of trust.
     :param diff_policy:
@@ -1492,15 +1716,15 @@
         "%s is not a recognized SubFilter type for timestamps."
     )
 
     embedded_sig.compute_integrity_info(
         diff_policy=diff_policy, skip_diff=skip_diff
     )
 
-    status_kwargs = _validate_timestamp(
+    status_kwargs = await _validate_timestamp(
         embedded_sig.signed_data, validation_context,
         embedded_sig.external_digest
     )
 
     status_kwargs['coverage'] = embedded_sig.coverage
     status_kwargs['diff_result'] = embedded_sig.diff_result
     return DocumentTimestampStatus(**status_kwargs)
@@ -1545,16 +1769,16 @@
     # Certs with OCSP/CRL endpoints should have the relevant revocation data
     # embedded, if no stricter revocation_mode policy is in place already
     rm = validation_context_kwargs.get('revocation_mode', None)
     if not rm or rm == 'soft-fail':
         validation_context_kwargs['revocation_mode'] = 'hard-fail'
 
 
-def _validate_timestamp(tst_signed_data, validation_context,
-                        expected_tst_imprint):
+async def _validate_timestamp(tst_signed_data, validation_context,
+                              expected_tst_imprint):
 
     assert expected_tst_imprint is not None
     tst_info = tst_signed_data['encap_content_info']['content'].parsed
     assert isinstance(tst_info, tsp.TSTInfo)
     # compare the expected TST digest against the message imprint
     # inside the signed data
     tst_imprint = tst_info['message_imprint']['hashed_message'].native
@@ -1563,25 +1787,25 @@
             f"Timestamp token imprint is {tst_imprint.hex()}, but expected "
             f"{expected_tst_imprint.hex()}."
         )
         encap_data_invalid = True
     else:
         encap_data_invalid = False
     timestamp = tst_info['gen_time'].native
-    return _validate_cms_signature(
+    return await _validate_cms_signature(
         tst_signed_data, status_cls=TimestampSignatureStatus,
         validation_context=validation_context,
         status_kwargs={'timestamp': timestamp},
         encap_data_invalid=encap_data_invalid
     )
 
 
-def _establish_timestamp_trust(tst_signed_data, bootstrap_validation_context,
-                               expected_tst_imprint):
-    timestamp_status_kwargs = _validate_timestamp(
+async def _establish_timestamp_trust(
+        tst_signed_data, bootstrap_validation_context, expected_tst_imprint):
+    timestamp_status_kwargs = await _validate_timestamp(
         tst_signed_data, bootstrap_validation_context, expected_tst_imprint
     )
     timestamp_status = TimestampSignatureStatus(**timestamp_status_kwargs)
 
     if not timestamp_status.valid or not timestamp_status.trusted:
         logger.warning(
             "Could not validate embedded timestamp token: %s.",
@@ -1608,28 +1832,28 @@
     """
     return filter(
         lambda sig: sig.sig_object.get('/Type', None) == '/DocTimeStamp',
         reversed(reader.embedded_signatures)
     )
 
 
-def _establish_timestamp_trust_lta(reader, bootstrap_validation_context,
+async def _establish_timestamp_trust_lta(reader, bootstrap_validation_context,
                                    validation_context_kwargs, until_revision):
     timestamps = get_timestamp_chain(reader)
     validation_context_kwargs = dict(validation_context_kwargs)
     current_vc = bootstrap_validation_context
     ts_status = None
     ts_count = -1
     emb_timestamp = None
     for ts_count, emb_timestamp in enumerate(timestamps):
         if emb_timestamp.signed_revision < until_revision:
             break
 
         emb_timestamp.compute_digest()
-        ts_status = _establish_timestamp_trust(
+        ts_status = await _establish_timestamp_trust(
             emb_timestamp.signed_data, current_vc, emb_timestamp.external_digest
         )
         # set up the validation kwargs for the next iteration
         _strict_vc_context_kwargs(
             ts_status.timestamp, validation_context_kwargs
         )
         # read the DSS at the current revision into a new
@@ -1656,14 +1880,70 @@
                                validation_context_kwargs=None,
                                bootstrap_validation_context=None,
                                force_revinfo=False,
                                diff_policy: DiffPolicy = None,
                                key_usage_settings: KeyUsageConstraints = None,
                                skip_diff: bool = False) -> PdfSignatureStatus:
     """
+    .. versionchanged:: 0.9.0
+        Wrapper around :func:`async_validate_pdf_ltv_signature`.
+
+    Validate a PDF LTV signature according to a particular profile.
+
+    :param embedded_sig:
+        Embedded signature to evaluate.
+    :param validation_type:
+        Validation profile to use.
+    :param validation_context_kwargs:
+        Keyword args to instantiate
+        :class:`.pyhanko_certvalidator.ValidationContext` objects needed over
+        the course of the validation.
+    :param bootstrap_validation_context:
+        Validation context used to validate the current timestamp.
+    :param force_revinfo:
+        Require all certificates encountered to have some form of live
+        revocation checking provisions.
+    :param diff_policy:
+        Policy to evaluate potential incremental updates that were appended
+        to the signed revision of the document.
+        Defaults to
+        :const:`~pyhanko.sign.diff_analysis.DEFAULT_DIFF_POLICY`.
+    :param key_usage_settings:
+        A :class:`.KeyUsageConstraints` object specifying which key usage
+        extensions must or must not be present in the signer's certificate.
+    :param skip_diff:
+        If ``True``, skip the difference analysis step entirely.
+    :return:
+        The status of the signature.
+    """
+    coro = async_validate_pdf_ltv_signature(
+        embedded_sig=embedded_sig,
+        validation_type=validation_type,
+        validation_context_kwargs=validation_context_kwargs,
+        bootstrap_validation_context=bootstrap_validation_context,
+        force_revinfo=force_revinfo,
+        diff_policy=diff_policy,
+        key_usage_settings=key_usage_settings,
+        skip_diff=skip_diff
+    )
+    return asyncio.run(coro)
+
+
+async def async_validate_pdf_ltv_signature(
+                               embedded_sig: EmbeddedPdfSignature,
+                               validation_type: RevocationInfoValidationType,
+                               validation_context_kwargs=None,
+                               bootstrap_validation_context=None,
+                               force_revinfo=False,
+                               diff_policy: DiffPolicy = None,
+                               key_usage_settings: KeyUsageConstraints = None,
+                               skip_diff: bool = False) -> PdfSignatureStatus:
+    """
+    .. versionadded:: 0.9.0
+
     Validate a PDF LTV signature according to a particular profile.
 
     :param embedded_sig:
         Embedded signature to evaluate.
     :param validation_type:
         Validation profile to use.
     :param validation_context_kwargs:
@@ -1684,14 +1964,15 @@
         A :class:`.KeyUsageConstraints` object specifying which key usage
         extensions must or must not be present in the signer's certificate.
     :param skip_diff:
         If ``True``, skip the difference analysis step entirely.
     :return:
         The status of the signature.
     """
+
     # create a fresh copy of the validation_kwargs
     validation_context_kwargs: dict = dict(validation_context_kwargs or {})
 
     # To validate the first timestamp, allow fetching by default
     # we'll turn it off later
     validation_context_kwargs.setdefault('allow_fetching', True)
     # same for revocation_mode: if force_revinfo is false, we simply turn on
@@ -1733,15 +2014,15 @@
     earliest_good_timestamp_st = None
     ts_chain_length = 0
     # also record the embedded sig object assoc. with the oldest applicable
     # DTS in the timestamp chain
     latest_dts = None
     if validation_type != RevocationInfoValidationType.ADOBE_STYLE:
         latest_dts, earliest_good_timestamp_st, ts_chain_length, current_vc = \
-            _establish_timestamp_trust_lta(
+            await _establish_timestamp_trust_lta(
                 reader, current_vc, validation_context_kwargs,
                 until_revision=embedded_sig.signed_revision
             )
         # In PAdES-LTA, we should only rely on DSS information that is covered
         # by an appropriate document timestamp.
         # If the validation profile is PAdES-LTA, then we must have seen
         # at least one document timestamp pass by, i.e. earliest_known_timestamp
@@ -1757,15 +2038,15 @@
 
     # now that we have arrived at the revision with the signature,
     # we can check for a timestamp token attribute there
     # (This is allowed, regardless of whether we use Adobe-style LTV or
     # a PAdES validation profile)
     tst_signed_data = embedded_sig.attached_timestamp_data
     if tst_signed_data is not None:
-        earliest_good_timestamp_st = _establish_timestamp_trust(
+        earliest_good_timestamp_st = await _establish_timestamp_trust(
             tst_signed_data, current_vc, embedded_sig.tst_signature_digest
         )
     elif validation_type == RevocationInfoValidationType.PADES_LTA \
             and ts_chain_length == 1:
         # TODO Pretty sure that this is the spirit of the LTA profile,
         #  but are we being too harsh here? I don't think so, but it's worth
         #  revisiting later
@@ -1820,35 +2101,36 @@
         if tst_signed_data is not None:
             ts_to_validate = tst_signed_data
         else:
             # we're in the PAdES-LT case with a detached TST now.
             # this should be conceptually equivalent to the above
             # so we run the same check here
             ts_to_validate = latest_dts.signed_data
-        timestamp_status: TimestampSignatureStatus = validate_cms_signature(
+        ts_status_coro = async_validate_cms_signature(
             ts_to_validate, status_cls=TimestampSignatureStatus,
             validation_context=stored_vc, status_kwargs={
                 'timestamp': earliest_good_timestamp_st.timestamp
             }
         )
+        timestamp_status: TimestampSignatureStatus = await ts_status_coro
     else:
         # In the LTA case, we don't have to do any further checks, since the
         # _establish_timestamp_trust_lta handled that for us.
         # We can therefore just take earliest_good_timestamp_st at face value.
         timestamp_status = earliest_good_timestamp_st
 
     embedded_sig.compute_integrity_info(
         diff_policy=diff_policy, skip_diff=skip_diff
     )
     status_kwargs = embedded_sig.summarise_integrity_info()
     status_kwargs.update({
         'signer_reported_dt': earliest_good_timestamp_st.timestamp,
         'timestamp_validity': timestamp_status
     })
-    status_kwargs = _validate_cms_signature(
+    status_kwargs = await _validate_cms_signature(
         embedded_sig.signed_data, status_cls=PdfSignatureStatus,
         raw_digest=embedded_sig.external_digest,
         validation_context=stored_vc, status_kwargs=status_kwargs,
         key_usage_settings=key_usage_settings
     )
 
     _validate_sv_and_update(embedded_sig, status_kwargs, timestamp_found=True)
@@ -1889,15 +2171,15 @@
     ocsps, crls = retrieve_adobe_revocation_info(signer_info)
     return ValidationContext(
         ocsps=ocsps, crls=crls, **validation_context_kwargs
     )
 
 
 DocMDPInfo = namedtuple(
-    'DocMDPInfo', ['permission', 'digest_method', 'author_sig']
+    'DocMDPInfo', ['permission', 'author_sig']
 )
 """
 Encodes certification information for a signed document, consisting of a 
 reference to the author signature, together with the associated DocMDP policy.
 """
 
 
@@ -1912,22 +2194,15 @@
     """
     try:
         certification_sig = reader.root['/Perms']['/DocMDP']
     except KeyError:
         return
 
     perm = _extract_docmdp_for_sig(certification_sig)
-    ref = _extract_reference_dict(certification_sig, '/DocMDP')
-    md = None
-    if ref is not None:
-        md = misc.get_and_apply(
-            ref, '/DigestMethod', lambda x: x[1:].lower()
-        )
-
-    return DocMDPInfo(perm, md, certification_sig)
+    return DocMDPInfo(perm, certification_sig)
 
 
 @dataclass
 class VRI:
     """
     VRI dictionary as defined in PAdES / ISO 32000-2.
     These dictionaries collect data that may be relevant for the validation of
@@ -1976,17 +2251,17 @@
     if status == 'successful':
         response_bytes = ocsp_response['response_bytes']
         if response_bytes['response_type'].native == 'basic_ocsp_response':
             response = response_bytes['response'].parsed
             yield from response['certs']
 
 
-def collect_validation_info(embedded_sig: EmbeddedPdfSignature,
-                            validation_context: ValidationContext,
-                            skip_timestamp=False):
+async def collect_validation_info(embedded_sig: EmbeddedPdfSignature,
+                                  validation_context: ValidationContext,
+                                  skip_timestamp=False):
     """
     Query revocation info for a PDF signature using a validation context,
     and store the results in a validation context.
 
     This works by validating the signer's certificate against the provided
     validation context, which causes revocation info to be cached for
     later retrieval.
@@ -2010,38 +2285,91 @@
         logger.warning(
             "Revocation mode is set to soft-fail; collected revocation "
             "information may be incomplete."
         )
 
     paths = []
 
-    def _validate_signed_data(signed_data):
+    async def _validate_signed_data(signed_data):
         signer_info, cert, other_certs = \
             _extract_signer_info_and_certs(signed_data)
 
         validator = CertificateValidator(
             cert, intermediate_certs=other_certs,
             validation_context=validation_context
         )
-        path = validator.validate_usage(key_usage=set())
+        path = await validator.async_validate_usage(key_usage=set())
         paths.append(path)
 
-    _validate_signed_data(embedded_sig.signed_data)
+    await _validate_signed_data(embedded_sig.signed_data)
     if not skip_timestamp and embedded_sig.attached_timestamp_data is not None:
-        _validate_signed_data(embedded_sig.attached_timestamp_data)
+        await _validate_signed_data(embedded_sig.attached_timestamp_data)
 
     return paths
 
 
 def add_validation_info(embedded_sig: EmbeddedPdfSignature,
                         validation_context: ValidationContext,
                         skip_timestamp=False, add_vri_entry=True,
                         in_place=False, output=None, force_write=False,
                         chunk_size=DEFAULT_CHUNK_SIZE):
     """
+    .. versionchanged:: 0.9.0
+        Wrapper around :func:`async_add_validation_info`
+
+    Add validation info (CRLs, OCSP responses, extra certificates) for a
+    signature to the DSS of a document in an incremental update.
+
+    :param embedded_sig:
+        The signature for which the revocation information needs to be
+        collected.
+    :param validation_context:
+        The validation context to use.
+    :param skip_timestamp:
+        If ``True``, do not attempt to validate the timestamp attached to
+        the signature, if one is present.
+    :param add_vri_entry:
+        Add a ``/VRI`` entry for this signature to the document security store.
+        Default is ``True``.
+    :param output:
+        Write the output to the specified output stream.
+        If ``None``, write to a new :class:`.BytesIO` object.
+        Default is ``None``.
+    :param in_place:
+        Sign the original input stream in-place.
+        This parameter overrides ``output``.
+    :param chunk_size:
+        Chunk size parameter to use when copying output to a new stream
+        (irrelevant if ``in_place`` is ``True``).
+    :param force_write:
+        Force a new revision to be written, even if not necessary (i.e.
+        when all data in the validation context is already present in the DSS).
+    :return:
+        The (file-like) output object to which the result was written.
+    """
+
+    coro = async_add_validation_info(
+        embedded_sig=embedded_sig, validation_context=validation_context,
+        skip_timestamp=skip_timestamp, add_vri_entry=add_vri_entry,
+        output=output, in_place=in_place, chunk_size=chunk_size,
+        force_write=force_write
+    )
+    return asyncio.run(coro)
+
+
+async def async_add_validation_info(embedded_sig: EmbeddedPdfSignature,
+                                    validation_context: ValidationContext,
+                                    skip_timestamp=False, add_vri_entry=True,
+                                    in_place=False, output=None,
+                                    force_write=False,
+                                    chunk_size=DEFAULT_CHUNK_SIZE,
+                                    embed_roots: bool = True):
+    """
+    .. versionadded: 0.9.0
+
     Add validation info (CRLs, OCSP responses, extra certificates) for a
     signature to the DSS of a document in an incremental update.
     This is a wrapper around :func:`collect_validation_info`.
 
     :param embedded_sig:
         The signature for which the revocation information needs to be
         collected.
@@ -2062,14 +2390,24 @@
         This parameter overrides ``output``.
     :param chunk_size:
         Chunk size parameter to use when copying output to a new stream
         (irrelevant if ``in_place`` is ``True``).
     :param force_write:
         Force a new revision to be written, even if not necessary (i.e.
         when all data in the validation context is already present in the DSS).
+    :param embed_roots:
+        Option that controls whether the root certificate of each validation
+        path should be embedded into the DSS. The default is ``True``.
+
+        .. note::
+            Trust roots are configured by the validator, so embedding them
+            typically does nothing in a typical validation process.
+            Therefore they can be safely omitted in most cases.
+            Nonetheless, embedding the roots can be useful for documentation
+            purposes.
     :return:
         The (file-like) output object to which the result was written.
     """
 
     reader: PdfFileReader = embedded_sig.reader
     # Take care of this first, so we get any errors re: stream properties
     # out of the way before doing the (potentially) expensive validation
@@ -2081,28 +2419,28 @@
         # raise an error if the output is not writable.
         # We put it in for forwards compatibility & consistency with future
         # changes to I/O internals.
         misc.assert_writable_and_random_access(output)
     else:
         working_output = misc.prepare_rw_output_stream(output)
 
-    paths = collect_validation_info(
+    paths = await collect_validation_info(
         embedded_sig, validation_context, skip_timestamp=skip_timestamp
     )
 
     if add_vri_entry:
         sig_contents = embedded_sig.pkcs7_content.hex().encode('ascii')
     else:
         sig_contents = None
 
     pdf_out = IncrementalPdfFileWriter.from_reader(reader)
     pdf_out.IO_CHUNK_SIZE = chunk_size
     resulting_dss = DocumentSecurityStore.supply_dss_in_writer(
         pdf_out, sig_contents, validation_context=validation_context,
-        paths=paths
+        paths=paths, embed_roots=embed_roots
     )
     if force_write or resulting_dss.modified:
         if in_place:
             pdf_out.write_in_place()
         else:
             pdf_out.write(working_output)
     elif not in_place:
@@ -2378,15 +2716,16 @@
         )
         return dss
 
     @classmethod
     def supply_dss_in_writer(cls, pdf_out: BasePdfFileWriter,
                              sig_contents, *, certs=None,
                              ocsps=None, crls=None, paths=None,
-                             validation_context=None) \
+                             validation_context=None,
+                             embed_roots: bool = True) \
             -> 'DocumentSecurityStore':
         """
         Add or update a DSS, and optionally associate the new information with a
         VRI entry tied to a signature object.
 
         You can either specify the CMS objects to include directly, or
         pass them in as output from `pyhanko_certvalidator`.
@@ -2405,14 +2744,30 @@
         :param crls:
             CRLs to include in the VRI entry.
         :param paths:
             Validation paths that have been established, and need to be added
             to the DSS.
         :param validation_context:
             Validation context from which to draw OCSP responses and CRLs.
+        :param embed_roots:
+            .. versionadded:: 0.9.0
+
+            Option that controls whether the root certificate of each validation
+            path should be embedded into the DSS. The default is ``True``.
+
+            .. note::
+                Trust roots are configured by the validator, so embedding them
+                typically does nothing in a typical validation process.
+                Therefore they can be safely omitted in most cases.
+                Nonetheless, embedding the roots can be useful for documentation
+                purposes.
+
+            .. warning::
+                This only applies to paths, not the ``certs`` parameter.
+
         :return:
             a :class:`DocumentSecurityStore` object containing both the new
             and existing contents of the DSS (if any).
         """
         try:
             dss = cls.read_dss(pdf_out)
             created = False
@@ -2426,15 +2781,19 @@
         else:
             identifier = None
 
         def _certs():
             yield from certs or ()
             path: ValidationPath
             for path in (paths or ()):
-                yield from path
+                path_parts = iter(path)
+                if not embed_roots:
+                    # skip the first cert (i.e. the root)
+                    next(path_parts)
+                yield from path_parts
 
         def _ocsps():
             yield from ocsps or ()
             if validation_context is not None:
                 yield from validation_context.ocsps
 
         def _crls():
@@ -2454,15 +2813,15 @@
             pdf_out.root[pdf_name('/DSS')] = dss_ref
             pdf_out.update_root()
         return dss
 
     @classmethod
     def add_dss(cls, output_stream, sig_contents, *, certs=None,
                 ocsps=None, crls=None, paths=None, validation_context=None,
-                force_write=False):
+                force_write: bool = False, embed_roots: bool = True):
         """
         Wrapper around :meth:`supply_dss_in_writer`.
 
         The result is applied to the output stream as an incremental update.
 
         :param output_stream:
             Output stream to write to.
@@ -2480,15 +2839,32 @@
         :param paths:
             Validation paths that have been established, and need to be added
             to the DSS.
         :param force_write:
             Force a write even if the DSS doesn't have any new content.
         :param validation_context:
             Validation context from which to draw OCSP responses and CRLs.
+        :param embed_roots:
+            .. versionadded:: 0.9.0
+
+            Option that controls whether the root certificate of each validation
+            path should be embedded into the DSS. The default is ``True``.
+
+            .. note::
+                Trust roots are configured by the validator, so embedding them
+                typically does nothing in a typical validation process.
+                Therefore they can be safely omitted in most cases.
+                Nonetheless, embedding the roots can be useful for documentation
+                purposes.
+
+            .. warning::
+                This only applies to paths, not the ``certs`` parameter.
+
         """
         pdf_out = IncrementalPdfFileWriter(output_stream)
         dss = cls.supply_dss_in_writer(
             pdf_out, sig_contents, certs=certs, ocsps=ocsps,
-            crls=crls, paths=paths, validation_context=validation_context
+            crls=crls, paths=paths, validation_context=validation_context,
+            embed_roots=embed_roots
         )
         if force_write or dss.modified:
             pdf_out.write_in_place()
```

### Comparing `pyHanko-0.8.0/pyhanko/stamp.py` & `pyHanko-0.9.0/pyhanko/stamp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,29 @@
 
 The code in this module is also used by the :mod:`.sign` module to render
 signature appearances.
 """
 import enum
 import uuid
 from binascii import hexlify
+from dataclasses import dataclass
+from datetime import datetime
 from typing import Optional
 
 import qrcode
 import tzlocal
 
+from pyhanko.pdf_utils import content, generic, layout
+from pyhanko.pdf_utils.config_utils import ConfigurableMixin, ConfigurationError
+from pyhanko.pdf_utils.generic import pdf_name, pdf_string
 from pyhanko.pdf_utils.incremental_writer import IncrementalPdfFileWriter
 from pyhanko.pdf_utils.misc import rd
-from pyhanko.pdf_utils.text import TextBoxStyle, TextBox, DEFAULT_BOX_LAYOUT
-from pyhanko.pdf_utils.writer import (
-    init_xobject_dictionary, BasePdfFileWriter
-)
-from dataclasses import dataclass
-from datetime import datetime
-
-from pyhanko.pdf_utils import generic, layout
-from pyhanko.pdf_utils.generic import (
-    pdf_name, pdf_string,
-)
-from pyhanko.pdf_utils import content
-from pyhanko.pdf_utils.config_utils import ConfigurableMixin, ConfigurationError
 from pyhanko.pdf_utils.qr import PdfStreamQRImage
-
+from pyhanko.pdf_utils.text import DEFAULT_BOX_LAYOUT, TextBox, TextBoxStyle
+from pyhanko.pdf_utils.writer import BasePdfFileWriter, init_xobject_dictionary
 
 __all__ = [
     "AnnotAppearances",
     "BaseStampStyle", "TextStampStyle", "QRStampStyle", "StaticStampStyle",
     "QRPosition",
     "BaseStamp", "TextStamp", "QRStamp", "StaticContentStamp",
     "text_stamp_file", "qr_stamp_file",
@@ -98,16 +91,17 @@
     # the module
     if bg_spec == '__stamp__':
         return STAMP_ART_CONTENT
     elif bg_spec.endswith('.pdf'):
         # import first page of PDF as background
         return content.ImportedPdfPage(bg_spec)
     else:
-        from pyhanko.pdf_utils.images import PdfImage
         from PIL import Image
+
+        from pyhanko.pdf_utils.images import PdfImage
         img = Image.open(bg_spec)
         # Setting the writer can be delayed
         return PdfImage(img, writer=None)
 
 
 @dataclass(frozen=True)
 class BaseStampStyle(ConfigurableMixin):
```

### Comparing `pyHanko-0.8.0/setup.py` & `pyHanko-0.9.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from setuptools import setup
 from os import path
 
+from setuptools import setup
+
 BASE_DIR = path.abspath(path.dirname(__file__))
 with open(path.join(BASE_DIR, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 # based on https://packaging.python.org/guides/single-sourcing-package-version/
 def get_version():
@@ -20,14 +21,15 @@
 setup(
     name='pyHanko',
     version=get_version(),
     packages=[
         'pyhanko',
         'pyhanko.pdf_utils', 'pyhanko.pdf_utils.font',
         'pyhanko.sign', 'pyhanko.sign.ades', 'pyhanko.sign.signers',
+        'pyhanko.sign.timestamps'
     ],
     url='https://github.com/MatthiasValvekens/pyHanko',
     license='MIT',
     author='Matthias Valvekens',
     author_email='dev@mvalvekens.be',
     description='Tools for stamping and signing PDF files',
     long_description=long_description,
@@ -52,35 +54,35 @@
         ]
     },
     install_requires=[
         'asn1crypto>=1.4.0',
         'pytz>=2020.1',
         'qrcode>=6.1',
         'tzlocal>=2.1',
-        'pyhanko-certvalidator~=0.16.0',
+        'pyhanko-certvalidator~=0.17.3',
         'click>=7.1.2',
         'requests>=2.24.0',
         'pyyaml>=5.3.1',
         'cryptography>=3.3.1'
     ],
     setup_requires=[
         'wheel', 'pytest-runner'
     ],
     extras_require={
         'extra_pubkey_algs': ['oscrypto>=1.2.1'],
-        'opentype': ['fonttools>=4.13.0', 'uharfbuzz==0.16.1'],
+        'opentype': ['fonttools>=4.27.1', 'uharfbuzz==0.16.1'],
         'image-support': [
             # Only tested systematically on 8.x,
             # but we allow 7.2.x to support system PIL on Ubuntu
             'Pillow>=7.2.0',
             'python-barcode>=0.13.1',
         ],
-        'pkcs11': ['python-pkcs11>=0.6.0']
+        'pkcs11': ['python-pkcs11~=0.7.0'],
+        'async_http': ['aiohttp~=3.7.4']
     },
     tests_require=[
-        'pytest>=6.1.1',
-        'requests-mock>=1.8.0',
-        'freezegun>=1.1.0',
-        'certomancer~=0.5.0'
+        'pytest>=6.1.1', 'requests-mock>=1.8.0',
+        'freezegun>=1.1.0', 'certomancer~=0.6.0',
+        'aiohttp>=3.7.4', 'pytest-aiohttp~=0.3.0'
     ],
     keywords="signature pdf pades digital-signature pkcs11"
 )
```

