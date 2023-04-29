# Comparing `tmp/dev-dependencies-0.0.2.tar.gz` & `tmp/dev-dependencies-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dev-dependencies-0.0.2.tar", last modified: Sat Apr 29 21:34:57 2023, max compression
+gzip compressed data, was "dev-dependencies-0.1.1.tar", last modified: Thu Apr 27 15:06:26 2023, max compression
```

## Comparing `dev-dependencies-0.0.2.tar` & `dev-dependencies-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.envrc
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.075523 dev-dependencies-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    39807 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/dev_dependencies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-29 21:34:57.000000 dev-dependencies-0.0.2/dev_dependencies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-29 21:34:57.000000 dev-dependencies-0.0.2/dev_dependencies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:34:57.000000 dev-dependencies-0.0.2/dev_dependencies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-29 21:34:57.000000 dev-dependencies-0.0.2/dev_dependencies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 21:34:57.000000 dev-dependencies-0.0.2/dev_dependencies.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/devdeps/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/devdeps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-29 21:34:56.000000 dev-dependencies-0.0.2/devdeps/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:34:57.079523 dev-dependencies-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-29 21:34:13.000000 dev-dependencies-0.0.2/tests/test_version.py
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.370403 dev-dependencies-0.1.1/
+-rw-r--r--   0 justinmills   (501) staff       (20)       14 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.envrc
+-rw-r--r--   0 justinmills   (501) staff       (20)      255 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.flake8
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.365117 dev-dependencies-0.1.1/.github/
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.368474 dev-dependencies-0.1.1/.github/workflows/
+-rw-r--r--   0 justinmills   (501) staff       (20)     1223 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.github/workflows/ci.yml
+-rw-r--r--   0 justinmills   (501) staff       (20)      192 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.gitignore
+-rw-r--r--   0 justinmills   (501) staff       (20)        7 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/.python-version
+-rw-r--r--   0 justinmills   (501) staff       (20)     1069 2023-04-26 12:26:45.000000 dev-dependencies-0.1.1/LICENSE
+-rw-r--r--   0 justinmills   (501) staff       (20)      955 2023-04-27 15:06:26.370220 dev-dependencies-0.1.1/PKG-INFO
+-rw-r--r--   0 justinmills   (501) staff       (20)      281 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/Pipfile
+-rw-r--r--   0 justinmills   (501) staff       (20)    38840 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/Pipfile.lock
+-rw-r--r--   0 justinmills   (501) staff       (20)      686 2023-04-27 15:04:07.000000 dev-dependencies-0.1.1/README.md
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369303 dev-dependencies-0.1.1/dev_dependencies.egg-info/
+-rw-r--r--   0 justinmills   (501) staff       (20)      955 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/PKG-INFO
+-rw-r--r--   0 justinmills   (501) staff       (20)      381 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/SOURCES.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)        1 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/dependency_links.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)      120 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/requires.txt
+-rw-r--r--   0 justinmills   (501) staff       (20)        8 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/dev_dependencies.egg-info/top_level.txt
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369710 dev-dependencies-0.1.1/devdeps/
+-rw-r--r--   0 justinmills   (501) staff       (20)      225 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/devdeps/__init__.py
+-rw-r--r--   0 justinmills   (501) staff       (20)      160 2023-04-27 15:06:26.000000 dev-dependencies-0.1.1/devdeps/_version.py
+-rw-r--r--   0 justinmills   (501) staff       (20)     1501 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/pyproject.toml
+-rw-r--r--   0 justinmills   (501) staff       (20)       38 2023-04-27 15:06:26.370456 dev-dependencies-0.1.1/setup.cfg
+drwxr-xr-x   0 justinmills   (501) staff       (20)        0 2023-04-27 15:06:26.369903 dev-dependencies-0.1.1/tests/
+-rw-r--r--   0 justinmills   (501) staff       (20)      273 2023-04-27 14:58:21.000000 dev-dependencies-0.1.1/tests/test_version.py
```

### Comparing `dev-dependencies-0.0.2/.github/workflows/ci.yml` & `dev-dependencies-0.1.1/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 name: Continuous Integration
-run-name: ${{ github.actor }} has pushed content to GitHub
+run-name: ${{ github.actor }} has added a commit trigger this GitHub Actions
 
 on: [push]
 
 jobs:
   continuous-integration:
     runs-on: ubuntu-latest
     steps:
@@ -11,15 +11,14 @@
       - uses: actions/setup-python@v4
         with:
           cache: pipenv
       - name: Install pipenv
         run: curl https://raw.githubusercontent.com/pypa/pipenv/master/get-pipenv.py | python
       - name: Install dependencies
         run: pipenv install --dev
-
       - name: Linting
         run: pipenv run ruff check .
       - name: Formatting
         run: pipenv run black --check .
       - name: Type checking
         run: pipenv run mypy devdeps tests
```

### Comparing `dev-dependencies-0.0.2/LICENSE` & `dev-dependencies-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dev-dependencies-0.0.2/PKG-INFO` & `dev-dependencies-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-dependencies
-Version: 0.0.2
+Version: 0.1.1
 Summary: An opinionated library of dev-time dependencies
 Author: Justin Mills
 License: MIT
 Keywords: library,dependencies
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,17 +35,12 @@
 
 * Tests
 
       pytest
 
 ## Building a package to release
 
