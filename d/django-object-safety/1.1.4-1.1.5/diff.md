# Comparing `tmp/django_object_safety-1.1.4.tar.gz` & `tmp/django_object_safety-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-1.1.4.tar", max compression
+gzip compressed data, was "django_object_safety-1.1.5.tar", max compression
```

## Comparing `django_object_safety-1.1.4.tar` & `django_object_safety-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/LICENSE
--rw-r--r--   0        0        0      129 2023-04-28 21:32:04.641638 django_object_safety-1.1.4/README.md
--rw-r--r--   0        0        0      697 2023-04-28 23:48:37.981889 django_object_safety-1.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.1.4/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.4/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.1.4/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.1.4/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-1.1.4/safety/models.py
--rw-r--r--   0        0        0    18141 2023-04-28 21:32:07.033636 django_object_safety-1.1.4/safety/shortcuts.py
--rw-r--r--   0        0        0     9846 2023-04-28 21:32:07.033636 django_object_safety-1.1.4/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.4/safety/views.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-28 21:32:04.641638 django_object_safety-1.1.5/README.md
+-rw-r--r--   0        0        0      697 2023-04-28 23:49:43.269855 django_object_safety-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.1.5/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.5/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.1.5/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.1.5/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-1.1.5/safety/models.py
+-rw-r--r--   0        0        0    18141 2023-04-28 21:32:07.033636 django_object_safety-1.1.5/safety/shortcuts.py
+-rw-r--r--   0        0        0     9846 2023-04-28 21:32:07.033636 django_object_safety-1.1.5/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.5/safety/views.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.1.5/PKG-INFO
```

### Comparing `django_object_safety-1.1.4/LICENSE` & `django_object_safety-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/pyproject.toml` & `django_object_safety-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "1.1.4"
+version = "1.1.5"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/en/latest/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
```

### Comparing `django_object_safety-1.1.4/safety/migrations/0001_initial.py` & `django_object_safety-1.1.5/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-1.1.5/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-1.1.5/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-1.1.5/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-1.1.5/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/models.py` & `django_object_safety-1.1.5/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/shortcuts.py` & `django_object_safety-1.1.5/safety/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/safety/tests.py` & `django_object_safety-1.1.5/safety/tests.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.4/PKG-INFO` & `django_object_safety-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 1.1.4
+Version: 1.1.5
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/en/latest/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >3.5
 Classifier: License :: OSI Approved :: MIT License
```

