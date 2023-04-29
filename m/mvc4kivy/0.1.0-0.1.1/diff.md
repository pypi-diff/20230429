# Comparing `tmp/mvc4kivy-0.1.0.tar.gz` & `tmp/mvc4kivy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvc4kivy-0.1.0.tar", max compression
+gzip compressed data, was "mvc4kivy-0.1.1.tar", max compression
```

## Comparing `mvc4kivy-0.1.0.tar` & `mvc4kivy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.0/mvc4kivy/__init__.py
--rw-r--r--   0        0        0     6747 2023-04-29 04:57:12.975087 mvc4kivy-0.1.0/mvc4kivy/add_view.py
--rw-r--r--   0        0        0    42680 2023-04-29 08:55:56.516304 mvc4kivy-0.1.0/mvc4kivy/create_project.py
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.0/mvc4kivy/MVC/__init__.py
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.0/mvc4kivy/MVC/data/locales/po/en.po
--rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.0/mvc4kivy/MVC/data/locales/po/ru.po
--rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.0/mvc4kivy/MVC/libs/__init__.py
--rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.0/mvc4kivy/MVC/libs/translation.py
--rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.0/mvc4kivy/MVC/messages.pot
--rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.0/mvc4kivy/MVC/Model/__init__.py
--rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.0/mvc4kivy/MVC/Model/database_firebase.py
--rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.0/mvc4kivy/MVC/Model/database_restdb.py
--rw-r--r--   0        0        0      418 2023-04-29 04:31:06.634234 mvc4kivy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.0/README.md
--rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 mvc4kivy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3255 2023-04-29 08:24:08.275191 mvc4kivy-0.1.1/mvc4kivy/__init__.py
+-rw-r--r--   0        0        0     7029 2023-04-29 09:29:50.333179 mvc4kivy-0.1.1/mvc4kivy/add_view.py
+-rw-r--r--   0        0        0    42474 2023-04-29 11:39:38.590717 mvc4kivy-0.1.1/mvc4kivy/create_project.py
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.301767 mvc4kivy-0.1.1/mvc4kivy/MVC/__init__.py
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.308770 mvc4kivy-0.1.1/mvc4kivy/MVC/data/locales/po/en.po
+-rw-r--r--   0        0        0      425 2023-04-28 04:02:52.309769 mvc4kivy-0.1.1/mvc4kivy/MVC/data/locales/po/ru.po
+-rw-r--r--   0        0        0     1202 2023-04-29 08:55:56.501660 mvc4kivy-0.1.1/mvc4kivy/MVC/libs/__init__.py
+-rw-r--r--   0        0        0     1411 2023-04-28 04:02:52.312767 mvc4kivy-0.1.1/mvc4kivy/MVC/libs/translation.py
+-rw-r--r--   0        0        0      582 2023-04-28 04:02:52.302769 mvc4kivy-0.1.1/mvc4kivy/MVC/messages.pot
+-rw-r--r--   0        0        0        0 2023-04-28 04:02:52.303773 mvc4kivy-0.1.1/mvc4kivy/MVC/Model/__init__.py
+-rw-r--r--   0        0        0      827 2023-04-28 04:21:40.764773 mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_firebase.py
+-rw-r--r--   0        0        0     3675 2023-04-28 04:21:40.785037 mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_restdb.py
+-rw-r--r--   0        0        0      418 2023-04-29 11:39:59.717568 mvc4kivy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      231 2023-04-29 04:31:06.582521 mvc4kivy-0.1.1/README.md
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 mvc4kivy-0.1.1/PKG-INFO
```

### Comparing `mvc4kivy-0.1.0/mvc4kivy/__init__.py` & `mvc4kivy-0.1.1/mvc4kivy/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.0/mvc4kivy/add_view.py` & `mvc4kivy-0.1.1/mvc4kivy/add_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,28 +57,32 @@
 screens = {%s
 }"""
 
 screns_comment = """# The screen's dictionary contains the objects of the models and controllers
 # of the screens of the application.
 """
 
+instantiate_responsive_view = ""
+
 
 def main():
     """The function of adding a new view to the project."""
 
     global screens_data
+    global instantiate_responsive_view
 
     parser = create_argument_parser()
     args = parser.parse_args()
 
     # pattern_name isn't used currently, will be used if new patterns is added in future
     pattern_name = args.pattern  # noqa F841
     path_to_project = args.directory
     name_view = args.name
     use_responsive = args.use_responsive
+    instantiate_responsive_view = args.instantiate_responsive_view
 
     if not os.path.exists(path_to_project):
         parser.error(f"Project <{path_to_project}> does not exist...")
 
     if name_view[-6:] != "Screen":
         parser.error(
             f"The name of the <{name_view}> screen should contain the word "
@@ -195,12 +199,17 @@
         help="the name of the view to add to an existing project.",
     )
     parser.add_argument(
         "--use_responsive",
         default="no",
         help="whether to create a view with responsive behavior.",
     )
+    parser.add_argument(
+        "--instantiate_responsive_view",
+        default="yes",
+        help="instantiate responsive"
+    )
     return parser
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mvc4kivy-0.1.0/mvc4kivy/create_project.py` & `mvc4kivy-0.1.1/mvc4kivy/create_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,27 +308,27 @@
 
 
 """
 
 temp_code_responsive_view = '''from kivymd.uix.responsivelayout import MDResponsiveLayout
 
 from View.{name_screen}.components import (
-    {name_screen_prefix}MobileScreenView,
-    {name_screen_prefix}TabletScreenView,
-    {name_screen_prefix}DesktopScreenView,
+    {name_screen}MobileView,
+    {name_screen}TabletView,
+    {name_screen}DesktopView,
 )
 from View.base_screen import BaseScreenView
 
 
 class {name_screen}View(MDResponsiveLayout, BaseScreenView):
     def __init__(self, **kw):
         super().__init__(**kw)
-        self.mobile_view = {name_screen_prefix}MobileScreenView{parenthesis}
-        self.tablet_view = {name_screen_prefix}TabletScreenView{parenthesis}
-        self.desktop_view = {name_screen_prefix}DesktopScreenView{parenthesis}
+        self.mobile_view = {name_screen}MobileView{parenthesis}
+        self.tablet_view = {name_screen}TabletView{parenthesis}
+        self.desktop_view = {name_screen}DesktopView{parenthesis}
 
     def model_is_changed(self) -> None:
         """
         Called whenever any change has occurred in the data model.
         The view in this method tracks these changes and updates the UI
         according to these changes.
         """
@@ -1045,21 +1045,19 @@
     os.makedirs(path_to_components)
 
     with open(
             os.path.join(path_to_view, "__init__.py"), "w", encoding="utf-8"
     ) as init_module:
         init_module.write("")
     with open(f"{view_module}.py", "w", encoding="utf-8") as view_file:
-        name_screen_prefix = re.findall("[A-Z][a-z]*", name_screen)[0]
         view_file.write(
             temp_code_view.format(name_screen=name_screen)
             if name_screen not in use_responsive
             else temp_code_responsive_view.format(
                 name_screen=name_screen,
-                name_screen_prefix=name_screen_prefix,
                 parenthesis="()" if instantiate_responsive_view else ""
             )
         )
 
     if name_screen in use_responsive:
         for name_platform in ["DesktopScreen", "MobileScreen", "TabletScreen"]:
             path_to_init_components = os.path.join(
```

### Comparing `mvc4kivy-0.1.0/mvc4kivy/MVC/libs/__init__.py` & `mvc4kivy-0.1.1/mvc4kivy/MVC/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.0/mvc4kivy/MVC/libs/translation.py` & `mvc4kivy-0.1.1/mvc4kivy/MVC/libs/translation.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.0/mvc4kivy/MVC/messages.pot` & `mvc4kivy-0.1.1/mvc4kivy/MVC/messages.pot`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.0/mvc4kivy/MVC/Model/database_firebase.py` & `mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_firebase.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.0/mvc4kivy/MVC/Model/database_restdb.py` & `mvc4kivy-0.1.1/mvc4kivy/MVC/Model/database_restdb.py`

 * *Files identical despite different names*

### Comparing `mvc4kivy-0.1.0/PKG-INFO` & `mvc4kivy-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mvc4kivy
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Kenechukwu Akubue
 Author-email: kengoon19@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