-    # Build a distribution (for releases, do this on main with a fresh tag)
     python -m build
 
     # To release that package
     twine upload dist/dev-dependencies-*.tar.gz dist/dev_dependencies-*-py3-none-any.whl
 
-    # To see what the current version will be
-    python -m setuptools_scm
-
-
```

### Comparing `dev-dependencies-0.0.2/Pipfile.lock` & `dev-dependencies-0.1.1/Pipfile.lock`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9808429118773946%*

 * *Differences: {"'default'": "{'platformdirs': {'hashes': "*

 * *              "['sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a', "*

 * *              "'sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad'], "*

 * *              "'version': '==3.4.0'}, delete: ['attrs', 'hypothesis', 'sortedcontainers']}",*

 * * "'develop'": "{'rich': {'hashes': "*

 * *              "['sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a', "*

 * *              "'sha256:b5d573e13605423ec80bdd0cd5f8541f784 […]*

```diff
@@ -12,22 +12,14 @@
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "attrs": {
-            "hashes": [
-                "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
-                "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.1.0"
-        },
         "black": {
             "hashes": [
                 "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
                 "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
                 "sha256:11c410f71b876f961d1de77b9699ad19f939094c3a677323f43d7a29855fe326",
                 "sha256:1c7b8d606e728a41ea1ccbd7264677e494e87cf630e399262ced92d4a8dac940",
                 "sha256:1d06691f1eb8de91cd1b322f21e3bfc9efe0c7ca1f0e1eb1db44ea367dff656b",
@@ -147,22 +139,14 @@
             "hashes": [
                 "sha256:0dfbca3274777792a5bcb2af887a4cad72c72d0e86c94e08e3a3de151bb41c34",
                 "sha256:fe8ea2eca98d8a504f22040d9117347f6b367458366952862ac3586e7d4eeaca"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.3.6"
         },
-        "hypothesis": {
-            "hashes": [
-                "sha256:6f19e61ac13bd35d5271b2788fd51b1e8cc673696b7a353d9a425960113efdbf",
-                "sha256:b933baab6569c6639f6d8e1232ecc9f5388faa0cc5fba15cfc4d3447143b5965"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==6.74.0"
-        },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
@@ -229,19 +213,19 @@
                 "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a",
+                "sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.4.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -372,21 +356,14 @@
                 "sha256:ddf4503595b560bfa5fae92fa2e4cb09ec465ee4cf88cc248f10ad2e956deec3",
                 "sha256:ebc778d95f29c9917e6e7608b2b67815707e6ab8eb5af9341617beda479c3edf",
                 "sha256:ee6c7a77f142c427fa73e1f5f603fc1a39413a36fe6966ed0fc55e97f6921d9c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.0.263"
         },
-        "sortedcontainers": {
-            "hashes": [
-                "sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88",
-                "sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0"
-            ],
-            "version": "==2.4.0"
-        },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
@@ -624,19 +601,19 @@
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
-                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
+                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
+                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.5"
+            "version": "==13.3.4"
         },
         "setuptools": {
             "hashes": [
                 "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
                 "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
             "index": "pypi",
```

### Comparing `dev-dependencies-0.0.2/README.md` & `dev-dependencies-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,17 +24,12 @@
 
 * Tests
 
       pytest
 
 ## Building a package to release
 
-    # Build a distribution (for releases, do this on main with a fresh tag)
     python -m build
 
     # To release that package
     twine upload dist/dev-dependencies-*.tar.gz dist/dev_dependencies-*-py3-none-any.whl
 
-    # To see what the current version will be
-    python -m setuptools_scm
-
-
```

### Comparing `dev-dependencies-0.0.2/dev_dependencies.egg-info/PKG-INFO` & `dev-dependencies-0.1.1/dev_dependencies.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dev-dependencies
-Version: 0.0.2
+Version: 0.1.1
 Summary: An opinionated library of dev-time dependencies
 Author: Justin Mills
 License: MIT
 Keywords: library,dependencies
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -35,17 +35,12 @@
 
 * Tests
 
       pytest
 
 ## Building a package to release
 
-    # Build a distribution (for releases, do this on main with a fresh tag)
     python -m build
 
     # To release that package
     twine upload dist/dev-dependencies-*.tar.gz dist/dev_dependencies-*-py3-none-any.whl
 
-    # To see what the current version will be
-    python -m setuptools_scm
-
-
```

### Comparing `dev-dependencies-0.0.2/pyproject.toml` & `dev-dependencies-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,17 @@
     "black",
     "flake8",
     "flake8-black",
     "ruff",
     "mypy",
     "pydantic",
     "pytest",
-    "pytest-mock",
-    "hypothesis",
     "pytest-cov",
     "pytest-xdist",
+    "pytest-mock",
     "pytest-md",
     "pytest-emoji",
 ]
 dynamic = ["version", "readme"]
 
 [tool.setuptools]
 packages = ["devdeps"]
```

