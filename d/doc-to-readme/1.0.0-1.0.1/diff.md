# Comparing `tmp/doc-to-readme-1.0.0.tar.gz` & `tmp/doc-to-readme-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-to-readme-1.0.0.tar", last modified: Tue Apr 25 20:57:11 2023, max compression
+gzip compressed data, was "doc-to-readme-1.0.1.tar", last modified: Fri Apr 28 22:52:11 2023, max compression
```

## Comparing `doc-to-readme-1.0.0.tar` & `doc-to-readme-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,37 @@
-drwxr-xr-x   0 mirjam     (501) staff       (20)        0 2023-04-25 20:57:11.085578 doc-to-readme-1.0.0/
--rw-r--r--   0 mirjam     (501) staff       (20)     1076 2023-04-15 07:22:20.000000 doc-to-readme-1.0.0/LICENSE
--rw-r--r--   0 mirjam     (501) staff       (20)     5073 2023-04-25 20:57:11.085443 doc-to-readme-1.0.0/PKG-INFO
--rw-r--r--   0 mirjam     (501) staff       (20)     3249 2023-04-25 20:39:56.000000 doc-to-readme-1.0.0/README.md
--rw-r--r--   0 mirjam     (501) staff       (20)      670 2023-04-25 20:56:54.000000 doc-to-readme-1.0.0/pyproject.toml
--rw-r--r--   0 mirjam     (501) staff       (20)       38 2023-04-25 20:57:11.085625 doc-to-readme-1.0.0/setup.cfg
-drwxr-xr-x   0 mirjam     (501) staff       (20)        0 2023-04-25 20:57:11.083246 doc-to-readme-1.0.0/src/
-drwxr-xr-x   0 mirjam     (501) staff       (20)        0 2023-04-25 20:57:11.084162 doc-to-readme-1.0.0/src/doc_to_md/
--rw-r--r--   0 mirjam     (501) staff       (20)        0 2023-04-21 22:17:41.000000 doc-to-readme-1.0.0/src/doc_to_md/__init__.py
--rw-r--r--   0 mirjam     (501) staff       (20)     9876 2023-04-25 20:33:39.000000 doc-to-readme-1.0.0/src/doc_to_md/doc_to_md.py
-drwxr-xr-x   0 mirjam     (501) staff       (20)        0 2023-04-25 20:57:11.084972 doc-to-readme-1.0.0/src/doc_to_readme.egg-info/
--rw-r--r--   0 mirjam     (501) staff       (20)     5073 2023-04-25 20:57:11.000000 doc-to-readme-1.0.0/src/doc_to_readme.egg-info/PKG-INFO
--rw-r--r--   0 mirjam     (501) staff       (20)      263 2023-04-25 20:57:11.000000 doc-to-readme-1.0.0/src/doc_to_readme.egg-info/SOURCES.txt
--rw-r--r--   0 mirjam     (501) staff       (20)        1 2023-04-25 20:57:11.000000 doc-to-readme-1.0.0/src/doc_to_readme.egg-info/dependency_links.txt
--rw-r--r--   0 mirjam     (501) staff       (20)       10 2023-04-25 20:57:11.000000 doc-to-readme-1.0.0/src/doc_to_readme.egg-info/top_level.txt
-drwxr-xr-x   0 mirjam     (501) staff       (20)        0 2023-04-25 20:57:11.085105 doc-to-readme-1.0.0/tests/
--rw-r--r--   0 mirjam     (501) staff       (20)     1773 2023-04-21 22:17:41.000000 doc-to-readme-1.0.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.949844 doc-to-readme-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.github/workflows/update_readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.github/workflows/update_readme_github.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/How_to_setup_the_pipelines.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/bitbucket-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/access_token_info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66748 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/cicd_variables.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91432 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/create_project_access_token_medium.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/project_access_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71484 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/repo_variables.png
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.949844 doc-to-readme-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/src/doc_to_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/src/doc_to_md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_md/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/src/doc_to_md/doc_to_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/templates/.update_readme_gitlab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/tests/classes_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/tests/functions_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/tests/test.py
```

### Comparing `doc-to-readme-1.0.0/LICENSE` & `doc-to-readme-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.0/PKG-INFO` & `doc-to-readme-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-to-readme
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automated Python Module Documentation in Markdown File (README)
 Author-email: Mirjam Ziselsberger <ziselsberger@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mirjam Ziselsberger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,20 +46,24 @@
 
 ### How?
 
 [doc_to_md.py](src/doc_to_md/doc_to_md.py) loops through all Python files in the Repository and extracts the function calls + the
 corresponding short description from the docstrings. These are added to a dictionary and afterwards converted to
 a Markdown Table. Finally, the section **_Functions & Classes_** is appended / updated in the README File.
 
