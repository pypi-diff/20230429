# Comparing `tmp/feed-archiver-2.0.3.tar.gz` & `tmp/feed-archiver-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed-archiver-2.0.3.tar", last modified: Wed Apr 26 22:46:36 2023, max compression
+gzip compressed data, was "feed-archiver-2.0.4.tar", last modified: Sat Apr 29 16:41:33 2023, max compression
```

## Comparing `feed-archiver-2.0.3.tar` & `feed-archiver-2.0.4.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/.dir-locals.el.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.dockerignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.env.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.070369 feed-archiver-2.0.3/.github/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/.github/workflows/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/.github/workflows/build-test.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.gitignore
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4357 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/.pre-commit-config.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/.prospector.yaml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/CONTRIBUTING.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/Dockerfile.devel
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/LICENSE
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    60319 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/Makefile
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      176 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/NEWS-VERSION.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4301 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/NEWS.rst
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    25086 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/README.rst
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/TODO.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/cz-check-bump
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/entrypoint
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/get-base-version
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/bin/hadolint
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/build-host/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/Dockerfile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/Makefile
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/README.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/build-host/bin/
--rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/bin/entrypoint
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py310.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py311.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py37.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py38.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/build-host/requirements-py39.txt
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/build-host/requirements.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/dist/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/dist/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/docker-compose-servarr.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/docker-compose.override.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/gitlab-runner/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/gitlab-runner/config/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/gitlab-runner/config/config.toml.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.3/gitlab-runner/docker-compose.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/home/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/home/.gitignore
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/home/.pypirc.in
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/link-fallbacks.feature.rst
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/nginx/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/nginx/templates/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/nginx/templates/default.conf.template
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2938 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/pyproject.toml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/requirements/build.txt.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py310/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py310/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6246 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py310/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py310/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py311/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py311/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6020 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py311/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py311/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py37/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py37/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6936 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py37/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py37/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py38/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py38/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6286 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py38/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py38/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/requirements/py39/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py39/build.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6273 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py39/devel.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-26 22:06:34.000000 feed-archiver-2.0.3/requirements/py39/user.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/server/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/server/docker-compose.yml
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/setup.cfg
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feed_archiver.egg-info/
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/PKG-INFO
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/entry_points.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/requires.txt
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feed_archiver.egg-info/top_level.txt
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/__main__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/archive.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/enclosures/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/enclosures/__init__.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/enclosures/servarr.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/enclosures/template.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/formats.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/newsfragments/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/newsfragments/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/__init__.py
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/downloads/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty/.gitignore
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-items/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/end-to-end/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink-wo-suffix/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/archives/simple/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.078369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.074369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
-drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-26 22:46:36.082369 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_archive.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_cli.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_download.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_feed.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_linking.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/tests/test_urls.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/src/feedarchiver/utils.py
--rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      160 2023-04-26 22:46:36.000000 feed-archiver-2.0.3/src/feedarchiver/version.py
--rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.3/tox.ini
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      543 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/.dir-locals.el.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/.dockerignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1150 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/.env.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/.github/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/.github/workflows/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3944 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/.github/workflows/build-test.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1733 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/.gitignore
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     4357 2023-04-26 22:06:34.000000 feed-archiver-2.0.4/.gitlab-ci.yml
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      777 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2442 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/.prospector.yaml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4121 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/CONTRIBUTING.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2481 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3218 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/Dockerfile.devel
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1081 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/LICENSE
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    60319 2023-04-26 22:06:34.000000 feed-archiver-2.0.4/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      173 2023-04-29 16:13:44.000000 feed-archiver-2.0.4/NEWS-VERSION.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4475 2023-04-29 16:13:44.000000 feed-archiver-2.0.4/NEWS.rst
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/PKG-INFO
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    25086 2023-04-29 09:13:48.000000 feed-archiver-2.0.4/README.rst
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3758 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/TODO.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2759 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/cz-check-bump
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/entrypoint
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     1101 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/get-base-version
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)      321 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/bin/hadolint
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/build-host/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2002 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/Dockerfile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1476 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/Makefile
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      746 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/README.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/build-host/bin/
+-rwxrwxrwx   0 feed-archiver  (1001) feed-archiver  (1001)     2047 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/build-host/bin/entrypoint
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      730 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py310.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      673 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py311.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      947 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py37.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py38.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      728 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/build-host/requirements-py39.txt
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)        4 2023-04-29 16:01:58.000000 feed-archiver-2.0.4/build-host/requirements.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/dist/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      122 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/dist/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      954 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/docker-compose-servarr.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5769 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/docker-compose.override.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      945 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/gitlab-runner/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/gitlab-runner/config/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1323 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/gitlab-runner/config/config.toml.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      566 2023-04-26 00:51:45.000000 feed-archiver-2.0.4/gitlab-runner/docker-compose.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/home/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       64 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/home/.gitignore
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      327 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/home/.pypirc.in
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      111 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/link-fallbacks.feature.rst
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/nginx/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/nginx/templates/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1086 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/nginx/templates/default.conf.template
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2938 2023-04-29 16:13:44.000000 feed-archiver-2.0.4/pyproject.toml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      668 2023-04-29 16:01:58.000000 feed-archiver-2.0.4/requirements/build.txt.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py310/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2567 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py310/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6244 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py310/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-29 16:02:19.000000 feed-archiver-2.0.4/requirements/py310/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py311/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2529 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py311/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6018 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py311/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1140 2023-04-29 16:03:05.000000 feed-archiver-2.0.4/requirements/py311/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py37/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2840 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py37/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6934 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py37/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1487 2023-04-29 16:03:20.000000 feed-archiver-2.0.4/requirements/py37/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py38/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2668 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py38/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6284 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py38/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-29 16:03:09.000000 feed-archiver-2.0.4/requirements/py38/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/requirements/py39/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     2565 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py39/build.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     6271 2023-04-29 16:12:17.000000 feed-archiver-2.0.4/requirements/py39/devel.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     1138 2023-04-29 16:03:18.000000 feed-archiver-2.0.4/requirements/py39/user.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/server/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4397 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/server/docker-compose.yml
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2152 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/setup.cfg
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feed_archiver.egg-info/
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)    26172 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)     7317 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)        1 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      277 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      345 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/requires.txt
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)       13 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feed_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5287 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      201 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/__main__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    11802 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/archive.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/enclosures/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3371 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/enclosures/__init__.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8155 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/enclosures/servarr.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1968 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/enclosures/template.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    34925 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7074 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/formats.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/newsfragments/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/newsfragments/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     9888 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/__init__.py
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/downloads/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1349 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       32 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty/.gitignore
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       60 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-feeds/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-items/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      337 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/empty-items/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/end-to-end/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      962 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      936 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink-wo-suffix/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      932 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/archives/simple/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      228 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/archives/simple/.feed-archiver.yml
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      243 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episode%3Fapikey=secret%26seriesId=7
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      224 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/episodeFile%3Fapikey=secret%26seriesId=7
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       91 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series/7%3Fapikey=secret
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      105 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/http/localhost%3A8989/api/v3/series%3Fapikey=secret
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    52079 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     5617 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3435 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      405 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/empty-items/orig/https/foo.example.com/podcast/empty.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1186 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)       92 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      831 1980-11-25 08:31:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.175225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      841 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)      989 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1014 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1550 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.179225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/
+drwxr-xr-x   0 feed-archiver  (1001) feed-archiver  (1001)        0 2023-04-29 16:41:33.183225 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     1102 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3286 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_archive.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     4257 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_cli.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    10833 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_download.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)    15051 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_feed.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     7436 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_linking.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     2165 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/tests/test_urls.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     8147 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/src/feedarchiver/utils.py
+-rw-r--r--   0 feed-archiver  (1001) feed-archiver  (1001)      160 2023-04-29 16:41:33.000000 feed-archiver-2.0.4/src/feedarchiver/version.py
+-rw-rw-rw-   0 feed-archiver  (1001) feed-archiver  (1001)     3368 2023-04-24 06:43:00.000000 feed-archiver-2.0.4/tox.ini
```

### Comparing `feed-archiver-2.0.3/.dir-locals.el.in` & `feed-archiver-2.0.4/.dir-locals.el.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/.dockerignore` & `feed-archiver-2.0.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/.env.in` & `feed-archiver-2.0.4/.env.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/.github/workflows/build-test.yml` & `feed-archiver-2.0.4/.github/workflows/build-test.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/.gitignore` & `feed-archiver-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/.gitlab-ci.yml` & `feed-archiver-2.0.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/.pre-commit-config.yaml` & `feed-archiver-2.0.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Run all test, linters and other code checks before committing and pushing.
 fail_fast: true
 repos:
 # Check commit message format and style before pushing to a remote
   - repo: "https://github.com/commitizen-tools/commitizen"
