# Comparing `tmp/fabric-3.0.0.tar.gz` & `tmp/fabric-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmp62_tyug4/dist/fabric-3.0.0.tar", last modified: Fri Jan 20 23:12:56 2023, max compression
+gzip compressed data, was "/tmp/tmp3qw33273/dist/fabric-3.0.1.tar", last modified: Sat Apr 29 18:59:33 2023, max compression
```

## Comparing `fabric-3.0.0.tar` & `fabric-3.0.1.tar`

### file list

```diff
@@ -1,124 +1,123 @@
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/sites/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/sites/www/
--rw-r--r--   0 jforcier  (1000) users      (100)     2437 2022-07-14 22:37:01.000000 fabric-3.0.0/sites/www/roadmap.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    15214 2023-01-20 23:12:20.000000 fabric-3.0.0/sites/www/changelog.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    51301 2023-01-17 21:10:02.000000 fabric-3.0.0/sites/www/changelog-v1.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     8478 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/www/faq.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2971 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/www/installing-1.x.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      809 2023-01-17 20:15:27.000000 fabric-3.0.0/sites/www/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5768 2022-07-14 22:37:01.000000 fabric-3.0.0/sites/www/installing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2536 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/www/troubleshooting.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2066 2022-07-14 22:37:01.000000 fabric-3.0.0/sites/www/development.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     6814 2022-07-14 22:37:01.000000 fabric-3.0.0/sites/www/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    76327 2023-01-17 20:09:34.000000 fabric-3.0.0/sites/www/upgrading.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1489 2022-07-14 22:37:01.000000 fabric-3.0.0/sites/www/contact.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    32768 2023-01-20 23:12:31.000000 fabric-3.0.0/sites/www/.changelog.rst.swp
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/sites/_shared_static/
--rw-r--r--   0 jforcier  (1000) users      (100)     6401 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/_shared_static/logo.png
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/sites/docs/
--rw-r--r--   0 jforcier  (1000) users      (100)    15384 2023-01-17 20:10:17.000000 fabric-3.0.0/sites/docs/getting-started.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1174 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/index.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     1107 2023-01-17 21:10:02.000000 fabric-3.0.0/sites/docs/conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5010 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/cli.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      260 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/upgrading.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/sites/docs/concepts/
--rw-r--r--   0 jforcier  (1000) users      (100)     4078 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/concepts/authentication.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     3742 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/concepts/networking.rst
--rw-r--r--   0 jforcier  (1000) users      (100)    10159 2023-01-17 20:21:40.000000 fabric-3.0.0/sites/docs/concepts/configuration.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/sites/docs/api/
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/exceptions.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/executor.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       74 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/tunnels.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       56 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/util.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       70 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/group.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      100 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/transfer.rst
--rw-r--r--   0 jforcier  (1000) users      (100)      637 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/testing.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       68 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/runners.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       60 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/tasks.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/connection.rst
--rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.0.0/sites/docs/api/config.rst
--rw-r--r--   0 jforcier  (1000) users      (100)     2393 2023-01-17 20:15:27.000000 fabric-3.0.0/sites/shared_conf.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1457 2022-07-14 22:37:01.000000 fabric-3.0.0/README.rst
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/
--rw-r--r--   0 jforcier  (1000) users      (100)    12204 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)      743 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13902 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4350 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/task.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12849 2023-01-17 21:10:02.000000 fabric-3.0.0/tests/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    59747 2023-01-17 21:44:42.000000 fabric-3.0.0/tests/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1083 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/conftest.py
--rw-r--r--   0 jforcier  (1000) users      (100)     2047 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_util.py
--rw-r--r--   0 jforcier  (1000) users      (100)    11328 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/group.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/_support/
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/_support/ssh_config/
--rw-r--r--   0 jforcier  (1000) users      (100)       97 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/proxyjump_multi.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       83 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/both_proxies.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      178 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/runtime.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       52 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/proxyjump_multi_recursive.conf
--rw-r--r--   0 jforcier  (1000) users      (100)      181 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/runtime_identity.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/system.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/user.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/overridden_hostname.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/proxyjump.conf
--rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/ssh_config/proxyjump_recursive.conf
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/_support/py_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/py_conf/fabric.py
--rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/py_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)      118 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/prompting.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/_support/json_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/json_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)       31 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/json_conf/fabric.json
--rw-r--r--   0 jforcier  (1000) users      (100)     1888 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)      330 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/runtime_fabfile.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/_support/yml_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/yml_conf/fabric.yml
--rw-r--r--   0 jforcier  (1000) users      (100)      455 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/yml_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)      322 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/config.yml
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/tests/_support/yaml_conf/
--rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/_support/yaml_conf/fabfile.py
--rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-04 23:24:42.000000 fabric-3.0.0/tests/_support/yaml_conf/fabric.yaml
--rw-r--r--   0 jforcier  (1000) users      (100)     5455 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1189 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/init.py
--rw-r--r--   0 jforcier  (1000) users      (100)     7105 2023-01-17 20:15:27.000000 fabric-3.0.0/tests/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)      475 2023-01-17 21:17:02.000000 fabric-3.0.0/dev-requirements.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/fabric/
--rw-r--r--   0 jforcier  (1000) users      (100)    14760 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)    44996 2023-01-17 21:46:22.000000 fabric-3.0.0/fabric/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)      139 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/__main__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6695 2023-01-17 20:32:44.000000 fabric-3.0.0/fabric/runners.py
--rw-r--r--   0 jforcier  (1000) users      (100)    13791 2023-01-17 21:10:02.000000 fabric-3.0.0/fabric/config.py
--rw-r--r--   0 jforcier  (1000) users      (100)    12340 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/group.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/fabric/testing/
--rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/testing/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5368 2023-01-17 21:10:55.000000 fabric-3.0.0/fabric/testing/fixtures.py
--rw-r--r--   0 jforcier  (1000) users      (100)    14911 2023-01-17 21:11:39.000000 fabric-3.0.0/fabric/testing/base.py
--rw-r--r--   0 jforcier  (1000) users      (100)      287 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/__init__.py
--rw-r--r--   0 jforcier  (1000) users      (100)      698 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/exceptions.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5512 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/executor.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4654 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/_version.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5415 2023-01-17 21:10:02.000000 fabric-3.0.0/fabric/tunnels.py
--rw-r--r--   0 jforcier  (1000) users      (100)     6610 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/main.py
--rw-r--r--   0 jforcier  (1000) users      (100)     1446 2023-01-17 20:15:27.000000 fabric-3.0.0/fabric/util.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/fabric.egg-info/
--rw-r--r--   0 jforcier  (1000) users      (100)     3524 2023-01-20 23:12:55.000000 fabric-3.0.0/fabric.egg-info/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)       49 2023-01-20 23:12:55.000000 fabric-3.0.0/fabric.egg-info/entry_points.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     2676 2023-01-20 23:12:55.000000 fabric-3.0.0/fabric.egg-info/SOURCES.txt
--rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-01-20 23:12:55.000000 fabric-3.0.0/fabric.egg-info/requires.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-01-20 23:12:55.000000 fabric-3.0.0/fabric.egg-info/dependency_links.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-01-20 23:12:55.000000 fabric-3.0.0/fabric.egg-info/top_level.txt
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/integration/
--rw-r--r--   0 jforcier  (1000) users      (100)     3584 2023-01-17 20:15:27.000000 fabric-3.0.0/integration/concurrency.py
-drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-01-20 23:12:56.000000 fabric-3.0.0/integration/_support/
--rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.0.0/integration/_support/funky-perms.txt
--rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.0.0/integration/_support/file.txt
--rw-r--r--   0 jforcier  (1000) users      (100)     1244 2023-01-17 20:15:27.000000 fabric-3.0.0/integration/group.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3395 2023-01-17 20:15:27.000000 fabric-3.0.0/integration/transfer.py
--rw-r--r--   0 jforcier  (1000) users      (100)     5684 2023-01-17 20:15:27.000000 fabric-3.0.0/integration/connection.py
--rw-r--r--   0 jforcier  (1000) users      (100)     3524 2023-01-20 23:12:56.000000 fabric-3.0.0/PKG-INFO
--rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-04 23:24:42.000000 fabric-3.0.0/LICENSE
--rw-r--r--   0 jforcier  (1000) users      (100)     2857 2023-01-17 20:15:27.000000 fabric-3.0.0/tasks.py
--rw-r--r--   0 jforcier  (1000) users      (100)     4175 2023-01-17 20:15:27.000000 fabric-3.0.0/setup.py
--rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-01-20 23:12:56.000000 fabric-3.0.0/setup.cfg
--rw-r--r--   0 jforcier  (1000) users      (100)      278 2021-12-04 23:24:42.000000 fabric-3.0.0/MANIFEST.in
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/integration/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3395 2023-01-17 20:15:27.000000 fabric-3.0.1/integration/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1244 2023-01-17 20:15:27.000000 fabric-3.0.1/integration/group.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/integration/_support/
+-rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.0.1/integration/_support/funky-perms.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        4 2021-12-04 23:24:42.000000 fabric-3.0.1/integration/_support/file.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     5684 2023-01-20 23:13:54.000000 fabric-3.0.1/integration/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3584 2023-01-20 23:13:54.000000 fabric-3.0.1/integration/concurrency.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     3580 2023-04-29 18:59:33.000000 fabric-3.0.1/PKG-INFO
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/fabric.egg-info/
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/entry_points.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        7 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/top_level.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     2647 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)       57 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/requires.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)        1 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 jforcier  (1000) users      (100)     3580 2023-04-29 18:59:32.000000 fabric-3.0.1/fabric.egg-info/PKG-INFO
+-rw-r--r--   0 jforcier  (1000) users      (100)     4230 2023-04-29 17:40:23.000000 fabric-3.0.1/setup.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2857 2023-01-20 23:13:54.000000 fabric-3.0.1/tasks.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/fabric/
+-rw-r--r--   0 jforcier  (1000) users      (100)    44996 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/connection.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/fabric/testing/
+-rw-r--r--   0 jforcier  (1000) users      (100)    14911 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/testing/base.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5368 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/testing/fixtures.py
+-rw-r--r--   0 jforcier  (1000) users      (100)        0 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/testing/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1446 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6610 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    14760 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5415 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/tunnels.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      139 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/__main__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     6702 2023-04-29 17:52:38.000000 fabric-3.0.1/fabric/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      698 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/exceptions.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    13791 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2023-04-29 18:58:51.000000 fabric-3.0.1/fabric/_version.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4654 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/tasks.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5512 2023-01-17 20:15:27.000000 fabric-3.0.1/fabric/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12340 2023-01-20 23:13:54.000000 fabric-3.0.1/fabric/group.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      287 2023-04-29 17:40:23.000000 fabric-3.0.1/fabric/__init__.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       38 2023-04-29 18:59:33.000000 fabric-3.0.1/setup.cfg
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/
+-rw-r--r--   0 jforcier  (1000) users      (100)    11328 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/group.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/json_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/json_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       31 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/json_conf/fabric.json
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/ssh_config/
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/system.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       52 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump_multi_recursive.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       83 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/both_proxies.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      178 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/runtime.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      181 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/runtime_identity.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       37 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump_recursive.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       49 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/user.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       97 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/proxyjump_multi.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)       51 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/ssh_config/overridden_hostname.conf
+-rw-r--r--   0 jforcier  (1000) users      (100)      118 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/prompting.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      330 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/runtime_fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      322 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/config.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/yml_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)      455 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/yml_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       84 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/yml_conf/fabric.yml
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/yaml_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       19 2021-12-04 23:24:42.000000 fabric-3.0.1/tests/_support/yaml_conf/fabric.yaml
+-rw-r--r--   0 jforcier  (1000) users      (100)       94 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/yaml_conf/fabfile.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/tests/_support/py_conf/
+-rw-r--r--   0 jforcier  (1000) users      (100)       20 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/py_conf/fabric.py
+-rw-r--r--   0 jforcier  (1000) users      (100)       92 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/py_conf/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1888 2023-01-17 20:15:27.000000 fabric-3.0.1/tests/_support/fabfile.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     2047 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/_util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12849 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/config.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5455 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/executor.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1083 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/conftest.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     1189 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/init.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    59747 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/connection.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     7306 2023-04-29 17:52:38.000000 fabric-3.0.1/tests/runners.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    12204 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/transfer.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      743 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/util.py
+-rw-r--r--   0 jforcier  (1000) users      (100)    13902 2023-04-29 17:40:23.000000 fabric-3.0.1/tests/main.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     4350 2023-01-20 23:13:54.000000 fabric-3.0.1/tests/task.py
+-rw-r--r--   0 jforcier  (1000) users      (100)      278 2021-12-04 23:24:42.000000 fabric-3.0.1/MANIFEST.in
+-rw-r--r--   0 jforcier  (1000) users      (100)     1457 2022-07-14 22:37:01.000000 fabric-3.0.1/README.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      417 2023-04-28 15:33:01.000000 fabric-3.0.1/dev-requirements.txt
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/_shared_static/
+-rw-r--r--   0 jforcier  (1000) users      (100)     6401 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/_shared_static/logo.png
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/www/
+-rw-r--r--   0 jforcier  (1000) users      (100)      809 2023-01-17 20:15:27.000000 fabric-3.0.1/sites/www/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     8478 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/www/faq.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     5768 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/installing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    15513 2023-04-29 18:58:49.000000 fabric-3.0.1/sites/www/changelog.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     6814 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1489 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/contact.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2066 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/development.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2536 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/www/troubleshooting.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    76327 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/www/upgrading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2971 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/www/installing-1.x.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2437 2022-07-14 22:37:01.000000 fabric-3.0.1/sites/www/roadmap.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    51301 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/www/changelog-v1.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     2393 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/shared_conf.py
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/docs/
+-rw-r--r--   0 jforcier  (1000) users      (100)     1174 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/index.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1107 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/docs/conf.py
+-rw-r--r--   0 jforcier  (1000) users      (100)     5010 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/cli.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    15384 2023-01-20 23:13:54.000000 fabric-3.0.1/sites/docs/getting-started.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/docs/api/
+-rw-r--r--   0 jforcier  (1000) users      (100)      637 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/testing.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       70 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/group.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/config.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       60 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/tasks.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       68 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/runners.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       72 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/executor.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/connection.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       56 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/util.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       74 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/tunnels.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)       80 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/exceptions.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      100 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/api/transfer.rst
+drwxr-xr-x   0 jforcier  (1000) users      (100)        0 2023-04-29 18:59:33.000000 fabric-3.0.1/sites/docs/concepts/
+-rw-r--r--   0 jforcier  (1000) users      (100)     3742 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/concepts/networking.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     4078 2023-04-29 17:40:23.000000 fabric-3.0.1/sites/docs/concepts/authentication.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)    10159 2023-04-29 17:40:23.000000 fabric-3.0.1/sites/docs/concepts/configuration.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)      260 2021-12-04 23:24:42.000000 fabric-3.0.1/sites/docs/upgrading.rst
+-rw-r--r--   0 jforcier  (1000) users      (100)     1314 2021-12-04 23:24:42.000000 fabric-3.0.1/LICENSE
```

### Comparing `fabric-3.0.0/sites/www/roadmap.rst` & `fabric-3.0.1/sites/www/roadmap.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/changelog.rst` & `fabric-3.0.1/sites/www/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,19 @@
     Keep in mind that Fabric is largely a thin wrapper around `Paramiko
     <https://paramiko.org/changelog.html>`_  and `Invoke
     <https://pyinvoke.org/changelog.html>`_ - just because Fabric itself hasn't
     had a release in a while doesn't mean its capabilities aren't improving!
     Click those projects' names in this paragraph to visit their changelogs and
     see what you might get if you upgrade your dependencies.
 
