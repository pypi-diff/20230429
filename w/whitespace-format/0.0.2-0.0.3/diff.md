# Comparing `tmp/whitespace_format-0.0.2.tar.gz` & `tmp/whitespace_format-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitespace_format-0.0.2.tar", max compression
+gzip compressed data, was "whitespace_format-0.0.3.tar", max compression
```

## Comparing `whitespace_format-0.0.2.tar` & `whitespace_format-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1076 2023-02-26 21:48:41.540872 whitespace_format-0.0.2/LICENSE
--rw-r--r--   0        0        0     9242 2023-03-04 21:08:48.517909 whitespace_format-0.0.2/README.md
--rw-r--r--   0        0        0     1506 2023-03-04 21:27:04.533275 whitespace_format-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0    22072 2023-03-04 21:27:15.861330 whitespace_format-0.0.2/whitespace_format.py
--rw-r--r--   0        0        0    10211 1970-01-01 00:00:00.000000 whitespace_format-0.0.2/setup.py
--rw-r--r--   0        0        0    10031 1970-01-01 00:00:00.000000 whitespace_format-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-02-26 21:48:41.540872 whitespace_format-0.0.3/LICENSE
+-rw-r--r--   0        0        0     9346 2023-03-11 18:52:14.254191 whitespace_format-0.0.3/README.md
+-rw-r--r--   0        0        0     1506 2023-04-29 18:51:36.317254 whitespace_format-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0    22072 2023-04-29 18:51:36.317254 whitespace_format-0.0.3/whitespace_format.py
+-rw-r--r--   0        0        0    10317 1970-01-01 00:00:00.000000 whitespace_format-0.0.3/setup.py
+-rw-r--r--   0        0        0    10135 1970-01-01 00:00:00.000000 whitespace_format-0.0.3/PKG-INFO
```

### Comparing `whitespace_format-0.0.2/LICENSE` & `whitespace_format-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `whitespace_format-0.0.2/README.md` & `whitespace_format-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # whitespace-format
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/DavidPal/whitespace-format/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/DavidPal/whitespace-format/tree/main)
 
+![GitHub Action](https://github.com/DavidPal/whitespace-format/actions/workflows/build.yaml/badge.svg)
+
 Linter and formatter for source code files and text files.
 
 The purpose of this tool is to normalize source code files (e.g. Python, Java,
 C/C++, Ruby, Go, JavaScript, etc.) and text files (HTML, JSON, YAML, CSV,
 MarkDown, LaTeX) before checking them into a version control system.
 
 The features include:
```

