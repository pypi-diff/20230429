# Comparing `tmp/dbm-agent-8.33.0.tar.gz` & `tmp/dbm-agent-8.33.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbm-agent-8.33.0.tar", last modified: Fri Apr 21 09:08:54 2023, max compression
+gzip compressed data, was "dbm-agent-8.33.3.tar", last modified: Sat Apr 29 08:41:21 2023, max compression
```

## Comparing `dbm-agent-8.33.0.tar` & `dbm-agent-8.33.3.tar`

### file list

```diff
@@ -1,100 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.321970 dbm-agent-8.33.0/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-21 09:08:54.321970 dbm-agent-8.33.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4453 2023-04-11 12:20:06.000000 dbm-agent-8.33.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.308970 dbm-agent-8.33.0/bin/
--rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.33.0/bin/dbm-agent
--rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.33.0/bin/dbm-bt-conn-stack
--rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.33.0/bin/dbma-cli-init
--rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.33.0/bin/dbma-cli-single-instance
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.309970 dbm-agent-8.33.0/dbm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2582 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-04-21 09:08:54.000000 dbm-agent-8.33.0/dbm_agent.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.309970 dbm-agent-8.33.0/dbma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.33.0/dbma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.311970 dbm-agent-8.33.0/dbma/bil/
--rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.33.0/dbma/bil/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.33.0/dbma/bil/cmdexecutor.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/daemon.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/fs.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/fun.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.33.0/dbma/bil/net.py
--rw-r--r--   0 root         (0) root         (0)     5900 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/osuser.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/bil/sudos.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.311970 dbm-agent-8.33.0/dbma/components/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.33.0/dbma/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.312970 dbm-agent-8.33.0/dbma/components/mysql/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.33.0/dbma/components/mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.312970 dbm-agent-8.33.0/dbma/components/mysql/backups/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:54:14.000000 dbm-agent-8.33.0/dbma/components/mysql/backups/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1665 2023-04-11 11:19:32.000000 dbm-agent-8.33.0/dbma/components/mysql/backups/cloneplugin.py
--rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.33.0/dbma/components/mysql/commons.py
--rw-r--r--   0 root         (0) root         (0)    21000 2023-04-13 09:44:10.000000 dbm-agent-8.33.0/dbma/components/mysql/config.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/components/mysql/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15140 2023-04-11 07:41:26.000000 dbm-agent-8.33.0/dbma/components/mysql/install.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/components/mysql/instance.py
--rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.33.0/dbma/components/mysql/replica.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-04-11 08:19:15.000000 dbm-agent-8.33.0/dbma/components/mysql/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.313970 dbm-agent-8.33.0/dbma/components/mysql/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.33.0/dbma/components/mysql/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13670 2023-04-12 08:33:24.000000 dbm-agent-8.33.0/dbma/components/mysql/views/defaultsview.py
--rw-r--r--   0 root         (0) root         (0)     4375 2023-04-11 11:43:08.000000 dbm-agent-8.33.0/dbma/components/mysql/views/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.313970 dbm-agent-8.33.0/dbma/components/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.33.0/dbma/components/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.314970 dbm-agent-8.33.0/dbma/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.33.0/dbma/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.314970 dbm-agent-8.33.0/dbma/core/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.33.0/dbma/core/agent/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/core/agent/init.py
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/core/agent/upgrade.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-04-21 09:07:34.000000 dbm-agent-8.33.0/dbma/core/configs.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-07 07:23:16.000000 dbm-agent-8.33.0/dbma/core/exception.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/httpserver.py
--rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 03:16:26.000000 dbm-agent-8.33.0/dbma/core/messages.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.315970 dbm-agent-8.33.0/dbma/core/threads/
--rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/threads/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/threads/backends.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.315970 dbm-agent-8.33.0/dbma/core/views/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/core/views/__init__.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/views/dbmagentview.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.33.0/dbma/core/views/response.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.307970 dbm-agent-8.33.0/dbma/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.320970 dbm-agent-8.33.0/dbma/static/cnfs/
--rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/auto-inseption-db.sql
--rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/create-innodb-cluster.js
--rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.33.0/dbma/static/cnfs/init-5.7.x.sql
--rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 09:18:43.000000 dbm-agent-8.33.0/dbma/static/cnfs/init-8.0.x.sql
--rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/init-users.sql.jinja
--rw-r--r--   0 root         (0) root         (0)    10685 2023-04-03 07:33:25.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    10847 2023-04-03 07:45:13.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0-init-only.jinja
--rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18787 2023-04-13 09:47:14.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18789 2023-04-13 09:47:41.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)    18789 2023-04-21 09:06:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.33.0/dbma/static/cnfs/mysqld.service.jinja
--rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/zabbix-agentd.service
--rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/zabbix_agentd.conf.jinja
--rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/cnfs/zoo.cnf.jinja
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 09:08:54.320970 dbm-agent-8.33.0/dbma/static/sql-scripts/
--rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.33.0/dbma/static/sql-scripts/常用SQL.md
--rw-r--r--   0 root         (0) root         (0)      346 2023-04-21 09:07:07.000000 dbm-agent-8.33.0/dbma/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 09:08:54.321970 dbm-agent-8.33.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1897 2023-04-11 09:42:31.000000 dbm-agent-8.33.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.526351 dbm-agent-8.33.3/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-04-29 08:41:21.525351 dbm-agent-8.33.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4453 2023-04-11 12:20:06.000000 dbm-agent-8.33.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.512351 dbm-agent-8.33.3/bin/
+-rw-r--r--   0 root         (0) root         (0)      898 2023-04-11 03:20:19.000000 dbm-agent-8.33.3/bin/dbm-agent
+-rw-r--r--   0 root         (0) root         (0)      322 2023-04-06 12:14:18.000000 dbm-agent-8.33.3/bin/dbm-bt-conn-stack
+-rw-r--r--   0 root         (0) root         (0)      794 2023-04-11 03:20:38.000000 dbm-agent-8.33.3/bin/dbma-cli-init
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-04-29 08:15:51.000000 dbm-agent-8.33.3/bin/dbma-cli-redis
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-04-11 08:35:08.000000 dbm-agent-8.33.3/bin/dbma-cli-single-instance
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.513351 dbm-agent-8.33.3/dbm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      626 2023-04-29 08:41:21.000000 dbm-agent-8.33.3/dbm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-04-29 08:41:21.000000 dbm-agent-8.33.3/dbm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 08:41:21.000000 dbm-agent-8.33.3/dbm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2023-04-29 08:41:21.000000 dbm-agent-8.33.3/dbm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      221 2023-04-29 08:41:21.000000 dbm-agent-8.33.3/dbm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.513351 dbm-agent-8.33.3/dbma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-30 02:17:13.000000 dbm-agent-8.33.3/dbma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.514351 dbm-agent-8.33.3/dbma/bil/
+-rw-r--r--   0 root         (0) root         (0)      104 2023-04-07 07:23:15.000000 dbm-agent-8.33.3/dbma/bil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-04-07 07:23:15.000000 dbm-agent-8.33.3/dbma/bil/cmdexecutor.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/bil/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/bil/fs.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/bil/fun.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-04-10 03:49:50.000000 dbm-agent-8.33.3/dbma/bil/net.py
+-rw-r--r--   0 root         (0) root         (0)     6820 2023-04-29 08:19:09.000000 dbm-agent-8.33.3/dbma/bil/osuser.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/bil/sudos.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.515351 dbm-agent-8.33.3/dbma/components/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:28.000000 dbm-agent-8.33.3/dbma/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.516351 dbm-agent-8.33.3/dbma/components/mysql/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:20:47.000000 dbm-agent-8.33.3/dbma/components/mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.516351 dbm-agent-8.33.3/dbma/components/mysql/backups/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-11 08:54:14.000000 dbm-agent-8.33.3/dbma/components/mysql/backups/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-04-11 11:19:32.000000 dbm-agent-8.33.3/dbma/components/mysql/backups/cloneplugin.py
+-rw-r--r--   0 root         (0) root         (0)     5674 2023-04-11 08:23:03.000000 dbm-agent-8.33.3/dbma/components/mysql/commons.py
+-rw-r--r--   0 root         (0) root         (0)    21072 2023-04-28 07:22:47.000000 dbm-agent-8.33.3/dbma/components/mysql/config.py
+-rw-r--r--   0 root         (0) root         (0)      517 2023-04-24 11:29:32.000000 dbm-agent-8.33.3/dbma/components/mysql/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15167 2023-04-28 07:25:52.000000 dbm-agent-8.33.3/dbma/components/mysql/install.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/components/mysql/instance.py
+-rw-r--r--   0 root         (0) root         (0)     3996 2023-04-11 08:39:21.000000 dbm-agent-8.33.3/dbma/components/mysql/replica.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-04-28 09:01:15.000000 dbm-agent-8.33.3/dbma/components/mysql/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.516351 dbm-agent-8.33.3/dbma/components/mysql/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-29 08:25:42.000000 dbm-agent-8.33.3/dbma/components/mysql/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13670 2023-04-12 08:33:24.000000 dbm-agent-8.33.3/dbma/components/mysql/views/defaultsview.py
+-rw-r--r--   0 root         (0) root         (0)     4375 2023-04-11 11:43:08.000000 dbm-agent-8.33.3/dbma/components/mysql/views/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.517351 dbm-agent-8.33.3/dbma/components/orchestrator/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-23 08:32:56.000000 dbm-agent-8.33.3/dbma/components/orchestrator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-04-24 11:31:39.000000 dbm-agent-8.33.3/dbma/components/orchestrator/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-04-25 10:26:23.000000 dbm-agent-8.33.3/dbma/components/orchestrator/install.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.518351 dbm-agent-8.33.3/dbma/components/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-28 02:21:47.000000 dbm-agent-8.33.3/dbma/components/redis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      566 2023-04-28 09:33:50.000000 dbm-agent-8.33.3/dbma/components/redis/commons.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-04-29 08:28:15.000000 dbm-agent-8.33.3/dbma/components/redis/config.py
+-rw-r--r--   0 root         (0) root         (0)      550 2023-04-28 08:47:44.000000 dbm-agent-8.33.3/dbma/components/redis/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5980 2023-04-29 08:32:41.000000 dbm-agent-8.33.3/dbma/components/redis/install.py
+-rw-r--r--   0 root         (0) root         (0)     2312 2023-04-29 08:09:50.000000 dbm-agent-8.33.3/dbma/components/redis/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.519351 dbm-agent-8.33.3/dbma/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-11 07:21:13.000000 dbm-agent-8.33.3/dbma/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.519351 dbm-agent-8.33.3/dbma/core/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 06:58:11.000000 dbm-agent-8.33.3/dbma/core/agent/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/core/agent/init.py
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-07 07:23:16.000000 dbm-agent-8.33.3/dbma/core/agent/upgrade.py
+-rw-r--r--   0 root         (0) root         (0)     3679 2023-04-28 05:54:34.000000 dbm-agent-8.33.3/dbma/core/configs.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-28 05:39:01.000000 dbm-agent-8.33.3/dbma/core/exception.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-04-22 08:57:17.000000 dbm-agent-8.33.3/dbma/core/httpserver.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-12 03:16:26.000000 dbm-agent-8.33.3/dbma/core/messages.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-07 07:23:17.000000 dbm-agent-8.33.3/dbma/core/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.519351 dbm-agent-8.33.3/dbma/core/threads/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-04-07 07:23:17.000000 dbm-agent-8.33.3/dbma/core/threads/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-04-07 07:23:17.000000 dbm-agent-8.33.3/dbma/core/threads/backends.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.520351 dbm-agent-8.33.3/dbma/core/views/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/core/views/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-07 07:23:17.000000 dbm-agent-8.33.3/dbma/core/views/dbmagentview.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-04-07 07:23:17.000000 dbm-agent-8.33.3/dbma/core/views/response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.511351 dbm-agent-8.33.3/dbma/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.525351 dbm-agent-8.33.3/dbma/static/cnfs/
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/auto-inseption-db.sql
+-rw-r--r--   0 root         (0) root         (0)      168 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/create-innodb-cluster.js
+-rw-r--r--   0 root         (0) root         (0)      286 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/dbm-backup-proxyd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      385 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/dbm-monitor-gatewayd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      514 2023-04-06 08:26:15.000000 dbm-agent-8.33.3/dbma/static/cnfs/init-5.7.x.sql
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-04-23 03:55:41.000000 dbm-agent-8.33.3/dbma/static/cnfs/init-8.0.x.sql
+-rw-r--r--   0 root         (0) root         (0)     6681 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/init-users.sql.jinja
+-rw-r--r--   0 root         (0) root         (0)    10685 2023-04-03 07:33:25.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-5.7-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    10847 2023-04-03 07:45:13.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-5.7.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    14716 2023-04-03 03:33:55.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0-init-only.jinja
+-rw-r--r--   0 root         (0) root         (0)    17621 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.17.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17631 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.18.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17687 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.19.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.20.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17766 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.21.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.22.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.23.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.25.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.26.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.27.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.28.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17528 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.29.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    17799 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.30.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18787 2023-04-13 09:47:14.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.31.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18776 2023-04-28 07:24:00.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.32.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)    18774 2023-04-28 09:40:34.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.33.cnf.jinja
+-rw-r--r--   0 root         (0) root         (0)      465 2023-03-29 06:32:45.000000 dbm-agent-8.33.3/dbma/static/cnfs/mysqld.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      598 2023-04-29 08:25:25.000000 dbm-agent-8.33.3/dbma/static/cnfs/redis.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      710 2023-04-29 07:42:18.000000 dbm-agent-8.33.3/dbma/static/cnfs/redisd.service.jinja
+-rw-r--r--   0 root         (0) root         (0)      362 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/zabbix-agentd.service
+-rw-r--r--   0 root         (0) root         (0)    10464 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/zabbix_agentd.conf.jinja
+-rw-r--r--   0 root         (0) root         (0)      258 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/cnfs/zoo.cnf.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 08:41:21.525351 dbm-agent-8.33.3/dbma/static/sql-scripts/
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-03-09 09:18:42.000000 dbm-agent-8.33.3/dbma/static/sql-scripts/常用SQL.md
+-rw-r--r--   0 root         (0) root         (0)      346 2023-04-29 08:37:07.000000 dbm-agent-8.33.3/dbma/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 08:41:21.526351 dbm-agent-8.33.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-28 09:25:35.000000 dbm-agent-8.33.3/setup.py
```

### Comparing `dbm-agent-8.33.0/PKG-INFO` & `dbm-agent-8.33.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.0
+Version: 8.33.3
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.*
```

### Comparing `dbm-agent-8.33.0/README.md` & `dbm-agent-8.33.3/README.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/bin/dbm-agent` & `dbm-agent-8.33.3/bin/dbm-agent`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/bin/dbma-cli-init` & `dbm-agent-8.33.3/bin/dbma-cli-init`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/bin/dbma-cli-single-instance` & `dbm-agent-8.33.3/bin/dbma-cli-single-instance`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbm_agent.egg-info/PKG-INFO` & `dbm-agent-8.33.3/dbm_agent.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: dbm-agent
-Version: 8.33.0
+Version: 8.33.3
 Summary: dbm-agent 数据库管理中心客户端程序
 Home-page: https://github.com/Neeky/dbm-agent
 Author: Neeky
 Author-email: neeky@live.com
 Maintainer: Neeky
 Maintainer-email: neeky@live.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8.*
```

