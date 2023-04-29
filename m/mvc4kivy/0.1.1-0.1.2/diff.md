# Comparing `tmp/mvc4kivy-0.1.1.tar.gz` & `tmp/mvc4kivy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvc4kivy-0.1.1.tar", max compression
+gzip compressed data, was "mvc4kivy-0.1.2.tar", max compression
```

## Comparing `mvc4kivy-0.1.1.tar` & `mvc4kivy-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.1/mvc4kivy/__init__.py
--rw-r--r--   0        0        0     7029 2023-04-29 09:29:50.333179 mvc4kivy-0.1.1/mvc4kivy/add_view.py
--rw-r--r--   0        0        0    42474 2023-04-29 11:39:38.590717 mvc4kivy-0.1.1/mvc4kivy/create_project.py
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.1/mvc4kivy/MVC/__init__.py
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.1/mvc4kivy/MVC/data/locales/po/en.po
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.1/mvc4kivy/MVC/data/locales/po/ru.po
--rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.1/mvc4kivy/MVC/libs/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.1/mvc4kivy/MVC/libs/translation.py
--rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.1/mvc4kivy/MVC/messages.pot
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.1/mvc4kivy/MVC/Model/__init__.py
--rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_firebase.py
--rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_restdb.py
--rw-r--r--   0        0        0      418 2023-04-29 11:39:59.717568 mvc4kivy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.1/README.md
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 mvc4kivy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.2/mvc4kivy/__init__.py
+-rw-r--r--   0        0        0     7029 2023-04-29 09:29:50.333179 mvc4kivy-0.1.2/mvc4kivy/add_view.py
+-rw-r--r--   0        0        0    42457 2023-04-29 12:10:36.326503 mvc4kivy-0.1.2/mvc4kivy/create_project.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.2/mvc4kivy/MVC/__init__.py
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.2/mvc4kivy/MVC/data/locales/po/en.po
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.2/mvc4kivy/MVC/data/locales/po/ru.po
+-rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.2/mvc4kivy/MVC/libs/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.2/mvc4kivy/MVC/libs/translation.py
+-rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.2/mvc4kivy/MVC/messages.pot
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.2/mvc4kivy/MVC/Model/__init__.py
+-rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.2/mvc4kivy/MVC/Model/database_firebase.py
+-rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.2/mvc4kivy/MVC/Model/database_restdb.py
+-rw-r--r--   0        0        0      418 2023-04-29 12:11:36.196277 mvc4kivy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.2/README.md
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 mvc4kivy-0.1.2/PKG-INFO
```

### Comparing `mvc4kivy-0.1.1/mvc4kivy/__init__.py` & `mvc4kivy-0.1.2/mvc4kivy/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/mvc4kivy/add_view.py` & `mvc4kivy-0.1.2/mvc4kivy/add_view.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/mvc4kivy/create_project.py` & `mvc4kivy-0.1.2/mvc4kivy/create_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,17 +330,17 @@
         """
         Called whenever any change has occurred in the data model.
         The view in this method tracks these changes and updates the UI
         according to these changes.
         """
 '''
 
-temp_responsive_component_imports = """from .platforms.MobileScreen.mobile_screen import MobileScreenView
-from .platforms.TabletScreen.tablet_screen import TabletScreenView
-from .platforms.DesktopScreen.desktop_screen import DesktopScreenView
+temp_responsive_component_imports = """from .platforms.Mobile.mobile_screen import {name_screen}MobileView
+from .platforms.Tablet.tablet_screen import {name_screen}TabletView
+from .platforms.Desktop.desktop_screen import {name_screen}DesktopView
 """
 
 temp_responsive_platform_baseclass = """from kivymd.uix.screen import MDScreen
 
 
 class {}View(MDScreen):
     pass
@@ -1055,15 +1055,15 @@
             else temp_code_responsive_view.format(
                 name_screen=name_screen,
                 parenthesis="()" if instantiate_responsive_view else ""
             )
         )
 
     if name_screen in use_responsive:
-        for name_platform in ["DesktopScreen", "MobileScreen", "TabletScreen"]:
+        for name_platform in ["Desktop", "Mobile", "Tablet"]:
             path_to_init_components = os.path.join(
                 path_to_project,
                 "View",
                 name_screen,
                 "components",
                 "__init__.py",
             )
@@ -1079,36 +1079,34 @@
                 os.path.join(path_to_view, "__init__.py"),
                 path_to_platform_components,
             )
             shutil.copy(
                 os.path.join(path_to_view, "__init__.py"), path_to_platforms
             )
 
-            name_platform_module = (
-                f'{name_platform.split("Screen")[0].lower()}_screen'
-            )
+            name_platform_module = name_platform.lower()
             with open(
                     os.path.join(path_to_platform, f"{name_platform_module}.kv"),
                     "w",
                     encoding="utf-8",
             ) as platform_rule:
-                platform_rule.write(f"<{name_platform}View>\n")
+                platform_rule.write(f"<{name_screen}{name_platform}View>\n")
             with open(
                     os.path.join(path_to_platform, f"{name_platform_module}.py"),
                     "w",
                     encoding="utf-8",
             ) as platform_baseclass:
                 platform_baseclass.write(
-                    temp_responsive_platform_baseclass.format(name_platform)
+                    temp_responsive_platform_baseclass.format(f"{name_screen}{name_platform}")
                 )
 
         with open(
                 path_to_init_components, "w", encoding="utf-8"
         ) as init_components:
-            init_components.write(temp_responsive_component_imports)
+            init_components.write(temp_responsive_component_imports.format(name_screen=name_screen))
 
     with open(f"{view_module}.kv", "w", encoding="utf-8") as view_file:
         view_file.write(f"<{name_screen}View>\n    name: '{module_name.replace('_', ' ')}'")
 
     if name_screen not in use_responsive:
         shutil.copy(
             os.path.join(path_to_view, "__init__.py"), path_to_components
```

### Comparing `mvc4kivy-0.1.1/mvc4kivy/MVC/libs/__init__.py` & `mvc4kivy-0.1.2/mvc4kivy/MVC/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/mvc4kivy/MVC/libs/translation.py` & `mvc4kivy-0.1.2/mvc4kivy/MVC/libs/translation.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/mvc4kivy/MVC/messages.pot` & `mvc4kivy-0.1.2/mvc4kivy/MVC/messages.pot`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_firebase.py` & `mvc4kivy-0.1.2/mvc4kivy/MVC/Model/database_firebase.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_restdb.py` & `mvc4kivy-0.1.2/mvc4kivy/MVC/Model/database_restdb.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.1/PKG-INFO` & `mvc4kivy-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvc4kivy
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Kenechukwu Akubue
 Author-email: kengoon19@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

