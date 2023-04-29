# Comparing `tmp/golem_garden-0.5.1.tar.gz` & `tmp/golem_garden-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_garden-0.5.1.tar", last modified: Thu Apr 27 16:55:40 2023, max compression
+gzip compressed data, was "golem_garden-0.5.2.tar", last modified: Sat Apr 29 14:42:32 2023, max compression
```

## Comparing `golem_garden-0.5.1.tar` & `golem_garden-0.5.2.tar`

### file list

```diff
@@ -1,50 +1,52 @@
--rw-r--r--   0        0        0      834 2023-04-27 16:55:31.633318 golem_garden-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-04-27 16:55:31.633318 golem_garden-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-27 16:55:31.633318 golem_garden-0.5.1/.github/workflows/deploy_docs.yml
--rw-r--r--   0        0        0     1142 2023-04-27 16:55:31.633318 golem_garden-0.5.1/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1883 2023-04-27 16:55:31.633318 golem_garden-0.5.1/.gitignore
--rw-r--r--   0        0        0     3348 2023-04-27 16:55:31.633318 golem_garden-0.5.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-04-27 16:55:31.633318 golem_garden-0.5.1/LICENSE
--rw-r--r--   0        0        0      178 2023-04-27 16:55:31.633318 golem_garden-0.5.1/README.md
--rw-r--r--   0        0        0       79 2023-04-27 16:55:31.633318 golem_garden-0.5.1/RUN_ME.py
--rw-r--r--   0        0        0       14 2023-04-27 16:55:31.633318 golem_garden-0.5.1/docs/development/contributing.md
--rw-r--r--   0        0        0     2359 2023-04-27 16:55:31.633318 golem_garden-0.5.1/docs/development/style_guide.md
--rw-r--r--   0        0        0     2396 2023-04-27 16:55:31.633318 golem_garden-0.5.1/docs/development/style_guide_for_gpt.md
--rw-r--r--   0        0        0     1306 2023-04-27 16:55:31.633318 golem_garden-0.5.1/docs/index.md
--rw-r--r--   0        0        0      251 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/__init__.py
--rw-r--r--   0        0        0      910 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/__main__.py
--rw-r--r--   0        0        0        0 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/data_loaders/__init__.py
--rw-r--r--   0        0        0      996 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/data_loaders/async_load_url_with_playwright.py
--rw-r--r--   0        0        0        0 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/golems/__init__.py
--rw-r--r--   0        0        0     2124 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/golems/golem.py
--rw-r--r--   0        0        0        0 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/output_parsers/__init__.py
--rw-r--r--   0        0        0     1186 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/output_parsers/output_parser.py
--rw-r--r--   0        0        0        0 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/prompts/__init__.py
--rw-r--r--   0        0        0     1777 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/prompts/prompts.py
--rw-r--r--   0        0        0        0 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/tools/__init__.py
--rw-r--r--   0        0        0     3378 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/tools/directory_printer.py
--rw-r--r--   0        0        0     5029 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/tools/grab_all_py_in_one_text_block.py
--rw-r--r--   0        0        0      484 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
--rw-r--r--   0        0        0     3686 2023-04-27 16:55:31.633318 golem_garden-0.5.1/golem_garden/tools/tools.py
--rw-r--r--   0        0        0    29940 2023-04-27 16:55:31.633318 golem_garden-0.5.1/jupyter_notebooks/ask_freemocap_docs.ipynb
--rw-r--r--   0        0        0     8092 2023-04-27 16:55:31.633318 golem_garden-0.5.1/jupyter_notebooks/dog_mailer_auto_gpt.py
--rw-r--r--   0        0        0    20524 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
--rw-r--r--   0        0        0     3912 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_agent_playground.py
--rw-r--r--   0        0        0    26686 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/autogpt.ipynb
--rw-r--r--   0        0        0    31113 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
--rw-r--r--   0        0        0    60363 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
--rw-r--r--   0        0        0    44476 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
--rw-r--r--   0        0        0    23377 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
--rw-r--r--   0        0        0      882 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
--rw-r--r--   0        0        0    18760 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
--rw-r--r--   0        0        0    60951 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/marathon_times.ipynb
--rw-r--r--   0        0        0    23334 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
--rw-r--r--   0        0        0    25052 2023-04-27 16:55:31.637318 golem_garden-0.5.1/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
--rw-r--r--   0        0        0      398 2023-04-27 16:55:31.637318 golem_garden-0.5.1/mkdocs.yml
--rw-r--r--   0        0        0      356 2023-04-27 16:55:31.637318 golem_garden-0.5.1/notes/bluesky_todos.md
--rw-r--r--   0        0        0     1214 2023-04-27 16:55:31.637318 golem_garden-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      127 2023-04-27 16:55:31.637318 golem_garden-0.5.1/sample.env
--rw-r--r--   0        0        0       99 2023-04-27 16:55:31.637318 golem_garden-0.5.1/utilities/env_setup.bat
--rw-r--r--   0        0        0     2280 2023-04-27 16:55:31.637318 golem_garden-0.5.1/utilities/pinecone.py
--rw-r--r--   0        0        0      507 2023-04-27 16:55:31.637318 golem_garden-0.5.1/utilities/try_mongo_connection.py
--rw-r--r--   0        0        0     1082 1970-01-01 00:00:00.000000 golem_garden-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      834 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/workflows/deploy_docs.yml
+-rw-r--r--   0        0        0     1123 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1883 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.gitignore
+-rw-r--r--   0        0        0     3348 2023-04-29 14:42:26.024752 golem_garden-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-04-29 14:42:26.024752 golem_garden-0.5.2/LICENSE
+-rw-r--r--   0        0        0      190 2023-04-29 14:42:26.024752 golem_garden-0.5.2/README.md
+-rw-r--r--   0        0        0       79 2023-04-29 14:42:26.024752 golem_garden-0.5.2/RUN_ME.py
+-rw-r--r--   0        0        0     1640 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/Community Guidelines/Code of Conduct.md
+-rw-r--r--   0        0        0     3511 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/Contributing guide/Contributing.md
+-rw-r--r--   0        0        0     2790 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/Contributing guide/python_style_guide.md
+-rw-r--r--   0        0        0      190 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/index.md
+-rw-r--r--   0        0        0     2485 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      251 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/__init__.py
+-rw-r--r--   0        0        0      910 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/data_loaders/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/data_loaders/async_load_url_with_playwright.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/golems/__init__.py
+-rw-r--r--   0        0        0     2125 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/golems/golem.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1186 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/output_parsers/output_parser.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/prompts/__init__.py
+-rw-r--r--   0        0        0     1777 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/prompts/prompts.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/__init__.py
+-rw-r--r--   0        0        0     3378 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/directory_printer.py
+-rw-r--r--   0        0        0     5029 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/grab_all_py_in_one_text_block.py
+-rw-r--r--   0        0        0      484 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
+-rw-r--r--   0        0        0     3686 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/tools.py
+-rw-r--r--   0        0        0    29940 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/ask_freemocap_docs.ipynb
+-rw-r--r--   0        0        0     8092 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/dog_mailer_auto_gpt.py
+-rw-r--r--   0        0        0    20524 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0     3890 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/langchain_agent_playground.py
+-rw-r--r--   0        0        0    26686 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/autogpt.ipynb
+-rw-r--r--   0        0        0    31113 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
+-rw-r--r--   0        0        0    18274 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb
+-rw-r--r--   0        0        0    60363 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
+-rw-r--r--   0        0        0    44476 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
+-rw-r--r--   0        0        0    23377 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0      882 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
+-rw-r--r--   0        0        0    18760 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
+-rw-r--r--   0        0        0    60951 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/marathon_times.ipynb
+-rw-r--r--   0        0        0    23334 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
+-rw-r--r--   0        0        0    25052 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
+-rw-r--r--   0        0        0      123 2023-04-29 14:42:26.032752 golem_garden-0.5.2/mkdocs.yml
+-rw-r--r--   0        0        0      356 2023-04-29 14:42:26.032752 golem_garden-0.5.2/notes/bluesky_todos.md
+-rw-r--r--   0        0        0     1296 2023-04-29 14:42:26.032752 golem_garden-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-04-29 14:42:26.032752 golem_garden-0.5.2/sample.env
+-rw-r--r--   0        0        0       99 2023-04-29 14:42:26.032752 golem_garden-0.5.2/utilities/env_setup.bat
+-rw-r--r--   0        0        0     2280 2023-04-29 14:42:26.032752 golem_garden-0.5.2/utilities/pinecone.py
+-rw-r--r--   0        0        0      507 2023-04-29 14:42:26.032752 golem_garden-0.5.2/utilities/try_mongo_connection.py
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 golem_garden-0.5.2/PKG-INFO
```

### Comparing `golem_garden-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `golem_garden-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `golem_garden-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/.github/workflows/deploy_docs.yml` & `golem_garden-0.5.2/.github/workflows/deploy_docs.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `golem_garden-0.5.2/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files 9% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 # separate terms of service, privacy policy, and support
 # documentation.
 
 name: Upload Python Package
 
 on:
   push:
-    branches: [ main ]
     tags: [ v* ]
 
 permissions:
   contents: read
 
 jobs:
   deploy:
-
+    
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v3
         with:
```

