# Comparing `tmp/garpy-0.3.8.tar.gz` & `tmp/garpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpy-0.3.8.tar", max compression
+gzip compressed data, was "garpy-0.4.0.tar", max compression
```

## Comparing `garpy-0.3.8.tar` & `garpy-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,11 @@
--rw-r--r--   0        0        0    11324 2019-08-24 10:51:23.000000 garpy-0.3.8/LICENSE
--rw-r--r--   0        0        0     4830 2022-12-25 16:25:48.988334 garpy-0.3.8/README.rst
--rw-r--r--   0        0        0      653 2022-12-25 16:26:11.603216 garpy-0.3.8/garpy/__init__.py
--rw-r--r--   0        0        0     5175 2022-12-21 21:09:38.000000 garpy-0.3.8/garpy/activity.py
--rw-r--r--   0        0        0     2755 2022-12-21 21:09:38.000000 garpy-0.3.8/garpy/cli.py
--rw-r--r--   0        0        0     8446 2022-12-21 21:30:40.000000 garpy-0.3.8/garpy/client.py
--rw-r--r--   0        0        0     5574 2022-01-23 11:53:52.234448 garpy-0.3.8/garpy/download.py
--rw-r--r--   0        0        0     1295 2022-12-25 16:25:48.988334 garpy-0.3.8/garpy/resources/default_config.yaml
--rw-r--r--   0        0        0     1399 2022-12-21 21:09:38.000000 garpy-0.3.8/garpy/settings.py
--rw-r--r--   0        0        0     1627 2022-12-21 21:09:38.000000 garpy-0.3.8/garpy/wellness.py
--rw-r--r--   0        0        0      707 2022-12-25 16:26:11.603216 garpy-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     5912 1970-01-01 00:00:00.000000 garpy-0.3.8/setup.py
--rw-r--r--   0        0        0     5657 1970-01-01 00:00:00.000000 garpy-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11324 2019-08-24 10:51:23.000000 garpy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4830 2022-12-25 16:25:48.988334 garpy-0.4.0/README.rst
+-rw-r--r--   0        0        0      620 2023-04-29 16:14:24.759835 garpy-0.4.0/garpy/__init__.py
+-rw-r--r--   0        0        0     5179 2023-04-29 16:18:50.097756 garpy-0.4.0/garpy/activity.py
+-rw-r--r--   0        0        0     2778 2023-04-29 15:58:49.235405 garpy-0.4.0/garpy/cli.py
+-rw-r--r--   0        0        0     5597 2023-04-29 16:18:50.097756 garpy-0.4.0/garpy/download.py
+-rw-r--r--   0        0        0     1295 2022-12-25 16:25:48.988334 garpy-0.4.0/garpy/resources/default_config.yaml
+-rw-r--r--   0        0        0     1399 2022-12-21 21:09:38.000000 garpy-0.4.0/garpy/settings.py
+-rw-r--r--   0        0        0     1630 2023-04-29 16:18:50.101756 garpy-0.4.0/garpy/wellness.py
+-rw-r--r--   0        0        0      730 2023-04-29 16:18:50.101756 garpy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5752 1970-01-01 00:00:00.000000 garpy-0.4.0/PKG-INFO
```

### Comparing `garpy-0.3.8/LICENSE` & `garpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garpy-0.3.8/README.rst` & `garpy-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `garpy-0.3.8/garpy/__init__.py` & `garpy-0.4.0/garpy/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-__version__ = "0.3.8"
+__version__ = "0.4.0"
 
 import logging
 import sys
 
 from .activity import Activities, Activity
-from .client import GarminClient
 from .download import ActivitiesDownloader
 from .wellness import Wellness
 
 # Create logger
 logger = logging.getLogger(__name__)
 
 # Avoid duplicate handlers
```

### Comparing `garpy-0.3.8/garpy/activity.py` & `garpy-0.4.0/garpy/activity.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import zipfile
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Dict
 
 import attr
 import pendulum
+from garpyclient import GarminClient
 