-    rev: "3.1.0"
+    rev: "3.1.1"
     hooks:
       - id: "commitizen"
 # Checks defined in the `./Makefile`
   - repo: "local"
     hooks:
 # Fail fast, run quicker checks first
     - id: "test-push"
```

### Comparing `feed-archiver-2.0.3/.prospector.yaml` & `feed-archiver-2.0.4/.prospector.yaml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/CONTRIBUTING.rst` & `feed-archiver-2.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/Dockerfile` & `feed-archiver-2.0.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/Dockerfile.devel` & `feed-archiver-2.0.4/Dockerfile.devel`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/LICENSE` & `feed-archiver-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/Makefile` & `feed-archiver-2.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/NEWS.rst` & `feed-archiver-2.0.4/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+feed-archiver 2.0.4 (2023-04-29)
+================================
+
+Bugfixes
+--------
+
+- Upgrade all requirements to the latest versions as of Sat Apr 29 16:01:07 UTC 2023.
+
+
 feed-archiver 2.0.3 (2023-04-26)
 ================================
 
 Bugfixes
 --------
 
 - Upgrade all requirements to the latest versions as of Wed Apr 26 05:24:13 PM UTC 2023.
```

### Comparing `feed-archiver-2.0.3/PKG-INFO` & `feed-archiver-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.3
+Version: 2.0.4
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 License-File: LICENSE
 
 ########################################################################################
