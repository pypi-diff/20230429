# Comparing `tmp/fastapi-users-9.3.1.tar.gz` & `tmp/fastapi-users-9.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-users-9.3.1.tar", last modified: Thu Apr 21 09:26:40 2022, max compression
+gzip compressed data, was "fastapi-users-9.3.2.tar", last modified: Thu May  5 10:00:35 2022, max compression
```

## Comparing `fastapi-users-9.3.1.tar` & `fastapi-users-9.3.2.tar`

### file list

```diff
@@ -1,169 +1,170 @@
--rw-r--r--   0        0        0    13456 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.all-contributorsrc
--rw-r--r--   0        0        0      230 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.editorconfig
--rw-r--r--   0        0        0       94 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      647 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      243 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      171 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0      724 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/stale.yml
--rw-r--r--   0        0        0     1584 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      676 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1257 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/.gitignore
--rw-r--r--   0        0        0     1072 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/LICENSE
--rw-r--r--   0        0        0      943 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/Makefile
--rw-r--r--   0        0        0    22911 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/README.md
--rw-r--r--   0        0        0     1176 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/backend.md
--rw-r--r--   0        0        0     2836 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/index.md
--rw-r--r--   0        0        0     3001 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/strategies/database.md
--rw-r--r--   0        0        0     2379 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/strategies/jwt.md
--rw-r--r--   0        0        0     1202 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/strategies/redis.md
--rw-r--r--   0        0        0     1812 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/transports/bearer.md
--rw-r--r--   0        0        0     1510 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/authentication/transports/cookie.md
--rw-r--r--   0        0        0     1461 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/databases/mongodb.md
--rw-r--r--   0        0        0     1143 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/databases/ormar.md
--rw-r--r--   0        0        0     2043 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/databases/sqlalchemy.md
--rw-r--r--   0        0        0     2313 2022-04-21 09:25:45.004834 fastapi-users-9.3.1/docs/configuration/databases/tortoise.md
--rw-r--r--   0        0        0     2675 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/full-example.md
--rw-r--r--   0        0        0     2156 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/models.md
--rw-r--r--   0        0        0     5971 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/oauth.md
--rw-r--r--   0        0        0     3674 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/overview.md
--rw-r--r--   0        0        0     2485 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/password-hash.md
--rw-r--r--   0        0        0      955 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/routers/auth.md
--rw-r--r--   0        0        0     1951 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/routers/index.md
--rw-r--r--   0        0        0      544 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/routers/register.md
--rw-r--r--   0        0        0      648 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/routers/reset.md
--rw-r--r--   0        0        0      873 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/routers/users.md
--rw-r--r--   0        0        0      684 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/routers/verify.md
--rw-r--r--   0        0        0     7304 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/configuration/user-manager.md
--rw-r--r--   0        0        0     2578 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/cookbook/create-user-programmatically.md
--rw-r--r--   0        0        0     1648 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/favicon.png
--rw-r--r--   0        0        0       19 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/index.md
--rw-r--r--   0        0        0      522 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/installation.md
--rw-r--r--   0        0        0     5701 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/08_to_1x.md
--rw-r--r--   0        0        0      810 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/1x_to_2x.md
--rw-r--r--   0        0        0      853 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/2x_to_3x.md
--rw-r--r--   0        0        0      371 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/3x_to_4x.md
--rw-r--r--   0        0        0      377 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/4x_to_5x.md
--rw-r--r--   0        0        0      961 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/6x_to_7x.md
--rw-r--r--   0        0        0     2970 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/7x_to_8x.md
--rw-r--r--   0        0        0     3585 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/migration/8x_to_9x.md
--rw-r--r--   0        0        0     1055 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/cookbook_create_user_programmatically.py
--rw-r--r--   0        0        0      378 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_mongodb.py
--rw-r--r--   0        0        0      638 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_mongodb_access_tokens.py
--rw-r--r--   0        0        0      534 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_ormar.py
--rw-r--r--   0        0        0     1042 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_sqlalchemy.py
--rw-r--r--   0        0        0     1421 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_sqlalchemy_access_tokens.py
--rw-r--r--   0        0        0     1246 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_sqlalchemy_oauth.py
--rw-r--r--   0        0        0      417 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_tortoise_access_tokens_adapter.py
--rw-r--r--   0        0        0      917 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_tortoise_access_tokens_model.py
--rw-r--r--   0        0        0      203 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_tortoise_adapter.py
--rw-r--r--   0        0        0      460 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_tortoise_model.py
--rw-r--r--   0        0        0      231 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_tortoise_oauth_adapter.py
--rw-r--r--   0        0        0      687 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/db_tortoise_oauth_model.py
--rw-r--r--   0        0        0     1002 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/src/user_manager.py
--rw-r--r--   0        0        0     4848 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/usage/current-user.md
--rw-r--r--   0        0        0    10893 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/usage/flow.md
--rw-r--r--   0        0        0    10364 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/docs/usage/routes.md
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/app/__init__.py
--rw-r--r--   0        0        0      992 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/app/app.py
--rw-r--r--   0        0        0      391 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/app/db.py
--rw-r--r--   0        0        0      257 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/app/models.py
--rw-r--r--   0        0        0     1894 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/app/users.py
--rw-r--r--   0        0        0      119 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/main.py
--rw-r--r--   0        0        0       55 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb-oauth/requirements.txt
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/app/__init__.py
--rw-r--r--   0        0        0      801 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/app/app.py
--rw-r--r--   0        0        0      391 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/app/db.py
--rw-r--r--   0        0        0      227 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/app/models.py
--rw-r--r--   0        0        0     1704 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/app/users.py
--rw-r--r--   0        0        0      119 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/main.py
--rw-r--r--   0        0        0       49 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/mongodb/requirements.txt
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/__init__.py
--rw-r--r--   0        0        0     1178 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/app.py
--rw-r--r--   0        0        0     1249 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/db.py
--rw-r--r--   0        0        0      257 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/models.py
--rw-r--r--   0        0        0     1906 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/users.py
--rw-r--r--   0        0        0      108 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/main.py
--rw-r--r--   0        0        0       69 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy-oauth/requirements.txt
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.008834 fastapi-users-9.3.1/examples/sqlalchemy/app/__init__.py
--rw-r--r--   0        0        0      987 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/sqlalchemy/app/app.py
--rw-r--r--   0        0        0     1045 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/sqlalchemy/app/db.py
--rw-r--r--   0        0        0      227 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/sqlalchemy/app/models.py
--rw-r--r--   0        0        0     1710 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/sqlalchemy/app/users.py
--rw-r--r--   0        0        0      108 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/sqlalchemy/main.py
--rw-r--r--   0        0        0       63 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/sqlalchemy/requirements.txt
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/app/__init__.py
--rw-r--r--   0        0        0     1203 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/app/app.py
--rw-r--r--   0        0        0      234 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/app/db.py
--rw-r--r--   0        0        0      687 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/app/models.py
--rw-r--r--   0        0        0     1896 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/app/users.py
--rw-r--r--   0        0        0      119 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/main.py
--rw-r--r--   0        0        0       60 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise-oauth/requirements.txt
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/app/__init__.py
--rw-r--r--   0        0        0     1012 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/app/app.py
--rw-r--r--   0        0        0      206 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/app/db.py
--rw-r--r--   0        0        0      460 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/app/models.py
--rw-r--r--   0        0        0     1706 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/app/users.py
--rw-r--r--   0        0        0      119 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/main.py
--rw-r--r--   0        0        0       54 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/examples/tortoise/requirements.txt
--rw-r--r--   0        0        0      411 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/__init__.py
--rw-r--r--   0        0        0      632 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/__init__.py
--rw-r--r--   0        0        0     9172 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/authenticator.py
--rw-r--r--   0        0        0     1791 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/backend.py
--rw-r--r--   0        0        0      632 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/__init__.py
--rw-r--r--   0        0        0      776 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/base.py
--rw-r--r--   0        0        0      318 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/db/__init__.py
--rw-r--r--   0        0        0     1108 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/db/adapter.py
--rw-r--r--   0        0        0      417 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/db/models.py
--rw-r--r--   0        0        0     1939 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/db/strategy.py
--rw-r--r--   0        0        0     2212 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/jwt.py
--rw-r--r--   0        0        0     1298 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/strategy/redis.py
--rw-r--r--   0        0        0      379 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/transport/__init__.py
--rw-r--r--   0        0        0     1058 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/transport/base.py
--rw-r--r--   0        0        0     1756 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/transport/bearer.py
--rw-r--r--   0        0        0     2190 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/authentication/transport/cookie.py
--rw-r--r--   0        0        0     1467 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/db/__init__.py
--rw-r--r--   0        0        0     1336 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/db/base.py
--rw-r--r--   0        0        0     4767 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/fastapi_users.py
--rw-r--r--   0        0        0     1028 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/jwt.py
--rw-r--r--   0        0        0    19118 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/manager.py
--rw-r--r--   0        0        0     1900 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/models.py
--rw-r--r--   0        0        0       97 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/openapi.py
--rw-r--r--   0        0        0     1220 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/password.py
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/py.typed
--rw-r--r--   0        0        0      706 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/__init__.py
--rw-r--r--   0        0        0     3425 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/auth.py
--rw-r--r--   0        0        0      878 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/common.py
--rw-r--r--   0        0        0     4755 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/oauth.py
--rw-r--r--   0        0        0     2802 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/register.py
--rw-r--r--   0        0        0     3174 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/reset.py
--rw-r--r--   0        0        0     8277 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/users.py
--rw-r--r--   0        0        0     2918 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/router/verify.py
--rw-r--r--   0        0        0      333 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/fastapi_users/types.py
--rw-r--r--   0        0        0     8777 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/logo.svg
--rw-r--r--   0        0        0    20084 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/logo_github.png
--rw-r--r--   0        0        0     2911 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/mkdocs.yml
--rw-r--r--   0        0        0     2830 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/pyproject.toml
--rw-r--r--   0        0        0      285 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/setup.cfg
--rw-r--r--   0        0        0      112 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/test_build.py
--rw-r--r--   0        0        0        0 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/__init__.py
--rw-r--r--   0        0        0    14482 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/conftest.py
--rw-r--r--   0        0        0     4960 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_authenticator.py
--rw-r--r--   0        0        0     1954 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_backend.py
--rw-r--r--   0        0        0     3917 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_strategy_db.py
--rw-r--r--   0        0        0     6293 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_strategy_jwt.py
--rw-r--r--   0        0        0     3264 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_strategy_redis.py
--rw-r--r--   0        0        0     1534 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_transport_bearer.py
--rw-r--r--   0        0        0     2953 2022-04-21 09:25:45.012834 fastapi-users-9.3.1/tests/test_authentication_transport_cookie.py
--rw-r--r--   0        0        0      794 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_db_base.py
--rw-r--r--   0        0        0    18193 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_fastapi_users.py
--rw-r--r--   0        0        0      393 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_jwt.py
--rw-r--r--   0        0        0    20441 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_manager.py
--rw-r--r--   0        0        0     4015 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_openapi.py
--rw-r--r--   0        0        0     7469 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_router_auth.py
--rw-r--r--   0        0        0     7378 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_router_oauth.py
--rw-r--r--   0        0        0     4480 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_router_register.py
--rw-r--r--   0        0        0     6233 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_router_reset.py
--rw-r--r--   0        0        0    32911 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_router_users.py
--rw-r--r--   0        0        0     6647 2022-04-21 09:25:45.016834 fastapi-users-9.3.1/tests/test_router_verify.py
--rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 fastapi-users-9.3.1/setup.py
--rw-r--r--   0        0        0    25776 1970-01-01 00:00:00.000000 fastapi-users-9.3.1/PKG-INFO
+-rw-r--r--   0        0        0    13948 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.all-contributorsrc
+-rw-r--r--   0        0        0      230 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.editorconfig
+-rw-r--r--   0        0        0       94 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      647 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      243 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      171 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      724 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/stale.yml
+-rw-r--r--   0        0        0     1584 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1086 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1257 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/.gitignore
+-rw-r--r--   0        0        0     1072 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/LICENSE
+-rw-r--r--   0        0        0      943 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/Makefile
+-rw-r--r--   0        0        0    23768 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/README.md
+-rw-r--r--   0        0        0      196 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs-overrides/main.html
+-rw-r--r--   0        0        0     1176 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/backend.md
+-rw-r--r--   0        0        0     2836 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/index.md
+-rw-r--r--   0        0        0     2953 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/strategies/database.md
+-rw-r--r--   0        0        0     2379 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/strategies/jwt.md
+-rw-r--r--   0        0        0     1202 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/strategies/redis.md
+-rw-r--r--   0        0        0     1812 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/transports/bearer.md
+-rw-r--r--   0        0        0     1510 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/authentication/transports/cookie.md
+-rw-r--r--   0        0        0     1461 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/databases/mongodb.md
+-rw-r--r--   0        0        0     1143 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/databases/ormar.md
+-rw-r--r--   0        0        0     2043 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/databases/sqlalchemy.md
+-rw-r--r--   0        0        0     2313 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/databases/tortoise.md
+-rw-r--r--   0        0        0     2228 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/full-example.md
+-rw-r--r--   0        0        0     2156 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/models.md
+-rw-r--r--   0        0        0     5524 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/oauth.md
+-rw-r--r--   0        0        0     3674 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/overview.md
+-rw-r--r--   0        0        0     2485 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/password-hash.md
+-rw-r--r--   0        0        0      955 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/routers/auth.md
+-rw-r--r--   0        0        0     1951 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/routers/index.md
+-rw-r--r--   0        0        0      544 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/routers/register.md
+-rw-r--r--   0        0        0      648 2022-05-05 09:59:42.353584 fastapi-users-9.3.2/docs/configuration/routers/reset.md
+-rw-r--r--   0        0        0      873 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/configuration/routers/users.md
+-rw-r--r--   0        0        0      684 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/configuration/routers/verify.md
+-rw-r--r--   0        0        0     7304 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/configuration/user-manager.md
+-rw-r--r--   0        0        0     2578 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/cookbook/create-user-programmatically.md
+-rw-r--r--   0        0        0     1648 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/favicon.png
+-rw-r--r--   0        0        0       19 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/index.md
+-rw-r--r--   0        0        0      522 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/installation.md
+-rw-r--r--   0        0        0     5701 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/08_to_1x.md
+-rw-r--r--   0        0        0      810 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/1x_to_2x.md
+-rw-r--r--   0        0        0      853 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/2x_to_3x.md
+-rw-r--r--   0        0        0      371 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/3x_to_4x.md
+-rw-r--r--   0        0        0      377 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/4x_to_5x.md
+-rw-r--r--   0        0        0      961 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/6x_to_7x.md
+-rw-r--r--   0        0        0     2970 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/7x_to_8x.md
+-rw-r--r--   0        0        0     3585 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/migration/8x_to_9x.md
+-rw-r--r--   0        0        0     1055 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/cookbook_create_user_programmatically.py
+-rw-r--r--   0        0        0      378 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_mongodb.py
+-rw-r--r--   0        0        0      638 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_mongodb_access_tokens.py
+-rw-r--r--   0        0        0      534 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_ormar.py
+-rw-r--r--   0        0        0     1042 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_sqlalchemy.py
+-rw-r--r--   0        0        0     1421 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_sqlalchemy_access_tokens.py
+-rw-r--r--   0        0        0     1246 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_sqlalchemy_oauth.py
+-rw-r--r--   0        0        0      417 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_tortoise_access_tokens_adapter.py
+-rw-r--r--   0        0        0      917 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_tortoise_access_tokens_model.py
+-rw-r--r--   0        0        0      203 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_tortoise_adapter.py
+-rw-r--r--   0        0        0      460 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_tortoise_model.py
+-rw-r--r--   0        0        0      231 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_tortoise_oauth_adapter.py
+-rw-r--r--   0        0        0      687 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/db_tortoise_oauth_model.py
+-rw-r--r--   0        0        0     1002 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/src/user_manager.py
+-rw-r--r--   0        0        0     4848 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/usage/current-user.md
+-rw-r--r--   0        0        0    10893 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/usage/flow.md
+-rw-r--r--   0        0        0    10364 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/docs/usage/routes.md
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/app/__init__.py
+-rw-r--r--   0        0        0      992 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/app/app.py
+-rw-r--r--   0        0        0      391 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/app/db.py
+-rw-r--r--   0        0        0      257 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/app/models.py
+-rw-r--r--   0        0        0     1894 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/app/users.py
+-rw-r--r--   0        0        0      119 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/main.py
+-rw-r--r--   0        0        0       55 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb-oauth/requirements.txt
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/app/__init__.py
+-rw-r--r--   0        0        0      801 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/app/app.py
+-rw-r--r--   0        0        0      391 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/app/db.py
+-rw-r--r--   0        0        0      227 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/app/models.py
+-rw-r--r--   0        0        0     1704 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/app/users.py
+-rw-r--r--   0        0        0      119 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/main.py
+-rw-r--r--   0        0        0       49 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/mongodb/requirements.txt
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/__init__.py
+-rw-r--r--   0        0        0     1178 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/app.py
+-rw-r--r--   0        0        0     1249 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/db.py
+-rw-r--r--   0        0        0      257 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/models.py
+-rw-r--r--   0        0        0     1906 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/users.py
+-rw-r--r--   0        0        0      108 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/main.py
+-rw-r--r--   0        0        0       69 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy-oauth/requirements.txt
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/app/__init__.py
+-rw-r--r--   0        0        0      987 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/app/app.py
+-rw-r--r--   0        0        0     1045 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/app/db.py
+-rw-r--r--   0        0        0      227 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/app/models.py
+-rw-r--r--   0        0        0     1710 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/app/users.py
+-rw-r--r--   0        0        0      108 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/main.py
+-rw-r--r--   0        0        0       63 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/sqlalchemy/requirements.txt
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/app/__init__.py
+-rw-r--r--   0        0        0     1203 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/app/app.py
+-rw-r--r--   0        0        0      234 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/app/db.py
+-rw-r--r--   0        0        0      687 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/app/models.py
+-rw-r--r--   0        0        0     1896 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/app/users.py
+-rw-r--r--   0        0        0      119 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/main.py
+-rw-r--r--   0        0        0       60 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise-oauth/requirements.txt
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/app/__init__.py
+-rw-r--r--   0        0        0     1012 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/app/app.py
+-rw-r--r--   0        0        0      206 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/app/db.py
+-rw-r--r--   0        0        0      460 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/app/models.py
+-rw-r--r--   0        0        0     1706 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/app/users.py
+-rw-r--r--   0        0        0      119 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/main.py
+-rw-r--r--   0        0        0       54 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/examples/tortoise/requirements.txt
+-rw-r--r--   0        0        0      411 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/__init__.py
+-rw-r--r--   0        0        0      632 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/__init__.py
+-rw-r--r--   0        0        0     9172 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/authenticator.py
+-rw-r--r--   0        0        0     1791 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/backend.py
+-rw-r--r--   0        0        0      632 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/__init__.py
+-rw-r--r--   0        0        0      776 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/base.py
+-rw-r--r--   0        0        0      318 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/db/__init__.py
+-rw-r--r--   0        0        0     1108 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/db/adapter.py
+-rw-r--r--   0        0        0      417 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/db/models.py
+-rw-r--r--   0        0        0     1939 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/db/strategy.py
+-rw-r--r--   0        0        0     2212 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/jwt.py
+-rw-r--r--   0        0        0     1298 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/strategy/redis.py
+-rw-r--r--   0        0        0      379 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/transport/__init__.py
+-rw-r--r--   0        0        0     1058 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/transport/base.py
+-rw-r--r--   0        0        0     1756 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/transport/bearer.py
+-rw-r--r--   0        0        0     2190 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/authentication/transport/cookie.py
+-rw-r--r--   0        0        0     1467 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/db/__init__.py
+-rw-r--r--   0        0        0     1336 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/db/base.py
+-rw-r--r--   0        0        0     4767 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/fastapi_users.py
+-rw-r--r--   0        0        0     1028 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/jwt.py
+-rw-r--r--   0        0        0    19118 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/manager.py
+-rw-r--r--   0        0        0     1900 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/models.py
+-rw-r--r--   0        0        0       97 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/openapi.py
+-rw-r--r--   0        0        0     1220 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/password.py
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/py.typed
+-rw-r--r--   0        0        0      706 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/__init__.py
+-rw-r--r--   0        0        0     3425 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/auth.py
+-rw-r--r--   0        0        0      878 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/common.py
+-rw-r--r--   0        0        0     4755 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/oauth.py
+-rw-r--r--   0        0        0     2802 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/register.py
+-rw-r--r--   0        0        0     3174 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/reset.py
+-rw-r--r--   0        0        0     8277 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/users.py
+-rw-r--r--   0        0        0     2918 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/router/verify.py
+-rw-r--r--   0        0        0      333 2022-05-05 09:59:42.357584 fastapi-users-9.3.2/fastapi_users/types.py
+-rw-r--r--   0        0        0     8777 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/logo.svg
+-rw-r--r--   0        0        0    20084 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/logo_github.png
+-rw-r--r--   0        0        0     3118 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/mkdocs.yml
+-rw-r--r--   0        0        0     2870 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/pyproject.toml
+-rw-r--r--   0        0        0      285 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/setup.cfg
+-rw-r--r--   0        0        0      112 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/test_build.py
+-rw-r--r--   0        0        0        0 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/__init__.py
+-rw-r--r--   0        0        0    14482 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/conftest.py
+-rw-r--r--   0        0        0     4960 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_authenticator.py
+-rw-r--r--   0        0        0     1954 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_backend.py
+-rw-r--r--   0        0        0     3917 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_strategy_db.py
+-rw-r--r--   0        0        0     6293 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_strategy_jwt.py
+-rw-r--r--   0        0        0     3264 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_strategy_redis.py
+-rw-r--r--   0        0        0     1534 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_transport_bearer.py
+-rw-r--r--   0        0        0     2953 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_authentication_transport_cookie.py
+-rw-r--r--   0        0        0      794 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_db_base.py
+-rw-r--r--   0        0        0    18193 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_fastapi_users.py
+-rw-r--r--   0        0        0      393 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_jwt.py
+-rw-r--r--   0        0        0    20441 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_manager.py
+-rw-r--r--   0        0        0     4015 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_openapi.py
+-rw-r--r--   0        0        0     7469 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_router_auth.py
+-rw-r--r--   0        0        0     7378 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_router_oauth.py
+-rw-r--r--   0        0        0     4480 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_router_register.py
+-rw-r--r--   0        0        0     6233 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_router_reset.py
+-rw-r--r--   0        0        0    32911 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_router_users.py
+-rw-r--r--   0        0        0     6647 2022-05-05 09:59:42.361584 fastapi-users-9.3.2/tests/test_router_verify.py
+-rw-r--r--   0        0        0     2013 1970-01-01 00:00:00.000000 fastapi-users-9.3.2/setup.py
+-rw-r--r--   0        0        0    26698 1970-01-01 00:00:00.000000 fastapi-users-9.3.2/PKG-INFO
```

### Comparing `fastapi-users-9.3.1/.all-contributorsrc` & `fastapi-users-9.3.2/.all-contributorsrc`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981818181818183%*

 * *Differences: {"'contributors'": "{insert: [(53, OrderedDict([('login', 'ricfri'), ('name', 'Richard Friberg'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/21967765?v=4'), "*

 * *                   "('profile', 'https://github.com/ricfri'), ('contributions', ['bug'])])), (54, "*

 * *                   "OrderedDict([('login', 'KentonParton'), ('name', 'Kenton Parton'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/20202312?v=4'), "*

 * *                   "('profile', 'ht […]*

```diff
@@ -490,14 +490,32 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/29302451?v=4",
             "contributions": [
                 "code"
             ],
             "login": "jtv8",
             "name": "Joe Taylor",
             "profile": "https://github.com/jtv8"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/21967765?v=4",
