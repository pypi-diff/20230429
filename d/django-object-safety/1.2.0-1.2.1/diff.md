# Comparing `tmp/django_object_safety-1.2.0.tar.gz` & `tmp/django_object_safety-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-1.2.0.tar", max compression
+gzip compressed data, was "django_object_safety-1.2.1.tar", max compression
```

## Comparing `django_object_safety-1.2.0.tar` & `django_object_safety-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/LICENSE
--rw-r--r--   0        0        0      129 2023-04-29 12:31:10.608042 django_object_safety-1.2.0/README.md
--rw-r--r--   0        0        0      697 2023-04-29 13:01:18.601803 django_object_safety-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.2.0/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/models.py
--rw-r--r--   0        0        0    18617 2023-04-29 13:01:18.601803 django_object_safety-1.2.0/safety/shortcuts.py
--rw-r--r--   0        0        0     9846 2023-04-28 21:32:07.033636 django_object_safety-1.2.0/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/views.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 13:08:10.717419 django_object_safety-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.2.1/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.1/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.2.1/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.2.1/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.2.1/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/models.py
+-rw-r--r--   0        0        0    18629 2023-04-29 13:08:10.717419 django_object_safety-1.2.1/safety/shortcuts.py
+-rw-r--r--   0        0        0     9846 2023-04-29 13:05:50.477556 django_object_safety-1.2.1/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.1/safety/views.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.2.1/PKG-INFO
```

### Comparing `django_object_safety-1.2.0/LICENSE` & `django_object_safety-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/pyproject.toml` & `django_object_safety-1.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "1.2.0"
+version = "1.2.1"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/en/latest/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
```

### Comparing `django_object_safety-1.2.0/safety/migrations/0001_initial.py` & `django_object_safety-1.2.1/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-1.2.1/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-1.2.1/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-1.2.1/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-1.2.1/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/safety/models.py` & `django_object_safety-1.2.1/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/safety/shortcuts.py` & `django_object_safety-1.2.1/safety/shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,27 +154,27 @@
         content_type (ContentType): The ContentType of the object.
     """
 
     if obj is None:
         if content_type is None:
             raise ValueError("Content type must be provided if obj is None.")
 
-        permission = Permission.objects.get_or_create(codename=perm, content_type=content_type)
+        permission = Permission.objects.get_or_create(codename=perm, content_type=content_type)[0]
 
         if isinstance(entity, get_user_model()):
             entity.user_permissions.add(
                 permission
             )
         elif isinstance(entity, Group):
             entity.permissions.add(
                 permission
             )
         return True
 
-    permission = Permission.objects.get_or_create(codename=perm, content_type=ContentType.objects.get_for_model(obj))
+    permission = Permission.objects.get_or_create(codename=perm, content_type=ContentType.objects.get_for_model(obj))[0]
 
     if isinstance(entity, get_user_model()):
         get_object_permission_model(obj).objects.get_or_create(permission=permission, to_id=entity.id,
                                                                to_ct=ContentType.objects.get_for_model(entity),
                                                                object_id=obj.id,
                                                                object_ct=ContentType.objects.get_for_model(obj))
         return True
@@ -429,15 +429,15 @@
         Group: The group object.
     """
 
     perm_group = get_object_group_model().objects.create(name=name, target_id=obj.id,
                                                          target_ct=ContentType.objects.get_for_model(obj))
 
     for permission in permissions:
-        perm_group.permissions.add(Permission.objects.get_or_create(codename=permission))
+        perm_group.permissions.add(Permission.objects.get_or_create(codename=permission)[0].id)
 
     return perm_group
 
 
 def delete_object_group(name: str, obj) -> bool:
     """
     Remove an object group.
```

### Comparing `django_object_safety-1.2.0/safety/tests.py` & `django_object_safety-1.2.1/safety/tests.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.2.0/PKG-INFO` & `django_object_safety-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 1.2.0
+Version: 1.2.1
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/en/latest/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >3.5
 Classifier: License :: OSI Approved :: MIT License
```

