# Comparing `tmp/bam-core-2023.4.28.1682737714.tar.gz` & `tmp/bam-core-2023.4.29.1682775214.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bam-core-2023.4.28.1682737714.tar", last modified: Sat Apr 29 03:11:08 2023, max compression
+gzip compressed data, was "bam-core-2023.4.29.1682775214.tar", last modified: Sat Apr 29 13:33:36 2023, max compression
```

## Comparing `bam-core-2023.4.28.1682737714.tar` & `bam-core-2023.4.29.1682775214.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 03:11:08.248388 bam-core-2023.4.28.1682737714/
--rw-r--r--   0 music      (501) staff       (20)       42 2023-04-29 03:10:09.000000 bam-core-2023.4.28.1682737714/MANIFEST.in
--rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 03:11:08.247878 bam-core-2023.4.28.1682737714/PKG-INFO
--rw-r--r--   0 music      (501) staff       (20)       62 2023-04-29 02:17:40.000000 bam-core-2023.4.28.1682737714/README.md
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 03:11:08.240773 bam-core-2023.4.28.1682737714/bam_core/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:38:01.000000 bam-core-2023.4.28.1682737714/bam_core/__init__.py
--rw-r--r--   0 music      (501) staff       (20)       32 2023-04-29 03:08:34.000000 bam-core-2023.4.28.1682737714/bam_core/__version__.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 03:11:08.244678 bam-core-2023.4.28.1682737714/bam_core/lib/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:39:14.000000 bam-core-2023.4.28.1682737714/bam_core/lib/__init__.py
--rw-r--r--   0 music      (501) staff       (20)     2346 2023-04-28 21:46:59.000000 bam-core-2023.4.28.1682737714/bam_core/lib/airtable.py
--rw-r--r--   0 music      (501) staff       (20)     6410 2023-04-29 02:40:34.000000 bam-core-2023.4.28.1682737714/bam_core/lib/listmonk.py
--rw-r--r--   0 music      (501) staff       (20)    14789 2023-04-28 21:39:14.000000 bam-core-2023.4.28.1682737714/bam_core/lib/s3.py
--rw-r--r--   0 music      (501) staff       (20)     2342 2023-04-29 02:54:27.000000 bam-core-2023.4.28.1682737714/bam_core/settings.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 03:11:08.246231 bam-core-2023.4.28.1682737714/bam_core/utils/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.28.1682737714/bam_core/utils/__init__.py
--rw-r--r--   0 music      (501) staff       (20)      913 2023-04-28 21:41:46.000000 bam-core-2023.4.28.1682737714/bam_core/utils/etc.py
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-28 21:41:46.000000 bam-core-2023.4.28.1682737714/bam_core/utils/phone.py
--rw-r--r--   0 music      (501) staff       (20)     6007 2023-04-29 02:21:08.000000 bam-core-2023.4.28.1682737714/bam_core/utils/serde.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 03:11:08.242765 bam-core-2023.4.28.1682737714/bam_core.egg-info/
--rw-r--r--   0 music      (501) staff       (20)      203 2023-04-29 03:11:08.000000 bam-core-2023.4.28.1682737714/bam_core.egg-info/PKG-INFO
--rw-r--r--   0 music      (501) staff       (20)      501 2023-04-29 03:11:08.000000 bam-core-2023.4.28.1682737714/bam_core.egg-info/SOURCES.txt
--rw-r--r--   0 music      (501) staff       (20)        1 2023-04-29 03:11:08.000000 bam-core-2023.4.28.1682737714/bam_core.egg-info/dependency_links.txt
--rw-r--r--   0 music      (501) staff       (20)       46 2023-04-29 03:11:08.000000 bam-core-2023.4.28.1682737714/bam_core.egg-info/requires.txt
--rw-r--r--   0 music      (501) staff       (20)       15 2023-04-29 03:11:08.000000 bam-core-2023.4.28.1682737714/bam_core.egg-info/top_level.txt
--rw-r--r--   0 music      (501) staff       (20)       46 2023-04-28 21:54:19.000000 bam-core-2023.4.28.1682737714/requirements.txt
--rw-r--r--   0 music      (501) staff       (20)       38 2023-04-29 03:11:08.248522 bam-core-2023.4.28.1682737714/setup.cfg
--rw-r--r--   0 music      (501) staff       (20)      598 2023-04-29 02:48:20.000000 bam-core-2023.4.28.1682737714/setup.py
-drwxr-xr-x   0 music      (501) staff       (20)        0 2023-04-29 03:11:08.247336 bam-core-2023.4.28.1682737714/tests/
--rw-r--r--   0 music      (501) staff       (20)        0 2023-04-29 02:31:15.000000 bam-core-2023.4.28.1682737714/tests/__init__.py
--rw-r--r--   0 music      (501) staff       (20)      200 2023-04-29 02:38:14.000000 bam-core-2023.4.28.1682737714/tests/test_serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.457665 bam-core-2023.4.29.1682775214/bam_core/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-29 13:33:34.000000 bam-core-2023.4.29.1682775214/bam_core/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/bam_core/lib/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2346 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/airtable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6410 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/listmonk.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14789 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/lib/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1961 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/bam_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      913 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/etc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/phone.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6007 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/bam_core/utils/serde.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/bam_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      472 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-29 13:33:36.000000 bam-core-2023.4.29.1682775214/bam_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:36.461665 bam-core-2023.4.29.1682775214/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      200 2023-04-29 13:33:11.000000 bam-core-2023.4.29.1682775214/tests/test_serde.py
```

### Comparing `bam-core-2023.4.28.1682737714/bam_core/lib/airtable.py` & `bam-core-2023.4.29.1682775214/bam_core/lib/airtable.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.28.1682737714/bam_core/lib/listmonk.py` & `bam-core-2023.4.29.1682775214/bam_core/lib/listmonk.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.28.1682737714/bam_core/lib/s3.py` & `bam-core-2023.4.29.1682775214/bam_core/lib/s3.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.28.1682737714/bam_core/settings.py` & `bam-core-2023.4.29.1682775214/bam_core/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,37 +2,23 @@
 import dotenv
 import logging
 import logging.config
 
 # load .env file
 dotenv.load_dotenv()
 