-feed-archiver
+Feed Archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
```

### Comparing `feed-archiver-2.0.3/README.rst` & `feed-archiver-2.0.4/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ########################################################################################
-feed-archiver
+Feed Archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
```

### Comparing `feed-archiver-2.0.3/TODO.rst` & `feed-archiver-2.0.4/TODO.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/bin/cz-check-bump` & `feed-archiver-2.0.4/bin/cz-check-bump`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/bin/entrypoint` & `feed-archiver-2.0.4/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/bin/get-base-version` & `feed-archiver-2.0.4/bin/get-base-version`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/build-host/Dockerfile` & `feed-archiver-2.0.4/build-host/Dockerfile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/build-host/Makefile` & `feed-archiver-2.0.4/build-host/Makefile`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/build-host/README.rst` & `feed-archiver-2.0.4/build-host/README.rst`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/build-host/bin/entrypoint` & `feed-archiver-2.0.4/build-host/bin/entrypoint`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/build-host/requirements-py310.txt` & `feed-archiver-2.0.4/build-host/requirements-py310.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `feed-archiver-2.0.3/build-host/requirements-py311.txt` & `feed-archiver-2.0.4/build-host/requirements-py311.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `feed-archiver-2.0.3/build-host/requirements-py37.txt` & `feed-archiver-2.0.4/build-host/requirements-py37.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     #   pluggy
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
@@ -40,11 +40,11 @@
 tox==4.5.1
     # via -r build-host/requirements.txt.in
 typing-extensions==4.5.0
     # via
     #   importlib-metadata
     #   platformdirs
     #   tox
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.3/build-host/requirements-py38.txt` & `feed-archiver-2.0.4/build-host/requirements-py38.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `feed-archiver-2.0.3/build-host/requirements-py39.txt` & `feed-archiver-2.0.4/build-host/requirements-py39.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     # via
     #   tox
     #   virtualenv
 packaging==23.1
     # via
     #   pyproject-api
     #   tox
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via tox
 pyproject-api==1.5.1
     # via tox
 tomli==2.0.1
     # via
     #   pyproject-api
     #   tox
 tox==4.5.1
     # via -r build-host/requirements.txt.in
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via tox
```

### Comparing `feed-archiver-2.0.3/docker-compose-servarr.yml` & `feed-archiver-2.0.4/docker-compose-servarr.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/docker-compose.override.yml` & `feed-archiver-2.0.4/docker-compose.override.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/docker-compose.yml` & `feed-archiver-2.0.4/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/gitlab-runner/config/config.toml.in` & `feed-archiver-2.0.4/gitlab-runner/config/config.toml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/gitlab-runner/docker-compose.yml` & `feed-archiver-2.0.4/gitlab-runner/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/nginx/templates/default.conf.template` & `feed-archiver-2.0.4/nginx/templates/default.conf.template`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/pyproject.toml` & `feed-archiver-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [tool.commitizen]
 # Parse commit messages according to conventional commits to decide wether the next
 # versin tag should be a major, minor or patch bump and create the VCS tag.  Also
 # provides VCS hooks to enforce that commit messages comply with conventional commits:
 # https://commitizen-tools.github.io/commitizen/
 name = "cz_conventional_commits"
 changelog_start_rev = "v0.0.0"
-version = "2.0.3"
+version = "2.0.4"
 tag_format = "v$version"
 annotated_tag = true
 gpg_sign = true
 bump_message = """\
 build(release): Version $current_version → $new_version
 
 [actions skip]
```