+- :release:`3.0.1 <2023-04-29>`
+- :bug:`2241` A typo prevented Fabric's command runner from properly calling
+  its superclass ``stop()`` method, which in tandem with a related Invoke bug
+  meant messy or long shutdowns in many scenarios. Thanks to Orlando
+  Rodríguez for report and initial patch.
 - :release:`3.0.0 <2023-01-20>`
 - :bug:`1981 major` (fixed in :issue:`2195`) Automatically close any open SFTP
   session during `fabric.connection.Connection.close`; this avoids issues
   encountered upon re-opening a previously-closed connection object. Thanks to
   Alexander Bodnya for the report and David JM Emmett for the patch.
 - :feature:`-` Change the default configuration value for ``inline_ssh_env``
   from ``False`` to ``True``, to better align with the practicalities of common
```

### Comparing `fabric-3.0.0/sites/www/changelog-v1.rst` & `fabric-3.0.1/sites/www/changelog-v1.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/faq.rst` & `fabric-3.0.1/sites/www/faq.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/installing-1.x.rst` & `fabric-3.0.1/sites/www/installing-1.x.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/conf.py` & `fabric-3.0.1/sites/www/conf.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/installing.rst` & `fabric-3.0.1/sites/www/installing.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/troubleshooting.rst` & `fabric-3.0.1/sites/www/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/development.rst` & `fabric-3.0.1/sites/www/development.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/index.rst` & `fabric-3.0.1/sites/www/index.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/upgrading.rst` & `fabric-3.0.1/sites/www/upgrading.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/www/contact.rst` & `fabric-3.0.1/sites/www/contact.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/_shared_static/logo.png` & `fabric-3.0.1/sites/_shared_static/logo.png`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/getting-started.rst` & `fabric-3.0.1/sites/docs/getting-started.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/index.rst` & `fabric-3.0.1/sites/docs/index.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/conf.py` & `fabric-3.0.1/sites/docs/conf.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/cli.rst` & `fabric-3.0.1/sites/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/concepts/authentication.rst` & `fabric-3.0.1/sites/docs/concepts/authentication.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/concepts/networking.rst` & `fabric-3.0.1/sites/docs/concepts/networking.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/concepts/configuration.rst` & `fabric-3.0.1/sites/docs/concepts/configuration.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/docs/api/testing.rst` & `fabric-3.0.1/sites/docs/api/testing.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/sites/shared_conf.py` & `fabric-3.0.1/sites/shared_conf.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/README.rst` & `fabric-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/transfer.py` & `fabric-3.0.1/tests/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/util.py` & `fabric-3.0.1/tests/util.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/main.py` & `fabric-3.0.1/tests/main.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/task.py` & `fabric-3.0.1/tests/task.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/config.py` & `fabric-3.0.1/tests/config.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/connection.py` & `fabric-3.0.1/tests/connection.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/conftest.py` & `fabric-3.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/_util.py` & `fabric-3.0.1/tests/_util.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/group.py` & `fabric-3.0.1/tests/group.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/_support/fabfile.py` & `fabric-3.0.1/tests/_support/fabfile.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/executor.py` & `fabric-3.0.1/tests/executor.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/init.py` & `fabric-3.0.1/tests/init.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tests/runners.py` & `fabric-3.0.1/tests/runners.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import StringIO
 
 from unittest.mock import Mock, patch
 from pytest import skip  # noqa
 
-from invoke import pty_size, Result
+from invoke import pty_size, Result, Runner
 
 from fabric import Config, Connection, Remote, RemoteShell
 
 
 # On most systems this will explode if actually executed as a shell command;
 # this lets us detect holes in our network mocking.
 CMD = "nope"
@@ -86,14 +86,20 @@
             try:
                 r.run(CMD)
             except Oops:
                 chan.close.assert_called_once_with()
             else:
                 assert False, "Runner failed to raise exception!"
 
+        def stop_calls_super_correctly(self, remote):
+            # RE: #2241
+            Runner.stop = Mock()
+            _runner().run(CMD)
+            Runner.stop.assert_called_once_with()
+
         def channel_close_skipped_when_channel_not_even_made(self):
             # I.e. if obtaining self.channel doesn't even happen (i.e. if
             # Connection.create_session() dies), we need to account for that
             # case...
             class Oops(Exception):
                 pass
```