-### Install & Use Python Package
+> There are several options how to use it:  
+> a) [Python Package](#a-install--use-python-package)   
+> b) [CI Pipeline](#b-add-to-pipeline-github-gitlab-or-bitbucket)  
 
-Currently available on [TestPyPI](https://test.pypi.org/project/doc-to-markdown-mz/).
- 
+
+### a) install & use Python Package
+
+Available on [PyPI](https://pypi.org/project/doc-to-readme/1.0.0/)
 ```shell
-pip install -i https://test.pypi.org/simple/ doc-to-markdown-mz
+pip install doc-to-readme
 ```
 
 - **Use within Python** 
 ```python
 import doc_to_md.doc_to_md as dtm
 
 dtm.update_markdown_file(
@@ -79,32 +83,33 @@
 -e EXCLUDE_MODULES      # List of modules to be excluded
 -s SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
-### Add to Pipeline (GitHub, GitLab or Bitbucket)
+### b) add to Pipeline (GitHub, GitLab or Bitbucket)
 _[Documentation](./How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
 
 > ### [**_Step-by-step guide_**](https://github.com/ziselsberger/use_doc_to_readme) on how to integrate _doc_to_readme_ in your Repository
 
 ---
 
 _Copyright &copy; 2023 by Mirjam Ziselsberger_  
 _This code is free to use under the terms of the [MIT license](/LICENSE)._
 
 ## Functions & Classes  
-### [doc_to_md](./src/doc_to_md/doc_to_md.py)
+
+### [doc_to_md.py](./src/doc_to_md/doc_to_md.py)
 
 | Type | Name/Call | Description |
 | --- | --- | --- |
-| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Tuple[str, ...] = (), specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
+| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
 | function  | `add_summary_to_md(overview_dict: Dict[str, Optional[Union[str, Dict[str, str]]]], markdown: str, separate: bool = True)` | Add Table with all Functions & Classes to Markdown file. |
-| function  | `update_markdown_file(file: str = "../README.md", root_dir: str = None, exclude_modules: Tuple[str, ...] = (), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
+| function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
 | function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-25
+**Last Update:** 2023-04-28
```

### Comparing `doc-to-readme-1.0.0/README.md` & `doc-to-readme-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 
 ### How?
 
 [doc_to_md.py](src/doc_to_md/doc_to_md.py) loops through all Python files in the Repository and extracts the function calls + the
 corresponding short description from the docstrings. These are added to a dictionary and afterwards converted to
 a Markdown Table. Finally, the section **_Functions & Classes_** is appended / updated in the README File.
 
-### Install & Use Python Package
+> There are several options how to use it:  
+> a) [Python Package](#a-install--use-python-package)   
+> b) [CI Pipeline](#b-add-to-pipeline-github-gitlab-or-bitbucket)  
 
-Currently available on [TestPyPI](https://test.pypi.org/project/doc-to-markdown-mz/).
- 
+
+### a) install & use Python Package
+
+Available on [PyPI](https://pypi.org/project/doc-to-readme/1.0.0/)
 ```shell
-pip install -i https://test.pypi.org/simple/ doc-to-markdown-mz
+pip install doc-to-readme
 ```
 
 - **Use within Python** 
 ```python
 import doc_to_md.doc_to_md as dtm
 
 dtm.update_markdown_file(
@@ -43,32 +47,33 @@
 -e EXCLUDE_MODULES      # List of modules to be excluded
 -s SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
-### Add to Pipeline (GitHub, GitLab or Bitbucket)
+### b) add to Pipeline (GitHub, GitLab or Bitbucket)
 _[Documentation](./How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
 
 > ### [**_Step-by-step guide_**](https://github.com/ziselsberger/use_doc_to_readme) on how to integrate _doc_to_readme_ in your Repository
 
 ---
 
 _Copyright &copy; 2023 by Mirjam Ziselsberger_  
 _This code is free to use under the terms of the [MIT license](/LICENSE)._
 
 ## Functions & Classes  
-### [doc_to_md](./src/doc_to_md/doc_to_md.py)
+
+### [doc_to_md.py](./src/doc_to_md/doc_to_md.py)
 
 | Type | Name/Call | Description |
 | --- | --- | --- |
-| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Tuple[str, ...] = (), specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
+| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
 | function  | `add_summary_to_md(overview_dict: Dict[str, Optional[Union[str, Dict[str, str]]]], markdown: str, separate: bool = True)` | Add Table with all Functions & Classes to Markdown file. |
-| function  | `update_markdown_file(file: str = "../README.md", root_dir: str = None, exclude_modules: Tuple[str, ...] = (), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
+| function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
 | function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-25
+**Last Update:** 2023-04-28
```

### Comparing `doc-to-readme-1.0.0/src/doc_to_md/doc_to_md.py` & `doc-to-readme-1.0.1/src/doc_to_md/doc_to_md.py`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.0/src/doc_to_readme.egg-info/PKG-INFO` & `doc-to-readme-1.0.1/src/doc_to_readme.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-to-readme
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automated Python Module Documentation in Markdown File (README)
 Author-email: Mirjam Ziselsberger <ziselsberger@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mirjam Ziselsberger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,20 +46,24 @@
 
 ### How?
 
 [doc_to_md.py](src/doc_to_md/doc_to_md.py) loops through all Python files in the Repository and extracts the function calls + the
 corresponding short description from the docstrings. These are added to a dictionary and afterwards converted to
 a Markdown Table. Finally, the section **_Functions & Classes_** is appended / updated in the README File.
 
-### Install & Use Python Package
+> There are several options how to use it:  
+> a) [Python Package](#a-install--use-python-package)   
+> b) [CI Pipeline](#b-add-to-pipeline-github-gitlab-or-bitbucket)  
 
-Currently available on [TestPyPI](https://test.pypi.org/project/doc-to-markdown-mz/).
- 
+
+### a) install & use Python Package
+
+Available on [PyPI](https://pypi.org/project/doc-to-readme/1.0.0/)
 ```shell
-pip install -i https://test.pypi.org/simple/ doc-to-markdown-mz
+pip install doc-to-readme
 ```
 
 - **Use within Python** 
 ```python
 import doc_to_md.doc_to_md as dtm
 
 dtm.update_markdown_file(
@@ -79,32 +83,33 @@
 -e EXCLUDE_MODULES      # List of modules to be excluded
 -s SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
-### Add to Pipeline (GitHub, GitLab or Bitbucket)
+### b) add to Pipeline (GitHub, GitLab or Bitbucket)
 _[Documentation](./How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
 
 > ### [**_Step-by-step guide_**](https://github.com/ziselsberger/use_doc_to_readme) on how to integrate _doc_to_readme_ in your Repository
 
 ---
 
 _Copyright &copy; 2023 by Mirjam Ziselsberger_  
 _This code is free to use under the terms of the [MIT license](/LICENSE)._
 
 ## Functions & Classes  
-### [doc_to_md](./src/doc_to_md/doc_to_md.py)
+
+### [doc_to_md.py](./src/doc_to_md/doc_to_md.py)
 
 | Type | Name/Call | Description |
 | --- | --- | --- |
-| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Tuple[str, ...] = (), specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
+| function  | `loop_through_repo(file: str, root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = None, specified_modules: Optional[Tuple[str, ...]] = None) -> None` | Collect documentation from functions & classes |
 | function  | `add_summary_to_md(overview_dict: Dict[str, Optional[Union[str, Dict[str, str]]]], markdown: str, separate: bool = True)` | Add Table with all Functions & Classes to Markdown file. |
-| function  | `update_markdown_file(file: str = "../README.md", root_dir: str = None, exclude_modules: Tuple[str, ...] = (), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
+| function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
 | function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-25
+**Last Update:** 2023-04-28
```

### Comparing `doc-to-readme-1.0.0/tests/test.py` & `doc-to-readme-1.0.1/tests/test.py`

 * *Files identical despite different names*

