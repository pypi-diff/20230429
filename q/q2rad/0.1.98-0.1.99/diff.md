# Comparing `tmp/q2rad-0.1.98.tar.gz` & `tmp/q2rad-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "q2rad-0.1.98.tar", max compression
+gzip compressed data, was "q2rad-0.1.99.tar", max compression
```

## Comparing `q2rad-0.1.98.tar` & `q2rad-0.1.99.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      728 2023-02-15 21:22:04.208976 q2rad-0.1.98/pyproject.toml
--rw-r--r--   0        0        0      181 2022-12-14 00:20:22.750681 q2rad-0.1.98/q2rad/__init__.py
--rw-r--r--   0        0        0       88 2022-12-11 12:44:53.852649 q2rad-0.1.98/q2rad/__main__.py
--rw-r--r--   0        0        0     5892 2023-01-10 23:08:36.060453 q2rad-0.1.98/q2rad/q2actions.py
--rw-r--r--   0        0        0    12679 2023-02-15 21:21:17.648427 q2rad-0.1.98/q2rad/q2appmanager.py
--rw-r--r--   0        0        0    11186 2023-01-09 22:00:08.378159 q2rad-0.1.98/q2rad/q2appselector.py
--rw-r--r--   0        0        0     2896 2023-02-14 09:31:29.059353 q2rad-0.1.98/q2rad/q2constants.py
--rw-r--r--   0        0        0     8474 2023-01-27 22:31:36.974481 q2rad-0.1.98/q2rad/q2forms.py
--rw-r--r--   0        0        0    10415 2023-02-07 14:03:39.703184 q2rad-0.1.98/q2rad/q2lines.py
--rw-r--r--   0        0        0     2133 2022-12-11 12:44:53.858756 q2rad-0.1.98/q2rad/q2market.py
--rw-r--r--   0        0        0     2844 2023-02-09 08:50:05.882650 q2rad-0.1.98/q2rad/q2modules.py
--rw-r--r--   0        0        0     2825 2023-01-09 22:41:49.435151 q2rad-0.1.98/q2rad/q2packages.py
--rw-r--r--   0        0        0    11231 2023-01-19 19:09:41.272235 q2rad-0.1.98/q2rad/q2queries.py
--rw-r--r--   0        0        0    28028 2023-02-15 11:20:35.071448 q2rad-0.1.98/q2rad/q2rad.py
--rw-r--r--   0        0        0     3590 2023-02-09 09:50:08.374679 q2rad-0.1.98/q2rad/q2raddb.py
--rw-r--r--   0        0        0    77493 2023-02-14 17:04:19.708186 q2rad-0.1.98/q2rad/q2reports.py
--rw-r--r--   0        0        0     2979 2023-01-25 23:44:01.866645 q2rad-0.1.98/q2rad/q2utils.py
--rw-r--r--   0        0        0       22 2023-02-15 21:22:07.587480 q2rad-0.1.98/q2rad/version.py
--rw-r--r--   0        0        0     2237 2022-12-11 12:44:53.818827 q2rad-0.1.98/README.md
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 q2rad-0.1.98/setup.py
--rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 q2rad-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0      728 2023-02-15 22:15:39.140482 q2rad-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0      181 2022-12-14 00:20:22.750681 q2rad-0.1.99/q2rad/__init__.py
+-rw-r--r--   0        0        0       88 2022-12-11 12:44:53.852649 q2rad-0.1.99/q2rad/__main__.py
+-rw-r--r--   0        0        0     5892 2023-01-10 23:08:36.060453 q2rad-0.1.99/q2rad/q2actions.py
+-rw-r--r--   0        0        0    12671 2023-02-15 21:51:26.243605 q2rad-0.1.99/q2rad/q2appmanager.py
+-rw-r--r--   0        0        0    11186 2023-01-09 22:00:08.378159 q2rad-0.1.99/q2rad/q2appselector.py
+-rw-r--r--   0        0        0     2896 2023-02-14 09:31:29.059353 q2rad-0.1.99/q2rad/q2constants.py
+-rw-r--r--   0        0        0     8474 2023-01-27 22:31:36.974481 q2rad-0.1.99/q2rad/q2forms.py
+-rw-r--r--   0        0        0    10415 2023-02-07 14:03:39.703184 q2rad-0.1.99/q2rad/q2lines.py
+-rw-r--r--   0        0        0     2133 2022-12-11 12:44:53.858756 q2rad-0.1.99/q2rad/q2market.py
+-rw-r--r--   0        0        0     2844 2023-02-09 08:50:05.882650 q2rad-0.1.99/q2rad/q2modules.py
+-rw-r--r--   0        0        0     2825 2023-01-09 22:41:49.435151 q2rad-0.1.99/q2rad/q2packages.py
+-rw-r--r--   0        0        0    11231 2023-01-19 19:09:41.272235 q2rad-0.1.99/q2rad/q2queries.py
+-rw-r--r--   0        0        0    28028 2023-02-15 11:20:35.071448 q2rad-0.1.99/q2rad/q2rad.py
+-rw-r--r--   0        0        0     3590 2023-02-09 09:50:08.374679 q2rad-0.1.99/q2rad/q2raddb.py
+-rw-r--r--   0        0        0    77493 2023-02-14 17:04:19.708186 q2rad-0.1.99/q2rad/q2reports.py
+-rw-r--r--   0        0        0     2979 2023-01-25 23:44:01.866645 q2rad-0.1.99/q2rad/q2utils.py
+-rw-r--r--   0        0        0       22 2023-02-15 22:15:41.182985 q2rad-0.1.99/q2rad/version.py
+-rw-r--r--   0        0        0     2237 2022-12-11 12:44:53.818827 q2rad-0.1.99/README.md
+-rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 q2rad-0.1.99/setup.py
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 q2rad-0.1.99/PKG-INFO
```

### Comparing `q2rad-0.1.98/pyproject.toml` & `q2rad-0.1.99/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "q2rad"
-version = "0.1.98"
+version = "0.1.99"
 description = "RAD - database, GUI, reports"
 authors = ["Andrei Puchko <andrei.puchko@gmx.de>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `q2rad-0.1.98/q2rad/q2actions.py` & `q2rad-0.1.99/q2rad/q2actions.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2appmanager.py` & `q2rad-0.1.99/q2rad/q2appmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,10 +348,10 @@
             db.cursor(f"delete from {table}")
             for row in data[table]:
                 wait_row.step()
                 if not db.raw_insert(table, row):
                     errors.append(db.last_sql_error)
                     print(db.last_sql_error)
             wait_row.close()
-            if errors:
-                q2Mess("<br>".join(errors))
+        if errors:
+            q2Mess("<br>".join(errors))
         wait_table.close()
```

### Comparing `q2rad-0.1.98/q2rad/q2appselector.py` & `q2rad-0.1.99/q2rad/q2appselector.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2constants.py` & `q2rad-0.1.99/q2rad/q2constants.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2forms.py` & `q2rad-0.1.99/q2rad/q2forms.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2lines.py` & `q2rad-0.1.99/q2rad/q2lines.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2market.py` & `q2rad-0.1.99/q2rad/q2market.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2modules.py` & `q2rad-0.1.99/q2rad/q2modules.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2packages.py` & `q2rad-0.1.99/q2rad/q2packages.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2queries.py` & `q2rad-0.1.99/q2rad/q2queries.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2rad.py` & `q2rad-0.1.99/q2rad/q2rad.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2raddb.py` & `q2rad-0.1.99/q2rad/q2raddb.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2reports.py` & `q2rad-0.1.99/q2rad/q2reports.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/q2rad/q2utils.py` & `q2rad-0.1.99/q2rad/q2utils.py`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/README.md` & `q2rad-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `q2rad-0.1.98/setup.py` & `q2rad-0.1.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['q2db>=0.1.9,<0.2.0', 'q2gui>=0.1.36,<0.2.0', 'q2report>=0.1.16,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['q2rad = q2rad.q2rad:main']}
 
 setup_kwargs = {
     'name': 'q2rad',
-    'version': '0.1.98',
+    'version': '0.1.99',
     'description': 'RAD - database, GUI, reports',
     'long_description': '# The RAD (rapid application development) system. \n\n**(code less, make more)**  \n**Based on:**  \n    q2db        (https://pypi.org/project/q2db)  \n    q2gui       (https://pypi.org/project/q2gui)  \n    q2report    (https://pypi.org/project/q2report)  \n\n## [Read the docs](docs/index.md) \n## Install & run\n**Linux**\n```bash\nmkdir q2rad && \\\n    cd q2rad && \\\n    python3 -m pip install --upgrade pip && \\\n    python3 -m venv q2rad && \\\n    source q2rad/bin/activate && \\\n    python3 -m pip install --upgrade q2rad && \\\n    q2rad\n```\n**Windows**\n```bash\nmkdir q2rad && \\\n    cd q2rad && \\\n    py -m pip install --upgrade pip && \\\n    py -m venv q2rad && \\\n    call q2rad/scripts/activate && \\\n    pip install --upgrade q2rad  && \\\n    q2rad\n```\n**Mac**\n```bash\nmkdir q2rad && \\\n    cd q2rad && \\\n    python3 -m pip install --upgrade pip && \\\n    python3 -m venv q2rad && \\\n    source q2rad/bin/activate && \\\n    python3 -m pip install --upgrade q2rad && \\\n    q2rad\n```\n**Docker**\n```bash\ncurl -s https://raw.githubusercontent.com/AndreiPuchko/q2rad/main/docker-x11/dockerfile > dockerfile && \\\n    mkdir -p q2rad_storage/Desktop && \\\n    chmod -R 777 q2rad_storage && \\\n    sudo docker build -t q2rad . && \\\n    sudo docker run -it \\\n        -v /tmp/.X11-unix:/tmp/.X11-unix \\\n        -v $(pwd)/q2rad_storage:/home/q2rad \\\n        -e DISPLAY=$DISPLAY \\\n        -u q2rad q2rad python3 -m q2rad\n\n```\n## Concept:\nApplication as a database\n```python\nForms:        #  may have main menu (menubar) definitions\n              #  may be linked to database table\n    \n    Lines:    #  form fields(type of data and type of form control) and \n              #  layout definitions\n              #  when form is linked to database - database columns definitions\n    \n    Actions:  #  applies for database linked forms\n              #  may be standard CRUD-action \n              #  or \n              #  run a script (run reports, forms and etc)\n              #  or\n              #  may have linked subforms (one-to-many)\n\nModules:      #  python scripts\n\nQueries:      #  query development and debugging tool\n\nReports:      #  multiformat (HTML, DOCX, XLSX) reporting tool \n```\n',
     'author': 'Andrei Puchko',
     'author_email': 'andrei.puchko@gmx.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `q2rad-0.1.98/PKG-INFO` & `q2rad-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: q2rad
-Version: 0.1.98
+Version: 0.1.99
 Summary: RAD - database, GUI, reports
 Author: Andrei Puchko
 Author-email: andrei.puchko@gmx.de
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