### Comparing `whitespace_format-0.0.2/pyproject.toml` & `whitespace_format-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whitespace-format"
-version = "0.0.2"
+version = "0.0.3"
 description = "Linter and formatter for source code files and text files"
 license = "MIT"
 authors = ["David Pal <davidko.pal@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/DavidPal/whitespace-format"
 repository = "https://github.com/DavidPal/whitespace-format"
 classifiers = [
@@ -13,25 +13,25 @@
     "Programming Language :: Python :: 3",
 ]
 
 [tool.poetry.scripts]
 whitespace-format = "whitespace_format:main"
 
 [tool.poetry.dependencies]
-python = "^3.7.5"
+python = "^3.7.2"
 
 [tool.poetry.dev-dependencies]
-black = "^23.1.0"
-coverage = "^7.2.1"
+black = "^23.3.0"
+coverage = "^7.2.4"
 flake8 = "^5.0.4"
 flake8-absolute-import = "^1.0.0.1"
 isort = {extras = ["colors"], version = "^5.11.5"}
-mypy = "^1.0.1"
+mypy = "^1.2.0"
 pydocstyle = {extras = ["toml"], version = "^6.3.0"}
-pytest = "^7.2.2"
+pytest = "^7.3.1"
 pylint = "^2.16.3"
 pylint-quotes = "^0.2.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `whitespace_format-0.0.2/whitespace_format.py` & `whitespace_format-0.0.3/whitespace_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import dataclasses
 import pathlib
 import re
 import sys
 from typing import Callable
 from typing import List
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 # Regular expression that does NOT match any string.
 UNMATCHABLE_REGEX = "$."
 
 NEW_LINE_MARKERS = {
     "linux": "\n",
     "windows": "\r\n",
```

### Comparing `whitespace_format-0.0.2/setup.py` & `whitespace_format-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 modules = \
 ['whitespace_format']
 entry_points = \
 {'console_scripts': ['whitespace-format = whitespace_format:main']}
 
 setup_kwargs = {
     'name': 'whitespace-format',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Linter and formatter for source code files and text files',
-    'long_description': '# whitespace-format\n\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/DavidPal/whitespace-format/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/DavidPal/whitespace-format/tree/main)\n\nLinter and formatter for source code files and text files.\n\nThe purpose of this tool is to normalize source code files (e.g. Python, Java,\nC/C++, Ruby, Go, JavaScript, etc.) and text files (HTML, JSON, YAML, CSV,\nMarkDown, LaTeX) before checking them into a version control system.\n\nThe features include:\n\n* Auto-detection of new line markers (Linux `\\n`, Windows `\\r\\r`, Mac `\\r`).\n* Add a new line marker at the end of the file if it is missing.\n* Make new line markers consistent.\n* Remove empty lines at the end of the file.\n* Remove whitespace at the end of each line.\n* Replace tabs with spaces.\n* Remove/replace non-standard whitespace characters.\n\nThe formatting changes are\n[idempotent](https://en.wikipedia.org/wiki/Idempotence), i.e., running the tool\nsecond time (with the same parameters) has no effect.\n\n## Installation\n\n```shell\npip install whitespace-format\n```\n\nInstallation requires Python 3.7.5 or higher.\n\n## Usage\n\nA sample command that formats source code files:\n```shell\nwhitespace-format \\\n    --exclude ".git/|.idea/|.pyc$" \\\n    --new-line-marker linux \\\n    --normalize-new-line-markers \\\n    foo.txt  my_project/\n```\nThe command above formats `foo.txt` and all files contained `my_project/` and\nits subdirectories. Files that contain `.git/` or `.idea/` in their (relative)\npath are excluded. For example, files in `my_project/.git/` and files in\n`my_project/.idea/` are excluded. Likewise, files ending with `*.pyc` are\nexcluded.\n\nIf you want only know if any changes **would be** made, add `--check-only` option:\n```shell\nwhitespace-format \\\n    --exclude ".git/|.idea/|.pyc$" \\\n    --check-only \\\n    --new-line-marker linux \\\n    --normalize-new-line-markers \\\n    foo.txt  my_project/\n```\nThis command can be used as a validation step before checking the source files\ninto a version control system. The command outputs non-zero exit code if any\nof the files would be formatted.\n\n### Options\n\n* `--check-only` -- Do not format files. Only report which files would be formatted.\n* `--follow-symlinks` -- Follow symbolic links when searching for files.\n* `--exclude=REGEX` -- Regular expression that specifies which files to exclude.\nThe regular expression is evaluated on the path of each file.\n* `--verbose` -- Print more messages than normally.\n* `--quiet` -- Do not print any messages, except for errors when reading or writing files.\n\n### Formatting options\n\n* `--add-new-line-marker-at-end-of-file` -- Add missing new line marker at end of each file.\n* `--remove-new-line-marker-from-end-of-file` -- Remove all new line marker(s) from the end of each file.\nThis option is ignored when `--add-new-line-marker-at-end-of-file` is used.\nEmpty lines at the end of the file are removed.\n* `--normalize-new-line-markers` -- Make new line markers consistent in each file\nby replacing `\\\\r\\\\n`, `\\\\n`, and `\\r` with a consistent new line marker.\n* `--remove-trailing-whitespace` -- Remove whitespace at the end of each line.\n* `--remove-trailing-empty-lines` -- Remove empty lines at the end of each file.\n* `--new-line-marker=MARKER` -- This option specifies what new line marker to use.\n`MARKER` must be one of the following:\n  * `auto` -- Use new line marker that is the most common in each individual file.\n  If no new line marker is present in the file, Linux `\\n` is used.\n  This is the default option.\n  * `linux` -- Use Linux new line marker `\\\\n`.\n  * `mac` -- Use Mac new line marker `\\\\r`.\n  * `windows` -- Use Windows new line marker `\\\\r\\\\n`.\n* `--encoding` -- Text encoding for both reading and writing files. Default encoding is `utf-8`.\nList of supported encodings can be found at\nhttps://docs.python.org/3/library/codecs.html#standard-encodings\n\nNote that input files can contain an arbitrary mix of new line markers `\\n`,\n`\\r`, `\\r\\n` even within the same file. The option `--new-line-marker`\nspecifies the character that should be in the formatted file.\n\nAn opinionated combination of options is:\n```shell\nwhitespace-format \\\n    --new-line-marker=linux \\\n    --add-new-line-marker-at-end-of-file \\\n    --normalize-new-line-markers \\\n    --remove-trailing-whitespace \\\n    --remove-trailing-empty-lines \\\n    foo.txt  my_project/\n```\nThis should work well for common programming languages (e.g. Python, Java,\nC/C++, JavaScript) and common text file formats (e.g. CSV, LaTeX, JSON, YAML,\nHTML, MarkDown).\n\n### Empty files\n\nThere are separate options for handling empty files and files consisting of\nwhitespace characters only:\n\n* `--normalize-empty-files=MODE`\n* `--normalize-whitespace-only-files=MODE`\n\nwhere `MODE` is one of the following:\n\n* `ignore` -- Leave the file as is. This is the default option.\n* `empty` -- Replace the file with an empty file.\n* `one-line` -- Replace each file with a file consisting of a single new line marker.\n\nDepending on the mode, an empty file or a whitespace-only file will be either\nignored, replaced by a zero-byte file, or replaced by a file consisting of\nsingle end of line marker.\n\nIf `--normalize-whitespace-only-files` is set to `empty`,\n`--normalize-empty-files setting` set to `empty` as well. In other words,\ncombination `--normalize-whitespace-only-files=empty` and\n`--normalize-empty-files=one-line` is not allowed, since it would lead to\nbehavior that is not idempotent.\n\n### Special characters\n\n* `--replace-tabs-with-spaces=N` -- Replace tabs with spaces.\nWhere is `N` is the number of spaces. If `N` is negative, tabs are not replaced.\nDefault value is `-1`.\n\n* `--normalize-non-standard-whitespace=MODE` -- Replace or remove\nnon-standard whitespace characters (`\\v` and `\\f`). `MODE` must be one of the following:\n  * `ignore` -- Leave `\\v` and `f` as is. This is the default option.\n  * `replace` -- Replace any occurrence of `\\v` or `\\f` with a single space.\n  * `remove` -- Remove all occurrences of `\\v` and `\\f`\n\n## License\n\nMIT\n\n## MacOS development setup\n\n1) Make sure you have [brew](https://brew.sh/) package manager installed.\n\n2) Install [pyenv](https://github.com/pyenv/pyenv), [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)\n   and [poetry](https://python-poetry.org/):\n    ```shell\n    brew install pyenv\n    brew install pyenv-virtualenv\n    brew install poetry\n    ```\n\n3) Create Python virtual environment with the correct Python version:\n   ```shell\n   make install-python\n   make create-environment\n   ```\n\n4) Add the following lines to `.zshrc` or `.bash_profile` and restart the terminal:\n   ```shell\n   # Pyenv settings\n   export PYENV_ROOT="$HOME/.pyenv"\n   export PATH="$PYENV_ROOT/bin:$PATH"\n   eval "$(pyenv init --path)"\n   eval "$(pyenv virtualenv-init -)"\n   ```\n\n5) Install all dependencies\n    ```shell\n    make install-dependecies\n    ```\n\nIf you need to delete the Python virtual environment, you can do so with the\ncommand `make delete-environment`.\n\n## Running unit tests and code checks\n\nIf you make code change, run unit tests and code checks with the command:\n```shell\nmake clean whitespace-format-check isort-check black-check flake8 pydocstyle pylint mypy test coverage\n```\n\nEach make target runs different checks:\n- `clean` deletes temporary files\n- `whitespace-format-check` runs [whitespace-format](https://github.com/DavidPal/whitespace-format) checker on all files\n- `isort-check` runs [isort](https://pycqa.github.io/isort/) checker of imports in `*.py` files\n- `black-check` runs [black](https://github.com/psf/black/) code format checker on `*.py` files\n- `flake8` runs [flake8](https://flake8.pycqa.org/) code style checker on `*.py` files\n- `pydocstyle` runs [pydocstyle](http://www.pydocstyle.org/) docstring checker on `*.py` files\n- `pylint` runs [pylint](https://pylint.org/) code checker on `*.py` files\n- `mypy` runs [mypy](http://mypy-lang.org/) type checker on `*.py` files\n- `test` runs unit tests\n- `coverage` generates code coverage report\n\nYou can automatically format code with the command:\n```shell\nmake isort-format black-format whitespace-format\n```\n\n## Modifying dependencies\n\nThe list of Python packages that this project depends on is specified in\n`pyproject.toml` and in `poetry.lock` files. The file `pyproject.toml` can be\nedited by humans. The file `poetry.lock` is automatically generated by\n`poetry`.\n\nInstall a development dependency with the command:\n```shell\npoetry add --dev <some_new_python_tool>\n```\n\nInstall a new production dependency with the command:\n```shell\npoetry add <some_python_library>\n```\n\n### Manual modification of `pyproject.toml`\n\nInstead of using `poetry add` command, you can edit `pyproject.toml` file. Then,\nregenerate `poetry.lock` file with the command:\n```shell\npoetry lock\n```\nor the command:\n```shell\npoetry lock --no-update\n```\nThe latter command does not update already locked packages.\n\n### Fixing broken Python environment\n\nIf your Python virtual environment becomes broken or polluted with unnecessary\npackages, delete it, recreate it from scratch and install dependencies a fresh\nwith the following commands:\n```shell\nmake delete-environment\nmake create-environment\nmake install-dependencies\n```\n',
+    'long_description': '# whitespace-format\n\n[![CircleCI](https://dl.circleci.com/status-badge/img/gh/DavidPal/whitespace-format/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/DavidPal/whitespace-format/tree/main)\n\n![GitHub Action](https://github.com/DavidPal/whitespace-format/actions/workflows/build.yaml/badge.svg)\n\nLinter and formatter for source code files and text files.\n\nThe purpose of this tool is to normalize source code files (e.g. Python, Java,\nC/C++, Ruby, Go, JavaScript, etc.) and text files (HTML, JSON, YAML, CSV,\nMarkDown, LaTeX) before checking them into a version control system.\n\nThe features include:\n\n* Auto-detection of new line markers (Linux `\\n`, Windows `\\r\\r`, Mac `\\r`).\n* Add a new line marker at the end of the file if it is missing.\n* Make new line markers consistent.\n* Remove empty lines at the end of the file.\n* Remove whitespace at the end of each line.\n* Replace tabs with spaces.\n* Remove/replace non-standard whitespace characters.\n\nThe formatting changes are\n[idempotent](https://en.wikipedia.org/wiki/Idempotence), i.e., running the tool\nsecond time (with the same parameters) has no effect.\n\n## Installation\n\n```shell\npip install whitespace-format\n```\n\nInstallation requires Python 3.7.5 or higher.\n\n## Usage\n\nA sample command that formats source code files:\n```shell\nwhitespace-format \\\n    --exclude ".git/|.idea/|.pyc$" \\\n    --new-line-marker linux \\\n    --normalize-new-line-markers \\\n    foo.txt  my_project/\n```\nThe command above formats `foo.txt` and all files contained `my_project/` and\nits subdirectories. Files that contain `.git/` or `.idea/` in their (relative)\npath are excluded. For example, files in `my_project/.git/` and files in\n`my_project/.idea/` are excluded. Likewise, files ending with `*.pyc` are\nexcluded.\n\nIf you want only know if any changes **would be** made, add `--check-only` option:\n```shell\nwhitespace-format \\\n    --exclude ".git/|.idea/|.pyc$" \\\n    --check-only \\\n    --new-line-marker linux \\\n    --normalize-new-line-markers \\\n    foo.txt  my_project/\n```\nThis command can be used as a validation step before checking the source files\ninto a version control system. The command outputs non-zero exit code if any\nof the files would be formatted.\n\n### Options\n\n* `--check-only` -- Do not format files. Only report which files would be formatted.\n* `--follow-symlinks` -- Follow symbolic links when searching for files.\n* `--exclude=REGEX` -- Regular expression that specifies which files to exclude.\nThe regular expression is evaluated on the path of each file.\n* `--verbose` -- Print more messages than normally.\n* `--quiet` -- Do not print any messages, except for errors when reading or writing files.\n\n### Formatting options\n\n* `--add-new-line-marker-at-end-of-file` -- Add missing new line marker at end of each file.\n* `--remove-new-line-marker-from-end-of-file` -- Remove all new line marker(s) from the end of each file.\nThis option is ignored when `--add-new-line-marker-at-end-of-file` is used.\nEmpty lines at the end of the file are removed.\n* `--normalize-new-line-markers` -- Make new line markers consistent in each file\nby replacing `\\\\r\\\\n`, `\\\\n`, and `\\r` with a consistent new line marker.\n* `--remove-trailing-whitespace` -- Remove whitespace at the end of each line.\n* `--remove-trailing-empty-lines` -- Remove empty lines at the end of each file.\n* `--new-line-marker=MARKER` -- This option specifies what new line marker to use.\n`MARKER` must be one of the following:\n  * `auto` -- Use new line marker that is the most common in each individual file.\n  If no new line marker is present in the file, Linux `\\n` is used.\n  This is the default option.\n  * `linux` -- Use Linux new line marker `\\\\n`.\n  * `mac` -- Use Mac new line marker `\\\\r`.\n  * `windows` -- Use Windows new line marker `\\\\r\\\\n`.\n* `--encoding` -- Text encoding for both reading and writing files. Default encoding is `utf-8`.\nList of supported encodings can be found at\nhttps://docs.python.org/3/library/codecs.html#standard-encodings\n\nNote that input files can contain an arbitrary mix of new line markers `\\n`,\n`\\r`, `\\r\\n` even within the same file. The option `--new-line-marker`\nspecifies the character that should be in the formatted file.\n\nAn opinionated combination of options is:\n```shell\nwhitespace-format \\\n    --new-line-marker=linux \\\n    --add-new-line-marker-at-end-of-file \\\n    --normalize-new-line-markers \\\n    --remove-trailing-whitespace \\\n    --remove-trailing-empty-lines \\\n    foo.txt  my_project/\n```\nThis should work well for common programming languages (e.g. Python, Java,\nC/C++, JavaScript) and common text file formats (e.g. CSV, LaTeX, JSON, YAML,\nHTML, MarkDown).\n\n### Empty files\n\nThere are separate options for handling empty files and files consisting of\nwhitespace characters only:\n\n* `--normalize-empty-files=MODE`\n* `--normalize-whitespace-only-files=MODE`\n\nwhere `MODE` is one of the following:\n\n* `ignore` -- Leave the file as is. This is the default option.\n* `empty` -- Replace the file with an empty file.\n* `one-line` -- Replace each file with a file consisting of a single new line marker.\n\nDepending on the mode, an empty file or a whitespace-only file will be either\nignored, replaced by a zero-byte file, or replaced by a file consisting of\nsingle end of line marker.\n\nIf `--normalize-whitespace-only-files` is set to `empty`,\n`--normalize-empty-files setting` set to `empty` as well. In other words,\ncombination `--normalize-whitespace-only-files=empty` and\n`--normalize-empty-files=one-line` is not allowed, since it would lead to\nbehavior that is not idempotent.\n\n### Special characters\n\n* `--replace-tabs-with-spaces=N` -- Replace tabs with spaces.\nWhere is `N` is the number of spaces. If `N` is negative, tabs are not replaced.\nDefault value is `-1`.\n\n* `--normalize-non-standard-whitespace=MODE` -- Replace or remove\nnon-standard whitespace characters (`\\v` and `\\f`). `MODE` must be one of the following:\n  * `ignore` -- Leave `\\v` and `f` as is. This is the default option.\n  * `replace` -- Replace any occurrence of `\\v` or `\\f` with a single space.\n  * `remove` -- Remove all occurrences of `\\v` and `\\f`\n\n## License\n\nMIT\n\n## MacOS development setup\n\n1) Make sure you have [brew](https://brew.sh/) package manager installed.\n\n2) Install [pyenv](https://github.com/pyenv/pyenv), [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)\n   and [poetry](https://python-poetry.org/):\n    ```shell\n    brew install pyenv\n    brew install pyenv-virtualenv\n    brew install poetry\n    ```\n\n3) Create Python virtual environment with the correct Python version:\n   ```shell\n   make install-python\n   make create-environment\n   ```\n\n4) Add the following lines to `.zshrc` or `.bash_profile` and restart the terminal:\n   ```shell\n   # Pyenv settings\n   export PYENV_ROOT="$HOME/.pyenv"\n   export PATH="$PYENV_ROOT/bin:$PATH"\n   eval "$(pyenv init --path)"\n   eval "$(pyenv virtualenv-init -)"\n   ```\n\n5) Install all dependencies\n    ```shell\n    make install-dependecies\n    ```\n\nIf you need to delete the Python virtual environment, you can do so with the\ncommand `make delete-environment`.\n\n## Running unit tests and code checks\n\nIf you make code change, run unit tests and code checks with the command:\n```shell\nmake clean whitespace-format-check isort-check black-check flake8 pydocstyle pylint mypy test coverage\n```\n\nEach make target runs different checks:\n- `clean` deletes temporary files\n- `whitespace-format-check` runs [whitespace-format](https://github.com/DavidPal/whitespace-format) checker on all files\n- `isort-check` runs [isort](https://pycqa.github.io/isort/) checker of imports in `*.py` files\n- `black-check` runs [black](https://github.com/psf/black/) code format checker on `*.py` files\n- `flake8` runs [flake8](https://flake8.pycqa.org/) code style checker on `*.py` files\n- `pydocstyle` runs [pydocstyle](http://www.pydocstyle.org/) docstring checker on `*.py` files\n- `pylint` runs [pylint](https://pylint.org/) code checker on `*.py` files\n- `mypy` runs [mypy](http://mypy-lang.org/) type checker on `*.py` files\n- `test` runs unit tests\n- `coverage` generates code coverage report\n\nYou can automatically format code with the command:\n```shell\nmake isort-format black-format whitespace-format\n```\n\n## Modifying dependencies\n\nThe list of Python packages that this project depends on is specified in\n`pyproject.toml` and in `poetry.lock` files. The file `pyproject.toml` can be\nedited by humans. The file `poetry.lock` is automatically generated by\n`poetry`.\n\nInstall a development dependency with the command:\n```shell\npoetry add --dev <some_new_python_tool>\n```\n\nInstall a new production dependency with the command:\n```shell\npoetry add <some_python_library>\n```\n\n### Manual modification of `pyproject.toml`\n\nInstead of using `poetry add` command, you can edit `pyproject.toml` file. Then,\nregenerate `poetry.lock` file with the command:\n```shell\npoetry lock\n```\nor the command:\n```shell\npoetry lock --no-update\n```\nThe latter command does not update already locked packages.\n\n### Fixing broken Python environment\n\nIf your Python virtual environment becomes broken or polluted with unnecessary\npackages, delete it, recreate it from scratch and install dependencies a fresh\nwith the following commands:\n```shell\nmake delete-environment\nmake create-environment\nmake install-dependencies\n```\n',
     'author': 'David Pal',
     'author_email': 'davidko.pal@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DavidPal/whitespace-format',
     'py_modules': modules,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.5,<4.0.0',
+    'python_requires': '>=3.7.2,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `whitespace_format-0.0.2/PKG-INFO` & `whitespace_format-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: whitespace-format
-Version: 0.0.2
+Version: 0.0.3
 Summary: Linter and formatter for source code files and text files
 Home-page: https://github.com/DavidPal/whitespace-format
 License: MIT
 Author: David Pal
 Author-email: davidko.pal@gmail.com
-Requires-Python: >=3.7.5,<4.0.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -18,14 +18,16 @@
 Project-URL: Repository, https://github.com/DavidPal/whitespace-format
 Description-Content-Type: text/markdown
 
 # whitespace-format
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/DavidPal/whitespace-format/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/DavidPal/whitespace-format/tree/main)
 
+![GitHub Action](https://github.com/DavidPal/whitespace-format/actions/workflows/build.yaml/badge.svg)
+
 Linter and formatter for source code files and text files.
 
 The purpose of this tool is to normalize source code files (e.g. Python, Java,
 C/C++, Ruby, Go, JavaScript, etc.) and text files (HTML, JSON, YAML, CSV,
 MarkDown, LaTeX) before checking them into a version control system.
 
 The features include:
```