### Comparing `golem_garden-0.5.1/.gitignore` & `golem_garden-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/CONTRIBUTING.md` & `golem_garden-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/LICENSE` & `golem_garden-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/docs/development/style_guide.md` & `golem_garden-0.5.2/docs/Contributing guide/python_style_guide.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,51 @@
-# Golem Garden Style Guide
-
-This style guide aims to maintain code readability, quality, and maintainability in the Golem Garden project. It
-incorporates best practices and focuses on a "universal design" approach to make the code understandable to both experts
-and non-experts.
-
-## General Guidelines
-
-1. **Include Google-formatted docstrings**: Use Google-style docstrings for functions, methods, and classes to provide
-   clear and concise documentation.
-
-2. **Type hints**: Use input and return type hints for functions and methods to improve code readability and facilitate
-   better tooling support.
-
-3. **Keyword arguments**: Prefer using keyword arguments over simple arguments for functions and methods to improve code
-   clarity.
-
-4. **Private methods and attributes**: Use leading underscores to denote private methods and attributes in classes, and
-   use `@property` decorators when appropriate.
-
-5. **Descriptive names**: Use full words in variable and class names instead of abbreviations (e.g., `database` instead
-   of `db`).
-
-6. **PEP8 and `black` formatting**: Follow PEP8 and `black` code formatting guidelines to maintain consistency and
-   readability.
-
-7. **Consistent naming conventions**: Adopt consistent naming conventions for variables, functions, and classes.
-    - Use `snake_case` for variables and functions (e.g., `my_variable`, `my_function`)
-    - Use `PascalCase` for class names (e.g., `MyClass`)
-    - Use `UPPERCASE` for constants (e.g., `MY_CONSTANT`)
-
-8. **Keep functions and methods short**: Aim to keep functions and methods concise, ideally not exceeding 15-20 lines of
-   code.
-
-9. **Modularize code**: Organize code into modules and packages to maintain a clean and organized codebase.
-
-10. **Minimal comments**: Avoid comments if possible. Write code that is simple and descriptive enough that comments are
-    not necessary. If needed, use comments sparingly to provide context or explain complex or non-obvious sections of
-    your code.
-
-11. **Error handling**: Use appropriate error handling techniques, such as `try` and `except` blocks, to handle
-    exceptions and provide meaningful error messages to users.
-
-12. **Write tests**: Write unit tests to ensure the correct functioning of your code.
-
-13. **Code reviews**: Perform code reviews with team members or peers to maintain a high-quality codebase.
 
