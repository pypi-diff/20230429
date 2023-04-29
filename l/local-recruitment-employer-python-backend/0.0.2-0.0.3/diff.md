# Comparing `tmp/local-recruitment-employer-python-backend-0.0.2.tar.gz` & `tmp/local-recruitment-employer-python-backend-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local-recruitment-employer-python-backend-0.0.2.tar", last modified: Fri Apr 28 11:31:17 2023, max compression
+gzip compressed data, was "local-recruitment-employer-python-backend-0.0.3.tar", last modified: Sat Apr 29 10:16:19 2023, max compression
```

## Comparing `local-recruitment-employer-python-backend-0.0.2.tar` & `local-recruitment-employer-python-backend-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:31:17.303832 local-recruitment-employer-python-backend-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-28 11:31:17.303832 local-recruitment-employer-python-backend-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 11:31:04.000000 local-recruitment-employer-python-backend-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:31:17.303832 local-recruitment-employer-python-backend-0.0.2/local_recruitment_employer_python_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-28 11:31:17.000000 local-recruitment-employer-python-backend-0.0.2/local_recruitment_employer_python_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-28 11:31:17.000000 local-recruitment-employer-python-backend-0.0.2/local_recruitment_employer_python_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:31:17.000000 local-recruitment-employer-python-backend-0.0.2/local_recruitment_employer_python_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:31:17.000000 local-recruitment-employer-python-backend-0.0.2/local_recruitment_employer_python_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-28 11:31:04.000000 local-recruitment-employer-python-backend-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:31:17.303832 local-recruitment-employer-python-backend-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 10:16:01.000000 local-recruitment-employer-python-backend-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:16:19.000000 local-recruitment-employer-python-backend-0.0.3/local_recruitment_employer_python_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-29 10:16:01.000000 local-recruitment-employer-python-backend-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:16:19.608783 local-recruitment-employer-python-backend-0.0.3/setup.cfg
```

