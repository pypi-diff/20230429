# Comparing `tmp/nua_orchestrator-0.5.14.tar.gz` & `tmp/nua_orchestrator-0.5.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_orchestrator-0.5.14.tar", max compression
+gzip compressed data, was "nua_orchestrator-0.5.15.tar", max compression
```

## Comparing `nua_orchestrator-0.5.14.tar` & `nua_orchestrator-0.5.15.tar`

### file list

```diff
@@ -1,126 +1,126 @@
--rw-r--r--   0        0        0     3789 2023-04-24 21:25:56.870296 nua_orchestrator-0.5.14/README.md
--rw-r--r--   0        0        0     2721 2023-04-26 06:46:56.050490 nua_orchestrator-0.5.14/pyproject.toml
--rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.14/src/nua/orchestrator/__init__.py
--rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.14/src/nua/orchestrator/__main__.py
--rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.14/src/nua/orchestrator/admin_local.py
--rw-r--r--   0        0        0    50949 2023-04-26 06:41:08.609843 nua_orchestrator-0.5.14/src/nua/orchestrator/app_deployment.py
--rw-r--r--   0        0        0    12482 2023-04-26 06:41:08.610306 nua_orchestrator-0.5.14/src/nua/orchestrator/app_instance.py
--rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.14/src/nua/orchestrator/app_management.py
--rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/__init__.py
--rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/db_utils.py
--rw-r--r--   0        0        0     3205 2023-04-04 11:21:10.875934 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/engine.py
--rw-r--r--   0        0        0     6378 2023-04-16 15:02:45.960265 nua_orchestrator-0.5.14/src/nua/orchestrator/assign/evaluators.py
--rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/__init__.py
--rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_engine.py
--rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_functions.py
--rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_report.py
--rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.14/src/nua/orchestrator/bootstrap/__init__.py
--rw-r--r--   0        0        0     7132 2023-04-24 21:25:56.873313 nua_orchestrator-0.5.14/src/nua/orchestrator/bootstrap/bootstrap.py
--rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/__init__.py
--rw-r--r--   0        0        0     2546 2023-04-21 16:49:16.834079 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/certbot.py
--rw-r--r--   0        0        0     4666 2023-04-24 21:25:56.873579 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/commands.py
--rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/__init__.py
--rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/cli.ini
--rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
--rw-r--r--   0        0        0     2507 2023-04-24 21:25:56.873772 nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/installer.py
--rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/__init__.py
--rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/api.py
--rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/backup.py
--rw-r--r--   0        0        0     1898 2023-04-26 06:41:08.610568 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/deploy_remove.py
--rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/restore.py
--rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/start_stop.py
--rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/status.py
--rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/configuration.py
--rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/debug.py
--rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/init.py
--rw-r--r--   0        0        0     6483 2023-04-16 08:46:30.714460 nua_orchestrator-0.5.14/src/nua/orchestrator/cli/main.py
--rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.14/src/nua/orchestrator/config.py
--rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.14/src/nua/orchestrator/constants.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.14/src/nua/orchestrator/db/__init__.py
--rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.14/src/nua/orchestrator/db/create.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/__init__.py
--rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/auth.py
--rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/base.py
--rw-r--r--   0        0        0     2073 2023-04-18 09:50:17.612727 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/deployconfig.py
--rw-r--r--   0        0        0      856 2023-04-18 09:50:17.612881 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/host.py
--rw-r--r--   0        0        0     1033 2023-04-18 09:50:17.613199 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/image.py
--rw-r--r--   0        0        0     4253 2023-04-26 06:41:08.610731 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/instance.py
--rw-r--r--   0        0        0     1602 2023-04-18 09:50:17.613874 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/setting.py
--rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/user_count.py
--rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.14/src/nua/orchestrator/db/session.py
--rw-r--r--   0        0        0    16464 2023-04-26 06:41:08.610982 nua_orchestrator-0.5.14/src/nua/orchestrator/db/store.py
--rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/__init__.py
--rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/migrations.py
--rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/tools.py
--rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/__init__.py
--rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.json
--rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.py
--rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mongo.json
--rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mongo.py
--rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.json
--rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.py
--rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/redis-cache.json
--rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/redis-cache.py
--rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/__init__.py
--rw-r--r--   0        0        0     7074 2023-04-24 21:25:56.874060 nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/mariadb_utils.py
--rw-r--r--   0        0        0     8130 2023-04-24 21:25:56.874228 nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/postgres_utils.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.14/src/nua/orchestrator/default_conf/__init__.py
--rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.14/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
--rw-r--r--   0        0        0    12004 2023-04-26 06:41:08.611177 nua_orchestrator-0.5.14/src/nua/orchestrator/deploy_utils.py
--rw-r--r--   0        0        0    18027 2023-04-24 21:25:56.874767 nua_orchestrator-0.5.14/src/nua/orchestrator/docker_utils.py
--rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.14/src/nua/orchestrator/domain_split.py
--rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.14/src/nua/orchestrator/healthcheck.py
--rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.14/src/nua/orchestrator/higher_package.py
--rw-r--r--   0        0        0     1417 2023-04-08 16:30:35.183610 nua_orchestrator-0.5.14/src/nua/orchestrator/internal_secrets.py
--rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.14/src/nua/orchestrator/net_utils/__init__.py
--rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.14/src/nua/orchestrator/net_utils/external_ip.py
--rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.14/src/nua/orchestrator/net_utils/ports.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/__init__.py
--rw-r--r--   0        0        0     1622 2023-04-24 21:25:56.874974 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/cmd.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/__init__.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/css/__init__.py
--rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/css/style.css
--rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/index.html
--rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/installer.py
--rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/__init__.py
--rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/default_site
--rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_located.j2
--rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_not_located.j2
--rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_located.j2
--rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located.j2
--rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
--rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/nginx.conf
--rw-r--r--   0        0        0     4895 2023-04-24 21:25:56.875166 nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/utils.py
--rw-r--r--   0        0        0     4621 2023-04-26 06:41:08.611435 nua_orchestrator-0.5.14/src/nua/orchestrator/nua_db_setup.py
--rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.14/src/nua/orchestrator/nua_env.py
--rw-r--r--   0        0        0     1078 2023-04-05 05:50:21.473685 nua_orchestrator-0.5.14/src/nua/orchestrator/persistent.py
--rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.14/src/nua/orchestrator/port_normalization.py
--rw-r--r--   0        0        0     3351 2023-04-24 21:25:56.875342 nua_orchestrator-0.5.14/src/nua/orchestrator/register_plugins.py
--rw-r--r--   0        0        0     2848 2023-01-08 20:45:01.446656 nua_orchestrator-0.5.14/src/nua/orchestrator/registry.py
--rw-r--r--   0        0        0    15807 2023-04-24 21:25:56.875604 nua_orchestrator-0.5.14/src/nua/orchestrator/resource.py
--rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.14/src/nua/orchestrator/resource_deps.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/__init__.py
--rw-r--r--   0        0        0      307 2023-02-06 17:21:30.505291 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/deactivate_all_instances.py
--rw-r--r--   0        0        0      263 2023-01-19 17:57:22.674122 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/docker_list_all.py
--rw-r--r--   0        0        0     1211 2023-04-17 20:53:06.739901 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/docker_remove_all.py
--rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/list_instances.py
--rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/mariadb_restore.py
--rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_instances.py
--rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_mounted_volumes.py
--rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_used_ports.py
--rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/set_pg_pwd.py
--rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.14/src/nua/orchestrator/search_cmd.py
--rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.14/src/nua/orchestrator/services/__init__.py
--rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.14/src/nua/orchestrator/services/mariadb.py
--rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.14/src/nua/orchestrator/services/postgres.py
--rw-r--r--   0        0        0     1127 2023-01-30 14:35:45.686645 nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_base.py
--rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_loader.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.14/src/nua/orchestrator/util/__init__.py
--rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.14/src/nua/orchestrator/util/deep_access_dict.py
--rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.14/src/nua/orchestrator/util/deep_update.py
--rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.14/src/nua/orchestrator/utils.py
--rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.14/src/nua/orchestrator/version.py
--rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.14/src/nua/orchestrator/volume.py
--rw-r--r--   0        0        0     4798 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.14/PKG-INFO
+-rw-r--r--   0        0        0     3876 2023-04-29 09:12:48.090789 nua_orchestrator-0.5.15/README.md
+-rw-r--r--   0        0        0     2630 2023-04-29 09:31:13.013118 nua_orchestrator-0.5.15/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-02-01 13:54:28.100764 nua_orchestrator-0.5.15/src/nua/orchestrator/__init__.py
+-rw-r--r--   0        0        0      118 2023-04-06 11:36:39.585136 nua_orchestrator-0.5.15/src/nua/orchestrator/__main__.py
+-rw-r--r--   0        0        0     2132 2023-04-08 16:30:35.041481 nua_orchestrator-0.5.15/src/nua/orchestrator/admin_local.py
+-rw-r--r--   0        0        0    51749 2023-04-29 09:12:48.108878 nua_orchestrator-0.5.15/src/nua/orchestrator/app_deployment.py
+-rw-r--r--   0        0        0    13298 2023-04-29 09:12:48.109438 nua_orchestrator-0.5.15/src/nua/orchestrator/app_instance.py
+-rw-r--r--   0        0        0     1639 2023-02-06 17:21:30.501023 nua_orchestrator-0.5.15/src/nua/orchestrator/app_management.py
+-rw-r--r--   0        0        0        0 2023-01-25 13:12:45.648052 nua_orchestrator-0.5.15/src/nua/orchestrator/assign/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-16 08:40:02.375778 nua_orchestrator-0.5.15/src/nua/orchestrator/assign/db_utils.py
+-rw-r--r--   0        0        0     3208 2023-04-29 09:12:48.109707 nua_orchestrator-0.5.15/src/nua/orchestrator/assign/engine.py
+-rw-r--r--   0        0        0     6382 2023-04-29 09:12:48.109928 nua_orchestrator-0.5.15/src/nua/orchestrator/assign/evaluators.py
+-rw-r--r--   0        0        0        0 2023-01-07 10:14:00.389172 nua_orchestrator-0.5.15/src/nua/orchestrator/backup/__init__.py
+-rw-r--r--   0        0        0     1618 2023-01-25 16:15:09.490835 nua_orchestrator-0.5.15/src/nua/orchestrator/backup/backup_engine.py
+-rw-r--r--   0        0        0      719 2023-04-08 16:18:44.073578 nua_orchestrator-0.5.15/src/nua/orchestrator/backup/backup_functions.py
+-rw-r--r--   0        0        0      973 2023-04-08 16:18:44.073632 nua_orchestrator-0.5.15/src/nua/orchestrator/backup/backup_report.py
+-rw-r--r--   0        0        0        0 2023-01-16 08:42:52.912983 nua_orchestrator-0.5.15/src/nua/orchestrator/bootstrap/__init__.py
+-rw-r--r--   0        0        0     7132 2023-04-26 08:44:27.773025 nua_orchestrator-0.5.15/src/nua/orchestrator/bootstrap/bootstrap.py
+-rw-r--r--   0        0        0      118 2023-01-08 08:57:33.879748 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/__init__.py
+-rw-r--r--   0        0        0     2566 2023-04-29 09:12:48.110171 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/certbot.py
+-rw-r--r--   0        0        0     4250 2023-04-29 09:12:48.110411 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/commands.py
+-rw-r--r--   0        0        0        0 2023-03-11 08:22:42.855026 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/config/__init__.py
+-rw-r--r--   0        0        0      403 2023-03-15 21:17:19.131952 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/config/cli.ini
+-rw-r--r--   0        0        0      774 2023-03-15 21:17:19.132102 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf
+-rw-r--r--   0        0        0     2507 2023-04-26 08:44:27.773490 nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/installer.py
+-rw-r--r--   0        0        0        0 2023-01-08 21:09:12.167216 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-03 19:23:00.344340 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2635 2023-04-10 14:02:02.204067 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/api.py
+-rw-r--r--   0        0        0      286 2023-02-16 11:05:25.839048 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/backup.py
+-rw-r--r--   0        0        0     2034 2023-04-29 09:12:48.110610 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/deploy_remove.py
+-rw-r--r--   0        0        0     1387 2023-04-04 11:21:10.877158 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/restore.py
+-rw-r--r--   0        0        0     1442 2023-04-11 14:23:48.026102 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/start_stop.py
+-rw-r--r--   0        0        0     1416 2023-04-16 08:46:30.714375 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/status.py
+-rw-r--r--   0        0        0     1404 2023-04-16 08:40:22.069040 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/configuration.py
+-rw-r--r--   0        0        0     1308 2023-04-06 11:36:39.585561 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/debug.py
+-rw-r--r--   0        0        0      798 2023-04-08 16:18:44.073946 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/init.py
+-rw-r--r--   0        0        0     6672 2023-04-29 09:12:48.110776 nua_orchestrator-0.5.15/src/nua/orchestrator/cli/main.py
+-rw-r--r--   0        0        0      267 2022-11-17 17:42:00.921923 nua_orchestrator-0.5.15/src/nua/orchestrator/config.py
+-rw-r--r--   0        0        0      248 2022-11-17 17:42:00.922443 nua_orchestrator-0.5.15/src/nua/orchestrator/constants.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922490 nua_orchestrator-0.5.15/src/nua/orchestrator/db/__init__.py
+-rw-r--r--   0        0        0      301 2023-01-06 12:47:38.582693 nua_orchestrator-0.5.15/src/nua/orchestrator/db/create.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.922589 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/__init__.py
+-rw-r--r--   0        0        0     1707 2022-11-17 17:42:00.922655 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/auth.py
+-rw-r--r--   0        0        0       96 2022-11-17 17:42:00.922706 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/base.py
+-rw-r--r--   0        0        0     2073 2023-04-26 08:53:06.277388 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/deployconfig.py
+-rw-r--r--   0        0        0      856 2023-04-26 08:53:06.277587 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/host.py
+-rw-r--r--   0        0        0     1033 2023-04-26 08:53:06.277787 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/image.py
+-rw-r--r--   0        0        0     4253 2023-04-26 08:53:06.278246 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/instance.py
+-rw-r--r--   0        0        0     1602 2023-04-26 08:53:06.278463 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/setting.py
+-rw-r--r--   0        0        0      392 2023-01-25 13:12:45.649061 nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/user_count.py
+-rw-r--r--   0        0        0      504 2023-01-06 12:47:38.583466 nua_orchestrator-0.5.15/src/nua/orchestrator/db/session.py
+-rw-r--r--   0        0        0    16885 2023-04-29 09:12:48.111070 nua_orchestrator-0.5.15/src/nua/orchestrator/db/store.py
+-rw-r--r--   0        0        0        0 2023-04-06 15:46:47.654975 nua_orchestrator-0.5.15/src/nua/orchestrator/db_migration/__init__.py
+-rw-r--r--   0        0        0      211 2023-04-08 16:30:07.204201 nua_orchestrator-0.5.15/src/nua/orchestrator/db_migration/migrations.py
+-rw-r--r--   0        0        0      724 2023-04-06 15:46:47.655336 nua_orchestrator-0.5.15/src/nua/orchestrator/db_migration/tools.py
+-rw-r--r--   0        0        0        0 2023-01-31 10:30:37.322898 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/__init__.py
+-rw-r--r--   0        0        0     1044 2023-02-02 12:51:27.404427 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mariadb.json
+-rw-r--r--   0        0        0     2250 2023-04-17 07:02:55.385046 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mariadb.py
+-rw-r--r--   0        0        0      160 2023-02-28 08:14:12.801866 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mongo.json
+-rw-r--r--   0        0        0     1438 2023-04-17 07:02:55.385309 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mongo.py
+-rw-r--r--   0        0        0      674 2023-02-02 12:51:27.404513 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/postgres.json
+-rw-r--r--   0        0        0     1734 2023-04-17 07:02:55.385618 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/postgres.py
+-rw-r--r--   0        0        0      414 2023-02-03 15:39:09.009427 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/redis-cache.json
+-rw-r--r--   0        0        0     1146 2023-04-17 07:02:55.385868 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/redis-cache.py
+-rw-r--r--   0        0        0     1399 2023-04-17 07:02:55.386092 nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:24:06.976924 nua_orchestrator-0.5.15/src/nua/orchestrator/db_utils/__init__.py
+-rw-r--r--   0        0        0     7072 2023-04-29 09:12:48.111345 nua_orchestrator-0.5.15/src/nua/orchestrator/db_utils/mariadb_utils.py
+-rw-r--r--   0        0        0     8128 2023-04-29 09:12:48.111558 nua_orchestrator-0.5.15/src/nua/orchestrator/db_utils/postgres_utils.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.403836 nua_orchestrator-0.5.15/src/nua/orchestrator/default_conf/__init__.py
+-rw-r--r--   0        0        0     1689 2023-01-25 16:15:09.491276 nua_orchestrator-0.5.15/src/nua/orchestrator/default_conf/nua_defaults_settings.toml
+-rw-r--r--   0        0        0    11985 2023-04-29 09:12:48.111822 nua_orchestrator-0.5.15/src/nua/orchestrator/deploy_utils.py
+-rw-r--r--   0        0        0    18157 2023-04-29 09:12:48.112112 nua_orchestrator-0.5.15/src/nua/orchestrator/docker_utils.py
+-rw-r--r--   0        0        0     1111 2023-04-08 16:18:44.074215 nua_orchestrator-0.5.15/src/nua/orchestrator/domain_split.py
+-rw-r--r--   0        0        0     2596 2023-01-07 09:59:37.811449 nua_orchestrator-0.5.15/src/nua/orchestrator/healthcheck.py
+-rw-r--r--   0        0        0     1444 2023-04-08 16:30:35.180413 nua_orchestrator-0.5.15/src/nua/orchestrator/higher_package.py
+-rw-r--r--   0        0        0     1413 2023-04-29 09:12:48.112276 nua_orchestrator-0.5.15/src/nua/orchestrator/internal_secrets.py
+-rw-r--r--   0        0        0        0 2023-01-11 17:21:08.504814 nua_orchestrator-0.5.15/src/nua/orchestrator/net_utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-04-08 16:30:07.252175 nua_orchestrator-0.5.15/src/nua/orchestrator/net_utils/external_ip.py
+-rw-r--r--   0        0        0      407 2023-01-11 17:21:08.504884 nua_orchestrator-0.5.15/src/nua/orchestrator/net_utils/ports.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132385 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/__init__.py
+-rw-r--r--   0        0        0     1622 2023-04-29 09:12:48.112428 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/cmd.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.132886 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/html/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133023 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/html/css/__init__.py
+-rw-r--r--   0        0        0     1410 2023-03-15 21:17:19.133148 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/html/css/style.css
+-rw-r--r--   0        0        0      528 2023-03-15 21:17:19.133492 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/html/index.html
+-rw-r--r--   0        0        0     2248 2023-04-15 14:11:09.451331 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/installer.py
+-rw-r--r--   0        0        0        0 2023-03-15 21:17:19.133754 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/__init__.py
+-rw-r--r--   0        0        0      585 2023-03-15 21:17:19.134024 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/default_site
+-rw-r--r--   0        0        0     1790 2023-03-15 21:17:19.134140 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/http_located.j2
+-rw-r--r--   0        0        0     1427 2023-04-04 11:21:10.877419 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/http_not_located.j2
+-rw-r--r--   0        0        0     2332 2023-03-15 21:17:19.134351 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/https_located.j2
+-rw-r--r--   0        0        0     3553 2023-04-04 11:21:10.878037 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/https_not_located.j2
+-rw-r--r--   0        0        0     2201 2023-04-04 11:21:10.878343 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2
+-rw-r--r--   0        0        0     1115 2023-03-15 21:17:19.134715 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/nginx.conf
+-rw-r--r--   0        0        0     4895 2023-04-29 09:12:48.112586 nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/utils.py
+-rw-r--r--   0        0        0     4621 2023-04-26 08:44:27.776287 nua_orchestrator-0.5.15/src/nua/orchestrator/nua_db_setup.py
+-rw-r--r--   0        0        0     1430 2023-04-08 16:30:35.213876 nua_orchestrator-0.5.15/src/nua/orchestrator/nua_env.py
+-rw-r--r--   0        0        0     1362 2023-04-29 09:12:48.112730 nua_orchestrator-0.5.15/src/nua/orchestrator/persistent.py
+-rw-r--r--   0        0        0     3860 2023-04-04 11:21:10.878990 nua_orchestrator-0.5.15/src/nua/orchestrator/port_normalization.py
+-rw-r--r--   0        0        0     3349 2023-04-29 09:12:48.112968 nua_orchestrator-0.5.15/src/nua/orchestrator/register_plugins.py
+-rw-r--r--   0        0        0     2830 2023-04-29 09:12:48.113193 nua_orchestrator-0.5.15/src/nua/orchestrator/registry.py
+-rw-r--r--   0        0        0    15805 2023-04-29 09:12:48.113413 nua_orchestrator-0.5.15/src/nua/orchestrator/resource.py
+-rw-r--r--   0        0        0     1737 2023-04-08 16:18:44.074313 nua_orchestrator-0.5.15/src/nua/orchestrator/resource_deps.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.924261 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-29 09:12:48.113562 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/deactivate_all_instances.py
+-rw-r--r--   0        0        0      263 2023-04-29 09:12:48.113700 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/docker_list_all.py
+-rw-r--r--   0        0        0     1211 2023-04-29 09:12:48.113837 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/docker_remove_all.py
+-rw-r--r--   0        0        0      337 2023-04-06 15:46:47.655692 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/list_instances.py
+-rw-r--r--   0        0        0      735 2023-04-17 08:29:13.917800 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/mariadb_restore.py
+-rw-r--r--   0        0        0      614 2023-04-06 15:46:47.655840 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/print_instances.py
+-rw-r--r--   0        0        0      319 2023-01-25 13:12:45.650893 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/print_mounted_volumes.py
+-rw-r--r--   0        0        0      307 2023-01-25 13:12:45.650983 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/print_used_ports.py
+-rw-r--r--   0        0        0      782 2023-04-17 08:29:27.370236 nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/set_pg_pwd.py
+-rw-r--r--   0        0        0     3738 2023-02-08 17:48:17.607646 nua_orchestrator-0.5.15/src/nua/orchestrator/search_cmd.py
+-rw-r--r--   0        0        0       59 2023-01-08 11:06:40.699794 nua_orchestrator-0.5.15/src/nua/orchestrator/services/__init__.py
+-rw-r--r--   0        0        0      451 2023-04-16 21:08:39.554885 nua_orchestrator-0.5.15/src/nua/orchestrator/services/mariadb.py
+-rw-r--r--   0        0        0      658 2023-04-16 21:08:39.554936 nua_orchestrator-0.5.15/src/nua/orchestrator/services/postgres.py
+-rw-r--r--   0        0        0     1109 2023-04-29 09:12:48.114065 nua_orchestrator-0.5.15/src/nua/orchestrator/services/service_base.py
+-rw-r--r--   0        0        0     1911 2023-02-08 11:40:48.305440 nua_orchestrator-0.5.15/src/nua/orchestrator/services/service_loader.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.925777 nua_orchestrator-0.5.15/src/nua/orchestrator/util/__init__.py
+-rw-r--r--   0        0        0     1521 2023-04-08 16:18:44.074369 nua_orchestrator-0.5.15/src/nua/orchestrator/util/deep_access_dict.py
+-rw-r--r--   0        0        0      397 2023-04-17 08:27:43.783766 nua_orchestrator-0.5.15/src/nua/orchestrator/util/deep_update.py
+-rw-r--r--   0        0        0     3782 2023-04-08 16:30:35.277111 nua_orchestrator-0.5.15/src/nua/orchestrator/utils.py
+-rw-r--r--   0        0        0       88 2022-11-17 17:42:00.925948 nua_orchestrator-0.5.15/src/nua/orchestrator/version.py
+-rw-r--r--   0        0        0     6470 2023-04-08 16:18:44.074470 nua_orchestrator-0.5.15/src/nua/orchestrator/volume.py
+-rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 nua_orchestrator-0.5.15/PKG-INFO
```

### Comparing `nua_orchestrator-0.5.14/README.md` & `nua_orchestrator-0.5.15/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -116,7 +116,13 @@
 [...]
 
 Nua installation done for user 'nua' on this host.
 Command 'nua --help':
 ```
 
 At the end of the installation, the available commands are displayed.
+
+## Development
+
+### Dependency graph
+
+![Dependency graph](./doc/dependency-graph.png)
```

