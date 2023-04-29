# Comparing `tmp/keepercommander-4.88.tar.gz` & `tmp/keepercommander-4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepercommander-4.88.tar", last modified: Fri Aug  6 23:25:30 2021, max compression
+gzip compressed data, was "dist/keepercommander-4.9.tar", last modified: Sat Jul 27 14:24:25 2019, max compression
```

## Comparing `keepercommander-4.88.tar` & `keepercommander-4.9.tar`

### file list

```diff
@@ -1,121 +1,93 @@
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.293290 keepercommander-4.88/
--rw-r--r--   0 mustinov   (502) staff       (20)     1065 2020-11-17 22:13:09.000000 keepercommander-4.88/LICENSE
--rw-r--r--   0 mustinov   (502) staff       (20)       54 2020-11-17 22:13:09.000000 keepercommander-4.88/MANIFEST.in
--rw-r--r--   0 mustinov   (502) staff       (20)     1598 2021-08-06 23:25:30.291388 keepercommander-4.88/PKG-INFO
--rw-r--r--   0 mustinov   (502) staff       (20)     1018 2021-07-22 19:09:51.000000 keepercommander-4.88/README.md
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.166328 keepercommander-4.88/keepercommander/
--rw-r--r--   0 mustinov   (502) staff       (20)   271764 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/APIRequest_pb2.py
--rw-r--r--   0 mustinov   (502) staff       (20)    86488 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/AccountSummary_pb2.py
--rw-r--r--   0 mustinov   (502) staff       (20)      262 2021-08-06 23:23:38.000000 keepercommander-4.88/keepercommander/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     8784 2021-05-10 19:55:37.000000 keepercommander-4.88/keepercommander/__main__.py
--rw-r--r--   0 mustinov   (502) staff       (20)    75279 2021-08-06 23:21:35.000000 keepercommander-4.88/keepercommander/api.py
--rw-r--r--   0 mustinov   (502) staff       (20)    11438 2021-05-07 15:15:12.000000 keepercommander-4.88/keepercommander/autocomplete.py
--rw-r--r--   0 mustinov   (502) staff       (20)    20533 2021-05-10 19:55:38.000000 keepercommander-4.88/keepercommander/cli.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.177979 keepercommander-4.88/keepercommander/commands/
--rw-r--r--   0 mustinov   (502) staff       (20)      511 2021-05-06 23:03:38.000000 keepercommander-4.88/keepercommander/commands/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     7095 2021-07-26 22:54:31.000000 keepercommander-4.88/keepercommander/commands/base.py
--rw-r--r--   0 mustinov   (502) staff       (20)   203261 2021-08-06 23:21:35.000000 keepercommander-4.88/keepercommander/commands/enterprise.py
--rw-r--r--   0 mustinov   (502) staff       (20)   272689 2021-07-26 22:54:31.000000 keepercommander-4.88/keepercommander/commands/enterprise_pb2.py
--rw-r--r--   0 mustinov   (502) staff       (20)    27728 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/commands/folder.py
--rw-r--r--   0 mustinov   (502) staff       (20)    14620 2021-05-11 15:55:34.000000 keepercommander-4.88/keepercommander/commands/msp.py
--rw-r--r--   0 mustinov   (502) staff       (20)    69515 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/commands/record.py
--rw-r--r--   0 mustinov   (502) staff       (20)    83457 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/commands/register.py
--rw-r--r--   0 mustinov   (502) staff       (20)    49878 2021-06-29 17:27:15.000000 keepercommander-4.88/keepercommander/commands/utils.py
--rw-r--r--   0 mustinov   (502) staff       (20)     7329 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/display.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1724 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/error.py
--rw-r--r--   0 mustinov   (502) staff       (20)    35004 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/folder_pb2.py
--rw-r--r--   0 mustinov   (502) staff       (20)     2413 2021-07-22 19:09:51.000000 keepercommander-4.88/keepercommander/generator.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.182294 keepercommander-4.88/keepercommander/importer/
--rw-r--r--   0 mustinov   (502) staff       (20)      337 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     8676 2021-04-23 21:47:13.000000 keepercommander-4.88/keepercommander/importer/commands.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.183663 keepercommander-4.88/keepercommander/importer/csv/
--rw-r--r--   0 mustinov   (502) staff       (20)      330 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/csv/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     3787 2021-04-26 21:29:36.000000 keepercommander-4.88/keepercommander/importer/csv/csv.py
--rw-r--r--   0 mustinov   (502) staff       (20)    41055 2021-04-23 21:47:13.000000 keepercommander-4.88/keepercommander/importer/imp_exp.py
--rw-r--r--   0 mustinov   (502) staff       (20)     6865 2021-04-23 21:47:13.000000 keepercommander-4.88/keepercommander/importer/importer.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.185626 keepercommander-4.88/keepercommander/importer/json/
--rw-r--r--   0 mustinov   (502) staff       (20)      333 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/json/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     5695 2021-04-26 21:29:36.000000 keepercommander-4.88/keepercommander/importer/json/json.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.189844 keepercommander-4.88/keepercommander/importer/keepass/
--rw-r--r--   0 mustinov   (502) staff       (20)      330 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/keepass/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)    23939 2021-04-23 21:47:13.000000 keepercommander-4.88/keepercommander/importer/keepass/keepass.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1470 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/keepass/template.kdbx
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.262254 keepercommander-4.88/keepercommander/importer/lastpass/
--rw-r--r--   0 mustinov   (502) staff       (20)      291 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)      306 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/account.py
--rw-r--r--   0 mustinov   (502) staff       (20)      458 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/blob.py
--rw-r--r--   0 mustinov   (502) staff       (20)      225 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/chunk.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1021 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/exceptions.py
--rw-r--r--   0 mustinov   (502) staff       (20)     4861 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/fetcher.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1616 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/lastpass.py
--rw-r--r--   0 mustinov   (502) staff       (20)     8529 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/parser.py
--rw-r--r--   0 mustinov   (502) staff       (20)      287 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/session.py
--rw-r--r--   0 mustinov   (502) staff       (20)     2389 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/importer/lastpass/vault.py
--rw-r--r--   0 mustinov   (502) staff       (20)    54755 2021-08-06 23:21:35.000000 keepercommander-4.88/keepercommander/loginv3.py
--rw-r--r--   0 mustinov   (502) staff       (20)     6014 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/params.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.265981 keepercommander-4.88/keepercommander/plugins/
--rw-r--r--   0 mustinov   (502) staff       (20)      337 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/__init__.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.267307 keepercommander-4.88/keepercommander/plugins/adpasswd/
--rw-r--r--   0 mustinov   (502) staff       (20)       45 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/adpasswd/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1703 2021-06-29 17:27:15.000000 keepercommander-4.88/keepercommander/plugins/adpasswd/adpasswd.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.268374 keepercommander-4.88/keepercommander/plugins/awskey/
--rw-r--r--   0 mustinov   (502) staff       (20)       50 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/awskey/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     2329 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/awskey/aws_accesskey.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.269559 keepercommander-4.88/keepercommander/plugins/awspswd/
--rw-r--r--   0 mustinov   (502) staff       (20)       47 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/awspswd/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1705 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/awspswd/aws_passwd.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.270855 keepercommander-4.88/keepercommander/plugins/azureadpwd/
--rw-r--r--   0 mustinov   (502) staff       (20)      288 2021-01-22 20:47:19.000000 keepercommander-4.88/keepercommander/plugins/azureadpwd/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     4410 2021-01-22 20:47:19.000000 keepercommander-4.88/keepercommander/plugins/azureadpwd/azureadpwd.py
--rw-r--r--   0 mustinov   (502) staff       (20)     9484 2021-08-06 23:21:35.000000 keepercommander-4.88/keepercommander/plugins/commands.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.272103 keepercommander-4.88/keepercommander/plugins/humps/
--rw-r--r--   0 mustinov   (502) staff       (20)      710 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/humps/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     4982 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/humps/humps.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.273383 keepercommander-4.88/keepercommander/plugins/mssql/
--rw-r--r--   0 mustinov   (502) staff       (20)       42 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/mssql/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1485 2020-12-28 22:29:30.000000 keepercommander-4.88/keepercommander/plugins/mssql/mssql.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.275068 keepercommander-4.88/keepercommander/plugins/mysql/
--rw-r--r--   0 mustinov   (502) staff       (20)       42 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/mysql/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1928 2020-12-28 22:29:30.000000 keepercommander-4.88/keepercommander/plugins/mysql/mysql.py
--rw-r--r--   0 mustinov   (502) staff       (20)      147 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/noop.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.276297 keepercommander-4.88/keepercommander/plugins/oracle/
--rw-r--r--   0 mustinov   (502) staff       (20)       43 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/oracle/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1599 2020-12-28 22:29:30.000000 keepercommander-4.88/keepercommander/plugins/oracle/oracle.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1042 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/plugin_manager.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.277395 keepercommander-4.88/keepercommander/plugins/postgresql/
--rw-r--r--   0 mustinov   (502) staff       (20)       47 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/postgresql/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1159 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/postgresql/postgresql.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.279070 keepercommander-4.88/keepercommander/plugins/pspasswd/
--rw-r--r--   0 mustinov   (502) staff       (20)       56 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/pspasswd/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)      887 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/pspasswd/pspasswd.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.280743 keepercommander-4.88/keepercommander/plugins/ssh/
--rw-r--r--   0 mustinov   (502) staff       (20)       40 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/ssh/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1788 2021-02-08 21:09:01.000000 keepercommander-4.88/keepercommander/plugins/ssh/ssh.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.282369 keepercommander-4.88/keepercommander/plugins/sshkey/
--rw-r--r--   0 mustinov   (502) staff       (20)       43 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/sshkey/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     4018 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/sshkey/sshkey.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.284507 keepercommander-4.88/keepercommander/plugins/unixpasswd/
--rw-r--r--   0 mustinov   (502) staff       (20)       47 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/unixpasswd/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1553 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/unixpasswd/unixpasswd.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.287278 keepercommander-4.88/keepercommander/plugins/windows/
--rw-r--r--   0 mustinov   (502) staff       (20)       54 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/windows/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)      787 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/plugins/windows/windows.py
--rw-r--r--   0 mustinov   (502) staff       (20)    13392 2021-07-08 16:15:08.000000 keepercommander-4.88/keepercommander/record.py
--rw-r--r--   0 mustinov   (502) staff       (20)    10794 2021-05-14 22:31:47.000000 keepercommander-4.88/keepercommander/rest_api.py
--rw-r--r--   0 mustinov   (502) staff       (20)     3618 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/shared_folder.py
--rw-r--r--   0 mustinov   (502) staff       (20)    71104 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/ssocloud_pb2.py
--rw-r--r--   0 mustinov   (502) staff       (20)     4086 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/subfolder.py
--rw-r--r--   0 mustinov   (502) staff       (20)     1523 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/team.py
--rw-r--r--   0 mustinov   (502) staff       (20)     3904 2021-06-29 17:27:15.000000 keepercommander-4.88/keepercommander/versioning.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.290217 keepercommander-4.88/keepercommander/yubikey/
--rw-r--r--   0 mustinov   (502) staff       (20)      286 2020-11-17 22:13:09.000000 keepercommander-4.88/keepercommander/yubikey/__init__.py
--rw-r--r--   0 mustinov   (502) staff       (20)     5376 2021-04-23 21:47:13.000000 keepercommander-4.88/keepercommander/yubikey/yubikey.py
-drwxr-xr-x   0 mustinov   (502) staff       (20)        0 2021-08-06 23:25:30.168721 keepercommander-4.88/keepercommander.egg-info/
--rw-r--r--   0 mustinov   (502) staff       (20)     1598 2021-08-06 23:25:29.000000 keepercommander-4.88/keepercommander.egg-info/PKG-INFO
--rw-r--r--   0 mustinov   (502) staff       (20)     3497 2021-08-06 23:25:29.000000 keepercommander-4.88/keepercommander.egg-info/SOURCES.txt
--rw-r--r--   0 mustinov   (502) staff       (20)        1 2021-08-06 23:25:29.000000 keepercommander-4.88/keepercommander.egg-info/dependency_links.txt
--rw-r--r--   0 mustinov   (502) staff       (20)       58 2021-08-06 23:25:29.000000 keepercommander-4.88/keepercommander.egg-info/entry_points.txt
--rw-r--r--   0 mustinov   (502) staff       (20)      140 2021-08-06 23:25:29.000000 keepercommander-4.88/keepercommander.egg-info/requires.txt
--rw-r--r--   0 mustinov   (502) staff       (20)       16 2021-08-06 23:25:29.000000 keepercommander-4.88/keepercommander.egg-info/top_level.txt
--rw-r--r--   0 mustinov   (502) staff       (20)       38 2021-08-06 23:25:30.293433 keepercommander-4.88/setup.cfg
--rw-r--r--   0 mustinov   (502) staff       (20)     1468 2020-11-17 22:13:09.000000 keepercommander-4.88/setup.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       54 2019-05-21 13:14:24.000000 keepercommander-4.9/MANIFEST.in
+-rw-r--r--   0 craiglurey   (501) staff       (20)    70107 2019-07-27 14:24:25.000000 keepercommander-4.9/PKG-INFO
+-rw-r--r--   0 craiglurey   (501) staff       (20)    58099 2019-07-27 02:49:18.000000 keepercommander-4.9/README.md
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/
+-rw-r--r--   0 craiglurey   (501) staff       (20)    66983 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/APIRequest_pb2.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)      261 2019-07-26 23:17:54.000000 keepercommander-4.9/keepercommander/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     5564 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/__main__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    62415 2019-06-18 04:21:04.000000 keepercommander-4.9/keepercommander/api.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     8934 2019-07-26 23:17:33.000000 keepercommander-4.9/keepercommander/autocomplete.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     9164 2019-07-27 02:49:39.000000 keepercommander-4.9/keepercommander/cli.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/commands/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      347 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/commands/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     3991 2019-06-18 04:21:04.000000 keepercommander-4.9/keepercommander/commands/base.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)   109324 2019-07-27 00:27:27.000000 keepercommander-4.9/keepercommander/commands/enterprise.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    27581 2019-06-18 04:21:04.000000 keepercommander-4.9/keepercommander/commands/folder.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    36812 2019-07-19 23:53:37.000000 keepercommander-4.9/keepercommander/commands/record.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    44515 2019-06-18 04:21:04.000000 keepercommander-4.9/keepercommander/commands/register.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    24741 2019-07-26 23:17:33.000000 keepercommander-4.9/keepercommander/commands/utils.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     5753 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/display.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1591 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/error.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1877 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/generator.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/importer/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      337 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     6619 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/commands.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/importer/csv/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      330 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/csv/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     3741 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/csv/csv.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    35572 2019-07-26 23:17:33.000000 keepercommander-4.9/keepercommander/importer/imp_exp.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     4739 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/importer.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/importer/json/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      333 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/json/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     5571 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/json/json.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/importer/keepass/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      330 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/keepass/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)    19236 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/keepass/keepass.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1470 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/importer/keepass/template.kdbx
+-rw-r--r--   0 craiglurey   (501) staff       (20)     4568 2019-06-18 04:21:04.000000 keepercommander-4.9/keepercommander/params.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      337 2019-05-21 13:14:24.000000 keepercommander-4.9/keepercommander/plugins/__init__.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/adpasswd/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       45 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/adpasswd/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1598 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/adpasswd/adpasswd.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/awskey/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       50 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/awskey/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     2329 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/awskey/aws_accesskey.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     3539 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/commands.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/mssql/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       42 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/mssql/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1448 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/mssql/mssql.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/mysql/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       42 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/mysql/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1865 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/mysql/mysql.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)      147 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/noop.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/oracle/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       43 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/oracle/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1297 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/oracle/oracle.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1042 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/plugin_manager.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/postgresql/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       47 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/postgresql/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1459 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/postgresql/postgresql.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/pspasswd/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       56 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/pspasswd/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)      887 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/pspasswd/pspasswd.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/ssh/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       40 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/ssh/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1535 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/ssh/ssh.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/sshkey/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       43 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/sshkey/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     3995 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/sshkey/sshkey.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/unixpasswd/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       47 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/unixpasswd/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1553 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/unixpasswd/unixpasswd.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/plugins/windows/
+-rw-r--r--   0 craiglurey   (501) staff       (20)       54 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/windows/__init__.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)      787 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/plugins/windows/windows.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     8459 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/record.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     9774 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/rest_api.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     3618 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/shared_folder.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     4034 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/subfolder.py
+-rw-r--r--   0 craiglurey   (501) staff       (20)     1523 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/team.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander/yubikey/
+-rw-r--r--   0 craiglurey   (501) staff       (20)      286 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/yubikey/__init__.py
+-rwxr-xr-x   0 craiglurey   (501) staff       (20)     5125 2019-05-21 13:14:25.000000 keepercommander-4.9/keepercommander/yubikey/yubikey.py
+drwxr-xr-x   0 craiglurey   (501) staff       (20)        0 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/
+-rw-r--r--   0 craiglurey   (501) staff       (20)    70107 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/PKG-INFO
+-rw-r--r--   0 craiglurey   (501) staff       (20)     2543 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/SOURCES.txt
+-rw-r--r--   0 craiglurey   (501) staff       (20)        1 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/dependency_links.txt
+-rw-r--r--   0 craiglurey   (501) staff       (20)       58 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/entry_points.txt
+-rw-r--r--   0 craiglurey   (501) staff       (20)      117 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/requires.txt
+-rw-r--r--   0 craiglurey   (501) staff       (20)       16 2019-07-27 14:24:25.000000 keepercommander-4.9/keepercommander.egg-info/top_level.txt
+-rw-r--r--   0 craiglurey   (501) staff       (20)       38 2019-07-27 14:24:25.000000 keepercommander-4.9/setup.cfg
+-rw-r--r--   0 craiglurey   (501) staff       (20)     2326 2019-07-27 00:27:27.000000 keepercommander-4.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `keepercommander-4.88/keepercommander/__main__.py` & `keepercommander-4.9/keepercommander/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,176 +15,123 @@
 import sys
 import os
 import argparse
 import shlex
 import json
 import logging
 import base64
-from pathlib import Path
 
 from . import __version__
 from .params import KeeperParams
 
 from . import cli
 
 
 def get_params_from_config(config_filename):
     params = KeeperParams()
+    params.config_filename = config_filename or 'config.json'
 
-    if os.getenv("KEEPER_COMMANDER_DEBUG"):
-        logging.getLogger().setLevel(logging.DEBUG)
-        logging.info('Debug ON')
+    try:
+        with open(params.config_filename) as config_file:
 
-    opts, flags = parser.parse_known_args(sys.argv[1:])
-
-    if os.getenv('KEEPER_CONFIG_FILE'):
-        logging.debug("Setting config file from KEEPER_CONFIG_FILE env variable %s" % os.getenv('KEEPER_CONFIG_FILE'))
-        params.config_filename = os.getenv('KEEPER_CONFIG_FILE')
-    elif opts.launched_with_shortcut:
-        current_user_home_path = str(Path.home())
-        path_sep = os.path.sep
-
-        # unix: /Users/username/.keeper/
-        # win: C:\\Users\\username\\.keeper\\
-
-        laucher_keeper_folder_path = current_user_home_path + path_sep + '.keeper'
-        logging.debug("Launcher keeper folder: %s" % laucher_keeper_folder_path)
-
-        Path(laucher_keeper_folder_path).mkdir(parents=True, exist_ok=True)
-
-        params.config_filename = laucher_keeper_folder_path + path_sep + 'config.json'
-    else:
-        params.config_filename = config_filename or 'config.json'
-
-    if os.path.exists(params.config_filename):
-        try:
             try:
-                with open(params.config_filename) as config_file:
-                    params.config = json.load(config_file)
+                params.config = json.load(config_file)
 
-                    if 'user' in params.config:
-                        params.user = params.config['user'].lower()
+                if 'user' in params.config:
+                    params.user = params.config['user']
 
-                    if 'server' in params.config:
-                        params.server = params.config['server']
+                if 'server' in params.config:
+                    params.server = params.config['server']
 
-                    if 'password' in params.config:
-                        params.password = params.config['password']
+                if 'password' in params.config:
+                    params.password = params.config['password']
 
-                    if 'timedelay' in params.config:
-                        params.timedelay = params.config['timedelay']
+                if 'challenge' in params.config:
+                    try:
+                        import keepercommander.yubikey.yubikey
+                        challenge = params.config['challenge']
+                        params.password = keepercommander.yubikey.yubikey.get_response(challenge)
+                    except Exception as e:
+                        print(e)
+                        sys.exit(1)
 
-                    if 'mfa_token' in params.config:
-                        params.mfa_token = params.config['mfa_token']
+                if 'timedelay' in params.config:
+                    params.timedelay = params.config['timedelay']
 
-                    if 'mfa_type' in params.config:
-                        params.mfa_type = params.config['mfa_type']
+                if 'mfa_token' in params.config:
+                    params.mfa_token = params.config['mfa_token']
 
-                    if 'commands' in params.config:
-                        if params.config['commands']:
-                            params.commands.extend(params.config['commands'])
+                if 'mfa_type' in params.config:
+                    params.mfa_type = params.config['mfa_type']
 
-                    if 'plugins' in params.config:
-                        params.plugins = params.config['plugins']
+                if 'commands' in params.config:
+                    if params.config['commands']:
+                        params.commands.extend(params.config['commands'])
 
-                    if 'debug' in params.config:
-                        if params.config['debug']:
-                            logging.getLogger().setLevel(logging.DEBUG)
-                            logging.info('Debug ON')
+                if 'plugins' in params.config:
+                    params.plugins = params.config['plugins']
 
-                    if 'batch_mode' in params.config:
-                        params.batch_mode = params.config['batch_mode'] == True
+                if 'debug' in params.config:
+                    params.debug = params.config['debug']
 
-                    if 'device_id' in params.config:
-                        device_id = base64.urlsafe_b64decode(params.config['device_id'] + '==')
-                        params.rest_context.device_id = device_id
+                if 'batch_mode' in params.config:
+                    params.batch_mode = params.config['batch_mode'] == True
 
-                    if 'logout_timer' in params.config:
-                        params.logout_timer = params.config['logout_timer']
+                if 'device_id' in params.config:
+                    device_id = base64.urlsafe_b64decode(params.config['device_id'] + '==')
+                    params.rest_context.device_id = device_id
 
-                    if 'login_v3' in params.config:
-                        params.login_v3 = params.config['login_v3']
+            except:
+                print('Error: Unable to parse JSON file ' + params.config_filename)
+                raise
 
-                    if 'private_key' in params.config:
-                        params.device_private_key = params.config['private_key']
-
-            except Exception as e:
-                logging.error('Unable to parse JSON configuration file "%s"', params.config_filename)
-                answer = input('Do you want to delete it (y/N): ')
-                if answer in ['y', 'Y']:
-                    os.remove(params.config_filename)
-                else:
-                    raise e
-        except IOError as ioe:
-            logging.warning('Error: Unable to open config file %s: %s', params.config_filename, ioe)
+    except IOError:
+        if config_filename:
+            print('Error: Unable to open config file ' + config_filename)
+        pass
 
     if not params.server:
         params.server = 'https://keepersecurity.com/api/v2/'
 
     return params
 
 
 def usage(m):
     print(m)
     parser.print_help()
     cli.display_command_help(show_enterprise=True, show_shell=True)
-    sys.exit(1)
-
+    exit(1)
 
-parser = argparse.ArgumentParser(prog='keeper', add_help=False, allow_abbrev=False)
+parser = argparse.ArgumentParser(prog='keeper', add_help=False)
 parser.add_argument('--server', '-ks', dest='server', action='store', help='Keeper Host address.')
 parser.add_argument('--user', '-ku', dest='user', action='store', help='Email address for the account.')
 parser.add_argument('--password', '-kp', dest='password', action='store', help='Master password for the account.')
 parser.add_argument('--version', dest='version', action='store_true', help='Display version')
 parser.add_argument('--config', dest='config', action='store', help='Config file to use')
 parser.add_argument('--debug', dest='debug', action='store_true', help='Turn on debug mode')
 parser.add_argument('--batch-mode', dest='batch_mode', action='store_true', help='Run commander in batch or basic UI mode.')
-parser.add_argument('--login-v3', '-lv3', dest='login_v3', action='store', help='Use Login v3 to login to Keeper.')
-parser.add_argument('--launched-with-shortcut', '-lwsc', dest='launched_with_shortcut', action='store',
-                    help='Indicates that the app was launched using a shortcut, for example using Mac App or from '
-                         'Windows Start Menu.')
 parser.add_argument('command', nargs='?', type=str, action='store', help='Command')
 parser.add_argument('options', nargs='*', action='store', help='Options')
 parser.error = usage
 
 
-def handle_exceptions(exc_type, exc_value, exc_traceback):
-    import traceback
-    traceback.print_exception(exc_type, exc_value, exc_traceback)
-    input('Press Enter to exit')
-    sys.exit(-1)
-
-
-def main(from_package=False):
-
-    set_working_dir()
-
-    errno = 0
-
-    if from_package:
-        sys.excepthook = handle_exceptions
+def main():
+    logging.basicConfig(level=logging.INFO, format='%(message)s')
 
     sys.argv[0] = re.sub(r'(-script\.pyw?|\.exe)?$', '', sys.argv[0])
 
     opts, flags = parser.parse_known_args(sys.argv[1:])
     params = get_params_from_config(opts.config)
 
     if opts.debug:
         params.debug = opts.debug
-        is_debug = logging.getLogger().level <= logging.DEBUG
-        logging.getLogger().setLevel((logging.WARNING if params.batch_mode else logging.INFO) if is_debug else logging.DEBUG)
-        logging.info('Debug %s', 'OFF' if is_debug else 'ON')
-
 
     if opts.batch_mode:
         params.batch_mode = True
 
-    if opts.login_v3:
-        params.login_v3 = 'TRUE'.startswith(str(opts.login_v3).upper())
-
     if opts.server:
         params.server = 'https://{0}/api/v2/'.format(opts.server)
 
     if opts.user:
         params.user = opts.user
 
     if opts.password:
@@ -199,53 +146,26 @@
         return
 
     if flags and len(flags) > 0:
         if flags[0] == '-h':
             flags.clear()
             opts.command = '?'
 
-    if not opts.command and from_package:
-        opts.command = 'shell'
-
     if (opts.command or '') in {'?', ''}:
         if opts.command == '?' or not params.commands:
             usage('')
 
-    logging.basicConfig(level=logging.WARNING if params.batch_mode else logging.INFO, format='%(message)s')
-
     if params.timedelay >= 1 and params.commands:
         cli.runcommands(params)
     else:
-        if opts.command not in {'shell', '-'}:
+        if opts.command != 'shell':
             if opts.command:
                 flags = ' '.join([shlex.quote(x) for x in flags]) if flags is not None else ''
                 options = ' '.join([shlex.quote(x) for x in opts.options]) if opts.options is not None else ''
-                command = ' '.join([opts.command, flags])
-                if options:
-                    command += ' -- ' + options
+                command = ' '.join([opts.command, flags, options])
                 params.commands.append(command)
             params.commands.append('q')
-            params.batch_mode = True
-        else:
-            if opts.command == '-':
-                params.batch_mode = True
-
-        errno = cli.loop(params)
-
-    sys.exit(errno)
-
-
-def set_working_dir():
-
-    opts, flags = parser.parse_known_args(sys.argv[1:])
-
-    if opts.launched_with_shortcut:
-        current_user_home_path = str(Path.home())
-
-        logging.debug("User home: %s" % current_user_home_path)
-
-        current_user_home_path = str(Path.home())
-        os.chdir(current_user_home_path)
+        cli.loop(params)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `keepercommander-4.88/keepercommander/api.py` & `keepercommander-4.9/keepercommander/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 # Keeper Commander 
 # Copyright 2017 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import json
 import base64
-import collections
 import re
 import getpass
 import time
 import os
 import hashlib
 import logging
 import urllib.parse
 
-from . import rest_api, APIRequest_pb2 as proto, loginv3
+from . import rest_api
 from .subfolder import UserFolderNode, SharedFolderNode, SharedFolderFolderNode, RootFolderNode
 from .record import Record
 from .shared_folder import SharedFolder
 from .team import Team
 from .error import AuthenticationError, CommunicationError, CryptoError, KeeperApiError
 from .params import KeeperParams, LAST_RECORD_UID
 from .display import bcolors
@@ -41,21 +40,18 @@
 
 # PKCS7 padding helpers
 BS = 16
 pad_binary = lambda s: s + ((BS - len(s) % BS) * chr(BS - len(s) % BS)).encode()
 unpad_binary = lambda s: s[0:-s[-1]]
 unpad_char = lambda s: s[0:-ord(s[-1])]
 
-decode_uid_to_str = lambda uid: base64.urlsafe_b64encode(uid).decode().rstrip('=')
 
 def run_command(params, request):
     # type: (KeeperParams, dict) -> dict
-    if 'client_version' not in request:
-        request['client_version'] = rest_api.CLIENT_VERSION
-
+    request['client_version'] = rest_api.CLIENT_VERSION
     return rest_api.v2_execute(params.rest_context, request)
 
 
 def derive_key(password, salt, iterations):
     # type: (str, bytes, int) -> bytes
     return hashlib.pbkdf2_hmac('sha256', password.encode('utf-8'), salt, iterations, 32)
 
@@ -68,25 +64,16 @@
 
 
 warned_on_fido_package = False
 install_fido_package_warning = 'You can use Security Key with Commander:\n' +\
                                'Install fido2 package ' + bcolors.OKGREEN +\
                                '\'pip install fido2\'' + bcolors.ENDC
 
-
 def login(params):
     # type: (KeeperParams) -> None
-
-    if params.login_v3:
-        logging.info('Logging in to Keeper Commander')
-        loginv3.LoginV3Flow.login(params)
-        return
-
-    logging.info("Logging in...")
-
     global should_cancel_u2f
     global u2f_response
     global warned_on_fido_package
 
     success = False
     store_config = False
 
@@ -94,55 +81,49 @@
         if not params.auth_verifier:
             if not params.user or not params.password:
                 return
 
             logging.debug('No auth verifier, sending pre-auth request')
             try:
                 pre_login_rs = rest_api.pre_login(params.rest_context, params.user)
-                auth_params = get_correct_salt(pre_login_rs.salt)
+                auth_params = pre_login_rs.salt[0]
                 params.iterations = auth_params.iterations
                 params.salt = auth_params.salt
                 params.auth_verifier = auth_verifier(params.password, params.salt, params.iterations)
+                logging.debug('<<< Auth Verifier:[%s]', params.auth_verifier)
             except KeeperApiError as e:
                 params.auth_verifier = None
                 if e.result_code == 'user_does_not_exist':
                     email = params.user
                     params.user = ''
                     params.password = ''
                     raise AuthenticationError('User account [{0}] not found.'.format(email))
                 raise
 
         rq = {
             'command': 'login',
             'include': ['keys', 'license', 'settings', 'enforcements', 'is_enterprise_admin'],
             'version': 2,
             'auth_response': params.auth_verifier,
-            'username': params.user.lower(),
-            'platform_device_token': base64.urlsafe_b64encode(params.rest_context.device_id).decode('utf-8').rstrip('=')
+            'username': params.user
         }
 
-        if params.enterprise_id > 0:
-            rq['enterprise_id'] = params.enterprise_id
-
         if params.mfa_token:
             rq['2fa_token'] = params.mfa_token
             rq['2fa_type'] = params.mfa_type or 'device_token'
             if params.mfa_type == 'one_time':
                 expire_token = params.config.get('device_token_expiration') or False
-                expire_days = 0 if expire_token else 9999
+                expire_days = 30 if expire_token else 9999
                 rq['device_token_expire_days'] = expire_days
 
-        rq['client_version'] = rest_api.LEGACY_CLIENT_VERSION   # this login only supports up to v14 clients.
-
         response_json = run_command(params, rq)
 
         if 'device_token' in response_json:
             logging.debug('params.mfa_token=%s', params.mfa_token)
             params.mfa_token = response_json['device_token']
-            params.mfa_type = 'device_token'
             if response_json.get('dt_scope') == 'expiration':
                 store_config = True
                 params.config['mfa_token'] = params.mfa_token
 
         if 'keys' in response_json:
             keys = response_json['keys']
             if 'encryption_params' in keys:
@@ -156,54 +137,44 @@
 
         if 'session_token' in response_json:
             params.session_token = response_json['session_token']
 
         if response_json['result_code'] == 'auth_success' and response_json['result'] == 'success':
             success = True
             logging.debug('Auth Success')
-            store_config = not params.config or params.config.get('user') != params.user
 
             params.session_token = response_json['session_token']
 
             device_id = base64.urlsafe_b64encode(params.rest_context.device_id).decode('utf-8').rstrip('=')
             if params.config.get('device_id') != device_id:
                 store_config = True
                 params.config['device_id'] = device_id
                 url1 = urllib.parse.urlsplit(params.server)
                 url2 = urllib.parse.urlsplit(params.rest_context.server_base)
                 if url1.netloc != url2.netloc:
                     params.config['server'] = params.rest_context.server_base
 
             params.license = response_json.get('license')
             params.enforcements = response_json.get('enforcements')
-            if params.enforcements:
-                if 'logout_timer_desktop' in params.enforcements:
-                    logout_timer = params.enforcements['logout_timer_desktop']
-                    if logout_timer > 0:
-                        if params.logout_timer == 0 or logout_timer < params.logout_timer:
-                            params.logout_timer = logout_timer
             params.settings = response_json.get('settings')
 
             if response_json.get('is_enterprise_admin'):
                 query_enterprise(params)
-                query_msp(params)
 
             params.sync_data = True
             params.prepare_commands = True
 
-            if store_config:    # save token to config file if the file exists
+            if store_config: # save token to config file if the file exists
                 params.config['user'] = params.user
-
-                if params.config_filename:
-                    try:
-                        with open(params.config_filename, 'w') as f:
-                            json.dump(params.config, f, ensure_ascii=False, indent=2)
-                            logging.info('Updated %s', params.config_filename)
-                    except Exception as e:
-                        logging.debug('Unable to update %s. %s', params.config_filename, e)
+                try:
+                    with open(params.config_filename, 'w') as f:
+                        json.dump(params.config, f, ensure_ascii=False, indent=2)
+                        logging.info('Updated %s', params.config_filename)
+                except Exception as e:
+                    logging.debug('Unable to update %s. %s', params.config_filename, e)
 
         elif response_json['result_code'] in ['need_totp', 'invalid_device_token', 'invalid_totp']:
             try:
                 params.mfa_token = ''
                 params.mfa_type = 'one_time'
 
                 if 'u2f_challenge' in response_json:
@@ -225,15 +196,15 @@
                         logging.error(e)
 
                 while not params.mfa_token:
                     try:
                         params.mfa_token = getpass.getpass(prompt='Two-Factor Code: ', stream=None)
                     except KeyboardInterrupt as e:
                         print('')
-                        params.clear_session()
+                        params.password = None
                         return
 
             except (EOFError, KeyboardInterrupt, SystemExit):
                 return
 
         elif response_json['result_code'] == 'auth_expired':
             try:
@@ -252,19 +223,21 @@
                 if not accept_account_transfer_consent(params, share_account_to):
                     raise AuthenticationError('')
             finally:
                 params.session_token = None
 
         elif response_json['result_code'] == 'auth_failed':
             params.password = ''
-            params.auth_verifier = None
             raise AuthenticationError('Authentication failed.')
 
+        elif response_json['result_code'] == 'throttled':
+            raise AuthenticationError(response_json['message'])
+
         elif response_json['result_code']:
-            raise KeeperApiError(response_json['result_code'], response_json['message'])
+            raise AuthenticationError(response_json['result_code'])
 
         else:
             raise CommunicationError('Unknown problem')
 
 
 def change_master_password(params):
     user_params = rest_api.get_new_user_params(params.rest_context, params.user)
@@ -324,59 +297,40 @@
         return True
     else:
         logging.info('Canceled')
 
     return False
 
 
-def decrypt_aes_plain(data: bytes, key: bytes):
-    cipher = AES.new(key=key, mode=AES.MODE_GCM, nonce=data[:12])
-    return cipher.decrypt_and_verify(data[12:-16], data[-16:])
-
-
 def decrypt_aes(data, key):
-    # type: (str, bytes) -> bytes
     decoded_data = base64.urlsafe_b64decode(data + '==')
     iv = decoded_data[:16]
     ciphertext = decoded_data[16:]
     cipher = AES.new(key, AES.MODE_CBC, iv)
     return cipher.decrypt(ciphertext)
 
 
 def decrypt_data(data, key):
-    # type: (str, bytes) -> bytes
     return unpad_binary(decrypt_aes(data, key))
 
 
-def encrypt_aes_plain(data: bytes, key: bytes):
-    iv = os.urandom(12)
-    cipher = AES.new(key=key, mode=AES.MODE_GCM, nonce=iv)
-    enc_data, tag = cipher.encrypt_and_digest(data)
-    return iv + enc_data + tag
-
-
 def encrypt_aes(data, key):
     iv = os.urandom(16)
     cipher = AES.new(key, AES.MODE_CBC, iv)
     encrypted_data = iv + cipher.encrypt(pad_binary(data))
     return (base64.urlsafe_b64encode(encrypted_data).decode()).rstrip('=')
 
 
 def encrypt_aes_key(key_to_encrypt, encryption_key):
     iv = os.urandom(16)
     cipher = AES.new(encryption_key, AES.MODE_CBC, iv)
     encrypted_data = iv + cipher.encrypt(key_to_encrypt)
     return (base64.urlsafe_b64encode(encrypted_data).decode()).rstrip('=')
 
 
-def encrypt_rsa_plain(data, rsa_key):
-    cipher = PKCS1_v1_5.new(rsa_key)
-    return cipher.encrypt(data)
-
-
 def encrypt_rsa(data, rsa_public_key):
     cipher = PKCS1_v1_5.new(rsa_public_key)
     encrypted_data = cipher.encrypt(data)
     return (base64.urlsafe_b64encode(encrypted_data).decode('utf-8')).rstrip('=')
 
 
 def decrypt_rsa(data, rsa_private_key):
@@ -458,28 +412,25 @@
             team = params.team_cache[team_uid]
             if 'team_key_unencrypted' in team:
                 del team['team_key_unencrypted']
                 if 'shared_folder_keys' in team:
                     for sfk in team['shared_folder_keys']:
                         delete_shared_folder_key(sfk['shared_folder_uid'])
 
-    params.available_team_cache = None
     if 'full_sync' in response_json:
         if response_json['full_sync']:
             if params.debug: print('Full Sync response')
             check_convert_to_folders = True
-            params.record_cache.clear()
-            params.meta_data_cache.clear()
-            params.shared_folder_cache.clear()
-            params.team_cache.clear()
-            params.available_team_cache = None
-            params.non_shared_data_cache.clear()
-            params.subfolder_cache.clear()
-            params.subfolder_record_cache.clear()
-            params.record_history.clear()
+            params.record_cache = {}
+            params.meta_data_cache = {}
+            params.shared_folder_cache = {}
+            params.team_cache = {}
+            params.non_shared_data_cache = {}
+            params.subfolder_cache = {}
+            params.subfolder_record_cache = {}
 
     if 'revision' in response_json:
         logging.debug('Getting revision %d', params.revision)
         params.revision = response_json['revision']
 
     if 'removed_records' in response_json:
         logging.debug('Processing removed records')
@@ -512,16 +463,14 @@
                 del params.team_cache[team_uid]
 
     if 'removed_shared_folders' in response_json:
         logging.debug('Processing removed shared folders')
         for sf_uid in response_json['removed_shared_folders']:
             if sf_uid in params.shared_folder_cache:
                 delete_shared_folder_key(sf_uid)
-                if sf_uid in params.subfolder_record_cache:
-                    del params.subfolder_record_cache[sf_uid]
                 shared_folder = params.shared_folder_cache[sf_uid]
                 if 'shared_folder_key' in shared_folder:
                     del shared_folder['shared_folder_key']
                 if 'key_type' in shared_folder:
                     del shared_folder['key_type']
                 if 'users' in shared_folder:
                     shared_folder['users'] = [x for x in shared_folder['users'] if x['username'] != params.user]
@@ -566,57 +515,55 @@
                 rs = params.subfolder_record_cache[f_uid]
                 r_uid = sfrrr['record_uid']
                 if r_uid in rs:
                     rs.remove(r_uid)
 
     if 'non_shared_data' in response_json:
         for non_shared_data in response_json['non_shared_data']:
-            if 'data' in non_shared_data and non_shared_data['data']:
-                try:
-                    decrypted_data = decrypt_data(non_shared_data['data'], params.data_key)
-                    non_shared_data['data_unencrypted'] = decrypted_data
-                    params.non_shared_data_cache[non_shared_data['record_uid']] = non_shared_data
-                except:
-                    logging.debug('Non-shared data for record %s could not be decrypted', non_shared_data['record_uid'])
+            try:
+                decrypted_data = decrypt_data(non_shared_data['data'], params.data_key)
+                non_shared_data['data_unencrypted'] = decrypted_data
+                params.non_shared_data_cache[non_shared_data['record_uid']] = non_shared_data
+            except:
+                logging.debug('Non-shared data for record %s could not be decrypted', non_shared_data['record_uid'])
 
     # convert record keys from RSA to AES-256
     if 'record_meta_data' in response_json:
         logging.debug('Processing record_meta_data')
         for meta_data in response_json['record_meta_data']:
-            try:
-                if 'record_key' not in meta_data:
-                    # old record that doesn't have a record key so make one
-                    logging.debug('...no record key.  creating...')
-                    # store as b64 encoded string
-                    # note: decode() converts bytestream (b') to string
-                    # note2: remove == from the end
-                    meta_data['record_key_unencrypted'] = os.urandom(32)
+
+            if 'record_key' not in meta_data:
+                # old record that doesn't have a record key so make one
+                logging.debug('...no record key.  creating...')
+                # store as b64 encoded string
+                # note: decode() converts bytestream (b') to string
+                # note2: remove == from the end
+                meta_data['record_key_unencrypted'] = os.urandom(32)
+                meta_data['record_key'] = encrypt_aes(meta_data['record_key_unencrypted'], params.data_key)
+                meta_data['record_key_type'] = 1
+                # temporary flag for decryption routine below
+                meta_data['old_record_flag'] = True
+                meta_data['is_converted_record_type'] = True
+
+            elif meta_data['record_key_type'] == 2:
+                logging.debug('Converting RSA-encrypted key')
+                # decrypt the type2 key using their RSA key
+                unencrypted_key = decrypt_rsa(meta_data['record_key'], params.rsa_key)
+                if len(unencrypted_key) == 32:
+                    meta_data['record_key_unencrypted'] = unencrypted_key
                     meta_data['record_key'] = encrypt_aes(meta_data['record_key_unencrypted'], params.data_key)
                     meta_data['record_key_type'] = 1
-                    # temporary flag for decryption routine below
-                    meta_data['old_record_flag'] = True
                     meta_data['is_converted_record_type'] = True
 
-                elif meta_data['record_key_type'] == 2:
-                    logging.debug('Converting RSA-encrypted key')
-                    # decrypt the type2 key using their RSA key
-                    unencrypted_key = decrypt_rsa(meta_data['record_key'], params.rsa_key)
-                    if len(unencrypted_key) == 32:
-                        meta_data['record_key_unencrypted'] = unencrypted_key
-                        meta_data['record_key'] = encrypt_aes(meta_data['record_key_unencrypted'], params.data_key)
-                        meta_data['record_key_type'] = 1
-                        meta_data['is_converted_record_type'] = True
-
-                elif meta_data['record_key_type'] == 1:
-                    meta_data['record_key_unencrypted'] = decrypt_data(meta_data['record_key'], params.data_key)
-            except Exception as e:
-                logging.debug('Decryption error: %s', e)
+            elif meta_data['record_key_type'] == 1:
+                meta_data['record_key_unencrypted'] = decrypt_data(meta_data['record_key'], params.data_key)
 
             # add to local cache
             if 'record_key_unencrypted' in meta_data:
+                logging.debug('Adding meta data to cache for ' + meta_data['record_uid'])
                 params.meta_data_cache[meta_data['record_uid']] = meta_data
             else:
                 logging.error('Could not decrypt meta data key: %s', meta_data['record_uid'])
 
     if 'teams' in response_json:
         for team in response_json['teams']:
             if team['team_key_type'] == 2:
@@ -687,35 +634,29 @@
             params.record_cache[record['record_uid']] = record
 
     # process team keys
     for team_uid in params.team_cache:
         team = params.team_cache[team_uid]
         for sf_key in team['shared_folder_keys']:
             if 'shared_folder_key_unencrypted' not in sf_key:
-                try:
-                    if sf_key['key_type'] == 2:
-                        sf_key['shared_folder_key_unencrypted'] = decrypt_rsa(sf_key['shared_folder_key'], team['team_private_key_unencrypted'])
-                    else:
-                        sf_key['shared_folder_key_unencrypted'] = decrypt_data(sf_key['shared_folder_key'], team['team_key_unencrypted'])
-                except Exception as e:
-                    logging.debug('Decryption error: %s', e)
+                if sf_key['key_type'] == 2:
+                    sf_key['shared_folder_key_unencrypted'] = decrypt_rsa(sf_key['shared_folder_key'], team['team_private_key_unencrypted'])
+                else:
+                    sf_key['shared_folder_key_unencrypted'] = decrypt_data(sf_key['shared_folder_key'], team['team_key_unencrypted'])
 
     # process shared folder keys
     sf_to_delete = []
     for shared_folder_uid in params.shared_folder_cache:
         shared_folder = params.shared_folder_cache[shared_folder_uid]
         if 'shared_folder_key_unencrypted' not in shared_folder:
             if 'shared_folder_key' in shared_folder:
-                try:
-                    if shared_folder['key_type'] == 2:
-                        shared_folder['shared_folder_key_unencrypted'] = decrypt_rsa(shared_folder['shared_folder_key'], params.rsa_key)
-                    else:
-                        shared_folder['shared_folder_key_unencrypted'] = decrypt_data(shared_folder['shared_folder_key'], params.data_key)
-                except Exception as e:
-                    logging.debug('Decryption error: %s', e)
+                if shared_folder['key_type'] == 2:
+                    shared_folder['shared_folder_key_unencrypted'] = decrypt_rsa(shared_folder['shared_folder_key'], params.rsa_key)
+                else:
+                    shared_folder['shared_folder_key_unencrypted'] = decrypt_data(shared_folder['shared_folder_key'], params.data_key)
             else:
                 if 'teams' in shared_folder:
                     teams_to_remove = set()
                     for to in shared_folder['teams']:
                         team_uid = to['team_uid']
                         if team_uid in params.team_cache:
                             team = params.team_cache[team_uid]
@@ -727,27 +668,19 @@
                                         break
                         else:
                             teams_to_remove.add(team_uid)
                         if len(teams_to_remove) > 0:
                             shared_folder['teams'] = [x for x in shared_folder['teams'] if x['team_uid'] not in teams_to_remove]
 
             if 'shared_folder_key_unencrypted' in shared_folder:
-                try:
-                    shared_folder['name_unencrypted'] = decrypt_data(shared_folder['name'], shared_folder['shared_folder_key_unencrypted']).decode('utf-8')
-                except Exception as e:
-                    logging.debug('Shared folder %s name decryption error: %s', shared_folder_uid, e)
-                    shared_folder['name_unencrypted'] = shared_folder_uid
+                shared_folder['name_unencrypted'] = decrypt_data(shared_folder['name'], shared_folder['shared_folder_key_unencrypted']).decode('utf-8')
                 if 'records' in shared_folder:
                     for sfr in shared_folder['records']:
                         if 'record_key_unencrypted' not in sfr:
-                            try:
-                                sfr['record_key_unencrypted'] = decrypt_data(sfr['record_key'], shared_folder['shared_folder_key_unencrypted'])
-                            except Exception as e:
-                                logging.debug('Shared folder %s record key decryption error: %s', shared_folder_uid, e)
-
+                            sfr['record_key_unencrypted'] = decrypt_data(sfr['record_key'], shared_folder['shared_folder_key_unencrypted'])
             else:
                 sf_to_delete.append(shared_folder_uid)
 
     if len(sf_to_delete) > 0:
         for shared_folder_uid in sf_to_delete:
             logging.debug('Delete shared folder with unresolved key: %s', shared_folder_uid)
             del params.shared_folder_cache[shared_folder_uid]
@@ -774,19 +707,16 @@
                         recs = [x['record_key_unencrypted'] for x in shared_folder['records'] if x['record_uid'] == record_uid and 'record_key_unencrypted' in x]
                         if len(recs) > 0:
                             record_key = recs[0]
                             record['record_key_unencrypted'] = record_key
                             break
 
             if record_key:
-                try:
-                    record['data_unencrypted'] = decrypt_data(record['data'], record_key) if 'data' in record else b'{}'
-                    record['extra_unencrypted'] = decrypt_data(record['extra'], record_key) if 'extra' in record else b'{}'
-                except Exception as e:
-                    logging.debug('Record %s data/extra decryption error: %s', record_uid, e)
+                record['data_unencrypted'] = decrypt_data(record['data'], record_key) if 'data' in record else b'{}'
+                record['extra_unencrypted'] = decrypt_data(record['extra'], record_key) if 'extra' in record else b'{}'
             else:
                 records_to_delete.append(record_uid)
 
     for record_uid in records_to_delete:
         params.record_cache.pop(record_uid)
 
     # decrypt user folders
@@ -838,21 +768,23 @@
                 params.subfolder_record_cache[key].add(record_uid)
 
     if 'sharing_changes' in response_json:
         for sharing_change in response_json['sharing_changes']:
             record_uid = sharing_change['record_uid']
             if record_uid in params.record_cache:
                 record = params.record_cache[record_uid]
-                record['shared'] = sharing_change['shared']
-    for record in params.record_cache.values():
-        if 'shares' in record:
-            del record['shares']
+                if 'shares' in record:
+                    del record['shares']
 
     prepare_folder_tree(params)
 
+    logging.debug('--- Meta Data Cache: %s', params.meta_data_cache)
+    logging.debug('--- Record Cache: %s', params.record_cache)
+    logging.debug('--- Folders Cache: %s', params.shared_folder_cache)
+
     if 'pending_shares_from' in response_json:
         params.pending_share_requests.update(response_json['pending_shares_from'])
 
     try:
         if check_convert_to_folders:
             rq = {
                 'command': 'check_flag',
@@ -916,38 +848,38 @@
 
 def create_auth_verifier(password, salt, iterations):
     # type: (str, bytes, int) -> str
 
     derived_key = derive_key(password, salt, iterations)
     enc_iter = int.to_bytes(iterations, length=3, byteorder='big', signed=False)
     auth_ver = b'\x01' + enc_iter + salt + derived_key
-    return loginv3.CommonHelperMethods.bytes_to_url_safe_str(auth_ver)
+    return base64.urlsafe_b64encode(auth_ver).decode().strip('=')
 
 
 def create_encryption_params(password, salt, iterations, data_key):
     # type: (str, bytes, int, bytes) -> str
 
     derived_key = derive_key(password, salt, iterations)
     enc_iter = int.to_bytes(iterations, length=3, byteorder='big', signed=False)
     enc_iv = os.urandom(16)
     cipher = AES.new(derived_key, AES.MODE_CBC, enc_iv)
     enc_data_key = cipher.encrypt(data_key + data_key)
     enc_params = b'\x01' + enc_iter + salt + enc_iv + enc_data_key
-    return loginv3.CommonHelperMethods.bytes_to_url_safe_str(enc_params)
+    return base64.urlsafe_b64encode(enc_params).decode().strip('=')
 
 
 def decrypt_encryption_params(encryption_params, password):
     """ Decrypt the data key returned by the server 
     Format:
     1 byte: Version number (currently only 1)
     3 bytes: Iterations, unsigned integer, big endian
     16 bytes: salt
     80 bytes: encrypted data key (broken down further below)
-        16 bytes: IV
-        64 bytes: ciphertextIn
+    16 bytes: IV
+    64 bytes: ciphertextIn
     Key for encrypting the data key: 
         PBKDF2_with_HMAC_SHA256(iterations, salt, master password, 256-bit)
     Encryption method: 256-bit AES, CBC mode, no padding
     Verification: the decrypted ciphertext should contain two 32 byte values, 
         identical to each other.
     """
     if not encryption_params:
@@ -979,58 +911,42 @@
 
     logging.debug('Decrypted data key with success.')
 
     # save the encryption params 
     return decrypted_data_key[:32]
 
 
-def decrypt_data_key(params: KeeperParams, encrypted_data_key):
-
-    encrypted_data_key_len = len(encrypted_data_key)
-
-    # [12 bytes: nonce / iv]
-    # [32 bytes: ciphertext]
-    # [16 bytes: auth - tag]
-
-    if encrypted_data_key_len != 60:
-        raise CryptoError('Invalid encryption params: Encrypted data key was unexpected length ' + str(encrypted_data_key_len))
-
-    decryption_key = rest_api.derive_key_v2('data_key', params.password, params.salt, params.iterations)
-
-    return rest_api.decrypt_aes(encrypted_data_key, decryption_key)
-
-
 def get_record(params,record_uid):
     """Return the referenced record cache"""
     record_uid = record_uid.strip()
 
     if not record_uid:
         logging.warning('No record UID provided')
         return
 
     if not params.record_cache:
         logging.warning('No record cache.  Sync down first.')
         return
 
     if not record_uid in params.record_cache:
-        logging.warning('Record UID %s not found in cache.' % record_uid)
+        logging.warning('Record UID not found.')
         return
 
     cached_rec = params.record_cache[record_uid]
+    logging.debug('Cached rec: %s', cached_rec)
+
     rec = Record()
 
     try:
         data = json.loads(cached_rec['data_unencrypted'].decode('utf-8'))
         rec = Record(record_uid)
         extra = None
         if 'extra_unencrypted' in cached_rec:
             extra = json.loads(cached_rec['extra_unencrypted'].decode('utf-8'))
         rec.load(data, revision=cached_rec['revision'], extra=extra)
-        if not resolve_record_view_path(params, record_uid):
-            rec.mask_password()
     except:
         logging.error('**** Error decrypting record %s', record_uid)
 
     return rec
 
 
 def is_shared_folder(params,shared_folder_uid):
@@ -1085,80 +1001,14 @@
 
     sf = SharedFolder(shared_folder_uid)
     sf.load(cached_sf, cached_sf['revision'])
 
     return sf
 
 
-def load_user_public_keys(params, emails):  # type: (KeeperParams, list) -> None
-    emails_to_load = [x for x in emails if x.lower() not in params.key_cache]
-    if not emails_to_load:
-        return
-    rq = {
-        'command': 'public_keys',
-        'key_owners': emails
-    }
-    rs = communicate(params, rq)
-    if 'public_keys' in rs:
-        for pk in rs['public_keys']:
-            if 'public_key' in pk:
-                email = pk['key_owner']
-                public_key = base64.urlsafe_b64decode(pk['public_key'] + '==')
-                try:
-                    params.key_cache[email] = RSA.importKey(public_key)
-                except Exception as e:
-                    logging.debug(e)
-
-
-def load_team_keys(params, team_uids):          # type: (KeeperParams, list) -> None
-    uids_to_load = [x for x in team_uids if x not in params.key_cache]
-    if not uids_to_load:
-        return
-    rq = {
-        'command': 'team_get_keys',
-        'teams': uids_to_load
-    }
-    rs = communicate(params, rq)
-    if 'keys' in rs:
-        for tk in rs['keys']:
-            if 'key' in tk:
-                team_uid = tk['team_uid']
-                try:
-                    if tk['type'] == 1:
-                        params.key_cache[team_uid] = decrypt_data(tk['key'], params.data_key)
-                    elif tk['type'] == 2:
-                        params.key_cache[team_uid] = decrypt_rsa(tk['key'], params.rsa_key)
-                    elif tk['type'] == 3:
-                        public_key = base64.urlsafe_b64decode(tk['key'] + '==')
-                        params.key_cache[team_uid] = RSA.importKey(public_key)
-                except Exception as e:
-                    logging.debug(e)
-
-
-def load_available_teams(params):
-    if params.available_team_cache is not None:
-        return
-
-    rq = {
-        'command': 'get_available_teams'
-    }
-    try:
-        rs = communicate(params, rq)
-        params.available_team_cache = rs.get('teams')
-        for t in params.available_team_cache:
-            team_uid = t['team_uid']
-            if team_uid in params.team_cache:
-                team = params.team_cache[team_uid]
-                if 'team_key_unencrypted' in team:
-                    params.key_cache[team_uid] = team['team_key_unencrypted']
-
-    except Exception as e:
-        logging.debug(e)
-
-
 def get_team(params,team_uid):
     """Return the referenced team """
     team_uid = team_uid.strip()
 
     if not team_uid:
         logging.warning('No team UID provided')
         return
@@ -1206,16 +1056,20 @@
 
     search_results = [] 
 
     for shared_folder_uid in params.shared_folder_cache:
 
         logging.debug('Getting Shared Folder UID: %s', shared_folder_uid)
         sf = get_shared_folder(params, shared_folder_uid)
+
+        logging.debug('sf: %s', sf)
         target = sf.to_lowerstring()
 
+        logging.debug('Lowercase: %s', target)
+
         if p.search(target):
             logging.debug('Search success')
             search_results.append(sf)
      
     return search_results
 
 
@@ -1228,22 +1082,26 @@
     search_results = [] 
 
     for team_uid in params.team_cache:
 
         logging.debug('Getting Team UID: %s', team_uid)
         team = get_team(params, team_uid)
 
+        logging.debug('team: %s', team)
         target = team.to_lowerstring()
 
+        logging.debug('Lowercase: %s', target)
+
         if p.search(target):
             logging.debug('Search success')
             search_results.append(team)
      
     return search_results
 
+
 def prepare_record(params, record):
     """ Prepares the Record() object to be sent to the Keeper Cloud API
         by serializing and encrypting it in the proper JSON format used for
         transmission.  If the record has no UID, one is generated and the
         encrypted record key is sent to the server.  If this record was
         converted from RSA to AES we send the new record key. If the record
         is in a shared folder, must send shared folder UID for edit permission.
@@ -1270,19 +1128,15 @@
         if path:
             record_object.update(path)
         else:
             logging.error('You do not have edit permissions on this record')
             return None
 
         rec = params.record_cache[record.record_uid]
-
         data.update(json.loads(rec['data_unencrypted'].decode('utf-8')))
-        if data.get('secret2') != record.password:
-            params.queue_audit_event('record_password_change', record_uid=record.record_uid)
-
         if 'extra' in rec:
             extra.update(json.loads(rec['extra_unencrypted'].decode('utf-8')))
         if 'udata' in rec:
             udata.update(rec['udata'])
         unencrypted_key = rec['record_key_unencrypted']
         record_object['revision'] = rec['revision']
         if record.record_uid in params.meta_data_cache and params.meta_data_cache[record.record_uid].get('is_converted_record_type'):
@@ -1297,126 +1151,83 @@
     data['title'] = record.title
     data['folder'] = record.folder
     data['secret1'] = record.login
     data['secret2'] = record.password
     data['link'] = record.login_url
     data['notes'] = record.notes
     data['custom'] = record.custom_fields
-    Record.validate_record_data(data, extra, udata)
 
     record_object['data'] = encrypt_aes(json.dumps(data).encode('utf-8'), unencrypted_key)
     record_object['extra'] = encrypt_aes(json.dumps(extra).encode('utf-8'), unencrypted_key)
     record_object['udata'] = udata
 
-    try:
-        if params.license and 'account_type' in params.license:
-            if record.password and params.license['account_type'] == 2:
-                for record_uid in params.record_cache:
-                    if record_uid != record.record_uid:
-                        rec = get_record(params, record_uid)
-                        if rec.password == record.password:
-                            params.queue_audit_event('reused_password', record_uid=record.record_uid)
-                            break
-    except:
-        pass
-
     return record_object
 
 
-def communicate_rest(params, request, endpoint):
-    api_request_payload = proto.ApiRequestPayload()
-    if params.session_token:
-        api_request_payload.encryptedSessionToken = base64.urlsafe_b64decode(params.session_token + '==')
-    if request:
-        api_request_payload.payload = request.SerializeToString()
-
-    rs = None
-    try:
-        rs = rest_api.execute_rest(params.rest_context, endpoint, api_request_payload)
-    except Exception as e:
-        raise KeeperApiError('Rest API', str(e))
-    if type(rs) == bytes:
-        return rs
-    elif type(rs) == dict:
-        raise KeeperApiError(rs['error'], rs['message'])
-    raise KeeperApiError('Error', endpoint)
-
-
 def communicate(params, request):
     # type: (KeeperParams, dict) -> dict
 
     def authorize_request(rq):
         rq['client_time'] = current_milli_time()
         rq['locale'] = 'en_US'
         rq['device_id'] = 'Commander'
         rq['session_token'] = params.session_token
-        rq['username'] = params.user.lower()
+        rq['username'] = params.user
 
     if not params.session_token:
         login(params)
 
     authorize_request(request)
     logging.debug('payload: %s', request)
 
     response_json = run_command(params, request)
 
     if response_json['result_code'] == 'auth_failed':
         logging.debug('Re-authorizing.')
         login(params)
-        if not params.session_token:
-            return response_json
         authorize_request(request)
         response_json = run_command(params, request)
+
     if response_json['result'] != 'success':
         if response_json['result_code']:
-            if response_json['result_code'] == 'auth_failed':
-                params.clear_session()
-            else:
-                raise KeeperApiError(response_json['result_code'], response_json['message'])
+            raise KeeperApiError(response_json['result_code'], response_json['message'])
 
     return response_json
 
 
 def execute_batch(params, requests):
-    # type: (KeeperParams, [dict]) -> [dict]
-    responses = []
     if not requests:
-        return responses
+        return
 
-    chunk_size = 80
+    chunk_size = 100
     queue = requests.copy()
     while len(queue) > 0:
         chunk = queue[:chunk_size]
         queue = queue[chunk_size:]
 
         rq = {
             'command': 'execute',
             'requests': chunk
         }
         try:
             rs = communicate(params, rq)
             if 'results' in rs:
-                results = rs['results']  # type: list
+                results = rs['results']
                 if len(results) > 0:
-                    responses.extend(results)
                     if params.debug:
                         pos = len(results) - 1
                         req = chunk[pos]
                         res = results[pos]
                         if res['result'] != 'success':
                             logging.info('execute failed: command %s: %s)', req.get('command'), res.get('message'))
                     if len(results) < len(chunk):
                         queue = chunk[len(results):] + queue
 
         except Exception as e:
             logging.error(e)
-        if len(chunk) > 50:
-            time.sleep(5)
-
-    return responses
 
 
 def update_record(params, record, **kwargs):
     """ Push a record update to the cloud. 
         Takes a Record() object, converts to record JSON
         and pushes to the Keeper cloud API
     """
@@ -1442,15 +1253,15 @@
         return False
 
     if new_revision == record_rq['revision']:
         logging.error('Error: Revision did not change')
         return False
 
     if not kwargs.get('silent'):
-        logging.info('Update record successful for record_uid=%s, revision=%d, new_revision=%s',
+        logging.info('New record successful for record_uid=%s, revision=%d, new_revision=%s',
                      record_rq['record_uid'], record_rq['revision'], new_revision)
 
     record_rq['revision'] = new_revision
 
     # sync down the data which updates the caches
     sync_down(params)
 
@@ -1511,15 +1322,15 @@
 
 def store_non_shared_data(params, record_uid, data):
     # type: (KeeperParams, str, dict) -> None
     if record_uid not in params.record_cache:
         logging.error('Record UID %s does not exist.', record_uid)
         return
 
-    ur = resolve_record_access_path(params, record_uid)
+    ur = resolve_record_write_path(params, record_uid)
     ur['non_shared_data'] = encrypt_aes(json.dumps(data).encode('utf-8'), params.data_key)
     ur['client_modified_time'] = current_milli_time()
     ur['version'] = 2
     if record_uid in params.non_shared_data_cache:
         ur['revision'] = params.non_shared_data_cache[record_uid]['revision']
     else:
         ur['revision'] = 0
@@ -1527,15 +1338,14 @@
     request = {
         'command': 'record_update',
         'update_records': [ur]
     }
     _ = communicate(params, request)
     sync_down(params)
 
-
 def generate_record_uid():
     """ Generate url safe base 64 16 byte uid """
     return base64.urlsafe_b64encode(os.urandom(16)).decode().rstrip('=')
 
 
 def generate_aes_key():
     return os.urandom(32)
@@ -1547,32 +1357,24 @@
     params.root_folder = RootFolderNode()
 
     for sf in params.subfolder_cache.values():
         if sf['type'] == 'user_folder':
             uf = UserFolderNode()
             uf.uid = sf['folder_uid']
             uf.parent_uid = sf.get('parent_uid')
-            try:
-                data = json.loads(decrypt_data(sf['data'], sf['folder_key_unencrypted']).decode())
-            except Exception as e:
-                logging.debug('Error decrypting user folder name. Folder UID: %s. Error: %s', uf.uid, e)
-                data = {}
+            data = json.loads(decrypt_data(sf['data'], sf['folder_key_unencrypted']).decode())
             uf.name = data['name'] if 'name' in data else uf.uid
             params.folder_cache[uf.uid] = uf
 
         elif sf['type'] == 'shared_folder_folder':
             sff = SharedFolderFolderNode()
             sff.uid = sf['folder_uid']
             sff.shared_folder_uid = sf['shared_folder_uid']
             sff.parent_uid = sf.get('parent_uid') or sff.shared_folder_uid
-            try:
-                data = json.loads(decrypt_data(sf['data'], sf['folder_key_unencrypted']).decode())
-            except Exception as e:
-                logging.debug('Error decrypting shared folder folder name. Folder UID: %s. Error: %s', sff.uid, e)
-                data = {}
+            data = json.loads(decrypt_data(sf['data'], sf['folder_key_unencrypted']).decode())
             sff.name = data['name'] if 'name' in data else sff.uid
             params.folder_cache[sff.uid] = sff
 
         elif sf['type'] == 'shared_folder':
             shf = SharedFolderNode()
             shf.uid = sf['shared_folder_uid']
             shf.parent_uid = sf.get('folder_uid')
@@ -1583,124 +1385,95 @@
 
     for f in params.folder_cache.values():
         parent_folder = params.folder_cache.get(f.parent_uid) if f.parent_uid else params.root_folder
         if parent_folder:
             parent_folder.subfolders.append(f.uid)
 
 
-def resolve_record_permission_path(params, record_uid, permission):
-    # type: (KeeperParams, str, str) -> dict or None
+def resolve_record_write_path(params, record_uid):
+    path = {
+        'record_uid': record_uid
+    }
 
-    for ap in enumerate_record_access_paths(params, record_uid):
-        if ap.get(permission):
-            path = {
-                'record_uid': record_uid
-            }
-            if 'shared_folder_uid' in ap:
-                path['shared_folder_uid'] = ap['shared_folder_uid']
-            if 'team_uid' in ap:
-                path['team_uid'] = ap['team_uid']
+    if record_uid in params.meta_data_cache:
+        rmd = params.meta_data_cache[record_uid]
+        if rmd['can_edit']:
             return path
 
+    #shared through shared folder
+    for sf in params.shared_folder_cache.values():
+        if 'records' in sf:
+            for ro in sf['records']:
+                if ro['record_uid'] == record_uid:
+                    if ro['can_edit']:
+                        if 'key_type' in sf:
+                            path['shared_folder_uid'] = sf['shared_folder_uid']
+                            return path
+                        elif 'teams' in sf: #check team
+                            for to in sf['teams']:
+                                if to['manage_records']:
+                                    team = params.team_cache[to['team_uid']]
+                                    if not team['restrict_edit']:
+                                        path['shared_folder_uid'] = sf['shared_folder_uid']
+                                        path['team_uid'] = team['team_uid']
+                                        return path
     return None
 
 
-def resolve_record_write_path(params, record_uid):
-    # type: (KeeperParams, str) -> dict or None
-    return resolve_record_permission_path(params, record_uid, 'can_edit')
-
-
 def resolve_record_share_path(params, record_uid):
-    # type: (KeeperParams, str) -> dict or None
-    return resolve_record_permission_path(params, record_uid, 'can_share')
+    path = {
+        'record_uid': record_uid
+    }
 
+    if record_uid in params.meta_data_cache:
+        rmd = params.meta_data_cache[record_uid]
+        if rmd['can_share']:
+            return path
 
-def resolve_record_view_path(params, record_uid):
-    # type: (KeeperParams, str) -> dict or None
-    return resolve_record_permission_path(params, record_uid, 'can_view')
+    #shared through shared folder
+    for sf in params.shared_folder_cache.values():
+        if 'records' in sf:
+            for ro in sf['records']:
+                if ro['record_uid'] == record_uid:
+                    if ro['can_share']:
+                        if 'key_type' in sf:
+                            path['shared_folder_uid'] = sf['shared_folder_uid']
+                            return path
+                        elif 'teams' in sf: #check team
+                            for to in sf['teams']:
+                                if to['manage_records']:
+                                    team = params.team_cache[to['team_uid']]
+                                    if not team['restrict_share']:
+                                        path['shared_folder_uid'] = sf['shared_folder_uid']
+                                        path['team_uid'] = team['team_uid']
+                                        return
+    return None
 
 
 def resolve_record_access_path(params, record_uid, path=None):
-    # type: (KeeperParams, str, dict or None) -> dict
-    best_path = None
-
-    for ap in enumerate_record_access_paths(params, record_uid):
-        use_this_path = False
-        if not best_path:
-            use_this_path = True
-        else:
-            if not best_path.get('can_edit') and ap.get('can_edit'):
-                use_this_path = True
-            elif not best_path.get('can_share') and ap.get('can_share'):
-                use_this_path = True
-            elif not best_path.get('can_view') and ap.get('can_view'):
-                use_this_path = True
-
-        if use_this_path:
-            best_path = ap
-            if best_path.get('can_edit') and best_path.get('can_share') and best_path.get('can_view'):
-                break
-
     if path is None:
         path = {}
 
-    if best_path:
-        path['record_uid'] = best_path['record_uid']
-        if 'shared_folder_uid' in best_path:
-            path['shared_folder_uid'] = best_path['shared_folder_uid']
-        if 'team_uid' in best_path:
-            path['team_uid'] = best_path['team_uid']
-
+    path['record_uid'] = record_uid
+    if not record_uid in params.meta_data_cache: #shared through shared folder
+        for sf_uid in params.shared_folder_cache:
+            sf = params.shared_folder_cache[sf_uid]
+            if 'records' in sf:
+                if any(sfr['record_uid'] == record_uid for sfr in sf['records']):
+                    if not 'key_type' in sf:
+                        if 'teams' in sf:
+                            for team in sf['teams']:
+                                path['shared_folder_uid'] = sf_uid
+                                path['team_uid'] = team['team_uid']
+                    else:
+                        path['shared_folder_uid'] = sf_uid
+                        break
     return path
 
 
-def enumerate_record_access_paths(params, record_uid):
-    # type: (KeeperParams, str) -> collections.Iterable[dict]
-
-    if record_uid in params.meta_data_cache:
-        rmd = params.meta_data_cache[record_uid]
-        yield {
-            'record_uid': record_uid,
-            'can_edit': rmd.get('can_edit') or False,
-            'can_share': rmd.get('can_share') or False,
-            'can_view': True
-        }
-
-    for sf_uid in params.shared_folder_cache:
-        sf = params.shared_folder_cache[sf_uid]
-        if 'records' in sf:
-            sfrs = [x for x in sf['records'] if x['record_uid'] == record_uid]
-            if len(sfrs) > 0:
-                sfr = sfrs[0]
-                can_edit = sfr['can_edit']
-                can_share = sfr['can_share']
-                if 'key_type' in sf:
-                    yield {
-                        'record_uid': record_uid,
-                        'shared_folder_uid': sf_uid,
-                        'can_edit': can_edit,
-                        'can_share': can_share,
-                        'can_view': True
-                    }
-                else:
-                    if 'teams' in sf:
-                        for sf_team in sf['teams']:
-                            team_uid = sf_team['team_uid']
-                            if team_uid in params.team_cache:
-                                team = params.team_cache[team_uid]
-                                yield {
-                                    'record_uid': record_uid,
-                                    'shared_folder_uid': sf_uid,
-                                    'team_uid': team_uid,
-                                    'can_edit': can_edit and not team['restrict_edit'],
-                                    'can_share': can_share and not team['restrict_share'],
-                                    'can_view': not team['restrict_view']
-                                }
-
-
 def get_record_shares(params, record_uids):
 
     def need_share_info(record_uid):
         if record_uid in params.record_cache:
             rec = params.record_cache[record_uid]
             return rec.get('shared') and 'shares' not in rec
         return False
@@ -1731,83 +1504,35 @@
                     if 'shared_folder_permissions' in r:
                         rec['shares']['shared_folder_permissions'] = r['shared_folder_permissions']
 
         except Exception as e:
             logging.error(e)
 
 
-def query_msp(params):
-    def fix_data(d):
-        idx = d.rfind(b'}')
-        if idx < len(d) - 1:
-            d = d[:idx+1]
-        return d
-
-    request = {
-        'command': 'get_enterprise_data',
-        'include': ['managed_companies']
-    }
-
-    try:
-        response = communicate(params, request)
-        if response['result'] == 'success':
-            if 'key_type_id' in response:
-                tree_key = None
-                if response['key_type_id'] == 1:
-                    tree_key = decrypt_data(response['tree_key'], params.data_key)
-                elif response['key_type_id'] == 2:
-                    tree_key = decrypt_rsa(response['tree_key'], params.rsa_key)
-                if not tree_key is None:
-                    tree_key = tree_key[:32]
-                    response['unencrypted_tree_key'] = tree_key
-                    if 'managed_companies' in response:
-                        for mc in response['managed_companies']:
-                            mc['data'] = {}
-                            if 'encrypted_data' in mc:
-                                try:
-                                    data = decrypt_data(mc['encrypted_data'], tree_key)
-                                    data = fix_data(data)
-                                    mc['data'] = json.loads(data.decode('utf-8'))
-                                except Exception as e:
-                                    pass
-                        if params.enterprise:
-                            params.enterprise['managed_companies'] = response['managed_companies']
-    except:
-        pass
-
-
 def query_enterprise(params):
     def fix_data(d):
         idx = d.rfind(b'}')
         if idx < len(d) - 1:
             d = d[:idx+1]
         return d
 
     request = {
         'command': 'get_enterprise_data',
         'include': ['nodes', 'users', 'teams', 'team_users', 'roles', 'role_enforcements', 'role_privileges',
-                    'role_users', 'managed_nodes', 'role_keys', 'role_keys2', 'licenses', 'queued_teams', 'queued_team_users',
-                    'licenses', 'keys', 'scims']
+                    'role_users', 'managed_nodes', 'role_keys', 'licenses', 'queued_teams', 'queued_team_users']
     }
     try:
         response = communicate(params, request)
         if response['result'] == 'success':
             if 'key_type_id' in response:
                 tree_key = None
                 if response['key_type_id'] == 1:
-                    tree_key = decrypt_data(response['tree_key'], params.data_key)  # old AES
+                    tree_key = decrypt_data(response['tree_key'], params.data_key)
                 elif response['key_type_id'] == 2:
-                    if params.enterprise_id > 0:
-
-                        decoded_data = base64.urlsafe_b64decode(response['tree_key'] + '==')
-
-                        tree_key = rest_api.decrypt_aes(decoded_data, params.msp_tree_key)  # new AES
-                        # tree_key = decrypt_data(response['tree_key'], msp_tree_key)
-                    else:
-                        tree_key = decrypt_rsa(response['tree_key'], params.rsa_key) # old RSA
+                    tree_key = decrypt_rsa(response['tree_key'], params.rsa_key)
                 if not tree_key is None:
                     tree_key = tree_key[:32]
                     response['unencrypted_tree_key'] = tree_key
                     if 'nodes' in response:
                         for node in response['nodes']:
                             node['data'] = {}
                             if 'encrypted_data' in node:
@@ -1822,79 +1547,22 @@
                             user['data'] = {}
                             if 'encrypted_data' in user:
                                 try:
                                     data = decrypt_data(user['encrypted_data'], tree_key)
                                     data = fix_data(data)
                                     user['data'] = json.loads(data.decode('utf-8'))
                                 except Exception as e:
-                                    if 'key_type' in user and user['key_type'] == 'no_key':
-                                        user['data']['displayname'] = user.get('encrypted_data') or ''
+                                    pass
                     if 'roles' in response:
                         for role in response['roles']:
                             role['data'] = {}
                             if 'encrypted_data' in role:
                                 try:
                                     data = decrypt_data(role['encrypted_data'], tree_key)
                                     data = fix_data(data)
                                     role['data'] = json.loads(data.decode('utf-8'))
                                 except Exception as e:
                                     pass
 
                     params.enterprise = response
-    except Exception as e:
-        logging.debug(e)
+    except:
         params.enterprise = None
-
-
-def login_and_get_mc_params_login_v3(params: KeeperParams, mc_id):
-
-    resp = loginv3.LoginV3API.loginToMc(params.rest_context, params.session_token, mc_id)
-
-    mc_params = KeeperParams(server=params.server, device_id=params.rest_context.device_id)
-
-    mc_params.config = params.config
-    mc_params.auth_verifier = params.auth_verifier
-    mc_params.mfa_token = params.mfa_token
-    mc_params.salt = params.salt
-    mc_params.iterations = params.iterations
-    mc_params.user = params.user
-    mc_params.password = params.password
-    mc_params.enterprise_id = mc_id
-    mc_params.session_token = params.session_token
-    mc_params.login_v3 = params.login_v3
-    mc_params.data_key = params.data_key
-
-    mc_params.session_token = loginv3.CommonHelperMethods.bytes_to_url_safe_str(resp.encryptedSessionToken)
-    mc_params.msp_tree_key = params.enterprise['unencrypted_tree_key']
-
-    query_enterprise(mc_params)
-
-    return mc_params
-
-
-def login_and_get_mc_params(params, mc_id):
-
-    mc_params = KeeperParams(server=params.server, device_id=params.rest_context.device_id)
-
-    mc_params.config = params.config
-    mc_params.auth_verifier = params.auth_verifier
-    mc_params.mfa_token = params.mfa_token
-    mc_params.salt = params.salt
-    mc_params.iterations = params.iterations
-    mc_params.user = params.user
-    mc_params.password = params.password
-    mc_params.enterprise_id = mc_id
-    mc_params.msp_tree_key = params.enterprise['unencrypted_tree_key']
-    mc_params.session_token = None
-
-    login(mc_params)
-    query_enterprise(mc_params)
-
-    return mc_params
-
-
-def get_correct_salt(salts):
-    if len(salts) > 1:
-        salt = next((s for s in salts if s.name.lower() == 'alternate'), salts[0])
-    else:
-        salt = salts[0]
-    return salt
```

### Comparing `keepercommander-4.88/keepercommander/autocomplete.py` & `keepercommander-4.9/keepercommander/autocomplete.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,23 +6,20 @@
 #
 # Keeper Commander
 # Copyright 2018 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import argparse
-import itertools
 import shlex
 
 from prompt_toolkit.completion import Completion, Completer
 
 from .params import KeeperParams
-from .commands.folder import mv_parser
-from .commands.utils import ConnectCommand
-from .commands import commands, enterprise_commands
+from .commands.folder import ls_parser, mv_parser
 from . import api
 
 
 def no_parse_exception(m):
     pass
 
 
@@ -100,16 +97,16 @@
 
         return folder, path
 
     return None
 
 
 class CommandCompleter(Completer):
-    def __init__(self, params, aliases):
-        # type: (CommandCompleter, KeeperParams, dict) -> None
+    def __init__(self, params, commands, aliases):
+        # type: (CommandCompleter, KeeperParams, dict, dict) -> None
         Completer.__init__(self)
         self.params = params
         self.commands = commands
         self.aliases = aliases
 
     @staticmethod
     def fix_input(txt):
@@ -138,45 +135,34 @@
         return txt
 
     def get_completions(self, document, complete_event):
         try:
             if document.is_cursor_at_the_end:
                 pos = document.text.find(' ')
                 if pos == -1:
-                    cmds = [x for x in commands if x.startswith(document.text)]
-                    if self.aliases:
-                        al_cmds = [x[0] for x in self.aliases.items() if type(x[1]) == tuple and x[0].startswith(document.text)]
-                        cmds.extend(al_cmds)
-                    if self.params.enterprise:
-                        e_cmds = [x for x in enterprise_commands if x.startswith(document.text)]
-                        cmds.extend(e_cmds)
+                    cmds = [x for x in self.commands if x.startswith(document.text)]
                     if len(cmds) > 0:
                         cmds.sort()
                         for c in cmds:
                             yield Completion(c, start_position=-len(document.text))
                 elif pos > 0:
                     cmd = document.text[:pos]
                     if cmd in self.aliases:
-                        ali = self.aliases[cmd]
-                        if type(ali) == tuple:
-                            cmd = ali[0]
-                        else:
-                            cmd = ali
+                        cmd = self.aliases[cmd]
                     raw_input = document.text[pos+1:].strip()
                     context = ''
                     extra = dict()
-                    if cmd in {'download-attachment', 'upload-attachment', 'share-record', 'edit', 'append-notes',
-                               'rm', 'clipboard-copy', 'find-password'}:
+                    if cmd in {'download-attachment', 'upload-attachment', 'share-record', 'append-notes', 'rm', 'clipboard-copy'} :
                         args = CommandCompleter.fix_input(raw_input)
                         if args is not None:
                             extra['escape_space'] = args == raw_input
                             opts, _ = record_parser.parse_known_args(shlex.split(args))
                             extra['prefix'] = opts.record or ''
                             context = 'path'
-                    elif cmd in {'ls', 'share-folder', 'mkdir', 'tree', 'rmdir', 'cd', 'record-permission'}:
+                    elif cmd in {'ls', 'share-folder', 'mkdir', 'tree', 'rmdir', 'cd', 'connect'}:
                         args = CommandCompleter.fix_input(raw_input)
                         if args is not None:
                             extra['escape_space'] = args == raw_input
                             opts, _ = folder_parser.parse_known_args(shlex.split(args))
                             extra['prefix'] = opts.folder or ''
                             context = 'folder'
                     elif cmd in {'mv', 'ln'}:
@@ -191,36 +177,23 @@
                                     context = 'folder'
                                 else:
                                     extra['prefix'] = opts.src or ''
                                     context = 'path'
                             else:
                                 extra['prefix'] = opts.dst or ''
                                 context = 'folder'
-                    elif cmd == 'help':
-                        args = CommandCompleter.fix_input(raw_input)
-                        if args is not None:
-                            extra['prefix'] = args
-                            context = 'command'
-                    elif cmd == 'connect':
-                        args = CommandCompleter.fix_input(raw_input)
-                        if args is not None:
-                            extra['prefix'] = args
-                            context = 'connect'
 
                     if context in {'folder', 'path'}:
                         rs = try_resolve_path(self.params, extra['prefix'])
                         if rs is not None:
                             folder, name = rs
-                            is_path = False if name else True
                             for uid in folder.subfolders:
                                 f = self.params.folder_cache[uid]
                                 if f.name.startswith(name) and len(name) < len(f.name):
                                     n = f.name
-                                    if is_path and not extra['prefix'].endswith('/'):
-                                        n = '/' + n
                                     if extra.get('escape_space'):
                                         n = n.replace(' ', '\\ ')
                                     yield Completion(n, display=n + '/', start_position=-len(name))
 
                             if context == 'path':
                                 name = name.lower()
                                 folder_uid = folder.uid or ''
@@ -235,30 +208,10 @@
                                             if n.lower().startswith(name) and len(name) < len(n):
                                                 if extra.get('escape_space'):
                                                     n = n.replace(' ', '\\ ')
                                                 d = n
                                                 if len(d) > 39:
                                                     d = d[:29] + '...' + d[-7:]
                                                 yield Completion(n, display=d, start_position=-len(name))
-                    elif context == 'command':
-                        cmd = extra['prefix']
-                        for c in itertools.chain(commands.keys(), enterprise_commands.keys()):
-                            if c.startswith(cmd):
-                                yield Completion(c, display=c, start_position=-len(cmd))
-                    elif context == 'connect':
-                        ConnectCommand.find_endpoints(self.params)
-                        cmd = extra['prefix']
-                        comp = cmd.casefold()
-                        names = []
-                        unique_names = set()
-                        for x in ConnectCommand.Endpoints:
-                            name = (x.name or '').casefold()
-                            if name not in unique_names:
-                                unique_names.add(name)
-                                if name.startswith(comp):
-                                    names.append(x.name)
-                        for name in names:
-                            yield Completion(name, display=name, start_position=-len(cmd))
-
         except Exception as e:
             pass
```

### Comparing `keepercommander-4.88/keepercommander/commands/enterprise.py` & `keepercommander-4.9/keepercommander/commands/enterprise.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,247 +7,156 @@
 # Keeper Commander
 # Copyright 2018 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import argparse
 import json
+import csv
 import base64
-import string
 
 import requests
 import logging
 import platform
 import datetime
+import fnmatch
 import re
 import gzip
 import time
 import socket
 import ssl
 import hashlib
 import hmac
 import copy
 import os
+import sys
 
-from urllib.parse import urlparse, urlunparse
+from urllib.parse import urlparse
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Util.asn1 import DerSequence
 from Cryptodome.Math.Numbers import Integer
+from tabulate import tabulate
 from asciitree import LeftAligned
 from collections import OrderedDict as OD
-from argparse import RawTextHelpFormatter
 
-from .base import user_choice, suppress_exit, raise_parse_exception, dump_report_data, Command
+from .base import user_choice, suppress_exit, raise_parse_exception, Command
 from .record import RecordAddCommand
-from .. import api, rest_api, APIRequest_pb2 as proto
+from .. import api
 from ..display import bcolors
 from ..record import Record
-from ..params import KeeperParams
+from ..params import KeeperParams, LAST_TEAM_UID
 from ..generator import generate
-from ..error import CommandError
-from .enterprise_pb2 import (EnterpriseUserIds, ApproveUserDeviceRequest, ApproveUserDevicesRequest,
-                             ApproveUserDevicesResponse, EnterpriseUserDataKeys, SetRestrictVisibilityRequest)
-from ..APIRequest_pb2 import ApiRequestPayload, UserDataKeyRequest, UserDataKeyResponse
 
 
 def register_commands(commands):
-    commands['enterprise-down'] = GetEnterpriseDataCommand()
     commands['enterprise-info'] = EnterpriseInfoCommand()
-    commands['enterprise-node'] = EnterpriseNodeCommand()
+    #commands['enterprise-node'] = EnterpriseNodeCommand()
     commands['enterprise-user'] = EnterpriseUserCommand()
     commands['enterprise-role'] = EnterpriseRoleCommand()
     commands['enterprise-team'] = EnterpriseTeamCommand()
     commands['enterprise-push'] = EnterprisePushCommand()
-    commands['team-approve'] = TeamApproveCommand()
-    commands['device-approve'] = DeviceApproveCommand()
-    commands['scim'] = EnterpriseScimCommand()
-
     commands['audit-log'] = AuditLogCommand()
     commands['audit-report'] = AuditReportCommand()
-    commands['security-audit-report'] = SecurityAuditReportCommand()
     commands['user-report'] = UserReportCommand()
 
 
 def register_command_info(aliases, command_info):
-    aliases['al'] = 'audit-log'
-    aliases['ed'] = 'enterprise-down'
     aliases['ei'] = 'enterprise-info'
-    aliases['en'] = 'enterprise-node'
     aliases['eu'] = 'enterprise-user'
     aliases['er'] = 'enterprise-role'
     aliases['et'] = 'enterprise-team'
-    aliases['sar'] = 'security-audit-report'
+    aliases['al'] = 'audit-log'
 
-    for p in [enterprise_data_parser, enterprise_info_parser, enterprise_node_parser, enterprise_user_parser,
-              enterprise_role_parser, enterprise_team_parser,
-              enterprise_push_parser,
-              team_approve_parser, device_approve_parser, scim_parser,
-              audit_log_parser, audit_report_parser, security_audit_report_parser, user_report_parser]:
+    for p in [enterprise_info_parser, enterprise_user_parser, enterprise_role_parser, enterprise_team_parser, enterprise_push_parser,
+              audit_log_parser, audit_report_parser, user_report_parser]:
         command_info[p.prog] = p.description
 
 
-SUPPORTED_USER_COLUMNS = ['name', 'status', 'transfer_status', 'node', 'team_count', 'teams', 'role_count', 'roles']
-SUPPORTED_TEAM_COLUMNS = ['restricts', 'node', 'user_count', 'users']
-SUPPORTED_ROLE_COLUMNS = ['is_visible_below', 'is_new_user', 'is_admin', 'node', 'user_count', 'users']
-
-enterprise_data_parser = argparse.ArgumentParser(prog='enterprise-down|ed',
-                                                                          description='Download & decrypt enterprise data.')
-
-enterprise_info_parser = argparse.ArgumentParser(prog='enterprise-info|ei',
-                                                 description='Display a tree structure of your enterprise.',
-                                                 formatter_class=RawTextHelpFormatter)
+enterprise_info_parser = argparse.ArgumentParser(prog='enterprise-info|ei', description='Display enterprise information')
 enterprise_info_parser.add_argument('-n', '--nodes', dest='nodes', action='store_true', help='print node tree')
 enterprise_info_parser.add_argument('-u', '--users', dest='users', action='store_true', help='print user list')
 enterprise_info_parser.add_argument('-t', '--teams', dest='teams', action='store_true', help='print team list')
 enterprise_info_parser.add_argument('-r', '--roles', dest='roles', action='store_true', help='print role list')
 enterprise_info_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='print ids')
 enterprise_info_parser.add_argument('--node', dest='node', action='store', help='limit results to node (name or ID)')
-enterprise_info_parser.add_argument('--format', dest='format', action='store', choices=['table', 'csv', 'json'],
-                                    default='table', help='output format. applicable to users, teams, and roles.')
-enterprise_info_parser.add_argument('--output', dest='output', action='store',
-                                    help='output file name. (ignored for table format)')
-enterprise_info_parser.add_argument('--columns', dest='columns', action='store',
-                                    help='comma-separated list of available columns per argument:' +
-                                         '\n for `users` (%s)' % ', '.join(SUPPORTED_USER_COLUMNS) +
-                                         '\n for `teams` (%s)' % ', '.join(SUPPORTED_TEAM_COLUMNS) +
-                                         '\n for `roles` (%s)' % ', '.join(SUPPORTED_ROLE_COLUMNS)
-                                    )
-
-enterprise_info_parser.add_argument('pattern', nargs='?', type=str,
-                                    help='search pattern. applicable to users, teams, and roles.')
 enterprise_info_parser.error = raise_parse_exception
 enterprise_info_parser.exit = suppress_exit
 
 
-enterprise_node_parser = argparse.ArgumentParser(prog='enterprise-node|en', description='Manage an enterprise node.')
-enterprise_node_parser.add_argument('--wipe-out', dest='wipe_out', action='store_true', help='wipe out node content')
-enterprise_node_parser.add_argument('--add', dest='add', action='store_true', help='create node')
-enterprise_node_parser.add_argument('--parent', dest='parent', action='store', help='Parent Node Name or ID')
-enterprise_node_parser.add_argument('--name', dest='displayname', action='store', help='set node display name')
-enterprise_node_parser.add_argument('--delete', dest='delete', action='store_true', help='delete node')
-enterprise_node_parser.add_argument('--toggle-isolated', dest='toggle_isolated', action='store_true', help='Render node invisible')
-enterprise_node_parser.add_argument('node', type=str, nargs='+', help='Node Name or ID. Can be repeated.')
+enterprise_node_parser = argparse.ArgumentParser(prog='enterprise-node|en', description='Enterprise node management')
+enterprise_node_parser.add_argument('--wipe-out', action='store_true', help='wipe out node content')
+enterprise_node_parser.add_argument('node', type=str, action='store', help='node name or node ID')
 enterprise_node_parser.error = raise_parse_exception
 enterprise_node_parser.exit = suppress_exit
 
 
-enterprise_user_parser = argparse.ArgumentParser(prog='enterprise-user|eu', description='Manage an enterprise user.')
+enterprise_user_parser = argparse.ArgumentParser(prog='enterprise-user|eu', description='Enterprise user management')
 enterprise_user_parser.add_argument('-f', '--force', dest='force', action='store_true', help='do not prompt for confirmation')
 enterprise_user_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='print ids')
 enterprise_user_parser.add_argument('--expire', dest='expire', action='store_true', help='expire master password')
-enterprise_user_parser.add_argument('--extend', dest='extend', action='store_true', help='extend vault transfer consent by 7 days')
 enterprise_user_parser.add_argument('--lock', dest='lock', action='store_true', help='lock user')
 enterprise_user_parser.add_argument('--unlock', dest='unlock', action='store_true', help='unlock user')
-enterprise_user_parser.add_argument('--disable-2fa', dest='disable_2fa', action='store_true', help='disable 2fa for user')
 enterprise_user_parser.add_argument('--add', dest='add', action='store_true', help='invite user')
 enterprise_user_parser.add_argument('--delete', dest='delete', action='store_true', help='delete user')
 enterprise_user_parser.add_argument('--name', dest='displayname', action='store', help='set user display name')
 enterprise_user_parser.add_argument('--node', dest='node', action='store', help='node name or node ID')
 enterprise_user_parser.add_argument('--add-role', dest='add_role', action='append', help='role name or role ID')
 enterprise_user_parser.add_argument('--remove-role', dest='remove_role', action='append', help='role name or role ID')
 enterprise_user_parser.add_argument('--add-team', dest='add_team', action='append', help='team name or team UID')
 enterprise_user_parser.add_argument('--remove-team', dest='remove_team', action='append', help='team name or team UID')
-enterprise_user_parser.add_argument('email', type=str, nargs='+', help='User Email or ID. Can be repeated.')
+enterprise_user_parser.add_argument('email', type=str, action='store', help='user email or user ID or user search pattern')
 enterprise_user_parser.error = raise_parse_exception
 enterprise_user_parser.exit = suppress_exit
 
 
-enterprise_role_parser = argparse.ArgumentParser(prog='enterprise-role|er', description='Manage an enterprise role(s).')
+enterprise_role_parser = argparse.ArgumentParser(prog='enterprise-role|er', description='Enterprise role management')
 #enterprise_role_parser.add_argument('-f', '--force', dest='force', action='store_true', help='do not prompt for confirmation')
 enterprise_role_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='print ids')
-enterprise_role_parser.add_argument('--add', dest='add', action='store_true', help='create role')
-enterprise_role_parser.add_argument('--visible-below', dest='visible_below', action='store', choices=['on', 'off'], help='visible to all nodes. \'add\' only')
-enterprise_role_parser.add_argument('--new-user', dest='new_user', action='store', choices=['on', 'off'], help='assign this role to new users. \'add\' only')
-enterprise_role_parser.add_argument('--delete', dest='delete', action='store_true', help='delete role')
-enterprise_role_parser.add_argument('--node', dest='node', action='store', help='node Name or ID')
-enterprise_role_parser.add_argument('--name', dest='name', action='store', help='role\'s new name')
 enterprise_role_parser.add_argument('--add-user', dest='add_user', action='append', help='add user to role')
 enterprise_role_parser.add_argument('--remove-user', dest='remove_user', action='append', help='remove user from role')
-enterprise_role_parser.add_argument('--add-admin', dest='add_admin', action='append', help='add managed node to role')
-enterprise_role_parser.add_argument('--cascade', dest='cascade', action='store', choices=['on', 'off'], help='apply to the children nodes. \'add-admin\' only')
-enterprise_role_parser.add_argument('--remove-admin', dest='remove_admin', action='append', help='remove managed node from role')
-enterprise_role_parser.add_argument('role', type=str, nargs='+', help='Role Name ID. Can be repeated.')
+enterprise_role_parser.add_argument('role', type=str, action='store', help='role name or role ID')
 enterprise_role_parser.error = raise_parse_exception
 enterprise_role_parser.exit = suppress_exit
 
 
-enterprise_team_parser = argparse.ArgumentParser(prog='enterprise-team|et', description='Manage an enterprise team.')
+enterprise_team_parser = argparse.ArgumentParser(prog='enterprise-team|et', description='Enterprise team management')
 enterprise_team_parser.add_argument('-f', '--force', dest='force', action='store_true', help='do not prompt for confirmation')
 enterprise_team_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='print ids')
 enterprise_team_parser.add_argument('--add', dest='add', action='store_true', help='create team')
-enterprise_team_parser.add_argument('--approve', dest='approve', action='store_true', help='approve queued team')
 enterprise_team_parser.add_argument('--delete', dest='delete', action='store_true', help='delete team')
 enterprise_team_parser.add_argument('--add-user', dest='add_user', action='append', help='add user to team')
 enterprise_team_parser.add_argument('--remove-user', dest='remove_user', action='append', help='remove user from team')
 enterprise_team_parser.add_argument('--restrict-edit', dest='restrict_edit', choices=['on', 'off'], action='store', help='disable record edits')
 enterprise_team_parser.add_argument('--restrict-share', dest='restrict_share', choices=['on', 'off'], action='store', help='disable record re-shares')
 enterprise_team_parser.add_argument('--restrict-view', dest='restrict_view', choices=['on', 'off'], action='store', help='disable view/copy passwords')
 enterprise_team_parser.add_argument('--node', dest='node', action='store', help='node name or node ID')
-enterprise_team_parser.add_argument('--name', dest='name', action='store', help='team\'s new name')
-enterprise_team_parser.add_argument('team', type=str, nargs='+', help='Team Name or UID')
+enterprise_team_parser.add_argument('team', type=str, action='store', help='team name or team UID (except --add command)')
 enterprise_team_parser.error = raise_parse_exception
 enterprise_team_parser.exit = suppress_exit
 
-team_approve_parser = argparse.ArgumentParser(prog='team-approve', description='Enable or disable automated team and user approval.')
-team_approve_parser.add_argument('--team', dest='team', action='store_true', help='Approve teams only.')
-team_approve_parser.add_argument('--email', dest='user', action='store_true', help='Approve team users only.')
-team_approve_parser.add_argument('--restrict-edit', dest='restrict_edit', choices=['on', 'off'], action='store', help='disable record edits')
-team_approve_parser.add_argument('--restrict-share', dest='restrict_share', choices=['on', 'off'], action='store', help='disable record re-shares')
-team_approve_parser.add_argument('--restrict-view', dest='restrict_view', choices=['on', 'off'], action='store', help='disable view/copy passwords')
-team_approve_parser.error = raise_parse_exception
-team_approve_parser.exit = suppress_exit
-
-device_approve_parser = argparse.ArgumentParser(prog='device-approve', description='Approve Cloud SSO Devices.')
-device_approve_parser.add_argument('--reload', '-r', dest='reload', action='store_true', help='reload list of pending approval requests')
-device_approve_parser.add_argument('--approve', '-a', dest='approve', action='store_true', help='approve user devices')
-device_approve_parser.add_argument('--deny', '-d', dest='deny', action='store_true', help='deny user devices')
-device_approve_parser.add_argument('--trusted-ip', dest='check_ip', action='store_true', help='approve only devices coming from a trusted IP address')
-device_approve_parser.add_argument('--format', dest='format', action='store', choices=['table', 'csv', 'json'],
-                                    default='table', help='Output format. Applicable to list of devices in the queue.')
-device_approve_parser.add_argument('--output', dest='output', action='store',
-                                    help='Output file name (ignored for table format)')
-device_approve_parser.add_argument('device', type=str, nargs='?', action="append", help='User email or device ID')
-device_approve_parser.error = raise_parse_exception
-device_approve_parser.exit = suppress_exit
-
-scim_parser = argparse.ArgumentParser(prog='scim', description='Manage SCIM endpoints.')
-scim_parser.add_argument('command', type=str, nargs='?', help='Automator Command. list, view, create, edit, delete')
-scim_parser.add_argument('target', type=str, nargs='?', help='Automator ID or Name. Command: view, edit, delete')
-scim_parser.add_argument('--reload', '-r', dest='reload', action='store_true', help='Reload list of scim endpoints')
-scim_parser.add_argument('--force', '-f', dest='force', action='store_true', help='Delete with no confirmation')
-scim_parser.add_argument('--node', dest='node', help='Node Name or ID. Command: create')
-scim_parser.add_argument('--prefix', dest='prefix', action='store',
-                         help='Role Prefix. Command: create, edit. '
-                              'SCIM groups staring with prefix will be imported to Keeper as Roles')
-scim_parser.add_argument('--unique-groups', dest='unique_groups', action='store_true',
-                         help='Unique Groups. Command: create, edit')
 
 enterprise_push_parser = argparse.ArgumentParser(prog='enterprise-push', description='Populate user\'s vault with default records')
-enterprise_push_parser.add_argument('--syntax-help', dest='syntax_help', action='store_true', help='Display help on file format and template parameters.')
+enterprise_push_parser.add_argument('--syntax-help', dest='syntax_help', action='store_true', help='display help on file format and template parameters')
 enterprise_push_parser.add_argument('--team', dest='team', action='append', help='Team name or team UID. Records will be assigned to all users in the team.')
-enterprise_push_parser.add_argument('--email', dest='user', action='append', help='User email or User ID. Records will be assigned to the user.')
-enterprise_push_parser.add_argument('file', nargs='?', type=str, action='store', help='File name in JSON format that contains template records.')
+enterprise_push_parser.add_argument('--user', dest='user', action='append', help='User email or User ID. Records will be assigned to the user.')
+enterprise_push_parser.add_argument('file', nargs='?', type=str, action='store', help='file name in JSON format that contains template records')
 enterprise_push_parser.error = raise_parse_exception
 enterprise_push_parser.exit = suppress_exit
 
 
-audit_log_parser = argparse.ArgumentParser(prog='audit-log', description='Export the enterprise audit log.')
-audit_log_parser.add_argument('--anonymize', dest='anonymize', action='store_true', help='Anonymizes audit log by replacing email and user name with corresponding enterprise user id. If user was removed or if user\'s email was changed then the audit report will show that particular entry as deleted user.')
+audit_log_parser = argparse.ArgumentParser(prog='audit-log', description='Export enterprise audit log')
 audit_log_parser.add_argument('--target', dest='target', choices=['splunk', 'syslog', 'syslog-port', 'sumo', 'azure-la', 'json'], required=True, action='store', help='export target')
 audit_log_parser.add_argument('--record', dest='record', action='store', help='keeper record name or UID')
 audit_log_parser.error = raise_parse_exception
 audit_log_parser.exit = suppress_exit
 
 
-audit_report_parser = argparse.ArgumentParser(prog='audit-report', description='Run an audit trail report.')
+audit_report_parser = argparse.ArgumentParser(prog='audit-report', description='Run audit report')
 audit_report_parser.add_argument('--syntax-help', dest='syntax_help', action='store_true', help='display help')
-audit_report_parser.add_argument('--format', dest='format', action='store', choices=['table', 'csv'], default='table', help='output format.')
-audit_report_parser.add_argument('--output', dest='output', action='store', help='output file name. (ignored for table format)')
-audit_report_parser.add_argument('--details', dest='details', action='store_true', help='lookup column details')
-audit_report_parser.add_argument('--report-type', dest='report_type', choices=['raw', 'dim', 'hour', 'day', 'week', 'month', 'span'], required=True, action='store', help='report type')
+audit_report_parser.add_argument('--report-type', dest='report_type', choices=['raw', 'dim', 'hour', 'day', 'week', 'month', 'span'], action='store', help='report type')
 audit_report_parser.add_argument('--report-format', dest='report_format', action='store', choices=['message', 'fields'], help='output format (raw reports only)')
 audit_report_parser.add_argument('--columns', dest='columns', action='append', help='Can be repeated. (ignored for raw reports)')
 audit_report_parser.add_argument('--aggregate', dest='aggregate', action='append', choices=['occurrences', 'first_created', 'last_created'], help='aggregated value. Can be repeated. (ignored for raw reports)')
 audit_report_parser.add_argument('--timezone', dest='timezone', action='store', help='return results for specific timezone')
 audit_report_parser.add_argument('--limit', dest='limit', type=int, action='store', help='maximum number of returned rows')
 audit_report_parser.add_argument('--order', dest='order', action='store', choices=['desc', 'asc'], help='sort order')
 audit_report_parser.add_argument('--created', dest='created', action='store', help='Filter: Created date. Predefined filters: today, yesterday, last_7_days, last_30_days, month_to_date, last_month, year_to_date, last_year')
@@ -256,73 +165,37 @@
 audit_report_parser.add_argument('--to-username', dest='to_username', action='store', help='Filter: Username of event target')
 audit_report_parser.add_argument('--record-uid', dest='record_uid', action='store', help='Filter: Record UID')
 audit_report_parser.add_argument('--shared-folder-uid', dest='shared_folder_uid', action='store', help='Filter: Shared Folder UID')
 audit_report_parser.error = raise_parse_exception
 audit_report_parser.exit = suppress_exit
 
 
-security_audit_report_parser = argparse.ArgumentParser(prog='security-audit-report', description='Run a security audit report.')
-security_audit_report_parser.add_argument('--syntax-help', dest='syntax_help', action='store_true', help='display help')
-security_audit_report_parser.add_argument('--format', dest='format', action='store', choices=['csv', 'json', 'table'], default='table', help='output format.')
-security_audit_report_parser.add_argument('--output', dest='output', action='store', help='output file name. (ignored for table format)')
-security_audit_report_parser.error = raise_parse_exception
-security_audit_report_parser.exit = suppress_exit
-
-
-user_report_parser = argparse.ArgumentParser(prog='user-report', description='Run a user report.')
+user_report_parser = argparse.ArgumentParser(prog='user-report', description='Run user report')
 user_report_parser.add_argument('--format', dest='format', action='store', choices=['table', 'json', 'csv'], default='table', help='output format.')
 user_report_parser.add_argument('--output', dest='output', action='store', help='output file name. (ignored for table format)')
 user_report_parser.add_argument('--days', dest='days', action='store', type=int, default=365, help='number of days to look back for last login.')
 user_report_parser.error = raise_parse_exception
 user_report_parser.exit = suppress_exit
 
 
-def get_user_status_dict(user):
-
-    def lock_text(lock):
-        return 'Locked' if lock == 1 else 'Disabled' if lock == 2 else ''
-
-    account_status = 'Invited' if user['status'] == 'invited' else 'Active'
-
-    if user['lock'] > 0:
-        account_status = lock_text(user['lock'])
-
-    acct_transfer_status = ''
-
-    if 'account_share_expiration' in user:
-        expire_at = datetime.datetime.fromtimestamp(user['account_share_expiration']/1000.0)
-        if expire_at < datetime.datetime.now():
-            acct_transfer_status = 'Blocked'
-        else:
-            acct_transfer_status = 'Pending Transfer'
-    return {
-        'acct_status': account_status,
-        'acct_transfer_status': acct_transfer_status
-    }
-
-
-class GetEnterpriseDataCommand(Command):
-    def get_parser(self):
-        return enterprise_data_parser
-
-    def execute(self, params, **kwargs):
-        api.query_enterprise(params)
+def lock_text(lock):
+    return 'Locked' if lock == 1 else 'Disabled' if lock == 2 else ''
 
 
 class EnterpriseCommand(Command):
     def __init__(self):
         Command.__init__(self)
         self.public_keys = {}
         self.team_keys = {}
 
     def execute_args(self, params, args, **kwargs):
         if params.enterprise:
             Command.execute_args(self, params, args, **kwargs)
         else:
-            raise CommandError('', 'This command  is only available for Administrators of Keeper.')
+            logging.error('This command  is only available for Administrators of Keeper.')
 
     def get_public_keys(self, params, emails):
         # type: (EnterpriseCommand, KeeperParams, dict) -> None
 
         for email in emails:
             emails[email] = self.public_keys.get(email.lower())
 
@@ -338,53 +211,46 @@
         for pko in rs['public_keys']:
             if 'public_key' in pko:
                 public_key = RSA.importKey(base64.urlsafe_b64decode(pko['public_key'] + '=='))
                 self.public_keys[pko['key_owner'].lower()] = public_key
                 emails[pko['key_owner']] = public_key
 
     def get_public_key(self, params, email):
-        # type: (EnterpriseCommand, KeeperParams, str) -> any
+        # type: (EnterpriseCommand, KeeperParams, str) -> None
 
         public_key = self.public_keys.get(email.lower())
         if public_key is None:
             emails = {
                 email: None
             }
             self.get_public_keys(params, emails)
             public_key = emails[email]
 
         return public_key
 
     def get_team_key(self, params, team_uid):
         team_key = self.team_keys.get(team_uid)
         if team_key is None:
-            if 'teams' in params.enterprise:
-                for team in params.enterprise['teams']:
-                    if team['team_uid'] == team_uid:
-                        if 'encrypted_team_key' in team:
-                            enc_team_key = team['encrypted_team_key']  # type: str
-                            team_key = rest_api.decrypt_aes(base64.urlsafe_b64decode(enc_team_key + '=='), params.enterprise['unencrypted_tree_key'])
-                        break
-
-        if team_key is None:
             rq = {
                 'command': 'team_get_keys',
                 'teams': [team_uid]
             }
             rs = api.communicate(params, rq)
             if rs['result'] == 'success':
                 ko = rs['keys'][0]
                 if 'key' in ko:
                     if ko['type'] == 1:
-                        team_key = api.decrypt_data(ko['key'], params.data_key)
+                        team_key = api.decrypt_aes(ko['key'], params.data_key)
                     elif ko['type'] == 2:
                         team_key = api.decrypt_rsa(ko['key'], params.rsa_key)
-
-        if team_key is not None:
-            self.team_keys[team_uid] = team_key
+                    elif ko['type'] == 3:
+                        team_key = base64.urlsafe_b64decode(ko['key'] + '==')
+                if team_key is not None:
+                    team_key = team_key[:32]
+                    self.team_keys[team_uid] = team_key
         return team_key
 
     @staticmethod
     def get_enterprise_id(params):
         rq = {
             'command': 'enterprise_allocate_ids',
             'number_requested': 1
@@ -401,41 +267,14 @@
         path = ''
         node = nodes.get(node_id)
         while node:
             path = '{0}{1}{2}'.format(node[0], '\\' if path else '', path)
             node = nodes.get(node[1])
         return path
 
-    @staticmethod
-    def resolve_nodes(params, name):   # type (KeeperParams, str) -> collections.Iterable[dict]
-        node_id = 0
-        node_name = ''
-        if name:
-            node_name = str(name).lower()
-            try:
-                node_id = int(name)
-            except ValueError:
-                pass
-
-        for node in params.enterprise['nodes']:
-            if node_id > 0:
-                if node['node_id'] == node_id:
-                    yield node
-                    continue
-            if node_name:
-                if 'parent_id' in node:
-                    display_name = node['data'].get('displayname') or ''
-                else:
-                    display_name = params.enterprise['enterprise_name'] or ''
-                if display_name and display_name.lower() == node_name:
-                    yield node
-            else:
-                if 'parent_id' not in node:
-                    yield node
-
 
 class EnterpriseInfoCommand(EnterpriseCommand):
     def get_parser(self):
         return enterprise_info_parser
 
     def execute(self, params, **kwargs):
 
@@ -477,16 +316,14 @@
 
             nodes[node_id] = {
                 'node_id': node_id,
                 'parent_id': node.get('parent_id') or 0,
                 'name': node['data'].get('displayname') or '',
                 'users': [],
                 'teams': [],
-                'queued_teams': [],
-                'roles': [],
                 'children': []
             }
         for node in nodes:
             parent_id = nodes[node]['parent_id']
             if parent_id in nodes:
                 nodes[parent_id]['children'].append(node)
 
@@ -497,15 +334,15 @@
                 if node_id not in node_scope:
                     continue
 
                 user_id = user['enterprise_user_id']
                 u = {
                     'id': user_id,
                     'node_id': node_id,
-                    'username': user['username'] if 'username' in user else '[none]',
+                    'username': user['username'],
                     'name': user['data'].get('displayname') or '',
                     'status': user['status'],
                     'lock': user['lock']
                 }
                 if 'account_share_expiration' in user:
                     u['account_share_expiration'] = user['account_share_expiration']
                 users[user_id] = u
@@ -532,67 +369,28 @@
                     nodes[node_id]['teams'].append(team_id)
 
         if 'team_users' in params.enterprise:
             for tu in params.enterprise['team_users']:
                 if tu['team_uid'] in teams:
                     teams[tu['team_uid']]['users'].append(tu['enterprise_user_id'])
 
-        queued_teams = {}
-        if 'queued_teams' in params.enterprise:
-            for queued_team in params.enterprise['queued_teams']:
-                node_id = queued_team['node_id']
-                if node_id not in node_scope:
-                    continue
-                team_id = queued_team['team_uid']
-                queued_teams[team_id] = {
-                    'id': team_id,
-                    'node_id': node_id,
-                    'name': queued_team['name'],
-                    'users': []
-                }
-                if node_id in nodes:
-                    nodes[node_id]['queued_teams'].append(team_id)
-
-        if 'queued_team_users' in params.enterprise:
-            for tu in params.enterprise['queued_team_users']:
-                if tu['team_uid'] in queued_teams:
-                    queued_teams[tu['team_uid']]['users'].extend(tu['users'])
-                elif tu['team_uid'] in teams:
-                    teams[tu['team_uid']]['users'].extend(tu['users'])
-
         roles = {}
         if 'roles' in params.enterprise:
             for role in params.enterprise['roles']:
                 node_id = role['node_id']
                 if node_id not in node_scope:
                     continue
                 role_id = role['role_id']
                 roles[role_id] = {
                     'id': role_id,
                     'node_id': node_id,
                     'name': role['data'].get('displayname') or '',
                     'visible_below': role['visible_below'],
-                    'new_user_inherit': role['new_user_inherit'],
-                    'is_admin': False,
-                    'users': []
+                    'new_user_inherit': role['new_user_inherit']
                 }
-                if node_id in nodes:
-                    nodes[node_id]['roles'].append(role_id)
-
-        if 'role_users' in params.enterprise:
-            for ru in params.enterprise['role_users']:
-                role_id = ru['role_id']
-                if role_id in roles:
-                    roles[role_id]['users'].append(ru['enterprise_user_id'])
-
-        if 'managed_nodes' in params.enterprise:
-            for mn in params.enterprise['managed_nodes']:
-                role_id = mn['role_id']
-                if role_id in roles:
-                    roles[role_id]['is_admin'] = True
 
         show_users = kwargs.get('users') or False
         show_teams = kwargs.get('teams') or False
         show_roles = kwargs.get('roles') or False
 
         def node_path(node_id):
             path = ''
@@ -604,20 +402,14 @@
                 path = name + path
                 if n['parent_id']:
                     n = nodes.get(n['parent_id'])
                 else:
                     n = None
             return path
 
-        def user_email(user_id):
-            if user_id in users:
-                return users[user_id]['username']
-            else:
-                return str(user_id)
-
         def restricts(team):
             rs = ''
             rs += 'R ' if team['restrict_view'] else '  '
             rs += 'W ' if team['restrict_edit'] else '  '
             rs += 'S' if team['restrict_sharing'] else ' '
             return rs
 
@@ -630,66 +422,33 @@
                     name = ch['name']
                     if kwargs.get('verbose'):
                         name += ' ({0})'.format(ch['node_id'])
                     n['[{0}]'.format(name)] = tree_node(ch)
 
                 if len(node['users']) > 0:
                     if kwargs.get('verbose'):
-                        logging.debug('users: %s' % json.dumps(users, indent=4, sort_keys=True))
                         us = [users[x] for x in node['users']]
-                        us.sort(key=lambda x: x['username'] if 'username' in x else 'a')
+                        us.sort(key=lambda x: x['username'])
                         ud = OD()
                         for u in us:
-                            ud['{0} ({1})'.format(u['username'] if 'username' in u else '[none]', u['id'])] = {}
+                            ud['{0} ({1})'.format(u['username'], u['id'])] = {}
                         n['User(s)'] = ud
                     else:
                         n['{0} user(s)'.format(len(node['users']))] = {}
 
-                if len(node['roles']) > 0:
-                    if kwargs.get('verbose'):
-                        ts = [roles[x] for x in node['roles']]
-                        ts.sort(key=lambda x: x['name'])
-                        td = OD()
-                        for i, t in enumerate(ts):
-                            td['{0} ({1})'.format(t['name'], t['id'])] = {}
-                            if i >= 50:
-                                td['{0} More Role(s)'.format(len(ts)-i)] = {}
-                                break
-                        n['Role(s)'] = td
-                    else:
-                        n['{0} role(s)'.format(len(node['roles']))] = {}
-
                 if len(node['teams']) > 0:
                     if kwargs.get('verbose'):
                         ts = [teams[x] for x in node['teams']]
                         ts.sort(key=lambda x: x['name'])
                         td = OD()
-                        for i, t in enumerate(ts):
+                        for t in ts:
                             td['{0} ({1})'.format(t['name'], t['id'])] = {}
-                            if i >= 50:
-                                td['{0} More Team(s)'.format(len(ts)-i)] = {}
-                                break
                         n['Teams(s)'] = td
                     else:
                         n['{0} team(s)'.format(len(node['teams']))] = {}
-
-                if len(node['queued_teams']) > 0:
-                    if kwargs.get('verbose'):
-                        ts = [queued_teams[x] for x in node['queued_teams']]
-                        ts.sort(key=lambda x: x['name'])
-                        td = OD()
-                        for i, t in enumerate(ts):
-                            td['{0} ({1})'.format(t['name'], t['id'])] = {}
-                            if i >= 50:
-                                td['{0} More Queued Team(s)'.format(len(ts)-i)] = {}
-                                break
-                        n['Queued Teams(s)'] = td
-                    else:
-                        n['{0} queued team(s)'.format(len(node['queued_teams']))] = {}
-
                 return n
 
             r = nodes[root_node]
             root_name = r['name']
             if not r['parent_id'] and root_name == '':
                 root_name = params.enterprise['enterprise_name']
                 if kwargs.get('verbose'):
@@ -697,162 +456,50 @@
             tree = {
                 '[{0}]'.format(root_name): tree_node(r)
             }
             tr = LeftAligned()
             print('')
             print(tr(tree))
         else:
-            columns = set()
-            if kwargs.get('columns'):
-                columns.update(kwargs.get('columns').split(','))
-            pattern = (kwargs.get('pattern') or '').lower()
             if show_users:
-                supported_columns = SUPPORTED_USER_COLUMNS
-                if len(columns) == 0:
-                    columns.update(('name', 'status', 'transfer_status', 'node'))
-                else:
-                    wc = columns.difference(supported_columns)
-                    if len(wc) > 0:
-                        logging.warning('\n\nSupported user columns: %s\n', ', '.join(supported_columns))
-
-                displayed_columns = [x for x in supported_columns if x in columns]
                 rows = []
                 for u in users.values():
-
-                    user_status_dict = get_user_status_dict(u)
-
-                    user_id = u['id']
-                    row = [user_id, u['username']]
-                    for column in displayed_columns:
-                        if column == 'name':
-                            row.append(u['name'])
-                        elif column == 'status':
-                            row.append(user_status_dict['acct_status'])
-                        elif column == 'transfer_status':
-                            row.append(user_status_dict['acct_transfer_status'])
-                        elif column == 'node':
-                            row.append(node_path(u['node_id']))
-                        elif column == 'team_count':
-                            row.append(len([1 for t in teams.values() if t['users'] and user_id in t['users']]))
-                        elif column == 'teams':
-                            team_names = [t['name'] for t in teams.values() if t['users'] and user_id in t['users']]
-                            row.append(team_names)
-                        elif column == 'role_count':
-                            row.append(len([1 for r in roles.values() if r['users'] and user_id in r['users']]))
-                        elif column == 'roles':
-                            role_names = [r['name'] for r in roles.values() if r['users'] and user_id in r['users']]
-                            row.append(role_names)
-
-                    if pattern:
-                        if not any(1 for x in row if x and str(x).lower().find(pattern) >= 0):
-                            continue
-                    rows.append(row)
+                    status = lock_text(u['lock'])
+                    if not status:
+                        if 'account_share_expiration' in u:
+                            expire_at = datetime.datetime.fromtimestamp(u['account_share_expiration']/1000.0)
+                            if expire_at < datetime.datetime.now():
+                                status = 'Blocked'
+                            else:
+                                status = 'Transfer Acceptance'
+                        else:
+                            status = u['status'].capitalize()
+                    rows.append([u['id'], u['username'], u['name'], status, node_path(u['node_id'])])
                 rows.sort(key=lambda x: x[1])
 
                 print('')
-                headers = ['user_id', 'email']
-                headers.extend(displayed_columns)
-                if kwargs.get('format') != 'json':
-                    headers = [string.capwords(x.replace('_', ' ')) for x in headers]
-                dump_report_data(rows, headers, fmt=kwargs.get('format'), filename=kwargs.get('output'))
+                print(tabulate(rows, headers=["User ID", 'Email', 'Name', 'Status', 'Node']))
 
             if show_teams:
-                supported_columns = SUPPORTED_TEAM_COLUMNS
-                if len(columns) == 0:
-                    columns.update(('restricts', 'node', 'user_count'))
-                else:
-                    wc = columns.difference(supported_columns)
-                    if len(wc) > 0:
-                        logging.warning('\n\nSupported team columns: %s\n', ', '.join(supported_columns))
-
-                displayed_columns = [x for x in supported_columns if x in columns]
                 rows = []
                 for t in teams.values():
-                    row = [t['id'], t['name']]
-                    for column in displayed_columns:
-                        if column == 'restricts':
-                            row.append(restricts(t))
-                        elif column == 'node':
-                            row.append(node_path(t['node_id']))
-                        elif column == 'user_count':
-                            row.append(len(t['users']))
-                        elif column == 'users':
-                            row.append([user_email(x) for x in t['users']])
-                    if pattern:
-                        if not any(1 for x in row if x and str(x).lower().find(pattern) >= 0):
-                            continue
-                    rows.append(row)
-
-                for t in queued_teams.values():
-                    row = [t['id'], t['name']]
-
-                    for column in displayed_columns:
-                        if column == 'restricts':
-                            row.append('Queued')
-                        elif column == 'node':
-                            row.append(node_path(t['node_id']))
-                        elif column == 'user_count':
-                            row.append(len(t['users']))
-                        elif column == 'users':
-                            row.append([user_email(x) for x in t['users']])
-                    if pattern:
-                        if not any(1 for x in row if x and str(x).lower().find(pattern) >= 0):
-                            continue
-                    rows.append(row)
-
+                    rows.append([t['id'], t['name'], restricts(t), node_path(t['node_id'])])
                 rows.sort(key=lambda x: x[1])
 
                 print('')
-                headers = ['team_uid', 'name']
-                headers.extend(displayed_columns)
-                if kwargs.get('format') != 'json':
-                    headers = [string.capwords(x.replace('_', ' ')) for x in headers]
-                dump_report_data(rows, headers, fmt=kwargs.get('format'), filename=kwargs.get('output'))
+                print(tabulate(rows, headers=["Team ID", 'Name', 'Restricts', 'Node']))
 
             if show_roles:
-                supported_columns = SUPPORTED_TEAM_COLUMNS
-                if len(columns) == 0:
-                    columns.update(('is_visible_below', 'is_new_user', 'is_admin','node', 'user_count'))
-                else:
-                    wc = columns.difference(supported_columns)
-                    if len(wc) > 0:
-                        logging.warning('\n\nSupported team columns: %s\n', ', '.join(supported_columns))
-
-                displayed_columns = [x for x in supported_columns if x in columns]
-
                 rows = []
                 for r in roles.values():
-                    row = [r['id'], r['name']]
-                    for column in displayed_columns:
-                        if column == 'is_visible_below':
-                            row.append('Y' if r['visible_below'] else '')
-                        elif column == 'is_new_user':
-                            row.append('Y' if r['new_user_inherit'] else '')
-                        elif column == 'is_admin':
-                            row.append('Y' if r['is_admin'] else '')
-                        elif column == 'node':
-                            row.append(node_path(r['node_id']))
-                        elif column == 'user_count':
-                            row.append(len(r['users']))
-                        elif column == 'users':
-                            row.append([user_email(x) for x in r['users']])
-                    if pattern:
-                        if not any(1 for x in row if x and str(x).lower().find(pattern) >= 0):
-                            continue
-                    rows.append(row)
-
+                    rows.append([r['id'], r['name'], 'Y' if r['visible_below'] else '', 'Y' if r['new_user_inherit'] else '', node_path(r['node_id'])])
                 rows.sort(key=lambda x: x[1])
 
                 print('')
-
-                headers = ['role_id', 'name']
-                headers.extend(displayed_columns)
-                if kwargs.get('format') != 'json':
-                    headers = [string.capwords(x.replace('_', ' ')) for x in headers]
-                dump_report_data(rows, headers, fmt=kwargs.get('format'), filename=kwargs.get('output'))
+                print(tabulate(rows, headers=["Role ID", 'Name', 'Cascade?', 'New User?', 'Node']))
 
         print('')
 
 
 class EnterpriseNodeCommand(EnterpriseCommand):
     def get_parser(self):
         return enterprise_node_parser
@@ -864,1131 +511,550 @@
             for node in params.enterprise['nodes']:
                 parent_id = node.get('parent_id')
                 if parent_id == node_id:
                     nodes.append(node['node_id'])
             EnterpriseNodeCommand.get_subnodes(params, nodes, index + 1)
 
     def execute(self, params, **kwargs):
-        if kwargs.get('delete') and kwargs.get('add'):
-            raise CommandError('enterprise-node', "'add' and 'delete' parameters are mutually exclusive.")
-
-        node_lookup = {}
-        if 'nodes' in params.enterprise:
-            for node in params.enterprise['nodes']:
-                node_lookup[str(node['node_id'])] = node
-                node_name = node['data'].get('displayname') or ''
-                if not node_name and 'parent_id' not in node:
-                    node_name = params.enterprise['enterprise_name']
-                if node_name:
-                    node_name = node_name.lower()
-                    n = node_lookup.get(node_name)
-                    if n is None:
-                        node_lookup[node_name] = node
-                    elif type(n) == list:
-                        n.append(node)
-                    else:
-                        node_lookup[node_name] = [n, node]
-
-        parent_id = None
-        if kwargs.get('parent'):
-            parent_name = kwargs.get('parent')
-            n = node_lookup.get(parent_name)
-            if not n:
-                n = node_lookup.get(parent_name.lower())
-            if n:
-                if type(n) == list:
-                    raise CommandError('enterprise-node', 'Parent node %s in not unique'.format(parent_name))
-                parent_id = n['node_id']
-            else:
-                raise CommandError('enterprise-node', 'Cannot resolve parent node %s'.format(parent_name))
+        node_name = kwargs['node']
+        node_id = None
+        for node in params.enterprise['nodes']:
+            if node_name in {str(node['node_id']), node['data'].get('displayname')}:
+                node_id = node['node_id']
+                break
+            elif not node.get('parent_id') and node_name == params.enterprise['enterprise_name']:
+                node_id = node['node_id']
+                break
+        if not node_id:
+            logging.error('Node %s is not found.', node_name)
+            return
 
-        matched = {}
-        unmatched_nodes = set()
+        node = [x for x in params.enterprise['nodes'] if x['node_id'] == node_id][0]
+        if not node.get('parent_id'):
+            logging.error('Cannot wipe out root node')
+            return
 
-        for node_name in kwargs['node']:
-            n = node_lookup.get(node_name)
-            if not n:
-                n = node_lookup.get(node_name.lower())
-            if n:
-                if type(n) == list:
-                    logging.warning('Node name \'%s\' is not unique. Skipping.', node_name)
-                else:
-                    matched[n['node_id']] = n
-            else:
-                unmatched_nodes.add(node_name)
+        answer = user_choice(
+            bcolors.FAIL + bcolors.BOLD + '\nALERT!\n' + bcolors.ENDC +
+            'This action cannot be undone.\n\n' +
+            'Do you want to proceed with deletion?', 'yn', 'n')
+        if answer.lower() != 'y':
+            return
 
-        matched_nodes = list(matched.values())
+        sub_nodes = [node['node_id']]
+        EnterpriseNodeCommand.get_subnodes(params, sub_nodes, 0)
 
-        request_batch = []
-        if kwargs.get('add'):
-            for node in matched_nodes:
-                logging.warning('Node \'%s\' already exists: Skipping.', node['data'].get('displayname'))
+        nodes = set(sub_nodes)
 
-            if not unmatched_nodes:
-                raise CommandError('enterprise-node', 'No nodes to add.')
-
-            if parent_id is None:
-                for node in params.enterprise['nodes']:
-                    if not node.get('parent_id'):
-                        parent_id = node['node_id']
-                        break
+        commands = []
 
-            for node_name in unmatched_nodes:
-                dt = {'displayname': node_name}
-                encrypted_data = api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key'])
+        if 'queued_teams' in params.enterprise:
+            queued_teams = [x for x in params.enterprise['queued_teams'] if x['node_id'] in nodes]
+            for qt in queued_teams:
                 rq = {
-                    'command': 'node_add',
-                    'node_id': self.get_enterprise_id(params),
-                    'parent_id': parent_id,
-                    'encrypted_data': encrypted_data
+                    'command': 'team_delete',
+                    'team_uid': qt['team_uid']
                 }
-                request_batch.append(rq)
-        elif kwargs.get('toggle_isolated'):
-            if not matched_nodes:
-                raise CommandError('enterprise-node', 'No nodes to toggle.')
-
-            for mn in matched_nodes:
-                node_id = mn['node_id']
-                data = mn['data']
-                displayname = data['displayname']
-                request = SetRestrictVisibilityRequest()
-                request.nodeId = node_id
-                api_request_payload = proto.ApiRequestPayload()
-                api_request_payload.payload = request.SerializeToString()
-                api_request_payload.encryptedSessionToken = base64.urlsafe_b64decode(params.session_token + '==')
-                rs = rest_api.execute_rest(params.rest_context, 'enterprise/set_restrict_visibility', api_request_payload)
-                # FIXME: Should this error checking/reporting be in a reusuble callable instead?
-                if rs == b'':
-                    print('good result: {}'.format(displayname))
-                elif isinstance(rs, dict):
-                    if 'error' in rs:
-                        print('bad result: {}:'.format(displayname))
-                        print('error: {}'.format(rs['error']))
-                        if 'additional_info' in rs:
-                            print('additional_info: {}'.format(rs['additional_info']))
-                else:
-                    print('Unexpected result: ', rs)
-                continue
-        else:
-            for node_name in unmatched_nodes:
-                logging.warning('Node \'%s\' is not found: Skipping', node_name)
-
-            if not matched_nodes:
-                return
+                commands.append(rq)
 
-            if kwargs.get('delete'):
-                depths = {}
-
-                def traverse_to_root(node_id, depth):
-                    if not node_id:
-                        return depth
-                    nd = node_lookup.get(str(node_id))
-                    if nd:
-                        return traverse_to_root(nd.get('parent_id'), depth + 1)
-                    else:
-                        return depth
-
-                for node in matched_nodes:
-                    depths[node['node_id']] = traverse_to_root(node['node_id'], 0)
-                matched_nodes.sort(key=lambda x: depths[x['node_id']] or 0, reverse=True)
-                for node in matched_nodes:
-                    rq = {
-                        'command': 'node_delete',
-                        'node_id': node['node_id']
-                    }
-                    request_batch.append(rq)
-            elif kwargs.get('wipe_out'):
-                if len(matched_nodes) != 1:
-                    raise CommandError('enterprise-node', 'Cannot wipe-out more than one node')
-                node = matched_nodes[0]
-                if not node.get('parent_id'):
-                    raise CommandError('enterprise-node', 'Cannot wipe out root node')
-
-                answer = user_choice(
-                    bcolors.FAIL + bcolors.BOLD + '\nALERT!\n' + bcolors.ENDC +
-                    'This action cannot be undone.\n\n' +
-                    'Do you want to proceed with deletion?', 'yn', 'n')
-                if answer.lower() != 'y':
-                    return
-
-                sub_nodes = [node['node_id']]
-                EnterpriseNodeCommand.get_subnodes(params, sub_nodes, 0)
-                nodes = set(sub_nodes)
-
-                if 'queued_teams' in params.enterprise:
-                    queued_teams = [x for x in params.enterprise['queued_teams'] if x['node_id'] in nodes]
-                    for qt in queued_teams:
-                        rq = {
-                            'command': 'team_delete',
-                            'team_uid': qt['team_uid']
-                        }
-                        request_batch.append(rq)
-
-                managed_nodes = [x for x in params.enterprise['managed_nodes'] if x['managed_node_id'] in nodes]
-                roles = [x for x in params.enterprise['roles'] if x['node_id'] in nodes]
-                role_set = set([x['role_id'] for x in managed_nodes])
-                role_set = role_set.union([x['role_id'] for x in roles])
-                for ru in params.enterprise['role_users']:
-                    if ru['role_id'] in role_set:
-                        rq = {
-                            'command': 'role_user_remove',
-                            'role_id': ru['role_id'],
-                            'enterprise_user_id': ru['enterprise_user_id']
-                        }
-                        request_batch.append(rq)
-                for mn in managed_nodes:
-                    rq = {
-                        'command': 'role_managed_node_remove',
-                        'role_id': mn['role_id'],
-                        'managed_node_id': mn['managed_node_id']
-                    }
-                    request_batch.append(rq)
-                for r in roles:
-                    rq = {
-                        'command': 'role_delete',
-                        'role_id': r['role_id']
-                    }
-                    request_batch.append(rq)
-
-                users = [x for x in params.enterprise['users'] if x['node_id'] in nodes]
-                for u in users:
-                    rq = {
-                        'command': 'enterprise_user_delete',
-                        'enterprise_user_id': u['enterprise_user_id']
-                    }
-                    request_batch.append(rq)
+        managed_nodes = [x for x in params.enterprise['managed_nodes'] if x['managed_node_id'] in nodes]
+        roles = [x for x in params.enterprise['roles'] if x['node_id'] in nodes]
+        role_set = set([x['role_id'] for x in managed_nodes])
+        role_set = role_set.union([x['role_id'] for x in roles])
+        for ru in params.enterprise['role_users']:
+            if ru['role_id'] in role_set:
+                rq = {
+                    'command': 'role_user_remove',
+                    'role_id': ru['role_id'],
+                    'enterprise_user_id': ru['enterprise_user_id']
+                }
+                commands.append(rq)
+        for mn in managed_nodes:
+            rq = {
+                'command': 'role_managed_node_remove',
+                'role_id': mn['role_id'],
+                'managed_node_id': mn['managed_node_id']
+            }
+            commands.append(rq)
+        for r in roles:
+            rq = {
+                'command': 'role_delete',
+                'role_id': r['role_id']
+            }
+            commands.append(rq)
+        users = [x for x in params.enterprise['users'] if x['node_id'] in nodes]
+        for u in users:
+            rq = {
+                'command': 'enterprise_user_delete',
+                'enterprise_user_id': u['enterprise_user_id']
+            }
+            commands.append(rq)
 
-                if 'teams' in params.enterprise:
-                    teams = [x for x in params.enterprise['teams'] if x['node_id'] in nodes]
-                    for t in teams:
-                        rq = {
-                            'command': 'team_delete',
-                            'team_uid': t['team_uid']
-                        }
-                        request_batch.append(rq)
+        teams = [x for x in params.enterprise['teams'] if x['node_id'] in nodes]
+        for t in teams:
+            rq = {
+                'command': 'team_delete',
+                'team_uid': t['team_uid']
+            }
+            commands.append(rq)
 
-                sub_nodes.pop(0)
-                sub_nodes.reverse()
-                for node_id in sub_nodes:
-                    rq = {
-                        'command': 'node_delete',
-                        'node_id': node_id
-                    }
-                    request_batch.append(rq)
-            elif parent_id or kwargs.get('name'):
+        sub_nodes.pop(0)
+        sub_nodes.reverse()
+        for node_id in sub_nodes:
+            rq = {
+                'command': 'node_delete',
+                'node_id': node_id
+            }
+            commands.append(rq)
 
-                def is_in_chain(node_id, parent_id):
-                    if node_id == parent_id:
-                        return True
-                    nn = node_lookup.get(node_id)
-                    if not nn:
-                        return False
-                    return is_in_chain(nn['parent_id'], parent_id)
-
-                if kwargs.get('name') and len(matched_nodes) > 1:
-                    logging.warning('Cannot assign the same name to % nodes', len(matched_nodes) > 1)
-                    kwargs['name'] = None
-                if not parent_id or not kwargs.get('name'):
-                    for node in matched_nodes:
-                        encrypted_data = node['encrypted_data']
-                        if kwargs.get('name'):
-                            dt = node['data']
-                            dt['dsplayname'] = kwargs.get('name')
-                            encrypted_data = api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key'])
-                        if parent_id:
-                            if is_in_chain(parent_id, node['node_id']):
-                                logging.warning('Cannot move node to itself or its children')
-                                continue
-                        rq = {
-                            'command': 'node_update',
-                            'encrypted_data': encrypted_data
-                        }
-                        if parent_id:
-                            rq['parent_id'] = parent_id
-                        request_batch.append(rq)
-
-        if request_batch:
-            rss = api.execute_batch(params, request_batch)
-            for rq, rs in zip(request_batch, rss):
-                command = rq.get('command')
-                if command == 'node_add':
-                    if rs['result'] == 'success':
-                        logging.info('Node is created')
-                    else:
-                        logging.warning('Failed to create node: %s', rs['message'])
-                elif command in {'node_delete', 'node_update'}:
-                    node_id = rq['node_id']
-                    node_name = str(node_id)
-                    node = node_lookup.get(node_name)
-                    if node:
-                        node_name = node['data'].get('displayname') or node_name
-                    verb = 'deleted' if command == 'node_delete' else 'updated'
-                    if rs['result'] == 'success':
-                        logging.info('\'%s\' node is %s', node_name, verb)
-                    else:
-                        logging.warning('\'%s\' node is not %s. Error: %s', node_name, verb, rs['message'])
-                else:
-                    if rs['result'] != 'success':
-                        raise CommandError('enterprise-node', '\'{0}\' command error: {1}'.format(command,  rs['message']))
-            api.query_enterprise(params)
+        api.execute_batch(params, commands)
+        api.query_enterprise(params)
 
 
 class EnterpriseUserCommand(EnterpriseCommand):
     def get_parser(self):
         return enterprise_user_parser
 
     def execute(self, params, **kwargs):
-        if kwargs.get('delete') and kwargs.get('add'):
-            raise CommandError('enterprise-user', "'add' and 'delete' parameters are mutually exclusive.")
-
-        if kwargs.get('lock') and kwargs.get('unlock'):
-            raise CommandError('enterprise-user', "'lock' and 'unlock' parameters are mutually exclusive.")
-
+        user = None
         matched_users = []
-        unmatched_emails = set()
-
-        user_lookup = {}
+        email = kwargs['email']
         if 'users' in params.enterprise:
             for u in params.enterprise['users']:
-                user_lookup[str(u['enterprise_user_id'])] = u
-
-                if 'username' in u:
-                    user_lookup[u['username'].lower()] = u
-                else:
-                    logging.debug('All users: %s' % params.enterprise['users'])
-                    logging.debug('WARNING: username is missing from the user id=%s, obj=%s' % (u['enterprise_user_id'], u))
+                if email in {str(u['enterprise_user_id']), u['username']}:
+                    user = u
+                    break
 
-        emails = kwargs['email']
-        if emails:
-            for email in emails:
-                email = email.lower()
-                if email in user_lookup:
-                    matched_users.append(user_lookup[email])
-                else:
-                    unmatched_emails.add(email)
+        if not user:
+            regex = re.compile(fnmatch.translate(email)).match
+            if 'users' in params.enterprise:
+                for u in params.enterprise['users']:
+                    if regex(u['username']):
+                        matched_users.append(u)
 
         node_id = None
         if kwargs.get('node'):
             for node in params.enterprise['nodes']:
                 if kwargs['node'] in {str(node['node_id']), node['data'].get('displayname')}:
                     node_id = node['node_id']
                     break
                 elif not node.get('parent_id') and kwargs['node'] == params.enterprise['enterprise_name']:
                     node_id = node['node_id']
                     break
 
         user_name = kwargs.get('displayname')
 
-        request_batch = []
-        disable_2fa_users = []
-
-        if kwargs.get('add'):
-            for user in matched_users:
-                logging.warning('User %s already exists: Skipping', user['username'])
-
-            if not unmatched_emails:
-                raise CommandError('enterprise-user', 'No email address to add.')
+        if kwargs.get('delete'):
+            if user:
+                answer = 'y' if kwargs.get('force') else \
+                    user_choice(
+                        bcolors.FAIL + bcolors.BOLD + '\nALERT!\n' + bcolors.ENDC +
+                        'Deleting a user will also delete any records owned and shared by this user.\n'+
+                        'Before you delete this user(s), we strongly recommend you lock their account\n' +
+                        'and transfer any important records to other user(s).\n' +
+                        'This action cannot be undone.\n\n' +
+                        'Do you want to proceed with deletion?', 'yn', 'n')
+                if answer.lower() == 'y':
+                    rq = {
+                        'command': 'enterprise_user_delete',
+                        'enterprise_user_id': user['enterprise_user_id']
+                    }
+                    rs = api.communicate(params, rq)
+                    if rs['result'] == 'success':
+                        logging.info('User %s is deleted', user['username'])
+                        api.query_enterprise(params)
+            else:
+                logging.warning('No such user')
+            return
 
+        elif kwargs.get('add'):
             dt = {}
             if user_name:
                 dt['displayname'] = user_name
-            encrypted_data = api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key'])
             if node_id is None:
                 for node in params.enterprise['nodes']:
                     if not node.get('parent_id'):
                         node_id = node['node_id']
                         break
+            rq = {
+                'command': 'enterprise_user_add',
+                'enterprise_user_id': self.get_enterprise_id(params),
+                'node_id': node_id,
+                'encrypted_data': api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key']),
+                'enterprise_user_username': email
+            }
+            rs = api.communicate(params, rq)
+            if rs['result'] == 'success':
+                logging.info('User %s is added', email)
+                api.query_enterprise(params)
+            return
 
-            for email in unmatched_emails:
+        if user:
+            if kwargs.get('lock') or kwargs.get('unlock'):
+                is_locked = user['lock'] != 0
+                to_lock = kwargs.get('lock')
+                if kwargs.get('lock') or kwargs.get('unlock'):
+                    to_lock = not is_locked
                 rq = {
-                    'command': 'enterprise_user_add',
-                    'enterprise_user_id': self.get_enterprise_id(params),
-                    'node_id': node_id,
-                    'encrypted_data': encrypted_data,
-                    'enterprise_user_username': email
+                    'command': 'enterprise_user_lock',
+                    'enterprise_user_id': user['enterprise_user_id'],
+                    'lock': 'locked' if to_lock else 'unlocked'
                 }
-                request_batch.append(rq)
-        else:
-            for email in unmatched_emails:
-                logging.warning('User %s is not found: Skipping', email)
-
-            if not matched_users:
-                raise CommandError('enterprise-user', 'No such user(s)')
+                rs = api.communicate(params, rq)
+                if rs['result'] == 'success':
+                    user['lock'] = 1 if to_lock else 0
+                    logging.info('User %s is %s', user['username'], 'locked' if to_lock else 'unlocked')
 
-            if kwargs.get('delete'):
-                answer = 'y' if kwargs.get('force') else \
+            elif kwargs.get('expire'):
+                answer = 'y' if  kwargs.get('force') else \
                     user_choice(
-                        bcolors.FAIL + bcolors.BOLD + '\nALERT!\n' + bcolors.ENDC +
-                        'Deleting a user will also delete any records owned and shared by this user.\n'+
-                        'Before you delete this user(s), we strongly recommend you lock their account\n' +
-                        'and transfer any important records to other user(s).\n' +
-                        'This action cannot be undone.\n\n' +
-                        'Do you want to proceed with deletion?', 'yn', 'n')
+                        bcolors.BOLD + '\nConfirm\n' + bcolors.ENDC +
+                        'User will be required to create a new Master Password on the next login.\n' +
+                        'Are you sure you want to expire master password?', 'yn', 'n')
                 if answer.lower() == 'y':
-                    for user in matched_users:
+                    rq = {
+                        'command': 'set_master_password_expire',
+                        'email': user['username']
+                    }
+                    rs = api.communicate(params, rq)
+                    if rs['result'] == 'success':
+                        logging.info('User %s has master password expired', user['username'])
+
+            elif kwargs.get('add_role') or kwargs.get('remove_role'):
+                roles = {}
+                for is_add in [False, True]:
+                    l = kwargs.get('add_role') if is_add else kwargs.get('remove_role')
+                    if l:
+                        for r in l:
+                            role_node = None
+                            if 'roles' in params.enterprise:
+                                for role in params.enterprise['roles']:
+                                    if r in {str(role['role_id']), role['data'].get('displayname')}:
+                                        role_node = role
+                                        break
+                            if role_node:
+                                roles[role_node['role_id']] = is_add, role_node['data'].get('displayname')
+                            else:
+                                logging.warning('Role %s cannot be resolved', r)
+                if len(roles) > 0:
+                    admin_confirmed = False
+                    for role_id in roles:
+                        is_add, role_name = roles[role_id]
                         rq = {
-                            'command': 'enterprise_user_delete',
-                            'enterprise_user_id': user['enterprise_user_id']
+                            'command': 'role_user_add' if is_add else 'role_user_remove',
+                            'enterprise_user_id': user['enterprise_user_id'],
+                            'role_id': role_id
                         }
-                        request_batch.append(rq)
-            else:
-                if kwargs.get('lock') or kwargs.get('unlock'):
-                    for user in matched_users:
-                        if user['status'] == 'active':
-                            to_lock = kwargs.get('lock')
-                            request_batch.append({
-                                'command': 'enterprise_user_lock',
-                                'enterprise_user_id': user['enterprise_user_id'],
-                                'lock': 'locked' if to_lock else 'unlocked'
-                            })
-                        else:
-                            logging.warning('%s has not accepted invitation yet: Skipping', user['username'])
-
-                if kwargs.get('disable_2fa'):
-                    for user in matched_users:
-                        if user['status'] == 'active':
-                            disable_2fa_users.append(user)
-                        else:
-                            logging.warning('%s has not accepted invitation yet: Skipping', user['username'])
-
-                if kwargs.get('expire'):
-                    answer = 'y' if  kwargs.get('force') else \
-                        user_choice(
-                            bcolors.BOLD + '\nConfirm\n' + bcolors.ENDC +
-                            'User will be required to create a new Master Password on the next login.\n' +
-                            'Are you sure you want to expire master password?', 'yn', 'n')
-                    if answer.lower() == 'y':
-                        for user in matched_users:
-                            request_batch.append({
-                                'command': 'set_master_password_expire',
-                                'email': user['username']
-                            })
-
-                if kwargs.get('extend'):
-                    for user in matched_users:
-                        request_batch.append({
-                            'command': 'extend_account_share_expiration',
-                            'enterprise_user_id': user['enterprise_user_id']
-                        })
-
-                if kwargs.get('add_role') or kwargs.get('remove_role'):
-                    role_changes = {}
-                    for is_add in [False, True]:
-                        l = kwargs.get('add_role') if is_add else kwargs.get('remove_role')
-                        if l:
-                            for r in l:
-                                role_node = None
-                                if 'roles' in params.enterprise:
-                                    for role in params.enterprise['roles']:
-                                        if r in {str(role['role_id']), role['data'].get('displayname')}:
-                                            role_node = role
-                                            break
-                                if role_node:
-                                    role_changes[role_node['role_id']] = is_add, role_node['data'].get('displayname')
-                                else:
-                                    logging.warning('Role %s cannot be resolved', r)
-
-                    if len(role_changes) > 0:
-                        for role_id in role_changes:
-                            is_add, role_name = role_changes[role_id]
-                            role_users = set()
-                            if 'role_users' in params.enterprise:
-                                for ru in params.enterprise['role_users']:
-                                    if ru['role_id'] == role_id:
-                                        role_users.add(ru['enterprise_user_id'])
-
-                            role_key = None
-                            is_managed_role = False
-                            if is_add:
-                                if 'managed_nodes' in params.enterprise:
-                                    for mn in params.enterprise['managed_nodes']:
-                                        if mn['role_id'] == role_id:
-                                            is_managed_role = True
-                                            break
-                            if is_managed_role:
-
-                                if 'role_keys2' in params.enterprise:
-                                    for rk2 in params.enterprise['role_keys2']:
-                                        if rk2['role_id'] == role_id:
-                                            encrypted_key_decoded = base64.urlsafe_b64decode(rk2['role_key'] + '==')
-                                            role_key = rest_api.decrypt_aes(encrypted_key_decoded,
-                                                                            params.enterprise['unencrypted_tree_key'])
-                                            break
-
-                                if 'role_keys' in params.enterprise and role_key is None:
-                                    for rk in params.enterprise['role_keys']:
-                                        if rk['role_id'] == role_id:
-                                            if rk['key_type'] == 'encrypted_by_data_key':
-                                                role_key = api.decrypt_data(rk['encrypted_key'], params.data_key)
-                                            elif rk['key_type'] == 'encrypted_by_public_key':
-                                                role_key = api.decrypt_rsa(rk['encrypted_key'], params.rsa_key)
-                                            break
-
-                            user_pkeys = {}
-                            for user in matched_users:
-                                if is_add and user['enterprise_user_id'] in role_users:
-                                    logging.warning('User %s is already in \'%s\' group: Add to group is skipped', user['username'], role_name)
-                                    continue
-                                if not is_add and user['enterprise_user_id'] not in role_users:
-                                    logging.warning('User %s is not in \'%s\': Remove from group is skipped', user['username'], role_name)
-                                    continue
-
-                                user_id = user['enterprise_user_id']
-                                rq = {
-                                    'command': 'role_user_add' if is_add else 'role_user_remove',
-                                    'enterprise_user_id': user['enterprise_user_id'],
-                                    'role_id': role_id
-                                }
-                                if is_managed_role:
-                                    if user_id not in user_pkeys:
-                                        answer = 'y' if kwargs.get('force') else user_choice('Do you want to grant administrative privileges to {0}'.format(user['username']), 'yn', 'n')
-                                        public_key = None
-                                        if answer == 'y':
-                                            public_key = self.get_public_key(params, user['username'])
-                                            if public_key is None:
-                                                logging.warning('Cannot get public key for user %s', user['username'])
-                                        user_pkeys[user_id] = public_key
-                                    if user_pkeys[user_id]:
-                                        rq['tree_key'] = api.encrypt_rsa(params.enterprise['unencrypted_tree_key'], user_pkeys[user_id])
-                                        if role_key:
-                                            rq['role_admin_key'] = api.encrypt_rsa(role_key, user_pkeys[user_id])
-                                        request_batch.append(rq)
-                                else:
-                                    request_batch.append(rq)
-
-                if kwargs.get('add_team') or kwargs.get('remove_team'):
-                    teams = {}
-                    for is_add in [False, True]:
-                        tl = kwargs.get('add_team') if is_add else kwargs.get('remove_team')
-                        if tl:
-                            for t in tl:
-                                team_node = None
-                                if 'teams' in params.enterprise:
-                                    for team in params.enterprise['teams']:
-                                        if t == team['team_uid'] or t.lower() == team['name'].lower():
-                                            team_node = team
-                                            break
-                                if team_node:
-                                    team_uid = team_node['team_uid']
-                                    teams[team_uid] = is_add, team_node['name']
-                                else:
-                                    raise CommandError('enterprise-user', 'Team {0} could be resolved'.format(t))
-
-                    if teams:
-                        for team_uid in teams:
-                            is_add, team_name = teams[team_uid]
-                            for user in matched_users:
-                                if is_add:
-                                    if user['status'] == 'active':
-                                        rq = {
-                                            'command': 'team_enterprise_user_add',
-                                            'team_uid': team_uid,
-                                            'enterprise_user_id': user['enterprise_user_id'],
-                                        }
-                                        team_key = self.get_team_key(params, team_uid)
+                        need_confirm = False
+                        if is_add:
+                            if 'managed_nodes' in params.enterprise:
+                                for mn in params.enterprise['managed_nodes']:
+                                    if mn['role_id'] == role_id:
                                         public_key = self.get_public_key(params, user['username'])
-                                        if team_key and public_key:
-                                            rq['team_key'] = api.encrypt_rsa(team_key, public_key)
-                                            rq['user_type'] = 0
-                                            request_batch.append(rq)
-                                    else:
-                                        rq = {
-                                            'command': 'team_queue_user',
-                                            'team_uid': team_uid,
-                                            'enterprise_user_id': user['enterprise_user_id']
-                                        }
-                                        request_batch.append(rq)
-                                else:
-                                    rq = {
-                                        'command': 'team_enterprise_user_remove',
-                                        'enterprise_user_id': user['enterprise_user_id'],
-                                        'team_uid': team_uid
-                                    }
-                                    request_batch.append(rq)
-                if node_id:
-                    for user in matched_users:
-                        if node_id != user['node_id']:
-                            encrypted_data = user['encrypted_data']
-                            if 'key_type' in user and user['key_type'] == 'no_key':
-                                dt = {
-                                    'displayname': user['data'].get('displayname') or ''
-                                }
-                                encrypted_data = api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key'])
-                            rq = {
-                                'command': 'enterprise_user_update',
-                                'enterprise_user_id': user['enterprise_user_id'],
-                                'node_id': node_id,
-                                'encrypted_data': encrypted_data,
-                                'enterprise_user_username': user['username']
-                            }
-                            request_batch.append(rq)
-
-        if request_batch:
-            rss = api.execute_batch(params, request_batch)
-            for rq, rs in zip(request_batch, rss):
-                command = rq.get('command')
-                if command == 'enterprise_user_add':
-                    if rs['result'] == 'success':
-                        logging.info('%s user invited', rq['enterprise_user_username'])
-                    else:
-                        logging.warning('%s failed to invite user: %s', rq['enterprise_user_username'], rs['message'])
-                else:
-                    user = None
-                    if not user and 'username' in rq:
-                        user = user_lookup.get(rq['username'].lower())
-                    if not user and 'email' in rq:
-                        user = user_lookup.get(rq['email'].lower())
-                    if not user and 'enterprise_user_id' in rq:
-                        user = user_lookup.get(str(rq['enterprise_user_id']))
-                    if user:
-                        if command == 'set_master_password_expire':
-                            if rs['result'] == 'success':
-                                logging.info('%s password expired', user['username'])
-                            else:
-                                logging.warning('%s failed to expire password: %s', user['username'], rs['message'])
-                        elif command == 'extend_account_share_expiration':
-                            if rs['result'] == 'success':
-                                logging.info('%s vault transfer consent expiration extended by 7 days', user['username'])
-                            else:
-                                logging.warning('%s failed to extend vault transfer consent expiration: %s', user['username'], rs['message'])
-                        elif command == 'enterprise_user_delete':
-                            if rs['result'] == 'success':
-                                logging.info('%s user deleted', user['username'])
-                            else:
-                                logging.warning('%s failed to delete user: %s', user['username'], rs['message'])
-                        elif command == 'enterprise_user_update':
-                            node_names = [x['data'].get('displayname') for x in params.enterprise['nodes'] if x['node_id'] == rq['node_id']]
-                            node_name = node_names[0] if len(node_names) > 0 else str(rq['node_id'])
-                            if rs['result'] == 'success':
-                                logging.info('%s user moved to node \'%s\'', user['username'], node_name or 'Root')
-                            else:
-                                logging.warning('%s failed to move user to node \'%s\': %s', user['username'], node_name or 'Root', rs['message'])
-                        elif command == 'enterprise_user_lock':
-                            is_locked = rq['lock'] == 'locked'
-                            if rs['result'] == 'success':
-                                logging.info('%s is %s', user['username'], 'locked' if is_locked else 'unlocked')
-                            else:
-                                logging.warning(' %s failed to %s user: %s', user['username'], 'lock' if is_locked else 'unlock', rs['message'])
-                        elif command in {'role_user_add', 'role_user_remove'}:
-                            role_names = [x['data'].get('displayname') for x in params.enterprise['roles'] if x['role_id'] == rq['role_id']]
-                            role_name = role_names[0] if len(role_names) > 0 else str(rq['role_id'])
-                            if rs['result'] == 'success':
-                                logging.info('%s %s role \'%s\'', user['username'], 'added to' if command == 'role_user_add' else 'removed from', role_name)
+                                        if public_key is None:
+                                            logging.warning('Cannot get public key for user %s', user['username'])
+                                            return
+                                        rq['tree_key'] = api.encrypt_rsa(params.enterprise['unencrypted_tree_key'], public_key)
+                                        need_confirm = True
+                                        break
+                            if 'role_keys' in params.enterprise:
+                                for rk in params.enterprise['role_keys']:
+                                    if rk['role_id'] == role_id:
+                                        public_key = self.get_public_key(params, user['username'])
+                                        if public_key is None:
+                                            logging.warning('Cannot get public key for user %s', user['username'])
+                                            return
+                                        role_key = None
+                                        if rk['key_type'] == 'encrypted_by_data_key':
+                                            role_key = api.decrypt_aes(rk['encrypted_key'], params.data_key)
+                                        elif rk['key_type'] == 'encrypted_by_public_key':
+                                            role_key = api.decrypt_rsa(rk['encrypted_key'], params.rsa_key)
+                                        if role_key:
+                                            need_confirm = True
+                                            rq['role_admin_key'] = api.encrypt_aes(role_key, public_key)
+                                        break
+                        if need_confirm and not admin_confirmed:
+                            answer = 'y' if kwargs.get('force') else user_choice('Do you want to grant administrative privileges to {0}'.format(user['username']), 'yn', 'n')
+                            if answer == 'y':
+                                admin_confirmed = True
                             else:
-                                logging.warning('%s failed to %s role \'%s\': %s', user['username'], 'add to' if command == 'role_user_add' else 'remove from', role_name, rs['message'])
-                        elif command in {'team_enterprise_user_add', 'team_enterprise_user_remove', 'team_queue_user'}:
-                            team_names = [x['name'] for x in params.enterprise['teams'] if x['team_uid'] == rq['team_uid']]
-                            team_name = team_names[0] if len(team_names) > 0 else rq['team_uid']
-                            if rs['result'] == 'success':
-                                logging.info('%s %s team \'%s\'', user['username'], 'removed from' if command == 'team_enterprise_user_remove' else 'added to', team_name)
+                                return
+                        rs = api.communicate(params, rq)
+                        if rs['result'] == 'success':
+                            logging.info('Role %s %s %s', role_name, 'added to' if is_add else 'removed from', user['username'])
+                    api.query_enterprise(params)
+
+            elif kwargs.get('add_team') or kwargs.get('remove_team'):
+                teams = {}
+                for is_add in [False, True]:
+                    tl = kwargs.get('add_team') if is_add else kwargs.get('remove_team')
+                    if tl:
+                        for t in tl:
+                            team_node = None
+                            if 'teams' in params.enterprise:
+                                for team in params.enterprise['teams']:
+                                    if t in { team['team_uid'], team['name']}:
+                                        team_node = team
+                                        break
+                            if team_node:
+                                team_uid = team_node['team_uid']
+                                teams[team_uid] = is_add, team_node['name']
                             else:
-                                logging.warning('%s failed to %s team \'%s\': %s', user['username'], 'removed from' if command == 'team_enterprise_user_remove' else 'added to', team_name, rs['message'])
-                        else:
-                            if rs['result'] != 'success':
-                                logging.warning('\'%s\' error: %s', command, rs['message'])
-                    else:
-                        if rs['result'] != 'success':
-                            logging.warning('Error: %s', rs['message'])
-            api.query_enterprise(params)
-
-        if disable_2fa_users:
-            uids = EnterpriseUserIds()
-            for user in disable_2fa_users:
-                uids.enterpriseUserId.append(user['enterprise_user_id'])
-            api.communicate_rest(params, uids, 'enterprise/disable_two_fa')
-            users = [x['username'] for x in disable_2fa_users]
-            logging.warning("2FA successfully removed for %s", ", ".join(users))
-
-        if not request_batch and not disable_2fa_users:
-            is_verbose = kwargs.get('verbose') or False
-            print('\n')
-            for user in matched_users:
+                                logging.warning('Team %s could be resolved', t)
+                if len(teams) > 0:
+                    for team_uid in teams:
+                        is_add, team_name = teams[team_uid]
+                        rq = {
+                            'command': 'team_enterprise_user_add' if is_add else 'team_enterprise_user_remove',
+                            'enterprise_user_id': user['enterprise_user_id'],
+                            'team_uid': team_uid
+                        }
+                        if is_add:
+                            team_key = self.get_team_key(params, team_uid)
+                            public_key = self.get_public_key(params, user['username'])
+                            if team_key and public_key:
+                                rq['team_key'] = api.encrypt_rsa(team_key, public_key)
+                                rq['user_type'] = 0
+                        rs = api.communicate(params, rq)
+                        if rs['result'] == 'success':
+                            logging.info('Team %s %s %s', team_name, 'added to' if is_add else 'removed from', user['username'])
+                    api.query_enterprise(params)
+
+            elif user_name or node_id:
+                dt = user['data'].copy()
+                if user_name:
+                    dt['displayname'] = user_name
+                rq = {
+                    'command': 'enterprise_user_update',
+                    'enterprise_user_id': user['enterprise_user_id'],
+                    'node_id': node_id if node_id is not None else user['node_id'],
+                    'encrypted_data': api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key']),
+                    'enterprise_user_username': user['username']
+                }
+                rs = api.communicate(params, rq)
+                if rs['result'] == 'success':
+                    logging.info('User %s is modified', user['username'])
+                    api.query_enterprise(params)
+
+            else:
+                is_verbose = kwargs.get('verbose') or False
                 self.display_user(params, user, is_verbose)
-                print('\n')
+        else:
+            if len(matched_users) > 0:
+                is_verbose = kwargs.get('verbose') or False
+                skip = True
+                for user in matched_users:
+                    if skip:
+                        skip = False
+                    else:
+                        print('\n')
+                    self.display_user(params, user, is_verbose)
+            else:
+                logging.warning('No such user')
 
-    def display_user(self, params, user, is_verbose=False):
+    def display_user(self, params, user, is_verbose = False):
         print('{0:>16s}: {1}'.format('User ID', user['enterprise_user_id']))
-        print('{0:>16s}: {1}'.format('Email', user['username'] if 'username' in user else '[empty]'))
+        print('{0:>16s}: {1}'.format('Email', user['username']))
         print('{0:>16s}: {1}'.format('Display Name', user['data'].get('displayname') or ''))
+        status = lock_text(user['lock'])
+        if not status:
+            if 'account_share_expiration' in user:
+                expire_at = datetime.datetime.fromtimestamp(user['account_share_expiration']/1000.0)
+                if expire_at < datetime.datetime.now():
+                    status = 'Blocked'
+                else:
+                    status = 'Transfer Acceptance'
+            else:
+                status = user['status'].capitalize()
+        print('{0:>16s}: {1}'.format('Status', status))
 
-        status_dict = get_user_status_dict(user)
-
-        acct_status = status_dict['acct_status']
-        acct_transfer_status = status_dict['acct_transfer_status']
-
-        print('{0:>16s}: {1}'.format('Status', acct_status))
-
-        if acct_transfer_status:
-            print('{0:>16s}: {1}'.format('Transfer Status', acct_transfer_status))
+        if 'team_users' in params.enterprise and 'teams' in params.enterprise:
+            team_nodes = {}
+            for t in params.enterprise['teams']:
+                team_nodes[t['team_uid']] = t
+            user_id = user['enterprise_user_id']
+            ts = [t['team_uid'] for t in params.enterprise['team_users'] if t['enterprise_user_id'] == user_id]
+            for i in range(len(ts)):
+                team_node = team_nodes[ts[i]]
+                print('{0:>16s}: {1:<22s} {2}'.format('Team' if i == 0 else '', team_node['name'], team_node['team_uid'] if is_verbose else ''))
 
         if 'role_users' in params.enterprise:
             role_ids = [x['role_id'] for x in params.enterprise['role_users'] if x['enterprise_user_id'] == user['enterprise_user_id']]
             if len(role_ids) > 0:
                 role_nodes = {}
                 for r in params.enterprise['roles']:
                     role_nodes[r['role_id']] = r
                 for i in range(len(role_ids)):
                     role_node = role_nodes[role_ids[i]]
                     print('{0:>16s}: {1:<22s} {2}'.format('Role' if i == 0 else '', role_node['data']['displayname'], role_node['role_id'] if is_verbose else ''))
 
-        team_nodes = {}
-        if 'teams' in params.enterprise:
-            for t in params.enterprise['teams']:
-                team_nodes[t['team_uid']] = t
-        if 'queued_teams' in params.enterprise:
-            for t in params.enterprise['queued_teams']:
-                team_nodes[t['team_uid']] = t
-
-        if 'team_users' in params.enterprise:
-            user_id = user['enterprise_user_id']
-            ts = [t['team_uid'] for t in params.enterprise['team_users'] if t['enterprise_user_id'] == user_id]
-            ts.sort(key=lambda x: team_nodes[x]['name'])
-            for i in range(len(ts)):
-                team_node = team_nodes[ts[i]]
-                print('{0:>16s}: {1:<22s} {2}'.format('Team' if i == 0 else '', team_node['name'], team_node['team_uid'] if is_verbose else ''))
-
-        if 'queued_team_users' in params.enterprise:
-            user_id = user['enterprise_user_id']
-            ts = [t['team_uid'] for t in params.enterprise['queued_team_users'] if user_id in t['users']]
-            ts.sort(key=lambda x: team_nodes[x]['name'])
-            for i in range(len(ts)):
-                team_node = team_nodes[ts[i]]
-                print('{0:>16s}: {1:<22s} {2}'.format('Queued Team' if i == 0 else '', team_node['name'], team_node['team_uid'] if is_verbose else ''))
-
 
 class EnterpriseRoleCommand(EnterpriseCommand):
     def get_parser(self):
         return enterprise_role_parser
 
     def execute(self, params, **kwargs):
-        if kwargs.get('add') and kwargs.get('remove'):
-            raise CommandError('enterprise-role', "'add' and 'delete' parameters are mutually exclusive.")
-
-        role_lookup = {}
+        r_arg = str(kwargs['role'])
+        role = None
         if 'roles' in params.enterprise:
             for r in params.enterprise['roles']:
-                role_lookup[str(r['role_id'])] = r
-                name = r['data'].get('displayname') or ''
-                if name:
-                    name = name.lower()
-                    if name in role_lookup:
-                        if type(role_lookup[name]) == list:
-                            role_lookup[name].append(r)
-                        else:
-                            old = role_lookup[name]
-                            role_lookup[name] = [old, r]
-                    else:
-                        role_lookup[name] = r
-
-        node_id = None
-        if kwargs.get('node'):
-            for node in params.enterprise['nodes']:
-                if kwargs['node'] in {str(node['node_id']), node['data'].get('displayname')}:
-                    node_id = node['node_id']
+                if r_arg in {str(r['role_id']), r['data'].get('displayname') or ''}:
+                    role = r
                     break
-                elif not node.get('parent_id') and kwargs['node'] == params.enterprise['enterprise_name']:
-                    node_id = node['node_id']
-                    break
-
-        matched = {}
-        role_names = set()
-
-        for role_name in kwargs['role']:
-            role_name = str(role_name)
-            r = role_lookup.get(role_name.lower())
-            if r is None:
-                role_names.add(role_name)
-            elif type(r) == list:
-                role_in_node = None
-                if node_id:
-                    for ro in r:
-                        if ro['node_id'] == node_id:
-                            role_in_node = ro
-                            break
-                if role_in_node:
-                    matched[role_in_node['role_id']] = role_in_node
-                else:
-                    logging.warning('Role name \'%s\' is not unique. Use Role ID. Skipping', role_name)
-            elif type(r) == dict:
-                matched[r['role_id']] = r
-
-        matched_roles = list(matched.values())
-
-        request_batch = []
-        if kwargs.get('add'):
-            for role in matched_roles:
-                logging.warning('Role \'%s\' already exists: Skipping', role['data'].get('displayname'))
-            if not role_names:
-                return
-
-            if node_id is None:
-                for node in params.enterprise['nodes']:
-                    if not node.get('parent_id'):
-                        node_id = node['node_id']
-                        break
-
-            for role_name in role_names:
-                dt = { "displayname": role_name }
-                rq = {
-                    "command": "role_add",
-                    "role_id": self.get_enterprise_id(params),
-                    "node_id": node_id,
-                    "encrypted_data": api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key']),
-                    "visible_below": (kwargs['visible_below'] == 'on') or False,
-                    "new_user_inherit": (kwargs['new_user'] == 'on') or False
-                }
-                request_batch.append(rq)
-        else:
-            for role_name in role_names:
-                logging.warning('Role %s is not found: Skipping', role_name)
-
-            if not matched_roles:
-                return
-
-            if kwargs.get('delete'):
-                for role in matched_roles:
-                    request_batch.append({ "command": "role_delete", "role_id": role['role_id'] })
 
-            elif kwargs.get('add_user') or kwargs.get('remove_user'):
-                user_changes = {}
-                for is_add in [False, True]:
-                    ul = kwargs.get('add_user') if is_add else kwargs.get('remove_user')
-                    if ul:
-                        for u in ul:
-                            uname = u.lower()
-                            user_node = None
-                            if 'users' in params.enterprise:
-                                for user in params.enterprise['users']:
-                                    if uname in { str(user['enterprise_user_id']),
-                                                  user['username'].lower() }:
-                                        user_node = user
-                                        break
-                            if user_node:
-                                user_id = user_node['enterprise_user_id']
-                                user_changes[user_id] = is_add, user_node['username']
-                            else:
-                                logging.warning('User %s could be resolved', u)
+        show_info = True
 
-                user_pkeys = {}
-                for role in matched_roles:
-                    role_id = role['role_id']
-                    for user_id in user_changes:
-                        is_add, email = user_changes[user_id]
-                        role_key = None
-                        is_managed_role = False
-                        if is_add:
-                            if 'managed_nodes' in params.enterprise:
-                                for mn in params.enterprise['managed_nodes']:
-                                    if mn['role_id'] == role_id:
-                                        is_managed_role = True
-                                        break
-                        if is_managed_role:
-
-                            if 'role_keys2' in params.enterprise:
-                                for rk2 in params.enterprise['role_keys2']:
-                                    if rk2['role_id'] == role_id:
-                                        encrypted_key_decoded = base64.urlsafe_b64decode(rk2['role_key'] + '==')
-                                        role_key = rest_api.decrypt_aes(encrypted_key_decoded, params.enterprise['unencrypted_tree_key'])
-                                        break
-
-                            if 'role_keys' in params.enterprise and role_key is None:
-                                for rk in params.enterprise['role_keys']:
-                                    if rk['role_id'] == role_id:
-                                        if rk['key_type'] == 'encrypted_by_data_key':
-                                            role_key = api.decrypt_data(rk['encrypted_key'], params.data_key)
-                                        elif rk['key_type'] == 'encrypted_by_public_key':
-                                            role_key = api.decrypt_rsa(rk['encrypted_key'], params.rsa_key)
-                                        break
-                        rq = {
-                            'command': 'role_user_add' if is_add else 'role_user_remove',
-                            'enterprise_user_id': user_id,
-                            'role_id': role_id
-                        }
-                        if is_managed_role:
-                            if user_id not in user_pkeys:
-                                answer = 'y' if kwargs.get('force') else user_choice('Do you want to grant administrative privileges to {0}'.format(email), 'yn', 'n')
-                                public_key = None
-                                if answer == 'y':
-                                    public_key = self.get_public_key(params, email)
-                                    if public_key is None:
-                                        logging.warning('Cannot get public key for user %s', email)
-                                user_pkeys[user_id] = public_key
-                            if user_pkeys[user_id]:
-                                rq['tree_key'] = api.encrypt_rsa(params.enterprise['unencrypted_tree_key'], user_pkeys[user_id])
-                                if role_key:
-                                    rq['role_admin_key'] = api.encrypt_rsa(role_key, user_pkeys[user_id])
-                                request_batch.append(rq)
-                        else:
-                            request_batch.append(rq)
-
-            elif kwargs.get('add_admin') or kwargs.get('remove_admin'):
-                node_lookup = {}
-                if 'nodes' in params.enterprise:
-                    for node in params.enterprise['nodes']:
-                        node_lookup[str(node['node_id'])] = node
-                        if node.get('parent_id'):
-                            node_name = node['data'].get('displayname')
+        if role and (kwargs.get('add_user') or kwargs.get('remove_user')):
+            show_info = False
+            users = {}
+            for is_add in [False, True]:
+                ul = kwargs.get('add_user') if is_add else kwargs.get('remove_user')
+                if ul:
+                    for u in ul:
+                        uname = u.lower()
+                        user_node = None
+                        if 'users' in params.enterprise:
+                            for user in params.enterprise['users']:
+                                if uname in { str(user['enterprise_user_id']),
+                                              user['username'].lower(),
+                                              (user['data'].get('displayname') or '').lower() }:
+                                    user_node = user
+                                    break
+                        if user_node:
+                            user_id = user_node['enterprise_user_id']
+                            users[user_id] = is_add, user_node['username']
                         else:
-                            node_name = params.enterprise['enterprise_name']
-                        node_name = node_name.lower()
-                        value = node_lookup.get(node_name)
-                        if value is None:
-                             value = node
-                        elif type(value) == list:
-                            value.append(node)
-                        else:
-                            value = [value, node]
-                        node_lookup[node_name] = value
-
-                node_changes = {}
-                for is_add in [False, True]:
-                    ul = kwargs.get('add_admin') if is_add else kwargs.get('remove_admin')
-                    if ul:
-                        for u in ul:
-                            value = node_lookup.get(u.lower())
-                            if value:
-                                if value is None:
-                                    logging.warning('Node %s could be resolved', u)
-                                if type(value) == dict:
-                                    node_changes[value['node_id']] = is_add, value['data'].get('displayname') or params.enterprise['enterprise_name']
-                                elif type(value) == list:
-                                    logging.warning('Node name \'%s\' is not unique. Use Node ID. Skipping', u)
-
-                for role in matched_roles:
-                    role_id = role['role_id']
-                    for node_id in node_changes:
-                        is_add, node_name = node_changes[node_id]
-                        rq = {
-                            "command": "role_managed_node_add" if is_add else "role_managed_node_remove",
-                            "role_id": role_id,
-                            "managed_node_id": node_id
-                        }
-                        if is_add:
-                            rq['cascade_node_management'] = (kwargs.get('cascade') == 'on') or False
-                            rq['tree_keys'] = []
-                            if 'role_users' in params.enterprise:
-                                for user_id in [x['enterprise_user_id'] for x in params.enterprise['role_users'] if x['role_id'] == role_id]:
-                                    emails = [x['username'] for x in params.enterprise['users'] if x['enterprise_user_id'] == user_id]
-                                    if emails:
-                                        public_key = self.get_public_key(params, emails[0])
-                                        if public_key:
-                                            rq['tree_keys'].append({
-                                                "enterprise_user_id": user_id,
-                                                "tree_key": api.encrypt_rsa(params.enterprise['unencrypted_tree_key'], public_key)
-                                            })
-                        request_batch.append(rq)
-            elif node_id or kwargs.get('visible_below') or kwargs.get('new_user') or kwargs.get('name'):
-                if kwargs.get('name') and len(matched_roles) > 1:
-                    logging.warning('Cannot assign the same name to %s roles', len(matched_roles))
-                    kwargs['name'] = None
-
-                for role in matched_roles:
-                    encrypted_data = role['encrypted_data']
-                    if kwargs.get('name'):
-                        role_name = kwargs.get('name').strip()
-                        dt = { "displayname": role_name }
-                        encrypted_data = api.encrypt_aes(json.dumps(dt).encode('utf-8'), params.enterprise['unencrypted_tree_key'])
+                            logging.warning('User %s could be resolved', u)
+            if len(users) > 0:
+                has_managed_nodes = False
+                role_key = False
+                if 'managed_nodes' in params.enterprise:
+                    for mn in params.enterprise['managed_nodes']:
+                        if mn['role_id'] == role['role_id']:
+                            has_managed_nodes = True
+                            break
+                if 'role_keys' in params.enterprise:
+                    for rk in params.enterprise['role_keys']:
+                        if rk['role_id'] == role['role_id']:
+                            if rk['key_type'] == 'encrypted_by_data_key':
+                                role_key = api.decrypt_aes(rk['encrypted_key'] , params.data_key)
+                            elif rk['key_type'] == 'encrypted_by_public_key':
+                                role_key = api.decrypt_rsa(rk['encrypted_key'] , params.rsa_key)
+                            break
+                for user_id in users:
+                    is_add, user_email = users[user_id]
                     rq = {
-                        "command": "role_update",
-                        "role_id": role['role_id'],
-                        "node_id": node_id or role['node_id'],
-                        "encrypted_data": encrypted_data
+                        'command': 'role_user_add' if is_add else 'role_user_remove',
+                        'role_id': role['role_id'],
+                        'enterprise_user_id': user_id
                     }
-                    if kwargs.get('visible_below'):
-                        rq['visible_below'] = kwargs.get('visible_below') == 'on'
-                    if kwargs.get('new_user'):
-                        rq['new_user_inherit'] = kwargs['new_user'] == 'on'
-                    request_batch.append(rq)
-
-        if request_batch:
-            rss = api.execute_batch(params, request_batch)
-            for rq, rs in zip(request_batch, rss):
-                command = rq.get('command')
-                if command == 'role_add':
+                    if is_add:
+                        if has_managed_nodes:
+                            public_key = self.get_public_key(params, user_email)
+                            if public_key:
+                                rq['tree_key'] = api.encrypt_rsa(params.enterprise['unencrypted_tree_key'], public_key)
+                        if role_key:
+                            public_key = self.get_public_key(params, user_email)
+                            if public_key:
+                                rq['role_admin_key'] = api.encrypt_rsa(role_key, public_key)
+
+                    rs = api.communicate(params, rq)
                     if rs['result'] == 'success':
-                        logging.info('Role created')
-                    else:
-                        logging.warning('Failed to create role: %s', rs['message'])
-                else:
-                    role = None
-                    if not role and 'role_id' in rq:
-                        role = role_lookup.get(str(rq['role_id']))
-                    if role:
-                        role_name = role['data'].get('displayname')
-                        if command in { 'role_delete', 'role_update' }:
-                            if rs['result'] == 'success':
-                                logging.info('\'%s\' role is %s', role_name, 'deleted' if command == 'role_delete' else 'updated')
-                            else:
-                                logging.warning('\'%s\' failed to %s role: %s', role_name, 'delete' if command == 'role_delete' else 'update',  rs['message'])
-                        elif command in {'role_user_add', 'role_user_remove'}:
-                            user_names = [x['username'] for x in params.enterprise['users'] if x['enterprise_user_id'] == rq['enterprise_user_id']]
-                            user_name = user_names[0] if len(user_names) > 0 else str(rq['enterprise_user_id'])
-                            if rs['result'] == 'success':
-                                logging.info('\'%s\' role %s %s', role_name, 'assigned to' if command == 'role_user_add' else 'removed from', user_name)
-                            else:
-                                logging.warning('\'%s\' role failed to %s %s: %s', role_name, 'assign' if command == 'role_user_add' else 'remove', user_name, rs['message'])
-                        elif command in {'role_managed_node_add', 'role_managed_node_remove'}:
-                            node_names = [x for x in params.enterprise['nodes'] if x['node_id'] == rq['managed_node_id']]
-                            node_name = (node_names[0]['data'].get('displayname') or params.enterprise['enterprise_name']) if len(node_names) > 0 else ''
-                            if rs['result'] == 'success':
-                                logging.info('\'%s\' role is %s managing node \'%s\'', role_name, 'assigned to' if command == 'role_managed_node_add' else 'removed from', node_name)
-                            else:
-                                logging.warning('\'%s\' role failed to %s managing node \'%s\': %s', role_name, 'assign' if command == 'role_managed_node_add' else 'remove', node_name, rs['message'])
-                        else:
-                            if rs['result'] != 'success':
-                                logging.warning('\'%s\' error: %s', command, rs['message'])
-                    else:
-                        if rs['result'] != 'success':
-                            logging.warning('Error: %s', rs['message'])
-            api.query_enterprise(params)
+                        logging.info('User %s %s role %s', user_email, 'added to' if is_add else 'removed from', role['data'].get('displayname') or '')
+                api.query_enterprise(params)
+
+        if role:
+            if show_info:
+                role_id = role['role_id']
+                print('{0:>24s}: {1}'.format('Role ID', role_id))
+                print('{0:>24s}: {1}'.format('Role Name', role['data'].get('displayname')))
+                print('{0:>24s}: {1}'.format('Node', self.get_node_path(params, role['node_id'])))
+                print('{0:>24s}: {1}'.format('Cascade?', 'Yes' if role['visible_below'] else 'No'))
+                print('{0:>24s}: {1}'.format('New user?', 'Yes' if role['new_user_inherit'] else 'No'))
+                if 'role_users' in params.enterprise:
+                    user_ids = [x['enterprise_user_id'] for x in params.enterprise['role_users'] if x['role_id'] == role_id]
+                    if len(user_ids) > 0:
+                        users = {}
+                        for user in params.enterprise['users']:
+                            users[user['enterprise_user_id']] = user['username']
+                        user_ids.sort(key=lambda x: users[x])
+                        for i in range(len(user_ids)):
+                            user_id = user_ids[i]
+                            print('{0:>24s}: {1:<32s} {2}'.format('User(s)' if i == 0 else '', users[user_id], user_id if kwargs.get('verbose') else ''))
+
+                if 'role_enforcements' in params.enterprise:
+                    enforcements = None
+                    for e in params.enterprise['role_enforcements']:
+                        if role_id == e['role_id']:
+                            enforcements = e['enforcements']
+                            break
+                    if enforcements:
+                        print('{0:>24s}: '.format('Role Enforcements'))
+                        if 'master_password_minimum_length' in enforcements:
+                            print('{0:>24s}: '.format('Password Complexity'))
+                            for p in [('Length', 'master_password_minimum_length'),
+                                      ('Digits', 'master_password_minimum_digits'),
+                                      ('Special Characters', 'master_password_minimum_special'),
+                                      ('Uppercase Letters', 'master_password_minimum_upper'),
+                                      ('Lowercase Letters', 'master_password_minimum_lower')]:
+                                if enforcements.get(p[1]) > 0:
+                                    print('{0:>24s}: {1}'.format(p[0], enforcements.get(p[1])))
         else:
-            for role in matched_roles:
-                print('\n')
-                self.display_role(params, role, kwargs.get('verbose'))
-            print('\n')
-
-    def display_role(self, params, role, is_verbose = False):
-        role_id = role['role_id']
-        print('{0:>24s}: {1}'.format('Role ID', role_id))
-        print('{0:>24s}: {1}'.format('Role Name', role['data'].get('displayname')))
-        print('{0:>24s}: {1}'.format('Node', self.get_node_path(params, role['node_id'])))
-        print('{0:>24s}: {1}'.format('Cascade?', 'Yes' if role['visible_below'] else 'No'))
-        print('{0:>24s}: {1}'.format('New user?', 'Yes' if role['new_user_inherit'] else 'No'))
-        if 'role_users' in params.enterprise:
-            user_ids = [x['enterprise_user_id'] for x in params.enterprise['role_users'] if x['role_id'] == role_id]
-            if len(user_ids) > 0:
-                users = {}
-                for user in params.enterprise['users']:
-                    users[user['enterprise_user_id']] = user['username']
-                user_ids.sort(key=lambda x: users[x])
-                for i in range(len(user_ids)):
-                    user_id = user_ids[i]
-                    print('{0:>24s}: {1:<32s} {2}'.format('User(s)' if i == 0 else '', users[user_id], user_id if is_verbose else ''))
-
-        if 'managed_nodes' in params.enterprise:
-            node_ids = [x['managed_node_id'] for x in params.enterprise['managed_nodes'] if x['role_id'] == role_id]
-            if len(node_ids) > 0:
-                nodes = {}
-                for node in params.enterprise['nodes']:
-                    nodes[node['node_id']] = node['data'].get('displayname') or params.enterprise['enterprise_name']
-                node_ids.sort(key=lambda x: nodes[x])
-                for i in range(len(node_ids)):
-                    node_id = node_ids[i]
-                    print('{0:>24s}: {1:<32s} {2}'.format('Manages Nodes(s)' if i == 0 else '', nodes[node_id], node_id if is_verbose else ''))
-
-        if 'role_enforcements' in params.enterprise:
-            enforcements = None
-            for e in params.enterprise['role_enforcements']:
-                if role_id == e['role_id']:
-                    enforcements = e['enforcements']
-                    break
-            if enforcements:
-                print('{0:>24s}: '.format('Role Enforcements'))
-                if 'master_password_minimum_length' in enforcements:
-                    print('{0:>24s}: '.format('Password Complexity'))
-                    for p in [('Length', 'master_password_minimum_length'),
-                              ('Digits', 'master_password_minimum_digits'),
-                              ('Special Characters', 'master_password_minimum_special'),
-                              ('Uppercase Letters', 'master_password_minimum_upper'),
-                              ('Lowercase Letters', 'master_password_minimum_lower')]:
-                        value = enforcements.get(p[1])
-                        if value is not None:
-                            print('{0:>24s}: {1}'.format(p[0], value))
+            logging.warning('Role not found')
 
 
 class EnterpriseTeamCommand(EnterpriseCommand):
     def get_parser(self):
         return enterprise_team_parser
 
     def execute(self, params, **kwargs):
-        if (kwargs.get('add') or kwargs.get('approve')) and kwargs.get('remove'):
-            raise CommandError('enterprise-team', "'add'/'approve' and 'delete' commands are mutually exclusive.")
-
-        team_lookup = {}
+        t_arg = kwargs['team']
+        team = None
         if 'teams' in params.enterprise:
-            for team in params.enterprise['teams']:
-                team_lookup[team['team_uid']] = team
-                team_lookup[team['name'].lower()] = team
-
-        if 'queued_teams' in params.enterprise:
-            for team in params.enterprise['queued_teams']:
-                team_lookup[team['team_uid']] = team
-                team_lookup[team['name'].lower()] = team
+            for t in params.enterprise['teams']:
+                if t_arg == t['team_uid'] or t_arg.lower() == t['name'].lower():
+                    team = t
+                    break
 
         node_id = None
         if kwargs.get('node'):
-            parent_node = kwargs.get('node')
+            for node in params.enterprise['nodes']:
+                if kwargs['node'] in {str(node['node_id']), node['data'].get('displayname')}:
+                    node_id = node['node_id']
+                    break
+                elif not node.get('parent_id') and kwargs['node'] == params.enterprise['enterprise_name']:
+                    node_id = node['node_id']
+                    break
 
-            if parent_node:
-                for node in params.enterprise['nodes']:
-                    if parent_node in {str(node['node_id']), node['data'].get('displayname')}:
-                        node_id = node['node_id']
-                        break
-                    elif not node.get('parent_id') and parent_node == params.enterprise['enterprise_name']:
-                        node_id = node['node_id']
-                        break
+        if kwargs.get('delete'):
+            if team is not None:
+                answer = 'y' if kwargs.get('force') else \
+                    user_choice('Delete Team\n\nAre you sure you want to delete {0}'.format(team['name']), 'yn', 'n')
+                if answer.lower() == 'y':
+                    rq = {
+                        'command': 'team_delete',
+                        'team_uid': team['team_uid']
+                    }
+                    rs = api.communicate(params, rq)
+                    if rs['result'] == 'success':
+                        logging.info('Team %s deleted', team['name'])
+                        api.query_enterprise(params)
+            else:
+                logging.warning('Team not found')
+            return
 
-                if not node_id:
-                    logging.warning("Node %s does not exist", parent_node)
-                    return
-
-        matched = {}
-        team_names = set()
-
-        for team_name in kwargs['team']:
-            t = team_lookup.get(team_name)
-            if t is None:
-                t = team_lookup.get(team_name.lower())
-            if t is None:
-                team_names.add(team_name)
-            elif type(t) == list:
-                team_in_node = None
-                if node_id:
-                    for ro in t:
-                        if ro['node_id'] == node_id:
-                            team_in_node = ro
+        if kwargs.get('add'):
+            if team is None:
+                if node_id is None:
+                    for node in params.enterprise['nodes']:
+                        if not node.get('parent_id'):
+                            node_id = node['node_id']
                             break
-                if team_in_node:
-                    matched[team_in_node['team_uid']] = team_in_node
-                else:
-                    logging.warning('Team name \'%s\' is not unique. Use Team UID. Skipping', team_name)
-            elif type(t) == dict:
-                matched[t['team_uid']] = t
-
-        matched_teams = list(matched.values())
-        request_batch = []
-
-        if kwargs.get('add') or kwargs.get('approve'):
-            queue = []
-            for team in matched_teams:
-                if kwargs.get('approve'):
-                    if 'restrict_edit' not in team:
-                        queue.append(team)
-                        continue
-                logging.warning('Team \'%s\' already exists: Skipping', team['name'])
-
-            if kwargs.get('add'):
-                queue.extend(team_names)
-
-            if not queue:
-                return
-
-            if node_id is None:
-                for node in params.enterprise['nodes']:
-                    if not node.get('parent_id'):
-                        node_id = node['node_id']
-                        break
-
-            for item in queue:
-                is_new_team = type(item) == str
-                team_name = item if is_new_team else item['name']
-                team_node_id = node_id if is_new_team else item['node_id']
-                team_uid = api.generate_record_uid() if is_new_team else item['team_uid']
+                team_uid = api.generate_record_uid()
                 team_key = api.generate_aes_key()
-                encrypted_team_key = rest_api.encrypt_aes(team_key, params.enterprise['unencrypted_tree_key'])
                 rsa_key = RSA.generate(2048)
                 private_key = DerSequence([0,
                                            rsa_key.n,
                                            rsa_key.e,
                                            rsa_key.d,
                                            rsa_key.p,
                                            rsa_key.q,
@@ -2000,180 +1066,111 @@
                 public_key = DerSequence([pub_key.n,
                                           pub_key.e
                                           ]).encode()
 
                 rq = {
                     'command': 'team_add',
                     'team_uid': team_uid,
-                    'team_name': team_name,
-                    'restrict_edit': kwargs.get('restrict_edit') == 'on',
-                    'restrict_share': kwargs.get('restrict_share') == 'on',
-                    'restrict_view': kwargs.get('restrict_view') == 'on',
-                    'public_key': base64.urlsafe_b64encode(public_key).decode().rstrip('='),
+                    'team_name': t_arg,
+                    'restrict_edit': kwargs.get('restrict_edit') == 'on' if kwargs.get('restrict_edit') else False,
+                    'restrict_share': kwargs.get('restrict_share') == 'on' if kwargs.get('restrict_share') else False,
+                    'restrict_view': kwargs.get('restrict_view') == 'on' if kwargs.get('restrict_view') else False,
+                    'public_key': base64.urlsafe_b64encode(public_key).rstrip(b'=').decode(),
                     'private_key': api.encrypt_aes(private_key, team_key),
-                    'node_id': team_node_id,
+                    'node_id': node_id,
                     'team_key': api.encrypt_aes(team_key, params.data_key),
-                    'encrypted_team_key': base64.urlsafe_b64encode(encrypted_team_key).decode().rstrip('='),
                     'manage_only': True
                 }
-                request_batch.append(rq)
-        else:
-            for team_name in team_names:
-                logging.warning('\'%s\' team is not found: Skipping', team_name)
-
-            if not matched_teams:
-                return
+                rs = api.communicate(params, rq)
+                if rs['result'] == 'success':
+                    logging.info('Team %s created', t_arg)
+                    api.query_enterprise(params)
+                    params.environment_variables[LAST_TEAM_UID] = team_uid
+            else:
+                logging.warning('Team %s already exists', t_arg)
+            return
 
-            if kwargs.get('delete'):
-                answer = 'y' if kwargs.get('force') else \
-                    user_choice('Delete Team(s)\n\nAre you sure you want to delete {0} team(s)'.format(len(matched_teams)), 'yn', 'n')
-                if answer.lower() == 'y':
-                    for team in matched_teams:
-                        rq = {
-                            'command': 'team_delete',
-                            'team_uid': team['team_uid']
-                        }
-                        request_batch.append(rq)
+        if team:
+            show_info = True
+            team_name = kwargs.get('name')
+            if team_name or node_id or kwargs.get('restrict_edit') or kwargs.get('restrict_share') or kwargs.get('restrict_view'):
+                rq = {
+                    'command': 'team_update',
+                    'team_uid': team['team_uid'],
+                    'team_name': team_name or team['name'],
+                    'restrict_edit': kwargs.get('restrict_edit') == 'on' if kwargs.get('restrict_edit') else team['restrict_edit'],
+                    'restrict_share': kwargs.get('restrict_share') == 'on' if kwargs.get('restrict_share') else team['restrict_sharing'],
+                    'restrict_view': kwargs.get('restrict_view') == 'on' if kwargs.get('restrict_view') else team['restrict_view'],
+                    'node_id': node_id or team['node_id']
+                }
+                rs = api.communicate(params, rq)
+                if rs['result'] == 'success':
+                    print('Team {0} modified'.format(team['name']))
+                    show_info = False
+                    api.query_enterprise(params)
 
             if kwargs.get('add_user') or kwargs.get('remove_user'):
+                show_info = False
                 users = {}
                 for is_add in [False, True]:
                     ul = kwargs.get('add_user') if is_add else kwargs.get('remove_user')
                     if ul:
                         for u in ul:
                             uname = u.lower()
                             user_node = None
                             if 'users' in params.enterprise:
                                 for user in params.enterprise['users']:
                                     if uname in { str(user['enterprise_user_id']),
-                                                  user['username'].lower() }:
+                                                  user['username'].lower(),
+                                                  (user['data'].get('displayname') or '').lower() }:
                                         user_node = user
                                         break
                             if user_node:
                                 user_id = user_node['enterprise_user_id']
-                                users[user_id] = is_add, user_node
+                                users[user_id] = is_add, user_node['username']
                             else:
                                 logging.warning('User %s could be resolved', u)
-
                 if len(users) > 0:
-                    for team in matched_teams:
-                        is_real_team = 'restrict_edit' in team
-                        for user_id in users:
-                            is_add, user = users[user_id]
-                            rq = None
-                            if is_add:
-                                is_active_user = user['status'] == 'active'
-                                if is_real_team and is_active_user:
-                                    public_key = self.get_public_key(params, user['username'])
-                                    team_key = self.get_team_key(params, team['team_uid'])
-                                    if public_key and team_key:
-                                        rq = {
-                                            'command': 'team_enterprise_user_add',
-                                            'team_uid': team['team_uid'],
-                                            'enterprise_user_id': user_id,
-                                            'user_type': 0,
-                                            'team_key': api.encrypt_rsa(team_key, public_key)
-                                        }
-                                else:
-                                    rq = {
-                                        'command': 'team_queue_user',
-                                        'team_uid': team['team_uid'],
-                                        'enterprise_user_id': user_id
-                                    }
-                            else:
-                                rq = {
-                                    'command': 'team_enterprise_user_remove',
-                                    'team_uid': team['team_uid'],
-                                    'enterprise_user_id': user_id
-                                }
-                            if rq:
-                                request_batch.append(rq)
-            elif node_id or kwargs.get('name') or kwargs.get('restrict_edit') or kwargs.get('restrict_share') or kwargs.get('restrict_view'):
-                if kwargs['name'] and len(matched_teams) > 1:
-                    logging.warning('Cannot set same name to %s teams', len(matched_teams))
-                    kwargs['name'] = None
-
-                for team in matched_teams:
-                    rq = {
-                        'command': 'team_update',
-                        'team_uid': team['team_uid'],
-                        'team_name': kwargs.get('name') or team['name'],
-                        'restrict_edit': kwargs.get('restrict_edit') == 'on' if kwargs.get('restrict_edit') else team['restrict_edit'],
-                        'restrict_share': kwargs.get('restrict_share') == 'on' if kwargs.get('restrict_share') else team['restrict_sharing'],
-                        'restrict_view': kwargs.get('restrict_view') == 'on' if kwargs.get('restrict_view') else team['restrict_view'],
-                        'node_id': node_id or team['node_id']
-                    }
-                    request_batch.append(rq)
+                    for user_id in users:
+                        is_add, user_email = users[user_id]
+                        rq = {
+                            'command': 'team_enterprise_user_add' if is_add else 'team_enterprise_user_remove',
+                            'team_uid': team['team_uid'],
+                            'enterprise_user_id': user_id
+                        }
+                        if is_add:
+                            public_key = self.get_public_key(params, user_email)
+                            team_key = self.get_team_key(params, team['team_uid'])
+                            if public_key and team_key:
+                                rq['user_type'] = 0
+                                rq['team_key'] = api.encrypt_rsa(team_key, public_key)
+                        rs = api.communicate(params, rq)
+                        if rs['result'] == 'success':
+                            api.query_enterprise(params)
+                            logging.info('User %s %s team %s', user_email, 'added to' if is_add else 'removed from', team['name'])
 
-        if request_batch:
-            rss = api.execute_batch(params, request_batch)
-            for rq, rs in zip(request_batch, rss):
-                command = rq.get('command')
-                team_name = None
-                if 'team_name' in rq:
-                    team_name = rq['team_name']
-                elif 'team_uid' in rq:
-                    team = team_lookup.get(rq['team_uid'])
-                    if team:
-                        team_name = team['name']
-                if not team_name:
-                    team_name = rq['team_uid']
-                if command in { 'team_add', 'team_delete', 'team_update' }:
-                    verb = 'created' if command == 'team_add' else 'deleted' if command == 'team_delete' else 'updated'
-                    if rs['result'] == 'success':
-                        logging.info('\'%s\' team is %s', team_name, verb)
-                    else:
-                        logging.warning('\'%s\' team is not %s: %s', team_name, verb, rs['message'])
-                elif command in {'team_enterprise_user_add', 'team_queue_user', 'team_enterprise_user_remove'}:
-                    user_id = rq['enterprise_user_id']
-                    user_names = [x['username'] for x in params.enterprise['users'] if x['enterprise_user_id'] == user_id]
-                    user_name = user_names[0] if len(user_names) > 0 else str(user_id)
-                    if rs['result'] == 'success':
-                        logging.info('\'%s\' %s team %s user %s', team_name, 'queued' if command == 'team_queue_user' else '',
-                                     'deleted' if command == 'team_enterprise_user_remove' else 'added', user_name)
-                    else:
-                        logging.warning('\'%s\' %s team failed to %s user %s: %s', team_name, 'queued' if command == 'team_queue_user' else '',
-                                        'delete' if command == 'team_enterprise_user_remove' else 'add', user_name, rs['message'])
-            api.query_enterprise(params)
+            if show_info:
+                team_uid = team['team_uid']
+                print('{0:>24s}: {1}'.format('Team UID', team_uid))
+                print('{0:>24s}: {1}'.format('Team Name', team['name']))
+                print('{0:>24s}: {1:<32s} {2}'.format('Node', self.get_node_path(params, team['node_id']), str(team['node_id'])))
+                print('{0:>24s}: {1}'.format('Restrict Edit?', 'Yes' if team['restrict_edit'] else 'No'))
+                print('{0:>24s}: {1}'.format('Restrict Share?', 'Yes' if team['restrict_sharing'] else 'No'))
+                print('{0:>24s}: {1}'.format('Restrict View?', 'Yes' if team['restrict_view'] else 'No'))
+
+                if 'team_users' in params.enterprise:
+                    user_ids = [x['enterprise_user_id'] for x in params.enterprise['team_users'] if x['team_uid'] == team_uid]
+                    user_names = {}
+                    for u in params.enterprise['users']:
+                        user_names[u['enterprise_user_id']] = u['username']
+                    user_ids.sort(key=lambda x: user_names.get(x))
+                    for i in range(len(user_ids)):
+                        print('{0:>24s}: {1:<32s} {2}'.format('User(s)' if i == 0 else '', user_names[user_ids[i]], user_ids[i] if kwargs.get('verbose') else ''))
         else:
-            for team in matched_teams:
-                print('\n')
-                self.display_team(params, team, kwargs.get('verbose'))
-            print('\n')
-
-    def display_team(self, params, team, is_verbose = False):
-        team_uid = team['team_uid']
-        is_queued_team = 'restrict_edit' not in team
-
-        print('{0:>24s}: {1}'.format('Queued ' if is_queued_team else '' + 'Team UID', team_uid))
-        print('{0:>24s}: {1}'.format('Queued ' if is_queued_team else '' + 'Team Name', team['name']))
-        print('{0:>24s}: {1:<32s} {2}'.format('Node', self.get_node_path(params, team['node_id']), str(team['node_id'])))
-        if not is_queued_team:
-            print('{0:>24s}: {1}'.format('Restrict Edit?', 'Yes' if team['restrict_edit'] else 'No'))
-            print('{0:>24s}: {1}'.format('Restrict Share?', 'Yes' if team['restrict_sharing'] else 'No'))
-            print('{0:>24s}: {1}'.format('Restrict View?', 'Yes' if team['restrict_view'] else 'No'))
-
-        user_names = {}
-        for u in params.enterprise['users']:
-            user_names[u['enterprise_user_id']] = u['username'] if 'username' in u else '[empty]'
-
-        if 'team_users' in params.enterprise:
-            user_ids = [x['enterprise_user_id'] for x in params.enterprise['team_users'] if x['team_uid'] == team_uid]
-            # user_ids.sort(key=lambda x: user_names.get(x))
-            for i in range(len(user_ids)):
-                print('{0:>24s}: {1:<32s} {2}'.format('Active User(s)' if i == 0 else '', (user_names[user_ids[i]] if user_ids[i] in user_names else "(Unmanaged User id: " + user_ids[i] + ")"), user_ids[i] if is_verbose else ''))
-
-        if 'queued_team_users' in params.enterprise:
-            user_ids = []
-            for qtu in params.enterprise['queued_team_users']:
-                if qtu['team_uid'] == team['team_uid']:
-                    user_ids.extend(qtu['users'])
-            user_ids.sort(key=lambda x: user_names.get(x))
-            for i in range(len(user_ids)):
-                print('{0:>24s}: {1:<32s} {2}'.format('Queued User(s)' if i == 0 else '', user_names[user_ids[i]], user_ids[i] if is_verbose else ''))
+            logging.warning('Team not found')
 
 
 syslog_templates = None
 
 
 def loadSyslogTemplates(params):
     global syslog_templates
@@ -2508,15 +1505,15 @@
     def chunk_size(self):
         return 250
 
 
 class AuditLogJsonExport(AuditLogBaseExport):
     def __init__(self):
         AuditLogBaseExport.__init__(self)
-
+        
     def default_record_title(self):
         return 'Audit Log: JSON'
 
     def get_properties(self, record, props):
         filename = record.login
         if not filename:
             filename = input('JSON File name: ')
@@ -2622,44 +1619,35 @@
         return "{0}:{1}".format(wsid, encoded_hash)
 
 
 class AuditLogCommand(EnterpriseCommand):
     def get_parser(self):
         return audit_log_parser
 
-    def resolve_uid(self, cache, username):
-        uname = username or ''
-        uid = cache.get(uname)
-        if not uid:
-            md5 = hashlib.md5(str(uname).encode('utf-8')).hexdigest()
-            cache[uname] = 'DELETED-'+md5
-            uid = cache.get(uname)
-        return uid
-
-
     def execute(self, params, **kwargs):
         loadSyslogTemplates(params)
 
         target = kwargs.get('target')
 
-        log_export = None        # type: AuditLogBaseExport
+        log_export = None # type: Optional[AuditLogBaseExport]
         if target == 'splunk':
             log_export = AuditLogSplunkExport()
         elif target == 'syslog':
             log_export = AuditLogSyslogFileExport()
         elif target == 'syslog-port':
             log_export = AuditLogSyslogPortExport()
         elif target == 'sumo':
             log_export = AuditLogSumologicExport()
         elif target == 'json':
             log_export = AuditLogJsonExport()
         elif target == 'azure-la':
             log_export = AuditLogAzureLogAnalyticsExport()
         else:
-            raise CommandError('audit-log', 'Audit log export: unsupported target')
+            print('Audit log export: unsupported target')
+            return
 
         record = None
         record_name = kwargs.get('record') or log_export.default_record_title()
         for r_uid in params.record_cache:
             rec = api.get_record(params, r_uid)
             if record_name in [rec.record_uid, rec.title]:
                 record = rec
@@ -2672,15 +1660,15 @@
                     'title': record_title,
                     'force': True
                 })
                 if record_uid:
                     api.sync_down(params)
                     record = api.get_record(params, record_uid)
         if record is None:
-            raise CommandError('audit-log', 'Record not found')
+            return
 
         props = {}
         props['enterprise_name'] = params.enterprise['enterprise_name']
         log_export.store_record = False
         log_export.get_properties(record, props)
 
         #query data
@@ -2694,19 +1682,14 @@
 
         events = []
         finished = False
         count = 0
         logged_ids = set()
         chunk_length = log_export.chunk_size()
 
-        anonymize = bool(kwargs.get('anonymize'))
-        ent_user_ids = {}
-        if anonymize and params.enterprise and 'users' in params.enterprise:
-            ent_user_ids = { x.get('username'): x.get('enterprise_user_id') for x in params.enterprise['users'] }
-
         while not finished:
             finished = True
             rq = {
                 'command': 'get_audit_event_reports',
                 'report_type': 'raw',
                 'scope': 'enterprise',
                 'limit': 1000,
@@ -2719,64 +1702,47 @@
                 }
 
             rs = api.communicate(params, rq)
             if rs['result'] == 'success':
                 finished = True
                 if 'audit_event_overview_report_rows' in rs:
                     audit_events = rs['audit_event_overview_report_rows']
-                    event_count = len(audit_events)
-                    if event_count > 1:
+                    if len(audit_events) > 1:
                         # remove events from the tail for the last second
                         last_event_time = int(audit_events[-1]['created'])
                         while len(audit_events) > 0:
                             event = audit_events[-1]
                             if int(event['created']) < last_event_time:
                                 break
                             audit_events = audit_events[:-1]
 
                         for event in audit_events:
                             event_id = event['id']
                             if event_id not in logged_ids:
                                 logged_ids.add(event_id)
-                                if anonymize:
-                                    uname = event.get('email') or event.get('username') or ''
-                                    ent_uid = self.resolve_uid(ent_user_ids, uname)
-                                    event['username'] = ent_uid
-                                    event['email'] = ent_uid
-                                    to_uname = event.get('to_username') or ''
-                                    if to_uname:
-                                        event['to_username'] = self.resolve_uid(ent_user_ids, to_uname)
-                                    from_uname = event.get('from_username') or ''
-                                    if from_uname:
-                                        event['from_username'] = self.resolve_uid(ent_user_ids, from_uname)
                                 events.append(log_export.convert_event(props, event))
 
                         finished = len(events) == 0
-                        if finished:
-                            if event_count > 900:
-                                finished = False
-                                last_event_time += 1
 
             while len(events) > 0:
                 to_store = events[:chunk_length]
                 events = events[chunk_length:]
                 log_export.export_events(props, to_store)
                 if log_export.should_cancel:
                     finished = True
                     break
                 count += len(to_store)
                 print('+', end='', flush=True)
 
         if last_event_time > 0:
             logging.info('')
             logging.info('Exported %d audit event(s)', count)
-            if count > 0:
-                record.set_field('last_event_time', str(last_event_time))
-                params.sync_data = True
-                api.update_record(params, record, silent=True)
+            record.set_field('last_event_time', str(last_event_time))
+            params.sync_data = True
+            api.update_record(params, record, silent=True)
 
 
 audit_report_description = '''
 Audit Report Command Syntax Description:
 
 Event properties
   id                event ID
@@ -2835,15 +1801,14 @@
 
 
 class AuditReportCommand(Command):
     def __init__(self):
         self.team_lookup = None
         self.role_lookup = None
         self.node_lookup = None
-        self._detail_lookup = None
 
     def get_value(self, params, field, event):
         if field == 'message':
             message = ''
             if event['audit_event_type'] in syslog_templates:
                 info = syslog_templates[event['audit_event_type']]
                 while True:
@@ -2915,21 +1880,16 @@
         if id in self.node_lookup:
             return '{0} ({1})'.format(self.node_lookup[id], id)
         return id
 
     def get_parser(self):
         return audit_report_parser
 
-    @property
-    def detail_lookup(self):
-        if self._detail_lookup is None:
-            self._detail_lookup = {}
-        return self._detail_lookup
-
-    def convert_value(self, field, value, **kwargs):
+    @staticmethod
+    def convert_value(field, value, **kwargs):
         if not value:
             return ''
 
         if field == "created":
             dt = datetime.datetime.utcfromtimestamp(int(value)).replace(tzinfo=datetime.timezone.utc).astimezone(tz=None)
             rt = kwargs.get('report_type') or ''
             if rt in {'day', 'week'}:
@@ -2938,58 +1898,26 @@
                 dt = dt.strftime('%B, %Y')
             elif rt == 'hour':
                 dt = dt.strftime('%Y-%m-%d @%H:00')
 
             return dt
         elif field in {"first_created", "last_created"}:
             return datetime.datetime.utcfromtimestamp(int(value)).replace(tzinfo=datetime.timezone.utc).astimezone(tz=None)
-        elif field in {'record_uid', 'shared_folder_uid', 'team_uid', 'node'}:
-            if kwargs.get('details') and kwargs.get('params'):
-                params = kwargs['params']
-                if value not in self.detail_lookup:
-                    self.detail_lookup[value] = ''
-                    if field == 'record_uid':
-                        if value in params.record_cache:
-                            r = api.get_record(params, value)
-                            if r:
-                                self.detail_lookup[value] = r.title or ''
-                    elif field == 'shared_folder_uid':
-                        if value in params.shared_folder_cache:
-                            sf = api.get_shared_folder(params, value)
-                            if sf:
-                                self.detail_lookup[value] = sf.name or ''
-                    elif field == 'team_uid' and params.enterprise:
-                        team = None
-                        if 'teams' in params.enterprise:
-                            team = next((x for x in params.enterprise['teams'] if x['team_uid'] == value), None)
-                        if not team and 'queued_teams' in params.enterprise:
-                            team = next((x for x in params.enterprise['queued_teams'] if x['team_uid'] == value), None)
-                        if team and 'name' in team:
-                            self.detail_lookup[value] = team['name'] or ''
-                    elif field == 'node' and params.enterprise:
-                        node = None
-                        if 'nodes' in params.enterprise:
-                            node = next((x for x in params.enterprise['nodes'] if str(x['node_id']) == value), None)
-                        if node and 'data' in node:
-                            self.detail_lookup[value] = node['data'].get('displayname') or ''
-
-                detail_value = self.detail_lookup.get(value)
-                if detail_value:
-                    return '{1} ({0})'.format(value, detail_value)
-        return value
+        else:
+            return value
 
     def execute(self, params, **kwargs):
         loadSyslogTemplates(params)
 
         if kwargs.get('syntax_help'):
             logging.info(audit_report_description)
             return
         if not kwargs['report_type']:
-            raise CommandError('audit-report', 'report-type parameter is missing')
-
+            logging.error('report-type parameter is missing')
+            return
         report_type = kwargs['report_type']
         rq = {
             'report_type': report_type,
             'scope': 'enterprise' if params is not None else 'user'
         }
         if report_type == 'dim':
             rq['command'] = 'get_audit_event_dimensions'
@@ -3012,15 +1940,16 @@
                 rq['timezone'] = hours
 
         columns = []
         if report_type != 'raw' and kwargs.get('columns'):
             columns = kwargs['columns']
             rq['columns'] = columns
         if report_type == 'dim' and len(columns) == 0:
-            raise CommandError('audit-report', "'columns' parameter is missing")
+            logging.error("'columns' parameter is missing")
+            return
 
         aggregates = []
         if report_type not in {'raw', 'dim'} and kwargs.get('aggregate'):
             if kwargs.get('aggregate'):
                 aggregates = kwargs['aggregate']
                 rq['aggregate'] = aggregates
 
@@ -3052,15 +1981,14 @@
         if filter:
             rq['filter'] = filter
 
         rs = api.communicate(params, rq)
         fields = []
         table = []
 
-        details = kwargs.get('details') or False
         if report_type == 'raw':
             fields.extend(['created', 'audit_event_type', 'username', 'ip_address', 'keeper_version', 'geo_location'])
             misc_fields = ['to_username', 'from_username', 'record_uid', 'shared_folder_uid', 'node',
                            'channel', 'status'] if kwargs.get('report_format') == 'fields' else ['message']
 
             for event in rs['audit_event_overview_report_rows']:
                 if misc_fields:
@@ -3075,54 +2003,51 @@
                     if len(fields) > lenf:
                         for f in fields[lenf:]:
                             misc_fields.remove(f)
 
                 row = []
                 for field in fields:
                     value = self.get_value(params, field, event)
-                    row.append(self.convert_value(field, value, details=details, params=params))
+                    row.append(self.convert_value(field, value))
                 table.append(row)
-            dump_report_data(table, fields, fmt=kwargs.get('format'), filename=kwargs.get('output'))
+            print(tabulate(table, headers=fields))
 
         elif report_type == 'dim':
-            to_append = False
             for dim in rs['dimensions']:
+                print('\n{0}\n'.format(dim))
                 if dim in {'audit_event_type', 'keeper_version', 'ip_address'}:
                     if dim == 'audit_event_type':
                         fields = ['id', 'name', 'category', 'syslog']
                     elif dim == 'keeper_version':
                         fields = ['version_id', 'type_id', 'type_name', 'type_category']
                     elif dim == 'ip_address':
                         fields = ['ip_address', 'city', 'region', 'country_code']
                     table = []
                     for row in rs['dimensions'][dim]:
                         table.append([row.get(x) for x in fields])
+                    print(tabulate(table, headers=fields))
                 else:
-                    fields = [dim]
-                    table = []
                     for row in rs['dimensions'][dim]:
-                        table.append([row])
-                dump_report_data(table, fields, fmt=kwargs.get('format'), filename=kwargs.get('output'), append=to_append)
-                to_append = True
+                        print(row)
 
         else:
             if aggregates:
                 fields.extend(aggregates)
             else:
                 fields.append('occurrences')
             if report_type != 'span':
                 fields.append('created')
             if columns:
                 fields.extend(columns)
             for event in rs['audit_event_overview_report_rows']:
                 row = []
                 for f in fields:
-                    row.append(self.convert_value(f, event.get(f), report_type=report_type, details=details, params=params))
+                    row.append(self.convert_value(f, event.get(f), report_type=report_type))
                 table.append(row)
-            dump_report_data(table, fields, fmt=kwargs.get('format'), filename=kwargs.get('output'))
+            print(tabulate(table, headers=fields))
 
     @staticmethod
     def convert_date(value):
         if not value.isdigit():
             if len(value) <= 10:
                 value = datetime.datetime.strptime(value, '%Y-%m-%d')
             else:
@@ -3174,133 +2099,14 @@
                 if prefix == '<':
                     return {'max': value, 'exclude_max': True}
                 return value
 
         return convert(filter_value)
 
 
-security_audit_report_description = '''
-Security Audit Report Command Syntax Description:
-
-Column Name       Description
-  username          user name
-  email             e-mail address
-  weak              number of records whose password strength is in the weak category
-  medium            number of records whose password strength is in the medium category
-  strong            number of records whose password strength is in the strong category
-  reused            number of reused passwords
-  unique            number of unique passwords
-  securityScore     security score
-  twoFactorChannel  2FA - ON/OFF
-
---report-type:
-            csv     CSV format
-            json    JSON format
-            table   Table format (default)
-'''
-
-
-class SecurityAuditReportCommand(Command):
-    def __init__(self):
-        self.user_lookup = None
-
-    def get_parser(self):
-        return security_audit_report_parser
-
-    def get_security_score(self, total, strong, unique, twoFactorOn, masterPassword):
-        strongByTotal = 0 if (total == 0 ) else (strong / total)
-        uniqueByTotal = 0 if (total == 0 ) else (unique / total)
-        twoFactorOnVal = 1 if (twoFactorOn == True) else 0
-        score = (strongByTotal + uniqueByTotal + masterPassword + twoFactorOnVal) / 4
-        return score
-
-    def resolve_user_info(self, params, enterprise_user_id):
-        if self.user_lookup is None:
-            self.user_lookup = {}
-            if params.enterprise:
-                if 'users' in params.enterprise:
-                    for user in params.enterprise['users']:
-                        if 'enterprise_user_id' in user and 'username' in user:
-                            email = user['username']
-                            username = user['data']['displayname'] if 'data' in user and 'displayname' in user['data'] else None
-                            if (username is None or not username.strip()) and 'encrypted_data' in user and 'key_type' in user:
-                                username = user['encrypted_data'] if user['key_type'] == 'no_key' else None
-                            username = email if username is None or not username.strip() else username
-                            self.user_lookup[user['enterprise_user_id']] = { 'username': username, 'email': email }
-
-        info = {
-            'username': enterprise_user_id,
-            'email': enterprise_user_id
-        }
-
-        if enterprise_user_id in self.user_lookup:
-            info = self.user_lookup[enterprise_user_id]
-
-        return info
-
-    def execute(self, params, **kwargs):
-        if kwargs.get('syntax_help'):
-            logging.info(security_audit_report_description)
-            return
-
-        format = 'table'
-        if kwargs.get('format'):
-            format = kwargs['format']
-
-        rq = proto.SecurityReportRequest()
-        rs = api.communicate_rest(params, rq, 'enterprise/get_security_report_data')
-
-        security_report_data_rs = proto.SecurityReportResponse()
-        security_report_data_rs.ParseFromString(rs)
-
-        rows = []
-        for sr in security_report_data_rs.securityReport:
-            user_info = self.resolve_user_info(params, sr.enterpriseUserId)
-            user = user_info['username'] if 'username' in user_info else str(sr.enterpriseUserId)
-            email = user_info['email'] if 'email' in user_info else str(sr.enterpriseUserId)
-            twofa_on = False if sr.twoFactor == 'two_factor_disabled' else True
-            row = {
-                'username': user,
-                'email': email,
-                'weak': 0,
-                'medium': 0,
-                'strong': 0,
-                'reused': sr.numberOfReusedPassword,
-                'unique': 0,
-                'securityScore': 25,
-                'twoFactorChannel': 'Off' if sr.twoFactor == 'two_factor_disabled' else 'On'
-            }
-            master_password_strength = 1
-
-            if sr.encryptedReportData:
-                sri = rest_api.decrypt_aes(sr.encryptedReportData, params.enterprise['unencrypted_tree_key'])
-                data = json.loads(sri)
-                row['weak'] = data['weak_record_passwords'] if 'weak_record_passwords' in data else 0
-                row['strong'] = data['strong_record_passwords'] if 'weak_record_passwords' in data else 0
-                row['medium'] = data['total_record_passwords'] - row['weak'] - row['strong']
-                row['unique'] = data['total_record_passwords'] - row['reused']
-                score = self.get_security_score(data['total_record_passwords'], row['strong'], row['unique'], twofa_on, master_password_strength)
-                score = int(100 * round(score, 2))
-                row['securityScore'] = score
-            rows.append(row)
-
-        fields = ('username', 'email', 'weak', 'medium', 'strong', 'reused', 'unique', 'securityScore', 'twoFactorChannel')
-        field_descriptions = fields
-        if format == 'table':
-            field_descriptions = ('User', 'e-mail', 'Weak', 'Medium', 'Strong', 'Reused', 'Unique', 'Security Score', '2FA')
-
-        table = []
-        for raw in rows:
-            row = []
-            for f in fields:
-                row.append(raw[f])
-            table.append(row)
-        dump_report_data(table, field_descriptions, fmt=format, filename=kwargs.get('output'))
-
-
 enterprise_push_description = '''
 Template record file example:
 
 [
     {
         "title": "Record For ${user_name}",
         "login": "${user_email}",
@@ -3392,27 +2198,75 @@
     def execute(self, params, **kwargs):
         if kwargs.get('syntax_help'):
             logging.info(enterprise_push_description)
             return
 
         name = kwargs.get('file') or ''
         if not name:
-            raise CommandError('enterprise-push', 'The template file name arguments are required')
+            logging.error('The template file name arguments are required')
+            return
 
+        template_records = None
         file_name = os.path.abspath(os.path.expanduser(name))
         if os.path.isfile(file_name):
             with open(file_name, 'r') as f:
                 template_records = json.load(f)
         else:
-            raise CommandError('enterprise-push', 'File {0} does not exists'.format(name))
+            logging.error('File %s does not exists', name)
+            return
 
-        emails = EnterprisePushCommand.collect_emails(params, kwargs)
+        emails = {}
+        users = kwargs.get('user')
+        if type(users) is list:
+            for user in users:
+                user_email = None
+                for u in params.enterprise['users']:
+                    if user.lower() in [u['username'].lower(), (u['data'].get('displayname') or '').lower(), str(u['enterprise_user_id'])]:
+                        user_email = u['username']
+                        break
+                if user_email:
+                    if user_email.lower() != params.user.lower():
+                        emails[user_email] = None
+                else:
+                    logging.warning('Cannot find user %s', user)
+
+        teams = kwargs.get('team')
+        if type(teams) is list:
+            users_map = {}
+            for u in params.enterprise['users']:
+                users_map[u['enterprise_user_id']] = u['username']
+            users_in_team = {}
+
+            if 'team_users' in params.enterprise:
+                for tu in params.enterprise['team_users']:
+                    team_uid = tu['team_uid']
+                    if not team_uid in users_in_team:
+                        users_in_team[team_uid] = []
+                    if tu['enterprise_user_id'] in users_map:
+                        users_in_team[team_uid].append(users_map[tu['enterprise_user_id']])
+
+            for team in teams:
+                team_uid = None
+                if team in params.enterprise['teams']:
+                    team_uid = team_uid
+                else:
+                    for t in params.enterprise['teams']:
+                        if team.lower() == t['name'].lower():
+                            team_uid = t['team_uid']
+                if team_uid:
+                    if team_uid in users_in_team:
+                        for user_email in users_in_team[team_uid]:
+                            if user_email.lower() != params.user.lower():
+                                emails[user_email] = None
+                else:
+                    logging.warning('Cannot find team %s', team)
 
         if len(emails) == 0:
-            raise CommandError('enterprise-push', 'No users')
+            logging.warning('No users')
+            return
 
         self.get_public_keys(params, emails)
         commands = []
         record_keys = {}
         for email in emails:
             if emails[email]:
                 record_keys[email] = {}
@@ -3446,92 +2300,36 @@
                         record_add_command['data'] = api.encrypt_aes(json.dumps(data).encode('utf-8'), record_key)
                         commands.append(record_add_command)
 
                         record_keys[email][record_uid] = api.encrypt_rsa(record_key, emails[email])
             else:
                 logging.warning('User %s is not created yet', email)
 
+        transfers = []
         for email in record_keys:
             for record_uid, record_key in record_keys[email].items():
-
-                commands.append({
-                    'command': 'record_share_update',
-                    'pt': 'Commander',
-                    'add_shares': [{
-                                        'to_username': email,
-                                        'record_uid': record_uid,
-                                        'record_key': record_key,
-                                        'transfer': True
-                                    }]
+                transfers.append({
+                    'to_username': email,
+                    'record_uid': record_uid,
+                    'record_key': record_key,
+                    'transfer': True
                 })
 
-        rss = api.execute_batch(params, commands)
-        if rss:
-            for rs in rss:
-                if 'result' in rs:
-                    if rs['result'] != 'success':
-                        logging.error('Push error (%s): %s', rs.get('result_code'), rs.get('message'))
-        params.sync_data = True
+        while transfers:
+            chunk = transfers[:90]
+            transfers = transfers[90:]
+            commands.append({
+                'command': 'record_share_update',
+                'pt': 'Commander',
+                'add_shares': chunk
+            })
 
-    @staticmethod
-    def collect_emails(params, kwargs):
-        # Collect emails from individual users and from teams
-        emails = {}
+        api.execute_batch(params, commands)
 
-        users = kwargs.get('user')
-        if type(users) is list:
-            for user in users:
-                user_email = None
-                for u in params.enterprise['users']:
-                    if user.lower() in [u['username'].lower(), (u['data'].get('displayname') or '').lower(), str(u['enterprise_user_id'])]:
-                        user_email = u['username']
-                        break
-                if user_email:
-                    if user_email.lower() != params.user.lower():
-                        emails[user_email] = None
-                else:
-                    logging.warning('Cannot find user %s', user)
-
-        teams = kwargs.get('team')
-        if type(teams) is list:
-            users_map = {}
-            for u in params.enterprise['users']:
-                users_map[u['enterprise_user_id']] = u['username']
-            users_in_team = {}
-
-            if 'team_users' in params.enterprise:
-                for tu in params.enterprise['team_users']:
-                    team_uid = tu['team_uid']
-                    if not team_uid in users_in_team:
-                        users_in_team[team_uid] = []
-                    if tu['enterprise_user_id'] in users_map:
-                        users_in_team[team_uid].append(users_map[tu['enterprise_user_id']])
-
-            if 'teams' in params.enterprise:
-
-                for team in teams:
-
-                    team_uid = None
-                    if team in params.enterprise['teams']:
-                        team_uid = team_uid
-                    else:
-                        for t in params.enterprise['teams']:
-                            if team.lower() == t['name'].lower():
-                                team_uid = t['team_uid']
-                    if team_uid:
-                        if team_uid in users_in_team:
-                            for user_email in users_in_team[team_uid]:
-                                if user_email.lower() != params.user.lower():
-                                    emails[user_email] = None
-                    else:
-                        logging.warning('Cannot find team %s', team)
-            else:
-                logging.warning('There are no teams to manage. Try to refresh your local data by synching data from the server (use command `enterprise-down`).')
-
-        return emails
+        params.sync_data = True
 
 
 class UserReportCommand(Command):
     def __init__(self):
         Command.__init__(self)
         self.nodes = {}
         self.roles = {}
@@ -3593,82 +2391,121 @@
                     self.user_teams[tu['enterprise_user_id']] = []
                 if tu['team_uid'] in self.teams:
                     self.user_teams[tu['enterprise_user_id']].append(self.teams[tu['team_uid']])
 
         look_back_days = kwargs.get('days') or 365
         logging.info('Quering latest login for the last {0} days'.format(look_back_days))
         from_date = datetime.datetime.utcnow() - datetime.timedelta(days=look_back_days)
-        report_filter = {
-            "audit_event_type": "login",
-            "created": {
-                "min": int(from_date.timestamp())
-            }
-        }
         rq = {
             "command": "get_enterprise_audit_event_reports",
             "report_type": "span",
             "aggregate": ["last_created"],
             "columns": ["username"],
-            "filter": report_filter,
+            "filter": {
+                "audit_event_type": "login",
+                "created": {
+                    "min": int(from_date.timestamp())
+                }
+            },
             "timezone": "UTC"
         }
 
         last_login = {}
         rs = api.communicate(params, rq)
         for row in rs['audit_event_overview_report_rows']:
             username = row['username']
             last_login[username.lower()] = row['last_created']
-        if len(rs['audit_event_overview_report_rows']) >= 1000:
-            active = (x['username'].lower() for x in self.users.values() if x['status'] == 'active')
-            missing = [x for x in active if x not in last_login]
-            while len(missing) > 0:
-                report_filter['username'] = missing[:999]
-                missing = missing[999:]
-                rs = api.communicate(params, rq)
-                for row in rs['audit_event_overview_report_rows']:
-                    username = row['username']
-                    last_login[username.lower()] = row['last_created']
 
         for user in self.users.values():
             key = user['username'].lower()
             if key in last_login:
                 user['last_login'] = datetime.datetime.utcfromtimestamp(int(last_login[key])).replace(tzinfo=datetime.timezone.utc).astimezone(tz=None)
 
         user_list = list(self.users.values())
         user_list.sort(key=lambda x: x['username'].lower())
 
-        rows = []
-        headers = ['email', 'name', 'status', 'transfer_status', 'last_login', 'node', 'roles', 'teams']
-        for user in user_list:
-            status_dict = get_user_status_dict(user)
-
-            acct_status = status_dict['acct_status']
-            acct_transfer_status = status_dict['acct_transfer_status']
-
-            path = self.get_node_path(user['node_id'])
-            teams = self.user_teams.get(user['enterprise_user_id']) or []
-            roles = self.user_roles.get(user['enterprise_user_id']) or []
-            teams.sort(key=str.lower)
-            roles.sort(key=str.lower)
-            ll = user.get('last_login')
-            last_log = str(ll) if ll else ''
-            rows.append([
-                user['username'],       # email
-                user['name'],           # name
-                acct_status,            # status == acct_status
-                acct_transfer_status,   # acct_transfer_status
-                last_log,               # last_login
-                ' -> '.join(path),      # node
-                roles,                  # roles
-                teams                   # teams
-            ])
-
-        if kwargs.get('format') != 'json':
-            headers = [string.capwords(x.replace('_', ' ')) for x in headers]
-        dump_report_data(rows, headers, fmt=kwargs.get('format'), filename=kwargs.get('output'))
+        file_name = kwargs['output'] or ''
+        if file_name == '-':
+            file_name = ''
+
+
+        if kwargs.get('format') == 'csv':
+            if file_name:
+                _, ext = os.path.splitext(file_name)
+                if not ext:
+                    file_name += '.csv'
+            fd = open(file_name, 'w') if file_name else sys.stdout
+            csv_writer = csv.writer(fd)
+            csv_writer.writerow(['Email', 'Name', 'Status', 'Last Login', 'Node', 'Roles', 'Teams'])
+            for user in user_list:
+                status = UserReportCommand.get_user_status(user)
+                path = self.get_node_path(user['node_id'])
+                teams = self.user_teams.get(user['enterprise_user_id']) or []
+                roles = self.user_roles.get(user['enterprise_user_id']) or []
+                teams.sort(key=str.lower)
+                roles.sort(key=str.lower)
+                ll = user.get('last_login')
+                las_log = str(ll) if ll else ''
+                csv_writer.writerow([user['username'], user['name'], status, las_log, ' -> '.join(path), ' | '.join(roles), ' | '.join(teams)])
+            if file_name:
+                fd.flush()
+                fd.close()
+
+        elif kwargs.get('format') == 'json':
+            if file_name:
+                _, ext = os.path.splitext(file_name)
+                if not ext:
+                    file_name += '.json'
+            result = []
+            for user in user_list:
+                path = self.get_node_path(user['node_id'])
+                entry = {
+                    'email': user['username'],
+                    'name': user['name'],
+                    'status':  UserReportCommand.get_user_status(user),
+                    'node':  '->'.join(path)
+                }
+                teams = self.user_teams.get(user['enterprise_user_id'])
+                if teams:
+                    teams.sort(key=str.lower)
+                    entry['teams'] = teams
+                roles = self.user_roles.get(user['enterprise_user_id'])
+                if roles:
+                    roles.sort(key=str.lower)
+                    entry['roles'] = roles
+                ll = user.get('last_login')
+                if ll:
+                    ll = ll.astimezone(tz=datetime.timezone.utc)
+                    entry['last_login'] = ll.strftime('%Y-%m-%dT%H:%M:%SZ')
+                result.append(entry)
+            if file_name:
+                with open(file_name, 'w') as jf:
+                    json.dump(result, jf, indent=2)
+            else:
+                print(json.dumps(result, indent=2))
+
+        else:
+            print('')
+            rows = []
+            headers = ['Email', 'Name', 'Status', 'Last Login', 'Node', 'Roles', 'Teams']
+            for user in user_list:
+                status = UserReportCommand.get_user_status(user)
+                path = self.get_node_path(user['node_id'])
+                teams = self.user_teams.get(user['enterprise_user_id']) or []
+                roles = self.user_roles.get(user['enterprise_user_id']) or []
+                team_len = len(teams)
+                role_len = len(roles)
+                teams.sort(key=str.lower)
+                roles.sort(key=str.lower)
+                ll = user.get('last_login')
+                las_log = str(ll) if ll else ''
+                rows.append([user['username'], user['name'], status, las_log, ' -> '.join(path), roles[0] if role_len > 0 else '', teams[0] if team_len > 0 else ''])
+                for i in range(1, max(role_len, team_len)):
+                    rows.append(['', '', '', '', '', roles[i] if i < role_len else '', teams[i] if i < team_len else ''])
+            print(tabulate(rows, headers=headers))
 
     def get_node_path(self, node_id):
         path = []
         while node_id:
             if node_id in self.nodes:
                 node = self.nodes[node_id]
                 node_name = node['name'] or 'Root'
@@ -3690,583 +2527,7 @@
         if 'account_share_expiration' in user:
             expire_at = datetime.datetime.fromtimestamp(user['account_share_expiration']/1000.0)
             if expire_at < datetime.datetime.now():
                 status = 'Blocked'
             else:
                 status = 'Pending Transfer'
         return status
-
-
-class TeamApproveCommand(EnterpriseCommand):
-    def get_parser(self):
-        return team_approve_parser
-
-    def execute(self, params, **kwargs):
-        approve_teams = True
-        approve_users = True
-        if kwargs['team'] or kwargs['user']:
-            approve_teams = kwargs['team'] or False
-            approve_users = kwargs['user'] or False
-
-        request_batch = []
-        if approve_teams and 'queued_teams' in params.enterprise:
-            for team in params.enterprise['queued_teams']:
-                team_name = team['name']
-                team_node_id = team['node_id']
-                team_uid = team['team_uid']
-                team_key = api.generate_aes_key()
-                encrypted_team_key = rest_api.encrypt_aes(team_key, params.enterprise['unencrypted_tree_key'])
-                rsa_key = RSA.generate(2048)
-                private_key = DerSequence([0,
-                                           rsa_key.n,
-                                           rsa_key.e,
-                                           rsa_key.d,
-                                           rsa_key.p,
-                                           rsa_key.q,
-                                           rsa_key.d % (rsa_key.p-1),
-                                           rsa_key.d % (rsa_key.q-1),
-                                           Integer(rsa_key.q).inverse(rsa_key.p)
-                                           ]).encode()
-                pub_key = rsa_key.publickey()
-                public_key = DerSequence([pub_key.n,
-                                          pub_key.e
-                                          ]).encode()
-
-                rq = {
-                    'command': 'team_add',
-                    'team_uid': team_uid,
-                    'team_name': team_name,
-                    'restrict_edit': kwargs.get('restrict_edit') == 'on',
-                    'restrict_share': kwargs.get('restrict_share') == 'on',
-                    'restrict_view': kwargs.get('restrict_view') == 'on',
-                    'public_key': base64.urlsafe_b64encode(public_key).decode().rstrip('='),
-                    'private_key': api.encrypt_aes(private_key, team_key),
-                    'node_id': team_node_id,
-                    'team_key': api.encrypt_aes(team_key, params.data_key),
-                    'encrypted_team_key': base64.urlsafe_b64encode(encrypted_team_key).decode().rstrip('='),
-                    'manage_only': True
-                }
-                request_batch.append(rq)
-            if request_batch:
-                rs = api.execute_batch(params, request_batch)
-                if rs:
-                    success = 0
-                    failure = 0
-                    for status in rs:
-                        if 'result' in status:
-                            if status['result'] == 'success':
-                                success += 1
-                            else:
-                                failure += 1
-                    if success or failure:
-                        logging.info('Team approval: success %s; failure %s', success, failure)
-                api.query_enterprise(params)
-
-        request_batch.clear()
-        if approve_users and 'queued_team_users' in params.enterprise and \
-                'teams' in params.enterprise and 'users' in params.enterprise:
-            active_users = {}
-            for u in params.enterprise['users']:
-                if u['status'] == 'active' and u['lock'] == 0:
-                    active_users[u['enterprise_user_id']] = u['username']
-
-            teams = {}
-            for t in params.enterprise['teams']:
-                teams[t['team_uid']] = t
-
-            for qtu in params.enterprise['queued_team_users']:
-                team_uid = qtu['team_uid']
-                if team_uid in teams:
-                    if 'users' in qtu:
-                        for u_id in qtu['users']:
-                            if u_id not in active_users:
-                                continue
-                            rq = {
-                                'command': 'team_enterprise_user_add',
-                                'team_uid': team_uid,
-                                'enterprise_user_id': u_id,
-                            }
-                            team_key = self.get_team_key(params, team_uid)
-                            public_key = self.get_public_key(params, active_users[u_id])
-                            if team_key and public_key:
-                                rq['team_key'] = api.encrypt_rsa(team_key, public_key)
-                                rq['user_type'] = 0
-                                request_batch.append(rq)
-            if request_batch:
-                rs = api.execute_batch(params, request_batch)
-                if rs:
-                    success = 0
-                    failure = 0
-                    for status in rs:
-                        if 'result' in status:
-                            if status['result'] == 'success':
-                                success += 1
-                            else:
-                                failure += 1
-                    if success or failure:
-                        logging.info('Team User approval: success %s; failure %s', success, failure)
-                api.query_enterprise(params)
-
-
-class DeviceApproveCommand(EnterpriseCommand):
-    def get_parser(self):
-        return device_approve_parser
-
-    DevicesToApprove = None
-
-    @staticmethod
-    def token_to_string(token): # type: (bytes) -> str
-        src = token[0:10]
-        if src.hex:
-            return src.hex()
-        return ''.join('{:02x}'.format(x) for x in src)
-
-    def execute(self, params, **kwargs):
-        try:
-            from cryptography.hazmat.backends import default_backend
-            from cryptography.hazmat.primitives.asymmetric import ec
-            from cryptography.hazmat.primitives.kdf.hkdf import HKDF
-            from cryptography.hazmat.primitives import hashes
-            from cryptography.hazmat.primitives import serialization
-        except:
-            print('To use this feature, install cryptography package\n' + bcolors.OKGREEN + '\'pip install cryptography\'' + bcolors.ENDC)
-            return
-
-        if DeviceApproveCommand.DevicesToApprove is None or kwargs.get('reload'):
-            request = {
-                'command': 'get_enterprise_data',
-                'include': ['devices_request_for_admin_approval']
-            }
-            response = api.communicate(params, request)
-            DeviceApproveCommand.DevicesToApprove = response.get('devices_request_for_admin_approval') or []
-        if not DeviceApproveCommand.DevicesToApprove:
-            logging.info('There are no pending devices to approve')
-            return
-
-        if kwargs.get('approve') and kwargs.get('deny'):
-            raise CommandError('device-approve', "'approve' and 'deny' parameters are mutually exclusive.")
-
-        devices = kwargs['device']
-        matching_devices = {}
-        for device in DeviceApproveCommand.DevicesToApprove:
-            device_id = device.get('encrypted_device_token')
-            if not device_id:
-                continue
-            device_id = DeviceApproveCommand.token_to_string(base64.urlsafe_b64decode(device_id + '=='))
-            found = False
-            if devices:
-                for name in devices:
-                    if name:
-                        if device_id.startswith(name):
-                            found = True
-                            break
-                        ent_user_id = device.get('enterprise_user_id')
-                        u = next((x for x in params.enterprise['users'] if x.get('enterprise_user_id') == ent_user_id), None)
-                        if u:
-                            if u.get('username') == name:
-                                found = True
-                                break
-                    else:
-                        found = True
-            else:
-                found = True
-            if found:
-                matching_devices[device_id] = device
-
-        if len(matching_devices) == 0:
-            logging.info('No matching devices found')
-            return
-
-        if kwargs.get('approve') and kwargs.get('check_ip'):
-            user_ids = set([x['enterprise_user_id'] for x in matching_devices.values() if 'enterprise_user_id' in x])
-            emails = {}
-            for u in params.enterprise['users']:
-                user_id = u['enterprise_user_id']
-                if user_id in user_ids:
-                    emails[user_id] = u['username']
-
-            last_year = datetime.datetime.now() - datetime.timedelta(days=365)
-            rq = {
-                'command': 'get_audit_event_reports',
-                'report_type': 'span',
-                'scope': 'enterprise',
-                'columns': ['ip_address', 'username'],
-                'filter': {
-                    'audit_event_type': 'login',
-                    'created': {
-                        "min": int(last_year.timestamp())
-                    },
-                    'username': list(emails.values())
-                },
-                'limit': 1000
-            }
-            rs = api.communicate(params, rq)
-            ip_map = {}
-            if 'audit_event_overview_report_rows' in rs:
-                for row in rs['audit_event_overview_report_rows']:
-                    if 'username' in row and 'ip_address' in row:
-                        uname = row['username']
-                        if uname not in ip_map:
-                            ip_map[uname] = set()
-                        ip_map[uname].add(row['ip_address'])
-
-            # Filter out users that tried to login from an untrusted IP
-            trusted_devices = {}    # To avoid array modification in a loop, we will store this into a separated dict
-
-            for k, v in matching_devices.items():
-                p_uname = emails.get(v.get('enterprise_user_id'))
-                p_ip_addr = v.get('ip_address')
-                keep = p_uname and p_ip_addr and p_uname in ip_map and p_ip_addr in ip_map[p_uname]
-                if keep:
-                    trusted_devices[k] = v
-                else:
-                    logging.warning("The user %s attempted to login from an unstrusted IP (%s). To force the approval, run the same command without the --trusted-ip argument", p_uname, p_ip_addr)
-
-            matching_devices = trusted_devices
-
-        if len(matching_devices) == 0:
-            logging.info('No matching devices found')
-            return
-
-        if kwargs.get('approve') or kwargs.get('deny'):
-            approve_rq = ApproveUserDevicesRequest()
-            data_keys = {}
-            if kwargs.get('approve'):
-
-                # resolve user data keys shared with enterprise
-                user_ids = set([x['enterprise_user_id'] for x in matching_devices.values()])
-                user_ids.difference_update(data_keys.keys())
-                if len(user_ids) > 0:
-                    ecc_private_key = None
-                    curve = ec.SECP256R1()
-                    if 'keys' in params.enterprise:
-                        if 'ecc_encrypted_private_key' in params.enterprise['keys']:
-                            keys = params.enterprise['keys']
-                            try:
-                                ecc_private_key_data = base64.urlsafe_b64decode(keys['ecc_encrypted_private_key'] + '==')
-                                ecc_private_key_data = rest_api.decrypt_aes(ecc_private_key_data, params.enterprise['unencrypted_tree_key'])
-                                private_value = int.from_bytes(ecc_private_key_data, byteorder='big', signed=False)
-                                ecc_private_key = ec.derive_private_key(private_value, curve, default_backend())
-                            except Exception as e:
-                                logging.debug(e)
-
-                    if ecc_private_key:
-                        data_key_rq = UserDataKeyRequest()
-                        data_key_rq.enterpriseUserId.extend(user_ids)
-                        api_request_payload = ApiRequestPayload()
-                        api_request_payload.payload = data_key_rq.SerializeToString()
-                        api_request_payload.encryptedSessionToken = base64.urlsafe_b64decode(params.session_token + '==')
-                        rs = api.rest_api.execute_rest(params.rest_context, 'enterprise/get_enterprise_user_data_key', api_request_payload)
-                        if type(rs) is bytes:
-                            data_key_rs = EnterpriseUserDataKeys()
-                            data_key_rs.ParseFromString(rs)
-                            for key in data_key_rs.keys:
-                                enc_data_key = key.userEncryptedDataKey
-                                if enc_data_key:
-                                    try:
-                                        ephemeral_public_key = ec.EllipticCurvePublicKey.from_encoded_point(curve, enc_data_key[:65])
-                                        shared_key = ecc_private_key.exchange(ec.ECDH(), ephemeral_public_key)
-                                        digest = hashes.Hash(hashes.SHA256(), backend=default_backend())
-                                        digest.update(shared_key)
-                                        enc_key = digest.finalize()
-                                        data_key = rest_api.decrypt_aes(enc_data_key[65:], enc_key)
-                                        data_keys[key.enterpriseUserId] = data_key
-                                    except Exception as e:
-                                        logging.debug(e)
-
-                # resolve user data keys from Account Transfer
-                user_ids = set([x['enterprise_user_id'] for x in matching_devices.values()])
-                user_ids.difference_update(data_keys.keys())
-                if len(user_ids) > 0:
-                    data_key_rq = UserDataKeyRequest()
-                    data_key_rq.enterpriseUserId.extend(user_ids)
-                    api_request_payload = ApiRequestPayload()
-                    api_request_payload.payload = data_key_rq.SerializeToString()
-                    api_request_payload.encryptedSessionToken = base64.urlsafe_b64decode(params.session_token + '==')
-                    rs = api.rest_api.execute_rest(params.rest_context, 'enterprise/get_user_data_key_shared_to_enterprise', api_request_payload)
-                    if type(rs) is bytes:
-                        data_key_rs = UserDataKeyResponse()
-                        data_key_rs.ParseFromString(rs)
-                        if data_key_rs.noEncryptedDataKey:
-                            user_ids = set(data_key_rs.noEncryptedDataKey)
-                            usernames = [x['username'] for x in params.enterprise['users'] if x['enterprise_user_id'] in user_ids]
-                            if usernames:
-                                logging.info('User(s) \"%s\" have no accepted account transfers or did not share encryption key', ', '.join(usernames))
-                        if data_key_rs.accessDenied:
-                            user_ids = set(data_key_rs.noEncryptedDataKey)
-                            usernames = [x['username'] for x in params.enterprise['users'] if x['enterprise_user_id'] in user_ids]
-                            if usernames:
-                                logging.info('You cannot manage these user(s): %s', ', '.join(usernames))
-                        if data_key_rs.userDataKeys:
-                            for dk in data_key_rs.userDataKeys:
-                                try:
-                                    role_key = rest_api.decrypt_aes(dk.roleKey, params.enterprise['unencrypted_tree_key'])
-                                    private_key = api.decrypt_rsa_key(dk.privateKey, role_key)
-                                    for user_dk in dk.enterpriseUserIdDataKeyPairs:
-                                        if user_dk.enterpriseUserId not in data_keys:
-                                            data_key_str = base64.urlsafe_b64encode(user_dk.encryptedDataKey).strip(b'=').decode()
-                                            data_key = api.decrypt_rsa(data_key_str, private_key)
-                                            data_keys[user_dk.enterpriseUserId] = data_key
-                                except Exception as ex:
-                                    logging.debug(ex)
-                    else:
-                        logging.warning(rs)
-
-            for device in matching_devices.values():
-                ent_user_id = device['enterprise_user_id']
-                device_rq = ApproveUserDeviceRequest()
-                device_rq.enterpriseUserId = ent_user_id
-                device_rq.encryptedDeviceToken = base64.urlsafe_b64decode(device['encrypted_device_token'] + '==')
-                device_rq.denyApproval = True if kwargs.get('deny') else False
-                if kwargs.get('approve'):
-                    public_key = device['device_public_key']
-                    if not public_key or len(public_key) == 0:
-                        continue
-                    data_key = data_keys.get(ent_user_id)
-                    if not data_key:
-                        continue
-                    try:
-                        curve = ec.SECP256R1()
-                        ephemeral_key = ec.generate_private_key(curve,  default_backend())
-                        device_public_key = ec.EllipticCurvePublicKey. \
-                            from_encoded_point(curve, base64.urlsafe_b64decode(device['device_public_key'] + '=='))
-                        shared_key = ephemeral_key.exchange(ec.ECDH(), device_public_key)
-                        digest = hashes.Hash(hashes.SHA256(), backend=default_backend())
-                        digest.update(shared_key)
-                        enc_key = digest.finalize()
-                        encrypted_data_key = rest_api.encrypt_aes(data_key, enc_key)
-                        eph_public_key = ephemeral_key.public_key().public_bytes(
-                            serialization.Encoding.X962, serialization.PublicFormat.UncompressedPoint)
-                        device_rq.encryptedDeviceDataKey = eph_public_key + encrypted_data_key
-                    except Exception as e:
-                        logging.info(e)
-                        return
-                approve_rq.deviceRequests.append(device_rq)
-
-            if len(approve_rq.deviceRequests) == 0:
-                return
-
-            api_request_payload = ApiRequestPayload()
-            api_request_payload.payload = approve_rq.SerializeToString()
-            api_request_payload.encryptedSessionToken = base64.urlsafe_b64decode(params.session_token + '==')
-            rs = api.rest_api.execute_rest(params.rest_context, 'enterprise/approve_user_devices', api_request_payload)
-            if type(rs) is bytes:
-                approve_rs = ApproveUserDevicesResponse()
-                approve_rs.ParseFromString(rs)
-                DeviceApproveCommand.DevicesToApprove = None
-            else:
-                logging.warning(rs)
-        else:
-            print('')
-            headers = [
-                'Date',
-                'Email',
-                'Device ID',
-                'Device Name',
-                'Device Type',
-                'IP Address',
-                'Client Version',
-                'Location']
-
-            if kwargs.get('format') == 'json':
-                headers = [x.replace(' ', '_').lower() for x in headers]
-
-            rows = []
-            for k, v in matching_devices.items():
-                user = next((x for x in params.enterprise['users']
-                             if x.get('enterprise_user_id') == v.get('enterprise_user_id')), None)
-                if not user:
-                    continue
-
-                date_formatted = time.strftime('%Y-%m-%d %H:%M:%S', time.gmtime(v.get('date')/1000.0))
-
-                rows.append([
-                    date_formatted,
-                    user.get('username'),
-                    k,
-                    v.get('device_name'),
-                    v.get('device_type'),
-                    v.get('ip_address'),
-                    v.get('client_version'),
-                    v.get('location')
-                ])
-            rows.sort(key=lambda x: x[0])
-            dump_report_data(rows, headers, fmt=kwargs.get('format'), filename=kwargs.get('output'))
-            print('')
-
-
-scim_description = '''
-SCIM Command Syntax Description:
-scim command [target] [--options]
- Command            Description
-=================================================================
- list               Displays the list of SCIM endpoints
- create             Creates SCIM endpoint
- view               Prints SCIM endpoint details
- edit               Changes SCIM endpoint configuration
- delete             Deletes SCIM endpoint
- 
-  list, create
- 'target' parameter is ignored 
- 
-view, edit, delete
- these commands require 'target' parameter: SCIM endpoint ID
- 
- Option             Commands
-=================================================================
- --reload           all : Reloads SCIM configuration
- --node             create : Node ID or Name 
- --prefix           create, edit : Role prefix
- --unique-groups    create, edit : Unique groups 
- --force            delete : Do not ask for delete confirmation
-'''
-
-
-class EnterpriseScimCommand(EnterpriseCommand):
-    def get_parser(self):  # type: () -> argparse.ArgumentParser or None
-        return scim_parser
-
-    def execute(self, params, **kwargs):  # type: (KeeperParams, **any) -> any
-        if kwargs.get('reload'):
-            api.query_enterprise(params)
-
-        command = kwargs.get('command') or ''
-        if command == 'list' or command == '':
-            if command == '':
-                logging.info(scim_description)
-
-            self.dump_scims(params)
-            return
-
-        if command == 'create':
-            node_name = kwargs.get('node')
-            if not node_name:
-                logging.warning('\"--node\" option is required for \"create\" command')
-                return
-            nodes = list(self.resolve_nodes(params, node_name))
-            if len(nodes) > 1:
-                logging.warning('Node name \'%s\' is not unique. Use Node ID.', node_name)
-                return
-            elif len(nodes) == 0:
-                logging.warning('Node name \'%s\' is not found', node_name)
-                return
-
-            matched_node = nodes[0]
-            if not matched_node.get('parent_id'):
-                logging.warning('Root node cannot be used for SCIM endpoint')
-                return
-            token = base64.urlsafe_b64encode(os.urandom(32)).decode().rstrip('=')
-            rq = {
-                'command': 'scim_add',
-                'scim_id': self.get_enterprise_id(params),
-                'node_id': matched_node['node_id'],
-                'token': token,
-            }
-            prefix = kwargs.get('prefix')
-            if prefix:
-                rq['prefix'] = prefix
-            if kwargs.get('unique_groups'):
-                rq['unique_groups'] = True
-
-            api.communicate(params, rq)
-            api.query_enterprise(params)
-            logging.info('')
-            logging.info('SCIM ID: %d', rq['scim_id'])
-            logging.info('SCIM URL: %s', self.get_scim_url(params, matched_node['node_id']))
-            logging.info('Provisioning Token: %s', token)
-            logging.info('')
-            return token
-
-        target = kwargs.get('target')
-        if not target:
-            logging.warning('\"target\" parameter is required for \"%s\" command', command)
-            return
-        scims = []
-        if params.enterprise and 'scims' in params.enterprise:
-            try:
-                target_id = int(target)
-            except ValueError:
-                logging.warning('SCIM ID should be integer: %s', target)
-                return
-            for info in params.enterprise['scims']:
-                if target_id == info['scim_id'] or target_id == info['node_id']:
-                    scims.append(info)
-                    break
-        if len(scims) == 0:
-            logging.warning('SCIM endpoint with ID \"%d\" not found', target)
-            return
-        scim = scims[0]
-
-        if command == 'edit':
-            token = base64.urlsafe_b64encode(os.urandom(32)).decode().rstrip('=')
-            rq = {
-                'command': 'scim_update',
-                'scim_id': scim['scim_id'],
-                'token': token,
-            }
-            prefix = kwargs.get('prefix')
-            if prefix:
-                rq['prefix'] = prefix
-            if kwargs.get('unique_groups'):
-                rq['unique_groups'] = True
-
-            api.communicate(params, rq)
-            api.query_enterprise(params)
-            logging.info('')
-            logging.info('SCIM ID: %d', scim['scim_id'])
-            logging.info('SCIM URL: %s', self.get_scim_url(params, scim['node_id']))
-            logging.info('Provisioning Token: %s', token)
-            logging.info('')
-            return token
-
-        if command == 'view':
-            logging.info('{0:>20s}: {1}'.format('SCIM ID', scim['scim_id']))
-            node_id = scim['node_id']
-            logging.info('{0:>20s}: {1}'.format('SCIM URL', self.get_scim_url(params, node_id)))
-            logging.info('{0:>20s}: {1}'.format('Node ID', node_id))
-            logging.info('{0:>20s}: {1}'.format('Node Name', EnterpriseCommand.get_node_path(params, node_id)))
-            logging.info('{0:>20s}: {1}'.format('Prefix', scim.get('role_prefix') or ''))
-            logging.info('{0:>20s}: {1}'.format('Status', scim['status']))
-            last_synced = scim.get('last_synced')
-            if last_synced:
-                logging.info('{0:>20s}: {1}'.format('Last Synced', time.localtime(last_synced)))
-
-        elif command == 'delete':
-            answer = 'y' if kwargs.get('force') else \
-                user_choice(bcolors.FAIL + bcolors.BOLD + '\nALERT!\n' + bcolors.ENDC +
-                            'You are about to delete SCIM endpoint {0}'.format(scim['scim_id']) +
-                            '\n\nDo you want to proceed with deletion?', 'yn', 'n')
-            if answer.lower() != 'y':
-                return
-
-            rq = {
-                'command': 'scim_delete',
-                'scim_id': scim['scim_id'],
-            }
-            api.communicate(params, rq)
-            api.query_enterprise(params)
-            logging.warning('SCIM endpoint \"%d\" at node \"%d\" deleted', scim['scim_id'], scim['node_id'])
-        else:
-            logging.warning('Unsupported command \"%s\"', command)
-
-
-    @staticmethod
-    def get_scim_url(params, node_id):  # type:  (KeeperParams, int) -> any
-        p = urlparse(params.rest_context.server_base)
-        return urlunparse((p.scheme, p.netloc, '/api/rest/scim/v2/' + str(node_id), None, None, None))
-
-    @staticmethod
-    def dump_scims(params):    # type: (KeeperParams) -> None
-        table = []
-        headers = ['SCIM ID', 'Node Name', 'Node ID', 'Prefix', 'Status', 'Last Synced']
-        if params.enterprise and 'scims' in params.enterprise:
-            for info in params.enterprise['scims']:
-                node_id = info['node_id']
-                last_synced = info.get('last_synced')
-                if last_synced:
-                    last_synced = str(time.localtime(last_synced))
-                else:
-                    last_synced = ''
-                row = [info['scim_id'], EnterpriseCommand.get_node_path(params, node_id), node_id,
-                       info.get('role_prefix') or '', info['status'], last_synced]
-                table.append(row)
-        dump_report_data(table, headers=headers)
```

### Comparing `keepercommander-4.88/keepercommander/commands/folder.py` & `keepercommander-4.9/keepercommander/commands/folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,30 +6,27 @@
 #
 # Keeper Commander
 # Copyright 2018 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import argparse
-import collections
 import re
 import fnmatch
 import shutil
 import functools
 import os
 import json
-
+import logging
 
 from .. import api, display
 from ..subfolder import BaseFolderNode, try_resolve_path, find_folders
 from ..record import Record
 from .base import user_choice, suppress_exit, raise_parse_exception, Command
 from ..params import LAST_SHARED_FOLDER_UID, LAST_FOLDER_UID
-from ..error import CommandError
-
 
 def register_commands(commands):
     commands['ls'] = FolderListCommand()
     commands['cd'] = FolderCdCommand()
     commands['tree'] = FolderTreeCommand()
     commands['mkdir'] = FolderMakeCommand()
     commands['rmdir'] = FolderRemoveCommand()
@@ -38,83 +35,89 @@
 
 
 def register_command_info(aliases, command_info):
     for p in [cd_parser, ls_parser, tree_parser, mkdir_parser, rmdir_parser, mv_parser, ln_parser]:
         command_info[p.prog] = p.description
 
 
-ls_parser = argparse.ArgumentParser(prog='ls', description='List folder contents.')
+ls_parser = argparse.ArgumentParser(prog='ls', description='List folder content')
 ls_parser.add_argument('-l', '--list', dest='detail', action='store_true', help='show detailed list')
 ls_parser.add_argument('-f', '--folders', dest='folders', action='store_true', help='display folders')
 ls_parser.add_argument('-r', '--records', dest='records', action='store_true', help='display records')
-ls_parser.add_argument('-v', '--verbose', dest='verbose', action='store_true', help='verbose output')
 ls_parser.add_argument('pattern', nargs='?', type=str, action='store', help='search pattern')
 ls_parser.error = raise_parse_exception
 ls_parser.exit = suppress_exit
 
 
-cd_parser = argparse.ArgumentParser(prog='cd', description='Change current folder.')
+cd_parser = argparse.ArgumentParser(prog='cd', description='Change current folder')
 cd_parser.add_argument('folder', nargs='?', type=str, action='store', help='folder path or UID')
 cd_parser.error = raise_parse_exception
 cd_parser.exit = suppress_exit
 
 
-tree_parser = argparse.ArgumentParser(prog='tree', description='Display the folder structure.')
+tree_parser = argparse.ArgumentParser(prog='tree', description='Display folder structure')
 tree_parser.add_argument('folder', nargs='?', type=str, action='store', help='folder path or UID')
 tree_parser.error = raise_parse_exception
 tree_parser.exit = suppress_exit
 
 
-rmdir_parser = argparse.ArgumentParser(prog='rmdir', description='Remove a folder and its contents.')
+rmdir_parser = argparse.ArgumentParser(prog='rmdir', description='Remove folder and its content')
 rmdir_parser.add_argument('-f', '--force', dest='force', action='store_true', help='remove folder without prompting')
 rmdir_parser.add_argument('folder', nargs='?', type=str, action='store', help='folder path or UID')
 rmdir_parser.error = raise_parse_exception
 rmdir_parser.exit = suppress_exit
 
 
-mkdir_parser = argparse.ArgumentParser(prog='mkdir', description='Create a folder.')
+mkdir_parser = argparse.ArgumentParser(prog='mkdir', description='Create folder')
 mkdir_parser.add_argument('-sf', '--shared-folder', dest='shared_folder', action='store_true', help='create shared folder')
 mkdir_parser.add_argument('-uf', '--user-folder', dest='user_folder', action='store_true', help='create user folder')
 mkdir_parser.add_argument('-a', '--all', dest='grant', action='store_true', help='anyone has all permissions by default')
 mkdir_parser.add_argument('-u', '--manage-users', dest='manage_users', action='store_true', help='anyone can manage users by default')
 mkdir_parser.add_argument('-r', '--manage-records', dest='manage_records', action='store_true', help='anyone can manage records by default')
 mkdir_parser.add_argument('-s', '--can-share', dest='can_share', action='store_true', help='anyone can share records by default')
 mkdir_parser.add_argument('-e', '--can-edit', dest='can_edit', action='store_true', help='anyone can edit records by default')
 mkdir_parser.add_argument('folder', nargs='?', type=str, action='store', help='folder path')
 mkdir_parser.error = raise_parse_exception
 mkdir_parser.exit = suppress_exit
 
 
-mv_parser = argparse.ArgumentParser(prog='mv', description='Move a record or folder to another folder.')
+mv_parser = argparse.ArgumentParser(prog='mv', description='Move record or folder')
 mv_parser.add_argument('-f', '--force', dest='force', action='store_true', help='do not prompt')
 mv_parser.add_argument('-s', '--can-reshare', dest='can_reshare', action='store_true', help='anyone can reshare records')
 mv_parser.add_argument('-e', '--can-edit', dest='can_edit', action='store_true', help='anyone can edit records')
 mv_parser.add_argument('src', nargs='?', type=str, action='store', help='source path to folder/record or UID')
 mv_parser.add_argument('dst', nargs='?', type=str, action='store', help='destination folder or UID')
 mv_parser.error = raise_parse_exception
 mv_parser.exit = suppress_exit
 
 
-ln_parser = argparse.ArgumentParser(prog='ln', description='Create a link between a record and a folder.')
+ln_parser = argparse.ArgumentParser(prog='ln', description='Create a link between record or folder')
 ln_parser.add_argument('-f', '--force', dest='force', action='store_true', help='do not prompt')
 ln_parser.add_argument('-s', '--can-reshare', dest='can_reshare', action='store_true', help='anyone can reshare records')
 ln_parser.add_argument('-e', '--can-edit', dest='can_edit', action='store_true', help='anyone can edit records')
 ln_parser.add_argument('src', nargs='?', type=str, action='store', help='source path to folder/record or UID')
 ln_parser.add_argument('dst', nargs='?', type=str, action='store', help='destination folder or UID')
 ln_parser.error = raise_parse_exception
 ln_parser.exit = suppress_exit
 
 
 class FolderListCommand(Command):
+
     @staticmethod
-    def folder_match_strings(folder):   # type: (BaseFolderNode) -> collections.Iterable[str]
+    def folder_match_strings(folder):
+        """
+        :type folder: BaseFolder
+        """
         return filter(lambda f: type(f) == str and len(f) > 0, [folder.name, folder.uid])
 
     @staticmethod
-    def record_match_strings(record):     # type: (Record) -> collections.Iterable[str]
+    def record_match_strings(record):
+        """
+        :type record: Record
+        """
         return filter(lambda f: type(f) == str and len(f) > 0, [record.title, record.record_uid, record.login, record.login_url, record.notes])
 
     @staticmethod
     def chunk_list(l, n):
         for i in range(0, len(l), n):
             yield l[i:i + n]
 
@@ -155,23 +158,23 @@
                 for uid in params.subfolder_record_cache[folder_uid]:
                     r = api.get_record(params, uid)
                     if any(filter(lambda x: regex(x) is not None, FolderListCommand.record_match_strings(r))) if regex is not None else True:
                         records.append(r)
 
         if len(folders) == 0 and len(records) == 0:
             if pattern:
-                raise CommandError('ls', '{0}: No such folder or record'.format(pattern))
+                logging.error("ls: %s: No such folder or record", pattern)
         else:
             if show_detail:
                 if len(folders) > 0:
                     display.formatted_folders(folders)
                 if len(records) > 0:
                     if len(records) < 5:
                         api.get_record_shares(params, [x.record_uid for x in records])
-                    display.formatted_records(records, folder=folder.uid, verbose=kwargs['verbose'])
+                    display.formatted_records(records, folder=folder.uid)
             else:
                 names = []
                 for f in folders:
                     name = f.name or f.uid
                     if len(name) > 40:
                         name = name[:25] + '...' + name[-12:]
                     names.append(name + '/')
@@ -185,21 +188,22 @@
                     rnames.append(name)
                 rnames.sort()
 
                 names.extend(rnames)
 
                 width, _ = shutil.get_terminal_size(fallback=(1, 1))
                 max_name = functools.reduce(lambda val, elem: len(elem) if len(elem) > val else val, names, 0)
+                max_name = max_name
                 cols = width // max_name
                 if cols == 0:
                     cols = 1
 
-                if cols > 2:
-                    if ((max_name * cols) + (cols - 1) * 2) > width:
-                        cols = cols - 1
+                if cols > 3:
+                    max_name = max_name + 2
+                    cols = width // max_name
 
                 tbl = FolderListCommand.chunk_list([x.ljust(max_name) if cols > 1 else x for x in names], cols)
 
                 rows = ['  '.join(x) for x in tbl]
                 print('\n'.join(rows))
 
 
@@ -215,15 +219,15 @@
             else:
                 rs = try_resolve_path(params, folder_name)
                 if rs is not None:
                     folder, pattern = rs
                     if len(pattern) == 0:
                         params.current_folder = folder.uid
                     else:
-                        raise CommandError('cd', 'Folder {0} not found'.format(folder_name))
+                        logging.warning('cd: Folder %s not found', folder_name)
 
 
 class FolderTreeCommand(Command):
     def get_parser(self):
         return tree_parser
 
     def execute(self, params, **kwargs):
@@ -233,15 +237,15 @@
         else:
             rs = try_resolve_path(params, folder_name)
             if rs is not None:
                 folder, pattern = rs
                 if len(pattern) == 0:
                     display.formatted_tree(params, folder)
                 else:
-                    raise CommandError('tree', 'Folder %s not found'.format(folder_name))
+                    logging.warning('Folder %s not found', folder_name)
 
 
 class FolderMakeCommand(Command):
     def get_parser(self):
         return mkdir_parser
 
     def execute(self, params, **kwargs):
@@ -249,29 +253,31 @@
 
         name = kwargs['folder'] if 'folder' in kwargs else None
         if name:
             rs = try_resolve_path(params, name)
             if rs is not None:
                 base_folder, name = rs
                 if len(name) == 0:
-                    raise CommandError('mkdir', 'Folder "{0}" already exists'.format(kwargs['folder']))
+                    logging.warning('Folder "%s" already exists', name)
+                    return
 
         shared_folder = kwargs['shared_folder'] if 'shared_folder' in kwargs else None
         user_folder = kwargs['user_folder'] if 'user_folder' in kwargs else None
 
         request = {"command": "folder_add"}
         if shared_folder:
             if base_folder.type in {BaseFolderNode.RootFolderType, BaseFolderNode.UserFolderType}:
                 request['folder_type'] = 'shared_folder'
                 grant = kwargs['grant'] if 'grant' in kwargs else None
                 for flag in ['manage_users', 'manage_records', 'can_share', 'can_edit']:
                     if grant or (flag in kwargs and kwargs[flag]):
                         request[flag] = True
             else:
-                raise CommandError('mkdir', 'Shared folders cannot be nested')
+                logging.error('Shared folders cannot be nested')
+                return
 
         elif user_folder:
             if base_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
                 request['folder_type'] = 'shared_folder_folder'
             else:
                 request['folder_type'] = 'user_folder'
 
@@ -331,15 +337,16 @@
 
         is_slash = False
         for x in range(0, len(name)-2):
             if name[x] == '/':
                 is_slash = not is_slash
             else:
                 if is_slash:
-                    raise CommandError('mkdir', 'Character "/" is reserved. Use "//" inside folder name')
+                    logging.warning('Character "/" is reserved. Use "//" inside folder name')
+                    return
 
         name = name.replace('//', '/')
 
         if request['folder_type'] == 'shared_folder':
             request['name'] = api.encrypt_aes(name.encode('utf-8'), folder_key)
 
         data = {'name': name}
@@ -354,29 +361,30 @@
 
 class FolderRemoveCommand(Command):
     def get_parser(self):
         return rmdir_parser
 
     def execute(self, params, **kwargs):
         folder = None
-        name = kwargs['folder'] if 'folder' in kwargs else ''
+        name = kwargs['folder'] if 'folder' in kwargs else None
         if name:
             if name in params.folder_cache:
                 folder = params.folder_cache[name]
             else:
                 rs = try_resolve_path(params, name)
                 if rs is not None:
                     folder, name = rs
                     if len(name or '') > 0:
                         folder = None
                     elif folder.type == BaseFolderNode.RootFolderType:
                         folder = None
 
         if folder is None:
-            raise CommandError('rmdir', 'Enter name of the existing folder. ({0})'.format(name))
+            logging.warning('Enter name of the existing folder')
+            return
 
         force = kwargs['force'] if 'force' in kwargs else None
         parent = params.folder_cache[folder.uid] if folder.uid is not None else None
         if folder.type == BaseFolderNode.SharedFolderType:
             if folder.uid in params.shared_folder_cache:
                 sf = params.shared_folder_cache[folder.uid]
 
@@ -486,39 +494,43 @@
             if src_folder is None:
                 src_folder = params.root_folder
         elif src_path in params.folder_cache:
             src_folder = params.folder_cache[src_path]
         else:
             src = try_resolve_path(params, src_path)
             if src is None:
-                raise CommandError('mv', 'Source path should be existing record or folder')
+                logging.warning('Source path should be existing record or folder')
+                return
 
             src_folder, name = src
             if len(name) > 0:
                 src_folder_uid = src_folder.uid or ''
                 if src_folder_uid in params.subfolder_record_cache:
                     for uid in params.subfolder_record_cache[src_folder_uid]:
                         rec = api.get_record(params, uid)
                         if name in {rec.title, rec.record_uid}:
                             src_record_uid = rec.record_uid
                             break
 
                 if src_record_uid is None:
-                    raise CommandError('mv', 'Record "{0}" not found'.format(name))
+                    logging.warning('Record "%s" not found', name)
+                    return
 
         dst_folder = None
         if dst_path in params.folder_cache:
             dst_folder = params.folder_cache[dst_path]
         else:
             dst = try_resolve_path(params, dst_path)
             if dst is None:
-                raise CommandError('mv', 'Destination path should be existing folder')
+                logging.warning('Destination path should be existing folder')
+                return
             dst_folder, name = dst
             if len(name) > 0:
-                raise CommandError('mv', 'Destination path should be existing folder')
+                logging.warning('Destination path should be existing folder')
+                return
 
         rq = {
             'command': 'move',
             'link': not self.is_move(),
             'move': []
         }
         if dst_folder.type == BaseFolderNode.RootFolderType:
@@ -526,23 +538,25 @@
         else:
             rq['to_type'] = dst_folder.type
             rq['to_uid'] = dst_folder.uid
 
         if src_record_uid is None:
             ''' folder '''
             if src_folder.type == BaseFolderNode.RootFolderType:
-                raise CommandError('mv', 'Root folder cannot be a source folder')
+                logging.warning('Root folder cannot be a source folder')
+                return
             dp = set()
             f = dst_folder
             while f is not None:
                 if len(f.uid) > 0:
                     dp.add(f.uid)
                 f = params.folder_cache.get(f.parent_uid) if f.parent_uid is not None else None
             if src_folder.uid in dp:
-                raise CommandError('mv', 'Cannot move/link folder to self or a child')
+                logging.warning('Cannot move/link folder to self or a child')
+                return
 
             parent_folder = params.folder_cache[src_folder.parent_uid] if src_folder.parent_uid is not None else None
             move = {
                 'uid': src_folder.uid,
                 'type': src_folder.type,
                 'cascade': True
             }
```

### Comparing `keepercommander-4.88/keepercommander/display.py` & `keepercommander-4.9/keepercommander/display.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 import json
 
 from colorama import init
 from tabulate import tabulate
 from asciitree import LeftAligned
 from collections import OrderedDict as OD
 from .subfolder import BaseFolderNode
-from keepercommander import __version__
-from keepercommander import versioning
+
 
 init()
 
 
 class bcolors:
     HEADER = '\033[95m'
     OKBLUE = '\033[94m'
@@ -33,53 +32,45 @@
 
 def welcome():
     print('\n')
     print(bcolors.OKBLUE,' _  __  ' + bcolors.ENDC)
     print(bcolors.OKBLUE,'| |/ /___ ___ _ __  ___ _ _ ' + bcolors.ENDC)
     print(bcolors.OKBLUE,'| \' </ -_) -_) \'_ \\/ -_) \'_|' + bcolors.ENDC)
     print(bcolors.OKBLUE,'|_|\\_\\___\\___| .__/\\___|_|' + bcolors.ENDC)
-    print(bcolors.OKBLUE + ' v{0:<12}|_|'.format(__version__) + bcolors.ENDC)
+    print(bcolors.OKBLUE,'             |_|            ' + bcolors.ENDC)
+    print('')
+    print(bcolors.FAIL,'password manager & digital vault' + bcolors.ENDC)
     print('')
-    print(bcolors.FAIL, 'password manager & digital vault' + bcolors.ENDC)
     print('')
-
-    versioning.welcome_print_version()
 
 
 def formatted_records(records, **kwargs):
     """Display folders/titles/uids for the supplied shared folders"""
     params = None
     if 'params' in kwargs:
         params = kwargs['params']
 
     # Sort by folder+title
     records.sort(key=lambda x: x.title.lower(), reverse=False)
 
-    def abbreviate_text(text: str, chars_num: int):
-        if 'verbose' in kwargs and kwargs['verbose']:
-            return text
-        else:
-            return text if len(text) < chars_num else text[:chars_num] + '...'
-
-
     if len(records) > 0:
         shared_folder = None
         if 'folder' in kwargs and params is not None:
             fuid = kwargs['folder']
             if fuid in params.folder_cache:
                 folder = params.folder_cache[fuid]
                 if folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
                     if folder.type == BaseFolderNode.SharedFolderFolderType:
                         fuid = folder.shared_folder_uid
                 else:
                     fuid = None
                 if fuid and fuid in params.shared_folder_cache:
                     shared_folder = params.shared_folder_cache[fuid]
 
-        table = [[i + 1, r.record_uid, abbreviate_text(r.title, 32), r.login, abbreviate_text(r.login_url, 32)] for i, r in enumerate(records)]
+        table = [[i + 1, r.record_uid, r.title if len(r.title) < 32 else r.title[:32] + '...', r.login, r.login_url[:32]] for i, r in enumerate(records)]
         headers = ["#", 'Record UID', 'Title', 'Login', 'URL']
         if shared_folder and 'records' in shared_folder:
             headers.append('Flags')
             for row in table:
                 flag = ''
                 for sfr in shared_folder['records']:
                     if sfr['record_uid'] == row[1]:
@@ -187,57 +178,18 @@
     print('----------------')
 
     for h in history:
         print(h)
 
     print('')
 
-
 def print_record(params, record_uid):
     """ Show record content """
 
     try:
         cached_rec = params.record_cache[record_uid]
     except KeyError as e:
         raise Exception('Record not found: ' + record_uid)
-    data = json.loads(cached_rec['data_unencrypted'].decode('utf-8'))
+    data = json.loads(cached_rec['data'].decode('utf-8'))
     print(data)
 
 
-def format_msp_licenses(licenses):
-
-    print('')
-    print('MSP Plans and Licenses')
-    print('-----------------------')
-
-    if len(licenses) > 0:
-
-        for i, lic in enumerate(licenses):
-
-            if len(licenses) > 1:
-                print('License # ', i+1)
-
-            msp_license_pool = lic['msp_pool']
-
-            table = [
-                [
-                    j + 1,
-                    ml['product_id'],
-                    ml['availableSeats'],
-                    ml['seats'],
-                    ml['stash'] if 'stash' in ml else ' -'   # sometimes stash won't be returned from the backend
-                ] for j, ml in enumerate(msp_license_pool)]
-            print(tabulate(table, headers=["#", 'Plan Id', 'Available Licenses', 'Total Licenses', 'Stash']))
-            print('')
-
-
-def format_managed_company(mcs):
-
-    # Sort by title
-    mcs.sort(key=lambda x: x['mc_enterprise_name'].lower(), reverse=False)
-
-    if len(mcs) > 0:
-        table = [[i + 1, mc['mc_enterprise_id'], mc['mc_enterprise_name'], mc['product_id'], mc['number_of_seats'], mc['number_of_users']] for i, mc in enumerate(mcs)]
-        print(tabulate(table, headers=["#", 'ID', 'Name', 'Plan', 'Allocated', 'Active']))
-        print('')
-
-
```

### Comparing `keepercommander-4.88/keepercommander/error.py` & `keepercommander-4.9/keepercommander/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,13 +62,7 @@
 
     Attributes:
         message -- explanation of crypto error
     """
 
     def __init__(self, message):
         self.message = message
-
-
-class CommandError(Error):
-    def __init__(self, command, message):
-        self.command = command
-        self.message = message
```

### Comparing `keepercommander-4.88/keepercommander/generator.py` & `keepercommander-4.9/keepercommander/generator.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,40 +3,24 @@
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|            
 #
 # Keeper Commander 
 # Contact: ops@keepersecurity.com
 #
-import logging
-import os
+
 import random
 import string
 
 
 def randomSample(sampleLength=0, sampleString=''):
     sample = ''
 
-    use_secrets = False
-
-    try:
-        # Older version of Python (before 3.6) don't have this module.
-        # If not installed, fall back to the original version of the code
-        import secrets
-        logging.debug("module 'secrets' is installed")
-        use_secrets = True
-    except ModuleNotFoundError:
-        logging.warning("module 'secrets' is not installed")
-
     for i in range(sampleLength):
-        if use_secrets:
-            sample += secrets.choice(sampleString)
-        else:
-            pos = int.from_bytes(os.urandom(2), 'big') % len(sampleString)
-            sample += sampleString[pos]
+        sample += sampleString[random.randint(0,len(sampleString)-1)]
 
     return sample
 
 
 def rules(uppercase=0, lowercase=0, digits=0, special_characters=0):
     """ Generate a password of specified length with specified number of """
     """ uppercase, lowercase, digits and special characters """
```

### Comparing `keepercommander-4.88/keepercommander/importer/commands.py` & `keepercommander-4.9/keepercommander/importer/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,31 +27,28 @@
 
 
 def register_command_info(aliases, command_info):
     for p in [import_parser, export_parser]:
         command_info[p.prog] = p.description
 
 
-import_parser = argparse.ArgumentParser(prog='import', description='Import data from a local file into Keeper.')
+import_parser = argparse.ArgumentParser(prog='import', description='Import data from local file to Keeper')
 import_parser.add_argument('--display-csv', '-dc', dest='display_csv', action='store_true',  help='display Keeper CSV import instructions')
 import_parser.add_argument('--display-json', '-dj', dest='display_json', action='store_true',  help='display Keeper JSON import instructions')
-import_parser.add_argument('--format', dest='format', choices=['json', 'csv', 'keepass', 'lastpass'], required=True, help='file format')
-import_parser.add_argument('--folder', dest='folder', action='store', help='import into a separate folder.')
+import_parser.add_argument('--format', dest='format', choices=['json', 'csv', 'keepass'], required=True, help='file format')
 import_parser.add_argument('-s', '--shared', dest='shared', action='store_true', help='import folders as Keeper shared folders')
 import_parser.add_argument('-p', '--permissions', dest='permissions', action='store', help='default shared folder permissions: manage (U)sers, manage (R)ecords, can (E)dit, can (S)hare, or (A)ll, (N)one')
-import_parser.add_argument('name', type=str, help='file name (json, csv, keepass) or account name (lastpass)')
+import_parser.add_argument('filename', type=str, help='file name')
 import_parser.error = raise_parse_exception
 import_parser.exit = suppress_exit
 
 
-export_parser = argparse.ArgumentParser(prog='export', description='Export data from Keeper to a local file.')
+export_parser = argparse.ArgumentParser(prog='export', description='Export data from Keeper to local file')
 export_parser.add_argument('--format', dest='format', choices=['json', 'csv', 'keepass'], required=True, help='file format')
-export_parser.add_argument('--max-size', dest='max_size', help='Maximum file attachment file. Example: 100K, 50M, 2G. Default: 10M')
-export_parser.add_argument('-kp', '--keepass-file-password', dest='keepass_file_password', action='store', help='Password for the exported Keepass file')
-export_parser.add_argument('name', type=str, nargs='?', help='file name or console output if omitted (except keepass)')
+export_parser.add_argument('filename', type=str, nargs='?', help='file name or console output if omitted (except keepass)')
 export_parser.error = raise_parse_exception
 export_parser.exit = suppress_exit
 
 
 csv_instructions = '''CSV Import Instructions
 
 File Format:
@@ -116,22 +113,22 @@
 
 
 class RecordImportCommand(ImporterCommand):
     def get_parser(self):
         return import_parser
 
     def execute(self, params, **kwargs):
-        import_format = kwargs['format'] if 'format' in kwargs else None
-        import_name = kwargs['name'] if 'name' in kwargs else None
+        file_format = kwargs['format'] if 'format' in kwargs else None
+        filename = kwargs['filename'] if 'filename' in kwargs else None
         shared = kwargs.get('shared') or False
         manage_users = False
         manage_records = False
         can_edit = False
         can_share = False
-        if import_format and import_name:
+        if file_format and filename:
             permissions = kwargs.get('permissions')
             if shared and not permissions:
                 permissions = user_choice('Default shared folder permissions: manage (U)sers, manage (R)ecords, can (E)dit, can (S)hare, or (A)ll, (N)one', 'uresan', show_choice=False, multi_choice=True)
             if permissions:
                 chars = set()
                 chars.update([x for x in permissions.lower()])
                 if 'a' in chars:
@@ -146,70 +143,26 @@
                         manage_records = True
                     if 'e' in chars:
                         can_edit = True
                     if 's' in chars:
                         can_share = True
 
             logging.info('Processing... please wait.')
-            imp_exp._import(params, import_format, import_name, shared=shared, import_into=kwargs.get('folder'),
+            imp_exp._import(params, file_format, filename, shared=shared,
                             manage_users=manage_users, manage_records=manage_records,
                             can_edit=can_edit, can_share=can_share)
         else:
             logging.error('Missing argument')
 
 
 class RecordExportCommand(ImporterCommand):
     def get_parser(self):
         return export_parser
 
     def execute(self, params, **kwargs):
-
-        if is_export_restricted(params):
-            logging.warning('Permissions Required: `export` command is disabled. Please contact your enterprise administrator.')
-            return
-
-        export_format = kwargs['format'] if 'format' in kwargs else None
-        export_name = kwargs['name'] if 'name' in kwargs else None
-
-        extra = {}
-        if kwargs.get('keepass_file_password'):
-            extra['keepass_file_password'] = kwargs.get('keepass_file_password')
-
+        file_format = kwargs['format'] if 'format' in kwargs else None
+        filename = kwargs['filename'] if 'filename' in kwargs else None
         if format:
             logging.info('Processing... please wait.')
-            msize = kwargs.get('max_size')    # type: str
-            if msize:
-                multiplier = 1
-                scale = msize[-1].upper()
-                if scale == 'K':
-                    multiplier = 1024
-                elif scale == 'M':
-                    multiplier = 1024 ** 2
-                elif scale == 'G':
-                    multiplier = 1024 ** 3
-
-                if multiplier != 1:
-                    msize = msize[:-1]
-                try:
-                    max_size = int(msize) * multiplier
-                    extra['max_size'] = max_size
-                except ValueError:
-                    logging.error('Invalid maximum attachment file size parameter: %s', kwargs.get('max_size'))
-                    return
-
-            imp_exp.export(params, export_format, export_name, **extra)
+            imp_exp.export(params, file_format, filename)
         else:
             logging.error('Missing argument')
-
-
-def is_export_restricted(params):
-    is_export_restricted = False
-
-    booleans = params.enforcements['booleans'] if params.enforcements and 'booleans' in params.enforcements else []
-
-    if len(booleans) > 0:
-        restrict_export_boolean = next((s for s in booleans if s['key'] == 'restrict_export'), None)
-
-        if restrict_export_boolean:
-            is_export_restricted = restrict_export_boolean['value']
-
-    return is_export_restricted
```

### Comparing `keepercommander-4.88/keepercommander/importer/csv/csv.py` & `keepercommander-4.9/keepercommander/importer/csv/csv.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 # Copyright 2018 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import csv
 import sys
 
-from ..importer import BaseFileImporter, BaseExporter, Record, Folder
+from ..importer import BaseImporter, BaseExporter, Record, Folder
 
 
 '''
 0 - folder
 1 - title
 2 - login
 3 - password
 4 - url
 5 - notes
 6 - shared folder
 7 + custom fields
 '''
 
 
-class KeeperCsvImporter(BaseFileImporter):
+class KeeperCsvImporter(BaseImporter):
 
     def do_import(self, filename):
-        with open(filename, "r", encoding='utf-8-sig') as csvfile:
+        with open(filename, "r", encoding='utf-8') as csvfile:
             reader = csv.reader(csvfile)
             for row in reader:
                 if len(row) >= 6:
                     record = Record()
                     record.title = (row[1] or '').strip()
                     record.login = (row[2] or '').strip()
                     record.password = (row[3] or '').strip()
@@ -70,16 +70,16 @@
 
     def extension(self):
         return 'csv'
 
 
 class KeeperCsvExporter(BaseExporter):
 
-    def do_export(self, filename, records, file_password):
-        csvfile = open(filename, 'w', encoding='utf-8', newline='') if filename else sys.stdout
+    def do_export(self, filename, records):
+        csvfile = open(filename, 'w', encoding='utf-8') if filename else sys.stdout
         writer = csv.writer(csvfile)
         for r in records:
             if type(r) == Record:
                 domain = ''
                 path = ''
                 if r.folders:
                     for folder in r.folders:
@@ -87,15 +87,15 @@
                         path = folder.path or ''
                         if domain:
                             if folder.can_edit:
                                 domain = domain + '#edit'
                             if folder.can_share:
                                 domain = domain + '#reshare'
                         break
-                row = [path, r.title or '', r.login or '', r.password or '', r.login_url or '', r.notes or '', domain, r.uid]
+                row = [path, r.title or '', r.login or '', r.password or '', r.login_url or '', r.notes or '', domain]
                 if r.custom_fields:
                     for cf in r.custom_fields:
                         row.append(cf)
                         row.append(r.custom_fields[cf])
                 writer.writerow(row)
         if filename:
             csvfile.flush()
```

### Comparing `keepercommander-4.88/keepercommander/importer/imp_exp.py` & `keepercommander-4.9/keepercommander/importer/imp_exp.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,32 +11,27 @@
 
 import os
 import json
 import hashlib
 import base64
 import requests
 import io
-import re
 import logging
 
 from contextlib import contextmanager
+from email.utils import parseaddr
+from Cryptodome.PublicKey import RSA
 from Cryptodome.Cipher import AES
 
 from keepercommander import api
-from ..params import KeeperParams
 
 from .importer import importer_for_format, exporter_for_format, path_components, PathDelimiter, BaseExporter, \
-    Record as ImportRecord, Folder as ImportFolder, SharedFolder as ImportSharedFolder,  Permission as ImportPermission,\
-    Attachment as ImportAttachment, BaseImporter
+    Record as ImportRecord, Folder as ImportFolder, SharedFolder as ImportSharedFolder, Permission as ImportPermission,\
+    Attachment as ImportAttachment
 from ..subfolder import BaseFolderNode, find_folders
-from .. import folder_pb2
-from ..record import Record
-
-TWO_FACTOR_CODE = 'TFC:Keeper'
-EMAIL_PATTERN = r"(^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$)"
 
 
 def get_import_folder(params, folder_uid, record_uid):
     folder = ImportFolder()
 
     uid = folder_uid
     is_path = True
@@ -87,21 +82,18 @@
         uid = f.parent_uid
         if not uid:
             break
 
     return path
 
 
-def export(params, file_format, filename, **export_args):
+def export(params, file_format, filename):
     api.sync_down(params)
 
     exporter = exporter_for_format(file_format)()  # type: BaseExporter
-    if export_args:
-        if 'max_size' in export_args:
-            exporter.max_size = int(export_args['max_size'])
 
     to_export = []
     if exporter.has_shared_folders():
         shfolders = [api.get_shared_folder(params, sf_uid) for sf_uid in params.shared_folder_cache]
         shfolders.sort(key=lambda x: x.name.lower(), reverse=False)
         for f in shfolders:
             fol = ImportSharedFolder()
@@ -143,17 +135,14 @@
         rec.login_url = r.login_url.strip('\x00') if r.login_url else ''
         rec.notes = r.notes.strip('\x00') if r.notes else ''
         for cf in r.custom_fields:
             name = cf.get('name')
             value = cf.get('value')
             if name and value:
                 rec.custom_fields[name] = value
-        if r.totp:
-            rec.custom_fields[TWO_FACTOR_CODE] = r.totp
-
         for folder_uid in find_folders(params, r.record_uid):
             if folder_uid in params.folder_cache:
                 folder = get_import_folder(params, folder_uid, r.record_uid)
                 if rec.folders is None:
                     rec.folders = []
                 rec.folders.append(folder)
         if exporter.has_attachments() and r.attachments:
@@ -175,69 +164,49 @@
                 atta.mime = a.get('type') or ''
                 rec.attachments.append(atta)
 
         to_export.append(rec)
     rec_count = len(to_export) - sf_count
 
     if len(to_export) > 0:
-        file_password = export_args.get('keepass_file_password') if export_args else None
-        exporter.execute(filename, to_export, file_password)
-        params.queue_audit_event('exported_records', file_format=file_format)
+        exporter.execute(filename, to_export)
         logging.info('%d records exported', rec_count)
 
 
 def _import(params, file_format, filename, **kwargs):
     api.sync_down(params)
 
     shared = kwargs.get('shared') or False
-    import_into = kwargs.get('import_into') or ''
-    if import_into:
-        import_into = import_into.replace(PathDelimiter, 2*PathDelimiter)
 
     importer = importer_for_format(file_format)()
-    # type: BaseImporter
+    """:type : BaseImporter"""
 
     records_before = len(params.record_cache)
 
     folders = []  # type: [ImportSharedFolder]
     records = []  # type: [ImportRecord]
     for x in importer.execute(filename):
         if type(x) is ImportRecord:
-            if shared or import_into:
-                if not x.folders:
-                    x.folders = [ImportFolder()]
-                for f in x.folders:
-                    if shared:
+            if shared:
+                if x.folders:
+                    for f in x.folders:
                         d_comps = list(path_components(f.domain)) if f.domain else []
                         p_comps = list(path_components(f.path)) if f.path else []
                         if len(d_comps) > 0:
                             f.domain = d_comps[0]
                             p_comps[0:0] = d_comps[1:]
                         elif len(p_comps) > 0:
                             f.domain = p_comps[0]
                             p_comps = p_comps[1:]
                         f.path = PathDelimiter.join([x.replace(PathDelimiter, 2*PathDelimiter) for x in p_comps])
-                    if import_into:
-                        if f.domain:
-                            f.domain = PathDelimiter.join([import_into, f.domain])
-                        elif f.path:
-                            f.path = PathDelimiter.join([import_into, f.path])
-                        else:
-                            f.path = import_into
 
-            x.validate()
             records.append(x)
         elif type(x) is ImportSharedFolder:
             if shared:
                 continue
-            x.validate()
-            if import_into:
-                if x.path:
-                    x.path = PathDelimiter.join([import_into, x.path])
-
             folders.append(x)
 
     if shared:
         manage_users = kwargs.get('manage_users') or False
         manage_records = kwargs.get('manage_records') or False
         can_edit = kwargs.get('can_edit') or False
         can_share = kwargs.get('can_share') or False
@@ -253,88 +222,55 @@
             sf.path = x
             sf.manage_users = manage_users
             sf.manage_records = manage_records
             sf.can_edit = can_edit
             sf.can_share = can_share
             folders.append(sf)
 
-    folder_add = prepare_folder_add(params, folders, records)
-    if folder_add:
-        fol_rs, _ = execute_import_folder_record(params, folder_add, None)
+    if folders:
+        shared_folder_add = prepare_shared_folder_add(params, folders)
+        api.execute_batch(params, shared_folder_add)
         api.sync_down(params)
 
-    if folders:
-        permissions = prepare_folder_permission(params, folders)
-        if permissions:
-            api.execute_batch(params, permissions)
-            api.sync_down(params)
-
-    if records:        # create records
-        record_add = prepare_record_add(params, records)
-        if record_add:
-            _, rec_rs = execute_import_folder_record(params, None, record_add)
-            api.sync_down(params)
+    if records:
+        # create folders
+        folder_add = prepare_folder_add(params, records)
+        api.execute_batch(params, folder_add)
+        api.sync_down(params)
+
+        # create records
+        record_adds = prepare_record_add(params, records)
+        api.execute_batch(params, record_adds)
+        api.sync_down(params)
 
         # ensure records are linked to folders
         record_links = prepare_record_link(params, records)
-        if record_links:
-            api.execute_batch(params, record_links)
-            api.sync_down(params)
+        api.execute_batch(params, record_links)
+        api.sync_down(params)
 
         # adjust shared folder permissions
         shared_update = prepare_record_permission(params, records)
-        if shared_update:
-            api.execute_batch(params, shared_update)
-            api.sync_down(params)
+        api.execute_batch(params, shared_update)
+        api.sync_down(params)
 
         # upload attachments
         atts = []
         for r in records:
             if r.attachments:
                 r_uid = r.uid
                 for a in r.attachments:
                     atts.append((r_uid, a))
         if len(atts) > 0:
             upload_attachment(params, atts)
 
     records_after = len(params.record_cache)
     if records_after > records_before:
-        params.queue_audit_event('imported_records', file_format=file_format.upper())
         logging.info("%d records imported successfully", records_after - records_before)
 
 
-def execute_import_folder_record(params, folders, records):
-    rs_folder = []
-    rs_record = []
-    while folders or records:
-        rq = folder_pb2.ImportFolderRecordRequest()
-        cap = 999
-        if folders:
-            chunk = folders[:cap]
-            folders = folders[cap:]
-            cap = cap - len(folders)
-            for e in chunk:
-                rq.folderRequest.append(e)
-        if records and cap > 0:
-            chunk = records[:cap]
-            records = records[cap:]
-            for e in chunk:
-                rq.recordRequest.append(e)
-
-        rs = api.communicate_rest(params, rq, "folder/import_folders_and_records")
-        import_rs = folder_pb2.ImportFolderRecordResponse()
-        import_rs.ParseFromString(rs)
-        if len(import_rs.folderResponse) > 0:
-            rs_folder.extend(import_rs.folderResponse)
-        if len(import_rs.recordResponse) > 0:
-            rs_record.extend(import_rs.recordResponse)
-
-    return rs_folder, rs_record
-
-
 def upload_attachment(params, attachments):
     '''
     :param attachments:
     :type attachments: [(str, ImportAttachment)]
     '''
 
     print('Uploading attachments:')
@@ -356,15 +292,15 @@
             'file_count': file_no
         }
         try:
             rs = api.communicate(params, rq)
             if rs['result'] == 'success':
                 uploads = rs['file_uploads']
         except Exception as e:
-            logging.error(e)
+            print(e)
             return
 
         uploaded = {}
         for record_id, atta in chunk:
             if not uploads:
                 break
 
@@ -409,15 +345,15 @@
                             'size': size
                         })
                         print('Done')
                     else:
                         print('Failed')
 
             except Exception as e:
-                logging.warning(e)
+                pass
 
         if len(uploaded) > 0:
             rq = {
                 'command': 'record_update',
                 'pt': 'Commander',
                 'device_id': 'Commander',
                 'client_time': api.current_milli_time(),
@@ -455,468 +391,392 @@
                     }
                     api.resolve_record_access_path(params, record_id, path=ru)
                     rq['update_records'].append(ru)
             try:
                 rs = api.communicate(params, rq)
                 if rs['result'] == 'success':
                     api.sync_down(params)
-            except Exception as e:
-                logging.debug(e)
+
+            except:
+                pass
 
 
-def prepare_folder_add(params, folders, records):
+def prepare_shared_folder_add(params, folders):
     folder_hash = {}
     for f_uid in params.folder_cache:
         fol = params.folder_cache[f_uid]
         h = hashlib.md5()
         hs = '{0}|{1}'.format((fol.name or '').lower(), fol.parent_uid or '')
         h.update(hs.encode())
         shared_folder_key = None
         if fol.type in { BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
             sf_uid = fol.shared_folder_uid if fol.type == BaseFolderNode.SharedFolderFolderType else fol.uid
             if sf_uid in params.shared_folder_cache:
                 shared_folder_key = params.shared_folder_cache[sf_uid]['shared_folder_key_unencrypted']
         folder_hash[h.hexdigest()] = f_uid, fol.type, shared_folder_key
 
-    folder_add = []      # type: [folder_pb2.FolderRequest]
-    if folders:
-        for fol in folders:
-            skip_folder = False
-            parent_uid = ''
-            comps = list(path_components(fol.path))
-            for i in range(len(comps)):
-                comp = comps[i]
-                h = hashlib.md5()
-                hs = '{0}|{1}'.format(comp.lower(), parent_uid)
-                h.update(hs.encode())
-                digest = h.hexdigest()
-
-                is_last = False
-                if i == len(comps) - 1:
-                    is_last = True
-
-                if digest not in folder_hash:
-                    folder_uid = api.generate_record_uid()
-                    folder_type = 'shared_folder' if is_last else 'user_folder'
-
-                    fol_req = folder_pb2.FolderRequest()
-                    fol_req.folderUid = base64.urlsafe_b64decode(folder_uid + '==')
-                    fol_req.folderType = 2 if folder_type == 'shared_folder' else 1
-
-                    if parent_uid:
-                        fol_req.parentFolderUid = base64.urlsafe_b64decode(parent_uid + '==')
-
-                    folder_key = os.urandom(32)
-                    fol_req.encryptedFolderKey = base64.urlsafe_b64decode(api.encrypt_aes(folder_key, params.data_key) + '==')
-
-                    data = {'name': comp}
-                    fol_req.folderData = base64.urlsafe_b64decode(api.encrypt_aes(json.dumps(data).encode('utf-8'), folder_key) + '==')
-
-                    if folder_type == 'shared_folder':
-                        fol_req.sharedFolderFields.encryptedFolderName = base64.urlsafe_b64decode(api.encrypt_aes(comp.encode('utf-8'), folder_key) + '==')
-                        fol_req.sharedFolderFields.manageUsers = fol.manage_users
-                        fol_req.sharedFolderFields.manageRecords = fol.manage_records
-                        fol_req.sharedFolderFields.canEdit = fol.can_edit
-                        fol_req.sharedFolderFields.canShare = fol.can_share
+    # public keys
+    emails = {}
+    for fol in folders:
+        if fol.permissions:
+            for perm in fol.permissions:
+                if perm.name not in emails:
+                    _, email = parseaddr(perm.name)
+                    if email:
+                        if email != params.user:
+                            emails[email.lower()] = None
+    if emails:
+        request = {
+            'command': "public_keys",
+            'key_owners': list(emails.keys())
+        }
+        try:
+            rs = api.communicate(params, request)
+            if 'public_keys' in rs:
+                for pk in rs['public_keys']:
+                    if 'public_key' in pk:
+                        emails[pk['key_owner']] = pk['public_key']
+        except Exception as e:
+            logging.debug(e)
 
-                    folder_add.append(fol_req)
-                    folder_hash[digest] = folder_uid, folder_type, folder_key if folder_type == 'shared_folder' else None
-                else:
-                    folder_uid, folder_type, folder_key = folder_hash[digest]
-                    if is_last:
-                        skip_folder = folder_type != 'shared_folder'
-                    else:
-                        skip_folder = folder_type != 'user_folder'
+    shared_folder_add = []
+    for fol in folders:
+        skip_folder = False
+        parent_uid = ''
+        parent_type = ''
+        parent_key = None
+        comps = list(path_components(fol.path))
+        for i in range(len(comps)):
+            comp = comps[i]
+            h = hashlib.md5()
+            hs = '{0}|{1}'.format(comp.lower(), parent_uid)
+            h.update(hs.encode())
+            digest = h.hexdigest()
+
+            is_last = False
+            if i == len(comps) - 1:
+                is_last = True
+            if digest not in folder_hash:
+                folder_uid = api.generate_record_uid()
+                request = {
+                    'command': 'folder_add',
+                    'folder_uid': folder_uid
+                }
+                folder_type = 'shared_folder' if is_last else 'user_folder'
+                request['folder_type'] = folder_type
+
+                encryption_key = params.data_key
+                folder_key = os.urandom(32)
+                request['key'] = api.encrypt_aes(folder_key, encryption_key)
+                if parent_uid:
+                    request['parent_uid'] = parent_uid
+                if folder_type == 'shared_folder':
+                    request['name'] = api.encrypt_aes(comp.encode('utf-8'), folder_key)
 
+                data = {'name': comp}
+                request['data'] = api.encrypt_aes(json.dumps(data).encode('utf-8'), folder_key)
+
+                shared_folder_add.append(request)
                 parent_uid = folder_uid
-                if skip_folder:
-                    break
+                parent_type = folder_type
+                parent_key = folder_key
+                folder_hash[digest] = folder_uid, folder_type, folder_key if folder_type == 'shared_folder' else None
+            else:
+                parent_uid, parent_type, parent_key = folder_hash[digest]
+                if is_last:
+                    skip_folder = parent_type != 'shared_folder'
+                else:
+                    skip_folder = parent_type != 'user_folder'
+            if skip_folder:
+                break
 
-    if records:
-        for rec in records:
-            if rec.folders:
-                for fol in rec.folders:
-                    parent_uid = ''
-                    parent_shared_folder_uid = None
-                    parent_shared_folder_key = None
-                    parent_type = ''
-                    for is_domain in [True, False]:
-                        path = fol.domain if is_domain else fol.path
-                        if not path:
-                            continue
-
-                        comps = list(path_components(path))
-                        for i in range(len(comps)):
-                            comp = comps[i]
-                            h = hashlib.md5()
-                            hs = '{0}|{1}'.format(comp.lower(), parent_uid)
-                            h.update(hs.encode())
-                            digest = h.hexdigest()
-
-                            if digest not in folder_hash:
-                                is_shared = False
-                                if i == len(comps) - 1:
-                                    is_shared = is_domain
-
-                                folder_uid = api.generate_record_uid()
-                                if not parent_type or parent_type == 'user_folder':
-                                    folder_type = 'shared_folder' if is_shared else 'user_folder'
-                                else:
-                                    folder_type = 'shared_folder_folder'
+        if not skip_folder and parent_type == 'shared_folder':
+            request = {
+                'command': 'shared_folder_update',
+                'operation': 'update',
+                'pt': 'Commander',
+                'shared_folder_uid': parent_uid,
+                'force_update': True,
+                'default_manage_users': fol.manage_users,
+                'default_manage_records': fol.manage_records,
+                'default_can_edit': fol.can_edit,
+                'default_can_share': fol.can_share
+            }
+            if fol.permissions:
+                for perm in fol.permissions:
+                    is_team = False
+                    if perm.uid and params.team_cache:
+                        is_team = perm.uid in params.team_cache
+                    else:
+                        _, email = parseaddr(perm.name)
+                        if not email:
+                            is_team = True
+                        if is_team:
+                            perm.uid = None
+                            for team in params.team_cache:
+                                if team['name'].lower() == perm.name.lower():
+                                    perm.uid = team['team_uid']
+                                    break
+                    if is_team:
+                        if perm.uid and perm.uid in params.team_cache:
+                            if 'add_teams' not in request:
+                                request['add_teams'] = []
+                            team = params.team_cache[perm.uid]
+                            request['add_teams'].append({
+                                'team_uid': perm.uid,
+                                'manage_users': perm.manage_users,
+                                'manage_records': perm.manage_records,
+                                'shared_folder_key': api.encrypt_aes(parent_key, team['team_key'])
+                            })
+                    else:
+                        if 'add_users' not in request:
+                            request['add_users'] = []
+                        email = perm.name.lower()
+                        if email == params.user.lower():
+                            request['add_users'].append({
+                                'username': email,
+                                'manage_users': perm.manage_users,
+                                'manage_records': perm.manage_records,
+                                'shared_folder_key': api.encrypt_aes(parent_key, params.data_key)
+                            })
+                        elif email in emails:
+                            public_key = emails[email]
+                            if public_key:
+                                try:
+                                    rsa_key = RSA.importKey(base64.urlsafe_b64decode(public_key + '=='))
+                                    request['add_users'].append({
+                                        'username': email,
+                                        'manage_users': perm.manage_users,
+                                        'manage_records': perm.manage_records,
+                                        'shared_folder_key': api.encrypt_rsa(parent_key, rsa_key)
+                                    })
+                                except:
+                                    pass
+            shared_folder_add.append(request)
 
-                                fol_req = folder_pb2.FolderRequest()
-                                fol_req.folderUid = base64.urlsafe_b64decode(folder_uid + '==')
-                                fol_req.folderType = 2 if folder_type == 'shared_folder' else 3 if folder_type == 'shared_folder_folder' else 1
-
-                                if parent_uid:
-                                    fol_req.parentFolderUid = base64.urlsafe_b64decode(parent_uid + '==')
-                                    if folder_type == 'shared_folder_folder' and parent_uid == parent_shared_folder_uid:
-                                        fol_req.parentFolderUid = b''
-
-                                folder_key = os.urandom(32)
-                                if folder_type == 'shared_folder_folder':
-                                    fol_req.encryptedFolderKey = base64.urlsafe_b64decode(api.encrypt_aes(folder_key, parent_shared_folder_key or params.data_key) + '==')
-                                else:
-                                    fol_req.encryptedFolderKey = base64.urlsafe_b64decode(api.encrypt_aes(folder_key, params.data_key) + '==')
+    return shared_folder_add
 
-                                data = {'name': comp}
-                                fol_req.folderData = base64.urlsafe_b64decode(api.encrypt_aes(json.dumps(data).encode('utf-8'), folder_key) + '==')
 
-                                if folder_type == 'shared_folder':
-                                    fol_req.sharedFolderFields.encryptedFolderName = base64.urlsafe_b64decode(api.encrypt_aes(comp.encode('utf-8'), folder_key) + '==')
+def prepare_folder_add(params, records):
+    folder_hash = {}
+    for f_uid in params.folder_cache:
+        fol = params.folder_cache[f_uid]
+        h = hashlib.md5()
+        hs = '{0}|{1}'.format((fol.name or '').lower(), fol.parent_uid or '')
+        h.update(hs.encode())
+        shared_folder_key = None
+        if fol.type in { BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
+            sf_uid = fol.shared_folder_uid if fol.type == BaseFolderNode.SharedFolderFolderType else fol.uid
+            if sf_uid in params.shared_folder_cache:
+                shared_folder_key = params.shared_folder_cache[sf_uid]['shared_folder_key_unencrypted']
+        folder_hash[h.hexdigest()] = f_uid, fol.type, shared_folder_key
 
-                                    parent_shared_folder_key = folder_key
-                                    parent_shared_folder_uid = folder_uid
+    folder_add = []
 
-                                elif folder_type == 'shared_folder_folder':
-                                    if parent_shared_folder_uid:
-                                        fol_req.sharedFolderFolderFields.sharedFolderUid = base64.urlsafe_b64decode(parent_shared_folder_uid + '==')
+    for rec in records:
+        if rec.folders:
+            for fol in rec.folders:
+                parent_uid = ''
+                parent_shared_folder_uid = None
+                parent_shared_folder_key = None
+                parent_type = BaseFolderNode.RootFolderType
+                for is_domain in [True, False]:
+                    path = fol.domain if is_domain else fol.path
+                    if not path:
+                        continue
 
-                                folder_add.append(fol_req)
-                                folder_hash[digest] = folder_uid, folder_type, parent_shared_folder_key
+                    comps = list(path_components(path))
+                    for i in range(len(comps)):
+                        comp = comps[i]
+                        h = hashlib.md5()
+                        hs = '{0}|{1}'.format(comp.lower(), parent_uid)
+                        h.update(hs.encode())
+                        digest = h.hexdigest()
+                        if digest not in folder_hash:
+                            is_shared = False
+                            if i == len(comps) - 1:
+                                is_shared = is_domain
+                            folder_uid = api.generate_record_uid()
+                            request = {
+                                'command': 'folder_add',
+                                'folder_uid': folder_uid
+                            }
+                            if parent_type in {BaseFolderNode.UserFolderType, BaseFolderNode.RootFolderType}:
+                                folder_type = 'shared_folder' if is_shared else 'user_folder'
                             else:
-                                folder_uid, folder_type, parent_shared_folder_key = folder_hash[digest]
-
-                            if folder_type == 'shared_folder':
-                                parent_shared_folder_uid = folder_uid
+                                folder_type = 'shared_folder_folder'
+                            request['folder_type'] = folder_type
 
+                            encryption_key = params.data_key
+                            if request['folder_type'] == 'shared_folder_folder' and parent_shared_folder_uid and parent_shared_folder_key:
+                                encryption_key = parent_shared_folder_key
+                                request['shared_folder_uid'] = parent_shared_folder_uid
+
+                            folder_key = os.urandom(32)
+                            request['key'] = api.encrypt_aes(folder_key, encryption_key)
+                            if parent_type not in {BaseFolderNode.RootFolderType, BaseFolderNode.SharedFolderType}:
+                                request['parent_uid'] = parent_uid
+
+                            if request['folder_type'] == 'shared_folder':
+                                request['name'] = api.encrypt_aes(comp.encode('utf-8'), folder_key)
+                                parent_shared_folder_key = folder_key
+
+                            data = {'name': comp}
+                            request['data'] = api.encrypt_aes(json.dumps(data).encode('utf-8'), folder_key)
+                            folder_add.append(request)
                             parent_uid = folder_uid
                             parent_type = folder_type
+                            folder_hash[digest] = parent_uid, parent_type, parent_shared_folder_key
+                        else:
+                            parent_uid, parent_type, parent_shared_folder_key = folder_hash[digest]
 
-                    fol.uid = parent_uid
+                        if parent_type == BaseFolderNode.SharedFolderType:
+                            parent_shared_folder_uid = parent_uid
+                fol.uid = parent_uid
 
     return folder_add
 
 
-def tokenize_record(record):   # type: (Record) -> [str]
-    yield record.title or ''
-    yield record.login or ''
-    yield record.password or ''
-    yield record.login_url or ''
-    yield record.notes or ''
-
-    custom = {}
-    if record.custom_fields:
-        for cf in record.custom_fields:
-            if cf.get('name') and cf.get('value'):
-                custom[cf.get('name')] = cf.get('value')
-    if record.totp:
-        custom[TWO_FACTOR_CODE] = record.totp
-    if len(custom) > 0:
-        keys = list(custom.keys())
-        keys.sort()
-        for key in keys:
-            yield key + ':' + custom[key]
-
-
-def tokenize_import_record(record):   # type: (ImportRecord) -> [str]
-    yield record.title or ''
-    yield record.login or ''
-    yield record.password or ''
-    yield record.login_url or ''
-    yield record.notes or ''
-
-    if len(record.custom_fields) > 0:
-        keys = list(record.custom_fields.keys())
-        keys.sort()
-        for key in keys:
-            yield key + ':' + record.custom_fields[key]
-
-
 def prepare_record_add(params, records):
     record_hash = {}
     for r_uid in params.record_cache:
         rec = api.get_record(params, r_uid)
-        h = hashlib.sha256()
-        for token in tokenize_record(rec):
-            h.update(token.encode())
+        h = hashlib.md5()
+        hs = '{0}|{1}|{2}'.format(rec.title or '', rec.login or '', rec.password or '')
+        h.update(hs.encode())
         record_hash[h.hexdigest()] = r_uid
 
     record_adds = []
     for rec in records:
-        h = hashlib.sha256()
-        for token in tokenize_import_record(rec):
-            h.update(token.encode())
-        r_hash = h.hexdigest()
-        if r_hash in record_hash:
-            rec.uid = record_hash[r_hash]
-        else:
-            rec.uid = api.generate_record_uid()
-            record_hash[r_hash] = rec.uid
-            record_key = os.urandom(32)
-            rec_req = folder_pb2.RecordRequest()
-            rec_req.recordUid = base64.urlsafe_b64decode(rec.uid + '==')
-            rec_req.recordType = 0
-            rec_req.encryptedRecordKey = base64.urlsafe_b64decode(api.encrypt_aes(record_key, params.data_key) + '==')
-            rec_req.howLongAgo = 0
-            rec_req.folderType = 1
+        h = hashlib.md5()
+        hs = '{0}|{1}|{2}'.format(rec.title or '', rec.login or '', rec.password or '')
+        h.update(hs.encode())
+        rec_hash = h.hexdigest()
 
+        record_uid = record_hash.get(rec_hash)
+        if record_uid is None:
+            record_key = os.urandom(32)
+            record_uid = api.generate_record_uid()
+            req = {
+                'command': 'record_add',
+                'record_uid': record_uid,
+                'record_type': 'password',
+                'record_key': api.encrypt_aes(record_key, params.data_key),
+                'how_long_ago': 0,
+                'folder_type': 'user_folder'
+            }
             folder_uid = None
             if rec.folders:
-                folder_uid = rec.folders[0].uid
+                if len(rec.folders) > 0:
+                    folder_uid = rec.folders[0].uid
             if folder_uid:
                 if folder_uid in params.folder_cache:
                     folder = params.folder_cache[folder_uid]
                     if folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
-                        rec_req.folderUid = base64.urlsafe_b64decode(folder.uid + '==')
-                        rec_req.folderType = 2 if folder.type == BaseFolderNode.SharedFolderType else 3
+                        req['folder_uid'] = folder.uid
+                        req['folder_type'] = 'shared_folder' if folder.type == BaseFolderNode.SharedFolderType else 'shared_folder_folder'
 
                         sh_uid = folder.uid if folder.type == BaseFolderNode.SharedFolderType else folder.shared_folder_uid
                         sf = params.shared_folder_cache[sh_uid]
-                        rec_req.encryptedRecordFolderKey = base64.urlsafe_b64decode(api.encrypt_aes(record_key, sf['shared_folder_key_unencrypted']) + '==')
+                        req['folder_key'] = api.encrypt_aes(record_key, sf['shared_folder_key_unencrypted'])
+                        if 'key_type' not in sf:
+                            if 'teams' in sf:
+                                for team in sf['teams']:
+                                    req['team_uid'] = team['team_uid']
+                                    if team['manage_records']:
+                                        break
                     else:
-                        rec_req.folderType = 1
+                        req['folder_type'] = 'user_folder'
                         if folder.type != BaseFolderNode.RootFolderType:
-                            rec_req.folderUid = base64.urlsafe_b64decode(folder.uid + '==')
+                            req['folder_uid'] = folder.uid
 
             custom_fields = []
-            totp = None
             if rec.custom_fields:
                 for cf in rec.custom_fields:
-                    if cf == TWO_FACTOR_CODE:
-                        totp = rec.custom_fields[cf]
-                    else:
-                        custom_fields.append({
-                            'name': cf,
-                            'value': rec.custom_fields[cf]
-                        })
+                    custom_fields.append({
+                        'name': cf,
+                        'value': rec.custom_fields[cf]
+                    })
 
             data = {
                 'title': rec.title or '',
                 'secret1': rec.login or '',
                 'secret2': rec.password or '',
                 'link': rec.login_url or '',
                 'notes': rec.notes or '',
                 'custom': custom_fields
             }
-            rec_req.recordData = base64.urlsafe_b64decode(api.encrypt_aes(json.dumps(data).encode('utf-8'), record_key) + '==')
-            if totp:
-                extra = {
-                    'fields': [
-                        {
-                            'id': api.generate_record_uid(),
-                            'field_type': 'totp',
-                            'field_title': 'Two-Factor Code',
-                            'type': 0,
-                            'data': totp
-                        }]
-                }
-                rec_req.extra = base64.urlsafe_b64decode(api.encrypt_aes(json.dumps(extra).encode('utf-8'), record_key) + '==')
-            record_adds.append(rec_req)
+            req['data'] =  api.encrypt_aes(json.dumps(data).encode('utf-8'), record_key)
+            record_adds.append(req)
+
+        rec.uid = record_uid
 
     return record_adds
 
 
 def prepare_record_link(params, records):
-    record_folders = {}    # type: [str, [str]]
     record_links = []
     for rec in records:
-        if rec.uid:
+        if rec.folders and rec.uid:
             if rec.uid in params.record_cache:
-                if rec.uid in record_folders:
-                    folder_ids = record_folders[rec.uid]
-                else:
-                    folder_ids = list(find_folders(params, rec.uid))
-                    record_folders[rec.uid] = folder_ids
                 record = params.record_cache[rec.uid]
-                for fol in rec.folders or [None]:
-                    folder_uid = fol.uid if fol else ''
-                    if folder_uid and folder_uid not in params.folder_cache:
-                        continue
-                    if folder_uid in folder_ids:
-                        continue
-                    if len(folder_ids) > 0:
-                        folder_ids.append(folder_uid)
-                        src_folder = params.folder_cache[folder_ids[0]]
-                        dst_folder = params.folder_cache[folder_uid] if folder_uid in params.folder_cache else params.root_folder
-                        req = {
-                            'command': 'move',
-                            'to_type': dst_folder.type if dst_folder.type != BaseFolderNode.RootFolderType else BaseFolderNode.UserFolderType,
-                            'link': True,
-                            'move': [],
-                            'transition_keys': []
-                        }
-                        if dst_folder.type != BaseFolderNode.RootFolderType:
-                            req['to_uid'] = dst_folder.uid
-                        mo = {
-                            'type': 'record',
-                            'uid': rec.uid,
-                            'from_type': src_folder.type if src_folder.type != BaseFolderNode.RootFolderType else BaseFolderNode.UserFolderType,
-                            'cascade': True
-                        }
-                        if src_folder.type != BaseFolderNode.RootFolderType:
-                            mo['from_uid'] = src_folder.uid
-                        req['move'].append(mo)
-
-                        transition_key = None
-                        record_key = record['record_key_unencrypted']
-                        if src_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
-                            if dst_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
-                                ssf_uid = src_folder.uid if src_folder.type == BaseFolderNode.SharedFolderType else \
-                                    src_folder.shared_folder_uid
-                                dsf_uid = dst_folder.uid if dst_folder.type == BaseFolderNode.SharedFolderType else \
-                                    dst_folder.shared_folder_uid
-                                if ssf_uid != dsf_uid:
-                                    shf = params.shared_folder_cache[dsf_uid]
-                                    transition_key = api.encrypt_aes(record_key, shf['shared_folder_key_unencrypted'])
-                            else:
-                                transition_key = api.encrypt_aes(record_key, params.data_key)
-                        else:
-                            if dst_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
-                                dsf_uid = dst_folder.uid if dst_folder.type == BaseFolderNode.SharedFolderType else \
-                                    dst_folder.shared_folder_uid
-                                shf = params.shared_folder_cache[dsf_uid]
-                                transition_key = api.encrypt_aes(record_key, shf['shared_folder_key_unencrypted'])
-                        if transition_key is not None:
-                            req['transition_keys'].append({
-                                'uid': rec.uid,
-                                'key': transition_key
-                            })
-                        record_links.append(req)
+                folder_ids = list(find_folders(params, rec.uid))
+                for fol in rec.folders:
+                    if fol.uid and fol.uid in params.folder_cache:
+                        if len(folder_ids) > 0:
+                            if fol.uid not in folder_ids:
+                                src_folder =  params.folder_cache[folder_ids[0]]
+                                dst_folder = params.folder_cache[fol.uid]
+                                req = {
+                                    'command': 'move',
+                                    'to_type': dst_folder.type if dst_folder.type != BaseFolderNode.RootFolderType else BaseFolderNode.UserFolderType,
+                                    'link': True,
+                                    'move': [],
+                                    'transition_keys': []
+                                }
+                                if dst_folder.type != BaseFolderNode.RootFolderType:
+                                    req['to_uid'] = dst_folder.uid
+                                mo = {
+                                    'type': 'record',
+                                    'uid': rec.uid,
+                                    'from_type': src_folder.type if src_folder.type != BaseFolderNode.RootFolderType else BaseFolderNode.UserFolderType,
+                                    'cascade': True
+                                }
+                                if src_folder.type != BaseFolderNode.RootFolderType:
+                                    mo['from_uid'] = src_folder.uid
+                                req['move'].append(mo)
+
+                                transition_key = None
+                                record_key = record['record_key_unencrypted']
+                                if src_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
+                                    if dst_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
+                                        ssf_uid = src_folder.uid if src_folder.type == BaseFolderNode.SharedFolderType else \
+                                            src_folder.shared_folder_uid
+                                        dsf_uid = dst_folder.uid if dst_folder.type == BaseFolderNode.SharedFolderType else \
+                                            dst_folder.shared_folder_uid
+                                        if ssf_uid != dsf_uid:
+                                            shf = params.shared_folder_cache[dsf_uid]
+                                            transition_key = api.encrypt_aes(record_key, shf['shared_folder_key_unencrypted'])
+                                    else:
+                                        transition_key = api.encrypt_aes(record_key, params.data_key)
+                                else:
+                                    if dst_folder.type in {BaseFolderNode.SharedFolderType, BaseFolderNode.SharedFolderFolderType}:
+                                        dsf_uid = dst_folder.uid if dst_folder.type == BaseFolderNode.SharedFolderType else \
+                                            dst_folder.shared_folder_uid
+                                        shf = params.shared_folder_cache[dsf_uid]
+                                        transition_key = api.encrypt_aes(record_key, shf['shared_folder_key_unencrypted'])
+                                if transition_key is not None:
+                                    req['transition_keys'].append({
+                                        'uid': rec.uid,
+                                        'key': transition_key
+                                    })
+                                record_links.append(req)
     return record_links
 
 
-def prepare_folder_permission(params, folders):    # type: (KeeperParams, list) -> list
-    shared_folder_lookup = {}
-    for shared_folder_uid in params.shared_folder_cache:
-        path = get_folder_path(params, shared_folder_uid)
-        if path:
-            shared_folder_lookup[path] = shared_folder_uid
-
-    email_pattern = re.compile(EMAIL_PATTERN)
-    emails = set()
-    teams = set()
-    for fol in folders:
-        if fol.permissions:
-            for perm in fol.permissions:
-                if perm.uid:
-                    teams.add(perm.uid)
-                    if perm.name:
-                        teams.add(perm.name)
-                elif perm.name:
-                    match = email_pattern.match(perm.name)
-                    if match:
-                        if perm.name != params.user:
-                            emails.add(perm.name.lower())
-                    else:
-                        teams.add(perm.name)
-
-    if len(emails) > 0:
-        api.load_user_public_keys(params, list(emails))
-
-    if len(teams) > 0:
-        api.load_available_teams(params)
-        team_uids = set()
-        for t in teams:
-            team_uid = next((x.get('team_uid') for x in params.available_team_cache
-                         if x.get('team_uid') == t or x.get('team_name').casefold() == t.casefold()), None)
-            if team_uid:
-                team_uids.add(team_uid)
-        if len(team_uids) > 0:
-            api.load_team_keys(params, list(team_uids))
-
-    folder_permissions = []
-    for fol in folders:
-        shared_folder_uid = shared_folder_lookup.get(fol.path)
-        if not shared_folder_uid:
-            continue
-        shared_folder = params.shared_folder_cache.get(shared_folder_uid)
-        if not shared_folder:
-            continue
-        shared_folder_key = shared_folder.get('shared_folder_key_unencrypted')
-        if not shared_folder_key:
-            continue
-
-        if fol.permissions:
-            add_users = []
-            add_teams = []
-            for perm in fol.permissions:
-                try:
-                    if perm.uid:
-                        if perm.uid in params.key_cache:
-                            team_key = params.key_cache[perm.uid]
-                            rq = {
-                                'team_uid': perm.uid,
-                                'manage_users': perm.manage_users,
-                                'manage_records': perm.manage_records,
-                            }
-                            if type(team_key) == bytes:
-                                rq['shared_folder_key'] = api.encrypt_aes(shared_folder_key, team_key)
-                            else:
-                                rq['shared_folder_key'] = api.encrypt_rsa(shared_folder_key, team_key)
-                            add_teams.append(rq)
-                            continue
-
-                    if perm.name:
-                        name = perm.name.casefold()
-                        if name in params.key_cache:
-                            rsa_key = params.key_cache[name]
-                            rq = {
-                                'username': name,
-                                'manage_users': perm.manage_users,
-                                'manage_records': perm.manage_records,
-                                'shared_folder_key': api.encrypt_rsa(shared_folder_key, rsa_key)
-                            }
-                            add_users.append(rq)
-                            continue
-
-                        team_uid = next((x.get('team_uid') for x in params.available_team_cache
-                                         if x.get('team_name').casefold() == name), None)
-                        if team_uid in params.key_cache:
-                            team_key = params.key_cache[team_uid]
-                            rq = {
-                                'team_uid': team_uid,
-                                'manage_users': perm.manage_users,
-                                'manage_records': perm.manage_records,
-                            }
-                            if type(team_key) == bytes:
-                                rq['shared_folder_key'] = api.encrypt_aes(shared_folder_key, team_key)
-                            else:
-                                rq['shared_folder_key'] = api.encrypt_rsa(shared_folder_key, team_key)
-                            add_teams.append(rq)
-                            continue
-
-                except Exception as e:
-                    logging.debug(e)
-
-            if add_teams or add_users:
-                request = {
-                    'command': 'shared_folder_update',
-                    'operation': 'update',
-                    'pt': 'Commander',
-                    'shared_folder_uid': shared_folder_uid,
-                    'force_update': True,
-                    'add_teams': add_teams,
-                    'add_users': add_users,
-                }
-                folder_permissions.append(request)
-
-    return folder_permissions
-
-
 def prepare_record_permission(params, records):
     shared_update = []
     for rec in records:
         if rec.folders and rec.uid:
             if rec.uid in params.record_cache:
                 for fol in rec.folders:
                     if fol.can_edit is None and fol.can_share is None:
```

### Comparing `keepercommander-4.88/keepercommander/importer/json/json.py` & `keepercommander-4.9/keepercommander/importer/json/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 # Copyright 2018 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import json
 import sys
 
-from ..importer import BaseFileImporter, BaseExporter, Record, Folder, SharedFolder, Permission
+from ..importer import BaseImporter, BaseExporter, Record, Folder, SharedFolder, Permission
 
 
-class KeeperJsonImporter(BaseFileImporter):
+class KeeperJsonImporter(BaseImporter):
     def do_import(self, filename):
         with open(filename, "r", encoding='utf-8') as json_file:
             j = json.load(json_file)
             records = j if type(j) == list else j.get('records')
             folders = None if type(j) == list else j.get('shared_folders')
             if folders:
                 for shf in folders:
@@ -41,19 +41,19 @@
                             fol.permissions.append(p)
 
                     yield fol
 
             if records:
                 for r in records:
                     record = Record()
-                    record.title = r.get('title')
-                    record.login = r.get('login')
-                    record.password = r.get('password')
-                    record.login_url = r.get('login_url')
-                    record.notes = r.get('notes')
+                    record.title = r['title']
+                    record.login = r['login']
+                    record.password = r['password']
+                    record.login_url = r['login_url']
+                    record.notes = r['notes']
                     if 'custom_fields' in r:
                         custom_fields = r['custom_fields']
                         if custom_fields:
                             record.custom_fields.update(custom_fields)
                     if 'folders' in r:
                         record.folders = []
                         for f in r['folders']:
@@ -67,23 +67,20 @@
                     yield record
 
     def extension(self):
         return 'json'
 
 
 class KeeperJsonExporter(BaseExporter):
-
-    def do_export(self, filename, records, file_password):
+    def do_export(self, filename, records):
         sfs = []
         rs = []
-        for elem in records:
-            if type(elem) == Record:
-                r = elem    # type: Record
+        for r in records:
+            if type(r) == Record:
                 ro = {
-                    'uid': r.uid or '',
                     'title': r.title or '',
                     'login': r.login or '',
                     'password': r.password or '',
                     'login_url': r.login_url or '',
                     'notes': r.notes or '',
                     'custom_fields': {}
                 }
@@ -100,16 +97,16 @@
                             if folder.path:
                                 fo['folder'] = folder.path
                             if folder.can_edit:
                                 fo['can_edit'] = True
                             if folder.can_share:
                                 fo['can_share'] = True
                 rs.append(ro)
-            elif type(elem) == SharedFolder:
-                sf = elem      # type: SharedFolder
+            elif type(r) == SharedFolder:
+                sf = r      # type: SharedFolder
                 sfo = {
                     'uid': sf.uid,
                     'path': sf.path,
                     'manage_users': sf.manage_users,
                     'manage_records': sf.manage_records,
                     'can_edit': sf.can_edit,
                     'can_share': sf.can_share
@@ -123,15 +120,15 @@
                             'manage_records': perm.manage_records
                         }
                         if perm.uid:
                             po['uid'] = perm.uid
                         sfo['permissions'].append(po)
                 sfs.append(sfo)
 
-        jo = {'shared_folders': sfs, 'records': rs}
+        jo = {'shared_folders': sfs, 'records': rs} if sfs else rs
         if filename:
             with open(filename, mode="w", encoding='utf-8') as f:
                 json.dump(jo, f, indent=2, ensure_ascii=False)
         else:
             json.dump(jo, sys.stdout, indent=2, ensure_ascii=False)
             print('')
```

### Comparing `keepercommander-4.88/keepercommander/importer/keepass/keepass.py` & `keepercommander-4.9/keepercommander/importer/keepass/keepass.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,37 +31,32 @@
 
 try:
     import libkeepass
 except:
     raise Exception(keepass_instructions)
 
 import os
-import logging
 import base64
 import getpass
 import gzip
 import io
-import re
-import uuid
 
 from contextlib import contextmanager
 
 from lxml import objectify, etree
 
 from Cryptodome.Cipher import AES
 
-from ..importer import path_components, PathDelimiter, BaseFileImporter, BaseExporter, \
+from ..importer import path_components, PathDelimiter, BaseImporter, BaseExporter, \
     Record, Folder, SharedFolder, Permission, Attachment
 
 from keepercommander.api import unpad_binary
 
 
-_REFERENCE = r'\{REF:([TUPAN])@([IT]):([^\}]+)\}'
-
-class KeepassImporter(BaseFileImporter):
+class KeepassImporter(BaseImporter):
 
     @staticmethod
     def get_folder(group):
         g = group
         path = ''
         comp = ''
         while g.tag == 'Group':
@@ -75,25 +70,17 @@
                 nm = g.Name.text
                 if nm is not None:
                     comp = nm.replace(PathDelimiter, PathDelimiter*2)
             g = g.getparent()
         return path
 
     def do_import(self, filename):
-        credentials = {}
         password = getpass.getpass(prompt='...' + 'Keepass Password'.rjust(20) + ': ', stream=None)
-        if password:
-            credentials['password'] = password
-        print('Press Enter if your Keepass file is not protected with a key file')
-        keyfile = input('...' + 'Path to Key file'.rjust(20) + ': ')
-        if keyfile:
-            keyfile = os.path.expanduser(keyfile)
-            credentials['keyfile'] = keyfile
 
-        with libkeepass.open(filename, **credentials) as kdb:
+        with libkeepass.open(filename, password=password) as kdb:
             root = kdb.obj_root.find('Root/Group')
             if root is not None:
                 groups = [root]
                 pos = 0
                 while pos < len(groups):
                     g = groups[pos]
                     groups.extend(g.findall('Group'))
@@ -130,26 +117,25 @@
                                                 perm.name = p.text
                                             elif p.tag == 'ManageUsers':
                                                 perm.manage_users = p == True
                                             elif p.tag == 'ManageRecords':
                                                 perm.manage_records = p == True
                                 yield sf
 
-                records = []
                 for group in groups:
                     entries = group.findall('Entry')
                     if len(entries) > 0:
                         folder = KeepassImporter.get_folder(group)
                         for entry in entries:
                             record = Record()
                             fol = Folder()
                             fol.path = folder
                             record.folders = [fol]
                             if hasattr(entry, 'UUID'):
-                                record.uid = base64.urlsafe_b64encode(base64.b64decode(entry.UUID.text)).decode().rstrip('=')
+                                record.record_uid = base64.urlsafe_b64encode(base64.b64decode(entry.UUID.text)).decode().rstrip('=')
                             if hasattr(entry, 'Keeper'):
                                 for sn in entry.Keeper.iterchildren():
                                     if sn.tag == 'CanEdit':
                                         fol.can_edit = sn == True
                                     elif sn.tag == 'CanShare':
                                         fol.can_share = sn == True
                                     elif sn.tag == 'Link':
@@ -196,99 +182,29 @@
                                             binary = kdb.obj_root.Meta.Binaries.find('Binary[@ID="{0}"]'.format(ref))
                                             if binary:
                                                 if record.attachments is None:
                                                     record.attachments = []
                                                 atta = KeepassAttachment(binary)
                                                 atta.name = bin.Key.text
                                                 record.attachments.append(atta)
-                                    except Exception as e:
-                                        logging.debug(e)
-                            records.append(record)
-                id_map = None
-                title_map = None
-                ref_re = re.compile(_REFERENCE, re.IGNORECASE)
-
-                def resolve_references(text):
-                    nonlocal id_map
-                    nonlocal title_map
-
-                    if not text:
-                        return text
-                    matches = list(ref_re.finditer(text))
-                    if not matches:
-                        return text
-                    values = []
-                    for match in matches:
-                        comps = match.groups()
-                        val = match.group(0)
-                        if len(comps) == 3:
-                            rec = None
-                            if comps[1].upper() == 'I':
-                                if id_map is None:
-                                    id_map = {}
-                                    for r in records:
-                                        if r.uid:
-                                            id_map[r.uid] = r
-                                uid = uuid.UUID(comps[2])
-                                if uid:
-                                    ref_id = base64.urlsafe_b64encode(uid.bytes).decode().rstrip('=')
-                                    rec = id_map.get(ref_id)
-                            elif comps[1].upper() == 'T':
-                                if title_map is None:
-                                    title_map = {}
-                                    for r in records:
-                                        if r.title:
-                                            title_map[r.title] = r
-                                rec = title_map.get(comps[2])
-                            if rec:
-                                field_id = comps[0].upper()
-                                if field_id == 'T':
-                                    val = rec.title
-                                elif field_id == 'U':
-                                    val = rec.login
-                                elif field_id == 'P':
-                                    val = rec.password
-                                elif field_id == 'A':
-                                    val = rec.login_url
-                                elif field_id == 'N':
-                                    val = rec.notes
-                        values.append(val or '')
-
-                        idx = list(range(len(matches)))
-                        idx.reverse()
-                        for index in idx:
-                            match = matches[index]
-                            val = values[index] if index < len(values) else ''
-                            text = text[:match.start()] + val + text[match.end():]
-                        return text
-
-                for record in records:
-                    try:
-                        record.login = resolve_references(record.login)
-                        record.password = resolve_references(record.password)
-                        record.login_url = resolve_references(record.login_url)
-                        record.notes = resolve_references(record.notes)
-                        if record.custom_fields:
-                            for key in record.custom_fields.keys():
-                                record.custom_fields[key] = resolve_references(record.custom_fields[key])
-                    except Exception as e:
-                        logging.debug(e)
-                    yield record
+                                    except:
+                                        pass
+
+
+                            yield record
 
     def extension(self):
         return 'kdbx'
 
 
 class KeepassExporter(BaseExporter):
 
-    def do_export(self, filename, records, file_password=None):
-        master_password = file_password
-        if not master_password:
-            print('Choose password for your Keepass file')
-            master_password = getpass.getpass(prompt='...' + 'Keepass Password'.rjust(20) + ': ', stream=None)
+    def do_export(self, filename, records):
+        print('Choose password for your Keepass file')
+        master_password = getpass.getpass(prompt='...' + 'Keepass Password'.rjust(20) + ': ', stream=None)
 
         sfs = []  # type: [SharedFolder]
         rs = []   # type: [Record]
         for x in records:
             if type(x) is Record:
                 rs.append(x)
             elif type(x) is SharedFolder:
@@ -299,15 +215,15 @@
         with libkeepass.open(template_file, password='111111') as kdb:
             root = kdb.obj_root.Root.Group
             for sf in sfs:
                 comps = list(path_components(sf.path))
                 node = root
                 for i in range(len(comps)):
                     comp = comps[i]
-                    sub_node = node.find("Group[Name=\'{0}\']".format(comp))
+                    sub_node = node.find('Group[Name=\'{0}\']'.format(comp))
                     if sub_node is None:
                         sub_node = objectify.Element('Group')
                         sub_node.UUID = base64.b64encode(os.urandom(16)).decode()
                         sub_node.Name = comp
                         node.append(sub_node)
                     if i == len(comps) - 1:  # store Keeper specific info
                         keeper = sub_node.find('Keeper')
@@ -340,15 +256,15 @@
                         fol = r.folders[0]
                         for is_shared in [True, False]:
                             path = fol.domain if is_shared else fol.path
                             if path:
                                 comps = list(path_components(path))
                                 for i in range(len(comps)):
                                     comp = comps[i]
-                                    sub_node = node.find("Group[Name=\'{0}\']".format(comp))
+                                    sub_node = node.find('Group[Name=\'{0}\']'.format(comp))
                                     if sub_node is None:
                                         sub_node = objectify.Element('Group')
                                         sub_node.UUID = base64.b64encode(os.urandom(16)).decode()
                                         sub_node.Name = comp
                                         node.append(sub_node)
                                     node = sub_node
                     entry = None
@@ -428,62 +344,49 @@
                             s_node = objectify.Element('String')
                             s_node.Key = key
                             s_node.Value = value
                             entry.append(s_node)
 
                     if r.attachments:
                         for atta in r.attachments:
-                            if atta.size < self.max_size:
+                            max_size = 1024 * 1024
+                            if atta.size < max_size:
+                                bins = None
+                                bId = 0
                                 if hasattr(kdb.obj_root.Meta, 'Binaries'):
                                     bins = kdb.obj_root.Meta.Binaries
                                     elems = bins.findall('Binary')
                                     bId = len(elems)
                                 else:
                                     bins = objectify.Element('Binaries')
                                     kdb.obj_root.Meta.append(bins)
                                     bId = 0
-
-                                out = io.BytesIO()
-                                with gzip.GzipFile(fileobj=out, mode='w') as gz:
-                                    with atta.open() as s:
-                                        iv = s.read(16)
+                                with atta.open() as s:
+                                    buffer = s.read(max_size)
+                                    if len(buffer) >= 32:
+                                        iv = buffer[:16]
                                         cipher = AES.new(atta.key, AES.MODE_CBC, iv)
-                                        finished = False
-                                        chunk_size = 1024 ** 2
-                                        while not finished:
-                                            buffer = s.read(chunk_size)
-                                            finished = len(buffer) < chunk_size
-                                            if buffer:
-                                                buffer = cipher.decrypt(buffer)
-                                                if finished:
-                                                    buffer = unpad_binary(buffer)
+                                        buffer = cipher.decrypt(buffer[16:])
+                                        if len(buffer) > 0:
+                                            buffer = unpad_binary(buffer)
+                                            out = io.BytesIO()
+                                            with gzip.GzipFile(fileobj=out, mode='w') as gz:
                                                 gz.write(buffer)
+                                            bin = objectify.E.Binary(base64.b64encode(out.getvalue()).decode(), Compressed=str(True), ID=str(bId))
+                                            bins.append(bin)
 
-                                bin = objectify.E.Binary(base64.b64encode(out.getvalue()).decode(), Compressed=str(True), ID=str(bId))
-                                bins.append(bin)
-
-                                bin = objectify.Element('Binary')
-                                bin.Key=atta.name
-                                bin.Value = objectify.Element('Value', Ref=str(bId))
-                                entry.append(bin)
+                                            bin = objectify.Element('Binary')
+                                            bin.Key=atta.name
+                                            bin.Value = objectify.Element('Value', Ref=str(bId))
+                                            entry.append(bin)
                             else:
-                                scale = ''
-                                msize = self.max_size
-                                if msize > 1024 ** 3:
-                                    scale = 'G'
-                                    msize //= 1024 ** 3
-                                elif msize > 1024 ** 2:
-                                    scale = 'M'
-                                    msize //= 1024 ** 2
-                                elif msize > 1024:
-                                    scale = 'K'
-                                    msize //= 1024
-                                print('Warning: File \'{0}\' was skipped because it exceeds the {1}{2} file size limit.'.format(atta.name, msize, scale))
+                                print('Warning: File \'{0}\' was skipped because it exceeds the 1MB Keepass filesize limit.'.format(atta.name))
+
                 except Exception as e:
-                    logging.debug(e)
+                    pass
 
             objectify.deannotate(root, xsi_nil=True)
             etree.cleanup_namespaces(root)
 
             kdb.clear_credentials()
             kdb.add_credentials(password=master_password)
             with open(filename, 'wb') as output:
```

### Comparing `keepercommander-4.88/keepercommander/importer/keepass/template.kdbx` & `keepercommander-4.9/keepercommander/importer/keepass/template.kdbx`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/plugins/adpasswd/adpasswd.py` & `keepercommander-4.9/keepercommander/plugins/adpasswd/adpasswd.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,22 @@
 """
 
 def rotate(record, newpassword):
     result = False
 
     old_password = record.password
     host = record.get('cmdr:host')
-    port = record.get('cmdr:port') or '389'
     user_dn = record.get('cmdr:userdn')
     use_ssl = record.get('cmdr:use_ssl')
 
     try:
         # print('Connecting to ' + host)
 
         server = Server(
             host=host,
-            port=int(port),
             use_ssl=(use_ssl in ['True','true','yes','Yes','y','Y','T','t']),
             get_info=ALL)
 
         conn = Connection(
             server=server,
             user=user_dn,
             password=record.password,
@@ -49,15 +47,15 @@
             user=user_dn, new_password=newpassword, old_password=old_password)
 
         if (changePwdResult == True):
             print('Password changed successfully')
             record.password = newpassword
             result = True
         else:
-            print('Error with adpasswd change: ' + str(conn.result))
+            print('Error with adpasswd change: ' + conn.result)
 
         conn.unbind()
 
-    except Exception as e:
-        print("Error during connection to AD server: %s" % str(e))
+    except:
+        print("Error during connection to AD server")
 
     return result
```

### Comparing `keepercommander-4.88/keepercommander/plugins/awskey/aws_accesskey.py` & `keepercommander-4.9/keepercommander/plugins/awskey/aws_accesskey.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/plugins/mssql/mssql.py` & `keepercommander-4.9/keepercommander/plugins/mssql/mssql.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,31 +27,31 @@
     host = record.get('cmdr:host')
     db = record.get('cmdr:db')
 
     connection = ''
 
     try:
         # Connect to the database
-        connection = pymssql.connect(server=host,
+        connection = pymssql.connect(host=host,
                                      user=user,
                                      password=oldpassword,
-                                     database=db)
+                                     db=db)
 
         with connection.cursor() as cursor:
             print("Connected to %s"%(host))
             # Create a new record
-            sql = "ALTER LOGIN %s WITH PASSWORD = '%s';" % (user, newpassword)
+            sql = 'ALTER LOGIN %s WITH PASSWORD="%s";'%(user, newpassword)
             cursor.execute(sql)
 
         # connection is not autocommit by default. So you must commit to save
         # your changes.
         connection.commit()
 
         record.password = newpassword
         result = True
-    except Exception as ex:
-        print("Error during connection to Microsoft SQL server: %s" % ex)
+    except:
+        print("Error during connection to Microsoft SQL server")
     finally:
         if connection:
             connection.close()
 
     return result
```

### Comparing `keepercommander-4.88/keepercommander/plugins/oracle/oracle.py` & `keepercommander-4.9/keepercommander/plugins/oracle/oracle.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,53 +8,45 @@
 # Keeper Commander 
 # Copyright 2015 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import cx_Oracle
 
-# cx_Oracle.init_oracle_client(lib_dir="/Users/[username]]/Downloads/instantclient_19_8") # To initialize
-
 """Commander Plugin for Oracle Database Server
    Dependencies: 
        pip3 install cx_Oracle
 """
 
 def rotate(record, newpassword):
     """ Grab any required fields from the record """
     user = record.login
     oldpassword = record.password
 
     result = False
 
-    host = ""
-
-    if record.get('cmdr:dsn'):
-        dsn_str = record.get('cmdr:dsn')
-    else:
-        host = record.get('cmdr:host')
-        db = record.get('cmdr:db')
-        dsn_str = host + '/' + db
+    host = record.get('cmdr:host')
+    db = record.get('cmdr:db')
 
     connection = ''
 
     try:
         # Connect to the database
-        connection = cx_Oracle.connect(dsn=dsn_str,
+        connection = cx_Oracle.connect(dsn=host + '/' + db,
                                      user=user,
                                      password=oldpassword)
 
         with connection.cursor() as cursor:
-            print("Connected to %s" % (dsn_str if record.get('cmdr:dsn') else host))
+            print("Connected to %s"%(host))
             # Create a new record
-            sql = 'ALTER USER %s IDENTIFIED BY "%s" ACCOUNT UNLOCK' % (user, newpassword)
+            sql = 'ALTER USER %s IDENTIFIED BY "%s" ACCOUNT UNLOCK'%(user, newpassword)
             cursor.execute(sql)
 
         record.password = newpassword
         result = True
-    except Exception as e:
-        print("Error during connection to Oracle server: %s", e)
+    except:
+        print("Error during connection to Oracle server")
     finally:
         if connection:
             connection.close()
 
-    return result
+    return result
```

### Comparing `keepercommander-4.88/keepercommander/plugins/plugin_manager.py` & `keepercommander-4.9/keepercommander/plugins/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/plugins/postgresql/postgresql.py` & `keepercommander-4.9/keepercommander/plugins/mysql/mysql.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,40 +2,62 @@
 #  _  __  
 # | |/ /___ ___ _ __  ___ _ _ ®
 # | ' </ -_) -_) '_ \/ -_) '_|
 # |_|\_\___\___| .__/\___|_|
 #              |_|            
 #
 # Keeper Commander 
-# Copyright 2015 Keeper Security Inc.
+# Copyright 2016 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
-import psycopg2
-import logging
+import pymysql.cursors
 
-"""Commander Plugin for Postgres Database Server
+"""Commander Plugin for MySQL Database Server
    Dependencies: 
-       pip3 install psycopg2-binary
+       pip3 install pymysql
 """
 
-
 def rotate(record, newpassword):
+    """ Grab any required fields from the record """
     user = record.login
     oldpassword = record.password
 
+    result = False
+
+    host = record.get('cmdr:host')
+    db = record.get('cmdr:db')
+
+    connection = ''
+
     try:
-        host = record.get('cmdr:host')
-        db = record.get('cmdr:db') or 'postgres'
-        port = record.get('cmdr:port') or '5432'
-
-        with psycopg2.connect(host=host, port=int(port), user=user, password=oldpassword, database=db) as connection:
-            logging.debug("Connected to %s", host)
-            with connection.cursor() as cursor:
-                sql = f'alter user {user} with password %s'
-                cursor.execute(sql, (newpassword,))
-                record.password = newpassword
-                return True
-    except Exception as e:
-        logging.error('Error rotating password at Postgres server: %s', e)
+        # Connect to the database
+        connection = pymysql.connect(host=host, 
+                                     user=user, 
+                                     password=oldpassword, 
+                                     db=db, 
+                                     charset='utf8mb4', 
+                                     cursorclass=pymysql.cursors.DictCursor)
+
+        with connection.cursor() as cursor:
+            escaped = connection.escape(newpassword)
+            """ TBD - For MySQL 5.7+ use below command:
+                sql = 'ALTER USER "{}"@"{}" IDENTIFIED BY "{}";'.format(
+                    user, host, newpassword)
+            """
+            sql = 'SET PASSWORD = PASSWORD({});'.format(escaped)
+            cursor.execute(sql)
+
+        connection.commit()
+        record.password = newpassword
+        result = True
+    except pymysql.err.OperationalError as e:
+        print("MySQL Plugin Error: Unable to establish connection: " + str(e))
+    except pymysql.err.ProgrammingError as e:
+        print("MySQL Plugin Syntax Error: " + str(e))
+    except:
+        print("Error during connection to MySQL server")
+    finally:
+        if connection:
+            connection.close()
 
-    return False
+    return result
```

### Comparing `keepercommander-4.88/keepercommander/plugins/pspasswd/pspasswd.py` & `keepercommander-4.9/keepercommander/plugins/pspasswd/pspasswd.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/plugins/ssh/ssh.py` & `keepercommander-4.9/keepercommander/plugins/ssh/ssh.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,48 +7,39 @@
 #
 # Keeper Commander 
 # Copyright 2016 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import logging
-import os
-from ...error import Error
 
-if os.name == 'posix':
-    from pexpect import pxssh, exceptions
-else:
-    raise Exception('Not available on Windows')
+from pexpect import pxssh, exceptions
 
 """Commander Plugin for SSH Command
-   Dependencies: s
+   Dependencies: 
        pip3 install pexpect
 """
 
 def rotate(record, newpassword):
     """ Grab any required fields from the record """
-
     user = record.login
     oldpassword = record.password
 
     result = False
 
     host = record.get('cmdr:host')
 
     try:
         s = pxssh.pxssh()
-        s.login(host, user, oldpassword, sync_multiplier=3)
+        s.login(host, user, oldpassword)
         s.sendline('passwd')
-        i = s.expect(['[Oo]ld.*[Pp]assword', '[Cc]urrent.*[Pp]assword', '[Nn]ew.*[Pp]assword'])
+        i = s.expect(['[Oo]ld [Pp]assword', 'current.*password', '[Nn]ew [Pp]assword'])
         if i == 0 or i == 1:
             s.sendline(oldpassword)
-            i = s.expect(['[Nn]ew.*[Pp]assword', 'password unchanged'])
-            if i != 0:
-                return False
-
+            s.expect('[Nn]ew.*[Pp]assword')
         s.sendline(newpassword)
         s.expect("Retype [Nn]ew.*[Pp]assword:")
         s.sendline(newpassword)
         s.prompt()
 
         pass_result = s.before
 
@@ -60,10 +51,9 @@
             logging.error("Password change failed: ", pass_result)
 
         s.logout()
     except exceptions.TIMEOUT as t:
         logging.error("Timed out waiting for response.")
     except pxssh.ExceptionPxssh as e:
         logging.error("Failed to login with ssh.")
-        logging.error(e)
 
     return result
```

### Comparing `keepercommander-4.88/keepercommander/plugins/sshkey/sshkey.py` & `keepercommander-4.9/keepercommander/plugins/sshkey/sshkey.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # Keeper Commander
 # Copyright 2016 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
 
 import subprocess
 import tempfile
-import logging
 import os
 import stat
 
 
 def rotate(record, newpassword):
     old_private_key = record.get('cmdr:private_key')
     key_file_name = None
@@ -77,14 +76,14 @@
         record.set_field('cmdr:rsa_public_key', new_public_key_PEM)
         record.set_field('cmdr:ssh_public_key', new_public_key_SSH)
         record.password = newpassword
 
         return True
 
     except Exception as e:
-        logging.error(e)
+        print(e)
         return False
 
     finally:
         if key_file_name:
             os.remove(key_file_name)
```

### Comparing `keepercommander-4.88/keepercommander/plugins/unixpasswd/unixpasswd.py` & `keepercommander-4.9/keepercommander/plugins/unixpasswd/unixpasswd.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/plugins/windows/windows.py` & `keepercommander-4.9/keepercommander/plugins/windows/windows.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/rest_api.py` & `keepercommander-4.9/keepercommander/rest_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # |_|\_\___\___| .__/\___|_|
 #              |_|
 #
 # Keeper Commander
 # Copyright 2019 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
+from typing import Optional, Union
 
 import requests
 import base64
 import os
 import json
 import hashlib
 import hmac
@@ -19,19 +20,18 @@
 
 from .params import RestApiContext
 from .error import KeeperApiError, CommunicationError
 from . import APIRequest_pb2 as proto
 
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Cipher import AES, PKCS1_v1_5
-from . import __version__
 
 
-LEGACY_CLIENT_VERSION = 'c14.0.0'
-CLIENT_VERSION = 'c15.' + __version__
+CLIENT_VERSION = 'c14.0.0'
+
 
 SERVER_PUBLIC_KEYS = {
     1: RSA.importKey(base64.urlsafe_b64decode(
         'MIIBCgKCAQEA9Z_CZzxiNUz8-npqI4V10-zW3AL7-M4UQDdd_17759Xzm0MOEfH' +
         'OOsOgZxxNK1DEsbyCTCE05fd3Hz1mn1uGjXvm5HnN2mL_3TOVxyLU6VwH9EDInn' +
         'j4DNMFifs69il3KlviT3llRgPCcjF4xrF8d4SR0_N3eqS1f9CBJPNEKEH-am5Xb' +
         '_FqAlOUoXkILF0UYxA_jNLoWBSq-1W58e4xDI0p0GuP0lN8f97HBtfB7ijbtF-V' +
@@ -102,159 +102,144 @@
 
 def derive_key_v2(domain, password, salt, iterations):
     # type: (str, str, bytes, int) -> bytes
     derived_key = hashlib.pbkdf2_hmac('sha512', (domain+password).encode('utf-8'), salt, iterations, 64)
     return hmac.new(derived_key, domain.encode('utf-8'), digestmod=hashlib.sha256).digest()
 
 
-def execute_rest(context, endpoint, payload):    # type: (RestApiContext, str, proto.ApiRequestPayload) -> any
+def execute_rest(context, endpoint, payload):
+    # type: (RestApiContext, str, bytes) -> Union[bytes, dict]
     if not context.transmission_key:
         context.transmission_key = os.urandom(32)
 
     if not context.server_key_id:
         context.server_key_id = 1
 
+    api_request_payload = proto.ApiRequestPayload()
+    api_request_payload.payload = payload
+
     run_request = True
     while run_request:
         run_request = False
 
         api_request = proto.ApiRequest()
         api_request.encryptedTransmissionKey = encrypt_rsa(context.transmission_key, SERVER_PUBLIC_KEYS[context.server_key_id])
         api_request.publicKeyId = context.server_key_id
         api_request.locale = context.locale or 'en_US'
 
-        api_request.encryptedPayload = encrypt_aes(payload.SerializeToString(), context.transmission_key)
+        api_request.encryptedPayload = encrypt_aes(api_request_payload.SerializeToString(), context.transmission_key)
 
         request_data = api_request.SerializeToString()
         url = context.server_base + endpoint
 
         logging.debug('>>> Request URL: [%s]', url)
         rs = requests.post(url, data=request_data, headers={'Content-Type': 'application/octet-stream'})
         logging.debug('<<< Response Code: [%d]', rs.status_code)
         logging.debug('<<< Response Headers: [%s]', str(rs.headers))
 
         content_type = rs.headers.get('Content-Type') or ''
         if rs.status_code == 200:
             if content_type == 'application/json':
-                return rs.json()        # type: dict
-
-            rs_body = rs.content
-            if rs_body:
-                rs_body = decrypt_aes(rs.content, context.transmission_key)
-            return rs_body
-        elif rs.status_code >= 400:
-            if content_type == 'application/json':
-                failure = rs.json()
-                logging.debug('<<< Response Error: [%s]', failure)
-                if rs.status_code == 401:
-                    if failure.get('error') == 'key':
-                        server_key_id = failure['key_id']
-                        if server_key_id != context.server_key_id:
-                            context.server_key_id = server_key_id
-                            run_request = True
-                            continue
-                return failure
+                return rs.json()
             else:
-                logging.debug('<<< HTTP Status: [%s]  Reason: [%s]', rs.status_code, rs.reason)
-                if logging.getLogger().level <= logging.DEBUG:
-                    if rs.text:
-                        logging.debug('<<< Response Content: [%s]', str(rs.text))
-                raise CommunicationError('Code {0}: {1}'.format(rs.status_code, rs.reason))
+                return decrypt_aes(rs.content, context.transmission_key)
+        elif rs.status_code >= 400:
+            failure = rs.json() if content_type == 'application/json' else None
+            if rs.status_code == 401 and json:
+                if failure.get('error') == 'key':
+                    server_key_id = failure['key_id']
+                    if server_key_id != context.server_key_id:
+                        context.server_key_id = server_key_id
+                        run_request = True
+                        continue
+
+            if logging.getLogger().level <= logging.DEBUG:
+                if rs.text:
+                    logging.debug('<<< Response Content: [%s]', str(rs.text))
+
+            return failure
 
 
 def get_device_token(context):
     # type: (RestApiContext) -> str
 
     if not context.device_id:
         rq = proto.DeviceRequest()
         rq.clientVersion = CLIENT_VERSION
         rq.deviceName = ''
-
-        api_request_payload = proto.ApiRequestPayload()
-        api_request_payload.payload = rq.SerializeToString()
-        rs = execute_rest(context, 'authentication/get_device_token', api_request_payload)
-        if type(rs) is bytes:
+        rs = execute_rest(context, 'authentication/get_device_token', rq.SerializeToString())
+        if type(rs) == bytes:
             device_rs = proto.DeviceResponse()
             device_rs.ParseFromString(rs)
-            if proto.DeviceStatus.Name(device_rs.status) == 'DEVICE_OK':
+            if proto.DeviceStatus.Name(device_rs.status) == 'OK':
                 context.device_id = device_rs.encryptedDeviceToken
-        elif type(rs) is dict:
+        elif type(rs) == dict:
             raise KeeperApiError(rs['error'], rs['message'])
 
     return context.device_id
 
 
 def pre_login(context, username, two_factor_token=None):
-    # type: (RestApiContext, str, bytes or None) -> proto.PreLoginResponse
+    # type: (RestApiContext, str, Optional[bytes], bool) -> proto.PreLoginResponse
 
     attempt = 0
     while attempt < 3:
         attempt += 1
         rq = proto.PreLoginRequest()
         rq.authRequest.clientVersion = CLIENT_VERSION
-        rq.authRequest.username = username.lower()
+        rq.authRequest.username = username
         rq.authRequest.encryptedDeviceToken = get_device_token(context)
         rq.loginType = proto.LoginType.Value('NORMAL')
         if two_factor_token:
             rq.twoFactorToken = two_factor_token
 
-        api_request_payload = proto.ApiRequestPayload()
-        api_request_payload.payload = rq.SerializeToString()
-        rs = execute_rest(context, 'authentication/pre_login', api_request_payload)
+        rs = execute_rest(context, 'authentication/pre_login', rq.SerializeToString())
         if type(rs) == bytes:
             pre_login_rs = proto.PreLoginResponse()
             pre_login_rs.ParseFromString(rs)
             return pre_login_rs
 
-        elif type(rs) is dict:
+        if type(rs) == dict:
             if 'error' in rs and 'message' in rs:
                 if rs['error'] == 'region_redirect':
                     context.device_id = None
                     context.server_base = 'https://{0}/'.format(rs['region_host'])
-                    logging.warning('Switching to region: %s', rs['region_host'])
+                    logging.warning('Switching to region: %s.', context.server_base)
                     continue
                 if rs['error'] == 'bad_request':
-                    logging.warning('Pre-Auth error: %s', rs.get('additional_info'))
+                    logging.warning('Invalid device id')
                     context.device_id = None
                     continue
 
                 raise KeeperApiError(rs['error'], rs['message'])
     raise CommunicationError('Cannot get user information')
 
 
 def get_new_user_params(context, username):
     # type: (RestApiContext, str) -> proto.NewUserMinimumParams
     rq = proto.AuthRequest()
     rq.clientVersion = CLIENT_VERSION
-    rq.username = username.lower()
+    rq.username = username
     rq.encryptedDeviceToken = get_device_token(context)
 
-    api_request_payload = proto.ApiRequestPayload()
-    api_request_payload.payload = rq.SerializeToString()
-    rs = execute_rest(context, 'authentication/get_new_user_params', api_request_payload)
-    if type(rs) is bytes:
+    rs = execute_rest(context, 'authentication/get_new_user_params', rq.SerializeToString())
+    if type(rs) == bytes:
         pre_login_rs = proto.NewUserMinimumParams()
         pre_login_rs.ParseFromString(rs)
         return pre_login_rs
 
-    if type(rs) is dict:
+    if type(rs) == dict:
         raise KeeperApiError(rs['error'], rs['message'])
 
 
 def v2_execute(context, rq):
     # type: (RestApiContext, dict) -> dict
 
-    api_request_payload = proto.ApiRequestPayload()
-    api_request_payload.payload = json.dumps(rq).encode('utf-8')
-    rs_data = execute_rest(context, 'vault/execute_v2_command', api_request_payload)
-    if rs_data:
-        if type(rs_data) is bytes:
-            rs = json.loads(rs_data.decode('utf-8'))
-            logger = logging.getLogger()
-            if logger.level <= logging.DEBUG:
-                logger.debug('>>> Request JSON: [%s]', json.dumps(rq, sort_keys=True, indent=4))
-                logger.debug('<<< Response JSON: [%s]', json.dumps(rs, sort_keys=True, indent=4))
-            return rs
+    rs_data = execute_rest(context, 'vault/execute_v2_command', json.dumps(rq).encode('utf-8'))
+    rs = json.loads(rs_data.decode('utf-8'))
+    logger = logging.getLogger()
+    if logger.level <= logging.DEBUG:
+        logger.debug('>>> Request JSON: [%s]', json.dumps(rq, sort_keys=True, indent=4))
+        logger.debug('<<< Response JSON: [%s]', json.dumps(rs, sort_keys=True, indent=4))
 
-        if type(rs_data) is dict:
-            raise KeeperApiError(rs_data['error'], rs_data['message'])
+    return rs
```

### Comparing `keepercommander-4.88/keepercommander/shared_folder.py` & `keepercommander-4.9/keepercommander/shared_folder.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/subfolder.py` & `keepercommander-4.9/keepercommander/subfolder.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,17 +62,16 @@
             if path_component == '.':
                 folder_uid = folder.uid
             elif path_component == '..':
                 folder_uid = folder.parent_uid or '/'
             else:
                 for uid in folder.subfolders:
                     sf = params.folder_cache[uid]
-                    if sf.name.strip().casefold() == path_component.casefold():
+                    if sf.name.strip() == path_component:
                         folder_uid = uid
-                        break
             if folder_uid:
                 folder = params.folder_cache[folder_uid] if folder_uid in params.folder_cache else params.root_folder
             else:
                 break
             if idx < 0:
                 path = ''
                 break
```

### Comparing `keepercommander-4.88/keepercommander/team.py` & `keepercommander-4.9/keepercommander/team.py`

 * *Files identical despite different names*

### Comparing `keepercommander-4.88/keepercommander/yubikey/yubikey.py` & `keepercommander-4.9/keepercommander/yubikey/yubikey.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 # |_|\_\___\___| .__/\___|_|
 #              |_|            
 #
 # Keeper Commander 
 # Copyright 2019 Keeper Security Inc.
 # Contact: ops@keepersecurity.com
 #
+from typing import Optional, List, Tuple
 
-import getpass
 import time
 import threading
-import logging
 import os
 import signal
 import base64
 from hashlib import sha256
 import json
 
 from fido2.hid import CtapHidDevice
@@ -36,26 +35,24 @@
 #
 #     for i in range(len(devices)):
 #         u2f_client = U2fClient(devices[i], "https://dev.keepersecurity.com")
 #         for rq in authenticateRequests:
 #             return u2f_client.sign(rq['appId'], rq['challenge'], [rq])
 #
 #
-from keepercommander.display import bcolors
 
 u2f_response = None
 should_cancel_u2f = False
 
 if os.name == 'nt':
     import msvcrt
     win_cancel_getch = False
 
 def get_input_interrupted(prompt):
-    # TODO: refactor to use interruptable prompt from prompt_toolkit in api.py:193 (login: process 2fa error codes).
-    #  This method to be removed.
+    # type: (str) -> str
     if os.name == 'nt':
         global win_cancel_getch
 
         print(prompt)
         win_cancel_getch = False
         result = b''
         while not win_cancel_getch:
@@ -66,29 +63,28 @@
                 result += ch
             else:
                 time.sleep(0.1)
         if win_cancel_getch:
             raise KeyboardInterrupt()
         return result.decode()
     else:
-        return getpass.getpass(prompt=prompt)
+        return input(prompt)
 
 
 def u2f_authenticate(authenticateRequests):
-    # type: ([dict]) -> dict or None
+    # type: (List[dict]) -> Optional[dict]
 
     global should_cancel_u2f
     global u2f_response
 
     if not authenticateRequests:
         return None
 
     devices = list(CtapHidDevice.list_devices())
     if not devices:
-        logging.warning("No U2F Devices detected")
         return None
 
     to_auth = []
     for i in range(len(devices)):
         u2f_client = CTAP1(devices[i])
         u2f_version = u2f_client.get_version()
         for request in authenticateRequests:
@@ -110,28 +106,29 @@
                         u2f_client.authenticate(client_param, app_id_hash, key_handle, check_only=True)
                     except ApduError as e:
                         if e.code == APDU.USE_NOT_SATISFIED:
                             to_auth.append((u2f_client, client_data, app_id_hash, key_handle))
             except:
                 pass
 
+
     if to_auth:
         u2f_thread = threading.Thread(target=thread_function, args=((to_auth,)))
         u2f_thread.start()
         try:
-            get_input_interrupted(bcolors.WARNING + '\nTouch the flashing U2F device to authenticate or press Enter to resume with the primary two factor authentication...\n' + bcolors.ENDC)
+            get_input_interrupted('\nTouch the flashing U2F device to authenticate or press Enter to resume with the primary two factor authentication...\n')
             should_cancel_u2f = True
             u2f_thread.join()
         except KeyboardInterrupt:
             pass
     return u2f_response
 
 
 def thread_function(auth_requests):
-    # type: ([(CTAP1, str, bytes, bytes)]) -> None
+    # type: (List[Tuple[CTAP1, str, bytes, bytes]]) -> None
     global should_cancel_u2f
     global u2f_response
 
     should_cancel_u2f = False
     u2f_response = None
 
     while len(auth_requests) > 0 and not u2f_response and not should_cancel_u2f:
@@ -154,13 +151,13 @@
             auth_requests[i] = None
         auth_requests = [x for x in auth_requests if x]
         if len(auth_requests) == 0:
             continue
         time.sleep(0.25)
 
     if u2f_response:
-        logging.info('OK')
+        print('OK')
     if os.name == 'nt':
         global win_cancel_getch
         win_cancel_getch = True
     else:
         os.kill(os.getpid(), signal.SIGINT)
```

### Comparing `keepercommander-4.88/keepercommander.egg-info/SOURCES.txt` & `keepercommander-4.9/keepercommander.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,57 @@
-LICENSE
 MANIFEST.in
 README.md
 setup.py
 keepercommander/APIRequest_pb2.py
-keepercommander/AccountSummary_pb2.py
 keepercommander/__init__.py
 keepercommander/__main__.py
 keepercommander/api.py
 keepercommander/autocomplete.py
 keepercommander/cli.py
 keepercommander/display.py
 keepercommander/error.py
-keepercommander/folder_pb2.py
 keepercommander/generator.py
-keepercommander/loginv3.py
 keepercommander/params.py
 keepercommander/record.py
 keepercommander/rest_api.py
 keepercommander/shared_folder.py
-keepercommander/ssocloud_pb2.py
 keepercommander/subfolder.py
 keepercommander/team.py
-keepercommander/versioning.py
 keepercommander.egg-info/PKG-INFO
 keepercommander.egg-info/SOURCES.txt
 keepercommander.egg-info/dependency_links.txt
 keepercommander.egg-info/entry_points.txt
 keepercommander.egg-info/requires.txt
 keepercommander.egg-info/top_level.txt
 keepercommander/commands/__init__.py
 keepercommander/commands/base.py
 keepercommander/commands/enterprise.py
-keepercommander/commands/enterprise_pb2.py
 keepercommander/commands/folder.py
-keepercommander/commands/msp.py
 keepercommander/commands/record.py
 keepercommander/commands/register.py
 keepercommander/commands/utils.py
 keepercommander/importer/__init__.py
 keepercommander/importer/commands.py
 keepercommander/importer/imp_exp.py
 keepercommander/importer/importer.py
 keepercommander/importer/csv/__init__.py
 keepercommander/importer/csv/csv.py
 keepercommander/importer/json/__init__.py
 keepercommander/importer/json/json.py
 keepercommander/importer/keepass/__init__.py
 keepercommander/importer/keepass/keepass.py
 keepercommander/importer/keepass/template.kdbx
-keepercommander/importer/lastpass/__init__.py
-keepercommander/importer/lastpass/account.py
-keepercommander/importer/lastpass/blob.py
-keepercommander/importer/lastpass/chunk.py
-keepercommander/importer/lastpass/exceptions.py
-keepercommander/importer/lastpass/fetcher.py
-keepercommander/importer/lastpass/lastpass.py
-keepercommander/importer/lastpass/parser.py
-keepercommander/importer/lastpass/session.py
-keepercommander/importer/lastpass/vault.py
 keepercommander/plugins/__init__.py
 keepercommander/plugins/commands.py
 keepercommander/plugins/noop.py
 keepercommander/plugins/plugin_manager.py
 keepercommander/plugins/adpasswd/__init__.py
 keepercommander/plugins/adpasswd/adpasswd.py
 keepercommander/plugins/awskey/__init__.py
 keepercommander/plugins/awskey/aws_accesskey.py
-keepercommander/plugins/awspswd/__init__.py
-keepercommander/plugins/awspswd/aws_passwd.py
-keepercommander/plugins/azureadpwd/__init__.py
-keepercommander/plugins/azureadpwd/azureadpwd.py
-keepercommander/plugins/humps/__init__.py
-keepercommander/plugins/humps/humps.py
 keepercommander/plugins/mssql/__init__.py
 keepercommander/plugins/mssql/mssql.py
 keepercommander/plugins/mysql/__init__.py
 keepercommander/plugins/mysql/mysql.py
 keepercommander/plugins/oracle/__init__.py
 keepercommander/plugins/oracle/oracle.py
 keepercommander/plugins/postgresql/__init__.py
```

