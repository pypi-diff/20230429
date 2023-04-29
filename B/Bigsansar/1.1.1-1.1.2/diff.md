# Comparing `tmp/Bigsansar-1.1.1.tar.gz` & `tmp/Bigsansar-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.1.1.tar", last modified: Sat Apr 29 08:56:33 2023, max compression
+gzip compressed data, was "Bigsansar-1.1.2.tar", last modified: Sat Apr 29 09:22:59 2023, max compression
```

## Comparing `Bigsansar-1.1.1.tar` & `Bigsansar-1.1.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.774030 Bigsansar-1.1.1/
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.754030 Bigsansar-1.1.1/Bigsansar.egg-info/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2830 2023-04-29 08:56:33.000000 Bigsansar-1.1.1/Bigsansar.egg-info/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2254 2023-04-29 08:56:33.000000 Bigsansar-1.1.1/Bigsansar.egg-info/SOURCES.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-04-29 08:56:33.000000 Bigsansar-1.1.1/Bigsansar.egg-info/dependency_links.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-04-29 08:56:33.000000 Bigsansar-1.1.1/Bigsansar.egg-info/entry_points.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-04-29 08:56:33.000000 Bigsansar-1.1.1/Bigsansar.egg-info/requires.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-04-29 08:56:33.000000 Bigsansar-1.1.1/Bigsansar.egg-info/top_level.txt
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/LICENSE
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2830 2023-04-29 08:56:33.774030 Bigsansar-1.1.1/PKG-INFO
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2195 2023-04-29 08:23:46.000000 Bigsansar-1.1.1/README.md
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.754030 Bigsansar-1.1.1/bigsansar/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.754030 Bigsansar-1.1.1/bigsansar/contrib/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.754030 Bigsansar-1.1.1/bigsansar/contrib/account/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.754030 Bigsansar-1.1.1/bigsansar/contrib/account/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/signals.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.754030 Bigsansar-1.1.1/bigsansar/contrib/account/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/account/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/contrib/blogs/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/apps.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/contrib/blogs/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2272 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1572 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/models.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/blogs/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/contrib/sites/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/admin.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/apps.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3018 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/forms.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/contrib/sites/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1826 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/contrib/sites/templatetags/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/templatetags/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/templatetags/pages.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/contrib/sites/views.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/core/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/core/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/core/host.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8722 2023-04-29 08:30:09.000000 Bigsansar-1.1.1/bigsansar/core/init.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/main.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/management/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/management/__init__.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/management/commands/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/management/commands/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.1.1/bigsansar/management/commands/createuser.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/migrations/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/migrations/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/models.py
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.764030 Bigsansar-1.1.1/bigsansar/static/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/static/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/static/logo.png
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/static/style.css
-drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 08:56:33.774030 Bigsansar-1.1.1/bigsansar/templates/
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/404.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/__init__.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/acc_active_email.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/base.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/default.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/defaultpage.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/nav.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/templates/parking.html
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/tests.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.1.1/bigsansar/urls.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1864 2023-04-28 15:30:13.000000 Bigsansar-1.1.1/bigsansar/views.py
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-04-29 08:56:33.774030 Bigsansar-1.1.1/setup.cfg
--rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-04-29 08:56:15.000000 Bigsansar-1.1.1/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.024026 Bigsansar-1.1.2/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:58.994027 Bigsansar-1.1.2/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2986 2023-04-29 09:22:58.000000 Bigsansar-1.1.2/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2254 2023-04-29 09:22:58.000000 Bigsansar-1.1.2/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-04-29 09:22:58.000000 Bigsansar-1.1.2/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-04-29 09:22:58.000000 Bigsansar-1.1.2/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-04-29 09:22:58.000000 Bigsansar-1.1.2/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-04-29 09:22:58.000000 Bigsansar-1.1.2/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2986 2023-04-29 09:22:59.024026 Bigsansar-1.1.2/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2363 2023-04-29 09:22:07.000000 Bigsansar-1.1.2/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:58.994027 Bigsansar-1.1.2/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.004027 Bigsansar-1.1.2/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.004027 Bigsansar-1.1.2/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.004027 Bigsansar-1.1.2/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.004027 Bigsansar-1.1.2/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.004027 Bigsansar-1.1.2/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.004027 Bigsansar-1.1.2/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2272 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1572 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3018 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1826 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     8722 2023-04-29 08:30:09.000000 Bigsansar-1.1.2/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.1.2/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.014026 Bigsansar-1.1.2/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/static/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 09:22:59.024026 Bigsansar-1.1.2/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/nav.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.1.2/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1881 2023-04-29 09:17:07.000000 Bigsansar-1.1.2/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-04-29 09:22:59.024026 Bigsansar-1.1.2/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-04-29 09:22:38.000000 Bigsansar-1.1.2/setup.py
```

### Comparing `Bigsansar-1.1.1/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.1.2/Bigsansar.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.1.1
+Version: 1.1.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -69,27 +69,39 @@
 * added setting for postgres 
 * added sercure proxy ssl header 
 * fixed domain index and pages views system
 * added virtual host in to admin pannel 
 * added pages system and working in this model 
 
 
