# Comparing `tmp/vents-0.0.3.tar.gz` & `tmp/vents-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.0.3.tar", last modified: Fri Apr 28 16:46:01 2023, max compression
+gzip compressed data, was "vents-0.0.4.tar", last modified: Sat Apr 29 18:37:37 2023, max compression
```

## Comparing `vents-0.0.3.tar` & `vents-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.921504 vents-0.0.3/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-28 16:45:21.000000 vents-0.0.3/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-28 16:46:01.921591 vents-0.0.3/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-28 16:46:01.922020 vents-0.0.3/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-28 16:45:21.000000 vents-0.0.3/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.917069 vents-0.0.3/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:45:21.000000 vents-0.0.3/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     5330 2023-04-28 16:45:21.000000 vents-0.0.3/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.918472 vents-0.0.3/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-28 16:45:21.000000 vents-0.0.3/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2100 2023-04-28 16:45:21.000000 vents-0.0.3/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-28 16:45:21.000000 vents-0.0.3/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-28 16:45:21.000000 vents-0.0.3/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-28 16:45:21.000000 vents-0.0.3/vents/connections/k8s_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-28 16:45:21.000000 vents-0.0.3/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.919744 vents-0.0.3/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-28 16:45:21.000000 vents-0.0.3/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-28 16:45:21.000000 vents-0.0.3/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.920150 vents-0.0.3/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.920566 vents-0.0.3/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.920982 vents-0.0.3/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1652 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.921372 vents-0.0.3/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-28 16:45:21.000000 vents-0.0.3/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-28 16:45:21.000000 vents-0.0.3/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-28 16:45:21.000000 vents-0.0.3/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-28 16:46:01.917762 vents-0.0.3/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-28 16:46:01.000000 vents-0.0.3/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1118 2023-04-28 16:46:01.000000 vents-0.0.3/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-28 16:46:01.000000 vents-0.0.3/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-28 16:46:01.000000 vents-0.0.3/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-28 16:46:01.000000 vents-0.0.3/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.965695 vents-0.0.4/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-04-29 18:34:33.000000 vents-0.0.4/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-29 18:37:37.965761 vents-0.0.4/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-04-29 18:37:37.966200 vents-0.0.4/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-04-29 18:34:33.000000 vents-0.0.4/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.961222 vents-0.0.4/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     5330 2023-04-29 18:34:33.000000 vents-0.0.4/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.962510 vents-0.0.4/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      321 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2100 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2888 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)      438 2023-04-29 18:34:33.000000 vents-0.0.4/vents/connections/k8s_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-04-29 18:34:33.000000 vents-0.0.4/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.963643 vents-0.0.4/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-04-29 18:34:33.000000 vents-0.0.4/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-04-29 18:34:33.000000 vents-0.0.4/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.964002 vents-0.0.4/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.964472 vents-0.0.4/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1520 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.965003 vents-0.0.4/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.965578 vents-0.0.4/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-04-29 18:34:33.000000 vents-0.0.4/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-04-29 18:34:33.000000 vents-0.0.4/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-04-29 18:34:33.000000 vents-0.0.4/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-04-29 18:37:37.961866 vents-0.0.4/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1209 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       66 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-04-29 18:37:37.000000 vents-0.0.4/vents.egg-info/top_level.txt
```

### Comparing `vents-0.0.3/PKG-INFO` & `vents-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.3
+Version: 0.0.4
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.3/setup.cfg` & `vents-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/setup.py` & `vents-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/config.py` & `vents-0.0.4/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/connections/catalog.py` & `vents-0.0.4/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/connections/connection.py` & `vents-0.0.4/vents/connections/connection.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/connections/connection_schema.py` & `vents-0.0.4/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/__init__.py` & `vents-0.0.4/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/base.py` & `vents-0.0.4/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/discord_webhook.py` & `vents-0.0.4/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/hipchat_webhook.py` & `vents-0.0.4/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/mattermost_webhook.py` & `vents-0.0.4/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/pagerduty_webhook.py` & `vents-0.0.4/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/slack_webhook.py` & `vents-0.0.4/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/notifiers/webhook.py` & `vents-0.0.4/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/aws/base.py` & `vents-0.0.4/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/aws/service.py` & `vents-0.0.4/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/azure/base.py` & `vents-0.0.4/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/azure/service.py` & `vents-0.0.4/vents/providers/azure/service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import os
 
 from typing import TYPE_CHECKING, Optional
 
 from vents.providers.azure.base import (
     get_account_key,
     get_account_name,
+    get_client_id,
+    get_client_secret,
     get_connection_string,
+    get_sas_token,
+    get_tenant_id,
 )
 from vents.providers.base import BaseService
 
 if TYPE_CHECKING:
     from vents.connections.connection import Connection
 
 
 class AzureService(BaseService):
     account_name: Optional[str]
     account_key: Optional[str]
     connection_string: Optional[str]
+    sas_token: Optional[str]
+    tenant_id: Optional[str]
+    client_id: Optional[str]
+    client_secret: Optional[str]
 
     @classmethod
     def load_from_connection(
         cls, connection: Optional["Connection"]
     ) -> Optional["AzureService"]:
         # Check if there are mounting based on secrets/configmaps
         context_paths = []
@@ -28,18 +36,26 @@
             if connection.secret and connection.secret.mount_path:
                 context_paths.append(connection.secret.mount_path)
             if connection.config_map and connection.config_map.mount_path:
                 context_paths.append(connection.config_map.mount_path)
         account_name = get_account_name(context_paths=context_paths)
         account_key = get_account_key(context_paths=context_paths)
         connection_string = get_connection_string(context_paths=context_paths)
+        sas_token = get_sas_token(context_paths=context_paths)
+        tenant_id = get_tenant_id(context_paths=context_paths)
+        client_id = get_client_id(context_paths=context_paths)
+        client_secret = get_client_secret(context_paths=context_paths)
         return cls(
             account_name=account_name,
             account_key=account_key,
             connection_string=connection_string,
+            sas_token=sas_token,
+            tenant_id=tenant_id,
+            client_id=client_id,
+            client_secre=client_secret,
         )
 
     def set_env_vars(self):
         if self._account_name:
             os.environ["AZURE_ACCOUNT_NAME"] = self._account_name
         if self._account_key:
             os.environ["AZURE_ACCOUNT_KEY"] = self._account_key
```

### Comparing `vents-0.0.3/vents/providers/base.py` & `vents-0.0.4/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/gcp/base.py` & `vents-0.0.4/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/gcp/service.py` & `vents-0.0.4/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents/providers/kinds.py` & `vents-0.0.4/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.0.3/vents.egg-info/PKG-INFO` & `vents-0.0.4/vents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.0.3
+Version: 0.0.4
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.0.3/vents.egg-info/SOURCES.txt` & `vents-0.0.4/vents.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 vents/notifiers/spec.py
 vents/notifiers/webhook.py
 vents/providers/__init__.py
 vents/providers/base.py
 vents/providers/kinds.py
 vents/providers/aws/__init__.py
 vents/providers/aws/base.py
+vents/providers/aws/s3.py
 vents/providers/aws/service.py
 vents/providers/azure/__init__.py
 vents/providers/azure/base.py
+vents/providers/azure/blob_storage.py
 vents/providers/azure/service.py
 vents/providers/gcp/__init__.py
 vents/providers/gcp/base.py
+vents/providers/gcp/gcs.py
 vents/providers/gcp/service.py
```