### Comparing `nua_orchestrator-0.5.14/pyproject.toml` & `nua_orchestrator-0.5.15/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nua-orchestrator"
-version = "0.5.14"
+version = "0.5.15"
 description = "Nua orchestrator - local implementation"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
@@ -28,18 +28,15 @@
 nua-deactivate-all = "nua.orchestrator.scripts.deactivate_all_instances:main"
 nua-docker-list-all = "nua.orchestrator.scripts.docker_list_all:main"
 nua-docker-rm-all = "nua.orchestrator.scripts.docker_remove_all:main"
 nua_test_services = "nua.orchestrator.service:test"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.14"
-nua-agent = "=0.5.14"
-nua-build = "=0.5.14"
-nua-autobuild = "=0.5.14"
+nua-lib = "=0.5.15"
 SQLAlchemy-serializer = "^1.4.1"
 SQLAlchemy = "^1.4.36"
 psycopg2-binary = "^2.9.3"
 setuptools = "*"
 wheel = "*"
 tomli = "^2"
 paramiko = "^2.11.0"
@@ -77,15 +74,14 @@
 [tool.deptry]
 exclude = [
     '.nox', 'noxfile.py', 'tests',
 ]
 ignore_obsolete = [
     "nua-lib",
     "nua-agent",
-    "nua-autobuild",
     "nua-build",
     "setuptools",
     "wheel",
     "psycopg2-binary",
 ]
 ignore_missing = [
     "nua",
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/admin_local.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/admin_local.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/app_deployment.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/app_deployment.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     Abort,
     bold_debug,
     debug,
     important,
     info,
     red_line,
     show,
+    vprint,
     warning,
 )
 from nua.lib.tool.state import verbosity
 
 from . import config
 from .app_instance import AppInstance
 from .assign.engine import instance_key_evaluator