-from .client import GarminClient
 from .settings import config
 
 
 @attr.s(frozen=True)
 class Activity:
     """Garmin activity
```

### Comparing `garpy-0.3.8/garpy/cli.py` & `garpy-0.4.0/garpy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pathlib import Path
 
 import click
+from garpyclient import GarminClient
 
-from garpy import ActivitiesDownloader, GarminClient
+from garpy import ActivitiesDownloader
 from garpy.settings import config
 
 FORMATS = set(config.get("activities").keys()) | {"fit"}
 
 
 @click.group()
 @click.version_option()
```

### Comparing `garpy-0.3.8/garpy/download.py` & `garpy-0.4.0/garpy/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #! /usr/bin/env python
 
 import logging
 from pathlib import Path
 from typing import Dict
 
 import attr
+from garpyclient import GarminClient
 
-from . import Activities, Activity, GarminClient
+from . import Activities, Activity
 from .settings import config
 
 logger = logging.getLogger(__name__)
 
 DEFAULT_FORMATS = tuple(config["activities"].keys())
```

### Comparing `garpy-0.3.8/garpy/resources/default_config.yaml` & `garpy-0.4.0/garpy/resources/default_config.yaml`

 * *Files identical despite different names*

### Comparing `garpy-0.3.8/garpy/settings.py` & `garpy-0.4.0/garpy/settings.py`

 * *Files identical despite different names*

### Comparing `garpy-0.3.8/garpy/wellness.py` & `garpy-0.4.0/garpy/wellness.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #! /usr/bin/env python
 
 from pathlib import Path
 
 import attr
 import pendulum
-
-from .client import GarminClient
+from garpyclient import GarminClient
 
 
 @attr.s(frozen=True)
 class Wellness:
     """Garmin wellness data
```

### Comparing `garpy-0.3.8/pyproject.toml` & `garpy-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "garpy"
-version = "0.3.8"
+version = "0.4.0"
 description = "Python client for downloading activities from Garmin Connect"
 authors = ["Felipe Aguirre Martinez <felipeam86@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/felipeam86/garpy"
 
 [tool.poetry.scripts]
@@ -15,14 +15,15 @@
 requests = "^2.22"
 attrs = "^21.4.0"
 pendulum = "^2.0"
 PyYAML = ">=5.1,<7.0"
 click = ">=7,<9"
 tqdm = "^4.36"
 cloudscraper = "^1.2.58"
+garpyclient = "^0.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0"
 coveralls = "^3.0"
 black = "^22.12.0"
 isort = "^5.11.4"
```

### Comparing `garpy-0.3.8/setup.py` & `garpy-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,147 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: garpy
+Version: 0.4.0
+Summary: Python client for downloading activities from Garmin Connect
+Home-page: https://github.com/felipeam86/garpy
+License: MIT
+Author: Felipe Aguirre Martinez
+Author-email: felipeam86@gmail.com
+Requires-Python: >=3.7.9,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=5.1,<7.0)
+Requires-Dist: attrs (>=21.4.0,<22.0.0)
+Requires-Dist: click (>=7,<9)
+Requires-Dist: cloudscraper (>=1.2.58,<2.0.0)
+Requires-Dist: garpyclient (>=0.1.1,<0.2.0)
+Requires-Dist: pendulum (>=2.0,<3.0)
+Requires-Dist: requests (>=2.22,<3.0)
+Requires-Dist: tqdm (>=4.36,<5.0)
+Description-Content-Type: text/x-rst
 
-packages = \
-['garpy']
+###################################
+Garpy: Make your garmin data yours!
+###################################
 
-package_data = \
-{'': ['*'], 'garpy': ['resources/*']}
+|PyPI-Versions| |PyPI-Status| |Codacy-Grade| |Tests| |Coveralls|
 
