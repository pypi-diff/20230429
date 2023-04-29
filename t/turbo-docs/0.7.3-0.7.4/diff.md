# Comparing `tmp/turbo_docs-0.7.3.tar.gz` & `tmp/turbo_docs-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.7.3.tar", last modified: Sat Apr 22 22:59:11 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.7.4.tar", last modified: Sat Apr 29 00:24:12 2023, max compression
```

## Comparing `turbo_docs-0.7.3.tar` & `turbo_docs-0.7.4.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.092223 turbo_docs-0.7.3/
--rw-rw-rw-   0        0        0     2010 2023-04-22 22:59:11.091223 turbo_docs-0.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2023-04-22 21:44:40.000000 turbo_docs-0.7.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-22 22:59:11.092223 turbo_docs-0.7.3/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-04-22 22:58:57.000000 turbo_docs-0.7.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.065692 turbo_docs-0.7.3/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.3/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.084221 turbo_docs-0.7.3/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-22 22:02:08.000000 turbo_docs-0.7.3/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2078 2023-04-22 21:34:48.000000 turbo_docs-0.7.3/turbo_docs/commands/commit.py
--rw-rw-rw-   0        0        0     2162 2023-04-22 21:34:03.000000 turbo_docs-0.7.3/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0     1590 2023-04-22 21:33:13.000000 turbo_docs-0.7.3/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1133 2023-04-22 21:31:48.000000 turbo_docs-0.7.3/turbo_docs/commands/unit_tests.py
--rw-rw-rw-   0        0        0     1993 2023-04-22 22:58:45.000000 turbo_docs-0.7.3/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.089219 turbo_docs-0.7.3/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.3/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0     1820 2023-04-22 21:27:40.000000 turbo_docs-0.7.3/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1928 2023-04-22 21:27:45.000000 turbo_docs-0.7.3/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1415 2023-04-22 21:35:25.000000 turbo_docs-0.7.3/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-04-22 22:59:11.074707 turbo_docs-0.7.3/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2010 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-04-22 22:59:11.000000 turbo_docs-0.7.3/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-22 22:59:10.000000 turbo_docs-0.7.3/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.801364 turbo_docs-0.7.4/
+-rw-rw-rw-   0        0        0     1199 2023-04-29 00:24:12.801364 turbo_docs-0.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0      743 2023-04-29 00:23:36.000000 turbo_docs-0.7.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 00:24:12.802474 turbo_docs-0.7.4/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-04-29 00:16:43.000000 turbo_docs-0.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.777153 turbo_docs-0.7.4/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.4/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.791747 turbo_docs-0.7.4/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-22 22:02:08.000000 turbo_docs-0.7.4/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2163 2023-04-28 23:59:47.000000 turbo_docs-0.7.4/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0     1669 2023-04-29 00:14:51.000000 turbo_docs-0.7.4/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1221 2023-04-29 00:15:18.000000 turbo_docs-0.7.4/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.799356 turbo_docs-0.7.4/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.7.4/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1222 2023-04-29 00:15:09.000000 turbo_docs-0.7.4/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1871 2023-04-29 00:15:05.000000 turbo_docs-0.7.4/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1467 2023-04-29 00:08:47.000000 turbo_docs-0.7.4/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-04-29 00:24:12.787229 turbo_docs-0.7.4/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     1199 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-29 00:24:12.000000 turbo_docs-0.7.4/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.7.3/setup.py` & `turbo_docs-0.7.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.7.3",
+	version="0.7.4",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.7.3/turbo_docs/commands/docstring.py` & `turbo_docs-0.7.4/turbo_docs/commands/docstring.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from redbaron import RedBaron
 import textwrap
 from turbo_docs.utils import openai_api
 
 
 def wrap_text(text):
     """
-    Wrap a given string of text to 80 characters
+    Wrap text to 80 chars and break long words.
     """
     line_length = 80
 
     # wrap text to 80 chars
     text = " ".join(text.split("\n"))
     wrapped_text = '\n'.join(textwrap.wrap(
         text, line_length, break_long_words=False))
 
     return wrapped_text
 
 
 def format_docstring(s):
     """
-    Apply specific formatting to docstring
+    Formats a docstring to adhere to PEP 8.
     """
     if s.startswith('"') or s.startswith('\n'):
         return format_docstring(s[1:])
 
     if s.endswith('"') or s.endswith('\n'):
         return format_docstring(s[:-1])
 
@@ -35,15 +35,15 @@
 
     wrapped_text = wrap_text(s.strip())
     return f'"""\n{wrapped_text}\n"""'
 
 
 def docstring(files):
     """
-    Generate docstrings for Python functions in specified files using OpenAI API.
+    Generate a docstring for Python functions using a GPT-3 text completion model.
     """
     for file_path, content in files.items():
         if file_path.split(".")[1]:
 
             red = RedBaron(content)
             functions = red.find_all("def")
             if functions:
