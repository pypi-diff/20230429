# Comparing `tmp/rabe_cridlib-0.6.0.tar.gz` & `tmp/rabe_cridlib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabe_cridlib-0.6.0.tar", max compression
+gzip compressed data, was "rabe_cridlib-0.7.0.tar", max compression
```

## Comparing `rabe_cridlib-0.6.0.tar` & `rabe_cridlib-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    34520 2023-02-18 18:30:04.908649 rabe_cridlib-0.6.0/LICENSE
--rw-r--r--   0        0        0     2844 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/README.md
--rw-r--r--   0        0        0      287 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/__init__.py
--rw-r--r--   0        0        0     1419 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/get.py
--rw-r--r--   0        0        0     4567 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/lib.py
--rw-r--r--   0        0        0      221 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/parse.py
--rw-r--r--   0        0        0        0 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/py.typed
--rw-r--r--   0        0        0      192 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/strategy/__init__.py
--rw-r--r--   0        0        0     1305 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/strategy/future.py
--rw-r--r--   0        0        0      620 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/strategy/now.py
--rw-r--r--   0        0        0      791 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/strategy/past.py
--rw-r--r--   0        0        0     1051 2023-02-18 18:30:04.912649 rabe_cridlib-0.6.0/cridlib/util.py
--rw-r--r--   0        0        0     1979 2023-02-18 18:30:22.336506 rabe_cridlib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 rabe_cridlib-0.6.0/setup.py
--rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rabe_cridlib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2844 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/README.md
+-rw-r--r--   0        0        0      343 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/get.py
+-rw-r--r--   0        0        0     4586 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/lib.py
+-rw-r--r--   0        0        0      221 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/parse.py
+-rw-r--r--   0        0        0        0 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/py.typed
+-rw-r--r--   0        0        0      192 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/__init__.py
+-rw-r--r--   0        0        0     1305 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/future.py
+-rw-r--r--   0        0        0      624 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/now.py
+-rw-r--r--   0        0        0      772 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/strategy/past.py
+-rw-r--r--   0        0        0     1051 2023-04-29 08:11:45.072889 rabe_cridlib-0.7.0/cridlib/util.py
+-rw-r--r--   0        0        0     1544 2023-04-29 08:12:02.445325 rabe_cridlib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3835 1970-01-01 00:00:00.000000 rabe_cridlib-0.7.0/PKG-INFO
```

### Comparing `rabe_cridlib-0.6.0/LICENSE` & `rabe_cridlib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.6.0/README.md` & `rabe_cridlib-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.6.0/cridlib/get.py` & `rabe_cridlib-0.7.0/cridlib/get.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.6.0/cridlib/lib.py` & `rabe_cridlib-0.7.0/cridlib/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from urllib.parse import parse_qs
 
 from slugify import slugify
 from uritools import uricompose, urisplit  # type: ignore
 
 
 def canonicalize_show(show: str) -> str:
