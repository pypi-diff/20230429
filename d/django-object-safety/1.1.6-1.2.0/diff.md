# Comparing `tmp/django_object_safety-1.1.6.tar.gz` & `tmp/django_object_safety-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_object_safety-1.1.6.tar", max compression
+gzip compressed data, was "django_object_safety-1.2.0.tar", max compression
```

## Comparing `django_object_safety-1.1.6.tar` & `django_object_safety-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/LICENSE
--rw-r--r--   0        0        0      129 2023-04-29 12:31:10.608042 django_object_safety-1.1.6/README.md
--rw-r--r--   0        0        0      697 2023-04-29 12:33:46.543786 django_object_safety-1.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.1.6/safety/__init__.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.6/safety/admin.py
--rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.1.6/safety/apps.py
--rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0001_initial.py
--rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
--rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0003_alter_objectpermission_options.py
--rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
--rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
--rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0006_alter_objectpermission_options.py
--rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0007_alter_objectpermission_options.py
--rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/migrations/0008_rename_permissiongroup_objectgroup.py
--rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.1.6/safety/migrations/__init__.py
--rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-1.1.6/safety/models.py
--rw-r--r--   0        0        0    18010 2023-04-29 12:33:46.543786 django_object_safety-1.1.6/safety/shortcuts.py
--rw-r--r--   0        0        0     9846 2023-04-28 21:32:07.033636 django_object_safety-1.1.6/safety/tests.py
--rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.1.6/safety/views.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/LICENSE
+-rw-r--r--   0        0        0      129 2023-04-29 12:31:10.608042 django_object_safety-1.2.0/README.md
+-rw-r--r--   0        0        0      697 2023-04-29 13:01:18.601803 django_object_safety-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/admin.py
+-rw-r--r--   0        0        0      144 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/apps.py
+-rw-r--r--   0        0        0     1705 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0001_initial.py
+-rw-r--r--   0        0        0      949 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py
+-rw-r--r--   0        0        0      445 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0003_alter_objectpermission_options.py
+-rw-r--r--   0        0        0     2656 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py
+-rw-r--r--   0        0        0      744 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py
+-rw-r--r--   0        0        0      444 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0006_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      434 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0007_alter_objectpermission_options.py
+-rw-r--r--   0        0        0      571 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:30:41.012284 django_object_safety-1.2.0/safety/migrations/__init__.py
+-rw-r--r--   0        0        0     2461 2023-04-22 17:57:27.834494 django_object_safety-1.2.0/safety/models.py
+-rw-r--r--   0        0        0    18617 2023-04-29 13:01:18.601803 django_object_safety-1.2.0/safety/shortcuts.py
+-rw-r--r--   0        0        0     9846 2023-04-28 21:32:07.033636 django_object_safety-1.2.0/safety/tests.py
+-rw-r--r--   0        0        0       63 2023-04-16 18:28:46.023260 django_object_safety-1.2.0/safety/views.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 django_object_safety-1.2.0/PKG-INFO
```

### Comparing `django_object_safety-1.1.6/LICENSE` & `django_object_safety-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/pyproject.toml` & `django_object_safety-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-object-safety"
-version = "1.1.6"
+version = "1.2.0"
 description = "Adds object permissions to Django."
 license = "MIT"
 authors = ["William Ferreira"]
 homepage = "https://django-object-safety-docs.readthedocs.io/en/latest/"
 repository = "https://github.com/williammferreira/django-object-safety/"
 keywords = ["django", "permissions", "object-permissions", "django-permissions", "django-object-permissions"]
 readme = "README.md"
```

### Comparing `django_object_safety-1.1.6/safety/migrations/0001_initial.py` & `django_object_safety-1.2.0/safety/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py` & `django_object_safety-1.2.0/safety/migrations/0002_alter_objectpermission_object_ct_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py` & `django_object_safety-1.2.0/safety/migrations/0004_alter_objectpermission_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py` & `django_object_safety-1.2.0/safety/migrations/0005_alter_permissiongroup_target_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/safety/migrations/0008_rename_permissiongroup_objectgroup.py` & `django_object_safety-1.2.0/safety/migrations/0008_rename_permissiongroup_objectgroup.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/safety/models.py` & `django_object_safety-1.2.0/safety/models.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/safety/shortcuts.py` & `django_object_safety-1.2.0/safety/shortcuts.py`

 * *Files 5% similar despite different names*

```diff
@@ -360,34 +360,47 @@
                                                                   object_id=obj.id,
                                                                   to_ct=ContentType.objects.get_for_model(Group),
                                                                   ).distinct()
 
     return [perm.to for perm in permissions]
 
 
-def get_objects_for_entity(entity: get_user_model() | Group, permissions: list[str] | str, ct: ContentType) -> \
+def get_objects_for_entity(entity: get_user_model() | Group, permissions: list[str] | str, ct: ContentType,
+                           with_group_users=True) -> \
         list[any]:
     """
     Get all objects that the user has the specified permissions on.
     Args:
         entity: The user that has access to the objects.
         permissions (list[str]): The permissions required.
         ct (ContentType): The content type of the objects.
+        with_group_users (bool): Include users in groups that have the permission in the result.
     """
 
+    assert not (with_group_users is True and isinstance(entity, Group)), \
+        "Entity must be a user if with_group_users is set."
+
     if not isinstance(permissions, list):
         permissions = [permissions]
 
     perms = get_object_permission_model().objects.filter(
         to_ct=ContentType.objects.get_for_model(entity),
         to_id=entity.id,
         permission__codename__in=permissions,
         permission__content_type=ct,
     )
 
+    if with_group_users:
+        perms = perms | get_object_permission_model().objects.filter(
+            to_ct=ContentType.objects.get_for_model(Group),
+            to_id__in=[group.id for group in entity.groups.all()],
+            permission__codename__in=permissions,
+            permission__content_type=ct,
+        )
+
     return [perm.object for perm in perms]
 
 
 def retrieve_object_group(name: str, obj) -> ObjectGroup:
     """
     Get an object group.
```

### Comparing `django_object_safety-1.1.6/safety/tests.py` & `django_object_safety-1.2.0/safety/tests.py`

 * *Files identical despite different names*

### Comparing `django_object_safety-1.1.6/PKG-INFO` & `django_object_safety-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-object-safety
-Version: 1.1.6
+Version: 1.2.0
 Summary: Adds object permissions to Django.
 Home-page: https://django-object-safety-docs.readthedocs.io/en/latest/
 License: MIT
 Keywords: django,permissions,object-permissions,django-permissions,django-object-permissions
 Author: William Ferreira
 Requires-Python: >3.5
 Classifier: License :: OSI Approved :: MIT License
```