### Comparing `dbm-agent-8.33.0/dbm_agent.egg-info/SOURCES.txt` & `dbm-agent-8.33.3/dbm_agent.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.md
 setup.py
 bin/dbm-agent
 bin/dbm-bt-conn-stack
 bin/dbma-cli-init
+bin/dbma-cli-redis
 bin/dbma-cli-single-instance
 dbm_agent.egg-info/PKG-INFO
 dbm_agent.egg-info/SOURCES.txt
 dbm_agent.egg-info/dependency_links.txt
 dbm_agent.egg-info/requires.txt
 dbm_agent.egg-info/top_level.txt
 dbma/__init__.py
@@ -29,15 +30,23 @@
 dbma/components/mysql/replica.py
 dbma/components/mysql/source.py
 dbma/components/mysql/backups/__init__.py
 dbma/components/mysql/backups/cloneplugin.py
 dbma/components/mysql/views/__init__.py
 dbma/components/mysql/views/defaultsview.py
 dbma/components/mysql/views/handlers.py
+dbma/components/orchestrator/__init__.py
+dbma/components/orchestrator/exceptions.py
+dbma/components/orchestrator/install.py
 dbma/components/redis/__init__.py
+dbma/components/redis/commons.py
+dbma/components/redis/config.py
+dbma/components/redis/exceptions.py
+dbma/components/redis/install.py
+dbma/components/redis/systemd.py
 dbma/core/__init__.py
 dbma/core/configs.py
 dbma/core/exception.py
 dbma/core/httpserver.py
 dbma/core/messages.py
 dbma/core/router.py
 dbma/core/agent/__init__.py
