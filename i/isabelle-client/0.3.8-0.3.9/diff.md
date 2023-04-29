# Comparing `tmp/isabelle-client-0.3.8.tar.gz` & `tmp/isabelle-client-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isabelle-client-0.3.8.tar", max compression
+gzip compressed data, was "isabelle-client-0.3.9.tar", max compression
```

## Comparing `isabelle-client-0.3.8.tar` & `isabelle-client-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11358 2022-04-20 19:15:05.623546 isabelle-client-0.3.8/LICENSE
--rw-r--r--   0        0        0     4121 2022-08-24 07:23:02.382775 isabelle-client-0.3.8/README.rst
--rw-r--r--   0        0        0      897 2022-08-30 09:49:47.416713 isabelle-client-0.3.8/isabelle_client/__init__.py
--rw-r--r--   0        0        0     3351 2022-08-24 07:23:02.446777 isabelle-client-0.3.8/isabelle_client/conftest.py
--rw-r--r--   0        0        0    11617 2022-08-24 07:23:02.450778 isabelle-client-0.3.8/isabelle_client/isabelle__client.py
--rw-r--r--   0        0        0        0 2022-04-20 19:15:05.651546 isabelle-client-0.3.8/isabelle_client/py.typed
--rw-r--r--   0        0        0      295 2022-08-04 13:52:33.523169 isabelle-client-0.3.8/isabelle_client/resources/Cygwin-Isabelle.bat
--rw-r--r--   0        0        0     1247 2022-08-24 07:23:02.458778 isabelle-client-0.3.8/isabelle_client/resources/example.txt
--rwxr-xr-x   0        0        0       79 2022-04-20 19:15:05.651546 isabelle-client-0.3.8/isabelle_client/resources/isabelle
--rw-r--r--   0        0        0     5186 2022-08-24 07:23:02.462778 isabelle-client-0.3.8/isabelle_client/socket_communication.py
--rw-r--r--   0        0        0     4339 2022-08-24 07:23:02.466778 isabelle-client-0.3.8/isabelle_client/utils.py
--rw-r--r--   0        0        0     3392 2022-08-30 09:49:47.428715 isabelle-client-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4977 2022-08-30 09:50:09.428986 isabelle-client-0.3.8/setup.py
--rw-r--r--   0        0        0     5184 2022-08-30 09:50:09.430068 isabelle-client-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-04-20 19:15:05.623546 isabelle-client-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4148 2022-09-29 10:12:35.509720 isabelle-client-0.3.9/README.rst
+-rw-r--r--   0        0        0      897 2022-09-29 10:12:35.601741 isabelle-client-0.3.9/isabelle_client/__init__.py
+-rw-r--r--   0        0        0     3351 2022-08-24 07:23:02.446777 isabelle-client-0.3.9/isabelle_client/conftest.py
+-rw-r--r--   0        0        0    11617 2022-08-24 07:23:02.450778 isabelle-client-0.3.9/isabelle_client/isabelle__client.py
+-rw-r--r--   0        0        0        0 2022-04-20 19:15:05.651546 isabelle-client-0.3.9/isabelle_client/py.typed
+-rw-r--r--   0        0        0      295 2022-08-04 13:52:33.523169 isabelle-client-0.3.9/isabelle_client/resources/Cygwin-Isabelle.bat
+-rw-r--r--   0        0        0     1247 2022-08-24 07:23:02.458778 isabelle-client-0.3.9/isabelle_client/resources/example.txt
+-rwxr-xr-x   0        0        0       79 2022-04-20 19:15:05.651546 isabelle-client-0.3.9/isabelle_client/resources/isabelle
+-rw-r--r--   0        0        0     5186 2022-08-24 07:23:02.462778 isabelle-client-0.3.9/isabelle_client/socket_communication.py
+-rw-r--r--   0        0        0     4339 2022-09-13 13:31:05.953877 isabelle-client-0.3.9/isabelle_client/utils.py
+-rw-r--r--   0        0        0     3441 2022-09-29 10:12:35.613743 isabelle-client-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5004 2022-09-29 10:19:02.882473 isabelle-client-0.3.9/setup.py
+-rw-r--r--   0        0        0     5211 2022-09-29 10:19:02.883760 isabelle-client-0.3.9/PKG-INFO
```

### Comparing `isabelle-client-0.3.8/LICENSE` & `isabelle-client-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.8/README.rst` & `isabelle-client-0.3.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -78,24 +78,23 @@
 
 More documentation can be found
 `here <https://isabelle-client.readthedocs.io/en/latest>`__.
 
 Video example
 =============
 
-.. image:: ../_static/tty.gif
-  :alt:
-
-(if not displayed correctly on this page, please watch `here <https://isabelle-client.readthedocs.io/en/latest/#video-example>`__).
-
+.. image:: https://isabelle-client.readthedocs.io/en/latest/_images/tty.gif
+	   
 How to cite
 ===========
 
