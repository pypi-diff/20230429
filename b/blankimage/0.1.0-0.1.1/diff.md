# Comparing `tmp/blankimage-0.1.0.tar.gz` & `tmp/blankimage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, was "blankimage-0.1.1.tar", max compression
```

## Comparing `blankimage-0.1.0.tar` & `blankimage-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,7 @@
--rw-r--r--   0        0        0      370 1970-01-01 00:00:00.000000 blankimage-0.1.0/Cargo.toml
--rw-rw-rw-   0     1000        0    35149 2023-04-08 12:12:16.000000 blankimage-0.1.0/LICENSE
--rw-rw-rw-   0     1000        0       39 2023-04-08 12:12:16.000000 blankimage-0.1.0/README.md
--rw-rw-rw-   0     1000     1000      115 2023-04-08 14:22:54.000000 blankimage-0.1.0/blankimage/__init__.py
--rw-rw-rw-   0     1000     1000      109 2023-04-08 14:19:30.000000 blankimage-0.1.0/blankimage/generate_image.py
--rw-rw-rw-   0     1000     1000      372 2023-04-08 13:07:41.000000 blankimage-0.1.0/pyproject.toml
--rw-rw-rw-   0     1000     1000     1169 2023-04-08 13:22:58.000000 blankimage-0.1.0/src/lib.rs
--rw-rw-rw-   0     1000     1000    16463 2023-04-08 13:15:26.000000 blankimage-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 blankimage-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2023-04-29 07:54:05.374779 blankimage-0.1.1/README.md
+-rw-r--r--   0        0        0       26 2023-04-29 07:54:10.458848 blankimage-0.1.1/blankimage/__init__.py
+-rw-r--r--   0        0        0     2615 2023-04-29 07:39:10.626691 blankimage-0.1.1/blankimage/format_options.py
+-rw-r--r--   0        0        0     1514 2023-04-29 07:09:53.422626 blankimage-0.1.1/blankimage/parse_cli_options.py
+-rw-r--r--   0        0        0     1255 2023-04-29 07:20:23.947407 blankimage-0.1.1/blankimage/process_task.py
+-rw-r--r--   0        0        0     1042 2023-04-29 07:53:50.282594 blankimage-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 blankimage-0.1.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