-install_requires = \
-['PyYAML>=5.1,<7.0',
- 'attrs>=21.4.0,<22.0.0',
- 'click>=7,<9',
- 'cloudscraper>=1.2.58,<2.0.0',
- 'pendulum>=2.0,<3.0',
- 'requests>=2.22,<3.0',
- 'tqdm>=4.36,<5.0']
-
-entry_points = \
-{'console_scripts': ['garpy = garpy.cli:main']}
-
-setup_kwargs = {
-    'name': 'garpy',
-    'version': '0.3.8',
-    'description': 'Python client for downloading activities from Garmin Connect',
-    'long_description': '###################################\nGarpy: Make your garmin data yours!\n###################################\n\n|PyPI-Versions| |PyPI-Status| |Codacy-Grade| |Tests| |Coveralls|\n\n``garpy`` is a simple app used to backup your data from Garmin Connect. It can be used to do incremental\nbackups of your data from Garmin Connect or to download one specific activity.\n\n********************************\nIncremental backup of activities\n********************************\n\nThe first time you use it, all the activities found on your Garmin Connect account will be downloaded to\nthe directory that you specify. Afterwards, each time you run the command, only the newly available\nactivities will be downloaded.\n\nThe command is used as follows:\n\n.. code:: sh\n\n    garpy download {backup-dir}\n\nBehind the scenes, this is what will happen:\n\n- `garpy` will prompt you for your password and will then authenticate against Garmin Connect.\n- It will first fetch the list of all your activities from garmin.\n- It will check which activities have already been backed up on the given `backup-dir`\n- It will proceed to download all the missing activities.\n\n************************************\nDownloading one activity from its ID\n************************************\n\nIf you wish to download only one activity or simple you want to refresh an already downloaded activity,\nuse the \'-a/--activity\' flag as follows:\n\n.. code:: sh\n\n    garpy download --activity 1674567326 {backup-dir}\n\nThis will download the activity in all existing formats to the given `backup_dir`\n\n****************\nFull CLI options\n****************\n\nFor more detailed usage, invoke the \'--help\' command:\n\n.. code:: sh\n\n    $ garpy download --help\n    Usage: garpy download [OPTIONS] [BACKUP_DIR]\n\n      Download activities from Garmin Connect\n\n      Entry point for downloading activities from Garmin Connect. By default, it\n      downloads all newly created activities since the last time you did a backup.\n\n      If you specify an activity ID with the "-a/--activity" flag, only that\n      activity will be downloaded, even if it has already been downloaded before.\n\n      If no format is specified, the app will download all possible formats.\n      Otherwise you can specify the formats you wish to download with the\n      "-f/--formats" flag. The flag can be used several  times if you wish to\n      specify several formats, e.g., \'garpy download [OPTIONS] -f original -f gpx\n      [BACKUP_DIR]\' will download .fit and .gpx files\n\n      Options:\n      -f, --formats [original|gpx|fit|tcx|kml|summary|details]\n                                      Which formats to download. The flag can be\n                                      used several times, e.g. \'-f original -f\n                                      gpx\'\n      -u, --username {username}       Username of your Garmin account\n      -p, --password {password}       Password of your Garmin account\n      -a, --activity {ID}             Activity ID. If indicated, download only\n                                      that activity, even if it has already been\n                                      downloaded. Otherwise, do incremental update\n                                      of backup\n      --user-agent {user_agent}       User agent to be used by requests\n      --help                          Show this message and exit.\n\n\n************\nInstallation\n************\n``garpy`` requires Python 3.7 or higher on your system. For those who know your way around with Python, install\n``garpy`` with pip as follows:\n\n.. code:: sh\n\n    pip install -U garpy\n\n\nIf you are new to Python or have Python 2 installed on your\ncomputer, I recommend you install Miniconda_. To my knowledge, it is the simplest way of installing a robust and\nlightweight Python environment.\n\n\n****************\nAcknowledgements\n****************\n\nThe library is based on garminexport_. I borrowed the GarminClient, refactored it to my taste and\ncreated a package from it.\n\n\n.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/garpy.svg?logo=python&logoColor=white\n   :target: https://pypi.org/project/garpy\n.. |PyPI-Status| image:: https://img.shields.io/pypi/v/garpy.svg\n   :target: https://pypi.org/project/garpy\n.. |Codacy-Grade| image:: https://api.codacy.com/project/badge/Grade/2fbbd268e0a04cd0983291227be53873\n   :target: https://app.codacy.com/manual/garpy/garpy/dashboard\n.. |Tests| image:: https://github.com/felipeam86/garpy/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/felipeam86/garpy/actions/workflows/test.yml\n.. |Coveralls| image:: https://coveralls.io/repos/github/felipeam86/garpy/badge.svg?branch=develop\n    :target: https://coveralls.io/github/felipeam86/garpy?branch=develop\n\n\n.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html\n.. _garminexport: https://github.com/petergardfjall/garminexport\n',
-    'author': 'Felipe Aguirre Martinez',
-    'author_email': 'felipeam86@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/felipeam86/garpy',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7.9,<4.0.0',
-}
+``garpy`` is a simple app used to backup your data from Garmin Connect. It can be used to do incremental
+backups of your data from Garmin Connect or to download one specific activity.
 
