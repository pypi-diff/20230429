# Comparing `tmp/oarepo-9.0.8.tar.gz` & `tmp/oarepo-9.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-9.0.8.tar", last modified: Sat Aug  6 07:55:42 2022, max compression
+gzip compressed data, was "oarepo-9.0.9.tar", last modified: Thu Aug 11 08:57:40 2022, max compression
```

## Comparing `oarepo-9.0.8.tar` & `oarepo-9.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 07:55:42.787979 oarepo-9.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-08-06 07:53:17.000000 oarepo-9.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-06 07:53:17.000000 oarepo-9.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-08-06 07:55:42.787979 oarepo-9.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-08-06 07:53:17.000000 oarepo-9.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 07:55:42.787979 oarepo-9.0.8/oarepo/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-06 07:53:17.000000 oarepo-9.0.8/oarepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-06 07:53:17.000000 oarepo-9.0.8/oarepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-06 07:55:42.787979 oarepo-9.0.8/oarepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-08-06 07:55:42.000000 oarepo-9.0.8/oarepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-06 07:55:42.000000 oarepo-9.0.8/oarepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-06 07:55:42.000000 oarepo-9.0.8/oarepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-06 07:55:29.000000 oarepo-9.0.8/oarepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     8032 2022-08-06 07:55:42.000000 oarepo-9.0.8/oarepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-06 07:55:42.000000 oarepo-9.0.8/oarepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-06 07:55:42.787979 oarepo-9.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    13915 2022-08-06 07:53:17.000000 oarepo-9.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:57:40.644108 oarepo-9.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-08-11 08:54:42.000000 oarepo-9.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-08-11 08:54:42.000000 oarepo-9.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-08-11 08:57:40.644108 oarepo-9.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-08-11 08:54:42.000000 oarepo-9.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:57:40.644108 oarepo-9.0.9/oarepo/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-11 08:54:42.000000 oarepo-9.0.9/oarepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-08-11 08:54:42.000000 oarepo-9.0.9/oarepo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-11 08:57:40.644108 oarepo-9.0.9/oarepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-08-11 08:57:40.000000 oarepo-9.0.9/oarepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-08-11 08:57:40.000000 oarepo-9.0.9/oarepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 08:57:40.000000 oarepo-9.0.9/oarepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-11 08:57:22.000000 oarepo-9.0.9/oarepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     8032 2022-08-11 08:57:40.000000 oarepo-9.0.9/oarepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-11 08:57:40.000000 oarepo-9.0.9/oarepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-08-11 08:57:40.644108 oarepo-9.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    13915 2022-08-11 08:54:42.000000 oarepo-9.0.9/setup.py
```

### Comparing `oarepo-9.0.8/LICENSE` & `oarepo-9.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-9.0.8/PKG-INFO` & `oarepo-9.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo
-Version: 9.0.8
+Version: 9.0.9
 Summary: CESNET, UCT Prague and NTK wrapper around Invenio v3.
 Home-page: https://github.com/oarepo/oarepo
 Author: UCT Prague, CESNET z.s.p.o., NTK
 Author-email: miroslav.simek@vscht.cz
 License: MIT
 Keywords: oarepo invenio
 Platform: any
```

### Comparing `oarepo-9.0.8/README.md` & `oarepo-9.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-9.0.8/oarepo.egg-info/PKG-INFO` & `oarepo-9.0.9/oarepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo
-Version: 9.0.8
+Version: 9.0.9
 Summary: CESNET, UCT Prague and NTK wrapper around Invenio v3.
 Home-page: https://github.com/oarepo/oarepo
 Author: UCT Prague, CESNET z.s.p.o., NTK
 Author-email: miroslav.simek@vscht.cz
 License: MIT
 Keywords: oarepo invenio
 Platform: any
```

### Comparing `oarepo-9.0.8/oarepo.egg-info/requires.txt` & `oarepo-9.0.9/oarepo.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 alembic==1.8.1
 amqp==5.1.1
 appdirs==1.4.4
 arrow==1.2.2