+  
+This style guide aims to maintain code readability, quality, and maintainability. 
+  
+## General Guidelines  
+
+- Follow a [Universal Design](https://99percentinvisible.org/episode/curb-cuts/) approach that aspires to be interpretable to the widest possible number of people 
+- Follow standard best practices, e.g  [S.O.L.I.D](https://realpython.com/preview/solid-principles-python/) etc
+- Follow  [PEP 8 Guidelines](https://peps.python.org/pep-0008/)
+- Use  [Black](https://black.readthedocs.io/en/stable/) to auto-format your code
+
+
+## Specific Guidelines
+
+```
+TO DO - Add code samples for each guideline (along with links to external references when applicable)
+```
+  
+1. **Include Google-formatted docstrings**: Use Google-style docstrings for functions, methods, and classes to provide  
+   clear and concise documentation.  
+  
+2. **Type hints**: Use input and return type hints for functions and methods to improve code readability and facilitate  
+   better tooling support.  
+  
+3. **Keyword arguments**: Prefer using keyword arguments over simple arguments for functions and methods to improve code  
+   clarity.  
+  
+4. **Private methods and attributes**: Use leading underscores to denote private methods and attributes in classes, and  
+   use `@property` decorators when appropriate.  
+  
+5. **Descriptive names**: Use full words in variable and class names instead of abbreviations (e.g., `database` instead   of `db`).  
+  
+6. **PEP8 and `black` formatting**: Follow PEP8 and `black` code formatting guidelines to maintain consistency and  readability.  
+  
+7. **Consistent naming conventions**: Adopt consistent naming conventions for variables, functions, and classes.  
+   - Use `snake_case` for variables and functions (e.g., `my_variable`, `my_function`)  
+   - Use `PascalCase` for class names (e.g., `MyClass`)  
+   - Use `UPPERCASE` for constants (e.g., `MY_CONSTANT`)  
+  
+8. **Keep functions and methods short**: Aim to keep functions and methods concise, ideally not exceeding 15-20 lines of  code.  
+  
+9. **Modularize code**: Organize code into modules and packages to maintain a clean and organized codebase.  
+  
+10. **Minimal comments**: Avoid comments if possible. Write code that is simple and descriptive (See pt 5) enough that comments are  not necessary. If needed, use comments sparingly to provide context or explain complex or non-obvious sections of  your code.  
+  
+11. **Error handling**: Use appropriate error handling techniques, such as `try` and `except` blocks, to handle  
+    exceptions and provide meaningful error messages to users.  
+  
+12. **Write tests**: Write unit tests to ensure the correct functioning of your code.  
+  
+13. **Code reviews**: Perform code reviews with team members or peers to maintain a high-quality codebase.
```

### Comparing `golem_garden-0.5.1/golem_garden/__main__.py` & `golem_garden-0.5.2/golem_garden/__main__.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/golem_garden/data_loaders/async_load_url_with_playwright.py` & `golem_garden-0.5.2/golem_garden/data_loaders/async_load_url_with_playwright.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/golem_garden/golems/golem.py` & `golem_garden-0.5.2/golem_garden/golems/golem.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             Tool(
                 name="Wolfram Alpha",
                 func=self._wolfram_alpha.run,
                 description="useful when you need to answer questions about the world around you."
             )
         ]
         self._memory = ConversationBufferMemory(memory_key="chat_history", return_messages=True)
-        self._llm = ChatOpenAI(temperature=1, model_name="gpt-4")
+        self._llm = ChatOpenAI(temperature=.8, model_name="gpt-4")
         self._chain = initialize_agent(self._tools,
                                        self._llm,
                                        agent=AgentType.CHAT_CONVERSATIONAL_REACT_DESCRIPTION,
                                        verbose=True,
                                        memory=self._memory)
 
     def intake_message(self, message: str):
```

### Comparing `golem_garden-0.5.1/golem_garden/output_parsers/output_parser.py` & `golem_garden-0.5.2/golem_garden/output_parsers/output_parser.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/golem_garden/prompts/prompts.py` & `golem_garden-0.5.2/golem_garden/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/golem_garden/tools/directory_printer.py` & `golem_garden-0.5.2/golem_garden/tools/directory_printer.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/golem_garden/tools/grab_all_py_in_one_text_block.py` & `golem_garden-0.5.2/golem_garden/tools/grab_all_py_in_one_text_block.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/golem_garden/tools/tools.py` & `golem_garden-0.5.2/golem_garden/tools/tools.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/ask_freemocap_docs.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/ask_freemocap_docs.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/dog_mailer_auto_gpt.py` & `golem_garden-0.5.2/jupyter_notebooks/dog_mailer_auto_gpt.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_agent_playground.py` & `golem_garden-0.5.2/jupyter_notebooks/langchain_agent_playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from langchain.embeddings import OpenAIEmbeddings
 from langchain.schema import Document
 from langchain.tools.file_management.read import ReadFileTool
 from langchain.tools.file_management.write import WriteFileTool
 from langchain.tools.human.tool import HumanInputRun
 from langchain.vectorstores import FAISS
 
-from golem_garden.prompts import task_completion_prompt_template, CustomPromptTemplate
-from golem_garden.output_parsers.output_parser import CustomOutputParser
+from golem_garden import task_completion_prompt_template, CustomPromptTemplate
+from golem_garden.output_parsers import CustomOutputParser
 from golem_garden.tools.tools import web_search, process_csv, query_website_tool, get_tools
 
 load_dotenv()
 os.environ["LANGCHAIN_HANDLER"] = "langchain"
```

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/autogpt.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/autogpt.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_playground.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_playground.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/marathon_times.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/marathon_times.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb` & `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/pyproject.toml` & `golem_garden-0.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -18,47 +18,52 @@
 keywords = [
     "chat"
 ]
 
 
 dependencies = [
     "python-dotenv",
-    "openai",
     "toml",
-    "openai",
+    "asyncio",
     "fastapi",
     "uvicorn",
-    "google-search-results",
-    "langchain",
     "rich",
+
+    #langchain et al
+    "langchain",
+    "openai",
+    "google-search-results",
     "wikipedia",
     "wolframalpha",
     "chromadb",
     "pydantic",
     "faiss-cpu",
+
+
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9 , <4"
 
 dynamic = ["version", "description"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/jonmatthis/golem_garden"
 
 [tool.bumpver]
-current_version = "v0.5.1"
+current_version = "v0.5.2"
 
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 
 "golem_garden/__init__.py" = ["{version}"]
 
 [project.scripts]
 golem_garden = "golem_garden.__main__:main"
+golem_discord = "golem_garden.discord_bot:bot_main"
```

### Comparing `golem_garden-0.5.1/utilities/pinecone.py` & `golem_garden-0.5.2/utilities/pinecone.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.1/PKG-INFO` & `golem_garden-0.5.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: golem_garden
-Version: 0.5.1
+Version: 0.5.2
 Summary: Welcome to the Garden - We're so glad you're here <3 
 Keywords: chat
 Author: Jonathan Samir Matthis
-Requires-Python: >=3.8
+Requires-Python: >=3.9 , <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: python-dotenv
-Requires-Dist: openai
 Requires-Dist: toml
-Requires-Dist: openai
+Requires-Dist: asyncio
 Requires-Dist: fastapi
 Requires-Dist: uvicorn
-Requires-Dist: google-search-results
-Requires-Dist: langchain
 Requires-Dist: rich
+Requires-Dist: langchain
+Requires-Dist: openai
+Requires-Dist: google-search-results
 Requires-Dist: wikipedia
 Requires-Dist: wolframalpha
 Requires-Dist: chromadb
 Requires-Dist: pydantic
 Requires-Dist: faiss-cpu
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
@@ -29,16 +29,16 @@
 Project-URL: Homepage, https://github.com/jonmatthis/golem_garden
 Provides-Extra: dev
 
 # Welcome to the Garden 
 
 We're so glad you're here 🌱✨
 
-In a terminal with a Python environment enabled, enter:
+In a terminal with a Python (3.10 or so) environment enabled, enter:
 ```bash
 pip install -e .
 ```
 Then:
 ```bash
-golem_garden`
+golem_garden
 ```
```

