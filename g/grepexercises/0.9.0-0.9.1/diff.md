# Comparing `tmp/grepexercises-0.9.0.tar.gz` & `tmp/grepexercises-0.9.1.tar.gz`

## Comparing `grepexercises-0.9.0.tar` & `grepexercises-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/__init__.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/app_guide.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/grep_exercises.css
--rw-r--r--   0        0        0     9798 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/grep_exercises.py
--rw-r--r--   0        0        0    33047 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/questions.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/user_progress.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/.hidden
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/code.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/colors_1
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/colors_2.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/lines.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/nul_separated
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/patterns.txt
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/pcre.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/regex_terms.txt
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/sample.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/substitute.sh
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/terms.txt
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/backups/color list.txt
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/backups/dot_files/.bash_aliases
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/backups/dot_files/.inputrc
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/projects/python/hello.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-0.9.0/src/grepexercises/sample_input/projects/shell/hello.sh
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grepexercises-0.9.0/LICENSE
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 grepexercises-0.9.0/README.md
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 grepexercises-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 grepexercises-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/__init__.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/app_guide.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/grep_exercises.css
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/grep_exercises.py
+-rw-r--r--   0        0        0    33047 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/questions.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/user_progress.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/.hidden
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/code.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/colors_1
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/colors_2.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/lines.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/nul_separated
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/patterns.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/pcre.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/regex_terms.txt
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/sample.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/substitute.sh
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/terms.txt
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/backups/color list.txt
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/backups/dot_files/.bash_aliases
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/backups/dot_files/.inputrc
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/projects/python/hello.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 grepexercises-0.9.1/src/grepexercises/sample_input/projects/shell/hello.sh
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 grepexercises-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 grepexercises-0.9.1/README.md
+-rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 grepexercises-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 grepexercises-0.9.1/PKG-INFO
```

### Comparing `grepexercises-0.9.0/src/grepexercises/app_guide.md` & `grepexercises-0.9.1/src/grepexercises/app_guide.md`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.0/src/grepexercises/grep_exercises.css` & `grepexercises-0.9.1/src/grepexercises/grep_exercises.css`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.0/src/grepexercises/grep_exercises.py` & `grepexercises-0.9.1/src/grepexercises/grep_exercises.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,24 @@
         ('ctrl+t', 'toggle_theme', 'Theme'),
         ('ctrl+q', 'app.quit', 'Quit'),
     ]
 
     def __init__(self):
         super().__init__()
 
+        Path('backups/text').mkdir(exist_ok=True)
         links = [Path('hello.py'), Path('backups/text/pat.txt')]
         targets = [Path('projects/python/hello.py'), Path('../../patterns.txt')]
         for link, target in zip(links, targets):
             if not link.is_file():
                 link.symlink_to(target)
+        for path in Path('.').rglob('*.pyc'):
+            path.unlink()
+        for path in Path('.').rglob('__pycache__'):
+            path.rmdir()
 
         self.l_question = Label(id='question')
         with open(SCRIPT_DIR.joinpath('questions.json'), encoding='ascii') as f:
             self.questions = tuple(json.load(f).values())
         self.q_idx = 0
         self.q_max_idx = len(self.questions) - 1
```

### Comparing `grepexercises-0.9.0/src/grepexercises/questions.json` & `grepexercises-0.9.1/src/grepexercises/questions.json`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.0/src/grepexercises/sample_input/patterns.txt` & `grepexercises-0.9.1/src/grepexercises/sample_input/patterns.txt`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.0/LICENSE` & `grepexercises-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.0/README.md` & `grepexercises-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `grepexercises-0.9.0/pyproject.toml` & `grepexercises-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "grepexercises"
-version = "0.9.0"
+version = "0.9.1"
 authors = [
   { name="Sundeep Agarwal", email="learnbyexample.net@gmail.com" },
 ]
 description = "50+ exercises for GNU grep (or alternatives like ripgrep)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `grepexercises-0.9.0/PKG-INFO` & `grepexercises-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepexercises
-Version: 0.9.0
+Version: 0.9.1
 Summary: 50+ exercises for GNU grep (or alternatives like ripgrep)
 Project-URL: Source, https://github.com/learnbyexample/TUI-apps/tree/main/GrepExercises
 Project-URL: Issues, https://github.com/learnbyexample/TUI-apps/issues
 Author-email: Sundeep Agarwal <learnbyexample.net@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