-asttokens==2.0.5
+asttokens==2.0.7
 async-timeout==4.0.2
 attrs==22.1.0
 Babel==2.10.3
 backcall==0.2.0
 base32-lib==1.0.2
 beautifulsoup4==4.11.1
 billiard==3.6.4.0
@@ -35,15 +35,15 @@
 dojson==1.4.0
 elasticsearch==7.13.4
 elasticsearch-dsl==7.4.0
 email-validator==1.2.1
 entrypoints==0.4
 executing==0.9.1
 fastjsonschema==2.16.1
-Flask==2.1.3
+Flask==2.2.2
 Flask-Admin==1.6.0
 Flask-Alembic==2.0.1
 Flask-BabelEx==0.9.4
 Flask-Breadcrumbs==0.5.1
 Flask-Caching==2.0.1
 Flask-CeleryExt==0.4.3
 Flask-Collect-Invenio==1.4.0
@@ -71,15 +71,15 @@
 infinity==1.5
 intervals==0.9.2
 invenio-access==1.4.4
 invenio-accounts==2.0.0
 invenio-admin==1.3.2
 invenio-app==1.3.4
 invenio-assets==1.3.0
-invenio-base==1.2.12
+invenio-base==1.2.13
 invenio-cache==1.1.1
 invenio-celery==1.2.4
 invenio-config==1.0.3
 invenio-db==1.0.14
 invenio-files-rest==1.3.3
 invenio-formatter==1.1.3
 invenio-i18n==1.3.2
@@ -123,15 +123,15 @@
 matplotlib-inline==0.1.3
 maxminddb==2.2.0
 maxminddb-geolite2==2018.703
 mistune==0.8.4
 mock==3.0.5
 msgpack==1.0.4
 nbclient==0.6.6
-nbconvert==6.5.0
+nbconvert==6.5.2
 nbformat==5.4.0
 nest-asyncio==1.5.5
 node-semver==0.1.1
 oauthlib==2.1.0
 packaging==21.3
 pandocfilters==1.5.0
 parso==0.8.3
@@ -159,21 +159,21 @@
 pytz==2022.1
 pywebpack==1.2.0
 pyzmq==23.2.0
 redis==4.3.4
 requests==2.28.1
 requests-oauthlib==1.1.0
 requirements-builder==0.4.4
-sentry-sdk==1.9.2
+sentry-sdk==1.9.3
 simplejson==3.17.6
 simplekv==0.14.1
 six==1.16.0
 soupsieve==2.3.2.post1
 speaklater==1.3
-SQLAlchemy==1.4.39
+SQLAlchemy==1.4.40
 SQLAlchemy-Continuum==1.3.12
 SQLAlchemy-Utils==0.38.3
 stack-data==0.3.0
 tinycss2==1.1.1
 tomli==2.0.1
 tornado==6.2
 traitlets==5.3.0
@@ -181,28 +181,28 @@
 uritools==4.0.0
 urllib3==1.26.11
 validators==0.20.0
 vine==5.0.0
 wcwidth==0.2.5
 webargs==5.5.3
 webencodings==0.5.1
-Werkzeug==2.1.2
+Werkzeug==2.2.2
 wrapt==1.14.1
 WTForms==2.3.3
 WTForms-Alchemy==0.18.0
 WTForms-Components==0.10.5
 zipp==3.8.1
 
 [tests]
 alabaster==0.7.12
 alembic==1.8.1
 amqp==5.1.1
 appdirs==1.4.4
 arrow==1.2.2
-asttokens==2.0.5
+asttokens==2.0.7
 async-timeout==4.0.2
 attrs==22.1.0
 Babel==2.10.3
 backcall==0.2.0
 base32-lib==1.0.2
 beautifulsoup4==4.11.1
 billiard==3.6.4.0
@@ -236,15 +236,15 @@
 dojson==1.4.0
 elasticsearch==7.13.4
 elasticsearch-dsl==7.4.0
 email-validator==1.2.1
 entrypoints==0.4
 executing==0.9.1
 fastjsonschema==2.16.1
-Flask==2.1.3
+Flask==2.2.2
 Flask-Admin==1.6.0
 Flask-Alembic==2.0.1
 Flask-BabelEx==0.9.4
 Flask-Breadcrumbs==0.5.1
 Flask-Caching==2.0.1
 Flask-CeleryExt==0.4.3
 Flask-Collect-Invenio==1.4.0