### Comparing `feed-archiver-2.0.3/requirements/build.txt.in` & `feed-archiver-2.0.4/requirements/build.txt.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/requirements/py310/build.txt` & `feed-archiver-2.0.4/requirements/py310/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py310/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,15 +16,15 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.1.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
@@ -63,15 +63,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -91,37 +91,37 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
 tomli==2.0.1
     # via setuptools-scm
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.3/requirements/py310/devel.txt` & `feed-archiver-2.0.4/requirements/py310/devel.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.4
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -147,15 +147,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -275,40 +275,40 @@
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   towncrier
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.4.29
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.8
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.28.11.17
+types-requests==2.29.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.10
+types-urllib3==1.26.25.11
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   mypy
     #   pydantic
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.3/requirements/py310/user.txt` & `feed-archiver-2.0.4/requirements/py310/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/requirements/py311/build.txt` & `feed-archiver-2.0.4/requirements/py311/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py311/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,15 +16,15 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.1.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
@@ -63,15 +63,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -91,35 +91,35 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.3/requirements/py311/devel.txt` & `feed-archiver-2.0.4/requirements/py311/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.4
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -145,15 +145,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -262,39 +262,39 @@
 tenacity==8.2.2
     # via feed-archiver (pyproject.toml)
 toml==0.10.2
     # via
     #   prospector
     #   requirements-detector
     #   vulture
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.4.29
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.8
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.28.11.17
+types-requests==2.29.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.10
+types-urllib3==1.26.25.11
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   mypy
     #   pydantic
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.3/requirements/py311/user.txt` & `feed-archiver-2.0.4/requirements/py311/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/requirements/py37/build.txt` & `feed-archiver-2.0.4/requirements/py37/build.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.7
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py37/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,15 +16,15 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.1.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
@@ -69,15 +69,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via virtualenv
 pre-commit==2.21.0
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -97,27 +97,27 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
 tomli==2.0.1
     # via setuptools-scm
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   commitizen
     #   importlib-metadata
```

### Comparing `feed-archiver-2.0.3/requirements/py37/devel.txt` & `feed-archiver-2.0.4/requirements/py37/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.4
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -164,15 +164,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==2.21.0
@@ -292,34 +292,34 @@
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   towncrier
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.4.29
     # via pyroma
 typed-ast==1.5.4
     # via
     #   astroid
     #   black
     #   mypy
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.8
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.28.11.17
+types-requests==2.29.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.10
+types-urllib3==1.26.25.11
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   anyio
     #   astroid
     #   black
     #   gitpython
```

### Comparing `feed-archiver-2.0.3/requirements/py37/user.txt` & `feed-archiver-2.0.4/requirements/py37/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/requirements/py38/build.txt` & `feed-archiver-2.0.4/requirements/py38/build.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py38/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,15 +16,15 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.1.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
@@ -65,15 +65,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -93,39 +93,39 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
 tomli==2.0.1
     # via setuptools-scm
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via
     #   rich
     #   setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via
