# Comparing `tmp/mitzu-0.6.0rc3.tar.gz` & `tmp/mitzu-0.6.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitzu-0.6.0rc3.tar", max compression
+gzip compressed data, was "mitzu-0.6.0rc4.tar", max compression
```

## Comparing `mitzu-0.6.0rc3.tar` & `mitzu-0.6.0rc4.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     1082 2023-04-25 15:24:54.935289 mitzu-0.6.0rc3/LICENSE.txt
--rw-r--r--   0        0        0     2235 2023-04-25 15:24:54.935289 mitzu-0.6.0rc3/README.md
--rw-r--r--   0        0        0     6148 2023-04-25 15:24:55.327295 mitzu-0.6.0rc3/mitzu/.DS_Store
--rw-r--r--   0        0        0      865 2023-04-25 15:25:54.424133 mitzu-0.6.0rc3/mitzu/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/__init__.py
--rw-r--r--   0        0        0     1762 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/adapter_factory.py
--rw-r--r--   0        0        0     5234 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/athena_adapter.py
--rw-r--r--   0        0        0     6072 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/databricks_adapter.py
--rw-r--r--   0        0        0     2261 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/file_adapter.py
--rw-r--r--   0        0        0     2563 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/generic_adapter.py
--rw-r--r--   0        0        0      898 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/helper.py
--rw-r--r--   0        0        0     3422 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/mysql_adapter.py
--rw-r--r--   0        0        0     2297 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/postgresql_adapter.py
--rw-r--r--   0        0        0     4085 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/redshift_adapter.py
--rw-r--r--   0        0        0     3344 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/snowflake_adapter.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      660 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/__init__.py
--rw-r--r--   0        0        0      701 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5071 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6415 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
--rw-r--r--   0        0        0     9751 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1844 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
--rw-r--r--   0        0        0      672 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/__init__.py
--rw-r--r--   0        0        0      713 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5010 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
--rw-r--r--   0        0        0     6601 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
--rw-r--r--   0        0        0    10073 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
--rw-r--r--   0        0        0     1848 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
--rw-r--r--   0        0        0    39656 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy_adapter.py
--rw-r--r--   0        0        0     5009 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/sqlite_adapter.py
--rw-r--r--   0        0        0     6687 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/adapters/trino_adapter.py
--rw-r--r--   0        0        0     1394 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/helper.py
--rw-r--r--   0        0        0    53851 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/model.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/notebook/__init__.py
--rw-r--r--   0        0        0     6818 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/notebook/model_loader.py
--rw-r--r--   0        0        0     5424 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/project_discovery.py
--rw-r--r--   0        0        0     2086 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/project_serialization.py
--rw-r--r--   0        0        0      785 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/samples/__init__.py
--rw-r--r--   0        0        0     3794 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/samples/data_ingestion.py
--rw-r--r--   0        0        0    10141 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/samples/sample_data_generator.py
--rw-r--r--   0        0        0    11910 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/serialization.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/__init__.py
--rw-r--r--   0        0        0     6951 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/charts.py
--rw-r--r--   0        0        0     1866 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/common.py
--rw-r--r--   0        0        0      941 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/labels.py
--rw-r--r--   0        0        0     7547 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/plot.py
--rw-r--r--   0        0        0     5767 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/titles.py
--rw-r--r--   0        0        0     3181 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/tooltips.py
--rw-r--r--   0        0        0     3339 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/transform_conv.py
--rw-r--r--   0        0        0     1278 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/visualization/transform_retention.py
--rw-r--r--   0        0        0     6148 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/.DS_Store
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/__init__.py
--rw-r--r--   0        0        0     5347 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/explore_page.css
--rw-r--r--   0        0        0   147145 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/favicon.ico
--rw-r--r--   0        0        0    46702 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/logo.png
--rw-r--r--   0        0        0    43472 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/mitzu-logo-light.svg
--rw-r--r--   0        0        0    49422 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/athena.png
--rw-r--r--   0        0        0    10321 2023-04-25 15:24:55.331295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/clickhouse.png
--rw-r--r--   0        0        0   119554 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/databricks.png
--rw-r--r--   0        0        0     3008 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/mysql.png
--rw-r--r--   0        0        0     2446 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/pandas.png
--rw-r--r--   0        0        0     5338 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/postgresql.png
--rw-r--r--   0        0        0     8512 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/redshift.png
--rw-r--r--   0        0        0    93500 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/snowflake.png
--rw-r--r--   0        0        0    48681 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/sqlite.png
--rw-r--r--   0        0        0    34219 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/trino.png
--rw-r--r--   0        0        0    13549 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/authorizer.py
--rw-r--r--   0        0        0     3557 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/cognito.py
--rw-r--r--   0        0        0     1594 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/decorator.py
--rw-r--r--   0        0        0     2777 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/auth/google.py
--rw-r--r--   0        0        0     7392 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/cache.py
--rw-r--r--   0        0        0     2966 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/caching_dataset_adapter.py
--rw-r--r--   0        0        0     2595 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/configs.py
--rw-r--r--   0        0        0     2750 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/dependencies.py
--rw-r--r--   0        0        0     4833 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/helper.py
--rw-r--r--   0        0        0     8355 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/model.py
--rw-r--r--   0        0        0      408 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/navbar.py
--rw-r--r--   0        0        0     6112 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/offcanvas.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/connections/__init__.py
--rw-r--r--   0        0        0    15406 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/connections/manage_connections_component.py
--rw-r--r--   0        0        0     4195 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/connections_page.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards/__init__.py
--rw-r--r--   0        0        0    21143 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
--rw-r--r--   0        0        0     9799 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards.py
--rw-r--r--   0        0        0    14789 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/edit_user.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/__init__.py
--rw-r--r--   0        0        0     5724 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/complex_segment_handler.py
--rw-r--r--   0        0        0     6488 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/dates_selector_handler.py
--rw-r--r--   0        0        0     5564 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/event_segment_handler.py
--rw-r--r--   0        0        0    16412 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/explore_page.py
--rw-r--r--   0        0        0    10152 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/graph_handler.py
--rw-r--r--   0        0        0    10940 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_config_handler.py
--rw-r--r--   0        0        0     2375 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_segments_handler.py
--rw-r--r--   0        0        0     1565 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_type_handler.py
--rw-r--r--   0        0        0     9783 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/simple_segment_handler.py
--rw-r--r--   0        0        0     4644 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore/toolbar_handler.py
--rw-r--r--   0        0        0     1401 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/explore_project.py
--rw-r--r--   0        0        0     1708 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/home.py
--rw-r--r--   0        0        0     3894 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/login.py
--rw-r--r--   0        0        0     4898 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_connection.py
--rw-r--r--   0        0        0     1315 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_dashboard.py
--rw-r--r--   0        0        0    10034 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_event_defs.py
--rw-r--r--   0        0        0    11756 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_project.py
--rw-r--r--   0        0        0    10013 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/manage_saved_metrics.py
--rw-r--r--   0        0        0     1733 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/paths.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/__init__.py
--rw-r--r--   0        0        0    35893 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/event_tables_config.py
--rw-r--r--   0        0        0      587 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/helper.py
--rw-r--r--   0        0        0     9400 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects/manage_project_component.py
--rw-r--r--   0        0        0     4901 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/projects_page.py
--rw-r--r--   0        0        0     3146 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/pages/users.py
--rw-r--r--   0        0        0        0 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/service/__init__.py
--rw-r--r--   0        0        0     2172 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/service/events_service.py
--rw-r--r--   0        0        0     5302 2023-04-25 15:24:55.335295 mitzu-0.6.0rc3/mitzu/webapp/service/navbar_service.py
--rw-r--r--   0        0        0     2105 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/service/secret_service.py
--rw-r--r--   0        0        0     4710 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/service/user_service.py
--rw-r--r--   0        0        0    20518 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/storage.py
--rw-r--r--   0        0        0    25909 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/storage_model.py
--rw-r--r--   0        0        0      666 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/toast.py
--rw-r--r--   0        0        0     4141 2023-04-25 15:24:55.339295 mitzu-0.6.0rc3/mitzu/webapp/webapp.py
--rw-r--r--   0        0        0     2943 2023-04-25 15:25:54.420133 mitzu-0.6.0rc3/pyproject.toml
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-04-29 20:11:16.877457 mitzu-0.6.0rc4/LICENSE.txt
+-rw-r--r--   0        0        0     2235 2023-04-29 20:11:16.877457 mitzu-0.6.0rc4/README.md
+-rw-r--r--   0        0        0     6148 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/.DS_Store
+-rw-r--r--   0        0        0      865 2023-04-29 20:12:16.723844 mitzu-0.6.0rc4/mitzu/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/__init__.py
+-rw-r--r--   0        0        0     1762 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/adapter_factory.py
+-rw-r--r--   0        0        0     5234 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/athena_adapter.py
+-rw-r--r--   0        0        0     6072 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/databricks_adapter.py
+-rw-r--r--   0        0        0     2261 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/file_adapter.py
+-rw-r--r--   0        0        0     2563 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/generic_adapter.py
+-rw-r--r--   0        0        0      898 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/helper.py
+-rw-r--r--   0        0        0     3422 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/mysql_adapter.py
+-rw-r--r--   0        0        0     2297 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/postgresql_adapter.py
+-rw-r--r--   0        0        0     4085 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/redshift_adapter.py
+-rw-r--r--   0        0        0     3344 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/snowflake_adapter.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      660 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/__init__.py
+-rw-r--r--   0        0        0      701 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5071 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6415 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0     9751 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1844 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py
+-rw-r--r--   0        0        0      672 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/__init__.py
+-rw-r--r--   0        0        0      713 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5010 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py
+-rw-r--r--   0        0        0     6601 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py
+-rw-r--r--   0        0        0    10073 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py
+-rw-r--r--   0        0        0     1848 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py
+-rw-r--r--   0        0        0    39656 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy_adapter.py
+-rw-r--r--   0        0        0     5009 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/sqlite_adapter.py
+-rw-r--r--   0        0        0     6687 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/adapters/trino_adapter.py
+-rw-r--r--   0        0        0     1394 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/helper.py
+-rw-r--r--   0        0        0    53851 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/model.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/notebook/__init__.py
+-rw-r--r--   0        0        0     6818 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/notebook/model_loader.py
+-rw-r--r--   0        0        0     5424 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/project_discovery.py
+-rw-r--r--   0        0        0     2086 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/project_serialization.py
+-rw-r--r--   0        0        0      785 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/samples/__init__.py
+-rw-r--r--   0        0        0     3794 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/samples/data_ingestion.py
+-rw-r--r--   0        0        0    10141 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/samples/sample_data_generator.py
+-rw-r--r--   0        0        0    11910 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/serialization.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/__init__.py
+-rw-r--r--   0        0        0     6951 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/charts.py
+-rw-r--r--   0        0        0     1866 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/common.py
+-rw-r--r--   0        0        0      941 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/labels.py
+-rw-r--r--   0        0        0     7547 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/plot.py
+-rw-r--r--   0        0        0     5767 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/titles.py
+-rw-r--r--   0        0        0     3181 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/tooltips.py
+-rw-r--r--   0        0        0     3339 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/transform_conv.py
+-rw-r--r--   0        0        0     1278 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/visualization/transform_retention.py
+-rw-r--r--   0        0        0     6148 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/.DS_Store
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/__init__.py
+-rw-r--r--   0        0        0     5347 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/assets/explore_page.css
+-rw-r--r--   0        0        0   147145 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/assets/favicon.ico
+-rw-r--r--   0        0        0    46702 2023-04-29 20:11:17.273473 mitzu-0.6.0rc4/mitzu/webapp/assets/logo.png
+-rw-r--r--   0        0        0    43472 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/mitzu-logo-light.svg
+-rw-r--r--   0        0        0    49422 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/athena.png
+-rw-r--r--   0        0        0    10321 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/clickhouse.png
+-rw-r--r--   0        0        0   119554 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/databricks.png
+-rw-r--r--   0        0        0     3008 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/mysql.png
+-rw-r--r--   0        0        0     2446 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/pandas.png
+-rw-r--r--   0        0        0     5338 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/postgresql.png
+-rw-r--r--   0        0        0     8512 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/redshift.png
+-rw-r--r--   0        0        0    93500 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/snowflake.png
+-rw-r--r--   0        0        0    48681 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/sqlite.png
+-rw-r--r--   0        0        0    34219 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/trino.png
+-rw-r--r--   0        0        0    13345 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/authorizer.py
+-rw-r--r--   0        0        0     3557 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/cognito.py
+-rw-r--r--   0        0        0     1594 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/decorator.py
+-rw-r--r--   0        0        0     2777 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/auth/google.py
+-rw-r--r--   0        0        0     7392 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/cache.py
+-rw-r--r--   0        0        0     2966 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/caching_dataset_adapter.py
+-rw-r--r--   0        0        0     2511 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/configs.py
+-rw-r--r--   0        0        0     2750 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/dependencies.py
+-rw-r--r--   0        0        0     4833 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/helper.py
+-rw-r--r--   0        0        0     8375 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/model.py
+-rw-r--r--   0        0        0      408 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/navbar.py
+-rw-r--r--   0        0        0     5802 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/offcanvas.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/connections/__init__.py
+-rw-r--r--   0        0        0    15464 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/connections/manage_connections_component.py
+-rw-r--r--   0        0        0     4281 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/connections_page.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards/__init__.py
+-rw-r--r--   0        0        0    21140 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py
+-rw-r--r--   0        0        0     9846 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards.py
+-rw-r--r--   0        0        0    14708 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/edit_user.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/__init__.py
+-rw-r--r--   0        0        0     5724 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/complex_segment_handler.py
+-rw-r--r--   0        0        0     6488 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/dates_selector_handler.py
+-rw-r--r--   0        0        0     5564 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/event_segment_handler.py
+-rw-r--r--   0        0        0    16412 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/explore_page.py
+-rw-r--r--   0        0        0    10152 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/graph_handler.py
+-rw-r--r--   0        0        0    10940 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_config_handler.py
+-rw-r--r--   0        0        0     2375 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_segments_handler.py
+-rw-r--r--   0        0        0     1565 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_type_handler.py
+-rw-r--r--   0        0        0     9783 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/simple_segment_handler.py
+-rw-r--r--   0        0        0     4644 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore/toolbar_handler.py
+-rw-r--r--   0        0        0     1401 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/explore_project.py
+-rw-r--r--   0        0        0     1751 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/home.py
+-rw-r--r--   0        0        0     3956 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/login.py
+-rw-r--r--   0        0        0     5027 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_connection.py
+-rw-r--r--   0        0        0     1315 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_dashboard.py
+-rw-r--r--   0        0        0    10128 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_event_defs.py
+-rw-r--r--   0        0        0    11849 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_project.py
+-rw-r--r--   0        0        0    10013 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/manage_saved_metrics.py
+-rw-r--r--   0        0        0     1733 2023-04-29 20:11:17.277473 mitzu-0.6.0rc4/mitzu/webapp/pages/paths.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/__init__.py
+-rw-r--r--   0        0        0    36159 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/event_tables_config.py
+-rw-r--r--   0        0        0      587 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/helper.py
+-rw-r--r--   0        0        0     9400 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects/manage_project_component.py
+-rw-r--r--   0        0        0     5034 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/projects_page.py
+-rw-r--r--   0        0        0     3185 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/pages/users.py
+-rw-r--r--   0        0        0        0 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/__init__.py
+-rw-r--r--   0        0        0     2172 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/events_service.py
+-rw-r--r--   0        0        0     5302 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/navbar_service.py
+-rw-r--r--   0        0        0     2105 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/secret_service.py
+-rw-r--r--   0        0        0     4758 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/service/user_service.py
+-rw-r--r--   0        0        0    20518 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/storage.py
+-rw-r--r--   0        0        0    25939 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/storage_model.py
+-rw-r--r--   0        0        0      666 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/toast.py
+-rw-r--r--   0        0        0     4141 2023-04-29 20:11:17.281473 mitzu-0.6.0rc4/mitzu/webapp/webapp.py
+-rw-r--r--   0        0        0     2943 2023-04-29 20:12:16.719844 mitzu-0.6.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 mitzu-0.6.0rc4/PKG-INFO
```

### Comparing `mitzu-0.6.0rc3/LICENSE.txt` & `mitzu-0.6.0rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/README.md` & `mitzu-0.6.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/.DS_Store` & `mitzu-0.6.0rc4/mitzu/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/__init__.py` & `mitzu-0.6.0rc4/mitzu/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     TimeWindow,
     TimeGroup,
     DiscoverySettings,
     WebappSettings,
 )
 from mitzu.samples import get_sample_discovered_project
 