@@ -274,15 +274,15 @@
 iniconfig==1.1.1
 intervals==0.9.2
 invenio-access==1.4.4
 invenio-accounts==2.0.0
 invenio-admin==1.3.2
 invenio-app==1.3.4
 invenio-assets==1.3.0
-invenio-base==1.2.12
+invenio-base==1.2.13
 invenio-cache==1.1.1
 invenio-celery==1.2.4
 invenio-config==1.0.3
 invenio-db==1.0.14
 invenio-files-rest==1.3.3
 invenio-formatter==1.1.3
 invenio-i18n==1.3.2
@@ -328,15 +328,15 @@
 maxminddb==2.2.0
 maxminddb-geolite2==2018.703
 mistune==0.8.4
 mock==3.0.5
 msgpack==1.0.4
 mypy-extensions==0.4.3
 nbclient==0.6.6
-nbconvert==6.5.0
+nbconvert==6.5.2
 nbformat==5.4.0
 nest-asyncio==1.5.5
 node-semver==0.1.1
 oauthlib==2.1.0
 packaging==21.3
 pandocfilters==1.5.0
 parso==0.8.3
@@ -364,42 +364,42 @@
 pynpm==0.1.2
 pyparsing==3.0.9
 pyrsistent==0.18.1
 pytest==6.2.5
 pytest-black==0.3.9
 pytest-cov==3.0.0
 pytest-flask==1.2.0
-pytest-invenio[docs]==1.4.11
+pytest-invenio[docs]==1.4.13
 pytest-isort==3.0.0
 pytest-pycodestyle==2.2.1
 pytest-pydocstyle==2.2.1
 python-dateutil==2.8.2
 pytz==2022.1
 pywebpack==1.2.0
 pyzmq==23.2.0
 redis==4.3.4
 requests==2.28.1
 requests-oauthlib==1.1.0
 requirements-builder==0.4.4
 selenium==3.141.0
-sentry-sdk==1.9.2
+sentry-sdk==1.9.3
 simplejson==3.17.6
 simplekv==0.14.1
 six==1.16.0
 snowballstemmer==2.2.0
 soupsieve==2.3.2.post1
 speaklater==1.3
 Sphinx==5.1.1
 sphinxcontrib-applehelp==1.0.2
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.0
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-SQLAlchemy==1.4.39
+SQLAlchemy==1.4.40
 SQLAlchemy-Continuum==1.3.12
 SQLAlchemy-Utils==0.38.3
 stack-data==0.3.0
 tinycss2==1.1.1
 toml==0.10.2
 tomli==2.0.1
 tornado==6.2
@@ -409,13 +409,13 @@
 uritools==4.0.0
 urllib3==1.26.11
 validators==0.20.0
 vine==5.0.0
 wcwidth==0.2.5
 webargs==5.5.3
 webencodings==0.5.1
-Werkzeug==2.1.2
+Werkzeug==2.2.2
 wrapt==1.14.1
 WTForms==2.3.3
 WTForms-Alchemy==0.18.0
 WTForms-Components==0.10.5
 zipp==3.8.1
