# Comparing `tmp/chef_helper-1.tar.gz` & `tmp/chef_helper-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chef_helper-1.tar", last modified: Sat Apr 29 13:50:35 2023, max compression
+gzip compressed data, was "chef_helper-2.tar", last modified: Sat Apr 29 13:58:27 2023, max compression
```

## Comparing `chef_helper-1.tar` & `chef_helper-2.tar`

### file list

```diff
@@ -1,13 +1,27 @@
-drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 13:50:35.424156 chef_helper-1/
--rw-r--r--   0 andriiosypenko   (501) staff       (20)     1065 2023-04-23 13:09:21.000000 chef_helper-1/LICENSE
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 13:50:35.423323 chef_helper-1/PKG-INFO
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      442 2023-04-29 11:54:03.000000 chef_helper-1/README.md
-drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 13:50:35.419633 chef_helper-1/chef_helper.egg-info/
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 13:50:35.000000 chef_helper-1/chef_helper.egg-info/PKG-INFO
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      238 2023-04-29 13:50:35.000000 chef_helper-1/chef_helper.egg-info/SOURCES.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)        1 2023-04-29 13:50:35.000000 chef_helper-1/chef_helper.egg-info/dependency_links.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       62 2023-04-29 13:50:35.000000 chef_helper-1/chef_helper.egg-info/entry_points.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       17 2023-04-29 13:50:35.000000 chef_helper-1/chef_helper.egg-info/requires.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       15 2023-04-29 13:50:35.000000 chef_helper-1/chef_helper.egg-info/top_level.txt
--rw-r--r--   0 andriiosypenko   (501) staff       (20)       38 2023-04-29 13:50:35.424481 chef_helper-1/setup.cfg
--rw-r--r--   0 andriiosypenko   (501) staff       (20)      468 2023-04-29 13:49:06.000000 chef_helper-1/setup.py
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 13:58:27.268777 chef_helper-2/
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)     1065 2023-04-23 13:09:21.000000 chef_helper-2/LICENSE
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 13:58:27.266993 chef_helper-2/PKG-INFO
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      442 2023-04-29 11:54:03.000000 chef_helper-2/README.md
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 13:58:27.184383 chef_helper-2/chef_helper.egg-info/
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      242 2023-04-29 13:58:27.000000 chef_helper-2/chef_helper.egg-info/PKG-INFO
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      507 2023-04-29 13:58:27.000000 chef_helper-2/chef_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)        1 2023-04-29 13:58:27.000000 chef_helper-2/chef_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       50 2023-04-29 13:58:27.000000 chef_helper-2/chef_helper.egg-info/entry_points.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       17 2023-04-29 13:58:27.000000 chef_helper-2/chef_helper.egg-info/requires.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       10 2023-04-29 13:58:27.000000 chef_helper-2/chef_helper.egg-info/top_level.txt
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)       38 2023-04-29 13:58:27.269023 chef_helper-2/setup.cfg
+-rw-r--r--   0 andriiosypenko   (501) staff       (20)      456 2023-04-29 13:58:07.000000 chef_helper-2/setup.py
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 13:58:27.160581 chef_helper-2/venv/
+drwxr-xr-x   0 andriiosypenko   (501) staff       (20)        0 2023-04-29 13:58:27.261222 chef_helper-2/venv/bin/
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      643 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2html.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      765 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)     1110 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      842 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      665 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2man.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      831 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)     1769 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      650 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      686 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      922 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      651 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 andriiosypenko   (501) staff       (20)      719 2023-04-29 13:52:05.000000 chef_helper-2/venv/bin/rstpep2html.py
```

### Comparing `chef_helper-1/LICENSE` & `chef_helper-2/LICENSE`

 * *Files identical despite different names*