+            "contributions": [
+                "bug"
+            ],
+            "login": "ricfri",
+            "name": "Richard Friberg",
+            "profile": "https://github.com/ricfri"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/20202312?v=4",
+            "contributions": [
+                "financial"
+            ],
+            "login": "KentonParton",
+            "name": "Kenton Parton",
+            "profile": "http://www.kentonparton.com"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `fastapi-users-9.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `fastapi-users-9.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/.github/stale.yml` & `fastapi-users-9.3.2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/.github/workflows/build.yml` & `fastapi-users-9.3.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/.gitignore` & `fastapi-users-9.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/LICENSE` & `fastapi-users-9.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/Makefile` & `fastapi-users-9.3.2/Makefile`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/README.md` & `fastapi-users-9.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users)
 [![PyPI version](https://badge.fury.io/py/fastapi-users.svg)](https://badge.fury.io/py/fastapi-users)
 [![Downloads](https://pepy.tech/badge/fastapi-users)](https://pepy.tech/project/fastapi-users)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-53-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-55-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <p align="center">
 <a href="https://www.buymeacoffee.com/frankie567"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Arial&outline_colour=000000&coffee_colour=FFDD00"></a>
 </p>
 
 ---
 
@@ -42,32 +42,34 @@
     * [X] [Tortoise ORM](https://tortoise-orm.readthedocs.io/en/latest/) backend included
     * [X] [ormar](https://collerek.github.io/ormar/) backend included
 * [X] Multiple customizable authentication backends
     * [X] Transports: Authorization header, Cookie
     * [X] Strategies: JWT, Database, Redis
 * [X] Full OpenAPI schema support, even with several authentication backends
 
-## 📚 Discover my book: *Building Data Science Applications with FastAPI*
+## In a hurry? Discover Fief, the open-source authentication platform
 
-<img src="https://static.packt-cdn.com/products/9781801079211/cover/smaller" alt="Building Data Science Applications with FastAPI" height="256px" align="right">
-
-**Develop, manage, and deploy efficient machine learning applications with Python**
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fief-dev/.github/main/logos/logo-full-red.svg?sanitize=true" alt="Fief" width="256" style="width: 256px">
+</p>
 
-### What is this book about?
+<img src="https://www.fief.dev/illustrations/guard-right.svg" alt="Fief" height="300" align="right" style="height: 300px">
 
-This book covers the following exciting features:
+**Implementing registration, login, social auth is hard and painful. We know it. With our highly secure and open-source users management platform, you can focus on your app while staying in control of your users data.**
 
-* Explore the basics of modern Python and async I/O programming
-* Get to grips with basic and advanced concepts of the FastAPI framework
-* Implement a FastAPI dependency to efficiently run a machine learning model
-* Integrate a simple face detection algorithm in a FastAPI backend
-* Integrate common Python data science libraries in a web backend
-* Deploy a performant and reliable web backend for a data science application
+* Based on **FastAPI Users**!
+* **Open-source**: self-host it for free or use our hosted version
+* **Bring your own database**: host your database anywhere, we'll take care of the rest
+* **Pre-built login and registration pages**: clean and fast authentication so you don't have to do it yourself
+* **Official Python client** with built-in **FastAPI integration**
 
-If you feel this book is for you, get your [copy](https://amzn.to/3kTvgjG) today!
+<p align="center">
+    <a href="https://www.fief.dev"><img width="150px" src="https://raw.githubusercontent.com/fief-dev/.github/main/graphics/join-the-beta-button.svg?sanitize=true" /></a>
+</p>
+<p align="center">It's free!</p>
 
 ## Contributors and sponsors ✨☕️
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -137,14 +139,16 @@
     <td align="center"><a href="https://ae-mc.ru"><img src="https://avatars.githubusercontent.com/u/43097289?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexandr Makurin</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=Ae-Mc" title="Code">💻</a> <a href="https://github.com/fastapi-users/fastapi-users/issues?q=author%3AAe-Mc" title="Bug reports">🐛</a></td>
   </tr>
   <tr>
     <td align="center"><a href="http://www.retoflow.de"><img src="https://avatars.githubusercontent.com/u/23637821?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Leon Thurner</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=lthurner" title="Documentation">📖</a></td>
     <td align="center"><a href="http://meka.rs"><img src="https://avatars.githubusercontent.com/u/610855?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Goran Mekić</b></sub></a><br /><a href="#platform-mekanix" title="Packaging/porting to new platform">📦</a></td>
     <td align="center"><a href="https://gaganpreet.in/"><img src="https://avatars.githubusercontent.com/u/815873?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Gaganpreet</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=gaganpreet" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/jtv8"><img src="https://avatars.githubusercontent.com/u/29302451?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Joe Taylor</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=jtv8" title="Code">💻</a></td>
+    <td align="center"><a href="https://github.com/ricfri"><img src="https://avatars.githubusercontent.com/u/21967765?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Richard Friberg</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/issues?q=author%3Aricfri" title="Bug reports">🐛</a></td>
+    <td align="center"><a href="http://www.kentonparton.com"><img src="https://avatars.githubusercontent.com/u/20202312?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kenton Parton</b></sub></a><br /><a href="#financial-KentonParton" title="Financial">💵</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 [![build](https://github.com/fastapi-users/fastapi-users/workflows/Build/
 badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [![codecov]
 (https://codecov.io/gh/fastapi-users/fastapi-users/branch/master/graph/
 badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users) [![PyPI version]
 (https://badge.fury.io/py/fastapi-users.svg)](https://badge.fury.io/py/fastapi-
 users) [![Downloads](https://pepy.tech/badge/fastapi-users)](https://pepy.tech/
 project/fastapi-users)  [![All Contributors](https://img.shields.io/badge/
-all_contributors-53-orange.svg?style=flat-square)](#contributors-)
+all_contributors-55-orange.svg?style=flat-square)](#contributors-)
             [https://img.buymeacoffee.com/button-api/?text=Buy_me_a
 coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Arial&outline_colour=000000&coffee_colour=FFDD00]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. ## Features * [X] Extensible base user
@@ -23,27 +23,29 @@
 docs.sqlalchemy.org/en/14/orm/extensions/asyncio.html) backend included * [X]
 MongoDB async backend included thanks to [mongodb/motor](https://github.com/
 mongodb/motor) * [X] [Tortoise ORM](https://tortoise-orm.readthedocs.io/en/
 latest/) backend included * [X] [ormar](https://collerek.github.io/ormar/
 ) backend included * [X] Multiple customizable authentication backends * [X]
 Transports: Authorization header, Cookie * [X] Strategies: JWT, Database, Redis
 * [X] Full OpenAPI schema support, even with several authentication backends ##
-ð Discover my book: *Building Data Science Applications with FastAPI*
-[Building Data Science Applications with FastAPI] **Develop, manage, and deploy
-efficient machine learning applications with Python** ### What is this book
-about? This book covers the following exciting features: * Explore the basics
-of modern Python and async I/O programming * Get to grips with basic and
-advanced concepts of the FastAPI framework * Implement a FastAPI dependency to
-efficiently run a machine learning model * Integrate a simple face detection
-algorithm in a FastAPI backend * Integrate common Python data science libraries
-in a web backend * Deploy a performant and reliable web backend for a data
-science application If you feel this book is for you, get your [copy](https://
-amzn.to/3kTvgjG) today! ## Contributors and sponsors â¨âï¸ Thanks goes to
-these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):
+In a hurry? Discover Fief, the open-source authentication platform
+                                    [Fief]
+[Fief] **Implementing registration, login, social auth is hard and painful. We
+know it. With our highly secure and open-source users management platform, you
+can focus on your app while staying in control of your users data.** * Based on
+**FastAPI Users**! * **Open-source**: self-host it for free or use our hosted
+version * **Bring your own database**: host your database anywhere, we'll take
+care of the rest * **Pre-built login and registration pages**: clean and fast
+authentication so you don't have to do it yourself * **Official Python client**
+with built-in **FastAPI integration**
+  [https://raw.githubusercontent.com/fief-dev/.github/main/graphics/join-the-
+                        beta-button.svg?sanitize=true]
+                                  It's free!
+## Contributors and sponsors â¨âï¸ Thanks goes to these wonderful people (
+[emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
         FranÃ§ois_Voron           Paolo_Dina              Dmytro_Ohorodnik          Matthew_D.         roywes              Satwik_Kansal        Edd_Salkield
                                                                                      Scholefield
              ð§               ðµ ð»             ð                              ð ð�         ð           ð» ð
                                                                                          ð
 
          mark-todd                    lill74                SelfhostedPro            Oskar_Gmerek    Martin_Collado         Eric_Lopes               Beau_Breon
@@ -66,17 +68,17 @@
 
            ð                 ð ð              ðµ              ð          ð»             ð»                ð»
 
      Just_van_den_Broecke           jakemanger                Ikko_Ashimine      MatyÃ¡Å¡_Richte     Hazedd                 Luis_Roel       Alexandr_Makurin
 
              ðµ               ð ð»             ð»             ð»         ð ð         ðµ          ð» ð
 
-           Leon_Thurner              Goran_MekiÄ             Gaganpreet            Joe_Taylor
+           Leon_Thurner              Goran_MekiÄ             Gaganpreet            Joe_Taylor     Richard_Friberg         Kenton_Parton
 
-               ð                  ð¦                  ð»              ð»
+               ð                  ð¦                  ð»              ð»         ð               ðµ
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Development ### Setup environment You should create a virtual
 environment and activate it: ```bash python -m venv venv/ ``` ```bash source
 venv/bin/activate ``` And then install the development dependencies: ```bash
 make install ``` ### Run unit tests You can run all the tests with: ```bash
 make test ``` Alternatively, you can run `pytest` yourself. ```bash pytest ```
```

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/backend.md` & `fastapi-users-9.3.2/docs/configuration/authentication/backend.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/index.md` & `fastapi-users-9.3.2/docs/configuration/authentication/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/strategies/database.md` & `fastapi-users-9.3.2/docs/configuration/authentication/strategies/database.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,20 @@
     --8<-- "docs/src/db_sqlalchemy_access_tokens.py"
     ```
 
 === "Tortoise ORM"
 
     With Tortoise ORM, you need to define a proper Tortoise model for `AccessToken` and manually specify the user foreign key. Besides, you need to modify the Pydantic model a bit so that it works well with this Tortoise model.
 
-    === ":octicons-file-code-16: model.py"
+    === "model.py"
         ```py hl_lines="2 4 31-38"
         --8<-- "docs/src/db_tortoise_access_tokens_model.py"
         ```
 
-    === ":octicons-file-code-16: adapter.py"
+    === "adapter.py"
         ```py hl_lines="2 4 13-14"
         --8<-- "docs/src/db_tortoise_access_tokens_adapter.py"
         ```
 
 === "MongoDB"
 
     ```py hl_lines="3 5 13 20-21"