```

### Comparing `oarepo-9.0.8/setup.py` & `oarepo-9.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 extras_require = {
     'tests': [
         'alabaster==0.7.12',
         'alembic==1.8.1',
         'amqp==5.1.1',
         'appdirs==1.4.4',
         'arrow==1.2.2',
-        'asttokens==2.0.5',
+        'asttokens==2.0.7',
         'async-timeout==4.0.2',
         'attrs==22.1.0',
         'Babel==2.10.3',
         'backcall==0.2.0',
         'base32-lib==1.0.2',
         'beautifulsoup4==4.11.1',
         'billiard==3.6.4.0',
@@ -59,15 +59,15 @@
         'dojson==1.4.0',
         'elasticsearch==7.13.4',
         'elasticsearch-dsl==7.4.0',
         'email-validator==1.2.1',
         'entrypoints==0.4',
         'executing==0.9.1',
         'fastjsonschema==2.16.1',
-        'Flask==2.1.3',
+        'Flask==2.2.2',
         'Flask-Admin==1.6.0',
         'Flask-Alembic==2.0.1',
         'Flask-BabelEx==0.9.4',
         'Flask-Breadcrumbs==0.5.1',
         'Flask-Caching==2.0.1',
         'Flask-CeleryExt==0.4.3',
         'Flask-Collect-Invenio==1.4.0',
@@ -97,15 +97,15 @@
         'iniconfig==1.1.1',
         'intervals==0.9.2',
         'invenio-access==1.4.4',
         'invenio-accounts==2.0.0',
         'invenio-admin==1.3.2',
         'invenio-app==1.3.4',
         'invenio-assets==1.3.0',
-        'invenio-base==1.2.12',
+        'invenio-base==1.2.13',
         'invenio-cache==1.1.1',
         'invenio-celery==1.2.4',
         'invenio-config==1.0.3',
         'invenio-db==1.0.14',
         'invenio-files-rest==1.3.3',
         'invenio-formatter==1.1.3',
         'invenio-i18n==1.3.2',
@@ -151,15 +151,15 @@
         'maxminddb==2.2.0',
         'maxminddb-geolite2==2018.703',
         'mistune==0.8.4',
         'mock==3.0.5',
         'msgpack==1.0.4',
         'mypy-extensions==0.4.3',
         'nbclient==0.6.6',
-        'nbconvert==6.5.0',
+        'nbconvert==6.5.2',
         'nbformat==5.4.0',
         'nest-asyncio==1.5.5',
         'node-semver==0.1.1',
         'oauthlib==2.1.0',
         'packaging==21.3',
         'pandocfilters==1.5.0',
         'parso==0.8.3',
@@ -187,42 +187,42 @@
         'pynpm==0.1.2',
         'pyparsing==3.0.9',
         'pyrsistent==0.18.1',
         'pytest==6.2.5',
         'pytest-black==0.3.9',
         'pytest-cov==3.0.0',
         'pytest-flask==1.2.0',
-        'pytest-invenio[docs]==1.4.11',
+        'pytest-invenio[docs]==1.4.13',
         'pytest-isort==3.0.0',
         'pytest-pycodestyle==2.2.1',
         'pytest-pydocstyle==2.2.1',
         'python-dateutil==2.8.2',
         'pytz==2022.1',
         'pywebpack==1.2.0',
         'pyzmq==23.2.0',
         'redis==4.3.4',
         'requests==2.28.1',
         'requests-oauthlib==1.1.0',
         'requirements-builder==0.4.4',
         'selenium==3.141.0',
-        'sentry-sdk==1.9.2',
+        'sentry-sdk==1.9.3',
         'simplejson==3.17.6',
         'simplekv==0.14.1',
         'six==1.16.0',
         'snowballstemmer==2.2.0',
         'soupsieve==2.3.2.post1',
         'speaklater==1.3',
         'Sphinx==5.1.1',
         'sphinxcontrib-applehelp==1.0.2',
         'sphinxcontrib-devhelp==1.0.2',
         'sphinxcontrib-htmlhelp==2.0.0',
         'sphinxcontrib-jsmath==1.0.1',
         'sphinxcontrib-qthelp==1.0.3',
         'sphinxcontrib-serializinghtml==1.1.5',
-        'SQLAlchemy==1.4.39',
+        'SQLAlchemy==1.4.40',
         'SQLAlchemy-Continuum==1.3.12',
         'SQLAlchemy-Utils==0.38.3',
         'stack-data==0.3.0',
         'tinycss2==1.1.1',
         'toml==0.10.2',
         'tomli==2.0.1',
         'tornado==6.2',
@@ -232,15 +232,15 @@
         'uritools==4.0.0',
         'urllib3==1.26.11',
         'validators==0.20.0',
         'vine==5.0.0',
         'wcwidth==0.2.5',
         'webargs==5.5.3',
         'webencodings==0.5.1',
-        'Werkzeug==2.1.2',
+        'Werkzeug==2.2.2',
         'wrapt==1.14.1',
         'WTForms==2.3.3',
         'WTForms-Alchemy==0.18.0',
         'WTForms-Components==0.10.5',
         'zipp==3.8.1',
     ]
 }