@@ -71,11 +80,13 @@
 dbma/static/cnfs/mysql-8.0.28.cnf.jinja
 dbma/static/cnfs/mysql-8.0.29.cnf.jinja
 dbma/static/cnfs/mysql-8.0.30.cnf.jinja
 dbma/static/cnfs/mysql-8.0.31.cnf.jinja
 dbma/static/cnfs/mysql-8.0.32.cnf.jinja
 dbma/static/cnfs/mysql-8.0.33.cnf.jinja
 dbma/static/cnfs/mysqld.service.jinja
+dbma/static/cnfs/redis.conf.jinja
+dbma/static/cnfs/redisd.service.jinja
 dbma/static/cnfs/zabbix-agentd.service
 dbma/static/cnfs/zabbix_agentd.conf.jinja
 dbma/static/cnfs/zoo.cnf.jinja
 dbma/static/sql-scripts/常用SQL.md
```

### Comparing `dbm-agent-8.33.0/dbma/bil/daemon.py` & `dbm-agent-8.33.3/dbma/bil/daemon.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/bil/fs.py` & `dbm-agent-8.33.3/dbma/bil/fs.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/bil/net.py` & `dbm-agent-8.33.3/dbma/bil/net.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/bil/osuser.py` & `dbm-agent-8.33.3/dbma/bil/osuser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf8 -*-
 
 """
 实现操作系统用户的相关操作
 """