-If you’re writing a research paper, you can cite Isabelle client (and
-Isabelle 2021) using the `following
+If you’re writing a research paper, you can cite Isabelle client
+using the `following DOI
+<https://doi.org/10.1007/978-3-031-16681-5_24>`__. You can also cite
+Isabelle 2021 (and the earlier version of the client) with `this
 DOI <https://doi.org/10.1007/978-3-030-81097-9_20>`__.
 
 .. |PyPI version| image:: https://badge.fury.io/py/isabelle-client.svg
    :target: https://badge.fury.io/py/isabelle-client
 .. |Anaconda version| image:: https://anaconda.org/conda-forge/isabelle-client/badges/version.svg
    :target: https://anaconda.org/conda-forge/isabelle-client
 .. |CircleCI| image:: https://circleci.com/gh/inpefess/isabelle-client.svg?style=svg
```

### Comparing `isabelle-client-0.3.8/isabelle_client/__init__.py` & `isabelle-client-0.3.9/isabelle_client/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 # noqa: D205
 """A Python client to `Isabelle <https://isabelle.in.tum.de>`__ server."""
 from isabelle_client.isabelle__client import IsabelleClient
 from isabelle_client.socket_communication import IsabelleResponse
 from isabelle_client.utils import get_isabelle_client, start_isabelle_server
 