@@ -147,57 +148,57 @@
             "apps": deepcopy(self.apps),
         }
         self.future_config_id = store.deploy_config_add_config(
             deploy_config, self.previous_config_id, ACTIVE
         )
 
     def remove_app_instance(self, removed_app: AppInstance):
-        domain = removed_app.hostname
-        apps = [app for app in self.apps if app != removed_app]
+        label_id = removed_app.label_id
+        apps = [app for app in self.apps if app.label_id != label_id]
         self.apps = apps
         self.sort_apps_per_name_domain()
-        self.remove_domain_from_config(domain)
+        self.remove_domain_from_config(removed_app.domain)
 
     def remove_domain_from_config(self, domain: str):
-        sites = self.loaded_config.get("site", [])
-        new_sites = [item for item in sites if item.get("domain", "") != domain]
-        self.loaded_config["site"] = new_sites
+        apps = self.loaded_config.get("site", [])
+        filtered = [app for app in apps if app.get("domain", "") != domain]
+        self.loaded_config["site"] = filtered
 
     def local_services_inventory(self):
         """Initialization step: inventory of available resources available on
         the host, like local databases."""
         # See later
         return
         # assuming nua_db_setup was run at initialization of the command
         services = Services()
         services.load()
         self.available_services = services.loaded
-        with verbosity(2):
+        with verbosity(1):
             bold_debug(
                 f"Available local services: {pformat(list(services.loaded.keys()))}"
             )
 
     def load_deploy_config(self, deploy_config: str):
         config_path = Path(deploy_config).expanduser().resolve()
-        with verbosity(1):
+        with verbosity(0):
             info(f"Deploy apps from: {config_path}")
         self.loaded_config = parse_any_format(config_path)
         self.parse_deploy_apps()
         self.sort_apps_per_name_domain()
         self.deployed_domains = sorted(
             {apps["hostname"] for apps in self.apps_per_domain}
         )
         self.deployed_labels = sorted(app.label_id for app in self.apps)
         with verbosity(3):
             self.print_host_list()
 
     def load_deployed_configuration(self):
         previous_config = self.previous_success_deployment_record()
         if not previous_config:
-            with verbosity(2):
+            with verbosity(1):
                 show("First deployment (no previous deployed configuration found)")
             self.loaded_config = {}
             self.apps = []
             self.deployed_domains = []
             return
         self.loaded_config = previous_config["deployed"]["requested"]
         self.apps = [
@@ -278,38 +279,41 @@
                     # same app on another domain
                     return "deploy_move_domain"
                 else:
                     # another app on another domain
                     return "deploy_reuse_label"
 
     def deploy_new_app(self, app: AppInstance):
-        """Deploy new label and app on new domain"""
+        """Deploy new label and app on new domain."""
         important(f"Deploy '{app.label}': a new {app.app_id} on '{app.domain}'")
-        self._deploy_new_app(app, load_persistent=False)
+        self._deploy_new_app(app)
 
     def _deploy_new_app(
         self,
         app: AppInstance,
-        load_persistent: bool = False,
+        persistent: dict | None = None,
     ):
         """Deploy an app."""
         # step 1:
         app.set_network_name()
         app.set_resources_names()
         app.merge_instance_to_resources()
         for resource in app.resources:
             resource.configure_db()
         app.set_volumes_names()
         for service in app.local_services:
             if service not in self.available_services:
                 raise Abort(f"Required service '{service}' is not available")
-        if load_persistent:
+        if persistent:
+            with verbosity(2):
+                debug(pformat(persistent))
             # if really new app, not persistent for now, but some persitent data if
-            # same reusing label
-            self.retrieve_persistent(app)
+            # reusing same label_id for a new app: then try to retrieve the persistent
+            # data of previous Appinstance:
+            app.set_persistent_full_dict(persistent)
         self.evaluate_dynamic_values(app)
 
         # step 2: ports
         start_ports = config.read("nua", "ports", "start") or 8100
         end_ports = config.read("nua", "ports", "end") or 9000
         allocated_ports = self.configured_ports()
         ports_instances_domains = store.ports_instances_domains()
@@ -329,88 +333,90 @@
                     f"app {app.domain}"
                 )
         self.store_initial_deployment_state()
         self.already_deployed_domains = set(self.deployed_domains)
         self.already_deployed_labels = set(self.deployed_labels)
         self.apps.append(app)
         self.sort_apps_per_name_domain()
+        self.merge_nginx_configuration()
         self.deployed_domains = sorted(
             {apps_dom["hostname"] for apps_dom in self.apps_per_domain}
         )
         self.deployed_labels = sorted(a.label_id for a in self.apps)
-        self.merge_nginx_configuration()
-        self.merge_start_apps([app])
+        self._start_apps([app], deactivate=False)
 
-    def deploy_update_app(self, app: AppInstance):
+    def deploy_update_app(self, merged_app: AppInstance):
         """Deploy same app on on same domain."""