### Comparing `fabric-3.0.0/fabric/transfer.py` & `fabric-3.0.1/fabric/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/connection.py` & `fabric-3.0.1/fabric/connection.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/runners.py` & `fabric-3.0.1/fabric/runners.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         return self.channel.recv_exit_status()
 
     def generate_result(self, **kwargs):
         kwargs["connection"] = self.context
         return Result(**kwargs)
 
     def stop(self):
-        super()
+        super().stop()
         if hasattr(self, "channel"):
             self.channel.close()
 
     def kill(self):
         # Just close the channel immediately, which is about as close as we can
         # get to a local SIGKILL unfortunately.
         # TODO: consider _also_ calling .send_interrupt() and only doing this
```

### Comparing `fabric-3.0.0/fabric/config.py` & `fabric-3.0.1/fabric/config.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/group.py` & `fabric-3.0.1/fabric/group.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/testing/fixtures.py` & `fabric-3.0.1/fabric/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/testing/base.py` & `fabric-3.0.1/fabric/testing/base.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/exceptions.py` & `fabric-3.0.1/fabric/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/executor.py` & `fabric-3.0.1/fabric/executor.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/tasks.py` & `fabric-3.0.1/fabric/tasks.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/tunnels.py` & `fabric-3.0.1/fabric/tunnels.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/main.py` & `fabric-3.0.1/fabric/main.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric/util.py` & `fabric-3.0.1/fabric/util.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/fabric.egg-info/PKG-INFO` & `fabric-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric
-Version: 3.0.0
+Version: 3.0.1
 Summary: High level SSH command execution
 Home-page: https://fabfile.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.fabfile.org
 Project-URL: Source, https://github.com/fabric/fabric