-
+import logging
 import os
 import pwd
 import grp
 from dbma.bil.cmdexecutor import exe_shell_cmd
 from dbma.bil.sudos import sudo
 
 
@@ -183,19 +183,20 @@
         """
         if (self.group is not None) and (not self.group.is_exists()):
             self.group.create()
         Identify.create(self)
 
     def chown(self, path, recursive=True):
         """ """
+        logging.info("execute User.chown.")
         if recursive == True:
             cmd = f"chown -R {str(self)} {path}"
         else:
             cmd = f"chown {str(self)} {path}"
-
+        logging.info(cmd)
         with sudo():
             exe_shell_cmd(cmd)
 
     def __str__(self):
         """
         返回 user:group 的形式
         """
@@ -247,14 +248,51 @@
         if self.group.is_exists() == False:
             self.group.create()
 
         BaseUser.create(self)
 
     def __str__(self):
         return f"{self.name}:{self.group}"
+
+
+class RedisGroup(BaseGroup):
+    """Redis 组"""
+
+    def __init__(self, name="redis"):
+        BaseGroup.__init__(self, name)
+
+
+class RedisUser(BaseUser):
+    """Redis 用户"""
+
+    # Redis 端口
+    port = 6379
+    # 所有的 Redis 都共用一个 Redis 组
+    group = RedisGroup()
+
+    def __init__(self, port: int = 6379):
+        """根据 Redis 监听的端口创建用户
+
+        Parameter
+        ---------
+            port: int
+        """
+        self.name = f"redis{port}"
+        self.port = port
+        BaseUser.__init__(self, self.name)
+
+    def create(self):
+        """创建 Redis 实例用户(如果属组不存在就先创建属组)"""
+        if self.group.is_exists() == False:
+            self.group.create()
+
+        BaseUser.create(self)
+
+    def __str__(self):
+        return f"{self.name}:{self.group}"
 
 
 class RootGroup(BaseGroup):
     """ """
 
     def __init__(self, name="root"):
         BaseGroup.__init__(self, name)
```

### Comparing `dbm-agent-8.33.0/dbma/bil/sudos.py` & `dbm-agent-8.33.3/dbma/bil/sudos.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/backups/cloneplugin.py` & `dbm-agent-8.33.3/dbma/components/mysql/backups/cloneplugin.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/commons.py` & `dbm-agent-8.33.3/dbma/components/mysql/commons.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/config.py` & `dbm-agent-8.33.3/dbma/components/mysql/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import os
 import json
 import logging
 import random
 from enum import Enum
 from pathlib import Path
 from jinja2 import Template
+from datetime import datetime
 from dataclasses import dataclass, asdict
 from dbma.core import messages
 from dbma.bil.fun import fname
 from dbma.core.configs import dbm_agent_config
 from dbma.components.mysql.exceptions import MySQLTemplateFileNotExistsException
 
 
@@ -38,14 +39,15 @@
 class MySQLConfig(object):
     """MySQL 配置文件的动态生成"""
 
     # basic
     basedir: str = None
     port: str = None
     innodb_buffer_pool_size: str = None
+    now: str = datetime.now().isoformat()
 
     # region global-config
     version: str = None
     user: str = None
     datadir: str = None
     server_id: int = None
     bind_address: str = "*"
```

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/install.py` & `dbm-agent-8.33.3/dbma/components/mysql/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,14 +368,15 @@
 
     config_file = "/etc/my-{}.cnf".format(port)
     config_backup_file = datadir / "my-{}.cnf-backup-{}".format(port, suffix)
     logging.info(messages.MOVE_FILE_TO.format(config_file, config_backup_file))
 
     # 备份文件
     shutil.copyfile(config_file, config_backup_file)
+    os.remove(config_file)
 
     logging.info(messages.FUN_ENDS.format(fname()))
 
 
 def decompression_pkg(pkg: Path = default_pkg):
     """解压安装包到 /usr/local/