-        important(f"Deploy '{app.label}': update {app.app_id} on '{app.domain}'")
-        self._deploy_remove_label_domain(app, remove_volumes=False)
-        self.load_deployed_configuration()
-        self._deploy_new_app(app, load_persistent=True)
+        important(
+            f"Deploy '{merged_app.label}': update {merged_app.app_id} "
+            f"on '{merged_app.domain}'"
+        )
+        same_label_app = next(
+            (app for app in self.apps if app.label_id == merged_app.label_id), None
+        )
+        persistent_data = same_label_app.persistent_full_dict()
+        self._remove_per_label(same_label_app, remove_volumes=False)
+        self._deploy_new_app(merged_app, persistent=persistent_data)
 
     def deploy_replace_app(self, merged_app: AppInstance):
         """Deploy another app on same domain."""
         same_label_app = next(
             (app for app in self.apps if app.label_id == merged_app.label_id), None
         )
         important(
             f"Deploy '{merged_app.label}': replace {same_label_app.app_id} "
             f"by {merged_app.app_id} on '{merged_app.domain}'"
         )
-        self._deploy_remove_label_domain(merged_app, remove_volumes=True)
-        self.load_deployed_configuration()
-        self._deploy_new_app(merged_app, load_persistent=False)
+        self._remove_per_label(merged_app, remove_volumes=True)
+        self._deploy_new_app(merged_app)
 
     def deploy_move_domain(self, merged_app: AppInstance):
         """Deploy same app on another domain."""