```

### Comparing `turbo_docs-0.7.3/turbo_docs/commands/readme.py` & `turbo_docs-0.7.4/turbo_docs/commands/readme.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import os
 from turbo_docs.utils import openai_api
 
 
 def readme(text):
     """
-    Generate a formatted & user-friendly README.md using openai API and output it to
-    a README.md file
+    Generate a formatted and user-friendly README.md using openAI API, or use an
+    alternative command if unable to generate.
     """
     readme = "README.md"
     prompt = f"Create a formatted & user-friendly readme.md from the following:\n\n{text}"
     response = openai_api.gpt_completion_error_handler(prompt)
     if response is None:
         print("Unable to generate README.md, try the folling command instead: turbo_docs --readme_large_repo")
     else:
         with open(readme, "w") as readme_file:
             readme_file.write(response)
         print(f"(--readme) Generated README.md")
 
 
-
-
 def readme_large_repo(files):
     """
-    Generate a README.md for larger repositories
+    return flatmap Create a summarization for files, soliciting user input if the
+    summary is satisfactory.
     """
     responses = {}
     for file_path, file_content in files.items():
         if os.stat(file_path).st_size and file_path.split(".")[1]:
             print(f"(--readme_large_repo) Summarizing {file_path}")
             prompt = f"Condense the following information, minimize the amount of tokens used and maximize the preservation of information:\n{file_content}"
             responses[file_path] = openai_api.gpt_completion_wrapper(prompt)
     flatmap = "\n\n\n".join([f"{file_path}:\n{summary}" for file_path, summary in responses.items()])
-    
+
     user_acceptance = False
     while not user_acceptance:
         readme(flatmap)
         resp = input("(--readme_plus) Check your README.md, want to generate a new one? (Y/n):")
         if resp != "y" and resp != "Y":
-            user_acceptance = True
+            user_acceptance = True
```

### Comparing `turbo_docs-0.7.3/turbo_docs/utils/directory.py` & `turbo_docs-0.7.4/turbo_docs/utils/directory.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,53 +2,51 @@
 import os
 from pathlib import Path
 from typing import List, Dict
 
 
 def ignored_files_init() -> List[str]:
     """
-    Initializes a list of ignored files from current directory.
+    Initialize a list of files to be ignored in directory.
     """
     ignored_files = ["README.md", "tests", "setup.py"]
     for file in os.listdir():
         if file[0] == ".":
             ignored_files.append(file)
     return ignored_files
 
 
 def read_gitignore() -> List[str]:
     """
-    Read '.gitignore' file and return a list of files to be excluded from
-    documentation generation.
+    Reads in a .gitignore file and returns a list of ignored files.
     """
     ignore_files = ignored_files_init()
     try:
         with open(".gitignore", "r") as gitignore:
             for line in gitignore:
                 ignore_files.append(line.strip())
     except FileNotFoundError:
         raise ValueError(
             ".gitignore file required for excluding files from documentation generation")
     return ignore_files
 
 
 def ignore_filepath(filepath: str, ignore_files: List[str]) -> bool:
     """
-    Check a file path to see if it should be ignored
+    Check if the given filepath contains any of the given ignored files.
     """
     for part in Path(filepath).parts:
         if part in ignore_files:
             return True
     return False
 
 
 def get_files() -> Dict:
     """
-    Retrieve and return all files in the working directory, ignoring those specified
-    in the .gitignore file.
+    Retrieve all text from files, excluding filepaths specified by .gitignore.
     """
     files_dict = {}
     ignore_files = read_gitignore()
 
     # Iterate over files
     for root, _, files in os.walk("."):
         for file in files:
```

### Comparing `turbo_docs-0.7.3/turbo_docs/utils/openai_api.py` & `turbo_docs-0.7.4/turbo_docs/utils/openai_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import json
 import os
 
 
 def openai_init():
     """
-    Initialize OpenAI API with API key, prompt user for key if not set
+    Initialize the OpenAI API and prompt the user for their API key if it is not
+    stored as an environment variable.
     """
     import openai
     openai.api_key = os.environ.get('OPENAI_API_KEY')
 
     if not openai.api_key:
         print("OpenAI API key is not set. Please set it as an environment variable (export OPENAI_API_KEY=<your_api_key>) or enter it below.")
         print("If you have not done so already, create an OpenAI account at https://platform.openai.com/overview.")
         openai.api_key = input("Secret key:")
     return openai
 
 
 def gpt_completion_wrapper(prompt, openai_package=None):
     """
-    Wrapper for OpenAI's GPT-3 completions using Text-Davinci-003 engine.
+    Provide GPT-3 completions for a given prompt and optional OpenAI package.
     """
     if not openai_package:
         openai_package = openai_init()
 
     completions = openai_package.Completion.create(
         engine="text-davinci-003",
         prompt=prompt,
@@ -31,15 +32,15 @@
         stop=None,
     )
     return completions.choices[0]['text'].strip()
 
 
 def gpt_completion_error_handler(prompt):
     """
-    Handle OpenAI API errors for GPT completion requests
+    Handle errors raised by OpenAI GPT completion API.
     """
     text = None
     openai_package = openai_init()
 
     try:
         text = gpt_completion_wrapper(prompt, openai_package=openai_package)
     except openai_package.error.InvalidRequestError as e:
```