@@ -54,14 +54,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
```

### Comparing `fabric-3.0.0/fabric.egg-info/SOURCES.txt` & `fabric-3.0.1/fabric.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 sites/docs/api/testing.rst
 sites/docs/api/transfer.rst
 sites/docs/api/tunnels.rst
 sites/docs/api/util.rst
 sites/docs/concepts/authentication.rst
 sites/docs/concepts/configuration.rst
 sites/docs/concepts/networking.rst
-sites/www/.changelog.rst.swp
 sites/www/changelog-v1.rst
 sites/www/changelog.rst
 sites/www/conf.py
 sites/www/contact.rst
 sites/www/development.rst
 sites/www/faq.rst
 sites/www/index.rst
```

### Comparing `fabric-3.0.0/integration/concurrency.py` & `fabric-3.0.1/integration/concurrency.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/integration/group.py` & `fabric-3.0.1/integration/group.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/integration/transfer.py` & `fabric-3.0.1/integration/transfer.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/integration/connection.py` & `fabric-3.0.1/integration/connection.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/PKG-INFO` & `fabric-3.0.1/fabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric
-Version: 3.0.0
+Version: 3.0.1
 Summary: High level SSH command execution
 Home-page: https://fabfile.org
 Author: Jeff Forcier
 Author-email: jeff@bitprophet.org
 License: BSD
 Project-URL: Docs, https://docs.fabfile.org
 Project-URL: Source, https://github.com/fabric/fabric
@@ -54,14 +54,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
```

### Comparing `fabric-3.0.0/LICENSE` & `fabric-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/tasks.py` & `fabric-3.0.1/tasks.py`

 * *Files identical despite different names*

### Comparing `fabric-3.0.0/setup.py` & `fabric-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         "License :: OSI Approved :: BSD License",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development",
```