-    """Get the slug for a show using [python-slugify](https://github.com/un33k/python-slugify).
+    """Get the slug for a show.
+
+    Uses [python-slugify](https://github.com/un33k/python-slugify).
 
     Parameters:
         show: Name of show with non-ascii chars.
     Returns:
         slugified show name.
     """
     return slugify(show)
@@ -58,15 +60,15 @@
 
         Generate a CRID and render it as str:
         ```python
         >>> str(CRID("crid://rabe.ch/v1/test#t=clock=19930301T131200.00Z"))
         'crid://rabe.ch/v1/test#t=clock=19930301T131200.00Z'
 
         ```
-    """
+    """  # noqa: E501
 
     def __init__(self, uri: Optional[str] = None) -> None:
         """
         Parameters:
             uri: CRID URL to base the new CRID off of.
         """
         self._show: Optional[str] = None
```

### Comparing `rabe_cridlib-0.6.0/cridlib/strategy/future.py` & `rabe_cridlib-0.7.0/cridlib/strategy/future.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.6.0/cridlib/strategy/now.py` & `rabe_cridlib-0.7.0/cridlib/strategy/now.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 
 __SONGTICKER_URL = "https://songticker.rabe.ch/songticker/0.9.3/current.xml"
 
 
 def get_show() -> str:
     """Return the currently running show.
 
-    Calls the the [nowplaying](https://github.com/radiorabe/nowplaying) songticker's API.
+    Calls the the [nowplaying](https://github.com/radiorabe/nowplaying)
+    songticker's API.
 
     Returns:
         Name of the currently running show.
     """
 
     _resp = get_session().get(__SONGTICKER_URL, timeout=10)
     _tree = ET.fromstring(_resp.text)
```

### Comparing `rabe_cridlib-0.6.0/cridlib/strategy/past.py` & `rabe_cridlib-0.7.0/cridlib/strategy/past.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,14 @@
     Parameters:
         past: Date to get the show name for.
 
     Returns:
         Show name from the archive for `past`.
     """
 
-    _url = f"{__ARCHIV_BROADCASTS_URL}{past.year}/{past.month:02d}/{past.day:02d}/{past.hour:02d}{past.minute:02d}{past.second:02d}"  # pylint: disable=line-too-long
+    _url = f"{__ARCHIV_BROADCASTS_URL}{past.year}/{past.month:02d}/{past.day:02d}/{past.hour:02d}{past.minute:02d}{past.second:02d}"  # noqa: E501
     _resp = get_session().get(_url, timeout=10)
     _json = _resp.json()
     _data = _json.get("data")
     _label = str(_data[0].get("attributes").get("label"))
 
     return _label.lower().replace(" ", "-")
```

### Comparing `rabe_cridlib-0.6.0/cridlib/util.py` & `rabe_cridlib-0.7.0/cridlib/util.py`

 * *Files identical despite different names*

### Comparing `rabe_cridlib-0.6.0/pyproject.toml` & `rabe_cridlib-0.7.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabe-cridlib"
-version = "v0.6.0" # 0.0.0 placeholder is replaced on release
+version = "v0.7.0" # 0.0.0 placeholder is replaced on release
 description = "Generate CRIDs for RaBe"
 repository = "https://github.com/radiorabe/python-rabe-cridlib"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -22,51 +22,35 @@
 uritools = "^4.0.0"
 pytz = ">=2022.6"
 python-slugify = "^8.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
-wheel = "^0.38.4"
+wheel = ">=0.38.4,<0.41.0"
 types-requests = "^2.28.11"
-flake8 = "^6.0.0"
-flake8-docstrings = "^1.6.0"
-flake8-string-format = "^0.3.0"
-flake8-tuple = "^0.4.1"
 freezegun = "^1.2.2"
 requests-mock = "^1.10.0"
-black = "^22.12.0"
+black = ">=22.12,<24.0"
 isort = "^5.11.4"
 Markdown = "^3.3"
 pytest-mypy = "^0.10.3"
-pytest-pylint = "^0.19.0"
 pytest-random-order = "^1.1.0"
-types-pytz = "^2022.7.0"
-mkdocstrings = {extras = ["python"], version = "^0.20.0"}
-mkdocs-material = "^8"
+types-pytz = ">=2022.7,<2024.0"
+mkdocstrings = {extras = ["python"], version = ">=0.20,<0.22"}
+mkdocs-material = ">=8,<10"
 mkdocs = "^1.4.2"
-mkdocs-gen-files = "^0.4.0"
+mkdocs-gen-files = ">=0.4,<0.6"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
-pytest-pycodestyle = "^2.3.1"
 types-python-slugify = "^8.0.0.0"
 
 [tool.isort]
 profile = "black"
 
-[tool.pylint.messages_control]
-# C0114 = missing-module-docstring
-# C0116 = missing-function-docstring
-disable = ["C0114","C0116"]
-
 [tool.pytest.ini_options]
 minversion = "7.2"
-addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=cridlib --cov-fail-under=100 --pylint --ignore=docs/ --mypy"
-filterwarnings = [
-    "ignore::pytest.PytestRemovedIn8Warning:pytest_pylint",
-    "ignore::DeprecationWarning:pylint",
-    "ignore::DeprecationWarning:pytest_pylint",
-]
+addopts = "-ra -q --random-order --doctest-glob='*.md' --doctest-modules --cov=cridlib --cov-fail-under=100 --ignore=docs/ --mypy"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rabe_cridlib-0.6.0/setup.py` & `rabe_cridlib-0.7.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,115 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rabe-cridlib
+Version: 0.7.0
+Summary: Generate CRIDs for RaBe
+Home-page: https://github.com/radiorabe/python-rabe-cridlib
+License: AGPL-3
+Author: RaBe IT-Reaktion
+Author-email: it@rabe.ch
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: python-slugify (>=8.0.0,<9.0.0)
+Requires-Dist: pytz (>=2022.6)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: uritools (>=4.0.0,<5.0.0)
+Project-URL: Repository, https://github.com/radiorabe/python-rabe-cridlib
+Description-Content-Type: text/markdown
 
-packages = \
-['cridlib', 'cridlib.strategy']
+# RaBe cridlib for Python
 
-package_data = \
-{'': ['*']}
+Generate [RaBe CRIDs](https://github.com/radiorabe/crid-spec) based on several data sources:
 
-install_requires = \
-['python-slugify>=8.0.0,<9.0.0',
- 'pytz>=2022.6',
- 'requests>=2.28.1,<3.0.0',
- 'uritools>=4.0.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'rabe-cridlib',
-    'version': '0.6.0',
-    'description': 'Generate CRIDs for RaBe',
-    'long_description': '# RaBe cridlib for Python\n\nGenerate [RaBe CRIDs](https://github.com/radiorabe/crid-spec) based on several data sources:\n\n* Songticker for current CRID\n* `archiv.rabe.ch` for past CRIDs\n* LibreTime for future CRIDs (currently only data for the next 7 days and only available internally at RaBe)\n\n## Installation\n\n```bash\npoetry add rabe-cridlib\n\n# or on old setup style projects\npip -m install rabe-cridlib\n```\n\n## Usage\n\n```python\n>>> import cridlib\n>>>\n>>> # parse an existing crid\n>>> crid = cridlib.parse("crid://rabe.ch/v1/klangbecken#t=clock=19930301T131200.00Z")\n>>> print(f"version: {crid.version}, show: {crid.show}, start: {crid.start}")\nversion: v1, show: klangbecken, start: 1993-03-01 13:12:00\n\n>>> # get crid for current show\n>>> crid = cridlib.get()\n>>> print(f"version: {crid.version}, show: {crid.show}")  # doctest:+ELLIPSIS\nversion: v1, show: ...\n\n```\n\n## Development\n\n```bash\n# setup a dev env\npython -mvenv env\n. env/bin/activate\n\n# install a modern poetry version\npython -mpip install poetry>=1.2.0\n\n# install deps and dev version\npoetry install\n\n# make changes, run tests\npytest\n```\n\n## Release Management\n\nThe CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).\nThere is a GitHub Action [`semantic-release.yaml` in radiorabe/actions](https://github.com/radiorabe/actions/blob/main/.github/workflows/semantic-release.yaml)\nthat uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new\nreleases.\n\nThe commit message should be structured as follows:\n\n```\n<type>[optional scope]: <description>\n\n[optional body]\n\n[optional footer(s)]\n```\n\nThe commit contains the following structural elements, to communicate intent to the consumers of your library:\n\n1. **fix:** a commit of the type `fix` patches gets released with a PATCH version bump\n1. **feat:** a commit of the type `feat` gets released as a MINOR version bump\n1. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:` gets released as a MAJOR version bump\n1. types other than `fix:` and `feat:` are allowed and don\'t trigger a release\n\nIf a commit does not contain a conventional commit style message you can fix\nit during the squash and merge operation on the PR.\n\nOnce a commit has landed on the `main` branch a release will be created and automatically published to [pypi](https://pypi.org/)\nusing the GitHub Action in [.github/workflows/release.yaml](./.github/workflows/release.yaml) which uses [poetry](https://python-poetry.org/)\nto publish the package to pypi.\n\n## License\n\nThis package is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, version 3 of the License.\n\n## Copyright\n\nCopyright (c) 2022 [Radio Bern RaBe](http://www.rabe.ch)\n',
-    'author': 'RaBe IT-Reaktion',
-    'author_email': 'it@rabe.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/radiorabe/python-rabe-cridlib',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+* Songticker for current CRID
+* `archiv.rabe.ch` for past CRIDs
+* LibreTime for future CRIDs (currently only data for the next 7 days and only available internally at RaBe)
 
+## Installation
+
+```bash
+poetry add rabe-cridlib
+
+# or on old setup style projects
+pip -m install rabe-cridlib
+```
+
+## Usage
+
+```python
+>>> import cridlib
+>>>
+>>> # parse an existing crid
+>>> crid = cridlib.parse("crid://rabe.ch/v1/klangbecken#t=clock=19930301T131200.00Z")
+>>> print(f"version: {crid.version}, show: {crid.show}, start: {crid.start}")
+version: v1, show: klangbecken, start: 1993-03-01 13:12:00
+
+>>> # get crid for current show
+>>> crid = cridlib.get()
+>>> print(f"version: {crid.version}, show: {crid.show}")  # doctest:+ELLIPSIS
+version: v1, show: ...
+
+```
+
+## Development
+
+```bash
+# setup a dev env
+python -mvenv env
+. env/bin/activate
+
+# install a modern poetry version
+python -mpip install poetry>=1.2.0
+
+# install deps and dev version
+poetry install
+
+# make changes, run tests
+pytest
+```
+
+## Release Management
+
+The CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).
+There is a GitHub Action [`semantic-release.yaml` in radiorabe/actions](https://github.com/radiorabe/actions/blob/main/.github/workflows/semantic-release.yaml)
+that uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new
+releases.
+
+The commit message should be structured as follows:
+
+```
+<type>[optional scope]: <description>
+
+[optional body]
+
+[optional footer(s)]
+```
+
+The commit contains the following structural elements, to communicate intent to the consumers of your library:
+
+1. **fix:** a commit of the type `fix` patches gets released with a PATCH version bump
+1. **feat:** a commit of the type `feat` gets released as a MINOR version bump
+1. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:` gets released as a MAJOR version bump
+1. types other than `fix:` and `feat:` are allowed and don't trigger a release
+
+If a commit does not contain a conventional commit style message you can fix
+it during the squash and merge operation on the PR.
+
+Once a commit has landed on the `main` branch a release will be created and automatically published to [pypi](https://pypi.org/)
+using the GitHub Action in [.github/workflows/release.yaml](./.github/workflows/release.yaml) which uses [poetry](https://python-poetry.org/)
+to publish the package to pypi.
+
+## License
+
+This package is free software: you can redistribute it and/or modify it under the terms of the GNU Affero General Public License as published by the Free Software Foundation, version 3 of the License.
+
+## Copyright
+
+Copyright (c) 2022 [Radio Bern RaBe](http://www.rabe.ch)
 
-setup(**setup_kwargs)
```