```

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/strategies/jwt.md` & `fastapi-users-9.3.2/docs/configuration/authentication/strategies/jwt.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/strategies/redis.md` & `fastapi-users-9.3.2/docs/configuration/authentication/strategies/redis.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/transports/bearer.md` & `fastapi-users-9.3.2/docs/configuration/authentication/transports/bearer.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/authentication/transports/cookie.md` & `fastapi-users-9.3.2/docs/configuration/authentication/transports/cookie.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/databases/mongodb.md` & `fastapi-users-9.3.2/docs/configuration/databases/mongodb.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/databases/ormar.md` & `fastapi-users-9.3.2/docs/configuration/databases/ormar.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/databases/sqlalchemy.md` & `fastapi-users-9.3.2/docs/configuration/databases/sqlalchemy.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/databases/tortoise.md` & `fastapi-users-9.3.2/docs/configuration/databases/tortoise.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/models.md` & `fastapi-users-9.3.2/docs/configuration/models.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/oauth.md` & `fastapi-users-9.3.2/docs/configuration/oauth.md`

 * *Files 15% similar despite different names*

```diff
@@ -119,124 +119,124 @@
 
 !!! warning
     Notice that **SECRET** should be changed to a strong passphrase.
     Insecure passwords may give attackers full access to your database.
 
 #### SQLAlchemy
 
-[Open :octicons-link-external-16:](https://github.com/fastapi-users/fastapi-users/tree/master/examples/sqlalchemy-oauth)
+[Open :material-open-in-new:](https://github.com/fastapi-users/fastapi-users/tree/master/examples/sqlalchemy-oauth)
 
-=== ":octicons-file-code-16: requirements.txt"
+=== "requirements.txt"
 
     ```
     --8<-- "examples/sqlalchemy-oauth/requirements.txt"
     ```
 
-=== ":octicons-file-code-16: main.py"
+=== "main.py"
 
     ```py
     --8<-- "examples/sqlalchemy-oauth/main.py"
     ```
 
-=== ":octicons-file-code-16: app/app.py"
+=== "app/app.py"
 
     ```py
     --8<-- "examples/sqlalchemy-oauth/app/app.py"
     ```
 
-=== ":octicons-file-code-16: app/db.py"
+=== "app/db.py"
 
     ```py
     --8<-- "examples/sqlalchemy-oauth/app/db.py"
     ```
 
-=== ":octicons-file-code-16: app/models.py"
+=== "app/models.py"
 
     ```py
     --8<-- "examples/sqlalchemy-oauth/app/models.py"
     ```
 
-=== ":octicons-file-code-16: app/users.py"
+=== "app/users.py"
 
     ```py
     --8<-- "examples/sqlalchemy-oauth/app/users.py"
     ```
 
 #### MongoDB
 
-[Open :octicons-link-external-16:](https://github.com/fastapi-users/fastapi-users/tree/master/examples/mongodb-oauth)
+[Open :material-open-in-new:](https://github.com/fastapi-users/fastapi-users/tree/master/examples/mongodb-oauth)
 
-=== ":octicons-file-code-16: requirements.txt"
+=== "requirements.txt"
 
     ```
     --8<-- "examples/mongodb-oauth/requirements.txt"
     ```
 
-=== ":octicons-file-code-16: main.py"
+=== "main.py"
 
     ```py
     --8<-- "examples/mongodb-oauth/main.py"
     ```
 
-=== ":octicons-file-code-16: app/app.py"
+=== "app/app.py"
 
     ```py
     --8<-- "examples/mongodb-oauth/app/app.py"
     ```
 
-=== ":octicons-file-code-16: app/db.py"
+=== "app/db.py"
 
     ```py
     --8<-- "examples/mongodb-oauth/app/db.py"
     ```
 
-=== ":octicons-file-code-16: app/models.py"
+=== "app/models.py"
 
     ```py
     --8<-- "examples/mongodb-oauth/app/models.py"
     ```
 
-=== ":octicons-file-code-16: app/users.py"
+=== "app/users.py"
 
     ```py
     --8<-- "examples/mongodb-oauth/app/users.py"
     ```
 
 #### Tortoise ORM
 
-[Open :octicons-link-external-16:](https://github.com/fastapi-users/fastapi-users/tree/master/examples/tortoise-oauth)
+[Open :material-open-in-new:](https://github.com/fastapi-users/fastapi-users/tree/master/examples/tortoise-oauth)
 
-=== ":octicons-file-code-16: requirements.txt"
+=== "requirements.txt"
 
     ```
     --8<-- "examples/tortoise-oauth/requirements.txt"
     ```
 
-=== ":octicons-file-code-16: main.py"
+=== "main.py"
 
     ```py
     --8<-- "examples/tortoise-oauth/main.py"
     ```
 
-=== ":octicons-file-code-16: app/app.py"
+=== "app/app.py"
 
     ```py
     --8<-- "examples/tortoise-oauth/app/app.py"
     ```
 
-=== ":octicons-file-code-16: app/db.py"
+=== "app/db.py"
 
     ```py
     --8<-- "examples/tortoise-oauth/app/db.py"
     ```
 
-=== ":octicons-file-code-16: app/models.py"
+=== "app/models.py"
 
     ```py
     --8<-- "examples/tortoise-oauth/app/models.py"
     ```
 
-=== ":octicons-file-code-16: app/users.py"
+=== "app/users.py"
 
     ```py
     --8<-- "examples/tortoise-oauth/app/users.py"
     ```
```