```

### Comparing `feed-archiver-2.0.3/requirements/py38/devel.txt` & `feed-archiver-2.0.4/requirements/py38/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.4
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -147,15 +147,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -275,43 +275,43 @@
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   towncrier
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.4.29
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.8
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.28.11.17
+types-requests==2.29.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.10
+types-urllib3==1.26.25.11
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
     #   rich
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.3/requirements/py38/user.txt` & `feed-archiver-2.0.4/requirements/py38/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/requirements/py39/build.txt` & `feed-archiver-2.0.4/requirements/py39/build.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/py39/build.txt --resolver=backtracking requirements/build.txt.in
 #
-argcomplete==2.1.2
+argcomplete==3.0.8
     # via commitizen
 bleach==6.0.0
     # via readme-renderer
 certifi==2022.12.7
     # via requests
 cffi==1.15.1
     # via cryptography
@@ -16,15 +16,15 @@
     # via pre-commit
 charset-normalizer==3.1.0
     # via
     #   commitizen
     #   requests
 colorama==0.4.6
     # via commitizen
-commitizen==3.1.0
+commitizen==3.1.1
     # via -r requirements/build.txt.in
 cryptography==40.0.2
     # via secretstorage
 decli==0.5.2
     # via commitizen
 distlib==0.3.6
     # via virtualenv
@@ -63,15 +63,15 @@
     # via pre-commit
 packaging==23.1
     # via
     #   commitizen
     #   setuptools-scm
 pkginfo==1.9.6
     # via twine
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via virtualenv
 pre-commit==3.2.2
     # via -r requirements/build.txt.in
 prompt-toolkit==3.0.38
     # via questionary
 pycparser==2.21
     # via cffi
@@ -91,37 +91,37 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 setuptools-scm==7.1.0
     # via -r requirements/build.txt.in
 six==1.16.0
     # via bleach
 termcolor==2.3.0
     # via commitizen
 tomli==2.0.1
     # via setuptools-scm
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via commitizen
 twine==4.0.2
     # via -r requirements/build.txt.in
 typing-extensions==4.5.0
     # via setuptools-scm
 urllib3==1.26.15
     # via
     #   requests
     #   twine
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 wcwidth==0.2.6
     # via prompt-toolkit
 webencodings==0.5.1
     # via bleach
 zipp==3.15.0
     # via importlib-metadata
```

### Comparing `feed-archiver-2.0.3/requirements/py39/devel.txt` & `feed-archiver-2.0.4/requirements/py39/devel.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     # via towncrier
 colorama==0.4.6
     # via
     #   radon
     #   typer
 commonmark==0.9.1
     # via rich
-coverage==7.2.3
+coverage==7.2.4
     # via feed-archiver (pyproject.toml)
 dill==0.3.6
     # via pylint
 distlib==0.3.6
     # via virtualenv
 docutils==0.19
     # via
@@ -147,15 +147,15 @@
     # via stevedore
 pep8==1.7.1
     # via flake8
 pep8-naming==0.10.0
     # via prospector
 pip-tools==6.13.0
     # via feed-archiver (pyproject.toml)
-platformdirs==3.4.0
+platformdirs==3.5.0
     # via
     #   black
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==3.2.2
@@ -275,42 +275,42 @@
     #   black
     #   build
     #   mypy
     #   pylint
     #   pyproject-hooks
     #   pytest
     #   towncrier
-tomlkit==0.11.7
+tomlkit==0.11.8
     # via pylint
 towncrier==22.12.0
     # via feed-archiver (pyproject.toml)
-trove-classifiers==2023.4.25
+trove-classifiers==2023.4.29
     # via pyroma
 typer[all]==0.7.0
     # via rstcheck
-types-docutils==0.19.1.7
+types-docutils==0.19.1.8
     # via rstcheck-core
 types-pyyaml==6.0.12.9
     # via feed-archiver (pyproject.toml)
-types-requests==2.28.11.17
+types-requests==2.29.0.0
     # via feed-archiver (pyproject.toml)