```

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/instance.py` & `dbm-agent-8.33.3/dbma/components/mysql/instance.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/replica.py` & `dbm-agent-8.33.3/dbma/components/mysql/replica.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/views/defaultsview.py` & `dbm-agent-8.33.3/dbma/components/mysql/views/defaultsview.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/components/mysql/views/handlers.py` & `dbm-agent-8.33.3/dbma/components/mysql/views/handlers.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/core/agent/init.py` & `dbm-agent-8.33.3/dbma/core/agent/init.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/core/configs.py` & `dbm-agent-8.33.3/dbma/core/configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,30 +9,29 @@
 import json
 import atexit
 from pathlib import Path
 from dataclasses import dataclass, asdict
 from dbma.version import VERSION
 from dbma.bil.osuser import DBMAUser
 
-# TODO
-# 这里之后要改成 dbma.core.version 文件中的 VERSION 值
 
 DBM_AGENT_BASE_DIR = Path("/usr/local/dbm-agent/")
 DBM_AGENT_ETC_DIR = DBM_AGENT_BASE_DIR / "etc"
 CONFIG_FILE_PATH = DBM_AGENT_BASE_DIR / "etc/dbm-agent.json"
 
 
 @dataclass
 class DBMAgentConfig(object):
     """ """
 
     host: str = "127.0.0.1"
     port: int = 8086
     version: str = VERSION
     dbmcenter_url_prefix: str = "http://127.0.0.1:8080"
+    dbmcenter_token: str = ""
     pid_file: str = "/tmp/dbm-agent.pid"
     log_level: str = "info"
     log_file: str = "/tmp/dbm-agent.log"
 
     # backends_xxx 后端线程运行周期
     backends_register_time_interval: int = 15
 
@@ -50,14 +49,17 @@
     mysql_dbma_password: str = "dbma@0352"
     # mysql_consts
     mysql_repl_user: str = "repl"
     mysql_repl_password: str = "2-4nw9A0-459st36"
     mysql_init_cnf: str = "/tmp/mysql-init.cnf"
     mysql_init_user_sql_file: str = "/tmp/mysql-init-user.sql"
 
+    # redis
+    redis_default_version: str = "7.0.11"
+
     def make_register_data(self):
         """ """
         return {"host": self.host, "port": self.port, "version": self.version}
 
     # 保存配置到磁盘
     def sync_to_disk(self):
         """对象的生命周期结束的时候保存信息到磁盘"""
@@ -109,15 +111,15 @@
     def __new__(cls, *args, **kw):
         if cls._instance is None:
             cls._instance = object.__new__(cls, *args, **kw)
         return cls._instance
 
 
 def _auto_save_to_disk():
-    """ """
+    """在 dbm-agent 程序退出的时候把配置对象持久化到配置文件"""
     if DBM_AGENT_BASE_DIR.exists():
         dbm_user = DBMAUser()
         dbm_user.chown(DBM_AGENT_BASE_DIR)
         dbm_agent_config.version = VERSION
         dbm_agent_config.sync_to_disk()
         dbm_user.chown(DBM_AGENT_BASE_DIR)
```