### Comparing `fastapi-users-9.3.1/docs/configuration/overview.md` & `fastapi-users-9.3.2/docs/configuration/overview.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/password-hash.md` & `fastapi-users-9.3.2/docs/configuration/password-hash.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/routers/auth.md` & `fastapi-users-9.3.2/docs/configuration/routers/auth.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/routers/index.md` & `fastapi-users-9.3.2/docs/configuration/routers/index.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/routers/register.md` & `fastapi-users-9.3.2/docs/configuration/routers/register.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/routers/reset.md` & `fastapi-users-9.3.2/docs/configuration/routers/reset.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/routers/users.md` & `fastapi-users-9.3.2/docs/configuration/routers/users.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/routers/verify.md` & `fastapi-users-9.3.2/docs/configuration/routers/verify.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/configuration/user-manager.md` & `fastapi-users-9.3.2/docs/configuration/user-manager.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/cookbook/create-user-programmatically.md` & `fastapi-users-9.3.2/docs/cookbook/create-user-programmatically.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/favicon.png` & `fastapi-users-9.3.2/docs/favicon.png`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/installation.md` & `fastapi-users-9.3.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/migration/08_to_1x.md` & `fastapi-users-9.3.2/docs/migration/08_to_1x.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/migration/1x_to_2x.md` & `fastapi-users-9.3.2/docs/migration/1x_to_2x.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/migration/2x_to_3x.md` & `fastapi-users-9.3.2/docs/migration/2x_to_3x.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/migration/6x_to_7x.md` & `fastapi-users-9.3.2/docs/migration/6x_to_7x.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/migration/7x_to_8x.md` & `fastapi-users-9.3.2/docs/migration/7x_to_8x.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/migration/8x_to_9x.md` & `fastapi-users-9.3.2/docs/migration/8x_to_9x.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/cookbook_create_user_programmatically.py` & `fastapi-users-9.3.2/docs/src/cookbook_create_user_programmatically.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_mongodb_access_tokens.py` & `fastapi-users-9.3.2/docs/src/db_mongodb_access_tokens.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_ormar.py` & `fastapi-users-9.3.2/docs/src/db_ormar.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_sqlalchemy.py` & `fastapi-users-9.3.2/docs/src/db_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_sqlalchemy_access_tokens.py` & `fastapi-users-9.3.2/docs/src/db_sqlalchemy_access_tokens.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_sqlalchemy_oauth.py` & `fastapi-users-9.3.2/docs/src/db_sqlalchemy_oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_tortoise_access_tokens_model.py` & `fastapi-users-9.3.2/docs/src/db_tortoise_access_tokens_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/db_tortoise_oauth_model.py` & `fastapi-users-9.3.2/docs/src/db_tortoise_oauth_model.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/src/user_manager.py` & `fastapi-users-9.3.2/docs/src/user_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/usage/current-user.md` & `fastapi-users-9.3.2/docs/usage/current-user.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/usage/flow.md` & `fastapi-users-9.3.2/docs/usage/flow.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/docs/usage/routes.md` & `fastapi-users-9.3.2/docs/usage/routes.md`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/mongodb-oauth/app/app.py` & `fastapi-users-9.3.2/examples/mongodb-oauth/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/mongodb-oauth/app/users.py` & `fastapi-users-9.3.2/examples/mongodb-oauth/app/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/mongodb/app/app.py` & `fastapi-users-9.3.2/examples/mongodb/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/mongodb/app/users.py` & `fastapi-users-9.3.2/examples/mongodb/app/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/app.py` & `fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/db.py` & `fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/db.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/sqlalchemy-oauth/app/users.py` & `fastapi-users-9.3.2/examples/sqlalchemy-oauth/app/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/sqlalchemy/app/app.py` & `fastapi-users-9.3.2/examples/sqlalchemy/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/sqlalchemy/app/db.py` & `fastapi-users-9.3.2/examples/sqlalchemy/app/db.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/sqlalchemy/app/users.py` & `fastapi-users-9.3.2/examples/sqlalchemy/app/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/tortoise-oauth/app/app.py` & `fastapi-users-9.3.2/examples/tortoise-oauth/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/tortoise-oauth/app/models.py` & `fastapi-users-9.3.2/examples/tortoise-oauth/app/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/tortoise-oauth/app/users.py` & `fastapi-users-9.3.2/examples/tortoise-oauth/app/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/tortoise/app/app.py` & `fastapi-users-9.3.2/examples/tortoise/app/app.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/examples/tortoise/app/users.py` & `fastapi-users-9.3.2/examples/tortoise/app/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/__init__.py` & `fastapi-users-9.3.2/fastapi_users/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/authenticator.py` & `fastapi-users-9.3.2/fastapi_users/authentication/authenticator.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/backend.py` & `fastapi-users-9.3.2/fastapi_users/authentication/backend.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/strategy/__init__.py` & `fastapi-users-9.3.2/fastapi_users/authentication/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/strategy/base.py` & `fastapi-users-9.3.2/fastapi_users/authentication/strategy/base.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/strategy/db/adapter.py` & `fastapi-users-9.3.2/fastapi_users/authentication/strategy/db/adapter.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/strategy/db/strategy.py` & `fastapi-users-9.3.2/fastapi_users/authentication/strategy/db/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/strategy/jwt.py` & `fastapi-users-9.3.2/fastapi_users/authentication/strategy/jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/strategy/redis.py` & `fastapi-users-9.3.2/fastapi_users/authentication/strategy/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/transport/base.py` & `fastapi-users-9.3.2/fastapi_users/authentication/transport/base.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/transport/bearer.py` & `fastapi-users-9.3.2/fastapi_users/authentication/transport/bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/authentication/transport/cookie.py` & `fastapi-users-9.3.2/fastapi_users/authentication/transport/cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/db/__init__.py` & `fastapi-users-9.3.2/fastapi_users/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/db/base.py` & `fastapi-users-9.3.2/fastapi_users/db/base.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/fastapi_users.py` & `fastapi-users-9.3.2/fastapi_users/fastapi_users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/jwt.py` & `fastapi-users-9.3.2/fastapi_users/jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/manager.py` & `fastapi-users-9.3.2/fastapi_users/manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/models.py` & `fastapi-users-9.3.2/fastapi_users/models.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/password.py` & `fastapi-users-9.3.2/fastapi_users/password.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/__init__.py` & `fastapi-users-9.3.2/fastapi_users/router/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/auth.py` & `fastapi-users-9.3.2/fastapi_users/router/auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/common.py` & `fastapi-users-9.3.2/fastapi_users/router/common.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/oauth.py` & `fastapi-users-9.3.2/fastapi_users/router/oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/register.py` & `fastapi-users-9.3.2/fastapi_users/router/register.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/reset.py` & `fastapi-users-9.3.2/fastapi_users/router/reset.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/users.py` & `fastapi-users-9.3.2/fastapi_users/router/users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/fastapi_users/router/verify.py` & `fastapi-users-9.3.2/fastapi_users/router/verify.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/logo.svg` & `fastapi-users-9.3.2/logo.svg`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/logo_github.png` & `fastapi-users-9.3.2/logo_github.png`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/mkdocs.yml` & `fastapi-users-9.3.2/mkdocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,74 @@
 site_name: FastAPI Users
 site_description: Ready-to-use and customizable users management for FastAPI
 
 theme:
   name: 'material'