-__version__ = "0.3.8"
+__version__ = "0.3.9"
```

### Comparing `isabelle-client-0.3.8/isabelle_client/conftest.py` & `isabelle-client-0.3.9/isabelle_client/conftest.py`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.8/isabelle_client/isabelle__client.py` & `isabelle-client-0.3.9/isabelle_client/isabelle__client.py`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.8/isabelle_client/resources/example.txt` & `isabelle-client-0.3.9/isabelle_client/resources/example.txt`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.8/isabelle_client/socket_communication.py` & `isabelle-client-0.3.9/isabelle_client/socket_communication.py`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.8/isabelle_client/utils.py` & `isabelle-client-0.3.9/isabelle_client/utils.py`

 * *Files identical despite different names*

### Comparing `isabelle-client-0.3.8/pyproject.toml` & `isabelle-client-0.3.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "isabelle-client"
-version = "0.3.8"
+version = "0.3.9"
 description = "A client to Isabelle proof assistant server"
 authors = ["Boris Shminke <boris@shminke.ml>"]
 license = "Apache-2.0"
 repository = "https://github.com/inpefess/isabelle-client"
 readme = "README.rst"
 classifiers=[
 	"Programming Language :: Python :: 3.10",
@@ -37,14 +37,15 @@
 sphinx-autodoc-typehints = "*"
 types-dataclasses = "*"
 jupyterlab = "*"
 pydocstyle = "*"
 tox = "*"
 pyenchant = "*"
 tbump = "*"
+nbconvert = {version = "*", extras = ["webpdf"]}
 
 [tool.black]
 line-length=79
 
 [tool.isort]
 profile = "black"
 src_paths = ["isabelle_client"]
@@ -127,15 +128,15 @@
     pytest
 """
 
 [tool.tbump]
 github_url = "https://github.com/inpfess/isabelle-client/"
 
 [tool.tbump.version]
-current = "0.3.8"
+current = "0.3.9"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   '''
```

### Comparing `isabelle-client-0.3.8/setup.py` & `isabelle-client-0.3.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'isabelle_client': ['resources/*']}
 
 extras_require = \
 {':python_version < "3.9"': ['importlib-resources']}
 
 setup_kwargs = {
     'name': 'isabelle-client',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'A client to Isabelle proof assistant server',
-    'long_description': "|Binder|\\ |PyPI version|\\ |Anaconda version|\\ |CircleCI|\\ |Documentation Status|\\ |codecov|\n\nPython client for Isabelle server\n=================================\n\n``isabelle-client`` is a TCP client for\n`Isabelle <https://isabelle.in.tum.de>`__ server. For more information\nabout the server see part 4 of `the Isabelle system\nmanual <https://isabelle.in.tum.de/dist/Isabelle2021-1/doc/system.pdf>`__.\n\nHow to Install\n==============\n\nThe best way to install this package is to use ``pip``:\n\n.. code:: sh\n\n   pip install isabelle-client\n\n\nAnother option is to use Anaconda:\n\n.. code:: sh\n\t  \n   conda install -c conda-forge isabelle-client \n\nOne can also download and run the client together with Isabelle in a\nDocker contanier:\n\n.. code:: sh\n\n   docker build -t isabelle-client https://github.com/inpefess/isabelle-client.git\n   docker run -it --rm -p 8888:8888 isabelle-client jupyter-lab --ip=0.0.0.0 --port=8888\n\nHow to use\n==========\n\nFollow the `usage\nexample <https://isabelle-client.readthedocs.io/en/latest/usage-example.html#usage-example>`__\nfrom documentation, run the\n`script <https://github.com/inpefess/isabelle-client/blob/master/examples/example.py>`__,\nor use ``isabelle-client`` from a\n`notebook <https://github.com/inpefess/isabelle-client/blob/master/examples/example.ipynb>`__,\ne.g.\xa0with\n`Binder <https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb>`__ (Binder might fail with 'Failed to create temporary user for ...' error which is `well known <https://mybinder-sre.readthedocs.io/en/latest/incident-reports/2018-02-20-jupyterlab-announcement.html>`__ and related neither to ``isabelle-client`` nor to the provided ``Dockerfile``. If that happens, try to run Docker as described in the section above).\n\nHow to Contribute\n=================\n\n`Pull requests <https://github.com/inpefess/isabelle-client/pulls>`__\nare welcome. To start:\n\n.. code:: sh\n\n   git clone https://github.com/inpefess/isabelle-client\n   cd isabelle-client\n   # activate python virtual environment with Python 3.7+\n   pip install -U pip\n   pip install -U setuptools wheel poetry\n   poetry install\n   # recommended but not necessary\n   pre-commit install\n\nTo check the code quality before creating a pull request, one might run\nthe script\n`local-build.sh <https://github.com/inpefess/isabelle-client/blob/master/local-build.sh>`__.\nIt locally does nearly the same as the CI pipeline after the PR is\ncreated.\n\nReporting issues or problems with the software\n==============================================\n\nQuestions and bug reports are welcome on `the\ntracker <https://github.com/inpefess/isabelle-client/issues>`__.\n\nMore documentation\n==================\n\nMore documentation can be found\n`here <https://isabelle-client.readthedocs.io/en/latest>`__.\n\nVideo example\n=============\n\n.. image:: ../_static/tty.gif\n  :alt:\n\n(if not displayed correctly on this page, please watch `here <https://isabelle-client.readthedocs.io/en/latest/#video-example>`__).\n\nHow to cite\n===========\n\nIf you’re writing a research paper, you can cite Isabelle client (and\nIsabelle 2021) using the `following\nDOI <https://doi.org/10.1007/978-3-030-81097-9_20>`__.\n\n.. |PyPI version| image:: https://badge.fury.io/py/isabelle-client.svg\n   :target: https://badge.fury.io/py/isabelle-client\n.. |Anaconda version| image:: https://anaconda.org/conda-forge/isabelle-client/badges/version.svg\n   :target: https://anaconda.org/conda-forge/isabelle-client\n.. |CircleCI| image:: https://circleci.com/gh/inpefess/isabelle-client.svg?style=svg\n   :target: https://circleci.com/gh/inpefess/isabelle-client\n.. |Documentation Status| image:: https://readthedocs.org/projects/isabelle-client/badge/?version=latest\n   :target: https://isabelle-client.readthedocs.io/en/latest/?badge=latest\n.. |codecov| image:: https://codecov.io/gh/inpefess/isabelle-client/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/inpefess/isabelle-client\n.. |Binder| image:: https://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb\n\n",
+    'long_description': "|Binder|\\ |PyPI version|\\ |Anaconda version|\\ |CircleCI|\\ |Documentation Status|\\ |codecov|\n\nPython client for Isabelle server\n=================================\n\n``isabelle-client`` is a TCP client for\n`Isabelle <https://isabelle.in.tum.de>`__ server. For more information\nabout the server see part 4 of `the Isabelle system\nmanual <https://isabelle.in.tum.de/dist/Isabelle2021-1/doc/system.pdf>`__.\n\nHow to Install\n==============\n\nThe best way to install this package is to use ``pip``:\n\n.. code:: sh\n\n   pip install isabelle-client\n\n\nAnother option is to use Anaconda:\n\n.. code:: sh\n\t  \n   conda install -c conda-forge isabelle-client \n\nOne can also download and run the client together with Isabelle in a\nDocker contanier:\n\n.. code:: sh\n\n   docker build -t isabelle-client https://github.com/inpefess/isabelle-client.git\n   docker run -it --rm -p 8888:8888 isabelle-client jupyter-lab --ip=0.0.0.0 --port=8888\n\nHow to use\n==========\n\nFollow the `usage\nexample <https://isabelle-client.readthedocs.io/en/latest/usage-example.html#usage-example>`__\nfrom documentation, run the\n`script <https://github.com/inpefess/isabelle-client/blob/master/examples/example.py>`__,\nor use ``isabelle-client`` from a\n`notebook <https://github.com/inpefess/isabelle-client/blob/master/examples/example.ipynb>`__,\ne.g.\xa0with\n`Binder <https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb>`__ (Binder might fail with 'Failed to create temporary user for ...' error which is `well known <https://mybinder-sre.readthedocs.io/en/latest/incident-reports/2018-02-20-jupyterlab-announcement.html>`__ and related neither to ``isabelle-client`` nor to the provided ``Dockerfile``. If that happens, try to run Docker as described in the section above).\n\nHow to Contribute\n=================\n\n`Pull requests <https://github.com/inpefess/isabelle-client/pulls>`__\nare welcome. To start:\n\n.. code:: sh\n\n   git clone https://github.com/inpefess/isabelle-client\n   cd isabelle-client\n   # activate python virtual environment with Python 3.7+\n   pip install -U pip\n   pip install -U setuptools wheel poetry\n   poetry install\n   # recommended but not necessary\n   pre-commit install\n\nTo check the code quality before creating a pull request, one might run\nthe script\n`local-build.sh <https://github.com/inpefess/isabelle-client/blob/master/local-build.sh>`__.\nIt locally does nearly the same as the CI pipeline after the PR is\ncreated.\n\nReporting issues or problems with the software\n==============================================\n\nQuestions and bug reports are welcome on `the\ntracker <https://github.com/inpefess/isabelle-client/issues>`__.\n\nMore documentation\n==================\n\nMore documentation can be found\n`here <https://isabelle-client.readthedocs.io/en/latest>`__.\n\nVideo example\n=============\n\n.. image:: https://isabelle-client.readthedocs.io/en/latest/_images/tty.gif\n\t   \nHow to cite\n===========\n\nIf you’re writing a research paper, you can cite Isabelle client\nusing the `following DOI\n<https://doi.org/10.1007/978-3-031-16681-5_24>`__. You can also cite\nIsabelle 2021 (and the earlier version of the client) with `this\nDOI <https://doi.org/10.1007/978-3-030-81097-9_20>`__.\n\n.. |PyPI version| image:: https://badge.fury.io/py/isabelle-client.svg\n   :target: https://badge.fury.io/py/isabelle-client\n.. |Anaconda version| image:: https://anaconda.org/conda-forge/isabelle-client/badges/version.svg\n   :target: https://anaconda.org/conda-forge/isabelle-client\n.. |CircleCI| image:: https://circleci.com/gh/inpefess/isabelle-client.svg?style=svg\n   :target: https://circleci.com/gh/inpefess/isabelle-client\n.. |Documentation Status| image:: https://readthedocs.org/projects/isabelle-client/badge/?version=latest\n   :target: https://isabelle-client.readthedocs.io/en/latest/?badge=latest\n.. |codecov| image:: https://codecov.io/gh/inpefess/isabelle-client/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/inpefess/isabelle-client\n.. |Binder| image:: https://mybinder.org/badge_logo.svg\n   :target: https://mybinder.org/v2/gh/inpefess/isabelle-client/HEAD?labpath=isabelle-client-examples/example.ipynb\n\n",
     'author': 'Boris Shminke',
     'author_email': 'boris@shminke.ml',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/inpefess/isabelle-client',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `isabelle-client-0.3.8/PKG-INFO` & `isabelle-client-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isabelle-client
-Version: 0.3.8
+Version: 0.3.9
 Summary: A client to Isabelle proof assistant server
 Home-page: https://github.com/inpefess/isabelle-client
 License: Apache-2.0
 Author: Boris Shminke
 Author-email: boris@shminke.ml
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -104,24 +104,23 @@
 
 More documentation can be found
 `here <https://isabelle-client.readthedocs.io/en/latest>`__.
 
 Video example
 =============
 
-.. image:: ../_static/tty.gif
-  :alt:
-
-(if not displayed correctly on this page, please watch `here <https://isabelle-client.readthedocs.io/en/latest/#video-example>`__).
-
+.. image:: https://isabelle-client.readthedocs.io/en/latest/_images/tty.gif
+	   
 How to cite
 ===========
 
-If you’re writing a research paper, you can cite Isabelle client (and
-Isabelle 2021) using the `following
+If you’re writing a research paper, you can cite Isabelle client
+using the `following DOI
+<https://doi.org/10.1007/978-3-031-16681-5_24>`__. You can also cite
+Isabelle 2021 (and the earlier version of the client) with `this
 DOI <https://doi.org/10.1007/978-3-030-81097-9_20>`__.
 
 .. |PyPI version| image:: https://badge.fury.io/py/isabelle-client.svg
    :target: https://badge.fury.io/py/isabelle-client
 .. |Anaconda version| image:: https://anaconda.org/conda-forge/isabelle-client/badges/version.svg
    :target: https://anaconda.org/conda-forge/isabelle-client
 .. |CircleCI| image:: https://circleci.com/gh/inpefess/isabelle-client.svg?style=svg
```

