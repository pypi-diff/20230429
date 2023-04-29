# Comparing `tmp/Bigsansar-1.0.5.tar.gz` & `tmp/Bigsansar-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bigsansar-1.0.5.tar", last modified: Sat Apr 29 05:26:50 2023, max compression
+gzip compressed data, was "Bigsansar-1.0.6.tar", last modified: Sat Apr 29 07:14:59 2023, max compression
```

## Comparing `Bigsansar-1.0.5.tar` & `Bigsansar-1.0.6.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:50.064394 Bigsansar-1.0.5/
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.672122 Bigsansar-1.0.5/Bigsansar.egg-info/
--rw-rw-rw-   0        0        0     2930 2023-04-29 05:26:49.000000 Bigsansar-1.0.5/Bigsansar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2254 2023-04-29 05:26:49.000000 Bigsansar-1.0.5/Bigsansar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 05:26:49.000000 Bigsansar-1.0.5/Bigsansar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-29 05:26:49.000000 Bigsansar-1.0.5/Bigsansar.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       82 2023-04-29 05:26:49.000000 Bigsansar-1.0.5/Bigsansar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 05:26:49.000000 Bigsansar-1.0.5/Bigsansar.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     2930 2023-04-29 05:26:50.064394 Bigsansar-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2239 2023-04-29 05:26:16.000000 Bigsansar-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.734632 Bigsansar-1.0.5/bigsansar/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/__init__.py
--rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/admin.py
--rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.734632 Bigsansar-1.0.5/bigsansar/contrib/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.781926 Bigsansar-1.0.5/bigsansar/contrib/account/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/__init__.py
--rw-rw-rw-   0        0        0      510 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/admin.py
--rw-rw-rw-   0        0        0      284 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/apps.py
--rw-rw-rw-   0        0        0     1176 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.813175 Bigsansar-1.0.5/bigsansar/contrib/account/migrations/
--rw-rw-rw-   0        0        0      999 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      417 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/migrations/__init__.py
--rw-rw-rw-   0        0        0      556 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/models.py
--rw-rw-rw-   0        0        0      351 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/signals.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.813175 Bigsansar-1.0.5/bigsansar/contrib/account/templates/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/templates/__init__.py
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/tests.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/urls.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/account/views.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.860454 Bigsansar-1.0.5/bigsansar/contrib/blogs/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/__init__.py
--rw-rw-rw-   0        0        0      541 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/admin.py
--rw-rw-rw-   0        0        0      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.860454 Bigsansar-1.0.5/bigsansar/contrib/blogs/migrations/
--rw-rw-rw-   0        0        0     2272 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/migrations/__init__.py
--rw-rw-rw-   0        0        0     1572 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/models.py
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/tests.py
--rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/blogs/views.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.922966 Bigsansar-1.0.5/bigsansar/contrib/sites/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/__init__.py
--rw-rw-rw-   0        0        0     1734 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/admin.py
--rw-rw-rw-   0        0        0      203 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/apps.py
--rw-rw-rw-   0        0        0     3018 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/forms.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.938592 Bigsansar-1.0.5/bigsansar/contrib/sites/migrations/
--rw-rw-rw-   0        0        0     1816 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/migrations/__init__.py
--rw-rw-rw-   0        0        0     1826 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/models.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.938592 Bigsansar-1.0.5/bigsansar/contrib/sites/templatetags/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/templatetags/__init__.py
--rw-rw-rw-   0        0        0      408 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/templatetags/pages.py
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/tests.py
--rw-rw-rw-   0        0        0       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/contrib/sites/views.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.970238 Bigsansar-1.0.5/bigsansar/core/
--rw-rw-rw-   0        0        0      524 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/core/__init__.py
--rw-rw-rw-   0        0        0      414 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/core/host.py
--rw-rw-rw-   0        0        0     7418 2023-04-28 15:57:57.000000 Bigsansar-1.0.5/bigsansar/core/init.py
--rw-rw-rw-   0        0        0       27 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/main.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.970238 Bigsansar-1.0.5/bigsansar/management/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.985877 Bigsansar-1.0.5/bigsansar/management/commands/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/management/commands/__init__.py
--rw-rw-rw-   0        0        0     1122 2023-04-27 12:44:33.000000 Bigsansar-1.0.5/bigsansar/management/commands/createuser.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:49.985877 Bigsansar-1.0.5/bigsansar/migrations/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/models.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:50.001513 Bigsansar-1.0.5/bigsansar/static/
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/static/__init__.py
--rw-rw-rw-   0        0        0     9230 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/static/logo.png
--rw-rw-rw-   0        0        0      525 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/static/style.css
-drwxrwxrwx   0        0        0        0 2023-04-29 05:26:50.064394 Bigsansar-1.0.5/bigsansar/templates/
--rw-rw-rw-   0        0        0      977 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/404.html
--rw-rw-rw-   0        0        0        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/__init__.py
--rw-rw-rw-   0        0        0      168 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/acc_active_email.html
--rw-rw-rw-   0        0        0     1134 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/base.html
--rw-rw-rw-   0        0        0     2252 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/default.html
--rw-rw-rw-   0        0        0     2250 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/defaultpage.html
--rw-rw-rw-   0        0        0     2171 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/nav.html
--rw-rw-rw-   0        0        0      758 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/templates/parking.html
--rw-rw-rw-   0        0        0       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/tests.py
--rw-rw-rw-   0        0        0      821 2023-04-27 12:27:15.000000 Bigsansar-1.0.5/bigsansar/urls.py
--rw-rw-rw-   0        0        0     1864 2023-04-28 15:30:13.000000 Bigsansar-1.0.5/bigsansar/views.py
--rw-rw-rw-   0        0        0       42 2023-04-29 05:26:50.064394 Bigsansar-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1294 2023-04-29 05:24:58.000000 Bigsansar-1.0.5/setup.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.484023 Bigsansar-1.0.6/
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.454023 Bigsansar-1.0.6/Bigsansar.egg-info/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2874 2023-04-29 07:14:59.000000 Bigsansar-1.0.6/Bigsansar.egg-info/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2254 2023-04-29 07:14:59.000000 Bigsansar-1.0.6/Bigsansar.egg-info/SOURCES.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        1 2023-04-29 07:14:59.000000 Bigsansar-1.0.6/Bigsansar.egg-info/dependency_links.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       51 2023-04-29 07:14:59.000000 Bigsansar-1.0.6/Bigsansar.egg-info/entry_points.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       82 2023-04-29 07:14:59.000000 Bigsansar-1.0.6/Bigsansar.egg-info/requires.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       10 2023-04-29 07:14:59.000000 Bigsansar-1.0.6/Bigsansar.egg-info/top_level.txt
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1091 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/LICENSE
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2874 2023-04-29 07:14:59.484023 Bigsansar-1.0.6/PKG-INFO
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2239 2023-04-29 05:26:16.000000 Bigsansar-1.0.6/README.md
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.464023 Bigsansar-1.0.6/bigsansar/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.464023 Bigsansar-1.0.6/bigsansar/contrib/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/account/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      510 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      284 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1176 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/account/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      999 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      417 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/migrations/0002_alter_userinfo_options.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      556 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      351 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/signals.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/account/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/account/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/blogs/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      541 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      195 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/apps.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/blogs/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2272 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1572 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/models.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/blogs/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/sites/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1734 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/admin.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      203 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/apps.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     3018 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/forms.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/sites/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1816 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/migrations/0001_initial.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1826 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/contrib/sites/templatetags/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/templatetags/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      408 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/templatetags/pages.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       66 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/contrib/sites/views.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/core/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      524 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/core/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      414 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/core/host.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     7418 2023-04-29 07:14:25.000000 Bigsansar-1.0.6/bigsansar/core/init.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       27 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/main.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/management/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/management/__init__.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/management/commands/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/management/commands/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1122 2023-04-27 12:44:33.000000 Bigsansar-1.0.6/bigsansar/management/commands/createuser.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/migrations/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/migrations/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       60 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/models.py
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.474023 Bigsansar-1.0.6/bigsansar/static/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/static/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     9230 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/static/logo.png
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      525 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/static/style.css
+drwxr-xr-x   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-29 07:14:59.484023 Bigsansar-1.0.6/bigsansar/templates/
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      977 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/404.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)        0 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/__init__.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      168 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/acc_active_email.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1134 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/base.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2252 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/default.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2250 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/defaultpage.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     2171 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/nav.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      758 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/templates/parking.html
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       63 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/tests.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)      821 2023-04-27 12:27:15.000000 Bigsansar-1.0.6/bigsansar/urls.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1864 2023-04-28 15:30:13.000000 Bigsansar-1.0.6/bigsansar/views.py
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)       38 2023-04-29 07:14:59.484023 Bigsansar-1.0.6/setup.cfg
+-rw-r--r--   0 bigsansar  (1000) bigsansar  (1000)     1294 2023-04-29 07:14:39.000000 Bigsansar-1.0.6/setup.py
```

### Comparing `Bigsansar-1.0.5/Bigsansar.egg-info/PKG-INFO` & `Bigsansar-1.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: Bigsansar
-Version: 1.0.5
-Summary: Build one in minutes with bigsansar - a visual site building tool!
-Home-page: https://bigsansar.com
-Author: Bikash Pokhrel
-Author-email: bigsansaroffice@gmail.com
-Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
-Project-URL: Documentations, https://docs.bigsansar.com/
-Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # How to get Bigsansar
 
 Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
 Bigsansar is Fully based on django.
 You can use
 [bigsansar](https://bigsansar.com)
@@ -85,8 +68,8 @@
 #### More variable for **page**
 * page.id
 * page.domain
 * page.title
 * page.slug
 * page.body
 * page.visitor
-* page.publish_date
+* page.publish_date
```

### Comparing `Bigsansar-1.0.5/Bigsansar.egg-info/SOURCES.txt` & `Bigsansar-1.0.6/Bigsansar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/LICENSE` & `Bigsansar-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/PKG-INFO` & `Bigsansar-1.0.6/Bigsansar.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,95 @@
-Metadata-Version: 2.1
-Name: Bigsansar
-Version: 1.0.5
-Summary: Build one in minutes with bigsansar - a visual site building tool!
-Home-page: https://bigsansar.com
-Author: Bikash Pokhrel
-Author-email: bigsansaroffice@gmail.com
-Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
-Project-URL: Documentations, https://docs.bigsansar.com/
-Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# How to get Bigsansar
-
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
-Bigsansar is Fully based on django.
-You can use
-[bigsansar](https://bigsansar.com)
-for install packaged.
-
-view our tutorials in 
-[youtube](https://youtube.com/bigsansar)
-
-for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
-
-# Get the latest development version
-The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
-Get it using this shell command, which requires [Git](https://git-scm.com/):
-
-`git clone https://github.com/pokhrelb9/bigsansar.git`
-
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
-This archive is updated every time we commit code.
-
-# After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
-
-# For manually setup
-
-### After you get it
-
-go to `www` path and open `settings.py` file then add 
-`'bigsansar.apps.BigsansarConfig'`
-`'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
-`INSTALLED_APPS = []` .
-
-### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
-`MIDDLEWARE = []` .
-
-## Some usefull commands:
-
-`python3 manage.py createuser` - get unlimited users.
-
-
-
-## New update 
-* added sercure proxy ssl header 
-* fixed domain index and pages views system
-* added virtual host in to admin pannel 
-* added pages system and working in this model 
-* making too easy to handel django with help of bigsansar in the future .
-
-
-## Load page in templates
-
-`{% load pages %}
-
-{% get_pages  as listpage %}
-{% for page in listpage %}
-<div>
-    < a href="{{ page.slug }}">{{ page.title }}</a>
-</div>
-{% endfor %}`
-
-#### More variable for **page**
-* page.id
-* page.domain
-* page.title
-* page.slug
-* page.body
-* page.visitor
-* page.publish_date
+Metadata-Version: 2.1
+Name: Bigsansar
+Version: 1.0.6
+Summary: Build one in minutes with bigsansar - a visual site building tool!
+Home-page: https://bigsansar.com
+Author: Bikash Pokhrel
+Author-email: bigsansaroffice@gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
+Project-URL: Documentations, https://docs.bigsansar.com/
+Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# How to get Bigsansar
+
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is Fully based on django.
+You can use
+[bigsansar](https://bigsansar.com)
+for install packaged.
+
+view our tutorials in 
+[youtube](https://youtube.com/bigsansar)
+
+for playlist:
+[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
+
+# Get the latest development version
+The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+Get it using this shell command, which requires [Git](https://git-scm.com/):
+
+`git clone https://github.com/pokhrelb9/bigsansar.git`
+
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+This archive is updated every time we commit code.
+
+# After you install bigsansar
+Type `bigsansar init` command for **automatically** setup server . 
+
+# For manually setup
+
+### After you get it
+
+go to `www` path and open `settings.py` file then add 
+`'bigsansar.apps.BigsansarConfig'`
+`'bigsansar.contrib.account.apps.AccountConfig'`
+in to 
+`INSTALLED_APPS = []` .
+
+### For Virtualhost middleware
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+`MIDDLEWARE = []` .
+
+## Some usefull commands:
+
+`python3 manage.py createuser` - get unlimited users.
+
+
+
+## New update 
+* added sercure proxy ssl header 
+* fixed domain index and pages views system
+* added virtual host in to admin pannel 
+* added pages system and working in this model 
+* making too easy to handel django with help of bigsansar in the future .
+
+
+## Load page in templates
+
+`{% load pages %}
+
+{% get_pages  as listpage %}
+{% for page in listpage %}
+<div>
+    < a href="{{ page.slug }}">{{ page.title }}</a>
+</div>
+{% endfor %}`
+
+#### More variable for **page**
+* page.id
+* page.domain
+* page.title
+* page.slug
+* page.body
+* page.visitor
+* page.publish_date
+
```

### Comparing `Bigsansar-1.0.5/README.md` & `Bigsansar-1.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,95 @@
-
-# How to get Bigsansar
-
-Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
-Bigsansar is Fully based on django.
-You can use
-[bigsansar](https://bigsansar.com)
-for install packaged.
-
-view our tutorials in 
-[youtube](https://youtube.com/bigsansar)
-
-for playlist:
-[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
-
-# Get the latest development version
-The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
-This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
-Get it using this shell command, which requires [Git](https://git-scm.com/):
-
-`git clone https://github.com/pokhrelb9/bigsansar.git`
-
-You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
-This archive is updated every time we commit code.
-
-# After you install bigsansar
-Type `bigsansar init` command for **automatically** setup server . 
-
-# For manually setup
-
-### After you get it
-
-go to `www` path and open `settings.py` file then add 
-`'bigsansar.apps.BigsansarConfig'`
-`'bigsansar.contrib.account.apps.AccountConfig'`
-in to 
-`INSTALLED_APPS = []` .
-
-### For Virtualhost middleware
-go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
-`MIDDLEWARE = []` .
-
-## Some usefull commands:
-
-`python3 manage.py createuser` - get unlimited users.
-
-
-
-## New update 
-* added sercure proxy ssl header 
-* fixed domain index and pages views system
-* added virtual host in to admin pannel 
-* added pages system and working in this model 
-* making too easy to handel django with help of bigsansar in the future .
-
-
-## Load page in templates
-
-`{% load pages %}
-
-{% get_pages  as listpage %}
-{% for page in listpage %}
-<div>
-    < a href="{{ page.slug }}">{{ page.title }}</a>
-</div>
-{% endfor %}`
-
-#### More variable for **page**
-* page.id
-* page.domain
-* page.title
-* page.slug
-* page.body
-* page.visitor
-* page.publish_date
+Metadata-Version: 2.1
+Name: Bigsansar
+Version: 1.0.6
+Summary: Build one in minutes with bigsansar - a visual site building tool!
+Home-page: https://bigsansar.com
+Author: Bikash Pokhrel
+Author-email: bigsansaroffice@gmail.com
+License: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/pokhrelb9/bigsansar/issues
+Project-URL: Documentations, https://docs.bigsansar.com/
+Keywords: python,django host,bigsansar,django,django sites framework,django flatpages
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# How to get Bigsansar
+
+Bigsansar is available open-source under the [MIT](https://en.wikipedia.org/wiki/MIT_License) license. We recommend using the latest version of Python 3. 
+Bigsansar is Fully based on django.
+You can use
+[bigsansar](https://bigsansar.com)
+for install packaged.
+
+view our tutorials in 
+[youtube](https://youtube.com/bigsansar)
+
+for playlist:
+[bigsansar for django](https://www.youtube.com/playlist?list=PLqdXqRSrD-LC6i7YQAaqB57FaCfWEZkth)
+
+# Get the latest development version
+The latest and greatest Bigsasnar version is the one that’s in our Git repository (our revision-control system).
+This is only for experienced users who want to try incoming changes and help identify bugs before an official release. 
+Get it using this shell command, which requires [Git](https://git-scm.com/):
+
+`git clone https://github.com/pokhrelb9/bigsansar.git`
+
+You can also download a [gzipped tarball](https://pypi.org/project/Bigsansar/#files) of the development version. 
+This archive is updated every time we commit code.
+
+# After you install bigsansar
+Type `bigsansar init` command for **automatically** setup server . 
+
+# For manually setup
+
+### After you get it
+
+go to `www` path and open `settings.py` file then add 
+`'bigsansar.apps.BigsansarConfig'`
+`'bigsansar.contrib.account.apps.AccountConfig'`
+in to 
+`INSTALLED_APPS = []` .
+
+### For Virtualhost middleware
+go to `www` path and open `settings.py` file then add `bigsansar.core.host.VirtualHostMiddleware`  in to top of 
+`MIDDLEWARE = []` .
+
+## Some usefull commands:
+
+`python3 manage.py createuser` - get unlimited users.
+
+
+
+## New update 
+* added sercure proxy ssl header 
+* fixed domain index and pages views system
+* added virtual host in to admin pannel 
+* added pages system and working in this model 
+* making too easy to handel django with help of bigsansar in the future .
+
+
+## Load page in templates
+
+`{% load pages %}
+
+{% get_pages  as listpage %}
+{% for page in listpage %}
+<div>
+    < a href="{{ page.slug }}">{{ page.title }}</a>
+</div>
+{% endfor %}`
+
+#### More variable for **page**
+* page.id
+* page.domain
+* page.title
+* page.slug
+* page.body
+* page.visitor
+* page.publish_date
+
```

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/account/forms.py` & `Bigsansar-1.0.6/bigsansar/contrib/account/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/account/migrations/0001_initial.py` & `Bigsansar-1.0.6/bigsansar/contrib/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/account/models.py` & `Bigsansar-1.0.6/bigsansar/contrib/account/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/blogs/admin.py` & `Bigsansar-1.0.6/bigsansar/contrib/blogs/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/blogs/migrations/0001_initial.py` & `Bigsansar-1.0.6/bigsansar/contrib/blogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/blogs/models.py` & `Bigsansar-1.0.6/bigsansar/contrib/blogs/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/sites/admin.py` & `Bigsansar-1.0.6/bigsansar/contrib/sites/admin.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/sites/forms.py` & `Bigsansar-1.0.6/bigsansar/contrib/sites/forms.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/sites/migrations/0001_initial.py` & `Bigsansar-1.0.6/bigsansar/contrib/sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/contrib/sites/models.py` & `Bigsansar-1.0.6/bigsansar/contrib/sites/models.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/core/__init__.py` & `Bigsansar-1.0.6/bigsansar/core/__init__.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/core/init.py` & `Bigsansar-1.0.6/bigsansar/core/init.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/management/commands/createuser.py` & `Bigsansar-1.0.6/bigsansar/management/commands/createuser.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/static/logo.png` & `Bigsansar-1.0.6/bigsansar/static/logo.png`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/static/style.css` & `Bigsansar-1.0.6/bigsansar/static/style.css`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/templates/404.html` & `Bigsansar-1.0.6/bigsansar/templates/404.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/templates/base.html` & `Bigsansar-1.0.6/bigsansar/templates/base.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/templates/default.html` & `Bigsansar-1.0.6/bigsansar/templates/default.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/templates/defaultpage.html` & `Bigsansar-1.0.6/bigsansar/templates/defaultpage.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/templates/nav.html` & `Bigsansar-1.0.6/bigsansar/templates/nav.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/templates/parking.html` & `Bigsansar-1.0.6/bigsansar/templates/parking.html`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/urls.py` & `Bigsansar-1.0.6/bigsansar/urls.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/bigsansar/views.py` & `Bigsansar-1.0.6/bigsansar/views.py`

 * *Files identical despite different names*

### Comparing `Bigsansar-1.0.5/setup.py` & `Bigsansar-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Bigsansar",
-    version="1.0.5",
+    version="1.0.6",
     author="Bikash Pokhrel",
     author_email="bigsansaroffice@gmail.com",
     description="Build one in minutes with bigsansar - a visual site building tool!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bigsansar.com",
     project_urls={
```