+  custom_dir: docs-overrides
   palette:
     - scheme: default
       primary: 'red'
       accent: 'red'
       toggle:
-          icon: material/lightbulb
+          icon: material/weather-sunny
           name: Switch to dark mode
     - scheme: slate
       primary: 'red'
       accent: 'red'
       toggle:
-          icon: material/lightbulb-outline
+          icon: material/weather-night
           name: Switch to light mode
   icon:
     logo: material/account-supervisor
   favicon: 'favicon.png'
+  features:
+    - navigation.instant
+    - navigation.top
+    - navigation.sections
+    - navigation.indexes
+    - search.suggest
+    - search.highlight
+    - content.code.annotate
 
 repo_name: frankie567/fastapi-users
 repo_url: https://github.com/fastapi-users/fastapi-users
 edit_uri: ""
 
 markdown_extensions:
   - toc:
       permalink: true
   - admonition
-  - codehilite
+  - pymdownx.details
+  - pymdownx.highlight:
+      anchor_linenums: true
+  - pymdownx.inlinehilite
+  - pymdownx.snippets
   - pymdownx.superfences:
       custom_fences:
         - name: mermaid
           class: mermaid
-          format: !!python/name:mermaid2.fence_mermaid
-  - pymdownx.tasklist
+          format: !!python/name:pymdownx.superfences.fence_code_format
+  - pymdownx.tasklist:
+      custom_checkbox: true
   - pymdownx.tabbed:
       alternate_style: true