### Comparing `dbm-agent-8.33.0/dbma/core/messages.py` & `dbm-agent-8.33.3/dbma/core/messages.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/core/threads/backends.py` & `dbm-agent-8.33.3/dbma/core/threads/backends.py`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/auto-inseption-db.sql` & `dbm-agent-8.33.3/dbma/static/cnfs/auto-inseption-db.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/init-5.7.x.sql` & `dbm-agent-8.33.3/dbma/static/cnfs/init-5.7.x.sql`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/init-users.sql.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/init-users.sql.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7-init-only.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-5.7-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-5.7.25.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-5.7.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0-init-only.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0-init-only.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.17.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.17.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.18.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.18.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.19.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.19.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.20.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.20.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.21.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.21.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.22.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.22.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.23.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.23.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.25.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.25.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.26.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.26.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.27.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.27.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.28.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.28.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.29.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.29.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.30.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.30.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.31.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.31.cnf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.32.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.32.cnf.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -294,12 +294,12 @@
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
 # base on mysql-8.0.32
-# generated by https://www.sqlpy.com 2023年03月30日 23:45
+# generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/mysql-8.0.33.cnf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/mysql-8.0.33.cnf.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -294,12 +294,11 @@
 performance_schema_consumer_events_waits_history                        =ON  
 performance_schema_consumer_events_waits_history_long                   =OFF 
 performance-schema-instrument                                           ='memory/%=COUNTED'
 
 
 # -- ~ _ ~    ~ _ ~     ~ _ ~ -- 
 # base on mysql-8.0.33
