# Comparing `tmp/nua_orchestrator-0.5.16.tar.gz` & `tmp/nua_orchestrator-0.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_orchestrator-0.5.16.tar", max compression
+gzip compressed data, was "nua_orchestrator-0.5.17.tar", max compression
```

## Comparing `nua_orchestrator-0.5.16.tar` & `nua_orchestrator-0.5.17.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     3876 2023-04-29 09:12:48.090789 nua_orchestrator-0.5.16/README.md
--rw-r--r--   0        0        0     2630 2023-04-29 10:19:23.882272 nua_orchestrator-0.5.16/pyproject.toml
--rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.16/src/nua/orchestrator/__init__.py
--rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.16/src/nua/orchestrator/__main__.py
--rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.16/src/nua/orchestrator/admin_local.py
--rw-r--r--   0        0        0    51749 2023-04-29 09:12:48.108878 nua_orchestrator-0.5.16/src/nua/orchestrator/app_deployment.py
--rw-r--r--   0        0        0    13298 2023-04-29 09:12:48.109438 nua_orchestrator-0.5.16/src/nua/orchestrator/app_instance.py
--rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.16/src/nua/orchestrator/app_management.py
--rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.16/src/nua/orchestrator/assign/__init__.py
--rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.16/src/nua/orchestrator/assign/db_utils.py
--rw-r--r--   0        0        0     3208 2023-04-29 09:12:48.109707 nua_orchestrator-0.5.16/src/nua/orchestrator/assign/engine.py
--rw-r--r--   0        0        0     6382 2023-04-29 09:12:48.109928 nua_orchestrator-0.5.16/src/nua/orchestrator/assign/evaluators.py
--rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.16/src/nua/orchestrator/backup/__init__.py
--rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.16/src/nua/orchestrator/backup/backup_engine.py
--rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.16/src/nua/orchestrator/backup/backup_functions.py
--rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.16/src/nua/orchestrator/backup/backup_report.py
--rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.16/src/nua/orchestrator/bootstrap/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-26 08:44:27.773025 nua_orchestrator-0.5.16/src/nua/orchestrator/bootstrap/bootstrap.py
--rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/__init__.py
--rw-r--r--   0        0        0     2566 2023-04-29 09:12:48.110171 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/certbot.py
--rw-r--r--   0        0        0     4250 2023-04-29 09:12:48.110411 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/commands.py
--rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/config/__init__.py
--rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/config/cli.ini
--rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
--rw-r--r--   0        0        0     2507 2023-04-26 08:44:27.773490 nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/installer.py
--rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/api.py
--rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/backup.py
--rw-r--r--   0        0        0     2034 2023-04-29 09:12:48.110610 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/deploy_remove.py
--rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/restore.py
--rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/start_stop.py
--rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/status.py
--rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/configuration.py
--rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/debug.py
--rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/init.py
--rw-r--r--   0        0        0     6672 2023-04-29 09:12:48.110776 nua_orchestrator-0.5.16/src/nua/orchestrator/cli/main.py
--rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.16/src/nua/orchestrator/config.py
--rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.16/src/nua/orchestrator/constants.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.16/src/nua/orchestrator/db/__init__.py
--rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.16/src/nua/orchestrator/db/create.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/__init__.py
--rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/auth.py
--rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/base.py
--rw-r--r--   0        0        0     2073 2023-04-26 08:53:06.277388 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/deployconfig.py
--rw-r--r--   0        0        0      856 2023-04-26 08:53:06.277587 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/host.py
--rw-r--r--   0        0        0     1033 2023-04-26 08:53:06.277787 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/image.py
--rw-r--r--   0        0        0     4253 2023-04-26 08:53:06.278246 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/instance.py
--rw-r--r--   0        0        0     1602 2023-04-26 08:53:06.278463 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/setting.py
--rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/user_count.py
--rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.16/src/nua/orchestrator/db/session.py
--rw-r--r--   0        0        0    16885 2023-04-29 09:12:48.111070 nua_orchestrator-0.5.16/src/nua/orchestrator/db/store.py
--rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.16/src/nua/orchestrator/db_migration/__init__.py
--rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.16/src/nua/orchestrator/db_migration/migrations.py
--rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.16/src/nua/orchestrator/db_migration/tools.py
--rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/__init__.py
--rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mariadb.json
--rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mariadb.py
--rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mongo.json
--rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mongo.py
--rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/postgres.json
--rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/postgres.py
--rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/redis-cache.json
--rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/redis-cache.py
--rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.16/src/nua/orchestrator/db_utils/__init__.py
--rw-r--r--   0        0        0     7072 2023-04-29 09:12:48.111345 nua_orchestrator-0.5.16/src/nua/orchestrator/db_utils/mariadb_utils.py
--rw-r--r--   0        0        0     8128 2023-04-29 09:12:48.111558 nua_orchestrator-0.5.16/src/nua/orchestrator/db_utils/postgres_utils.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.16/src/nua/orchestrator/default_conf/__init__.py
--rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.16/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
--rw-r--r--   0        0        0    11985 2023-04-29 09:12:48.111822 nua_orchestrator-0.5.16/src/nua/orchestrator/deploy_utils.py
--rw-r--r--   0        0        0    18157 2023-04-29 09:12:48.112112 nua_orchestrator-0.5.16/src/nua/orchestrator/docker_utils.py
--rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.16/src/nua/orchestrator/domain_split.py
--rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.16/src/nua/orchestrator/healthcheck.py
--rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.16/src/nua/orchestrator/higher_package.py
--rw-r--r--   0        0        0     1413 2023-04-29 09:12:48.112276 nua_orchestrator-0.5.16/src/nua/orchestrator/internal_secrets.py
--rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.16/src/nua/orchestrator/net_utils/__init__.py
--rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.16/src/nua/orchestrator/net_utils/external_ip.py
--rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.16/src/nua/orchestrator/net_utils/ports.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/__init__.py
--rw-r--r--   0        0        0     1622 2023-04-29 09:12:48.112428 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/cmd.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/html/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/html/css/__init__.py
--rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/html/css/style.css
--rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/html/index.html
--rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/installer.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/__init__.py
--rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/default_site
--rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/http_located.j2
--rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/http_not_located.j2
--rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/https_located.j2
--rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/https_not_located.j2
--rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
--rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/nginx.conf
--rw-r--r--   0        0        0     4895 2023-04-29 09:12:48.112586 nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/utils.py
--rw-r--r--   0        0        0     4621 2023-04-26 08:44:27.776287 nua_orchestrator-0.5.16/src/nua/orchestrator/nua_db_setup.py
--rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.16/src/nua/orchestrator/nua_env.py
--rw-r--r--   0        0        0     1362 2023-04-29 09:12:48.112730 nua_orchestrator-0.5.16/src/nua/orchestrator/persistent.py
--rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.16/src/nua/orchestrator/port_normalization.py
--rw-r--r--   0        0        0     3349 2023-04-29 09:12:48.112968 nua_orchestrator-0.5.16/src/nua/orchestrator/register_plugins.py
--rw-r--r--   0        0        0     2830 2023-04-29 09:12:48.113193 nua_orchestrator-0.5.16/src/nua/orchestrator/registry.py
--rw-r--r--   0        0        0    15805 2023-04-29 09:12:48.113413 nua_orchestrator-0.5.16/src/nua/orchestrator/resource.py
--rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.16/src/nua/orchestrator/resource_deps.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/__init__.py
--rw-r--r--   0        0        0      307 2023-04-29 09:12:48.113562 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/deactivate_all_instances.py
--rw-r--r--   0        0        0      263 2023-04-29 09:12:48.113700 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/docker_list_all.py
--rw-r--r--   0        0        0     1211 2023-04-29 09:12:48.113837 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/docker_remove_all.py
--rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/list_instances.py
--rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/mariadb_restore.py
--rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/print_instances.py
--rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/print_mounted_volumes.py
--rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/print_used_ports.py
--rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/set_pg_pwd.py
--rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.16/src/nua/orchestrator/search_cmd.py
--rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.16/src/nua/orchestrator/services/__init__.py
--rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.16/src/nua/orchestrator/services/mariadb.py
--rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.16/src/nua/orchestrator/services/postgres.py
--rw-r--r--   0        0        0     1109 2023-04-29 09:12:48.114065 nua_orchestrator-0.5.16/src/nua/orchestrator/services/service_base.py
--rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.16/src/nua/orchestrator/services/service_loader.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.16/src/nua/orchestrator/util/__init__.py
--rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.16/src/nua/orchestrator/util/deep_access_dict.py
--rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.16/src/nua/orchestrator/util/deep_update.py
--rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.16/src/nua/orchestrator/utils.py
--rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.16/src/nua/orchestrator/version.py
--rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.16/src/nua/orchestrator/volume.py
--rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.16/PKG-INFO
+-rw-r--r--   0        0        0     3876 2023-04-29 09:12:48.090789 nua_orchestrator-0.5.17/README.md
+-rw-r--r--   0        0        0     2630 2023-04-29 10:37:33.246599 nua_orchestrator-0.5.17/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.17/src/nua/orchestrator/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.17/src/nua/orchestrator/__main__.py
+-rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.17/src/nua/orchestrator/admin_local.py
+-rw-r--r--   0        0        0    51749 2023-04-29 09:12:48.108878 nua_orchestrator-0.5.17/src/nua/orchestrator/app_deployment.py
+-rw-r--r--   0        0        0    13298 2023-04-29 09:12:48.109438 nua_orchestrator-0.5.17/src/nua/orchestrator/app_instance.py
+-rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.17/src/nua/orchestrator/app_management.py
+-rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.17/src/nua/orchestrator/assign/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.17/src/nua/orchestrator/assign/db_utils.py
+-rw-r--r--   0        0        0     3208 2023-04-29 09:12:48.109707 nua_orchestrator-0.5.17/src/nua/orchestrator/assign/engine.py
+-rw-r--r--   0        0        0     6382 2023-04-29 09:12:48.109928 nua_orchestrator-0.5.17/src/nua/orchestrator/assign/evaluators.py
+-rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.17/src/nua/orchestrator/backup/__init__.py
+-rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.17/src/nua/orchestrator/backup/backup_engine.py
+-rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.17/src/nua/orchestrator/backup/backup_functions.py
+-rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.17/src/nua/orchestrator/backup/backup_report.py
+-rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.17/src/nua/orchestrator/bootstrap/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-26 08:44:27.773025 nua_orchestrator-0.5.17/src/nua/orchestrator/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/__init__.py
+-rw-r--r--   0        0        0     2566 2023-04-29 09:12:48.110171 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/certbot.py
+-rw-r--r--   0        0        0     4250 2023-04-29 09:12:48.110411 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/commands.py
+-rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/config/__init__.py
+-rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/config/cli.ini
+-rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
+-rw-r--r--   0        0        0     2507 2023-04-26 08:44:27.773490 nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/installer.py
+-rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/api.py
+-rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/backup.py
+-rw-r--r--   0        0        0     2034 2023-04-29 09:12:48.110610 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/deploy_remove.py
+-rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/restore.py
+-rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/start_stop.py
+-rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/status.py
+-rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/configuration.py
+-rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/debug.py
+-rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/init.py
+-rw-r--r--   0        0        0     6672 2023-04-29 09:12:48.110776 nua_orchestrator-0.5.17/src/nua/orchestrator/cli/main.py
+-rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.17/src/nua/orchestrator/config.py
+-rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.17/src/nua/orchestrator/constants.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.17/src/nua/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.17/src/nua/orchestrator/db/create.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/__init__.py
+-rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/auth.py
+-rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/base.py
+-rw-r--r--   0        0        0     2073 2023-04-26 08:53:06.277388 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/deployconfig.py
+-rw-r--r--   0        0        0      856 2023-04-26 08:53:06.277587 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/host.py
+-rw-r--r--   0        0        0     1033 2023-04-26 08:53:06.277787 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/image.py
+-rw-r--r--   0        0        0     4253 2023-04-26 08:53:06.278246 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/instance.py
+-rw-r--r--   0        0        0     1602 2023-04-26 08:53:06.278463 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/setting.py
+-rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/user_count.py
+-rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.17/src/nua/orchestrator/db/session.py
+-rw-r--r--   0        0        0    16885 2023-04-29 09:12:48.111070 nua_orchestrator-0.5.17/src/nua/orchestrator/db/store.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.17/src/nua/orchestrator/db_migration/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.17/src/nua/orchestrator/db_migration/migrations.py
+-rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.17/src/nua/orchestrator/db_migration/tools.py
+-rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/__init__.py
+-rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mariadb.json
+-rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mariadb.py
+-rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mongo.json
+-rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mongo.py
+-rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/postgres.json
+-rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/postgres.py
+-rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/redis-cache.json
+-rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/redis-cache.py
+-rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.17/src/nua/orchestrator/db_utils/__init__.py
+-rw-r--r--   0        0        0     7072 2023-04-29 09:12:48.111345 nua_orchestrator-0.5.17/src/nua/orchestrator/db_utils/mariadb_utils.py
+-rw-r--r--   0        0        0     8128 2023-04-29 09:12:48.111558 nua_orchestrator-0.5.17/src/nua/orchestrator/db_utils/postgres_utils.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.17/src/nua/orchestrator/default_conf/__init__.py
+-rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.17/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
+-rw-r--r--   0        0        0    11985 2023-04-29 09:12:48.111822 nua_orchestrator-0.5.17/src/nua/orchestrator/deploy_utils.py
+-rw-r--r--   0        0        0    18157 2023-04-29 09:12:48.112112 nua_orchestrator-0.5.17/src/nua/orchestrator/docker_utils.py
+-rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.17/src/nua/orchestrator/domain_split.py
+-rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.17/src/nua/orchestrator/healthcheck.py
+-rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.17/src/nua/orchestrator/higher_package.py
+-rw-r--r--   0        0        0     1413 2023-04-29 09:12:48.112276 nua_orchestrator-0.5.17/src/nua/orchestrator/internal_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.17/src/nua/orchestrator/net_utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.17/src/nua/orchestrator/net_utils/external_ip.py
+-rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.17/src/nua/orchestrator/net_utils/ports.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/__init__.py
+-rw-r--r--   0        0        0     1622 2023-04-29 09:12:48.112428 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/cmd.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/html/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/html/css/__init__.py
+-rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/html/css/style.css
+-rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/html/index.html
+-rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/installer.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/__init__.py
+-rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/default_site
+-rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/http_located.j2
+-rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/http_not_located.j2
+-rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/https_located.j2
+-rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/https_not_located.j2
+-rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
+-rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/nginx.conf
+-rw-r--r--   0        0        0     4895 2023-04-29 09:12:48.112586 nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/utils.py
+-rw-r--r--   0        0        0     4621 2023-04-26 08:44:27.776287 nua_orchestrator-0.5.17/src/nua/orchestrator/nua_db_setup.py
+-rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.17/src/nua/orchestrator/nua_env.py
+-rw-r--r--   0        0        0     1362 2023-04-29 09:12:48.112730 nua_orchestrator-0.5.17/src/nua/orchestrator/persistent.py
+-rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.17/src/nua/orchestrator/port_normalization.py
+-rw-r--r--   0        0        0     3349 2023-04-29 09:12:48.112968 nua_orchestrator-0.5.17/src/nua/orchestrator/register_plugins.py
+-rw-r--r--   0        0        0     2830 2023-04-29 09:12:48.113193 nua_orchestrator-0.5.17/src/nua/orchestrator/registry.py
+-rw-r--r--   0        0        0    15805 2023-04-29 09:12:48.113413 nua_orchestrator-0.5.17/src/nua/orchestrator/resource.py
+-rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.17/src/nua/orchestrator/resource_deps.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-29 09:12:48.113562 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/deactivate_all_instances.py
+-rw-r--r--   0        0        0      263 2023-04-29 09:12:48.113700 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/docker_list_all.py
+-rw-r--r--   0        0        0     1211 2023-04-29 09:12:48.113837 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/docker_remove_all.py
+-rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/list_instances.py
+-rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/mariadb_restore.py
+-rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/print_instances.py
+-rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/print_mounted_volumes.py
+-rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/print_used_ports.py
+-rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/set_pg_pwd.py
+-rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.17/src/nua/orchestrator/search_cmd.py
+-rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.17/src/nua/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.17/src/nua/orchestrator/services/mariadb.py
+-rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.17/src/nua/orchestrator/services/postgres.py
+-rw-r--r--   0        0        0     1109 2023-04-29 09:12:48.114065 nua_orchestrator-0.5.17/src/nua/orchestrator/services/service_base.py
+-rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.17/src/nua/orchestrator/services/service_loader.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.17/src/nua/orchestrator/util/__init__.py
+-rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.17/src/nua/orchestrator/util/deep_access_dict.py
+-rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.17/src/nua/orchestrator/util/deep_update.py
+-rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.17/src/nua/orchestrator/utils.py
+-rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.17/src/nua/orchestrator/version.py
+-rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.17/src/nua/orchestrator/volume.py
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.17/PKG-INFO
```

### Comparing `nua_orchestrator-0.5.16/README.md` & `nua_orchestrator-0.5.17/README.md`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/pyproject.toml` & `nua_orchestrator-0.5.17/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-orchestrator"
-version = "0.5.16"
+version = "0.5.17"
 description = "Nua orchestrator - local implementation"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -28,15 +28,15 @@
 nua-deactivate-all = "nua.orchestrator.scripts.deactivate_all_instances:main"
 nua-docker-list-all = "nua.orchestrator.scripts.docker_list_all:main"
 nua-docker-rm-all = "nua.orchestrator.scripts.docker_remove_all:main"
 nua_test_services = "nua.orchestrator.service:test"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.16"
+nua-lib = "=0.5.17"
 SQLAlchemy-serializer = "^1.4.1"
 SQLAlchemy = "^1.4.36"
 psycopg2-binary = "^2.9.3"
 setuptools = "*"
 wheel = "*"
 tomli = "^2"
 paramiko = "^2.11.0"
```

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/admin_local.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/admin_local.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/app_deployment.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/app_deployment.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/app_instance.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/app_instance.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/app_management.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/app_management.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/assign/engine.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/assign/engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/assign/evaluators.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/assign/evaluators.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/backup/backup_engine.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/backup/backup_engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/backup/backup_functions.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/backup/backup_functions.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/backup/backup_report.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/backup/backup_report.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/bootstrap/bootstrap.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/certbot.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/certbot.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/commands.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/commands.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf` & `nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/certbot/installer.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/certbot/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/api.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/deploy_remove.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/deploy_remove.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/restore.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/start_stop.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/start_stop.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/commands/status.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/configuration.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/debug.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/debug.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/init.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/init.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/cli/main.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/cli/main.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/auth.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/auth.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/deployconfig.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/deployconfig.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/host.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/host.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/image.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/image.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/instance.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/instance.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/model/setting.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/model/setting.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db/store.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db/store.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_migration/tools.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_migration/tools.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mariadb.json` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mariadb.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mariadb.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mariadb.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/mongo.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/mongo.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/postgres.json` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/postgres.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/postgres.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/redis-cache.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/redis-cache.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_plugins/sqlite.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_plugins/sqlite.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_utils/mariadb_utils.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_utils/mariadb_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/db_utils/postgres_utils.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/db_utils/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/default_conf/nua_defaults_settings.toml` & `nua_orchestrator-0.5.17/src/nua/orchestrator/default_conf/nua_defaults_settings.toml`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/deploy_utils.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/deploy_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/docker_utils.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/docker_utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/domain_split.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/domain_split.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/healthcheck.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/healthcheck.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/higher_package.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/higher_package.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/internal_secrets.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/internal_secrets.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/cmd.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/cmd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/html/css/style.css` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/html/css/style.css`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/html/index.html` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/html/index.html`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/installer.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/default_site` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/default_site`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/http_located.j2` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/http_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/http_not_located.j2` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/http_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/https_located.j2` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/https_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/https_not_located.j2` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/https_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/templates/nginx.conf` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nginx/utils.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nginx/utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nua_db_setup.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nua_db_setup.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/nua_env.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/nua_env.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/persistent.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/persistent.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/port_normalization.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/port_normalization.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/register_plugins.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/register_plugins.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/registry.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/registry.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/resource.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/resource.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/resource_deps.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/resource_deps.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/docker_remove_all.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/docker_remove_all.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/mariadb_restore.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/mariadb_restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/print_instances.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/print_instances.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/scripts/set_pg_pwd.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/scripts/set_pg_pwd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/search_cmd.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/search_cmd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/services/postgres.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/services/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/services/service_base.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/services/service_base.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/services/service_loader.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/services/service_loader.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/util/deep_access_dict.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/util/deep_access_dict.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/utils.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/src/nua/orchestrator/volume.py` & `nua_orchestrator-0.5.17/src/nua/orchestrator/volume.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.16/PKG-INFO` & `nua_orchestrator-0.5.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nua-orchestrator
-Version: 0.5.16
+Version: 0.5.17
 Summary: Nua orchestrator - local implementation
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=1.4.36,<2.0.0)
 Requires-Dist: SQLAlchemy-serializer (>=1.4.1,<2.0.0)
 Requires-Dist: docker (>=6,<7)
-Requires-Dist: nua-lib (==0.5.16)
+Requires-Dist: nua-lib (==0.5.17)
 Requires-Dist: paramiko (>=2.11.0,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2,<3)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
```

