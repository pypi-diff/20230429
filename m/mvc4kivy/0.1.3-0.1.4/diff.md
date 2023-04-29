# Comparing `tmp/mvc4kivy-0.1.3.tar.gz` & `tmp/mvc4kivy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvc4kivy-0.1.3.tar", max compression
+gzip compressed data, was "mvc4kivy-0.1.4.tar", max compression
```

## Comparing `mvc4kivy-0.1.3.tar` & `mvc4kivy-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.3/mvc4kivy/__init__.py
--rw-r--r--   0        0        0     7029 2023-04-29 09:29:50.333179 mvc4kivy-0.1.3/mvc4kivy/add_view.py
--rw-r--r--   0        0        0    42621 2023-04-29 13:10:36.831031 mvc4kivy-0.1.3/mvc4kivy/create_project.py
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.3/mvc4kivy/MVC/__init__.py
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.3/mvc4kivy/MVC/data/locales/po/en.po
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.3/mvc4kivy/MVC/data/locales/po/ru.po
--rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.3/mvc4kivy/MVC/libs/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.3/mvc4kivy/MVC/libs/translation.py
--rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.3/mvc4kivy/MVC/messages.pot
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.3/mvc4kivy/MVC/Model/__init__.py
--rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.3/mvc4kivy/MVC/Model/database_firebase.py
--rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.3/mvc4kivy/MVC/Model/database_restdb.py
--rw-r--r--   0        0        0      453 2023-04-29 13:21:22.223897 mvc4kivy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.3/README.md
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 mvc4kivy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.4/mvc4kivy/__init__.py
+-rw-r--r--   0        0        0     7029 2023-04-29 09:29:50.333179 mvc4kivy-0.1.4/mvc4kivy/add_view.py
+-rw-r--r--   0        0        0    42630 2023-04-29 13:30:02.668298 mvc4kivy-0.1.4/mvc4kivy/create_project.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.4/mvc4kivy/MVC/__init__.py
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.4/mvc4kivy/MVC/data/locales/po/en.po
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.4/mvc4kivy/MVC/data/locales/po/ru.po
+-rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.4/mvc4kivy/MVC/libs/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.4/mvc4kivy/MVC/libs/translation.py
+-rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.4/mvc4kivy/MVC/messages.pot
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.4/mvc4kivy/MVC/Model/__init__.py
+-rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.4/mvc4kivy/MVC/Model/database_firebase.py
+-rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.4/mvc4kivy/MVC/Model/database_restdb.py
+-rw-r--r--   0        0        0      453 2023-04-29 13:31:34.309342 mvc4kivy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.4/README.md
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 mvc4kivy-0.1.4/PKG-INFO
```

### Comparing `mvc4kivy-0.1.3/mvc4kivy/__init__.py` & `mvc4kivy-0.1.4/mvc4kivy/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/mvc4kivy/add_view.py` & `mvc4kivy-0.1.4/mvc4kivy/add_view.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/mvc4kivy/create_project.py` & `mvc4kivy-0.1.4/mvc4kivy/create_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1054,15 +1054,15 @@
         init_module.write("")
     with open(f"{view_module}.py", "w", encoding="utf-8") as view_file:
         view_file.write(
             temp_code_view.format(name_screen=name_screen)
             if name_screen not in use_responsive
             else temp_code_responsive_view.format(
                 name_screen=name_screen,
-                parenthesis="()" if instantiate_responsive_view else ""
+                parenthesis="()" if instantiate_responsive_view == "yes" else ""
             )
         )
 
     if name_screen in use_responsive:
         for name_platform in ["Desktop", "Mobile", "Tablet"]:
             path_to_init_components = os.path.join(
                 path_to_project,
```

### Comparing `mvc4kivy-0.1.3/mvc4kivy/MVC/libs/__init__.py` & `mvc4kivy-0.1.4/mvc4kivy/MVC/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/mvc4kivy/MVC/libs/translation.py` & `mvc4kivy-0.1.4/mvc4kivy/MVC/libs/translation.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/mvc4kivy/MVC/messages.pot` & `mvc4kivy-0.1.4/mvc4kivy/MVC/messages.pot`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/mvc4kivy/MVC/Model/database_firebase.py` & `mvc4kivy-0.1.4/mvc4kivy/MVC/Model/database_firebase.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/mvc4kivy/MVC/Model/database_restdb.py` & `mvc4kivy-0.1.4/mvc4kivy/MVC/Model/database_restdb.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.3/PKG-INFO` & `mvc4kivy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvc4kivy
-Version: 0.1.3
+Version: 0.1.4
 Summary: tool to create MVC project for kivy
 Author: Kenechukwu Akubue
 Author-email: kengoon19@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