-# generated by https://www.sqlpy.com 2023年04月21日 23:45
+# generated by https://www.sqlpy.com at {{now}}
 # wechat: jianglegege
 # email: 1721900707@qq.com
 # -- ~ _ ~ --
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `dbm-agent-8.33.0/dbma/static/cnfs/zabbix_agentd.conf.jinja` & `dbm-agent-8.33.3/dbma/static/cnfs/zabbix_agentd.conf.jinja`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/dbma/static/sql-scripts/常用SQL.md` & `dbm-agent-8.33.3/dbma/static/sql-scripts/常用SQL.md`

 * *Files identical despite different names*

### Comparing `dbm-agent-8.33.0/setup.py` & `dbm-agent-8.33.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,40 +28,41 @@
     author_email="neeky@live.com",
     maintainer="Neeky",
     maintainer_email="neeky@live.com",
     scripts=[
         "bin/dbm-agent",
         "bin/dbma-cli-single-instance",
         "bin/dbma-cli-init",
+        "bin/dbma-cli-redis",
         "bin/dbm-bt-conn-stack",
     ],
     packages=[
         "dbma",
         "dbma/core",
         "dbma/core/views",
         "dbma/core/agent",
         "dbma/core/threads",
         "dbma/bil",
         "dbma/components",
         "dbma/components/mysql",
-        "dbma/components/redis",
         "dbma/components/mysql/views",
         "dbma/components/mysql/backups",
+        "dbma/components/redis",
+        "dbma/components/orchestrator",
     ],
     package_data={"dbma": ["static/cnfs/*", "static/sql-scripts/*"]},
     url="https://github.com/Neeky/dbm-agent",
     install_requires=[
         "Jinja2>=2.10.1",
         "mysql-connector-python>=8.0.31",
         "psutil>=5.6.6",
         "requests>=2.22.0",
         "distro>=1.4.0",
         "aiohttp>=3.8.1",
     ],
-    python_requires=">=3.8.*",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Operating System :: POSIX",
         "Operating System :: MacOS :: MacOS X",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

