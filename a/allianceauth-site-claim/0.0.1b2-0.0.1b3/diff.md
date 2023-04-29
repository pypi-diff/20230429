# Comparing `tmp/allianceauth-site-claim-0.0.1b2.tar.gz` & `tmp/allianceauth-site-claim-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-site-claim-0.0.1b2.tar", last modified: Sat Apr 29 03:20:49 2023, max compression
+gzip compressed data, was "allianceauth-site-claim-0.0.1b3.tar", last modified: Sat Apr 29 03:39:01 2023, max compression
```

## Comparing `allianceauth-site-claim-0.0.1b2.tar` & `allianceauth-site-claim-0.0.1b3.tar`

### file list

```diff
@@ -1,30 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:20:49.870299 allianceauth-site-claim-0.0.1b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-29 03:20:49.870299 allianceauth-site-claim-0.0.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:20:49.870299 allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-29 03:20:49.000000 allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-29 03:20:49.000000 allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:20:49.000000 allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-29 03:20:49.000000 allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 03:20:49.000000 allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:20:49.870299 allianceauth-site-claim-0.0.1b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:20:49.870299 allianceauth-site-claim-0.0.1b2/siteclaim/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:20:49.870299 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0002_rename_catconfiguration_siteclaimconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0003_siteclaimconfiguration_valid_site_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0004_site.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0005_siteclaimconfiguration_site_claim_output_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0006_siteclaimconfiguration_ess_output_channel_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 03:20:18.000000 allianceauth-site-claim-0.0.1b2/siteclaim/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.590398 allianceauth-site-claim-0.0.1b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-29 03:39:01.590398 allianceauth-site-claim-0.0.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.586398 allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-29 03:39:01.000000 allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-29 03:39:01.000000 allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:39:01.000000 allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-29 03:39:01.000000 allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 03:39:01.000000 allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:39:01.590398 allianceauth-site-claim-0.0.1b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.586398 allianceauth-site-claim-0.0.1b3/siteclaim/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.586398 allianceauth-site-claim-0.0.1b3/siteclaim/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-29 03:38:31.000000 allianceauth-site-claim-0.0.1b3/siteclaim/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.590398 allianceauth-site-claim-0.0.1b3/siteclaim/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/cogs/ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/cogs/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.586398 allianceauth-site-claim-0.0.1b3/siteclaim/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.590398 allianceauth-site-claim-0.0.1b3/siteclaim/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/management/commands/__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/management/commands/sc_setup_sde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:39:01.590398 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0002_rename_catconfiguration_siteclaimconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0003_siteclaimconfiguration_valid_site_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0004_site.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0005_siteclaimconfiguration_site_claim_output_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0006_siteclaimconfiguration_ess_output_channel_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-29 03:38:21.000000 allianceauth-site-claim-0.0.1b3/siteclaim/tasks.py
```

### Comparing `allianceauth-site-claim-0.0.1b2/LICENCE` & `allianceauth-site-claim-0.0.1b3/LICENCE`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/PKG-INFO` & `allianceauth-site-claim-0.0.1b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-site-claim
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/Solar-Helix-Independent-Transport/allianceauth-site-claim
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-site-claim-0.0.1b2/README.md` & `allianceauth-site-claim-0.0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/PKG-INFO` & `allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-site-claim
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/Solar-Helix-Independent-Transport/allianceauth-site-claim
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-site-claim-0.0.1b2/allianceauth_site_claim.egg-info/SOURCES.txt` & `allianceauth-site-claim-0.0.1b3/allianceauth_site_claim.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 siteclaim/admin.py
 siteclaim/app_settings.py
 siteclaim/apps.py
 siteclaim/auth_hooks.py
 siteclaim/models.py
 siteclaim/providers.py
 siteclaim/tasks.py
+siteclaim/__pycache__/__init__.cpython-39.pyc
+siteclaim/cogs/ess.py
+siteclaim/cogs/sites.py
+siteclaim/management/commands/__init.py
+siteclaim/management/commands/sc_setup_sde.py
 siteclaim/migrations/0001_initial.py
 siteclaim/migrations/0002_rename_catconfiguration_siteclaimconfiguration.py
 siteclaim/migrations/0003_siteclaimconfiguration_valid_site_regions.py
 siteclaim/migrations/0004_site.py
 siteclaim/migrations/0005_siteclaimconfiguration_site_claim_output_channel.py
 siteclaim/migrations/0006_siteclaimconfiguration_ess_output_channel_and_more.py
 siteclaim/migrations/__init__.py
```

### Comparing `allianceauth-site-claim-0.0.1b2/setup.py` & `allianceauth-site-claim-0.0.1b3/setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0001_initial.py` & `allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0004_site.py` & `allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0004_site.py`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/siteclaim/migrations/0006_siteclaimconfiguration_ess_output_channel_and_more.py` & `allianceauth-site-claim-0.0.1b3/siteclaim/migrations/0006_siteclaimconfiguration_ess_output_channel_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/siteclaim/models.py` & `allianceauth-site-claim-0.0.1b3/siteclaim/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-site-claim-0.0.1b2/siteclaim/providers.py` & `allianceauth-site-claim-0.0.1b3/siteclaim/providers.py`

 * *Files identical despite different names*

