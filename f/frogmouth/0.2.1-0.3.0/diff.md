# Comparing `tmp/frogmouth-0.2.1.tar.gz` & `tmp/frogmouth-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frogmouth-0.2.1.tar", max compression
+gzip compressed data, was "frogmouth-0.3.0.tar", max compression
```

## Comparing `frogmouth-0.2.1.tar` & `frogmouth-0.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.2.1/LICENSE
--rw-r--r--   0        0        0     2704 2023-04-29 14:55:46.077902 frogmouth-0.2.1/README.md
--rw-r--r--   0        0        0      283 2023-04-27 14:46:52.802054 frogmouth-0.2.1/frogmouth/__init__.py
--rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.2.1/frogmouth/__main__.py
--rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.2.1/frogmouth/app/__init__.py
--rw-r--r--   0        0        0     2110 2023-04-27 14:46:52.802301 frogmouth-0.2.1/frogmouth/app/app.py
--rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.2.1/frogmouth/data/__init__.py
--rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.2.1/frogmouth/data/bookmarks.py
--rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.2.1/frogmouth/data/config.py
--rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.2.1/frogmouth/data/data_directory.py
--rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.2.1/frogmouth/data/history.py
--rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.2.1/frogmouth/dialogs/__init__.py
--rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.2.1/frogmouth/dialogs/error.py
--rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.2.1/frogmouth/dialogs/help_dialog.py
--rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.2.1/frogmouth/dialogs/information.py
--rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.2.1/frogmouth/dialogs/input_dialog.py
--rw-r--r--   0        0        0     2168 2023-04-28 17:16:37.419494 frogmouth-0.2.1/frogmouth/dialogs/text_dialog.py
--rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.2.1/frogmouth/dialogs/yes_no_dialog.py
--rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.2.1/frogmouth/screens/__init__.py
--rw-r--r--   0        0        0    19015 2023-04-29 14:55:46.086907 frogmouth-0.2.1/frogmouth/screens/main.py
--rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.2.1/frogmouth/utility/__init__.py
--rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.2.1/frogmouth/utility/advertising.py
--rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.2.1/frogmouth/utility/forge.py
--rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.2.1/frogmouth/utility/type_tests.py
--rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.2.1/frogmouth/widgets/__init__.py
--rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.2.1/frogmouth/widgets/navigation.py
--rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/__init__.py
--rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/bookmarks.py
--rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/history.py
--rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/local_files.py
--rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/navigation_pane.py
--rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.2.1/frogmouth/widgets/navigation_panes/table_of_contents.py
--rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.2.1/frogmouth/widgets/omnibox.py
--rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.2.1/frogmouth/widgets/viewer.py
--rw-r--r--   0        0        0     1468 2023-04-29 14:58:49.538003 frogmouth-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 frogmouth-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-27 14:46:52.801782 frogmouth-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2743 2023-04-29 20:43:33.817264 frogmouth-0.3.0/README.md
+-rw-r--r--   0        0        0      283 2023-04-27 14:46:52.802054 frogmouth-0.3.0/frogmouth/__init__.py
+-rw-r--r--   0        0        0      112 2023-04-27 14:46:52.802125 frogmouth-0.3.0/frogmouth/__main__.py
+-rw-r--r--   0        0        0       74 2023-04-27 14:46:52.802222 frogmouth-0.3.0/frogmouth/app/__init__.py
+-rw-r--r--   0        0        0     2162 2023-04-29 20:42:18.209107 frogmouth-0.3.0/frogmouth/app/app.py
+-rw-r--r--   0        0        0      395 2023-04-27 14:46:52.802403 frogmouth-0.3.0/frogmouth/data/__init__.py
+-rw-r--r--   0        0        0     1639 2023-04-27 14:46:52.802497 frogmouth-0.3.0/frogmouth/data/bookmarks.py
+-rw-r--r--   0        0        0     2166 2023-04-27 14:46:52.802580 frogmouth-0.3.0/frogmouth/data/config.py
+-rw-r--r--   0        0        0      582 2023-04-27 14:46:52.802650 frogmouth-0.3.0/frogmouth/data/data_directory.py
+-rw-r--r--   0        0        0     1370 2023-04-27 14:46:52.802714 frogmouth-0.3.0/frogmouth/data/history.py
+-rw-r--r--   0        0        0      354 2023-04-27 14:46:52.802828 frogmouth-0.3.0/frogmouth/dialogs/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-28 13:52:42.406602 frogmouth-0.3.0/frogmouth/dialogs/error.py
+-rw-r--r--   0        0        0     4483 2023-04-29 14:55:46.078480 frogmouth-0.3.0/frogmouth/dialogs/help_dialog.py
+-rw-r--r--   0        0        0      269 2023-04-27 14:55:30.387330 frogmouth-0.3.0/frogmouth/dialogs/information.py
+-rw-r--r--   0        0        0     4278 2023-04-27 14:46:52.803185 frogmouth-0.3.0/frogmouth/dialogs/input_dialog.py
+-rw-r--r--   0        0        0     2168 2023-04-29 20:35:07.295162 frogmouth-0.3.0/frogmouth/dialogs/text_dialog.py
+-rw-r--r--   0        0        0     4898 2023-04-27 14:46:52.803359 frogmouth-0.3.0/frogmouth/dialogs/yes_no_dialog.py
+-rw-r--r--   0        0        0       83 2023-04-27 14:46:52.803485 frogmouth-0.3.0/frogmouth/screens/__init__.py
+-rw-r--r--   0        0        0    19015 2023-04-29 20:35:07.285373 frogmouth-0.3.0/frogmouth/screens/main.py
+-rw-r--r--   0        0        0      327 2023-04-27 14:46:52.803762 frogmouth-0.3.0/frogmouth/utility/__init__.py
+-rw-r--r--   0        0        0      894 2023-04-28 13:00:47.734733 frogmouth-0.3.0/frogmouth/utility/advertising.py
+-rw-r--r--   0        0        0     4237 2023-04-27 14:46:52.803923 frogmouth-0.3.0/frogmouth/utility/forge.py
+-rw-r--r--   0        0        0     1205 2023-04-27 14:46:52.804003 frogmouth-0.3.0/frogmouth/utility/type_tests.py
+-rw-r--r--   0        0        0      184 2023-04-27 14:46:52.804110 frogmouth-0.3.0/frogmouth/widgets/__init__.py
+-rw-r--r--   0        0        0     4398 2023-04-29 14:55:46.079307 frogmouth-0.3.0/frogmouth/widgets/navigation.py
+-rw-r--r--   0        0        0      298 2023-04-27 14:46:52.804311 frogmouth-0.3.0/frogmouth/widgets/navigation_panes/__init__.py
+-rw-r--r--   0        0        0     5889 2023-04-29 14:55:46.079533 frogmouth-0.3.0/frogmouth/widgets/navigation_panes/bookmarks.py
+-rw-r--r--   0        0        0     3235 2023-04-29 14:55:46.079738 frogmouth-0.3.0/frogmouth/widgets/navigation_panes/history.py
+-rw-r--r--   0        0        0     3412 2023-04-29 14:55:46.079932 frogmouth-0.3.0/frogmouth/widgets/navigation_panes/local_files.py
+-rw-r--r--   0        0        0      667 2023-04-29 14:55:46.080110 frogmouth-0.3.0/frogmouth/widgets/navigation_panes/navigation_pane.py
+-rw-r--r--   0        0        0     1704 2023-04-29 14:55:46.080286 frogmouth-0.3.0/frogmouth/widgets/navigation_panes/table_of_contents.py
+-rw-r--r--   0        0        0    11675 2023-04-28 17:16:37.437633 frogmouth-0.3.0/frogmouth/widgets/omnibox.py
+-rw-r--r--   0        0        0     9806 2023-04-27 15:34:09.464460 frogmouth-0.3.0/frogmouth/widgets/viewer.py
+-rw-r--r--   0        0        0     1468 2023-04-29 20:43:54.166747 frogmouth-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 frogmouth-0.3.0/PKG-INFO
```

### Comparing `frogmouth-0.2.1/LICENSE` & `frogmouth-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/README.md` & `frogmouth-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -55,55 +55,55 @@
 <img width="100%" alt="Screenshot 2023-04-28 at 15 16 39" src="https://user-images.githubusercontent.com/554369/235173418-58c23583-3fb3-4ff1-a723-10fa607cdd48.png">
 </td>
 
 </tr>
 
 </table>
 