+********************************
+Incremental backup of activities
+********************************
+
+The first time you use it, all the activities found on your Garmin Connect account will be downloaded to
+the directory that you specify. Afterwards, each time you run the command, only the newly available
+activities will be downloaded.
+
+The command is used as follows:
+
+.. code:: sh
+
+    garpy download {backup-dir}
+
+Behind the scenes, this is what will happen:
+
+- `garpy` will prompt you for your password and will then authenticate against Garmin Connect.
+- It will first fetch the list of all your activities from garmin.
+- It will check which activities have already been backed up on the given `backup-dir`
+- It will proceed to download all the missing activities.
+
+************************************
+Downloading one activity from its ID
+************************************
+
+If you wish to download only one activity or simple you want to refresh an already downloaded activity,
+use the '-a/--activity' flag as follows:
+
+.. code:: sh
+
+    garpy download --activity 1674567326 {backup-dir}
+
+This will download the activity in all existing formats to the given `backup_dir`
+
+****************
+Full CLI options
+****************
+
+For more detailed usage, invoke the '--help' command:
+
+.. code:: sh
+
+    $ garpy download --help
+    Usage: garpy download [OPTIONS] [BACKUP_DIR]
+
+      Download activities from Garmin Connect
+
+      Entry point for downloading activities from Garmin Connect. By default, it
+      downloads all newly created activities since the last time you did a backup.
+
+      If you specify an activity ID with the "-a/--activity" flag, only that
+      activity will be downloaded, even if it has already been downloaded before.
+
+      If no format is specified, the app will download all possible formats.
+      Otherwise you can specify the formats you wish to download with the
+      "-f/--formats" flag. The flag can be used several  times if you wish to
+      specify several formats, e.g., 'garpy download [OPTIONS] -f original -f gpx
+      [BACKUP_DIR]' will download .fit and .gpx files
+
+      Options:
+      -f, --formats [original|gpx|fit|tcx|kml|summary|details]
+                                      Which formats to download. The flag can be
+                                      used several times, e.g. '-f original -f
+                                      gpx'
+      -u, --username {username}       Username of your Garmin account
+      -p, --password {password}       Password of your Garmin account
+      -a, --activity {ID}             Activity ID. If indicated, download only
+                                      that activity, even if it has already been
+                                      downloaded. Otherwise, do incremental update
+                                      of backup
+      --user-agent {user_agent}       User agent to be used by requests
+      --help                          Show this message and exit.
+
+
+************
+Installation
+************
+``garpy`` requires Python 3.7 or higher on your system. For those who know your way around with Python, install
+``garpy`` with pip as follows:
+
+.. code:: sh
+
+    pip install -U garpy
+
+
+If you are new to Python or have Python 2 installed on your
+computer, I recommend you install Miniconda_. To my knowledge, it is the simplest way of installing a robust and
+lightweight Python environment.
+
+
+****************
+Acknowledgements
+****************
+
+The library is based on garminexport_. I borrowed the GarminClient, refactored it to my taste and
+created a package from it.
+
+
+.. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/garpy.svg?logo=python&logoColor=white
+   :target: https://pypi.org/project/garpy
+.. |PyPI-Status| image:: https://img.shields.io/pypi/v/garpy.svg
+   :target: https://pypi.org/project/garpy
+.. |Codacy-Grade| image:: https://api.codacy.com/project/badge/Grade/2fbbd268e0a04cd0983291227be53873
+   :target: https://app.codacy.com/manual/garpy/garpy/dashboard
+.. |Tests| image:: https://github.com/felipeam86/garpy/actions/workflows/test.yml/badge.svg
+    :target: https://github.com/felipeam86/garpy/actions/workflows/test.yml
+.. |Coveralls| image:: https://coveralls.io/repos/github/felipeam86/garpy/badge.svg?branch=develop
+    :target: https://coveralls.io/github/felipeam86/garpy?branch=develop
+
+
+.. _Miniconda: https://docs.conda.io/en/latest/miniconda.html
+.. _garminexport: https://github.com/petergardfjall/garminexport
 
-setup(**setup_kwargs)
```

