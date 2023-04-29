# Comparing `tmp/covalent-cloud-0.1.0.tar.gz` & `tmp/covalent-cloud-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-cloud-0.1.0.tar", last modified: Thu Mar  9 20:03:44 2023, max compression
+gzip compressed data, was "covalent-cloud-0.8.0rc0.tar", last modified: Sat Apr 29 00:10:27 2023, max compression
```

## Comparing `covalent-cloud-0.1.0.tar` & `covalent-cloud-0.8.0rc0.tar`

### file list

```diff
@@ -1,12 +1,76 @@
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-03-09 20:03:44.785966 covalent-cloud-0.1.0/
--rw-r--r--   0 will      (1000) will      (1000)      303 2023-03-09 20:03:44.785966 covalent-cloud-0.1.0/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)       12 2023-03-09 20:01:04.000000 covalent-cloud-0.1.0/README.md
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-03-09 20:03:44.785966 covalent-cloud-0.1.0/covalent_cloud/
--rw-r--r--   0 will      (1000) will      (1000)        0 2023-03-09 20:01:04.000000 covalent-cloud-0.1.0/covalent_cloud/__init__.py
-drwxr-sr-x   0 will      (1000) will      (1000)        0 2023-03-09 20:03:44.785966 covalent-cloud-0.1.0/covalent_cloud.egg-info/
--rw-r--r--   0 will      (1000) will      (1000)      303 2023-03-09 20:03:44.000000 covalent-cloud-0.1.0/covalent_cloud.egg-info/PKG-INFO
--rw-r--r--   0 will      (1000) will      (1000)      207 2023-03-09 20:03:44.000000 covalent-cloud-0.1.0/covalent_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 will      (1000) will      (1000)        1 2023-03-09 20:03:44.000000 covalent-cloud-0.1.0/covalent_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 will      (1000) will      (1000)       15 2023-03-09 20:03:44.000000 covalent-cloud-0.1.0/covalent_cloud.egg-info/top_level.txt
--rw-r--r--   0 will      (1000) will      (1000)       79 2023-03-09 20:03:44.785966 covalent-cloud-0.1.0/setup.cfg
--rw-r--r--   0 will      (1000) will      (1000)      367 2023-03-09 20:03:35.000000 covalent-cloud-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/_serialize/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/analytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/cloud_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/cloud_executor/models/sw_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/interface_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/dispatch_management/results_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/auth_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/service_account_interface/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/classes/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/electron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/shared/schemas/transport_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/software_environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/covalent_cloud/swe_management/swe_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 00:10:27.000000 covalent-cloud-0.8.0rc0/covalent_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-29 00:10:27.444949 covalent-cloud-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.436949 covalent-cloud-0.8.0rc0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/future_classes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/dispatch_management_tests/interface_functions_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/shared/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/APIClient_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/shared/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:10:27.440949 covalent-cloud-0.8.0rc0/tests/swe_management_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-04-29 00:10:17.000000 covalent-cloud-0.8.0rc0/tests/swe_management_tests/swe_manager_test.py
```

