# Comparing `tmp/doc-to-readme-1.0.1.tar.gz` & `tmp/doc-to-readme-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doc-to-readme-1.0.1.tar", last modified: Fri Apr 28 22:52:11 2023, max compression
+gzip compressed data, was "doc-to-readme-1.1.0.tar", last modified: Sat Apr 29 10:17:44 2023, max compression
```

## Comparing `doc-to-readme-1.0.1.tar` & `doc-to-readme-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.949844 doc-to-readme-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.github/workflows/update_readme.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.github/workflows/update_readme_github.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/How_to_setup_the_pipelines.md
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/bitbucket-pipelines.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/images/
--rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/access_token_info.png
--rw-r--r--   0 runner    (1001) docker     (123)    66748 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/cicd_variables.png
--rw-r--r--   0 runner    (1001) docker     (123)    91432 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/create_project_access_token_medium.png
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/project_access_token.png
--rw-r--r--   0 runner    (1001) docker     (123)    71484 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/images/repo_variables.png
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.949844 doc-to-readme-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/src/doc_to_md/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/src/doc_to_md/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_md/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/src/doc_to_md/doc_to_md.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5288 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 22:52:11.000000 doc-to-readme-1.0.1/src/doc_to_readme.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/templates/.update_readme_gitlab.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:52:11.953845 doc-to-readme-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/tests/classes_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/tests/functions_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-28 22:51:58.000000 doc-to-readme-1.0.1/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.github/workflows/update_readme.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.github/workflows/update_readme_github.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/How_to_setup_the_pipelines.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/bitbucket-pipelines.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    51867 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/access_token_info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66748 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/cicd_variables.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91432 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/create_project_access_token_medium.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/project_access_token.png
+-rw-r--r--   0 runner    (1001) docker     (123)    71484 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/images/repo_variables.png
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.811923 doc-to-readme-1.1.0/src/doc_to_md/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/src/doc_to_md/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_md/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9876 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/src/doc_to_md/doc_to_md.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 10:17:44.000000 doc-to-readme-1.1.0/src/doc_to_readme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/templates/.update_readme_gitlab.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:17:44.815923 doc-to-readme-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/tests/classes_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/tests/functions_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-29 10:17:30.000000 doc-to-readme-1.1.0/tests/test.py
```

### Comparing `doc-to-readme-1.0.1/.github/workflows/publish.yml` & `doc-to-readme-1.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/.github/workflows/update_readme.yml` & `doc-to-readme-1.1.0/.github/workflows/update_readme.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/.github/workflows/update_readme_github.yml` & `doc-to-readme-1.1.0/.github/workflows/update_readme_github.yml`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 on:
   workflow_call:
     inputs:
       PATH_TO_README:
         required: false
         default: "README.md"
         type: string
+      ROOT_DIR:
+        required: false
+        type: string
       EXCLUDED_MODULES:
         required: false
         type: string
       SELECTED_MODULES:
         required: false
         type: string
       SEPARATED:
@@ -41,14 +44,17 @@
           rm -rf doc_to_readme
           cmd="doc_to_md.py -f ${{ inputs.PATH_TO_README }}"
           if [[ ! -z "${{ inputs.EXCLUDED_MODULES }}" ]]; then
             cmd="$cmd -e ${{ inputs.EXCLUDED_MODULES }}"
           elif [[ ! -z "${{ inputs.SELECTED_MODULES }}" ]]; then
             cmd="$cmd -m ${{ inputs.SELECTED_MODULES }}"
           fi
+          if [ ! -z "${{ inputs.ROOT_DIR }}" ]; then
+            cmd="$cmd -r ${{ inputs.ROOT_DIR }}"
+          fi
           if [ "${{ inputs.SEPARATED }}" = "true" ]; then
             cmd="$cmd --separated"
           fi
           echo $cmd
           python3 $cmd
           rm doc_to_md.py
           lines=$(git status -s | wc -l)
```