-## Load page in templates
+## Load page list in templates
 
 `{% load pages %}
 
 {% get_pages  as listpage %}
 {% for page in listpage %}
 <div>
     < a href="{{ page.slug }}">{{ page.title }}</a>
 </div>
 {% endfor %}`
 
-#### More variable for **page**
+
+#### More variable for **page** list
 * page.id
 * page.domain
 * page.title
 * page.slug
 * page.body
 * page.visitor
 * page.publish_date
 
+
+## for single page title
+* getpage.id
+* getpage.domain
+* getpage.title
+* getpage.slug
+* getpage.body
+* getpage.visitor
+* getpage.publish_date
+
+
```

### Comparing `Bigsansar-1.1.1/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.1.2/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/LICENSE` & `Bigsansar-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/PKG-INFO` & `Bigsansar-1.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bigsansar
-Version: 1.1.1
+Version: 1.1.2
 Summary: Build one in minutes with bigsansar - a visual site building tool!
 Home-page: https://bigsansar.com
 Author: Bikash Pokhrel
 Author-email: bigsansaroffice@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
 Project-URL: Documentations, https://docs.bigsansar.com/
@@ -69,27 +69,39 @@
 * added setting for postgres 
 * added sercure proxy ssl header 
 * fixed domain index and pages views system
 * added virtual host in to admin pannel 
 * added pages system and working in this model 
 
 
-## Load page in templates
+## Load page list in templates
 
 `{% load pages %}
 
 {% get_pages  as listpage %}
 {% for page in listpage %}
 <div>
     < a href="{{ page.slug }}">{{ page.title }}</a>
 </div>
 {% endfor %}`
 
-#### More variable for **page**
+
+#### More variable for **page** list
 * page.id
 * page.domain
 * page.title
 * page.slug
 * page.body
 * page.visitor
 * page.publish_date
 
+
+## for single page title
+* getpage.id
+* getpage.domain
+* getpage.title
+* getpage.slug
+* getpage.body
+* getpage.visitor
+* getpage.publish_date
+
+
```

### Comparing `Bigsansar-1.1.1/README.md` & `Bigsansar-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -50,26 +50,37 @@
 * added setting for postgres 
 * added sercure proxy ssl header 
 * fixed domain index and pages views system
 * added virtual host in to admin pannel 
 * added pages system and working in this model 
 
 
-## Load page in templates
+## Load page list in templates
 
 `{% load pages %}
 
 {% get_pages  as listpage %}
 {% for page in listpage %}
 <div>
     < a href="{{ page.slug }}">{{ page.title }}</a>
 </div>
 {% endfor %}`
 
-#### More variable for **page**
+
+#### More variable for **page** list
 * page.id
 * page.domain
 * page.title
 * page.slug
 * page.body
 * page.visitor
-* page.publish_date
+* page.publish_date
+
+
+## for single page title
+* getpage.id
+* getpage.domain
+* getpage.title
+* getpage.slug
+* getpage.body
+* getpage.visitor
+* getpage.publish_date
```

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/account/forms.py` & `Bigsansar-1.1.2/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.1.2/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/account/models.py` & `Bigsansar-1.1.2/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.1.2/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.1.2/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.1.2/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.1.2/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.1.2/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.1.2/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/contrib/sites/models.py` & `Bigsansar-1.1.2/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/core/__init__.py` & `Bigsansar-1.1.2/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/core/init.py` & `Bigsansar-1.1.2/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/management/commands/createuser.py` & `Bigsansar-1.1.2/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/static/logo.png` & `Bigsansar-1.1.2/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/static/style.css` & `Bigsansar-1.1.2/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/templates/404.html` & `Bigsansar-1.1.2/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/templates/base.html` & `Bigsansar-1.1.2/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/templates/default.html` & `Bigsansar-1.1.2/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/templates/defaultpage.html` & `Bigsansar-1.1.2/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/templates/nav.html` & `Bigsansar-1.1.2/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/templates/parking.html` & `Bigsansar-1.1.2/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/urls.py` & `Bigsansar-1.1.2/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.1.1/bigsansar/views.py` & `Bigsansar-1.1.2/bigsansar/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,8 +49,8 @@
 
         return render(request, '404.html')
 
     else:
         asp = 'templates/' + str(db.id) + '/' + page.slug + '.html'
         full_url = os.path.join(BASE_DIR, asp)
         template = loader.select_template((full_url, default_page))
-        return HttpResponse(template.render({'path': url}, request))
+        return HttpResponse(template.render({'path': url, 'getpage': page}, request))
```

### Comparing `Bigsansar-1.1.1/setup.py` & `Bigsansar-1.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.1.1",
+    version="1.1.2",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