-  - pymdownx.snippets
   - pymdownx.emoji:
       emoji_index: !!python/name:materialx.emoji.twemoji
       emoji_generator: !!python/name:materialx.emoji.to_svg
+  - attr_list
+  - tables
+  - def_list
 
 plugins:
   - search
-  - mermaid2:
-      arguments:
-        theme: |
-          ^(JSON.parse(window.localStorage.getItem('/.__palette')).index == 1) ? 'dark' : 'light'
+  - mike
 
-extra_javascript:
-    - https://unpkg.com/mermaid/dist/mermaid.min.js
+extra:
+  version:
+    provider: mike
 
 nav:
   - About: index.md
   - installation.md
   - Configuration:
     - configuration/overview.md
     - configuration/models.md
```

### Comparing `fastapi-users-9.3.1/pyproject.toml` & `fastapi-users-9.3.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 dev = [
     "flake8",
     "pytest",
     "requests",
     "isort",
     "pytest-asyncio",
     "flake8-docstrings",
+    "mike",
     "mkdocs",
     "mkdocs-material",
     "mkdocs-mermaid2-plugin",
     "black",
     "mypy",
     "codecov",
     "pytest-cov",
@@ -104,24 +105,24 @@
     "asgi_lifespan",
     "uvicorn",
 ]
 sqlalchemy = [
     "fastapi-users-db-sqlalchemy >=1.1.0,<2.0.0",
 ]
 sqlalchemy2 = [
-    "fastapi-users-db-sqlalchemy >=2.0.0",
+    "fastapi-users-db-sqlalchemy >=2.0.0,<4.0.0",
 ]
 mongodb = [
-    "fastapi-users-db-mongodb >=1.1.0",
+    "fastapi-users-db-mongodb >=1.1.0,<2.0.0",
 ]
 tortoise-orm = [
-    "fastapi-users-db-tortoise >=1.1.0",
+    "fastapi-users-db-tortoise >=1.1.0,<2.0.0",
 ]
 ormar = [
-    "fastapi-users-db-ormar >=1.0.0",
+    "fastapi-users-db-ormar >=1.0.0,<2.0.0",
 ]
 oauth = [
     "httpx-oauth >=0.4,<0.7"
 ]
 redis = [
     "aioredis >=2.0.1,<2.1.0",
     "hiredis >=2.0.0,<2.1.0",
```

### Comparing `fastapi-users-9.3.1/tests/conftest.py` & `fastapi-users-9.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_authenticator.py` & `fastapi-users-9.3.2/tests/test_authentication_authenticator.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_backend.py` & `fastapi-users-9.3.2/tests/test_authentication_backend.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_strategy_db.py` & `fastapi-users-9.3.2/tests/test_authentication_strategy_db.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_strategy_jwt.py` & `fastapi-users-9.3.2/tests/test_authentication_strategy_jwt.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_strategy_redis.py` & `fastapi-users-9.3.2/tests/test_authentication_strategy_redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_transport_bearer.py` & `fastapi-users-9.3.2/tests/test_authentication_transport_bearer.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_authentication_transport_cookie.py` & `fastapi-users-9.3.2/tests/test_authentication_transport_cookie.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_db_base.py` & `fastapi-users-9.3.2/tests/test_db_base.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_fastapi_users.py` & `fastapi-users-9.3.2/tests/test_fastapi_users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_manager.py` & `fastapi-users-9.3.2/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_openapi.py` & `fastapi-users-9.3.2/tests/test_openapi.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_router_auth.py` & `fastapi-users-9.3.2/tests/test_router_auth.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_router_oauth.py` & `fastapi-users-9.3.2/tests/test_router_oauth.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_router_register.py` & `fastapi-users-9.3.2/tests/test_router_register.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_router_reset.py` & `fastapi-users-9.3.2/tests/test_router_reset.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_router_users.py` & `fastapi-users-9.3.2/tests/test_router_users.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/tests/test_router_verify.py` & `fastapi-users-9.3.2/tests/test_router_verify.py`

 * *Files identical despite different names*

### Comparing `fastapi-users-9.3.1/setup.py` & `fastapi-users-9.3.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 {":python_version < '3.8'": ['typing-extensions >=4.1.1'],
  'dev': ['flake8',
          'pytest',
          'requests',
          'isort',
          'pytest-asyncio',
          'flake8-docstrings',
+         'mike',
          'mkdocs',
          'mkdocs-material',
          'mkdocs-mermaid2-plugin',
          'black',
          'mypy',
          'codecov',
          'pytest-cov',
@@ -44,24 +45,24 @@
          'pygments',
          'pymdown-extensions',
          'bumpversion',
          'httpx-oauth',
          'httpx',
          'asgi_lifespan',
          'uvicorn'],
- 'mongodb': ['fastapi-users-db-mongodb >=1.1.0'],
+ 'mongodb': ['fastapi-users-db-mongodb >=1.1.0,<2.0.0'],
  'oauth': ['httpx-oauth >=0.4,<0.7'],
- 'ormar': ['fastapi-users-db-ormar >=1.0.0'],
+ 'ormar': ['fastapi-users-db-ormar >=1.0.0,<2.0.0'],
  'redis': ['aioredis >=2.0.1,<2.1.0', 'hiredis >=2.0.0,<2.1.0'],
  'sqlalchemy': ['fastapi-users-db-sqlalchemy >=1.1.0,<2.0.0'],
- 'sqlalchemy2': ['fastapi-users-db-sqlalchemy >=2.0.0'],
- 'tortoise-orm': ['fastapi-users-db-tortoise >=1.1.0']}
+ 'sqlalchemy2': ['fastapi-users-db-sqlalchemy >=2.0.0,<4.0.0'],
+ 'tortoise-orm': ['fastapi-users-db-tortoise >=1.1.0,<2.0.0']}
 
 setup(name='fastapi-users',
-      version='9.3.1',
+      version='9.3.2',
       description='Ready-to-use and customizable users management for FastAPI',
       author=None,
       author_email='François Voron <fvoron@gmail.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `fastapi-users-9.3.1/PKG-INFO` & `fastapi-users-9.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-users
-Version: 9.3.1
+Version: 9.3.2
 Summary: Ready-to-use and customizable users management for FastAPI
 Author-email: François Voron <fvoron@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: FastAPI
@@ -25,14 +25,15 @@
 Requires-Dist: typing-extensions >=4.1.1; python_version < '3.8'
 Requires-Dist: flake8 ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: requests ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pytest-asyncio ; extra == "dev"
 Requires-Dist: flake8-docstrings ; extra == "dev"
+Requires-Dist: mike ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "dev"
 Requires-Dist: mkdocs-material ; extra == "dev"
 Requires-Dist: mkdocs-mermaid2-plugin ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: mypy ; extra == "dev"
 Requires-Dist: codecov ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
@@ -42,22 +43,22 @@
 Requires-Dist: pygments ; extra == "dev"
 Requires-Dist: pymdown-extensions ; extra == "dev"
 Requires-Dist: bumpversion ; extra == "dev"
 Requires-Dist: httpx-oauth ; extra == "dev"
 Requires-Dist: httpx ; extra == "dev"
 Requires-Dist: asgi_lifespan ; extra == "dev"
 Requires-Dist: uvicorn ; extra == "dev"
-Requires-Dist: fastapi-users-db-mongodb >=1.1.0 ; extra == "mongodb"
+Requires-Dist: fastapi-users-db-mongodb >=1.1.0,<2.0.0 ; extra == "mongodb"
 Requires-Dist: httpx-oauth >=0.4,<0.7 ; extra == "oauth"
-Requires-Dist: fastapi-users-db-ormar >=1.0.0 ; extra == "ormar"
+Requires-Dist: fastapi-users-db-ormar >=1.0.0,<2.0.0 ; extra == "ormar"
 Requires-Dist: aioredis >=2.0.1,<2.1.0 ; extra == "redis"
 Requires-Dist: hiredis >=2.0.0,<2.1.0 ; extra == "redis"
 Requires-Dist: fastapi-users-db-sqlalchemy >=1.1.0,<2.0.0 ; extra == "sqlalchemy"
-Requires-Dist: fastapi-users-db-sqlalchemy >=2.0.0 ; extra == "sqlalchemy2"
-Requires-Dist: fastapi-users-db-tortoise >=1.1.0 ; extra == "tortoise-orm"
+Requires-Dist: fastapi-users-db-sqlalchemy >=2.0.0,<4.0.0 ; extra == "sqlalchemy2"
+Requires-Dist: fastapi-users-db-tortoise >=1.1.0,<2.0.0 ; extra == "tortoise-orm"
 Project-URL: Documentation, https://fastapi-users.github.io/fastapi-users/
 Provides-Extra: dev
 Provides-Extra: mongodb
 Provides-Extra: oauth
 Provides-Extra: ormar
 Provides-Extra: redis
 Provides-Extra: sqlalchemy
@@ -75,15 +76,15 @@
 </p>
 
 [![build](https://github.com/fastapi-users/fastapi-users/workflows/Build/badge.svg)](https://github.com/fastapi-users/fastapi-users/actions)
 [![codecov](https://codecov.io/gh/fastapi-users/fastapi-users/branch/master/graph/badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users)
 [![PyPI version](https://badge.fury.io/py/fastapi-users.svg)](https://badge.fury.io/py/fastapi-users)
 [![Downloads](https://pepy.tech/badge/fastapi-users)](https://pepy.tech/project/fastapi-users)
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-53-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-55-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 <p align="center">
 <a href="https://www.buymeacoffee.com/frankie567"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Arial&outline_colour=000000&coffee_colour=FFDD00"></a>
 </p>
 
 ---
 
@@ -108,32 +109,34 @@
     * [X] [Tortoise ORM](https://tortoise-orm.readthedocs.io/en/latest/) backend included
     * [X] [ormar](https://collerek.github.io/ormar/) backend included
 * [X] Multiple customizable authentication backends
     * [X] Transports: Authorization header, Cookie
     * [X] Strategies: JWT, Database, Redis
 * [X] Full OpenAPI schema support, even with several authentication backends
 
-## 📚 Discover my book: *Building Data Science Applications with FastAPI*
+## In a hurry? Discover Fief, the open-source authentication platform
 
-<img src="https://static.packt-cdn.com/products/9781801079211/cover/smaller" alt="Building Data Science Applications with FastAPI" height="256px" align="right">
-
-**Develop, manage, and deploy efficient machine learning applications with Python**
+<p align="center">
+  <img src="https://raw.githubusercontent.com/fief-dev/.github/main/logos/logo-full-red.svg?sanitize=true" alt="Fief" width="256" style="width: 256px">
+</p>
 
-### What is this book about?
+<img src="https://www.fief.dev/illustrations/guard-right.svg" alt="Fief" height="300" align="right" style="height: 300px">
 
-This book covers the following exciting features:
+**Implementing registration, login, social auth is hard and painful. We know it. With our highly secure and open-source users management platform, you can focus on your app while staying in control of your users data.**
 
-* Explore the basics of modern Python and async I/O programming
-* Get to grips with basic and advanced concepts of the FastAPI framework
-* Implement a FastAPI dependency to efficiently run a machine learning model
-* Integrate a simple face detection algorithm in a FastAPI backend
-* Integrate common Python data science libraries in a web backend
-* Deploy a performant and reliable web backend for a data science application
+* Based on **FastAPI Users**!
+* **Open-source**: self-host it for free or use our hosted version
+* **Bring your own database**: host your database anywhere, we'll take care of the rest
+* **Pre-built login and registration pages**: clean and fast authentication so you don't have to do it yourself
+* **Official Python client** with built-in **FastAPI integration**
 
-If you feel this book is for you, get your [copy](https://amzn.to/3kTvgjG) today!
+<p align="center">
+    <a href="https://www.fief.dev"><img width="150px" src="https://raw.githubusercontent.com/fief-dev/.github/main/graphics/join-the-beta-button.svg?sanitize=true" /></a>
+</p>
+<p align="center">It's free!</p>
 
 ## Contributors and sponsors ✨☕️
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
@@ -203,14 +206,16 @@
     <td align="center"><a href="https://ae-mc.ru"><img src="https://avatars.githubusercontent.com/u/43097289?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexandr Makurin</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=Ae-Mc" title="Code">💻</a> <a href="https://github.com/fastapi-users/fastapi-users/issues?q=author%3AAe-Mc" title="Bug reports">🐛</a></td>
   </tr>
   <tr>
     <td align="center"><a href="http://www.retoflow.de"><img src="https://avatars.githubusercontent.com/u/23637821?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Leon Thurner</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=lthurner" title="Documentation">📖</a></td>
     <td align="center"><a href="http://meka.rs"><img src="https://avatars.githubusercontent.com/u/610855?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Goran Mekić</b></sub></a><br /><a href="#platform-mekanix" title="Packaging/porting to new platform">📦</a></td>
     <td align="center"><a href="https://gaganpreet.in/"><img src="https://avatars.githubusercontent.com/u/815873?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Gaganpreet</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=gaganpreet" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/jtv8"><img src="https://avatars.githubusercontent.com/u/29302451?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Joe Taylor</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/commits?author=jtv8" title="Code">💻</a></td>
+    <td align="center"><a href="https://github.com/ricfri"><img src="https://avatars.githubusercontent.com/u/21967765?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Richard Friberg</b></sub></a><br /><a href="https://github.com/fastapi-users/fastapi-users/issues?q=author%3Aricfri" title="Bug reports">🐛</a></td>
+    <td align="center"><a href="http://www.kentonparton.com"><img src="https://avatars.githubusercontent.com/u/20202312?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Kenton Parton</b></sub></a><br /><a href="#financial-KentonParton" title="Financial">💵</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-users Version: 9.3.1 Summary: Ready-to-use
+Metadata-Version: 2.1 Name: fastapi-users Version: 9.3.2 Summary: Ready-to-use
 and customizable users management for FastAPI Author-email: FranÃ§ois Voron
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License Classifier: Development
 Status :: 5 - Production/Stable Classifier: Framework :: FastAPI Classifier:
 Framework :: AsyncIO Classifier: Intended Audience :: Developers Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -11,45 +11,46 @@
 Requires-Dist: fastapi >=0.65.2,<0.76.0 Requires-Dist: passlib[bcrypt] ==1.7.4
 Requires-Dist: email-validator >=1.1.0,<1.2 Requires-Dist: pyjwt[crypto]
 ==2.3.0 Requires-Dist: python-multipart ==0.0.5 Requires-Dist: makefun
 >=1.11.2,<1.14 Requires-Dist: typing-extensions >=4.1.1; python_version < '3.8'
 Requires-Dist: flake8 ; extra == "dev" Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: requests ; extra == "dev" Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pytest-asyncio ; extra == "dev" Requires-Dist: flake8-docstrings
-; extra == "dev" Requires-Dist: mkdocs ; extra == "dev" Requires-Dist: mkdocs-
-material ; extra == "dev" Requires-Dist: mkdocs-mermaid2-plugin ; extra ==
-"dev" Requires-Dist: black ; extra == "dev" Requires-Dist: mypy ; extra ==
-"dev" Requires-Dist: codecov ; extra == "dev" Requires-Dist: pytest-cov ; extra
-== "dev" Requires-Dist: pytest-mock ; extra == "dev" Requires-Dist: flit ;
-extra == "dev" Requires-Dist: markdown-include ; extra == "dev" Requires-Dist:
-pygments ; extra == "dev" Requires-Dist: pymdown-extensions ; extra == "dev"
-Requires-Dist: bumpversion ; extra == "dev" Requires-Dist: httpx-oauth ; extra
-== "dev" Requires-Dist: httpx ; extra == "dev" Requires-Dist: asgi_lifespan ;
-extra == "dev" Requires-Dist: uvicorn ; extra == "dev" Requires-Dist: fastapi-
-users-db-mongodb >=1.1.0 ; extra == "mongodb" Requires-Dist: httpx-oauth
->=0.4,<0.7 ; extra == "oauth" Requires-Dist: fastapi-users-db-ormar >=1.0.0 ;
-extra == "ormar" Requires-Dist: aioredis >=2.0.1,<2.1.0 ; extra == "redis"
-Requires-Dist: hiredis >=2.0.0,<2.1.0 ; extra == "redis" Requires-Dist:
-fastapi-users-db-sqlalchemy >=1.1.0,<2.0.0 ; extra == "sqlalchemy" Requires-
-Dist: fastapi-users-db-sqlalchemy >=2.0.0 ; extra == "sqlalchemy2" Requires-
-Dist: fastapi-users-db-tortoise >=1.1.0 ; extra == "tortoise-orm" Project-URL:
+; extra == "dev" Requires-Dist: mike ; extra == "dev" Requires-Dist: mkdocs ;
+extra == "dev" Requires-Dist: mkdocs-material ; extra == "dev" Requires-Dist:
+mkdocs-mermaid2-plugin ; extra == "dev" Requires-Dist: black ; extra == "dev"
+Requires-Dist: mypy ; extra == "dev" Requires-Dist: codecov ; extra == "dev"
+Requires-Dist: pytest-cov ; extra == "dev" Requires-Dist: pytest-mock ; extra
+== "dev" Requires-Dist: flit ; extra == "dev" Requires-Dist: markdown-include ;
+extra == "dev" Requires-Dist: pygments ; extra == "dev" Requires-Dist: pymdown-
+extensions ; extra == "dev" Requires-Dist: bumpversion ; extra == "dev"
+Requires-Dist: httpx-oauth ; extra == "dev" Requires-Dist: httpx ; extra ==
+"dev" Requires-Dist: asgi_lifespan ; extra == "dev" Requires-Dist: uvicorn ;
+extra == "dev" Requires-Dist: fastapi-users-db-mongodb >=1.1.0,<2.0.0 ; extra
+== "mongodb" Requires-Dist: httpx-oauth >=0.4,<0.7 ; extra == "oauth" Requires-
+Dist: fastapi-users-db-ormar >=1.0.0,<2.0.0 ; extra == "ormar" Requires-Dist:
+aioredis >=2.0.1,<2.1.0 ; extra == "redis" Requires-Dist: hiredis
+>=2.0.0,<2.1.0 ; extra == "redis" Requires-Dist: fastapi-users-db-sqlalchemy
+>=1.1.0,<2.0.0 ; extra == "sqlalchemy" Requires-Dist: fastapi-users-db-
+sqlalchemy >=2.0.0,<4.0.0 ; extra == "sqlalchemy2" Requires-Dist: fastapi-
+users-db-tortoise >=1.1.0,<2.0.0 ; extra == "tortoise-orm" Project-URL:
 Documentation, https://fastapi-users.github.io/fastapi-users/ Provides-Extra:
 dev Provides-Extra: mongodb Provides-Extra: oauth Provides-Extra: ormar
 Provides-Extra: redis Provides-Extra: sqlalchemy Provides-Extra: sqlalchemy2
 Provides-Extra: tortoise-orm # FastAPI Users
                                 [FastAPI Users]
           Ready-to-use and customizable users management for FastAPI
 [![build](https://github.com/fastapi-users/fastapi-users/workflows/Build/
 badge.svg)](https://github.com/fastapi-users/fastapi-users/actions) [![codecov]
 (https://codecov.io/gh/fastapi-users/fastapi-users/branch/master/graph/
 badge.svg)](https://codecov.io/gh/fastapi-users/fastapi-users) [![PyPI version]
 (https://badge.fury.io/py/fastapi-users.svg)](https://badge.fury.io/py/fastapi-
 users) [![Downloads](https://pepy.tech/badge/fastapi-users)](https://pepy.tech/
 project/fastapi-users)  [![All Contributors](https://img.shields.io/badge/
-all_contributors-53-orange.svg?style=flat-square)](#contributors-)
+all_contributors-55-orange.svg?style=flat-square)](#contributors-)
             [https://img.buymeacoffee.com/button-api/?text=Buy_me_a
 coffee&emoji=&slug=frankie567&button_colour=FF5F5F&font_colour=ffffff&font_family=Arial&outline_colour=000000&coffee_colour=FFDD00]
 --- **Documentation**: https://fastapi-users.github.io/fastapi-users/ **Source
 Code**: https://github.com/fastapi-users/fastapi-users --- Add quickly a
 registration and authentication system to your [FastAPI](https://
 fastapi.tiangolo.com/) project. **FastAPI Users** is designed to be as
 customizable and adaptable as possible. ## Features * [X] Extensible base user
@@ -60,27 +61,29 @@
 docs.sqlalchemy.org/en/14/orm/extensions/asyncio.html) backend included * [X]
 MongoDB async backend included thanks to [mongodb/motor](https://github.com/
 mongodb/motor) * [X] [Tortoise ORM](https://tortoise-orm.readthedocs.io/en/
 latest/) backend included * [X] [ormar](https://collerek.github.io/ormar/
 ) backend included * [X] Multiple customizable authentication backends * [X]
 Transports: Authorization header, Cookie * [X] Strategies: JWT, Database, Redis
 * [X] Full OpenAPI schema support, even with several authentication backends ##
-ð Discover my book: *Building Data Science Applications with FastAPI*
-[Building Data Science Applications with FastAPI] **Develop, manage, and deploy
-efficient machine learning applications with Python** ### What is this book
-about? This book covers the following exciting features: * Explore the basics
-of modern Python and async I/O programming * Get to grips with basic and
-advanced concepts of the FastAPI framework * Implement a FastAPI dependency to
-efficiently run a machine learning model * Integrate a simple face detection
-algorithm in a FastAPI backend * Integrate common Python data science libraries
-in a web backend * Deploy a performant and reliable web backend for a data
-science application If you feel this book is for you, get your [copy](https://
-amzn.to/3kTvgjG) today! ## Contributors and sponsors â¨âï¸ Thanks goes to
-these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-
-key)):
+In a hurry? Discover Fief, the open-source authentication platform
+                                    [Fief]
+[Fief] **Implementing registration, login, social auth is hard and painful. We
+know it. With our highly secure and open-source users management platform, you
+can focus on your app while staying in control of your users data.** * Based on
+**FastAPI Users**! * **Open-source**: self-host it for free or use our hosted
+version * **Bring your own database**: host your database anywhere, we'll take
+care of the rest * **Pre-built login and registration pages**: clean and fast
+authentication so you don't have to do it yourself * **Official Python client**
+with built-in **FastAPI integration**
+  [https://raw.githubusercontent.com/fief-dev/.github/main/graphics/join-the-
+                        beta-button.svg?sanitize=true]
+                                  It's free!
+## Contributors and sponsors â¨âï¸ Thanks goes to these wonderful people (
+[emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
         FranÃ§ois_Voron           Paolo_Dina              Dmytro_Ohorodnik          Matthew_D.         roywes              Satwik_Kansal        Edd_Salkield
                                                                                      Scholefield
              ð§               ðµ ð»             ð                              ð ð�         ð           ð» ð
                                                                                          ð
 
          mark-todd                    lill74                SelfhostedPro            Oskar_Gmerek    Martin_Collado         Eric_Lopes               Beau_Breon
@@ -103,17 +106,17 @@
 
            ð                 ð ð              ðµ              ð          ð»             ð»                ð»
 
      Just_van_den_Broecke           jakemanger                Ikko_Ashimine      MatyÃ¡Å¡_Richte     Hazedd                 Luis_Roel       Alexandr_Makurin
 
              ðµ               ð ð»             ð»             ð»         ð ð         ðµ          ð» ð
 
-           Leon_Thurner              Goran_MekiÄ             Gaganpreet            Joe_Taylor
+           Leon_Thurner              Goran_MekiÄ             Gaganpreet            Joe_Taylor     Richard_Friberg         Kenton_Parton
 
-               ð                  ð¦                  ð»              ð»
+               ð                  ð¦                  ð»              ð»         ð               ðµ
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Development ### Setup environment You should create a virtual
 environment and activate it: ```bash python -m venv venv/ ``` ```bash source
 venv/bin/activate ``` And then install the development dependencies: ```bash
 make install ``` ### Run unit tests You can run all the tests with: ```bash
 make test ``` Alternatively, you can run `pytest` yourself. ```bash pytest ```
```