+
+## Compatibility
+
+Frogmouth runs on Linux, macOS, and Windows. Frogmouth requires Python **3.8** or above.
+
+
 ## Installing
 
-The easiest way to install Frogmouth is probably via [pipx](https://pypa.github.io/pipx/) (particularly if you aren't a Python developer).
+The easiest way to install Frogmouth is with [pipx](https://pypa.github.io/pipx/) (particularly if you aren't a Python developer).
 
 ```
 pipx install frogmouth
 ```
 
-You can also install it via `pip`:
+You can also install Frogmouth with `pip`:
 
 ```
 pip install frogmouth
 ```
 
 Whichever method you use, you should have a `frogmouth` command on your path.
 
 ## Running
 
 Enter `frogmouth` at the prompt to run the app, optionally followed by a path to a Markdown file:
 
 ```
-frogmouth
+frogmouth README.md
 ```
 
 You can navigate with the mouse or the keyboard.
 Use <kbd>tab</kbd> and <kbd>shift</kbd>+<kbd>tab</kbd> to navigate between the various controls on screen.
 
 ## Features
 
-You can view local files from the command line with this:
-
-```
-frogmouth README.md
-```
-
-You can also load README files from GitHub repositories with the `gh` command.
+You can load README files direct from GitHub repositories with the `gh` command.
 Use the following syntax:
 
 ```
-frogmouth "gh textualize/textual"
+frogmouth gh textualize/textual
 ```
 
 This also works with the address bar in the app.
-See the help (**F1**) in the app for details.
+See the help (<kbd>F1</kbd>) in the app for details.
 
 ## Follow this project
 
 If this app interests you, you may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr).
```

#### html2text {}

```diff
@@ -8,21 +8,21 @@
 Demonstration
 ===============================================================================
 A quick video tour of Frogmouth. https://user-images.githubusercontent.com/
 554369/235305502-2699a70e-c9a6-495e-990e-67606d84bbfa.mp4 (thanks [Screen
 Studio](https://www.screen.studio/))  ## Screenshots
 [Screenshot 2023-04-28 at 15 14 53] [Screenshot 2023-04-28 at 15 17 56]
 [Screenshot 2023-04-28 at 15 18 36] [Screenshot 2023-04-28 at 15 16 39]
-## Installing The easiest way to install Frogmouth is probably via [pipx]
-(https://pypa.github.io/pipx/) (particularly if you aren't a Python developer).
-``` pipx install frogmouth ``` You can also install it via `pip`: ``` pip
-install frogmouth ``` Whichever method you use, you should have a `frogmouth`
-command on your path. ## Running Enter `frogmouth` at the prompt to run the
-app, optionally followed by a path to a Markdown file: ``` frogmouth ``` You
-can navigate with the mouse or the keyboard. Use tab and shift+tab to navigate
-between the various controls on screen. ## Features You can view local files
-from the command line with this: ``` frogmouth README.md ``` You can also load
-README files from GitHub repositories with the `gh` command. Use the following
-syntax: ``` frogmouth "gh textualize/textual" ``` This also works with the
-address bar in the app. See the help (**F1**) in the app for details. ## Follow
-this project If this app interests you, you may want to join the Textual
-[Discord server](https://discord.gg/Enf6Z3qhVr).
+## Compatibility Frogmouth runs on Linux, macOS, and Windows. Frogmouth
+requires Python **3.8** or above. ## Installing The easiest way to install
+Frogmouth is with [pipx](https://pypa.github.io/pipx/) (particularly if you
+aren't a Python developer). ``` pipx install frogmouth ``` You can also install
+Frogmouth with `pip`: ``` pip install frogmouth ``` Whichever method you use,
+you should have a `frogmouth` command on your path. ## Running Enter
+`frogmouth` at the prompt to run the app, optionally followed by a path to a
+Markdown file: ``` frogmouth README.md ``` You can navigate with the mouse or
+the keyboard. Use tab and shift+tab to navigate between the various controls on
+screen. ## Features You can load README files direct from GitHub repositories
+with the `gh` command. Use the following syntax: ``` frogmouth gh textualize/
+textual ``` This also works with the address bar in the app. See the help (F1)
+in the app for details. ## Follow this project If this app interests you, you
+may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr).
```

### Comparing `frogmouth-0.2.1/frogmouth/app/app.py` & `frogmouth-0.3.0/frogmouth/app/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,16 @@
         """
         super().__init__()
         self._args = cli_args
         self.dark = not load_config().light_mode
 
     def on_mount(self) -> None:
         """Set up the application after the DOM is ready."""
-        self.push_screen(Main(self._args.file))
+        file_or_command = " ".join(self._args.file)
+        self.push_screen(Main(file_or_command))
 
     def action_visit(self, url: str) -> None:
         """Visit the given URL, via the operating system.
 
         Args:
             url: The URL to visit.
         """
@@ -64,15 +65,15 @@
         "--version",
         help="Show version information.",
         action="version",
         version=f"%(prog)s {__version__} (Textual v{textual_version})",
     )
 
     # The remainder is the file to view.
-    parser.add_argument("file", help="The Markdown file to view", nargs="?")
+    parser.add_argument("file", help="The Markdown file to view", nargs="*")
 
     # Finally, parse the command line.
     return parser.parse_args()
 
 
 def run() -> None:
     """Run the application."""
```

### Comparing `frogmouth-0.2.1/frogmouth/data/bookmarks.py` & `frogmouth-0.3.0/frogmouth/data/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/data/config.py` & `frogmouth-0.3.0/frogmouth/data/config.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/data/data_directory.py` & `frogmouth-0.3.0/frogmouth/data/data_directory.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/data/history.py` & `frogmouth-0.3.0/frogmouth/data/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/dialogs/error.py` & `frogmouth-0.3.0/frogmouth/dialogs/error.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/dialogs/help_dialog.py` & `frogmouth-0.3.0/frogmouth/dialogs/help_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/dialogs/input_dialog.py` & `frogmouth-0.3.0/frogmouth/dialogs/input_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/dialogs/text_dialog.py` & `frogmouth-0.3.0/frogmouth/dialogs/text_dialog.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     }
 
     TextDialog Center {
         width: 100%;
     }
 
     TextDialog > Vertical {
-        background: $panel;
+        background: $boost;
         min-width: 30%;
         width: auto;
         height: auto;
         border: round $primary;
     }
 
     TextDialog Static {
```

### Comparing `frogmouth-0.2.1/frogmouth/dialogs/yes_no_dialog.py` & `frogmouth-0.3.0/frogmouth/dialogs/yes_no_dialog.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/screens/main.py` & `frogmouth-0.3.0/frogmouth/screens/main.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/utility/advertising.py` & `frogmouth-0.3.0/frogmouth/utility/advertising.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/utility/forge.py` & `frogmouth-0.3.0/frogmouth/utility/forge.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/utility/type_tests.py` & `frogmouth-0.3.0/frogmouth/utility/type_tests.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/navigation.py` & `frogmouth-0.3.0/frogmouth/widgets/navigation.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/bookmarks.py` & `frogmouth-0.3.0/frogmouth/widgets/navigation_panes/bookmarks.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/history.py` & `frogmouth-0.3.0/frogmouth/widgets/navigation_panes/history.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/local_files.py` & `frogmouth-0.3.0/frogmouth/widgets/navigation_panes/local_files.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/navigation_pane.py` & `frogmouth-0.3.0/frogmouth/widgets/navigation_panes/navigation_pane.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/navigation_panes/table_of_contents.py` & `frogmouth-0.3.0/frogmouth/widgets/navigation_panes/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/omnibox.py` & `frogmouth-0.3.0/frogmouth/widgets/omnibox.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/frogmouth/widgets/viewer.py` & `frogmouth-0.3.0/frogmouth/widgets/viewer.py`

 * *Files identical despite different names*

### Comparing `frogmouth-0.2.1/pyproject.toml` & `frogmouth-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "frogmouth"
 homepage = "https://github.com/Textualize/frogmouth"
-version = "0.2.1"
+version = "0.3.0"
 description = "A Markdown document viewer for the terminal"
 authors = ["Dave Pearson <dave@textualize.io>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "frogmouth"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `frogmouth-0.2.1/PKG-INFO` & `frogmouth-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frogmouth
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Markdown document viewer for the terminal
 Home-page: https://github.com/Textualize/frogmouth
 License: MIT
 Author: Dave Pearson
 Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -92,56 +92,56 @@
 <img width="100%" alt="Screenshot 2023-04-28 at 15 16 39" src="https://user-images.githubusercontent.com/554369/235173418-58c23583-3fb3-4ff1-a723-10fa607cdd48.png">
 </td>
 
 </tr>
 
 </table>
 
+
+## Compatibility
+
+Frogmouth runs on Linux, macOS, and Windows. Frogmouth requires Python **3.8** or above.
+
+
 ## Installing
 
-The easiest way to install Frogmouth is probably via [pipx](https://pypa.github.io/pipx/) (particularly if you aren't a Python developer).
+The easiest way to install Frogmouth is with [pipx](https://pypa.github.io/pipx/) (particularly if you aren't a Python developer).
 
 ```
 pipx install frogmouth
 ```
 
-You can also install it via `pip`:
+You can also install Frogmouth with `pip`:
 
 ```
 pip install frogmouth
 ```
 
 Whichever method you use, you should have a `frogmouth` command on your path.
 
 ## Running
 
 Enter `frogmouth` at the prompt to run the app, optionally followed by a path to a Markdown file:
 
 ```
-frogmouth
+frogmouth README.md
 ```
 
 You can navigate with the mouse or the keyboard.
 Use <kbd>tab</kbd> and <kbd>shift</kbd>+<kbd>tab</kbd> to navigate between the various controls on screen.
 
 ## Features
 
-You can view local files from the command line with this:
-
-```
-frogmouth README.md
-```
-
-You can also load README files from GitHub repositories with the `gh` command.
+You can load README files direct from GitHub repositories with the `gh` command.
 Use the following syntax:
 
 ```
-frogmouth "gh textualize/textual"
+frogmouth gh textualize/textual
 ```
 
 This also works with the address bar in the app.
-See the help (**F1**) in the app for details.
+See the help (<kbd>F1</kbd>) in the app for details.
 
 ## Follow this project
 
 If this app interests you, you may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: frogmouth Version: 0.2.1 Summary: A Markdown
+Metadata-Version: 2.1 Name: frogmouth Version: 0.3.0 Summary: A Markdown
 document viewer for the terminal Home-page: https://github.com/Textualize/
 frogmouth License: MIT Author: Dave Pearson Author-email: dave@textualize.io
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience :: Other
 Audience Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -29,21 +29,21 @@
 Demonstration
 ===============================================================================
 A quick video tour of Frogmouth. https://user-images.githubusercontent.com/
 554369/235305502-2699a70e-c9a6-495e-990e-67606d84bbfa.mp4 (thanks [Screen
 Studio](https://www.screen.studio/))  ## Screenshots
 [Screenshot 2023-04-28 at 15 14 53] [Screenshot 2023-04-28 at 15 17 56]
 [Screenshot 2023-04-28 at 15 18 36] [Screenshot 2023-04-28 at 15 16 39]
-## Installing The easiest way to install Frogmouth is probably via [pipx]
-(https://pypa.github.io/pipx/) (particularly if you aren't a Python developer).
-``` pipx install frogmouth ``` You can also install it via `pip`: ``` pip
-install frogmouth ``` Whichever method you use, you should have a `frogmouth`
-command on your path. ## Running Enter `frogmouth` at the prompt to run the
-app, optionally followed by a path to a Markdown file: ``` frogmouth ``` You
-can navigate with the mouse or the keyboard. Use tab and shift+tab to navigate
-between the various controls on screen. ## Features You can view local files
-from the command line with this: ``` frogmouth README.md ``` You can also load
-README files from GitHub repositories with the `gh` command. Use the following
-syntax: ``` frogmouth "gh textualize/textual" ``` This also works with the
-address bar in the app. See the help (**F1**) in the app for details. ## Follow
-this project If this app interests you, you may want to join the Textual
-[Discord server](https://discord.gg/Enf6Z3qhVr).
+## Compatibility Frogmouth runs on Linux, macOS, and Windows. Frogmouth
+requires Python **3.8** or above. ## Installing The easiest way to install
+Frogmouth is with [pipx](https://pypa.github.io/pipx/) (particularly if you
+aren't a Python developer). ``` pipx install frogmouth ``` You can also install
+Frogmouth with `pip`: ``` pip install frogmouth ``` Whichever method you use,
+you should have a `frogmouth` command on your path. ## Running Enter
+`frogmouth` at the prompt to run the app, optionally followed by a path to a
+Markdown file: ``` frogmouth README.md ``` You can navigate with the mouse or
+the keyboard. Use tab and shift+tab to navigate between the various controls on
+screen. ## Features You can load README files direct from GitHub repositories
+with the `gh` command. Use the following syntax: ``` frogmouth gh textualize/
+textual ``` This also works with the address bar in the app. See the help (F1)
+in the app for details. ## Follow this project If this app interests you, you
+may want to join the Textual [Discord server](https://discord.gg/Enf6Z3qhVr).
```