-__version__ = "0.6.0-rc.3"
+__version__ = "0.6.0-rc.4"
 
 
 __all__ = [
     "Connection",
     "ConnectionType",
     "Project",
     "EventDataTable",
```

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/adapter_factory.py` & `mitzu-0.6.0rc4/mitzu/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/athena_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/athena_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/databricks_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/databricks_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/file_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/file_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/generic_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/generic_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/helper.py` & `mitzu-0.6.0rc4/mitzu/adapters/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/mysql_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/mysql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/postgresql_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/postgresql_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/redshift_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/redshift_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/snowflake_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/snowflake_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/__init__.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/athena/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/__init__.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/compiler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/datatype.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy/databricks/sqlalchemy/error.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlalchemy_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/sqlite_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/sqlite_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/adapters/trino_adapter.py` & `mitzu-0.6.0rc4/mitzu/adapters/trino_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/helper.py` & `mitzu-0.6.0rc4/mitzu/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/model.py` & `mitzu-0.6.0rc4/mitzu/model.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/notebook/model_loader.py` & `mitzu-0.6.0rc4/mitzu/notebook/model_loader.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/project_discovery.py` & `mitzu-0.6.0rc4/mitzu/project_discovery.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/project_serialization.py` & `mitzu-0.6.0rc4/mitzu/project_serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/samples/__init__.py` & `mitzu-0.6.0rc4/mitzu/samples/__init__.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/samples/data_ingestion.py` & `mitzu-0.6.0rc4/mitzu/samples/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/samples/sample_data_generator.py` & `mitzu-0.6.0rc4/mitzu/samples/sample_data_generator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/serialization.py` & `mitzu-0.6.0rc4/mitzu/serialization.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/charts.py` & `mitzu-0.6.0rc4/mitzu/visualization/charts.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/common.py` & `mitzu-0.6.0rc4/mitzu/visualization/common.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/labels.py` & `mitzu-0.6.0rc4/mitzu/visualization/labels.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/plot.py` & `mitzu-0.6.0rc4/mitzu/visualization/plot.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/titles.py` & `mitzu-0.6.0rc4/mitzu/visualization/titles.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/tooltips.py` & `mitzu-0.6.0rc4/mitzu/visualization/tooltips.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/transform_conv.py` & `mitzu-0.6.0rc4/mitzu/visualization/transform_conv.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/visualization/transform_retention.py` & `mitzu-0.6.0rc4/mitzu/visualization/transform_retention.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/.DS_Store` & `mitzu-0.6.0rc4/mitzu/webapp/.DS_Store`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/explore_page.css` & `mitzu-0.6.0rc4/mitzu/webapp/assets/explore_page.css`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/favicon.ico` & `mitzu-0.6.0rc4/mitzu/webapp/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/logo.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/logo.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/mitzu-logo-light.svg` & `mitzu-0.6.0rc4/mitzu/webapp/assets/mitzu-logo-light.svg`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/athena.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/athena.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/clickhouse.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/databricks.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/databricks.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/mysql.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/mysql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/pandas.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/pandas.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/postgresql.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/postgresql.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/redshift.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/redshift.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/snowflake.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/snowflake.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/sqlite.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/sqlite.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/assets/warehouse/trino.png` & `mitzu-0.6.0rc4/mitzu/webapp/assets/warehouse/trino.png`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/auth/authorizer.py` & `mitzu-0.6.0rc4/mitzu/webapp/auth/authorizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,24 +255,21 @@
                         self._config.redirect_cookie_name, MITZU_WEBAPP_URL
                     )
 
                     user_email = self._validate_foreign_token(id_token)
                     if not user_email:
                         raise Exception("Unauthorized (Invalid jwt token)")
 
-                    user_role = WM.Role.MEMBER
-                    token_identity = user_email
-                    if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
-                        user = self._config.user_service.get_user_by_email(user_email)
-                        if user is None:
-                            raise Exception(
-                                f"User tried to login without having a local user: {user_email}"
-                            )
-                        user_role = user.role
-                        token_identity = user.id
+                    user = self._config.user_service.get_user_by_email(user_email)
+                    if user is None:
+                        raise Exception(
+                            f"User tried to login without having a local user: {user_email}"
+                        )
+                    user_role = user.role
+                    token_identity = user.id
 
                     token = self._generate_new_token_for_identity(
                         token_identity, role=user_role
                     )
 
                     resp = self._redirect(redirect_url)
                     resp.set_cookie(self._config.token_cookie_name, token)
@@ -338,15 +335,15 @@
         claims = self._validate_token(auth_token)
         if claims is None or JWT_CLAIM_ROLE not in claims.keys():
             return None
 
         return WM.Role(claims[JWT_CLAIM_ROLE])
 
     def login_local_user(self, email: str, password: str) -> bool:
-        if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
+        if self._config.oauth:
             raise ValueError("Password login is not enabled, need to use SSO")
 
         user = self._config.user_service.get_user_by_email_and_password(email, password)
         if user is None:
             return False
 
         token = self._generate_new_token_for_identity(user.id, role=user.role)
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/auth/cognito.py` & `mitzu-0.6.0rc4/mitzu/webapp/auth/cognito.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/auth/decorator.py` & `mitzu-0.6.0rc4/mitzu/webapp/auth/decorator.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/auth/google.py` & `mitzu-0.6.0rc4/mitzu/webapp/auth/google.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/cache.py` & `mitzu-0.6.0rc4/mitzu/webapp/cache.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/caching_dataset_adapter.py` & `mitzu-0.6.0rc4/mitzu/webapp/caching_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/configs.py` & `mitzu-0.6.0rc4/mitzu/webapp/configs.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 
 
 # auth
 AUTH_BACKEND = os.getenv("AUTH_BACKEND")
 AUTH_ALLOWED_EMAIL_DOMAIN = os.getenv("AUTH_ALLOWED_EMAIL_DOMAIN")
 AUTH_JWT_SECRET = os.getenv("AUTH_JWT_SECRET", "mitzu-dev-env")
 AUTH_SESSION_TIMEOUT = os.getenv("AUTH_SESSION_TIMEOUT", 7 * 24 * 60 * 60)
-AUTH_SSO_ONLY_FOR_LOCAL_USERS = bool(os.getenv("AUTH_SSO_ONLY_FOR_LOCAL_USERS", False))
-AUTH_ROOT_PASSWORD = os.getenv("AUTH_ROOT_PASSWORD", "test")
+AUTH_ROOT_PASSWORD = os.getenv("AUTH_ROOT_PASSWORD", "testuser")
 AUTH_ROOT_USER_EMAIL = os.getenv("AUTH_ROOT_USER_EMAIL", "root@local")
 
 
 # cache
 CACHE_EXPIRATION = int(os.getenv("CACHE_EXPIRATION", "600"))
 CACHE_PREFIX = os.getenv("CACHE_PREFIX")
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/dependencies.py` & `mitzu-0.6.0rc4/mitzu/webapp/dependencies.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/helper.py` & `mitzu-0.6.0rc4/mitzu/webapp/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/model.py` & `mitzu-0.6.0rc4/mitzu/webapp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,11 +265,11 @@
 @dataclass
 class User:
     """
     Container class for describing a user
     """
 
     email: str
-    password_hash: str
-    password_salt: str
+    password_hash: Optional[str]
+    password_salt: Optional[str]
     id: str = field(default_factory=create_unique_id)
     role: Role = Role.MEMBER
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/offcanvas.py` & `mitzu-0.6.0rc4/mitzu/webapp/offcanvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,21 +127,14 @@
             dbc.Button(
                 [html.B(className="bi bi-person-circle me-1"), "Users"],
                 color=BUTTON_COLOR,
                 class_name=MENU_ITEM_CSS,
                 href=P.USERS_PATH,
                 id=USERS_BUTTON,
             ),
-            dbc.Button(
-                [html.B(className="bi bi-person-circle me-1"), "My Account"],
-                color=BUTTON_COLOR,
-                class_name=MENU_ITEM_CSS,
-                href=P.create_path(P.USERS_HOME_PATH, user_id="my-account"),
-                id=MY_ACCOUNT_BUTTON,
-            ),
             html.Hr(className="mb-3 d-none"),
             dbc.Button(
                 [html.B(className="bi bi-box-arrow-right me-1"), "Sign out"],
                 color="light",
                 class_name=MENU_ITEM_CSS,
                 href=P.SIGN_OUT_URL,
                 external_link=True,
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/connections/manage_connections_component.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/connections/manage_connections_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
 
 
 def create_delete_button(connection: Optional[M.Connection]) -> bc.Component:
     if connection is not None:
         return dbc.Button(
             [html.B(className="bi bi-x-circle"), " Delete connection"],
             id=CONNECTION_DELETE_BUTTON,
+            size="sm",
             color="danger",
         )
     else:
         return html.Div()
 
 
 def create_confirm_dialog():
@@ -296,14 +297,15 @@
             html.Div(
                 [
                     dbc.Button(
                         [html.B(className="bi bi-check-circle"), " Test connection"],
                         id=CONNECTION_TEST_BUTTON,
                         color="primary",
                         class_name="me-3",
+                        size="sm",
                     ),
                     create_delete_button(con),
                 ],
                 className="mb-3",
             ),
             dbc.Button(
                 [dbc.Spinner(size="sm"), " Loading..."],
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/connections_page.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/connections_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
                     dbc.Row(
                         dbc.Col(
                             dbc.Button(
                                 [
                                     html.B(className="bi bi-plus-circle"),
                                     " New Warehouse Connection",
                                 ],
+                                size="sm",
                                 color="primary",
                                 href=P.CONNECTIONS_CREATE_PATH,
                             ),
                             lg=3,
                             sm=12,
                         )
                     ),
@@ -103,14 +104,15 @@
                     ),
                     *[html.Div(d) for d in details],
                     html.Hr(),
                     html.Div(
                         [
                             dbc.Button(
                                 "Manage",
+                                size="sm",
                                 color="primary",
                                 href=P.create_path(
                                     P.CONNECTIONS_MANAGE_PATH,
                                     connection_id=connection.id,
                                 ),
                             ),
                         ],
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards/manage_dashboards_component.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards/manage_dashboards_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     return dbc.Offcanvas(
         children=[
             html.Hr(),
             dbc.Button(
                 [html.B(className="bi bi-plus-circle me-1"), "Explore projects"],
                 href=P.PROJECTS_PATH,
                 target="_blank",
-                size="small",
+                size="sm",
                 color="light",
                 class_name="w-100 mb-3",
             ),
             dmc.TextInput(
                 id=SAVED_METRICS_SEARCH,
                 placeholder="Search",
                 debounce=200,
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/dashboards.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/dashboards.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,14 +59,15 @@
                                             className="bi bi-plus-circle me-1",
                                         ),
                                         "Add Dashboard",
                                     ],
                                     color="primary",
                                     href=P.DASHBOARDS_CREATE_PATH,
                                     id=CREATE_NEW_DASHBOARD_BTN,
+                                    size="sm",
                                 ),
                                 width="auto",
                                 class_name="ms-auto",
                             ),
                         ]
                     ),
                     html.Hr(),
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/edit_user.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/edit_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 import dash_bootstrap_components as dbc
 import dash.development.base_component as bc
 import dash_mantine_components as dmc
 import mitzu.webapp.dependencies as DEPS
 import mitzu.webapp.navbar as NB
 import mitzu.webapp.pages.paths as P
 import mitzu.webapp.model as WM
-import mitzu.webapp.configs as configs
 from mitzu.webapp.helper import create_form_property_input
 from mitzu.webapp.auth.decorator import (
     restricted_layout,
     restricted,
     restricted_for_admin,
 )
 from mitzu.webapp.webapp import MITZU_LOCATION
@@ -29,15 +28,15 @@
 INDEX_TYPE = "user_property"
 PROP_EMAIL = "email"
 PROP_ROLE = "role"
 PROP_PASSWORD = "password"
 PROP_CONFIRM_PASSWORD = "confirm_password"
 
 
-USER_SAVE_BUTTON = "user_save_button"
+USER_CREATE_BUTTON = "user_create_button"
 USER_CLOSE_BUTTON = "user_close_button"
 NOT_FOUND_USER_CLOSE_BUTTON = "not_found_user_close_button"
 USER_DELETE_BUTTON = "user_delete_button"
 USER_CHANGE_PASSWORD_BUTTON = "user_change_password_button"
 USER_CHANGE_ROLE_BUTTON = "user_change_role_button"
 
 SAVE_RESPONSE_CONTAINER = "user_save_response_container"
@@ -47,32 +46,31 @@
 
 
 @restricted_layout
 def layout(user_id: str, **query_params) -> bc.Component:
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
+    is_sso = deps.authorizer._config.oauth is not None
+
     logged_in_user_id = deps.authorizer.get_current_user_id()
     if logged_in_user_id is None:
         raise ValueError("Cannot determine logged in user id")
     logged_in_user = user_service.get_user_by_id(logged_in_user_id)
     if logged_in_user is None:
         raise ValueError("Logged in user is not found")
 
     is_admin = deps.authorizer.get_current_user_role(flask.request) == WM.Role.ADMIN
-    show_password_fields = user_id == "new"
+    show_password_fields = user_id == "new" and not is_sso
     show_change_password = False
-    show_delete_button = user_id != "new"
-    if user_id is not None and user_id != "new":
-        if user_id == "my-account":
-            user_id = logged_in_user.id
 
+    if user_id is not None and user_id != "new":
         show_change_password = (
             user_id == logged_in_user.id or logged_in_user.role == WM.Role.ADMIN
-        )
+        ) and not is_sso
         user = user_service.get_user_by_id(user_id)
         show_delete_button = (
             logged_in_user.role == WM.Role.ADMIN
             and user is not None
             and user.id != logged_in_user.id
         )
     else:
@@ -86,14 +84,15 @@
                     [
                         html.H4("Users not found"),
                         html.Hr(),
                         dbc.Button(
                             [html.B(className="bi bi-x"), " Close"],
                             color="secondary",
                             class_name="me-3",
+                            size="sm",
                             id=NOT_FOUND_USER_CLOSE_BUTTON,
                             href=P.USERS_PATH,
                         ),
                     ]
                 ),
             ]
         )
@@ -120,94 +119,102 @@
                         icon_cls="bi bi-person-fill",
                         component_type=dmc.Select,
                         data=[
                             {"label": v.name.lower(), "value": v.value}
                             for v in WM.Role.all_values()
                         ],
                         required=True,
+                        read_only=not (
+                            logged_in_user.role == WM.Role.ADMIN
+                            and (user is not None or user_id == "new")
+                        ),
                         value=user.role if user is not None else WM.Role.MEMBER.value,
-                        read_only=user_service.is_root_user(user_id),
                     ),
                     create_form_property_input(
                         index_type=INDEX_TYPE,
                         property=PROP_PASSWORD,
                         icon_cls="bi bi-key",
                         type="password",
                         required=True,
                         value="",
-                        hidden=configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS,
                     )
                     if show_password_fields
                     else None,
                     create_form_property_input(
                         index_type=INDEX_TYPE,
                         property=PROP_CONFIRM_PASSWORD,
                         icon_cls="bi bi-key",
                         type="password",
                         required=True,
                         value="",
-                        hidden=configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS,
                     )
                     if show_password_fields
                     else None,
                 ]
                 + (
                     [
                         html.Hr(),
                         html.Div(
                             [
                                 dbc.Button(
                                     [
                                         html.B(className="bi bi-check-circle me-1"),
-                                        "Save",
+                                        "Create user",
                                     ],
                                     color="success",
                                     class_name="me-3",
-                                    id=USER_SAVE_BUTTON,
+                                    size="sm",
+                                    id=USER_CREATE_BUTTON,
                                 ),
-                                dbc.Button(
-                                    [html.B(className="bi bi-x me-1"), "Delete"],
-                                    color="danger",
-                                    class_name="me-3",
-                                    id=USER_DELETE_BUTTON,
-                                    external_link=True,
-                                    href=P.create_path(P.USERS_PATH),
-                                )
-                                if show_delete_button
-                                else None,
                             ],
                             className="mb-3",
                         ),
                         html.Div(
                             children=[], id=SAVE_RESPONSE_CONTAINER, className="lead"
                         ),
-                        html.Div(
-                            children=[], id=DELETE_RESPONSE_CONTAINER, className="lead"
-                        ),
                     ]
-                    if user is None
+                    if user_id == "new"
                     else (
                         [
                             html.Hr(),
                             html.Div(
                                 [
                                     dbc.Button(
-                                        ["Update"],
+                                        [
+                                            html.B(className="bi bi-check-circle me-1"),
+                                            "Update",
+                                        ],
                                         color="primary",
                                         class_name="me-3",
                                         id=USER_CHANGE_ROLE_BUTTON,
-                                        disabled=user_service.is_root_user(user_id),
+                                        size="sm",
                                     )
                                     if user is not None
                                     else None,
+                                    dbc.Button(
+                                        [html.B(className="bi bi-x me-1"), "Delete"],
+                                        color="danger",
+                                        class_name="me-3",
+                                        id=USER_DELETE_BUTTON,
+                                        external_link=True,
+                                        href=P.create_path(P.USERS_PATH),
+                                        size="sm",
+                                    )
+                                    if show_delete_button
+                                    else None,
                                 ],
                                 className="mb-3",
                             ),
                             html.Div(
                                 children=[],
+                                id=DELETE_RESPONSE_CONTAINER,
+                                className="lead",
+                            ),
+                            html.Div(
+                                children=[],
                                 id=CHANGE_ROLE_RESPONSE_CONTAINER,
                                 className="lead",
                             ),
                         ]
                         if is_admin
                         else []
                     )
@@ -217,25 +224,23 @@
                     html.Hr(),
                     dbc.Button(
                         [html.B(className="bi bi-x me-1"), "Close"],
                         color="secondary",
                         class_name="me-3",
                         id=USER_CLOSE_BUTTON,
                         href=P.USERS_PATH,
+                        size="sm",
                     ),
                 ],
             ),
         ]
     )
 
 
 def change_password_form():
-    if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
-        return []
-
     return [
         html.Hr(),
         create_form_property_input(
             index_type=INDEX_TYPE,
             property=PROP_PASSWORD,
             icon_cls="bi bi-key",
             type="password",
@@ -251,26 +256,27 @@
             value="",
         ),
         html.Hr(),
         dbc.Button(
             ["Change password"],
             color="primary",
             className="mb-3",
+            size="sm",
             id=USER_CHANGE_PASSWORD_BUTTON,
         ),
         html.Div(children=[], id=CHANGE_PASSWORD_RESPONSE_CONTAINER, className="lead"),
     ]
 
 
 @callback(
     output={
         SAVE_RESPONSE_CONTAINER: Output(SAVE_RESPONSE_CONTAINER, "children"),
     },
     inputs={
-        "n_clicks": Input(USER_SAVE_BUTTON, "n_clicks"),
+        "n_clicks": Input(USER_CREATE_BUTTON, "n_clicks"),
     },
     state={
         "email": State({"type": INDEX_TYPE, "index": PROP_EMAIL}, "value"),
         "role": State({"type": INDEX_TYPE, "index": PROP_ROLE}, "value"),
         "password": State({"type": INDEX_TYPE, "index": PROP_PASSWORD}, "value"),
         "confirm_password": State(
             {"type": INDEX_TYPE, "index": PROP_CONFIRM_PASSWORD}, "value"
@@ -279,20 +285,18 @@
     prevent_initial_call=True,
 )
 @restricted_for_admin
 def create_new_user(n_clicks: int, email="", role="", password="", confirm_password=""):
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
-    if configs.AUTH_SSO_ONLY_FOR_LOCAL_USERS:
-        # new user need a password other than empty string
-        from uuid import uuid4
-
-        password = str(uuid4())
-        confirm_password = password
+    if deps.authorizer._config.oauth:
+        # SSO users don't have passwords
+        password = None
+        confirm_password = None
 
     try:
         user_service.new_user(email, password, confirm_password, role=WM.Role(role))
         return {
             SAVE_RESPONSE_CONTAINER: "User created!",
         }
     except Exception as e:
@@ -331,20 +335,14 @@
         logged_in_user_id = deps.authorizer.get_current_user_id()
         logged_in_user = user_service.get_user_by_id(logged_in_user_id)
 
         user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
         if logged_in_user is None:
             raise Exception("User is not signed in")
 
-        if user_id == "my-account":
-            user_id = logged_in_user_id
-
-        if logged_in_user is None:
-            raise Exception("User is not signed in")
-
         if logged_in_user.role != WM.Role.ADMIN and logged_in_user.id != user_id:
             raise Exception("User is not authorized to change this password")
 
         user_service.update_password(user_id, password, confirm_password)
         return {CHANGE_PASSWORD_RESPONSE_CONTAINER: "Password changed"}
     except Exception as e:
         return {
@@ -376,17 +374,14 @@
     try:
         logged_in_user_id = deps.authorizer.get_current_user_id()
 
         user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
         if logged_in_user_id is None:
             raise Exception("User is not signed in")
 
-        if user_id == "my-account":
-            user_id = logged_in_user_id
-
         user_service.update_role(user_id, WM.Role(role))
         return {CHANGE_ROLE_RESPONSE_CONTAINER: "Role updated"}
     except Exception as e:
         return {
             CHANGE_ROLE_RESPONSE_CONTAINER: str(e),
         }
 
@@ -406,17 +401,14 @@
 @restricted_for_admin
 def delete_user(n_clicks: int, pathname: str = ""):
     user_id = P.get_path_value(P.USERS_HOME_PATH, pathname, P.USER_PATH_PART)
     deps = cast(DEPS.Dependencies, flask.current_app.config.get(DEPS.CONFIG_KEY))
     user_service = deps.user_service
 
     try:
-        if user_id == "my-account":
-            raise Exception("Own account cannot be deleted")
-
         user_service.delete_user(user_id)
         return {
             DELETE_RESPONSE_CONTAINER: "User deleted",
         }
 
     except Exception as e:
         return {DELETE_RESPONSE_CONTAINER: str(e)}
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/complex_segment_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/complex_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/dates_selector_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/dates_selector_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/event_segment_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/event_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/explore_page.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/explore_page.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/graph_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/graph_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_config_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_config_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_segments_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_segments_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/metric_type_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/metric_type_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/simple_segment_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/simple_segment_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore/toolbar_handler.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore/toolbar_handler.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/explore_project.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/explore_project.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/home.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/home.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                                 [
                                     html.B(className="bi bi-play-circle me-1"),
                                     "Start exploring",
                                 ],
                                 color="secondary",
                                 class_name="mb-3 w-25",
                                 href=P.PROJECTS_PATH,
+                                size="sm",
                             ),
                         ],
                         justify="center",
                     ),
                     html.Hr(),
                     dbc.Row(
                         [],
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/login.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
                     [
                         "Login",
                     ],
                     color="secondary",
                     class_name="mb-3 w-25",
                     href=P.REDIRECT_TO_LOGIN_URL,
                     external_link=True,
+                    size="sm",
                 ),
             ],
             justify="center",
         ),
     ]
 
 
@@ -107,14 +108,15 @@
                     ],
                     color="secondary",
                     class_name="mb-3 w-25",
                     external_link=True,
                     type="submit",
                     name="login",
                     id=BUTTON_LOGIN,
+                    size="sm",
                 ),
             ],
             justify="center",
         ),
         dbc.Row(
             [
                 dbc.Col(
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_connection.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,29 +61,32 @@
                         [
                             dbc.Button(
                                 [html.B(className="bi bi-x"), " Close"],
                                 color="secondary",
                                 class_name="me-3",
                                 id=CONNECTION_CLOSE_BUTTON,
                                 href=P.CONNECTIONS_PATH,
+                                size="sm",
                             ),
                             dbc.Button(
                                 [html.B(className="bi bi-check-circle"), " Save"],
                                 color="success",
                                 class_name="me-3",
                                 id=CONNECTION_SAVE_BUTTON,
+                                size="sm",
                             ),
                             dbc.Button(
                                 [
                                     html.B(className="bi bi-plus-circle"),
                                     " Save and add project",
                                 ],
                                 color="primary",
                                 class_name="me-3",
                                 id=CONNECTION_SAVE_AND_ADD_PROJECT_BUTTON,
+                                size="sm",
                             ),
                         ],
                         className="mb-3",
                     ),
                     html.Div(children=[], id=SAVE_RESPONSE_CONTAINER),
                 ],
                 class_name="mb-3",
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_dashboard.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_dashboard.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_event_defs.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_event_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,27 +145,29 @@
                                     [
                                         html.B(className="bi bi-x-circle me-1"),
                                         "Cancel",
                                     ],
                                     id=DISCOVER_CANCEL_BUTTON,
                                     color="light",
                                     class_name="d-inline-block mb-3",
+                                    size="sm",
                                 ),
                                 width="auto",
                                 class_name="invisible",
                             ),
                             dbc.Col(
                                 dbc.Button(
                                     [
                                         html.B(className="bi bi-search me-1"),
                                         "Discover project",
                                     ],
                                     id=DISCOVER_PROJECT_BUTTON,
                                     disabled=project_id is None,
                                     class_name="d-inline-block mb-3 me-3",
+                                    size="sm",
                                 ),
                                 width="auto",
                             ),
                         ],
                     ),
                     html.Hr(),
                     html.Div(
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_project.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 def create_delete_button(project: Optional[M.Project]) -> bc.Component:
     if project is not None:
         return dbc.Button(
             [html.B(className="bi bi-x-circle me-1"), "Delete Project"],
             id=DELETE_BUTTON,
             color="danger",
             class_name="d-inline-block me-3 mb-1",
+            size="sm",
         )
     else:
         return html.Div()
 
 
 def create_confirm_dialog(project: Optional[M.Project]):
     if project is None:
@@ -165,24 +166,26 @@
                     MPC.create_project_settings(project, dependencies, **query_params),
                     html.Hr(),
                     dbc.Button(
                         [html.B(className="bi bi-check-circle"), " Save"],
                         color="success",
                         id=SAVE_BUTTON,
                         class_name="d-inline-block me-3 mb-1",
+                        size="sm",
                     ),
                     dbc.Button(
                         [
                             html.B(className="bi bi-search me-1"),
                             (
                                 "Discover Project"
                                 if project_id is not None
                                 else "Discover Projects"
                             ),
                         ],
+                        size="sm",
                         color="primary",
                         class_name="d-inline-block me-3 mb-1",
                         href=(
                             P.create_path(
                                 P.EVENTS_AND_PROPERTIES_PROJECT_PATH,
                                 project_id=project_id,
                             )
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/manage_saved_metrics.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/manage_saved_metrics.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/paths.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/paths.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/projects/event_tables_config.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/projects/event_tables_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,40 +363,47 @@
             dbc.Row(
                 [
                     dbc.Col(
                         dbc.Button(
                             [html.B(className="bi bi-plus-circle me-1"), "Add tables"],
                             color="primary",
                             id=ADD_TABLES_BUTTON,
+                            size="sm",
                         ),
                         width="auto",
                         class_name="mb-3",
                     ),
                     dbc.Col(
                         dbc.Button(
                             [html.B(className="bi bi-gear me-1"), "Configure"],
                             color="secondary",
                             disabled=True,
                             id=CONFIGURE_TABLES_BUTTON,
+                            size="sm",
                         ),
                         class_name="mb-3",
                         width="auto",
                     ),
                     dbc.Col(
                         dbc.Button(
                             [html.B(className="bi bi-x-circle me-1"), "Remove"],
                             color="danger",
                             disabled=True,
                             id=REMOVE_TABLES_BUTTON,
+                            size="sm",
                         ),
                         class_name="mb-3",
                         width="auto",
                     ),
                     dbc.Col(
-                        dbc.Input(id=TBL_SEARCH_INPUT, placeholder="Search tables"),
+                        dbc.Input(
+                            id=TBL_SEARCH_INPUT,
+                            placeholder="Search tables",
+                            size="sm",
+                        ),
                         class_name="ms-auto mb-3",
                         width="3",
                     ),
                 ],
                 class_name="me-auto",
             ),
             table,
@@ -404,14 +411,15 @@
             dbc.Button(
                 [
                     html.B(className="bi bi-check-circle me-1"),
                     "Validate",
                 ],
                 id=EDT_VALIDATE_BUTTON,
                 color="primary",
+                size="sm",
                 className="me-3 d-inline-block shadow-sm mb-3",
             ),
             html.Div(
                 children=[],
                 id=TBL_PROGRESS_INFO,
                 className="lead d-inline-block mb-3",
             ),
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/projects/helper.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/projects/helper.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/projects/manage_project_component.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/projects/manage_project_component.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/projects_page.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/projects_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
                             dbc.Col(
                                 dbc.Button(
                                     children=[
                                         html.I(className="bi bi-plus-circle me-1"),
                                         "Add project",
                                     ],
                                     href=P.PROJECTS_CREATE_PATH,
+                                    size="sm",
                                 ),
                                 width="auto",
                                 class_name="ms-auto",
                             ),
                         ]
                     ),
                     html.Hr(),
@@ -117,20 +118,22 @@
                     html.P(project.description),
                     html.Div(
                         [
                             dbc.Button(
                                 "Explore",
                                 color="primary",
                                 class_name="me-3",
+                                size="sm",
                                 href=P.create_path(
                                     P.PROJECTS_EXPLORE_PATH, project_id=project_id
                                 ),
                             ),
                             dbc.Button(
                                 "Manage",
+                                size="sm",
                                 color="secondary",
                                 href=P.create_path(
                                     P.PROJECTS_MANAGE_PATH, project_id=project_id
                                 ),
                             ),
                         ],
                     ),
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/pages/users.py` & `mitzu-0.6.0rc4/mitzu/webapp/pages/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
                     [
                         html.Hr(),
                         dbc.Button(
                             [html.I(className="bi bi-plus-circle me-1"), "Add user"],
                             color="primary",
                             href=P.create_path(P.USERS_HOME_PATH, user_id="new"),
                             id=ADD_USER_BUTTON,
+                            size="sm",
                         ),
                     ]
                     if is_admin
                     else []
                 )
             ),
         ]
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/service/events_service.py` & `mitzu-0.6.0rc4/mitzu/webapp/service/events_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/service/navbar_service.py` & `mitzu-0.6.0rc4/mitzu/webapp/service/navbar_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/service/secret_service.py` & `mitzu-0.6.0rc4/mitzu/webapp/service/secret_service.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/storage.py` & `mitzu-0.6.0rc4/mitzu/webapp/storage.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/storage_model.py` & `mitzu-0.6.0rc4/mitzu/webapp/storage_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
 
 
 class UserStorageRecord(Base):
     __tablename__ = "users"
 
     user_id = SA.Column(SA.String, primary_key=True)
     email = SA.Column(SA.String)
-    password_hash = SA.Column(SA.String)
-    password_salt = SA.Column(SA.String)
+    password_hash = SA.Column(SA.String, nullable=True)
+    password_salt = SA.Column(SA.String, nullable=True)
     role = SA.Column(SA.String)
 
     def update(self, user: WM.User):
         self.email = user.email
         self.password_hash = user.password_hash
         self.password_salt = user.password_salt
         self.role = user.role.value
```

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/toast.py` & `mitzu-0.6.0rc4/mitzu/webapp/toast.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/mitzu/webapp/webapp.py` & `mitzu-0.6.0rc4/mitzu/webapp/webapp.py`

 * *Files identical despite different names*

### Comparing `mitzu-0.6.0rc3/pyproject.toml` & `mitzu-0.6.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mitzu"
-version = "0.6.0-rc.3"
+version = "0.6.0-rc.4"
 description = "Product analytics over your data warehouse"
 authors = ["Istvan Meszaros <istvan.meszaros.88@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://mitzu.io"
 repository = "https://github.com/mitzu-io/mitzu"
 documentation = "https://mitzu.io/documentation/"
```

### Comparing `mitzu-0.6.0rc3/PKG-INFO` & `mitzu-0.6.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitzu
-Version: 0.6.0rc3
+Version: 0.6.0rc4
 Summary: Product analytics over your data warehouse
 Home-page: https://mitzu.io
 License: MIT
 Author: Istvan Meszaros
 Author-email: istvan.meszaros.88@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