-# DEFAULT SETTINGS
-
-API_VERSION = "v1"
-API_KEY_HEADER = "X-BAM-API-KEY"
-API_KEY_PARAM = "api_key"
-
-# api spec
-APISPEC_SWAGGER_URL = os.getenv("BAM_APISPEC_SWAGGER_URL", "/spec/")
-APISPEC_SWAGGER_UI_URL = os.getenv("BAM_APISPEC_SWAGGER_UI_URL", "/docs/")
-
-# bam settings
 AIRTABLE_TOKEN = os.getenv("BAM_AIRTABLE_TOKEN", None)
 AIRTABLE_BASE_ID = os.getenv("BAM_AIRTABLE_BASE_ID", None)
 AIRTABLE_ASSISTANCE_REQUESTS_TABLE_NAME = os.getenv(
     "BAM_AIRTABLE_ASSISTANCE_REQUESTS_TABLE_NAME", "Assistance Requests: Main"
 )
 AIRTABLE_MESH_VIEW_NAME = os.getenv(
     "BAM_AIRTABLE_MESH_VIEW_NAME", "MESH - Pending installs, by address (Lu)"
 )
 
-# flask settings
-SECRET_KEY = os.getenv("BAM_SESSION_SECRET_KEY", "secret")
-
 # logging settings
 LOG_LEVEL = os.getenv("BAM_LOG_LEVEL", "INFO")
 LOG_FORMAT = os.getenv(
     "BAM_LOG_FORMAT",
     r"<%(levelname)s> %(module)s:%(lineno)d -> %(message)s [%(asctime)s]",
 )
 
@@ -70,10 +56,10 @@
     "BAM_S3_ENDPOINT_URL", "https://nyc3.digitaloceanspaces.com"
 )
 S3_ACCESS_KEY_ID = os.getenv("BAM_S3_ACCESS_KEY_ID", None)
 S3_SECRET_ACCESS_KEY = os.getenv("BAM_S3_SECRET_ACCESS_KEY", None)
 S3_BUCKET = os.getenv("BAM_S3_BUCKET", "bam-file")
 S3_REGION_NAME = os.getenv("BAM_S3_REGION_NAME", "nyc3")
 S3_PLATFORM = os.getenv("BAM_S3_PLATFORM", "do")
-S3_CDN_ID = os.getenv("BAM_S3_CDN_ID", "4d57a938-0336-4bda-a27f-929125be460b")
+S3_CDN_ID = os.getenv("BAM_S3_CDN_ID", None)
 
 logging.config.dictConfig(LOGGING_CONFIG)
```

### Comparing `bam-core-2023.4.28.1682737714/bam_core/utils/etc.py` & `bam-core-2023.4.29.1682775214/bam_core/utils/etc.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.28.1682737714/bam_core/utils/serde.py` & `bam-core-2023.4.29.1682775214/bam_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `bam-core-2023.4.28.1682737714/setup.py` & `bam-core-2023.4.29.1682775214/setup.py`

 * *Files identical despite different names*