### Comparing `doc-to-readme-1.0.1/.gitlab-ci.yml` & `doc-to-readme-1.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/How_to_setup_the_pipelines.md` & `doc-to-readme-1.1.0/How_to_setup_the_pipelines.md`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/LICENSE` & `doc-to-readme-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/PKG-INFO` & `doc-to-readme-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-to-readme
-Version: 1.0.1
+Version: 1.1.0
 Summary: Automated Python Module Documentation in Markdown File (README)
 Author-email: Mirjam Ziselsberger <ziselsberger@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mirjam Ziselsberger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,15 +53,15 @@
 > There are several options how to use it:  
 > a) [Python Package](#a-install--use-python-package)   
 > b) [CI Pipeline](#b-add-to-pipeline-github-gitlab-or-bitbucket)  
 
 
 ### a) install & use Python Package
 
-Available on [PyPI](https://pypi.org/project/doc-to-readme/1.0.0/)
+Available on [PyPI](https://pypi.org/project/doc-to-readme)
 ```shell
 pip install doc-to-readme
 ```
 
 - **Use within Python** 
 ```python
 import doc_to_md.doc_to_md as dtm
@@ -84,15 +84,15 @@
 -s SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
 ### b) add to Pipeline (GitHub, GitLab or Bitbucket)
-_[Documentation](./How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
+_[Documentation](https://github.com/ziselsberger/doc_to_readme/blob/main/How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
 
 > ### [**_Step-by-step guide_**](https://github.com/ziselsberger/use_doc_to_readme) on how to integrate _doc_to_readme_ in your Repository
 
 ---
 
 _Copyright &copy; 2023 by Mirjam Ziselsberger_  
 _This code is free to use under the terms of the [MIT license](/LICENSE)._
@@ -108,8 +108,8 @@
 | function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
 | function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-28
+**Last Update:** 2023-04-29
```

### Comparing `doc-to-readme-1.0.1/README.md` & `doc-to-readme-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 > There are several options how to use it:  
 > a) [Python Package](#a-install--use-python-package)   
 > b) [CI Pipeline](#b-add-to-pipeline-github-gitlab-or-bitbucket)  
 
 
 ### a) install & use Python Package
 
-Available on [PyPI](https://pypi.org/project/doc-to-readme/1.0.0/)
+Available on [PyPI](https://pypi.org/project/doc-to-readme)
 ```shell
 pip install doc-to-readme
 ```
 
 - **Use within Python** 
 ```python
 import doc_to_md.doc_to_md as dtm
@@ -48,15 +48,15 @@
 -s SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
 ### b) add to Pipeline (GitHub, GitLab or Bitbucket)
-_[Documentation](./How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
+_[Documentation](https://github.com/ziselsberger/doc_to_readme/blob/main/How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
 
 > ### [**_Step-by-step guide_**](https://github.com/ziselsberger/use_doc_to_readme) on how to integrate _doc_to_readme_ in your Repository
 
 ---
 
 _Copyright &copy; 2023 by Mirjam Ziselsberger_  
 _This code is free to use under the terms of the [MIT license](/LICENSE)._
@@ -72,8 +72,8 @@
 | function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
 | function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-28
+**Last Update:** 2023-04-29
```

### Comparing `doc-to-readme-1.0.1/bitbucket-pipelines.yml` & `doc-to-readme-1.1.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/images/access_token_info.png` & `doc-to-readme-1.1.0/images/access_token_info.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/images/cicd_variables.png` & `doc-to-readme-1.1.0/images/cicd_variables.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/images/create_project_access_token_medium.png` & `doc-to-readme-1.1.0/images/create_project_access_token_medium.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/images/project_access_token.png` & `doc-to-readme-1.1.0/images/project_access_token.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/images/repo_variables.png` & `doc-to-readme-1.1.0/images/repo_variables.png`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/pyproject.toml` & `doc-to-readme-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/src/doc_to_md/doc_to_md.py` & `doc-to-readme-1.1.0/src/doc_to_md/doc_to_md.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
     return functions
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("-f", "--file", required=False, help="Path to README", default="../../README.md")
-    parser.add_argument("-d", "--root_dir", required=False, help="Path to rood dir", default=None)
+    parser.add_argument("-r", "--root_dir", required=False, help="Path to rood dir", default=None)
     parser.add_argument("-e", "--exclude", required=False, help="Exclude modules", default=[], nargs='+')
     parser.add_argument("-m", "--modules", required=False, help="Specify modules", default=[], nargs='+')
     parser.add_argument("--separated", required=False, help="Separate tables for each module", action='store_true')
     args = parser.parse_args()
 
     exclude = ("test", "functions_for_testing", "classes_for_testing")
     if args.exclude is not None and args.exclude != [""]:
```

### Comparing `doc-to-readme-1.0.1/src/doc_to_readme.egg-info/PKG-INFO` & `doc-to-readme-1.1.0/src/doc_to_readme.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doc-to-readme
-Version: 1.0.1
+Version: 1.1.0
 Summary: Automated Python Module Documentation in Markdown File (README)
 Author-email: Mirjam Ziselsberger <ziselsberger@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mirjam Ziselsberger
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,15 +53,15 @@
 > There are several options how to use it:  
 > a) [Python Package](#a-install--use-python-package)   
 > b) [CI Pipeline](#b-add-to-pipeline-github-gitlab-or-bitbucket)  
 
 
 ### a) install & use Python Package
 
-Available on [PyPI](https://pypi.org/project/doc-to-readme/1.0.0/)
+Available on [PyPI](https://pypi.org/project/doc-to-readme)
 ```shell
 pip install doc-to-readme
 ```
 
 - **Use within Python** 
 ```python
 import doc_to_md.doc_to_md as dtm
@@ -84,15 +84,15 @@
 -s SELECTED_MODULES     # Only these modules will be included
 --separated             # Create one table per module
 ```
 
 ---
 
 ### b) add to Pipeline (GitHub, GitLab or Bitbucket)
-_[Documentation](./How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
+_[Documentation](https://github.com/ziselsberger/doc_to_readme/blob/main/How_to_setup_the_pipelines.md) on how to set up the pipelines to update a file on every push._
 
 > ### [**_Step-by-step guide_**](https://github.com/ziselsberger/use_doc_to_readme) on how to integrate _doc_to_readme_ in your Repository
 
 ---
 
 _Copyright &copy; 2023 by Mirjam Ziselsberger_  
 _This code is free to use under the terms of the [MIT license](/LICENSE)._
@@ -108,8 +108,8 @@
 | function  | `update_markdown_file(file: str = "../../README.md", root_dir: str = None, exclude_modules: Optional[Tuple[str, ...]] = ("test", "functions_for_testing", "classes_for_testing", "doc_to_md"), specified_modules: Optional[Tuple[str, ...]] = None, separate: bool = True)` | Add/update 'Functions & Classes' Section in Markdown file. |
 | function  | `parse_through_file(file: str) -> Dict[str, Dict[str, str]]` | Parse through module and gather info on classes and functions |
 
 Created with: [doc_to_readme](https://github.com/ziselsberger/doc_to_readme)  
 [MIT](https://github.com/ziselsberger/doc_to_readme/blob/main/LICENSE) &copy; 2023 Mirjam Ziselsberger
 
 ---
-**Last Update:** 2023-04-28
+**Last Update:** 2023-04-29
```

### Comparing `doc-to-readme-1.0.1/src/doc_to_readme.egg-info/SOURCES.txt` & `doc-to-readme-1.1.0/src/doc_to_readme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/templates/.update_readme_gitlab.yml` & `doc-to-readme-1.1.0/templates/.update_readme_gitlab.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 variables:
   BOT_NAME: "AUTO-UPDATE-README"
   BOT_EMAIL: "doc@update_readme.com"
   COMMIT_MESSAGE: "Auto-update README.md"
   PATH_TO_README: "README.md"
+  ROOT_DIR: ""
   EXCLUDED_MODULES: ""
   SELECTED_MODULES: ""
   SEPARATED: "true"
 
 .push: &push |
   git status
   lines=$(git status -s | wc -l)
@@ -21,14 +22,17 @@
 .exec: &exec |
   cmd="doc_to_md.py -f $PATH_TO_README"
   if [[ ! -z $EXCLUDED_MODULES ]]; then
     cmd="$cmd -e $EXCLUDED_MODULES"
   elif [[ ! -z $SELECTED_MODULES ]]; then
     cmd="$cmd -m $SELECTED_MODULES"
   fi
+  if [ ! -z $ROOT_DIR ]; then
+    cmd="$cmd -r $ROOT_DIR"
+  fi
   if [ $SEPARATED = "true" ]; then
     cmd="$cmd --separated"
   fi
   echo $cmd
   python $cmd
   rm doc_to_md.py
```

### Comparing `doc-to-readme-1.0.1/tests/classes_for_testing.py` & `doc-to-readme-1.1.0/tests/classes_for_testing.py`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/tests/functions_for_testing.py` & `doc-to-readme-1.1.0/tests/functions_for_testing.py`

 * *Files identical despite different names*

### Comparing `doc-to-readme-1.0.1/tests/test.py` & `doc-to-readme-1.1.0/tests/test.py`

 * *Files identical despite different names*

