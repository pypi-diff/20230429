# Comparing `tmp/recoverpy-2.0.5.tar.gz` & `tmp/recoverpy-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recoverpy-2.0.5.tar", max compression
+gzip compressed data, was "recoverpy-2.0.6.tar", max compression
```

## Comparing `recoverpy-2.0.5.tar` & `recoverpy-2.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rwxr-xr-x   0        0        0    32501 2023-03-31 08:11:11.195256 recoverpy-2.0.5/LICENSE
--rwxr-xr-x   0        0        0     3876 2023-03-31 08:11:11.195256 recoverpy-2.0.5/README.md
--rw-r--r--   0        0        0     3182 2023-03-31 08:11:11.219256 recoverpy-2.0.5/pyproject.toml
--rwxr-xr-x   0        0        0      181 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/__init__.py
--rwxr-xr-x   0        0        0       66 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/__main__.py
--rwxr-xr-x   0        0        0     1044 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/helper.py
--rwxr-xr-x   0        0        0     1219 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/lsblk.py
--rwxr-xr-x   0        0        0     1449 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/saver.py
--rwxr-xr-x   0        0        0      258 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/search/grep_consumer.py
--rwxr-xr-x   0        0        0      729 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/search/progress_monitoring.py
--rwxr-xr-x   0        0        0     2656 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/search/result_processor.py
--rwxr-xr-x   0        0        0     2587 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/search/search_engine.py
--rwxr-xr-x   0        0        0     1336 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/lib/search/thread_factory.py
--rwxr-xr-x   0        0        0      629 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/models/grep_result.py
--rwxr-xr-x   0        0        0      247 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/models/partition.py
--rwxr-xr-x   0        0        0      383 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/models/search_params.py
--rwxr-xr-x   0        0        0      120 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/models/search_progress.py
--rwxr-xr-x   0        0        0     2072 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/app.py
--rwxr-xr-x   0        0        0      152 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/__init__.py
--rwxr-xr-x   0        0        0       45 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/common.css
--rwxr-xr-x   0        0        0      292 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/screen-modal.css
--rwxr-xr-x   0        0        0      609 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/screen-params.css
--rwxr-xr-x   0        0        0      253 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/screen-path-edit.css
--rwxr-xr-x   0        0        0     1286 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/screen-result.css
--rwxr-xr-x   0        0        0      469 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/screen-save.css
--rwxr-xr-x   0        0        0     1050 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/css/screen-search.css
--rwxr-xr-x   0        0        0      897 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/screens/screen_modal.py
--rwxr-xr-x   0        0        0     1879 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/screens/screen_params.py
--rwxr-xr-x   0        0        0     1107 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/screens/screen_path_edit.py
--rwxr-xr-x   0        0        0     3659 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/screens/screen_result.py
--rwxr-xr-x   0        0        0     2266 2023-03-31 08:11:11.219256 recoverpy-2.0.5/recoverpy/ui/screens/screen_save.py
--rwxr-xr-x   0        0        0     4062 2023-03-31 08:11:11.223256 recoverpy-2.0.5/recoverpy/ui/screens/screen_search.py
--rwxr-xr-x   0        0        0     4098 2023-03-31 08:11:11.223256 recoverpy-2.0.5/recoverpy/ui/widgets/directory_tree.py
--rwxr-xr-x   0        0        0     1985 2023-03-31 08:11:11.223256 recoverpy-2.0.5/recoverpy/ui/widgets/grep_result_list.py
--rwxr-xr-x   0        0        0     1061 2023-03-31 08:11:11.223256 recoverpy-2.0.5/recoverpy/ui/widgets/partition_list.py
--rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 recoverpy-2.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    32501 2023-04-29 08:26:05.605463 recoverpy-2.0.6/LICENSE
+-rwxr-xr-x   0        0        0     4013 2023-04-29 08:26:05.605463 recoverpy-2.0.6/README.md
+-rw-r--r--   0        0        0     3270 2023-04-29 08:26:05.625463 recoverpy-2.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0      181 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/__init__.py
+-rwxr-xr-x   0        0        0       66 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/__main__.py
+-rwxr-xr-x   0        0        0     1044 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/helper.py
+-rwxr-xr-x   0        0        0     1219 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/lsblk.py
+-rwxr-xr-x   0        0        0     1449 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/saver.py
+-rwxr-xr-x   0        0        0      258 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/search/grep_consumer.py
+-rwxr-xr-x   0        0        0      729 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/search/progress_monitoring.py
+-rwxr-xr-x   0        0        0     2656 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/search/result_processor.py
+-rwxr-xr-x   0        0        0     2587 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/search/search_engine.py
+-rwxr-xr-x   0        0        0     1336 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/lib/search/thread_factory.py
+-rwxr-xr-x   0        0        0      629 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/models/grep_result.py
+-rwxr-xr-x   0        0        0      247 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/models/partition.py
+-rwxr-xr-x   0        0        0      383 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/models/search_params.py
+-rwxr-xr-x   0        0        0      120 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/models/search_progress.py
+-rwxr-xr-x   0        0        0     2005 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/app.py
+-rwxr-xr-x   0        0        0      152 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/__init__.py
+-rwxr-xr-x   0        0        0       45 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/common.css
+-rwxr-xr-x   0        0        0      292 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/screen-modal.css
+-rwxr-xr-x   0        0        0      609 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/screen-params.css
+-rwxr-xr-x   0        0        0      253 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/screen-path-edit.css
+-rwxr-xr-x   0        0        0     1286 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/screen-result.css
+-rwxr-xr-x   0        0        0      469 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/screen-save.css
+-rwxr-xr-x   0        0        0     1050 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/css/screen-search.css
+-rwxr-xr-x   0        0        0      932 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/screens/screen_modal.py
+-rwxr-xr-x   0        0        0     1921 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/screens/screen_params.py
+-rwxr-xr-x   0        0        0     1149 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/screens/screen_path_edit.py
+-rwxr-xr-x   0        0        0     3680 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/screens/screen_result.py
+-rwxr-xr-x   0        0        0     2308 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/screens/screen_save.py
+-rwxr-xr-x   0        0        0     4146 2023-04-29 08:26:05.625463 recoverpy-2.0.6/recoverpy/ui/screens/screen_search.py
+-rwxr-xr-x   0        0        0     4119 2023-04-29 08:26:05.629463 recoverpy-2.0.6/recoverpy/ui/widgets/directory_tree.py
+-rwxr-xr-x   0        0        0     2011 2023-04-29 08:26:05.629463 recoverpy-2.0.6/recoverpy/ui/widgets/grep_result_list.py
+-rwxr-xr-x   0        0        0     1082 2023-04-29 08:26:05.629463 recoverpy-2.0.6/recoverpy/ui/widgets/partition_list.py
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 recoverpy-2.0.6/PKG-INFO
```

### Comparing `recoverpy-2.0.5/LICENSE` & `recoverpy-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/README.md` & `recoverpy-2.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ---
 
 <!--ts-->
    * [Demo](#Demo)
    * [Installation](#Installation)
       * [Dependancies](#arrow_right-dependancies)
       * [Installation from pip](#arrow_right-installation-from-pip)
+      * [Installation from AUR](#arrow_right-installation-from-aur)
    * [Usage](#Usage)
    * [Tips](#Tips)
    * [Contributing](#Contributing)
 <!--te-->
 
 ---
 
@@ -64,14 +65,18 @@
 - Arch: `pacman -S grep coreutils util-linux progress`
 - Fedora: `dnf install grep coreutils util-linux progress`
 
 #### :arrow_right: Installation from pip
 
 `python3 -m pip install recoverpy`
 
+#### :arrow_right: Installation from AUR
+
+`yay -S python-recoverpy`
+
 ## Usage
 
 ```bash
 python3 -m recoverpy
 ```
 
 :red_circle: **You must be root or use sudo**.
```

#### html2text {}

```diff
@@ -1,41 +1,43 @@
                                   [RecoverPy]
                      Recover overwritten or deleted data.
                     [Release] [License] [Downloads] [Tests]
 ---  * [Demo](#Demo) * [Installation](#Installation) * [Dependancies]
 (#arrow_right-dependancies) * [Installation from pip](#arrow_right-
-installation-from-pip) * [Usage](#Usage) * [Tips](#Tips) * [Contributing]
-(#Contributing)  --- # RecoverPy RecoverPy is a powerful tool that leverages
-your system capabilities to recover lost files. Unlike others, you can not only
-recover deleted files but also **overwritten** data. Every block of your
-partition will be scanned. You can even find a string in binary files. ## Demo
+installation-from-pip) * [Installation from AUR](#arrow_right-installation-
+from-aur) * [Usage](#Usage) * [Tips](#Tips) * [Contributing](#Contributing)  --
+- # RecoverPy RecoverPy is a powerful tool that leverages your system
+capabilities to recover lost files. Unlike others, you can not only recover
+deleted files but also **overwritten** data. Every block of your partition will
+be scanned. You can even find a string in binary files. ## Demo
                             [docs/assets/demo.gif]
 ## Installation :penguin: RecoverPy is currently only available on Linux
 systems. #### :arrow_right: Dependancies **Mandatory:** To list and search
 through your partitions, recoverpy uses `grep`, `dd`, and `lsblk` commands.
 Although, if you're running a major Linux distrucition these tools should
 already be installed. **Optional:** To display real time grep progress, you can
 install `progress`. To install all dependencies: - Debian-like: `apt install
 grep coreutils util-linux progress` - Arch: `pacman -S grep coreutils util-
 linux progress` - Fedora: `dnf install grep coreutils util-linux progress` ####
-:arrow_right: Installation from pip `python3 -m pip install recoverpy` ## Usage
-```bash python3 -m recoverpy ``` :red_circle: **You must be root or use sudo**.
---- :one: **Select the system partition** in which your file was. If you are
-out of luck, you can alternatively search in your home partition, maybe your
-IDE, text editor, etc. made a backup at some point. :two: **Type a text string
-to search**. See tips below for better results. :three: **Start search**,
-Results will appear in the left-hand box. :four: **Select a result**. :five:
-Once you have found your precious, **select `Open`**. :six: You can now either
-save this block individually or explore neighboring blocks for the remaining
-parts of the file. You could then save it all in one file. ## Tips - Always do
-backups! Yes, maybe too late... - **Unmount your partition before you do
-anything!** Although you can search with your partition still mounted, it is
-highly recommended to unmount your partition to avoid any alteration to your
-file. Regarding the searched string: - Be concise, find something that could be
-unique to your file. - Stay simple, your string is escaped but exotic
-characters may affect your results. - Try to remember the last edit you have
-made to your file. When you have found your file: - You might see multiple
-results. Your system often use different partion blocks to save successive
-versions of a file. Make sure you've found the last version. - Try exploring
-neighboring blocks to be sure to save your whole file. ## Contributing Thank
-you for considering contributing to RecoverPy. Any request, bug report or PR
-are welcome. Please read the [contributing guide](CONTRIBUTING.md).
+:arrow_right: Installation from pip `python3 -m pip install recoverpy` #### :
+arrow_right: Installation from AUR `yay -S python-recoverpy` ## Usage ```bash
+python3 -m recoverpy ``` :red_circle: **You must be root or use sudo**. --- :
+one: **Select the system partition** in which your file was. If you are out of
+luck, you can alternatively search in your home partition, maybe your IDE, text
+editor, etc. made a backup at some point. :two: **Type a text string to
+search**. See tips below for better results. :three: **Start search**, Results
+will appear in the left-hand box. :four: **Select a result**. :five: Once you
+have found your precious, **select `Open`**. :six: You can now either save this
+block individually or explore neighboring blocks for the remaining parts of the
+file. You could then save it all in one file. ## Tips - Always do backups! Yes,
+maybe too late... - **Unmount your partition before you do anything!** Although
+you can search with your partition still mounted, it is highly recommended to
+unmount your partition to avoid any alteration to your file. Regarding the
+searched string: - Be concise, find something that could be unique to your
+file. - Stay simple, your string is escaped but exotic characters may affect
+your results. - Try to remember the last edit you have made to your file. When
+you have found your file: - You might see multiple results. Your system often
+use different partion blocks to save successive versions of a file. Make sure
+you've found the last version. - Try exploring neighboring blocks to be sure to
+save your whole file. ## Contributing Thank you for considering contributing to
+RecoverPy. Any request, bug report or PR are welcome. Please read the
+[contributing guide](CONTRIBUTING.md).
```

### Comparing `recoverpy-2.0.5/pyproject.toml` & `recoverpy-2.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "recoverpy"
-version = "2.0.5"
+version = "2.0.6"
 description = "A TUI to recover overwritten or deleted data."
 authors = ["PabloLec <pablolec@pm.me>"]
 license = "GPL-3.0 License"
 readme = "README.md"
 homepage = "https://github.com/PabloLec/recoverpy"
 repository = "https://github.com/PabloLec/recoverpy"
 documentation = "https://github.com/PabloLec/recoverpy#readme"
@@ -64,46 +64,50 @@
         "Topic :: System :: Systems Administration",
         "Topic :: Terminals",
         "Topic :: Utilities",
         "Typing :: Typed",
         "Framework :: AsyncIO",
 ]
 
+[tool.poetry.scripts]
+recoverpy = "recoverpy.__init__:main"
+
 [tool.poetry.dependencies]
 python = "^3.8.1"
-textual = "^0.17.1"
+textual = ">=0.17.1,<0.23.0"
 
 [tool.poetry.dev-dependencies]
-coverage = "^7.2.2"
-pytest = "^7.2.2"
-pylint = "^2.17.1"
+coverage = "^7.2.4"
+pytest = "^7.3.1"
+pylint = "^2.17.3"
 isort = "^5.12.0"
 black = "^23.3"
 flake8 = "^6.0.0"
-pre-commit = "^3.2.1"
+pre-commit = "^3.2.2"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.3.23"
 flake8-builtins = "^2.0.0"
-flake8-comprehensions = "^3.11.1"
+flake8-comprehensions = "^3.12.0"
 darglint = "^1.8.1"
 flake8-docstrings = "^1.7.0"
 flake8-isort = "^6.0.0"
 flake8-pytest-style = "^1.7.2"
 flake8-mutable = "^1.2.0"
 flake8-html = "^0.4.1"
 flake8-simplify = "^0.20.0"
-flake8-aaa = "^0.14.0"
+flake8-aaa = "^0.14.1"
 pytest-mock = "3.10.0"
 pytest-cov = "^4.0.0"
 coverage-badge = "^1.1.0"
-mypy = "^1.1"
+mypy = "^1.2"
 types-PyYAML = "^6.0.12"
 
 [tool.poetry.group.dev.dependencies]
 pytest-asyncio = ">=0.20.3,<0.22.0"
+ruff = "^0.0.263"
 
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
 python_version = 3.8
 ignore_missing_imports = "true"
```

### Comparing `recoverpy-2.0.5/recoverpy/lib/helper.py` & `recoverpy-2.0.6/recoverpy/lib/helper.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/lib/lsblk.py` & `recoverpy-2.0.6/recoverpy/lib/lsblk.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/lib/saver.py` & `recoverpy-2.0.6/recoverpy/lib/saver.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/lib/search/progress_monitoring.py` & `recoverpy-2.0.6/recoverpy/lib/search/progress_monitoring.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/lib/search/result_processor.py` & `recoverpy-2.0.6/recoverpy/lib/search/result_processor.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/lib/search/search_engine.py` & `recoverpy-2.0.6/recoverpy/lib/search/search_engine.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/lib/search/thread_factory.py` & `recoverpy-2.0.6/recoverpy/lib/search/thread_factory.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/models/grep_result.py` & `recoverpy-2.0.6/recoverpy/models/grep_result.py`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/ui/app.py` & `recoverpy-2.0.6/recoverpy/ui/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "params": ParamsScreen(),
         "search": SearchScreen(),
         "result": ResultScreen(),
         "save": SaveScreen(),
         "path_edit": PathEditScreen(),
         "modal": ModalScreen(),
     }
-    CSS_PATH = get_css()  # type: ignore # mypy bug, List[str] = List[Union[str, PurePath]]
+    CSS_PATH = get_css()
 
     def __init__(self, *args, **kwargs) -> None:  # type: ignore
         super().__init__(*args, **kwargs)
         self._is_user_root = True
 
     def on_mount(self) -> None:
         if self._is_user_root:
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/css/screen-params.css` & `recoverpy-2.0.6/recoverpy/ui/css/screen-params.css`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/ui/css/screen-result.css` & `recoverpy-2.0.6/recoverpy/ui/css/screen-result.css`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/ui/css/screen-search.css` & `recoverpy-2.0.6/recoverpy/ui/css/screen-search.css`

 * *Files identical despite different names*

### Comparing `recoverpy-2.0.5/recoverpy/ui/screens/screen_modal.py` & `recoverpy-2.0.6/recoverpy/ui/screens/screen_modal.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 
 from textual.app import ComposeResult
 from textual.containers import Grid, Horizontal
 from textual.screen import Screen
 from textual.widgets import Button, Label
 
 
-class ModalScreen(Screen):
+class ModalScreen(Screen):  # type:ignore[misc]
     _message_label = Label("", id="modal-message")
     _callback: Callable  # type: ignore
 
-    def set(self, message: str, callback: Optional[Callable] = None) -> None:  # type: ignore
+    def set(
+        self, message: str, callback: Optional[Callable] = None
+    ) -> None:  # type: ignore
         self._message_label.update(message)
         self._callback = callback or self.app.pop_screen
 
     def compose(self) -> ComposeResult:
         yield Grid(
             self._message_label,
             Horizontal(
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/screens/screen_params.py` & `recoverpy-2.0.6/recoverpy/ui/screens/screen_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from textual.screen import Screen
 from textual.widgets import Button, Input, Label
 
 from recoverpy.models.partition import Partition
 from recoverpy.ui.widgets.partition_list import PartitionList
 
 
-class ParamsScreen(Screen):
+class ParamsScreen(Screen):  # type:ignore[misc]
     _partition_list: PartitionList
     _search_input: Input
     _start_search_button: Button
 
-    class Continue(Message):
+    class Continue(Message):  # type:ignore[misc]
         def __init__(self, searched_string: str, selected_partition: str) -> None:
             self.searched_string = searched_string
             self.selected_partition = selected_partition
             super().__init__()
 
     def compose(self) -> ComposeResult:
         self._partition_list = PartitionList()
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/screens/screen_path_edit.py` & `recoverpy-2.0.6/recoverpy/ui/screens/screen_path_edit.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from textual.message import Message
 from textual.screen import Screen
 from textual.widgets import Button
 
 from recoverpy.ui.widgets.directory_tree import DirectoryTree
 
 
-class PathEditScreen(Screen):
+class PathEditScreen(Screen):  # type:ignore[misc]
     def __init__(self, *args, **kwargs) -> None:  # type: ignore
         self._directory_tree = DirectoryTree("/")
         super().__init__(*args, **kwargs)
 
-    class Confirm(Message):
+    class Confirm(Message):  # type:ignore[misc]
         def __init__(self, selected_dir: str) -> None:
             self.selected_dir = selected_dir
             super().__init__()
 
     def compose(self) -> ComposeResult:
         yield self._directory_tree
         yield Horizontal(
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/screens/screen_result.py` & `recoverpy-2.0.6/recoverpy/ui/screens/screen_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from textual.widgets import Button, Label, TextLog
 
 from recoverpy.lib.helper import decode_result, get_dd_output, get_printable
 from recoverpy.lib.saver import Saver
 from recoverpy.ui.screens.screen_save import SaveScreen
 
 
-class ResultScreen(Screen):
+class ResultScreen(Screen):  # type:ignore[misc]
     def __init__(self, *args, **kwargs) -> None:  # type: ignore
         self._saver = Saver()
         self._partition = ""
         self._block_size = 0
         self._inode = 0
         self._inode_label = Label("", id="inode-label")
         self._block_count_label = Label("0 block selected", id="block-count")
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/screens/screen_save.py` & `recoverpy-2.0.6/recoverpy/ui/screens/screen_save.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from textual.screen import Screen
 from textual.widgets import Button, Label
 
 from recoverpy.lib.saver import Saver
 from recoverpy.ui.screens.screen_path_edit import PathEditScreen
 
 
-class SaveScreen(Screen):
-    class Saved(Message):
+class SaveScreen(Screen):  # type:ignore[misc]
+    class Saved(Message):  # type:ignore[misc]
         def __init__(self, save_path: str) -> None:
             self.save_path = save_path
             super().__init__()
 
     def __init__(self, *args, **kwargs) -> None:  # type: ignore
         self._saver: Optional[Saver] = None
         self._save_path_label = Label("", id="save-path-label")
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/screens/screen_search.py` & `recoverpy-2.0.6/recoverpy/ui/screens/screen_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 from textual.screen import Screen
 from textual.widgets import Button, Label
 
 from recoverpy.lib.search.search_engine import SearchEngine
 from recoverpy.ui.widgets.grep_result_list import GrepResultList
 
 
-class SearchScreen(Screen):
+class SearchScreen(Screen):  # type:ignore[misc]
     _grep_result_list: GrepResultList
     _result_count_label: Label
     _progress_title_label: Label
     _progress_label: Label
     _open_button: Button
     search_engine: SearchEngine
 
-    class Start(Message):
+    class Start(Message):  # type:ignore[misc]
         def __init__(self, searched_string: str, selected_partition: str) -> None:
             self.searched_string = searched_string
             self.selected_partition = selected_partition
             super().__init__()
 
-    class Open(Message):
+    class Open(Message):  # type:ignore[misc]
         def __init__(self, inode: int, block_size: int, partition: str) -> None:
             self.inode = inode
             self.block_size = block_size
             self.partition = partition
             super().__init__()
 
-    class InfoContainer(Horizontal):
+    class InfoContainer(Horizontal):  # type:ignore[misc]
         def __init__(self, *args, **kwargs) -> None:  # type: ignore
             super().__init__(classes="info-container", *args, **kwargs)
 
     def __init__(self, *args, **kwargs) -> None:  # type: ignore
         self.results: List[str] = []
         super().__init__(*args, **kwargs)
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/widgets/directory_tree.py` & `recoverpy-2.0.6/recoverpy/ui/widgets/directory_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """Attaches directory information ot a node."""
 
     path: str
     is_dir: bool
     loaded: bool = False
 
 
-class DirectoryTree(Tree[DirEntry]):
+class DirectoryTree(Tree[DirEntry]):  # type:ignore[misc]
     COMPONENT_CLASSES: ClassVar[set[str]] = {
         "tree--label",
         "tree--guides",
         "tree--guides-hover",
         "tree--guides-selected",
         "tree--cursor",
         "tree--highlight",
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/widgets/grep_result_list.py` & `recoverpy-2.0.6/recoverpy/ui/widgets/grep_result_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from textual.widget import Widget
 from textual.widgets import Label, ListView
 
 from recoverpy.models.grep_result import GrepResult
 
 
-class GrepResultList(ListView):
+class GrepResultList(ListView):  # type:ignore[misc]
     list_items_background_color = {0: "red", 1: "green"}
 
     def __init__(self, *children, **kwargs) -> None:  # type: ignore
         super().__init__(*children, **kwargs)
         self.results: List[str] = []
         self.lock = Lock()
         self.grep_results: List[GrepResult] = []
@@ -37,15 +37,15 @@
             return
         async with self.lock:
             self.grep_results.append(grep_result)
             self._resize_item(len(self.grep_results) - 1, grep_result.list_item)
             await super().append(grep_result.list_item)
 
     def _get_list_index_to_show(self) -> int:
-        return self.size.height + int(self.scroll_y) + 10
+        return int(self.size.height) + int(self.scroll_y) + 10
 
     def _should_add_more(self) -> bool:
         return len(self.children) < self._get_list_index_to_show()
 
     def on_resize(self) -> None:
         for index, item in enumerate(self.children):
             self._resize_item(index, item)
```

### Comparing `recoverpy-2.0.5/recoverpy/ui/widgets/partition_list.py` & `recoverpy-2.0.6/recoverpy/ui/widgets/partition_list.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def _get_label(partition: Partition) -> Label:
     label_content = f"{partition.name} | {partition.fs_type}"
     if partition.is_mounted:
         label_content += f" | Mounted on: {partition.mount_point}"
     return Label(label_content)
 
 
-class PartitionList(ListView):
+class PartitionList(ListView):  # type:ignore[misc]
     def __init__(self, *children, **kwargs) -> None:  # type: ignore
         super().__init__(*children, **kwargs)
         self.list_items: Dict[Optional[str], Partition] = {}
         self._append_partitions()
 
     def _append_partitions(self) -> None:
         for partition in get_partitions():
```

### Comparing `recoverpy-2.0.5/PKG-INFO` & `recoverpy-2.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recoverpy
-Version: 2.0.5
+Version: 2.0.6
 Summary: A TUI to recover overwritten or deleted data.
 Home-page: https://github.com/PabloLec/recoverpy
 License: GPL-3.0 License
 Keywords: data,recovery,search,cli,console,cui,tui,ncurses,terminal,cybersec,cybersecurity,security,pentesting,pentest,forensics,forensic,hack,hacking,data recovery,data recovery tool,grep,linux,unix,education,teaching,training,teach,learn,textual,asyncio,async
 Author: PabloLec
 Author-email: pablolec@pm.me
 Requires-Python: >=3.8.1,<4.0.0
@@ -34,15 +34,15 @@
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: System :: Recovery Tools
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: textual (>=0.17.1,<0.18.0)
+Requires-Dist: textual (>=0.17.1,<0.23.0)
 Project-URL: Documentation, https://github.com/PabloLec/recoverpy#readme
 Project-URL: Repository, https://github.com/PabloLec/recoverpy
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img src="docs/assets/logo.png" alt="RecoverPy">
 </div>
@@ -70,14 +70,15 @@
 ---
 
 <!--ts-->
    * [Demo](#Demo)
    * [Installation](#Installation)
       * [Dependancies](#arrow_right-dependancies)
       * [Installation from pip](#arrow_right-installation-from-pip)
+      * [Installation from AUR](#arrow_right-installation-from-aur)
    * [Usage](#Usage)
    * [Tips](#Tips)
    * [Contributing](#Contributing)
 <!--te-->
 
 ---
 
@@ -109,14 +110,18 @@
 - Arch: `pacman -S grep coreutils util-linux progress`
 - Fedora: `dnf install grep coreutils util-linux progress`
 
 #### :arrow_right: Installation from pip
 
 `python3 -m pip install recoverpy`
 
+#### :arrow_right: Installation from AUR
+
+`yay -S python-recoverpy`
+
 ## Usage
 
 ```bash
 python3 -m recoverpy
 ```
 
 :red_circle: **You must be root or use sudo**.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: recoverpy Version: 2.0.5 Summary: A TUI to recover
+Metadata-Version: 2.1 Name: recoverpy Version: 2.0.6 Summary: A TUI to recover
 overwritten or deleted data. Home-page: https://github.com/PabloLec/recoverpy
 License: GPL-3.0 License Keywords:
 data,recovery,search,cli,console,cui,tui,ncurses,terminal,cybersec,cybersecurity,security,pentesting,pentest,forensics,forensic,hack,hacking,data
 recovery,data recovery
 tool,grep,linux,unix,education,teaching,training,teach,learn,textual,asyncio,async
 Author: PabloLec Author-email: pablolec@pm.me Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
@@ -19,52 +19,54 @@
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Security
 Classifier: Topic :: System :: Archiving :: Backup Classifier: Topic :: System
 :: Filesystems Classifier: Topic :: System :: Recovery Tools Classifier: Topic
 :: System :: Shells Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Terminals Classifier: Topic :: Utilities Classifier:
-Typing :: Typed Requires-Dist: textual (>=0.17.1,<0.18.0) Project-URL:
+Typing :: Typed Requires-Dist: textual (>=0.17.1,<0.23.0) Project-URL:
 Documentation, https://github.com/PabloLec/recoverpy#readme Project-URL:
 Repository, https://github.com/PabloLec/recoverpy Description-Content-Type:
 text/markdown
                                   [RecoverPy]
                      Recover overwritten or deleted data.
                     [Release] [License] [Downloads] [Tests]
 ---  * [Demo](#Demo) * [Installation](#Installation) * [Dependancies]
 (#arrow_right-dependancies) * [Installation from pip](#arrow_right-
-installation-from-pip) * [Usage](#Usage) * [Tips](#Tips) * [Contributing]
-(#Contributing)  --- # RecoverPy RecoverPy is a powerful tool that leverages
-your system capabilities to recover lost files. Unlike others, you can not only
-recover deleted files but also **overwritten** data. Every block of your
-partition will be scanned. You can even find a string in binary files. ## Demo
+installation-from-pip) * [Installation from AUR](#arrow_right-installation-
+from-aur) * [Usage](#Usage) * [Tips](#Tips) * [Contributing](#Contributing)  --
+- # RecoverPy RecoverPy is a powerful tool that leverages your system
+capabilities to recover lost files. Unlike others, you can not only recover
+deleted files but also **overwritten** data. Every block of your partition will
+be scanned. You can even find a string in binary files. ## Demo
                             [docs/assets/demo.gif]
 ## Installation :penguin: RecoverPy is currently only available on Linux
 systems. #### :arrow_right: Dependancies **Mandatory:** To list and search
 through your partitions, recoverpy uses `grep`, `dd`, and `lsblk` commands.
 Although, if you're running a major Linux distrucition these tools should
 already be installed. **Optional:** To display real time grep progress, you can
 install `progress`. To install all dependencies: - Debian-like: `apt install
 grep coreutils util-linux progress` - Arch: `pacman -S grep coreutils util-
 linux progress` - Fedora: `dnf install grep coreutils util-linux progress` ####
-:arrow_right: Installation from pip `python3 -m pip install recoverpy` ## Usage
-```bash python3 -m recoverpy ``` :red_circle: **You must be root or use sudo**.
---- :one: **Select the system partition** in which your file was. If you are
-out of luck, you can alternatively search in your home partition, maybe your
-IDE, text editor, etc. made a backup at some point. :two: **Type a text string
-to search**. See tips below for better results. :three: **Start search**,
-Results will appear in the left-hand box. :four: **Select a result**. :five:
-Once you have found your precious, **select `Open`**. :six: You can now either
-save this block individually or explore neighboring blocks for the remaining
-parts of the file. You could then save it all in one file. ## Tips - Always do
-backups! Yes, maybe too late... - **Unmount your partition before you do
-anything!** Although you can search with your partition still mounted, it is
-highly recommended to unmount your partition to avoid any alteration to your
-file. Regarding the searched string: - Be concise, find something that could be
-unique to your file. - Stay simple, your string is escaped but exotic
-characters may affect your results. - Try to remember the last edit you have
-made to your file. When you have found your file: - You might see multiple
-results. Your system often use different partion blocks to save successive
-versions of a file. Make sure you've found the last version. - Try exploring
-neighboring blocks to be sure to save your whole file. ## Contributing Thank
-you for considering contributing to RecoverPy. Any request, bug report or PR
-are welcome. Please read the [contributing guide](CONTRIBUTING.md).
+:arrow_right: Installation from pip `python3 -m pip install recoverpy` #### :
+arrow_right: Installation from AUR `yay -S python-recoverpy` ## Usage ```bash
+python3 -m recoverpy ``` :red_circle: **You must be root or use sudo**. --- :
+one: **Select the system partition** in which your file was. If you are out of
+luck, you can alternatively search in your home partition, maybe your IDE, text
+editor, etc. made a backup at some point. :two: **Type a text string to
+search**. See tips below for better results. :three: **Start search**, Results
+will appear in the left-hand box. :four: **Select a result**. :five: Once you
+have found your precious, **select `Open`**. :six: You can now either save this
+block individually or explore neighboring blocks for the remaining parts of the
+file. You could then save it all in one file. ## Tips - Always do backups! Yes,
+maybe too late... - **Unmount your partition before you do anything!** Although
+you can search with your partition still mounted, it is highly recommended to
+unmount your partition to avoid any alteration to your file. Regarding the
+searched string: - Be concise, find something that could be unique to your
+file. - Stay simple, your string is escaped but exotic characters may affect
+your results. - Try to remember the last edit you have made to your file. When
+you have found your file: - You might see multiple results. Your system often
+use different partion blocks to save successive versions of a file. Make sure
+you've found the last version. - Try exploring neighboring blocks to be sure to
+save your whole file. ## Contributing Thank you for considering contributing to
+RecoverPy. Any request, bug report or PR are welcome. Please read the
+[contributing guide](CONTRIBUTING.md).
```