-        same_domain_app = next(
-            (app for app in self.apps if app.domain == merged_app.domain), None
+        same_label_app = next(
+            (app for app in self.apps if app.label_id == merged_app.label_id), None
         )
         important(
             f"Deploy '{merged_app.label}': move {merged_app.app_id} "
-            f"from '{same_domain_app.domain}' to '{merged_app.domain}'"
+            f"from '{same_label_app.domain}' to '{merged_app.domain}'"
         )
-        self._deploy_remove_label_domain(same_domain_app, remove_volumes=False)
-        self.load_deployed_configuration()
-        self._deploy_new_app(merged_app, load_persistent=True)
+        persistent_data = same_label_app.persistent_full_dict()
+        self._remove_per_label(same_label_app, remove_volumes=False)
+        self._deploy_new_app(merged_app, persistent=persistent_data)
 
     def deploy_reuse_label(self, merged_app: AppInstance):
         """Deploy another app on another domain."""
         same_label_app = next(
             (app for app in self.apps if app.label_id == merged_app.label_id), None
         )
         important(
-            f"Deploy '{merged_app.label}': remove {same_label_app.app_id} and"
+            f"Deploy '{merged_app.label}': remove {same_label_app.app_id} "
             f"from '{same_label_app.domain}' and\n"
             f"install {merged_app.app_id} to '{merged_app.domain}'"
         )
         # do not keep data:
-        self._deploy_remove_label_domain(same_label_app, remove_volumes=True)
-        self.load_deployed_configuration()
-        self._deploy_new_app(merged_app, load_persistent=True)
+        self._remove_per_label(same_label_app, remove_volumes=True)
+        self._deploy_new_app(merged_app)
 
-    def _deploy_remove_label_domain(
+    def _remove_per_label(
         self,
-        merged_app: AppInstance,
+        current_app: AppInstance,
         remove_volumes: bool = False,
     ):
-        # deployed_app = next(
-        #     (a for a in self.apps if a.label_id == merged_app.label_id), None
-        # )
-        domain = merged_app.domain
-        stopping_apps = self.instances_of_domain(domain)
-        self.remove_nginx_configuration(domain)
-        self.stop_deployed_apps(domain, stopping_apps)
-        self.remove_container_and_network(domain, stopping_apps)
+        self.remove_nginx_configuration(current_app.domain)
+        self.deployed_domains = [
+            d for d in self.deployed_domains if d != current_app.domain
+        ]
+        self.stop_deployed_apps([current_app])
+        self.remove_container_and_network([current_app])
         if remove_volumes:
-            self.remove_managed_volumes(stopping_apps)
-        if verbosity(3):
+            self.remove_managed_volumes([current_app])
+        with verbosity(3):
             debug("remove_deployed_instance:")
-            debug(" ".join([a.domain for a in stopping_apps]))
-        self.remove_deployed_instance(domain, stopping_apps)
+            debug(current_app.label_id)
+        self.remove_deployed_instance([current_app])
 
     def merge_add(self, additional: AppDeployment):
         """Merge by simple addtion of new domain to list."""
         with verbosity(3):
             debug(f"self.deployed_domains       {self.deployed_domains}")
             debug(f"additional.deployed_domains {additional.deployed_domains}")
         conflict = known_strings(self.deployed_domains, additional.deployed_domains)
@@ -433,33 +439,42 @@
         self.apps.extend(additional.apps)
         self.sort_apps_per_name_domain()
         self.deployed_domains = sorted(
             {apps_dom["hostname"] for apps_dom in self.apps_per_domain}
         )
         self.deployed_labels = sorted(app.label_id for app in self.apps)
         self.merge_nginx_configuration()
-        self.merge_start_apps(additional.apps)
+        self._start_apps(additional.apps, deactivate=True)
 
     def instances_of_domain(self, domain: str) -> list[AppInstance]:
         """Select deployed instances of domain."""
         self.load_deployed_configuration()
         for apps_dom in self.apps_per_domain:
             if apps_dom["hostname"] == domain:
                 return apps_dom["apps"]
         raise Abort(f"No instance found for domain '{domain}'")
 
+    def instance_of_label(self, label: str) -> AppInstance:
+        """Select deployed instances per label."""
+        label_id = AppInstance.docker_sanitized_name(label)
+        self.load_deployed_configuration()
+        for app in self.apps:
+            if app.label_id == label_id:
+                return app
+        raise Abort(f"No instance found for label_id '{label_id}'")
+
     def restore_previous_deploy_config_strict(self):
         """Retrieve last successful deployment configuration (strict mode)."""
-        with verbosity(1):
+        with verbosity(0):
             show("Deploy apps from previous deployment (strict mode).")
         self.load_deployed_configuration()
 
     def restore_previous_deploy_config_replay(self):
         """Retrieve last successful deployment configuration (replay mode)."""
-        with verbosity(1):
+        with verbosity(0):
             show("Deploy apps from previous deployment (replay deployment).")
         self.load_deployed_configuration()
         with verbosity(3):
             self.print_host_list()
 
     def gather_requirements(self):
         self.install_required_images()
@@ -527,19 +542,18 @@
         """Apply configuration to Nginx, when apps are already deployed."""
         if not self.already_deployed_domains:
             # easy, either first deployment or all apps removed, start from zero:
             return self.apply_nginx_configuration()
         for host in self.apps_per_domain:
             hostname = host["hostname"]
             with verbosity(3):
-                print(f"merge_nginx_configuration for {hostname}")
-
+                debug(f"merge_nginx_configuration for {hostname}")
             if hostname in self.already_deployed_domains:
                 with verbosity(3):
-                    print("continue, already_deployed_domains")
+                    debug("continue, already_deployed_domains")
                 continue
             with verbosity(1):
                 info(f"Configure Nginx for domain '{hostname}'")
             configure_nginx_hostname(host)
         # registering https apps with certbot requires that the base nginx config is
         # deployed.
         register_certbot_domains(self.apps)
@@ -548,41 +562,43 @@
             debug(self.apps)
 
     def remove_nginx_configuration(self, stop_domain: str):
         """Remove apps from the nginx configuration.
 
         To stop nginx redirection before actually stopping the apps.
         """
-        with verbosity(1):
-            info(f"Remove domain from Nginx: '{stop_domain}'")
+        with verbosity(0):
+            info(f"Remove Nginx configuration: '{stop_domain}'")
+
         remove_nginx_configuration_hostname(stop_domain)
         nginx_reload()
 
     def remove_all_deployed_nginx_configuration(self):
         """Remove all deployed apps from the nginx configuration.
 
         To stop nginx redirection before actually stopping the apps.
         """
         if not self.deployed_domains:
             return
-        with verbosity(1):
+        with verbosity(0):
             show("Removing Nginx configuration.")
         for domain in self.deployed_domains:
             remove_nginx_configuration_hostname(domain)
         nginx_reload()
 
-    def merge_start_apps(self, new_apps: list[AppInstance]):
+    def _start_apps(self, new_apps: list[AppInstance], deactivate: bool = False):
         """Start new deployed apps."""
         if not self.already_deployed_domains:
             # easy, either first deployment or all apps removed, start from zero:
             return self.start_apps()
         # restarting local services:
         self.restart_local_services()
         for app in new_apps:
-            deactivate_app(app)
+            if deactivate:
+                deactivate_app(app)
             self.start_network(app)
             self.evaluate_container_params(app)
             self.start_resources_containers(app)
             self.setup_resources_db(app)
             self.merge_volume_only_resources(app)
             self.start_main_app_container(app)
             app.running_status = RUNNING
@@ -605,67 +621,74 @@
             app.running_status = RUNNING
             self.store_container_instance(app)
         chown_r_nua_nginx()
         nginx_restart()
 
     def start_deployed_apps(self, domain: str, apps: list[AppInstance]):
         """Start deployed instances previously stopped."""
-        with verbosity(1):
+        with verbosity(0):
             info(f"Start instance of domain '{domain}'.")
         for site in apps:
             # self.start_network(site)
             start_one_app_containers(site)
             site.running_status = RUNNING
             self.store_container_instance(site)
 
-    def stop_deployed_apps(self, domain: str, apps: list[AppInstance]):
+    def remove_app_list(self, apps: list[AppInstance]):
+        self.stop_deployed_apps(apps)
+        self.remove_container_and_network(apps)
+        self.remove_managed_volumes(apps)
+        self.remove_deployed_instance(apps)
+
+    def stop_deployed_apps(self, apps: list[AppInstance]):
         """Stop deployed app instances."""
-        with verbosity(1):
-            info(f"Stop instance of domain '{domain}'.")
-        for site in apps:
-            stop_one_app_containers(site)
-            site.running_status = STOPPED
-            self.store_container_instance(site)
+        with verbosity(0):
+            for app in apps:
+                info(f"Stop app '{app.label_id}'")
+        for app in apps:
+            stop_one_app_containers(app)
+            app.running_status = STOPPED
+            self.store_container_instance(app)
 
     def stop_all_deployed_apps(self, store_status: bool = False):
         """Stop all deployed app instances."""
         if not self.apps:
             return
-        with verbosity(1):
+        with verbosity(0):
             show("Stop all instances.")
         for site in self.apps:
             stop_one_app_containers(site)
             if store_status:
                 site.running_status = STOPPED
                 self.store_container_instance(site)
 
     def restart_deployed_apps(self, domain: str, apps: list[AppInstance]):
         """Restart deployed instances."""
-        with verbosity(1):
+        with verbosity(0):
             info(f"Restart instance of domain '{domain}'.")
         for site in apps:
             # self.start_network(site)
             restart_one_app_containers(site)
             site.running_status = RUNNING
             self.store_container_instance(site)
 
-    def remove_container_and_network(self, domain: str, apps: list[AppInstance]):
+    def remove_container_and_network(self, apps: list[AppInstance]):
         """Remove stopped app: container, network, but not volumes."""
-        with verbosity(1):
-            info(f"Remove instance of domain '{domain}'.")
+        with verbosity(3):
+            debug(f"Remove instances '{apps}'")
         self._mounted_before_removing = store.list_instances_container_active_volumes()
-        for site in apps:
-            deactivate_app(site)
-            remove_container_private_network(site.network_name)
+        for app in apps:
+            deactivate_app(app)
+            remove_container_private_network(app.network_name)
 
     def remove_all_deployed_container_and_network(self):
         """Remove all (stopped) apps container, network, but not volumes."""
         if not self.apps:
             return
-        with verbosity(1):
+        with verbosity(0):
             show("Remove all instances.")
         self._mounted_before_removing = store.list_instances_container_active_volumes()
         for site in self.apps:
             deactivate_app(site)
             remove_container_private_network(site.network_name)
 
     @staticmethod
@@ -688,18 +711,18 @@
 
     def remove_all_deployed_managed_volumes(self):
         """Remove local volumes of all (stopped) apps."""
         before = self._local_volumes_dict(self._mounted_before_removing)
         for source in before:
             remove_volume_by_source(source)
 
-    def remove_deployed_instance(self, domain: str, apps: list[AppInstance]):
+    def remove_deployed_instance(self, apps: list[AppInstance]):
         """Remove data of stopped app: local managed volumes."""
-        with verbosity(1):
-            info(f"Remove app instance of domain '{domain}' from DB.")
+        with verbosity(3):
+            info(f"Remove instance '{apps}' from loaded configuration")
         for app in apps:
             self.remove_app_instance(app)
 
     def parse_deploy_apps(self):
         """Make the list of AppInstances to be deployed/merged.
 
         Check config syntax, replace missing information by defaults.
@@ -841,15 +864,15 @@
         self.install_images()
 
     def find_all_apps_images(self) -> bool:
         for app in self.apps:
             if not app.find_registry_path():
                 show(f"No image found for '{app.image}'")
                 return False
-        with verbosity(1):
+        with verbosity(0):
             seen = set()
             for app in self.apps:
                 if app.image not in seen:
                     seen.add(app.image)
                     info(f"Image found: '{app.image}'")
         return True
 
@@ -950,35 +973,35 @@
     def apps_set_volumes_names(self):
         for app in self.apps:
             app.set_volumes_names()
         with verbosity(3):
             debug("apps_set_volumes_names() done")
 
     def restart_local_services(self):
-        with verbosity(2):
+        with verbosity(1):
             if self.required_services:
                 show("Services to restart:", pformat(self.required_services))
             else:
                 info("Services to restart: None")
         for service in self.required_services:
             handler = self.available_services[service]
             handler.restart()
 
     def configure_nginx(self):
         clean_nua_nginx_default_site()
         for host in self.apps_per_domain:
-            with verbosity(1):
+            with verbosity(0):
                 info(f"Configure Nginx for domain '{host['hostname']}'")
             configure_nginx_hostname(host)
 
     def reconfigure_nginx_domain(self, domain: str):
         for host in self.apps_per_domain:
             if host["hostname"] != domain:
                 continue
-            with verbosity(1):
+            with verbosity(0):
                 info(f"Configure Nginx for domain '{host['hostname']}'")
             configure_nginx_hostname(host)
         nginx_reload()
 
     def apps_generate_ports(self):
         start_ports = config.read("nua", "ports", "start") or 8100
         end_ports = config.read("nua", "ports", "end") or 9000
@@ -1199,47 +1222,47 @@
     def display_deployment_status(self):
         self.display_deployed_apps()
         self.display_used_volumes()
         self.display_unused_volumes()
 
     def display_deployed_apps(self):
         if not self.apps:
-            show("No app deployed.")
+            important("No app deployed.")
             return
 
-        show("Deployed apps:")
+        important("Deployed apps:")
         protocol = protocol_prefix()
         for app in self.apps:
             msg = f"Label: {app.label_id}"
             info(msg)
             msg = f"Image '{app.image}' deployed as {protocol}{app.domain}"
             info(msg)
             msg = f"Deployment status: {app.running_status}"
             info(msg)
             self.display_persistent_data(app)
-        print()
+        vprint("")
 
     def display_persistent_data(self, app: AppInstance):
         with verbosity(3):
             content = app.persistent_full_dict()
             if content:
                 bold_debug("Persistent generated variables:")
                 debug(pformat(content))
 
     def display_used_volumes(self):
-        with verbosity(1):
+        with verbosity(0):
             current_mounted = store.list_instances_container_active_volumes()
             if not current_mounted:
                 return
             important("Volumes used by current Nua configuration:")
             for volume in current_mounted:
                 show(Volume.string(volume))
 
     def display_unused_volumes(self):
-        with verbosity(1):
+        with verbosity(0):
             unused = unused_volumes(self.orig_mounted_volumes)
             if not unused:
                 return
             important(
                 "Some volumes are mounted but not used by current Nua configuration:"
             )
             for volume in unused:
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/app_instance.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/app_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
+import string
 from copy import deepcopy
 from pathlib import Path
 from pprint import pformat
 
-from nua.agent.nua_config import hyphen_get
-from nua.agent.nua_tag import nua_tag_string
+from nua.lib.nua_config import hyphen_get
+from nua.lib.nua_tag import nua_tag_string
 from nua.lib.panic import Abort, debug, info, warning
 from nua.lib.tool.state import verbosity
 
 from .db.model.instance import STOPPED
 from .domain_split import DomainSplit
 from .persistent import Persistent
 from .port_normalization import (
@@ -302,16 +303,38 @@
         """Return a label based on app id and domain.
 
         To use when the user does not provide an app label or as default
         value.
         """
         return f"{self.image_short}-{self.domain}"
 
+    @staticmethod
+    def docker_sanitized_name(name: str) -> str:
+        """Docker valid name.
+
+        https://docs.docker.com/engine/reference/commandline/
+        tag/#extended-description
+        """
+        # first replace spaces per underscores
+        content = "_".join(name.split())
+        # then apply docjer rules
+        allowed = set(string.ascii_lowercase + string.digits + ".-_")
+        content = "".join([c for c in content.strip().lower() if c in allowed])
+        while ("___") in content:
+            content.replace("___", "__")
+        for sep in ".-_":
+            while content.startswith(sep):
+                content = content[1:]
+            while content.endswith(sep):
+                content = content[:-1]
+        content = content[:128]
+        return content
+
     def set_instance_label(self, label: str):
-        label_id = "_".join(label.split())
+        label_id = self.docker_sanitized_name(label)
         if not label_id:
             raise ValueError("Empty label is not allowed")
         self["label_id"] = label_id
         self["label"] = label.strip()
 
     def rebase_volumes_upon_nua_conf(self):
         self.volume = self.rebased_volumes_upon_package_conf(self.image_nua_config)
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/app_management.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/app_management.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/assign/engine.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/assign/engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Functions to respond to requirement from instance declarations."""
 from collections.abc import Callable
 from pprint import pformat
 
-from nua.lib.panic import info, show, warning
+from nua.lib.panic import debug, show, warning
 from nua.lib.tool.state import verbosity
 
 from ..app_instance import AppInstance
 from ..persistent import Persistent
 from ..resource import Resource
 from ..utils import dehyphen
 from .evaluators import (  # site_environment,
@@ -28,46 +28,47 @@
     "unique_db": unique_db,
     "unique_user": unique_user,
 }
 EVALUATOR_LATE_FCT = {}
 
 
 def instance_key_evaluator(
-    site: AppInstance,
+    app: AppInstance,
     resource: Resource | None = None,
     late_evaluation: bool = False,
     port: dict | None = None,
 ) -> dict:
     """Evaluate value for 'env' values declared as dict with dynamic
     parameters, through retrieving persistent value or compute value from
-    specialized functions."""
+    specialized functions.
+    """
     result = {}
     if resource is None:
-        resource = site
-        persistent = site.persistent("")
+        resource = app
+        persistent = app.persistent("")
     else:
-        persistent = site.persistent(resource.resource_name)
+        persistent = app.persistent(resource.resource_name)
     if port is None:
         dynamics = {k: v for k, v in resource.env.items() if isinstance(v, dict)}
     else:
         dynamics = {k: v for k, v in port.items() if isinstance(v, dict)}
     with verbosity(3):
-        info(f"instance_key_evaluator ({late_evaluation=}):\n    {pformat(dynamics)}")
+        debug(f"instance_key_evaluator ({late_evaluation=}):\n    {pformat(dynamics)}")
     if not dynamics:
         return {}
     for destination_key, requirement in dynamics.items():
         evaluate_requirement(
             resource,
             destination_key,
             requirement,
             persistent,
             result,
             late_evaluation,
         )
-    site.set_persistent(persistent)
+    app.set_persistent(persistent)
     return result
 
 
 def evaluate_requirement(
     resource: Resource,
     destination_key: str,
     requirement: dict,
@@ -83,15 +84,15 @@
         result = function(
             resource,
             destination_key,
             requirement,
             persistent,
         )
         with verbosity(3):
-            show(f"generated value: {result}")
+            debug(f"generated value: {result}")
     else:
         warning(f"Requirement maybe not valid for {destination_key}, key set to empty")
         result = {destination_key: ""}
     env.update(result)
     maybe_display_value(requirement, result)
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/assign/evaluators.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/assign/evaluators.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         persistent.delete(destination_key)
         return func(resource, destination_key, requirement)
 
     return wrapper
 
 
 def no_persistent_value(func):
-    """Dummy wrapper to remove thirf argument."""
+    """Wrapper to mask of the persistent argument."""
 
     @wraps(func)
     def wrapper(
         resource: Resource,
         destination_key: str,
         requirement: dict,
         _persistent: Persistent,
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_engine.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/backup/backup_engine.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_functions.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/backup/backup_functions.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/backup/backup_report.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/backup/backup_report.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/bootstrap/bootstrap.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/bootstrap/bootstrap.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/certbot.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/certbot.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,16 +9,15 @@
     - NUA_CERTBOT_VERBOSE: show certbot log
     - NUA_CERTBOT_TEST: use certbot test environment (only for tests)
 """
 
 import os
 from pprint import pformat
 
-from nua.lib.console import print_red
-from nua.lib.panic import Abort, vprint
+from nua.lib.panic import Abort, bold_debug, debug, red_line
 from nua.lib.tool.state import verbosity
 
 from nua.orchestrator import config
 
 from .commands import apply_auto_strategy, apply_none_strategy
 
 CERTBOT_CONF = "nua.orchestrator.certbot.config"
@@ -45,22 +44,22 @@
     for site in apps:
         # hostname is "www.exemple.com"
         # -> top domain is "exemple.com"
         domains = tops.get(site.top_domain, set())
         domains.add(site.hostname)
         tops[site.top_domain] = domains
     with verbosity(3):
-        print("certbot registration for:")
-        print(pformat(tops))
+        bold_debug("certbot registration for:")
+        debug(pformat(tops))
     strategy = get_certbot_strategy()
     strategy_function = ALLOWED_STRATEGY[strategy]
     for top_domain, domains in tops.items():
         strategy_function(top_domain, list(domains))
     with verbosity(3):
-        vprint("register_certbot_domains() done")
+        debug("register_certbot_domains() done")
 
 
 def get_certbot_strategy() -> str:
     default = "auto"
     strategy = config.read("nua", "host", "certbot_strategy") or default
     strategy = os.environ.get("NUA_CERTBOT_STRATEGY") or strategy
     strategy = strategy.strip().lower()
@@ -70,10 +69,11 @@
 
 def protocol_prefix() -> str:
     return STRATEGY_PROTO[get_certbot_strategy()]
 
 
 def assert_valid_certbot_strategy(strategy: str):
     if strategy not in ALLOWED_STRATEGY:
-        print_red("Allowed values for certbot_strategy are:")
-        print_red(f"{ALLOWED_STRATEGY}")
-        raise Abort(f"Unknown certbot_strategy: {strategy}")
+        with verbosity(0):
+            red_line("Allowed values for certbot_strategy are:")
+            red_line(f"{ALLOWED_STRATEGY}")
+        raise Abort(f"Unknown certbot strategy: {strategy}")
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/commands.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     - NUA_CERTBOT_VERBOSE: show certbot log
     - NUA_CERTBOT_TEST: use certbot test environment (only for tests)
 """
 
 import os
 from pathlib import Path
 
-from nua.lib.panic import important, show, vprint
+from nua.lib.panic import debug, important, show
 from nua.lib.shell import sh
 from nua.lib.tool.state import verbosity
 
 from nua.orchestrator import config
 
 from ..nginx.cmd import nginx_is_active, nginx_restart, nginx_stop
 from ..nua_env import certbot_exe, nua_home_path
@@ -61,15 +61,15 @@
         email = "--register-unsafely-without-email"
     run_args.append(email)
     run_args.append(f"-d {domain}")
     return " ".join(run_args)
 
 
 def apply_none_strategy(_top_domain: str, domains: list[str]):
-    with verbosity(1):
+    with verbosity(0):
         important(f"Use HTTP protocol for: {' '.join(domains)}")
     return
 
 
 def cert_exists(domain: str) -> bool:
     path = letsencrypt_path() / "live" / domain
     if os.getuid():  # aka not root
@@ -86,60 +86,49 @@
     else:
         prefix = ""
     standalone_cmd = certbot_certonly(domain, "--standalone")
     cmd = f"{prefix}{standalone_cmd}"
     with verbosity(2):
         show(cmd)
     output = sh(cmd, show_cmd=False, capture_output=True)
-    with verbosity(2):
-        vprint(output)
-    # cmd = f"{prefix}systemctl start nginx"
-    # with verbosity(2):
-    #     show(cmd)
-    # output = sh(cmd, show_cmd=False, capture_output=True)
-    # with verbosity(3):
-    #     vprint(output)
+    if output:
+        with verbosity(2):
+            debug(output)
 
 
 def gen_cert_nginx(domain: str):
     with verbosity(3):
-        print("known domain, will register with --nginx certbot option:", domain)
+        debug("known domain, will register with --nginx certbot option:", domain)
     if os.getuid():  # aka not root
         prefix = "sudo "
     else:
         prefix = ""
     nginx_cmd = certbot_certonly(domain, "--nginx")
     cmd = f"{prefix}{nginx_cmd}"
     with verbosity(2):
         show(cmd)
     output = sh(cmd, show_cmd=False, capture_output=True)
-    with verbosity(2):
-        vprint(output)
-    # replaced by deploy-hook tag in cli.ini :
-    # cmd = f"{prefix}systemctl reload-or-restart nginx"
-    # with verbosity(2):
-    #     show(cmd)
-    # output = sh(cmd, show_cmd=False, capture_output=True)
-    # with verbosity(3):
-    #     vprint(output)
+    if output:
+        with verbosity(2):
+            debug(output)
 
 
 def apply_auto_strategy(top_domain: str, domains: list[str]):
     """Convert just created HTTP configuration (by nginx template) to HTTPS
     using certbot (if strategy is 'auto').
 
     Each domain of the list uses the same SSL key.
 
     - implementation mode "auto":
         - let certbot rewrite redirections,
         - let certbot manage cron,
         - apply "auto" rules and parameters.
     """
     sorted_domains = sorted(domains)
-    with verbosity(1):
+    with verbosity(0):
         important(f"Use HTTPS protocol (Certbot) for: {' '.join(sorted_domains)}")
     # cmd = certbot_run(top_domain, domains)
     # cmd = certbot_certonly(top_domain, domains)
     #
     # If all domain are already known from letsencrypt, we may try a direct
     # reload using nginx (so without killing nginx websites)
     # Else, we need to stop nginx and use the standalone procedure.
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf` & `nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/config/options-ssl-nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/certbot/installer.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/certbot/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/api.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/api.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/deploy_remove.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/deploy_remove.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,23 +24,29 @@
     uninstaller.remove_all_deployed_managed_volumes()
     uninstaller.post_full_uninstall()
 
 
 def remove_nua_domain(domain: str):
     """Remove some deployed app instance, erasing its data and container.
 
-    WIP: at the moment requires identification of the instance per domain name.
+    Deprecated: requires identification of the instance per domain name.
     """
     deployer = AppDeployment()
     stopping_apps = deployer.instances_of_domain(domain)
     deployer.remove_nginx_configuration(domain)
-    deployer.stop_deployed_apps(domain, stopping_apps)
-    deployer.remove_container_and_network(domain, stopping_apps)
-    deployer.remove_managed_volumes(stopping_apps)
-    deployer.remove_deployed_instance(domain, stopping_apps)
+    deployer.remove_app_list(stopping_apps)
+    deployer.post_deployment()
+
+
+def remove_nua_label(label: str):
+    """Remove some deployed app instance, erasing its data and container."""
+    deployer = AppDeployment()
+    removed_app = deployer.instance_of_label(label)
+    deployer.remove_nginx_configuration(removed_app.domain)
+    deployer.remove_app_list([removed_app])
     deployer.post_deployment()
 
 
 def deploy_merge_nua_app(merge_config: str):
     """Add somme app config to the deplyed list."""
     deployer = AppDeployment()
     deployer.local_services_inventory()
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/restore.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/start_stop.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/start_stop.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/commands/status.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/configuration.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/configuration.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/debug.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/debug.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/init.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/init.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/cli/main.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from . import debug
 from .commands.api import API
 from .commands.backup import backup_all
 from .commands.deploy_remove import (
     deploy_merge_nua_app,
     deploy_nua_apps,
     remove_nua_domain,
+    remove_nua_label,
 )
 from .commands.restore import restore_nua_apps_replay, restore_nua_apps_strict
 from .commands.start_stop import (
     restart_nua_instance_domain,
     start_nua_instance_domain,
     stop_nua_instance_domain,
 )
@@ -61,14 +62,15 @@
 option_restore_strict = typer.Option(
     False, "--strict/--replay", help="Use strict restore mode."
 )
 option_json = typer.Option(False, "--json", help="Output result as JSON.")
 option_short = typer.Option(False, help="Show short text result.")
 option_raw = typer.Option(False, "--raw", help="Return raw result (not JSON).")
 option_domain = typer.Option("", "--domain", "-d", help="Select domain to stop.")
+option_label = typer.Option("", "--label", "-l", help="Select label to stop.")
 
 
 def _print_version():
     typer.echo(f"Nua orchestrator local version: {__version__}")
 
 
 def usage():
@@ -77,15 +79,15 @@
     raise typer.Exit(0)
 
 
 @app.command("status")
 def status_local():
     """Status of orchestrator."""
     initialization()
-    set_verbosity(1)
+    set_verbosity(0)
     status()
 
 
 @app.command("reload")
 def reload_local():
     """Rebuild config and restart apps."""
     print("Not implemented yet.")
@@ -137,24 +139,27 @@
         warning("Unknown file format.")
 
 
 @app.command("remove")
 def remove_local(
     verbose: int = opt_verbose,
     colorize: bool = option_color,
+    label: str = option_label,
     domain: str = option_domain,
 ):
     """Remove a deployed instance and all its data."""
     set_verbosity(verbose)
     set_color(colorize)
     initialization()
-    if domain:
+    if label:
+        remove_nua_label(label)
+    elif domain:
         remove_nua_domain(domain)
     else:
-        print("WIP: currently a domain must be provided.")
+        print("WIP: currently a label or domain must be provided.")
 
 
 @app.command("restore")
 def restore_local(
     verbose: int = opt_verbose,
     colorize: bool = option_color,
     strict: bool = option_restore_strict,
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/auth.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/auth.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/deployconfig.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/deployconfig.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/host.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/host.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/image.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/image.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/instance.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/instance.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/model/setting.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/model/setting.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db/store.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db/store.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,26 @@
         if existing:
             session.delete(existing)
         session.flush()
         session.add(new_instance)
         session.commit()
 
 
+# for future use
+# def load_instance_config(label_id: str = "") -> dict:
+#     """Load nua instance configuration dict from local DB (table 'instance')."""
+#     with Session() as session:
+#         existing = session.query(Instance).filter_by(label_id=label_id).first()
+#         if existing:
+#             site_config = existing.site_config
+#         else:
+#             site_config = {}
+#         return site_config
+
+
 def list_instances_all() -> list[Instance]:
     with Session() as session:
         return session.query(Instance).all()
 
 
 # Not used ?
 # def list_instances_all_short() -> list[str]:
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_migration/tools.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_migration/tools.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.json` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mariadb.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mariadb.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mariadb.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/mongo.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/mongo.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.json` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/postgres.json`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/postgres.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/redis-cache.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/redis-cache.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_plugins/sqlite.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_plugins/sqlite.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/mariadb_utils.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_utils/mariadb_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     sudo apt-get install libmariadb3 libmariadb-dev
 """
 import os
 import re
 from pathlib import Path
 from time import sleep
 
-from nua.agent.db.mariadb_manager import NUA_MARIADB_PWD_FILE
 from nua.lib.actions import install_package_list, installed_packages
 from nua.lib.console import print_magenta, print_red
+from nua.lib.db.mariadb_manager import NUA_MARIADB_PWD_FILE
 from nua.lib.exec import exec_as_root, exec_as_root_daemon
 from nua.lib.gen_password import gen_password
 from nua.lib.panic import warning
 from nua.lib.shell import chown_r, sh
 
 MARIADB_VERSION = "10.6"
 RE_PORT = re.compile(r"\s*port\s*=\s*(\d+)")
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/db_utils/postgres_utils.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/db_utils/postgres_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Nua postgresql related commands."""
 import os
 import re
 from pathlib import Path
 
-from nua.agent.db.postgres_manager import NUA_PG_PWD_FILE
 from nua.lib.actions import install_package_list, installed_packages
 from nua.lib.console import print_magenta, print_red
+from nua.lib.db.postgres_manager import NUA_PG_PWD_FILE
 from nua.lib.exec import mp_exec_as_postgres
 from nua.lib.gen_password import gen_password
 from nua.lib.panic import warning
 from nua.lib.shell import chown_r, sh
 
 from ..docker_utils import docker_host_gateway_ip
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/default_conf/nua_defaults_settings.toml` & `nua_orchestrator-0.5.15/src/nua/orchestrator/default_conf/nua_defaults_settings.toml`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/deploy_utils.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/deploy_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Class to manage the deployment of a group of AppInstance."""
 from collections.abc import Callable
 from pathlib import Path
 from pprint import pformat
 
 import docker
 import docker.types
-from nua.autobuild.docker_build_utils import display_one_docker_img, docker_require
-from nua.build.archive_search import ArchiveSearch
+from nua.lib.archive_search import ArchiveSearch
+from nua.lib.docker import display_one_docker_img, docker_require
 from nua.lib.panic import Abort, important, info, vprint, warning
 from nua.lib.tool.state import verbosity
 
 from .app_instance import AppInstance
 from .db import store
 from .docker_utils import (  # docker_volume_prune,
     docker_host_gateway_ip,
@@ -45,15 +45,15 @@
     path = Path(image_path)
     # image is local, so we can mount it directly
     if not path.is_file():
         warning("Local Docker image does not exist")
         raise FileNotFoundError(path)
 
     arch_search = ArchiveSearch(path)
-    image_nua_config = arch_search.nua_config_dict()
+    image_nua_config = arch_search.get_nua_config_dict()
     if not image_nua_config:
         raise Abort(
             f"image non compatible Nua: {path}.", explanation="No Nua config found"
         )
 
     metadata = image_nua_config["metadata"]
     msg = "Installing App: {id} {version}, {title}".format(**metadata)
@@ -65,15 +65,15 @@
     with open(path, "rb") as input:  # noqa: S108
         loaded = client.images.load(input)
     if not loaded or len(loaded) > 1:
         warning("loaded image result is strange:", f"{loaded=}")
     loaded_img = loaded[0]
     # images_after = {img.id for img in client.images.list()}
     # new = images_after - images_before
-    with verbosity(1):
+    with verbosity(0):
         important("Installing image:")
         display_one_docker_img(loaded_img)
     return loaded_img.id, image_nua_config
 
 
 def port_allocator(start_ports: int, end_ports: int, allocated_ports: set) -> Callable:
     def allocator() -> int:
@@ -180,24 +180,24 @@
     with verbosity(4):
         vprint(f"start_one_container() run_params:\n{pformat(run_params)}")
     secrets = secrets_dict(rsite.requested_secrets)
     new_container = docker_run(rsite, secrets)
     rsite.container_id = new_container.id
     if mounted_volumes:
         rsite.run_params["mounts"] = True
-    with verbosity(1):
+    with verbosity(0):
         info(f"    -> container of name: {rsite.container_name}")
         info(f"            container id: {rsite.container_id_short}")
         if rsite.network_name:
             info(f"    connected to network: {rsite.network_name}")
 
 
-def stop_one_app_containers(site: AppInstance):
-    stop_one_container(site)
-    for resource in site.resources:
+def stop_one_app_containers(app: AppInstance):
+    stop_one_container(app)
+    for resource in app.resources:
         stop_one_container(resource)
     # docker_network_prune() : no, need to keep same network to easily restart the
     # container with same network.
 
 
 def start_one_app_containers(site: AppInstance):
     for resource in site.resources:
@@ -208,36 +208,36 @@
 def restart_one_app_containers(site: AppInstance):
     for resource in site.resources:
         restart_one_deployed_container(resource)
     restart_one_deployed_container(site)
 
 
 def stop_one_container(rsite: Resource):
-    with verbosity(1):
+    with verbosity(0):
         info(f"    -> stop container of name: {rsite.container_name}")
         info(f"                 container id: {rsite.container_id_short}")
     stop_containers([rsite.container_name])
 
 
 def stop_containers(container_names: list[str]):
     for name in container_names:
         if not name:
             continue
         docker_stop_container_name(name)
 
 
 def start_one_deployed_container(rsite: Resource):
-    with verbosity(1):
+    with verbosity(0):
         info(f"    -> start container of name: {rsite.container_name}")
         info(f"                  container id: {rsite.container_id_short}")
     start_containers([rsite.container_name])
 
 
 def restart_one_deployed_container(rsite: Resource):
-    with verbosity(1):
+    with verbosity(0):
         info(f"    -> restart container of name: {rsite.container_name}")
         info(f"                    container id: {rsite.container_id_short}")
     restart_containers([rsite.container_name])
 
 
 def start_containers(container_names: list[str]):
     for name in container_names:
@@ -272,15 +272,15 @@
 def deactivate_all_instances():
     """Find all instances in DB.
 
     - remove container if it exists
     - remove site from DB
     """
     for instance in store.list_instances_all():
-        with verbosity(2):
+        with verbosity(1):
             msg = f"Removing instance '{instance.app_id}' on '{instance.domain}'"
             info(msg)
         site_config = instance.site_config
         container_names = [
             res.get("container_name", "") for res in site_config.get("resources", [])
         ]
         container_names.append(site_config.get("container_name", ""))
@@ -358,15 +358,15 @@
 
     resource.image_id = PULLED_IMAGES[resource.image]
     return True
 
 
 def _actual_pull_container(resource: Resource):
     """Retrieve a resource container."""
-    with verbosity(1):
+    with verbosity(0):
         info(f"Pulling image '{resource.image}'")
 
     docker_image = docker_require(resource.image)
     if docker_image:
         PULLED_IMAGES[resource.image] = docker_image.id
-        with verbosity(1):
+        with verbosity(0):
             display_one_docker_img(docker_image)
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/docker_utils.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/docker_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,26 @@
 from subprocess import run  # noqa: S404
 from time import sleep
 
 from docker import DockerClient
 from docker.errors import APIError, NotFound
 from docker.models.containers import Container
 from docker.models.images import Image
-from nua.autobuild.docker_build_utils import docker_require
 from nua.lib.console import print_red
-from nua.lib.panic import Abort, important, info, show, vprint, warning
+from nua.lib.docker import docker_require
+from nua.lib.panic import (
+    Abort,
+    bold_debug,
+    debug,
+    important,
+    info,
+    show,
+    vprint,
+    warning,
+)
 from nua.lib.shell import chmod_r, mkdir_p
 from nua.lib.tool.state import verbosity
 
 from . import config
 from .db import store
 from .resource import Resource
 from .volume import Volume
@@ -145,16 +154,17 @@
     try:
         container.restart()
     except APIError as e:
         warning(f"Restarting container error: {e}")
 
 
 def _docker_remove_container(name: str, force=False, volume=False):
-    if force and verbosity(1):
-        warning(f"removing container with '--force': {name}")
+    if force:
+        with verbosity(0):
+            warning(f"removing container with '--force': {name}")
     for cont in docker_container_of_name(name):
         cont.remove(v=volume, force=force)
 
 
 def _docker_display_not_removed(name: str):
     for remain in docker_container_of_name(name):
         warning(f"container not removed: {remain}")
@@ -204,15 +214,15 @@
         # FIXME for resource containers
         return
 
     previous_name = store.instance_container(rsite.domain)
     if not previous_name:
         return
 
-    with verbosity(1):
+    with verbosity(0):
         info(f"    -> remove previous container: {previous_name}")
 
     docker_stop_container_name(previous_name)
     docker_remove_container(previous_name)
 
     with verbosity(4):
         containers = docker_container_of_name(previous_name)
@@ -225,23 +235,23 @@
     """Remove container of full domain name from running container and DB."""
     containers = docker_container_of_name(name)
     with verbosity(4):
         vprint(f"Stopping container: {pformat(containers)}")
 
     if not containers:
         if show_warning:
-            with verbosity(2):
+            with verbosity(1):
                 warning(f"no previous container to stop '{name}'")
         return
 
     container = containers[0]
-    with verbosity(2):
+    with verbosity(1):
         info(f"Stopping container '{container.name}'")
     _docker_stop_container(container)
-    with verbosity(2):
+    with verbosity(1):
         info(f"Removing container '{container.name}'")
     try:
         container.remove(v=False, force=True)
     except (NotFound, APIError):
         # container was "autoremoved" after stop
         pass
 
@@ -254,23 +264,26 @@
     could be found in docker daemon:
     """
     previous_name = rsite.run_params.get("name", "")
     if not previous_name:
         return
 
     for container in docker_container_of_name(previous_name):
-        print_red(f"Try removing a container not listed in Nua DB: {container.name}")
+        with verbosity(3):
+            debug(
+                f"For security, try to remove a container not listed in Nua DB: {container.name}"
+            )
         docker_stop_container_name(container.name)
         docker_remove_container(container.name)
 
 
 def erase_previous_container(client: DockerClient, name: str):
     try:
-        with verbosity(2):
-            info(f"Search previous container of name: {name}")
+        with verbosity(4):
+            bold_debug(f"Search previous container of name: {name}")
         container = client.containers.get(name)
         info(f"    -> Remove existing container '{container.name}'")
         container.remove(force=True)
     except APIError:
         pass
 
 
@@ -293,24 +306,24 @@
 def docker_run(rsite: Resource, secrets: dict) -> Container:
     """Wrapper on top of the py-docker run() command.
 
     Returns:
         The new started container.
     """
     params = docker_run_params(rsite)
-    with verbosity(1):
+    with verbosity(0):
         # info(f"Docker run image: {rsite.image_id}")
         info(f"Docker run image: {rsite.image}")
         info(f"        image id: {rsite.image_id_short}")
         with verbosity(2):
             important("Docker run parameters:")
             show(pformat(params))
 
     docker_remove_prior_container_live(rsite)
-    with verbosity(2):
+    with verbosity(1):
         if "network" in params:
             info("Network:", params["network"])
 
     container = _docker_run(rsite, secrets, params)
     with verbosity(3):
         vprint("Docker secrets:", secrets)
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/domain_split.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/domain_split.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/healthcheck.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/healthcheck.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/higher_package.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/higher_package.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/internal_secrets.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/internal_secrets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 
-from nua.agent.db.mariadb_manager import NUA_MARIADB_PWD_FILE
-from nua.agent.db.postgres_manager import NUA_PG_PWD_FILE
+from nua.lib.db.mariadb_manager import NUA_MARIADB_PWD_FILE
+from nua.lib.db.postgres_manager import NUA_PG_PWD_FILE
 
 
 def secrets_dict(key_list: list) -> dict:
     result = {}
     for key in key_list:
         val = read_secret(key)
         if val is not None:
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/cmd.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,41 +21,41 @@
 
 def nginx_stop():
     stop_cmd = "systemctl stop nginx || true"
     if os.geteuid() == 0:
         cmd = stop_cmd
     else:
         cmd = f"sudo {stop_cmd}"
-    with verbosity(2):
+    with verbosity(1):
         show(cmd)
     output = sh(cmd, show_cmd=False, capture_output=True)
     with verbosity(3):
         debug(output)
     sleep(1)
 
 
 def nginx_restart():
     # assuming some recent ubuntu distribution:
     delay = config.read("host", "nginx_wait_after_restart") or 1
-    with verbosity(2):
+    with verbosity(1):
         important("Restart Nginx")
     cmd = "systemctl restart nginx"
     if os.geteuid() == 0:
         sh(cmd, show_cmd=False)
     else:
         sh(f"sudo {cmd}", show_cmd=False)
     sleep(delay)
 
 
 def nginx_reload():
     # assuming some recent ubuntu distribution:
     if not nginx_is_active():
         return nginx_restart()
     delay = config.read("host", "nginx_wait_after_restart") or 1
-    with verbosity(2):
+    with verbosity(1):
         important("Reload Nginx")
     cmd = "systemctl reload nginx"
     if os.geteuid() == 0:
         sh(cmd, show_cmd=False)
     else:
         sh(f"sudo {cmd}", show_cmd=False)
     sleep(delay)
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/css/style.css` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/html/css/style.css`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/html/index.html` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/html/index.html`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/installer.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/installer.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/default_site` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/default_site`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_located.j2` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/http_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/http_not_located.j2` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/http_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_located.j2` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/https_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located.j2` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/https_not_located.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/https_not_located_insec.j2`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/templates/nginx.conf` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/templates/nginx.conf`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nginx/utils.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nginx/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     template: str,
     dest_path: str | Path,
     host: dict,
 ):
     with verbosity(4):
         bold_debug(f"{host['hostname']} template:")
         debug(template)
-    with verbosity(2):
+    with verbosity(1):
         info("Nginx configuration:", dest_path)
     jinja2_render_from_str_template(template, dest_path, host)
     if dest_path.exists():
         with verbosity(3):
             bold_debug("Nginx configuration content:")
             with open(dest_path, encoding="utf8") as rfile:
                 debug(rfile.read())
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nua_db_setup.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nua_db_setup.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/nua_env.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/nua_env.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/persistent.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/persistent.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,21 @@
 from dataclasses import dataclass, field
 from pprint import pformat
 from typing import Any
 
 
 @dataclass
 class Persistent:
-    """Management of persistent generated values (like passwords)."""
+    """Management of persistent generated values (like passwords).
+
+    Persistent data is stored in the AppInstance. A Persistent object contains
+    persitent values for the AppInstance and its ressources. The 'name'
+    attribute identifies the resource owning the data, use '' as resource_name for
+    the data own by the AppInstance itself.
+    """
 
     name: str
     _dict: dict = field(default_factory=dict)
 
     @classmethod
     def from_name_dict(cls, name: str, persist_dict: dict) -> Persistent:
         persistent = cls(name)
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/port_normalization.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/port_normalization.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/register_plugins.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/register_plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 import importlib.util
 from collections.abc import Callable
 from importlib import resources as rso
 from pathlib import Path
 from pprint import pformat
 
-from nua.agent.nua_config import hyphen_get
+from nua.lib.nua_config import hyphen_get
 from nua.lib.panic import bold_debug, debug
 from nua.lib.tool.state import verbosity
 
 from .utils import dehyphen, hyphen
 
 LOADED_MODULES = {}
 MODULES_PROPERTIES = {}
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/registry.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   for storage.
 """
 
 import sys
 from pathlib import Path
 
 import docker
-from nua.autobuild.docker_build_utils import image_created_as_iso
+from nua.lib.docker import image_created_as_iso
 
 from . import config
 from .db import store
 
 # need something like: fuser -k 5001/tcp
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/resource.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from collections.abc import Callable
 from copy import deepcopy
 from pprint import pformat
 from typing import Any
 
-from nua.agent.nua_config import nomalize_env_values
+from nua.lib.nua_config import nomalize_env_values
 from nua.lib.panic import Abort, debug, important, vprint, warning
 from nua.lib.tool.state import verbosity
 
 from .backup.backup_engine import backup_resource, backup_volume
 from .backup.backup_report import global_backup_report
 from .healthcheck import HealthCheck
 from .port_normalization import (
@@ -464,15 +464,15 @@
         return reports
 
     def setup_db(self):
         if not is_db_plugins(self.type):
             return
         if setup_fct := load_plugin_function(self.type, "setup_db"):
             setup_fct(self)
-            with verbosity(2):
+            with verbosity(1):
                 vprint(f"setup_db() for resource '{self.resource_name}': {self.type}")
             with verbosity(3):
                 vprint(pformat(self.env))
 
     def configure_db(self):
         with verbosity(4):
             vprint(f"configure_db: {self.type}")
@@ -480,15 +480,15 @@
             with verbosity(4):
                 vprint(f"not a DB: {self.type}")
             return
         if configure_fct := load_plugin_function(self.type, "configure_db"):
             with verbosity(4):
                 vprint(f"configure_fct: {configure_fct}")
             configure_fct(self)
-            with verbosity(2):
+            with verbosity(1):
                 important(f"Configure resource DB '{self.resource_name}': {self.type}")
             with verbosity(3):
                 debug(pformat(self))
 
     def load_meta_packages_requirements(self):
         """Some plugin may require some meta-packages requirements for main
         app.
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/resource_deps.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/resource_deps.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/docker_remove_all.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/docker_remove_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             print(f"Remove {ctn.name}")
             ctn.remove(force=True)
         except (APIError, NotFound) as e:
             print(f"Error while stopping: {e}")
 
 
 def main():
-    set_verbosity(2)
+    set_verbosity(1)
     print("Docker containers:")
     list_containers()
     stop_containers()
     print("Docker containers after stop:")
     list_containers()
     remove_containers()
     print("Docker containers after remove:")
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/mariadb_restore.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/mariadb_restore.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/print_instances.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/print_instances.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/scripts/set_pg_pwd.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/scripts/set_pg_pwd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/search_cmd.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/search_cmd.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/services/postgres.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/services/postgres.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_base.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/services/service_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from nua.autobuild.docker_build_utils import display_one_docker_img
+from nua.lib.docker import display_one_docker_img
 from nua.lib.panic import vprint
 from nua.lib.tool.state import verbosity
 
 from ..docker_utils import pull_docker_image
 
 
 class ServiceBase:
     def __init__(self, options: dict):
         self.options = options
 
     def aliases(self) -> list:
         return []
 
     def _pull_docker_image(self, required_image) -> bool:
-        with verbosity(1):
+        with verbosity(0):
             vprint(f"pulling docker image '{required_image}'")
         image = pull_docker_image(required_image)
         if image:
-            with verbosity(1):
+            with verbosity(0):
                 display_one_docker_img(image)
             return True
         else:
             return False
 
     def check_site_configuration(self, _site: dict | None = None) -> bool:
         required_image = self.options.get("image")
```

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/services/service_loader.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/services/service_loader.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/util/deep_access_dict.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/util/deep_access_dict.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/utils.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/src/nua/orchestrator/volume.py` & `nua_orchestrator-0.5.15/src/nua/orchestrator/volume.py`

 * *Files identical despite different names*

### Comparing `nua_orchestrator-0.5.14/PKG-INFO` & `nua_orchestrator-0.5.15/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: nua-orchestrator
-Version: 0.5.14
+Version: 0.5.15
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
-Requires-Dist: nua-agent (==0.5.14)
-Requires-Dist: nua-autobuild (==0.5.14)
-Requires-Dist: nua-build (==0.5.14)
-Requires-Dist: nua-lib (==0.5.14)
+Requires-Dist: nua-lib (==0.5.15)
 Requires-Dist: paramiko (>=2.11.0,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21,<0.22)
 Requires-Dist: pyyaml (>=6,<7)
 Requires-Dist: setuptools
 Requires-Dist: tomli (>=2,<3)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
@@ -146,7 +143,13 @@
 
 Nua installation done for user 'nua' on this host.
 Command 'nua --help':
 ```
 
 At the end of the installation, the available commands are displayed.
 
+## Development
+
+### Dependency graph
+
+![Dependency graph](./doc/dependency-graph.png)
+
```