@@ -250,15 +250,15 @@
 ]
 
 install_requires = [
     'alembic==1.8.1',
     'amqp==5.1.1',
     'appdirs==1.4.4',
     'arrow==1.2.2',
-    'asttokens==2.0.5',
+    'asttokens==2.0.7',
     'async-timeout==4.0.2',
     'attrs==22.1.0',
     'Babel==2.10.3',
     'backcall==0.2.0',
     'base32-lib==1.0.2',
     'beautifulsoup4==4.11.1',
     'billiard==3.6.4.0',
@@ -287,15 +287,15 @@
     'dojson==1.4.0',
     'elasticsearch==7.13.4',
     'elasticsearch-dsl==7.4.0',
     'email-validator==1.2.1',
     'entrypoints==0.4',
     'executing==0.9.1',
     'fastjsonschema==2.16.1',
-    'Flask==2.1.3',
+    'Flask==2.2.2',
     'Flask-Admin==1.6.0',
     'Flask-Alembic==2.0.1',
     'Flask-BabelEx==0.9.4',
     'Flask-Breadcrumbs==0.5.1',
     'Flask-Caching==2.0.1',
     'Flask-CeleryExt==0.4.3',
     'Flask-Collect-Invenio==1.4.0',
@@ -323,15 +323,15 @@
     'infinity==1.5',
     'intervals==0.9.2',
     'invenio-access==1.4.4',
     'invenio-accounts==2.0.0',
     'invenio-admin==1.3.2',
     'invenio-app==1.3.4',
     'invenio-assets==1.3.0',
-    'invenio-base==1.2.12',
+    'invenio-base==1.2.13',
     'invenio-cache==1.1.1',
     'invenio-celery==1.2.4',
     'invenio-config==1.0.3',
     'invenio-db==1.0.14',
     'invenio-files-rest==1.3.3',
     'invenio-formatter==1.1.3',
     'invenio-i18n==1.3.2',
@@ -375,15 +375,15 @@
     'matplotlib-inline==0.1.3',
     'maxminddb==2.2.0',
     'maxminddb-geolite2==2018.703',
     'mistune==0.8.4',
     'mock==3.0.5',
     'msgpack==1.0.4',
     'nbclient==0.6.6',
-    'nbconvert==6.5.0',
+    'nbconvert==6.5.2',
     'nbformat==5.4.0',
     'nest-asyncio==1.5.5',
     'node-semver==0.1.1',
     'oauthlib==2.1.0',
     'packaging==21.3',
     'pandocfilters==1.5.0',
     'parso==0.8.3',
@@ -411,21 +411,21 @@
     'pytz==2022.1',
     'pywebpack==1.2.0',
     'pyzmq==23.2.0',
     'redis==4.3.4',
     'requests==2.28.1',
     'requests-oauthlib==1.1.0',
     'requirements-builder==0.4.4',
-    'sentry-sdk==1.9.2',
+    'sentry-sdk==1.9.3',
     'simplejson==3.17.6',
     'simplekv==0.14.1',
     'six==1.16.0',
     'soupsieve==2.3.2.post1',
     'speaklater==1.3',
-    'SQLAlchemy==1.4.39',
+    'SQLAlchemy==1.4.40',
     'SQLAlchemy-Continuum==1.3.12',
     'SQLAlchemy-Utils==0.38.3',
     'stack-data==0.3.0',
     'tinycss2==1.1.1',
     'tomli==2.0.1',
     'tornado==6.2',
     'traitlets==5.3.0',
@@ -433,15 +433,15 @@
     'uritools==4.0.0',
     'urllib3==1.26.11',
     'validators==0.20.0',
     'vine==5.0.0',
     'wcwidth==0.2.5',
     'webargs==5.5.3',
     'webencodings==0.5.1',
-    'Werkzeug==2.1.2',
+    'Werkzeug==2.2.2',
     'wrapt==1.14.1',
     'WTForms==2.3.3',
     'WTForms-Alchemy==0.18.0',
     'WTForms-Components==0.10.5',
     'zipp==3.8.1',
 ]
```