-types-urllib3==1.26.25.10
+types-urllib3==1.26.25.11
     # via types-requests
 typing-extensions==4.5.0
     # via
     #   astroid
     #   black
     #   mypy
     #   pydantic
     #   pylint
 urllib3==1.26.15
     # via requests
 user-agent==0.1.10
     # via feed-archiver (pyproject.toml)
-virtualenv==20.22.0
+virtualenv==20.23.0
     # via pre-commit
 vulture==2.7
     # via prospector
 wheel==0.40.0
     # via pip-tools
 wrapt==1.15.0
     # via astroid
```

### Comparing `feed-archiver-2.0.3/requirements/py39/user.txt` & `feed-archiver-2.0.4/requirements/py39/user.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/server/docker-compose.yml` & `feed-archiver-2.0.4/server/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/setup.cfg` & `feed-archiver-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feed_archiver.egg-info/PKG-INFO` & `feed-archiver-2.0.4/src/feed_archiver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed-archiver
-Version: 2.0.3
+Version: 2.0.4
 Summary: Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 Home-page: https://gitlab.com/rpatterson/feed-archiver
 Author: Ross Patterson
 Author-email: me@rpatterson.net
 License: MIT
 Keywords: feeds,syndication,rss,atom,podcasts,enclosures
 Classifier: Development Status :: 4 - Beta
@@ -23,15 +23,15 @@
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: devel
 License-File: LICENSE
 
 ########################################################################################
-feed-archiver
+Feed Archiver
 ########################################################################################
 Archive the full contents of RSS/Atom syndication feeds including enclosures and assets.
 ****************************************************************************************
 
 .. list-table::
    :class: borderless align-right
```

### Comparing `feed-archiver-2.0.3/src/feed_archiver.egg-info/SOURCES.txt` & `feed-archiver-2.0.4/src/feed_archiver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/__init__.py` & `feed-archiver-2.0.4/src/feedarchiver/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/archive.py` & `feed-archiver-2.0.4/src/feedarchiver/archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/enclosures/__init__.py` & `feed-archiver-2.0.4/src/feedarchiver/enclosures/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/enclosures/servarr.py` & `feed-archiver-2.0.4/src/feedarchiver/enclosures/servarr.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/enclosures/template.py` & `feed-archiver-2.0.4/src/feedarchiver/enclosures/template.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/feed.py` & `feed-archiver-2.0.4/src/feedarchiver/feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/formats.py` & `feed-archiver-2.0.4/src/feedarchiver/formats.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/__init__.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml` & `feed-archiver-2.0.4/src/feedarchiver/tests/archives/downloads/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in` & `feed-archiver-2.0.4/src/feedarchiver/tests/archives/end-to-end/.feed-archiver.yml.in`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink/.feed-archiver.yml` & `feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml` & `feed-archiver-2.0.4/src/feedarchiver/tests/archives/relink-wo-suffix/.feed-archiver.yml`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/bar.example.com/media/el-ni%25C3%25B1o.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/common-id.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/bah-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/el-ni%25C3%25B1o.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/el-ni%25C3%25B1o-episode-title/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/fred-episode-title/download`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/episodes/garply-bonus-episode/download.mp3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/feed.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/image.png`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/downloads/orig/https/foo.example.com/podcast/index.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/added-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/empty/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/orig/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/removed-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/1`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/2`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/blog/post/3`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/http/www.example.com/main.html`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/foo-username%3Asecret@grault.example.com/feeds/garply%3Fbar=qux%252Fbaz#corge.rss`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo` & `feed-archiver-2.0.4/src/feedarchiver/tests/remotes/simple/reordered-item/https/waldo.example.com/feeds/waldo`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/test_archive.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/test_cli.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/test_download.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/test_feed.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/test_linking.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/tests/test_urls.py` & `feed-archiver-2.0.4/src/feedarchiver/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/src/feedarchiver/utils.py` & `feed-archiver-2.0.4/src/feedarchiver/utils.py`

 * *Files identical despite different names*

### Comparing `feed-archiver-2.0.3/tox.ini` & `feed-archiver-2.0.4/tox.ini`

 * *Files identical despite different names*

