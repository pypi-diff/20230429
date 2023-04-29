# Comparing `tmp/allianceauth-discordbot-3.4.0b2.tar.gz` & `tmp/allianceauth-discordbot-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-discordbot-3.4.0b2.tar", last modified: Sat Oct 22 03:08:35 2022, max compression
+gzip compressed data, was "allianceauth-discordbot-3.5.0.tar", last modified: Sat Apr 29 03:14:35 2023, max compression
```

## Comparing `allianceauth-discordbot-3.4.0b2.tar` & `allianceauth-discordbot-3.5.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 03:08:35.656336 allianceauth-discordbot-3.4.0b2/
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14841 2022-10-22 03:08:35.656336 allianceauth-discordbot-3.4.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13932 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 03:08:35.648336 allianceauth-discordbot-3.4.0b2/aadiscordbot/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1854 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     3385 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      928 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    15703 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)     3143 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/bot_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 03:08:35.652336 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1982 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/about.py
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/abuse.py
--rw-r--r--   0 runner    (1001) docker     (121)    14473 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/eastereggs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/eightball.py
--rw-r--r--   0 runner    (1001) docker     (121)    11751 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/members.py
--rw-r--r--   0 runner    (1001) docker     (121)     3560 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/price_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/quote.py
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/reaction_roles.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/remind.py
--rw-r--r--   0 runner    (1001) docker     (121)     6532 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/services.py
--rw-r--r--   0 runner    (1001) docker     (121)    15830 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/sov.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/timers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 03:08:35.656336 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/welcomegoodbye.py
--rw-r--r--   0 runner    (1001) docker     (121)      235 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 03:08:35.656336 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0003_authbotconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (121)      485 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0004_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      759 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0007_quotemessage.py
--rw-r--r--   0 runner    (1001) docker     (121)      413 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0008_channels_deleted.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0009_alter_quotemessage_options.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4556 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/providers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/aadiscordbot/views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 03:08:35.656336 allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14841 2022-10-22 03:08:35.000000 allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1757 2022-10-22 03:08:35.000000 allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 03:08:35.000000 allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-10-22 03:08:35.000000 allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-22 03:08:35.000000 allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-22 03:08:35.656336 allianceauth-discordbot-3.4.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-10-22 03:07:57.000000 allianceauth-discordbot-3.4.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.692330 allianceauth-discordbot-3.5.0/aadiscordbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16122 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/bot_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/abuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16421 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eastereggs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eightball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/price_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/prom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5180 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/reaction_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/remind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/sov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/timers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/cogs/welcomegoodbye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0003_authbotconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0004_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0007_quotemessage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0008_channels_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0009_alter_quotemessage_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/aadiscordbot/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14900 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 03:14:35.000000 allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 03:14:35.696330 allianceauth-discordbot-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-29 03:13:56.000000 allianceauth-discordbot-3.5.0/setup.py
```

### Comparing `allianceauth-discordbot-3.4.0b2/PKG-INFO` & `allianceauth-discordbot-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.4.0b2
+Version: 3.5.0
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -136,14 +136,15 @@
   "aadiscordbot.cogs.reaction_roles", # auth group integrated reaction roles
   "aadiscordbot.cogs.services", # service activation data
   "aadiscordbot.cogs.price_check", # Price Checks
   "aadiscordbot.cogs.eightball", # 8ball should i install this cog
   "aadiscordbot.cogs.welcomegoodbye", # Customizable user join/leave messages
   "aadiscordbot.cogs.models", # Populate and Maintain Django Models for Channels and Servers
   "aadiscordbot.cogs.quote", # Save and recall messages
+  "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   ]
 
 # configure the optional rate limited
 # this is a bot_task function and how many / time period
 # 100/s equates to 100 per second max
 # 10/m equates to 10 per minute or 1 every 6 seconds max
 # 60/h equates to 60 per hour or one per minute max
```

### Comparing `allianceauth-discordbot-3.4.0b2/README.md` & `allianceauth-discordbot-3.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
   "aadiscordbot.cogs.reaction_roles", # auth group integrated reaction roles
   "aadiscordbot.cogs.services", # service activation data
   "aadiscordbot.cogs.price_check", # Price Checks
   "aadiscordbot.cogs.eightball", # 8ball should i install this cog
   "aadiscordbot.cogs.welcomegoodbye", # Customizable user join/leave messages
   "aadiscordbot.cogs.models", # Populate and Maintain Django Models for Channels and Servers
   "aadiscordbot.cogs.quote", # Save and recall messages
+  "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   ]
 
 # configure the optional rate limited
 # this is a bot_task function and how many / time period
 # 100/s equates to 100 per second max
 # 10/m equates to 10 per minute or 1 every 6 seconds max
 # 60/h equates to 60 per hour or one per minute max
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/admin.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/app_settings.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/app_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -104,7 +104,10 @@
         settings, 'DISCORD_APP_ID', None))
 
 
 DISCORD_BOT_TASK_RATE_LIMITS = getattr(settings, 'DISCORD_BOT_TASK_RATE_LIMITS',
                                        {"send_channel_message_by_discord_id": "100/s",
                                         "send_direct_message_by_discord_id": "100/s",
                                         "send_direct_message_by_user_id": "100/s"})
+
+DISCORD_BOT_ESS_PING_CHANNEL_ID = getattr(
+    settings, 'DISCORD_BOT_ESS_PING_CHANNEL_ID', None)
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/auth_hooks.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/bot.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,16 +145,16 @@
             command_prefix=DISCORD_BOT_PREFIX,
             description=description,
             intents=intents,
         )
         print(f"Authbot Started with command prefix {DISCORD_BOT_PREFIX}")
 
         self.redis = None
-        self.redis = self.loop.run_until_complete(aioredis.create_pool(getattr(
-            settings, "BROKER_URL", "redis://localhost:6379/0"), minsize=5, maxsize=10))
+        self.redis = self.loop.run_until_complete(aioredis.from_url(getattr(
+            settings, "BROKER_URL", "redis://localhost:6379/0"), encoding="utf-8", decode_responses=True))
         print('redis pool started', self.redis)
         self.client_id = client_id
         self.session = aiohttp.ClientSession(loop=self.loop)
 
         self.tasks = []
         self.pending_tasks = PendingQueue()
         self.rate_limits = RateLimiter()
@@ -357,22 +357,28 @@
         elif isinstance(error, commands.NotOwner):
             print(error)
             await ctx.send(error)
         elif isinstance(error, commands.CommandOnCooldown):
             await ctx.message.add_reaction(chr(0x274C))
         elif isinstance(error, commands.CheckFailure):
             await ctx.send(error)
+        else:
+            logger.error(f"Unknown Error {error}", exc_info=True)
+            await ctx.send("Something Went Wrong, Please try again Later.",)
 
     async def on_application_command_error(self, context: ApplicationContext, exception: DiscordException) -> None:
         if isinstance(exception, commands.CheckFailure):
             await context.send_response(exception, ephemeral=True)
         elif isinstance(exception, commands.MissingPermissions):
             await context.send_response(exception, ephemeral=True)
         elif isinstance(exception, NotAuthenticated):
             await context.send_response(exception, ephemeral=True)
+        else:  # Catch everything, and close out the interactions gracefully.
+            logger.error(f"Unknown Error {exception}", exc_info=True)
+            await context.respond("Something Went Wrong, Please try again Later.", ephemeral=True)
 
     def run(self):
         # self.load_extension("aadiscordbot.slash.admin")
         try:
 
             logger.info(
                 "******************************************************")
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/bot_tasks.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/bot_tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import importlib
 import logging
 import warnings
 from datetime import timedelta
 
 from discord import Embed
 from discord.ext import tasks
+from discord.ui import View
 
 import django
 from django.utils import timezone
 
 logger = logging.getLogger(__name__)
 
 
@@ -34,21 +36,29 @@
             except Exception as e:
                 logger.error(f"Failed to run task {task} {args} {kwargs} {e}")
     else:
         run_tasks.stop()
     django.db.close_old_connections()
 
 
-async def send_channel_message_by_discord_id(bot, channel_id, message, embed=False):
+async def send_channel_message_by_discord_id(bot, channel_id, message, embed=False, view_class=False, view_args=[], view_kwargs={}):
     logger.debug(f"Sending Channel Message to Discord ID {channel_id}")
+    e = None
+    v = None
     if embed:
         e = Embed.from_dict(embed)
-        await bot.get_channel(channel_id).send(message, embed=e)
-    else:
-        await bot.get_channel(channel_id).send(message)
+
+    if view_class:
+        m = ".".join(view_class.split(".")[:-1])
+        c = view_class.split(".")[-1]
+        my_module = importlib.import_module(m)
+        Viewclass = getattr(my_module, c)
+        v = Viewclass(*view_args, **view_kwargs)
+
+    await bot.get_channel(channel_id).send(message, embed=e, view=v)
 
 
 async def send_channel_message(bot, channel_id, message, embed=False):
     warnings.warn(
         "send_channel_message is deprecated, use send_channel_message_by_discord_id instead",
         DeprecationWarning
     )
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/about.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/about.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,10 +54,47 @@
         )
         embed.add_field(
             name="Version", value=f"{__version__}@{__branch__}", inline=False
         )
 
         return await ctx.respond(embed=embed)
 
+    @about_commands.command(name="server", description="About this Discord Server", guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    async def server(self, ctx):
+        """
+        All about a server
+        """
+        embed = Embed(title=ctx.guild.name)
+
+        if ctx.guild.icon:
+            embed.set_thumbnail(
+                url=ctx.guild.icon.url
+            )
+        embed.color = Color.blue()
+        embed.description = "Alliance Auth Managed EvE Online Discord Server!"
+        if ctx.guild.description:
+            embed.description = ctx.guild.description
+        embed.set_footer(
+            text="AuthBot Lovingly developed for Init.™ by AaronRin and ArielKable")
+
+        members = ctx.guild.member_count
+        embed.add_field(name="Unwilling Monitorees:",
+                        value=members, inline=True)
+
+        channels = len(ctx.guild.channels)
+        cats = len(ctx.guild.categories)
+        embed.add_field(name="Channel Count:",
+                        value=channels-cats, inline=True)
+
+        roles = len(ctx.guild.roles)
+        embed.add_field(name="Role Count:",
+                        value=roles, inline=True)
+
+        embed.add_field(
+            name="Auth Link", value=f"[{get_site_url()}]({get_site_url()})", inline=False
+        )
+
+        return await ctx.respond(embed=embed)
+
 
 def setup(bot):
     bot.add_cog(About(bot))
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/abuse.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eightball.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,58 @@
 import logging
 from random import randrange
 
 from discord.ext import commands
+from discord.utils import get
 
 from django.conf import settings
 
 from aadiscordbot import __branch__, __version__
 
 logger = logging.getLogger(__name__)
 
 
-class Abuse(commands.Cog):
+class EightBall(commands.Cog):
     """
     All about me!
     """
 
     def __init__(self, bot):
         self.bot = bot
 
-    @commands.Cog.listener("on_message")
-    async def respond_to_abuse(self, message):
+    def eightball(self):
         replies = [
-            "get a dog up ya, cunt",
-            "Can I help you? Do you want a time out?",
-            "No u",
-            "How about Nooooooooo!",
-            "Thats a horrible thing to say about your mother",
-            "I know you are, but what am I",
-            "I'm sorry, did you say something? I don't speak moron",
-            "Command accepted! Now commencing with your time out",
-            "You kiss your mother with that mouth?!?",
-            "Thats what she said"
+            "It is certain",
+            "It is decidedly so",
+            "Without a doubt",
+            "Yes definitely!",
+            "As I see it, yes",
+            "Most likely",
+            "Outlook good",
+            "Yes",
+            "Signs point to yes",
+            "Reply hazy, try again",
+            "Better not tell you now",
+            "Cannot predict now",
+            "Concentrate and ask again",
+            "Don't count on it",
+            "My reply is no",
+            "My sources say no",
+            "Outlook not so good",
+            "Very doubtful",
         ]
-        rand = randrange(0, len(replies)-1)
-        if message.mention_everyone:
-            return
-        if self.bot.user.mentioned_in(message):
-            await message.reply(replies[rand])
+        return replies[randrange(0, len(replies)-1)]
+
+    @commands.command(pass_context=True, aliases=['8ball'])
+    async def meb(self, message):
+        """
+        8 ball go brrrr
+        """
+        await message.reply(self.eightball())
+
+    @commands.slash_command(name='8ball', guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    async def meb_slash(self, ctx, question: str):
+        await ctx.respond(f" You Asked: `{question}`\n\n{self.eightball()}")
 
 
 def setup(bot):
-    bot.add_cog(Abuse(bot))
+    bot.add_cog(EightBall(bot))
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/admin.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from django.conf import settings
 from django.contrib.auth.models import Group
 from django.core.exceptions import ObjectDoesNotExist
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.eveonline.tasks import update_character
 from allianceauth.services.modules.discord.models import DiscordUser
+from allianceauth.services.modules.discord.tasks import (
+    update_groups, update_nickname,
+)
 
 from .. import app_settings
 
 logger = logging.getLogger(__name__)
 
 
 class Admin(commands.Cog):
@@ -345,10 +348,47 @@
                 update_character.delay(c)
             return await ctx.respond(f"Sent tasks to update **{character}**'s Alts")
         except EveCharacter.DoesNotExist:
             return await ctx.respond(f"Character **{character}** does not exist in our Auth system")
         except ObjectDoesNotExist:
             return await ctx.respond(f"**{character}** is Unlinked unable to update characters")
 
+    @admin_commands.command(name='sync_commands', guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    @option("force", description="Force Sync Everything")
+    async def sync_commands(
+        self,
+        ctx,
+        force: bool
+    ):
+        """
+        Re-Sync the commands to discord.
+        """
+        if ctx.author.id not in app_settings.get_admins():
+            return await ctx.respond(f"You do not have permission to use this command", ephemeral=True)
+
+        await ctx.defer(ephemeral=True)
+
+        await self.bot.sync_commands(force=force)
+
+        return await ctx.respond(f"Sync Complete!", ephemeral=True)
+
+    @commands.user_command(name="Group Sync", guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    async def group_sync_user_context(self, ctx, user):
+        # https://media1.tenor.com/images/1796f0fa0b4b07e51687fad26a2ce735/tenor.gif
+        if ctx.author.id not in app_settings.get_admins():
+            return await ctx.respond(f"You do not have permission to use this command", ephemeral=True)
+        auth_user = DiscordUser.objects.get(uid=user.id)
+        update_groups.delay(auth_user.user_id)
+        await ctx.respond(f"Requested Group Sync for {auth_user.user.profile.main_character}", ephemeral=True)
+
+    @commands.user_command(name="Nickname Sync", guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    async def nick_sync_user_context(self, ctx, user):
+        # https://media1.tenor.com/images/1796f0fa0b4b07e51687fad26a2ce735/tenor.gif
+        if ctx.author.id not in app_settings.get_admins():
+            return await ctx.respond(f"You do not have permission to use this command", ephemeral=True)
+        auth_user = DiscordUser.objects.get(uid=user.id)
+        update_nickname.delay(auth_user.user_id)
+        await ctx.respond(f"Requested Nickname Sync for {auth_user.user.profile.main_character}", ephemeral=True)
+
 
 def setup(bot):
     bot.add_cog(Admin(bot))
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/auth.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/auth.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/eastereggs.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/eastereggs.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/members.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/members.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from discord.ext import commands
 
 from django.conf import settings
 from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
 
 from allianceauth.eveonline.evelinks import evewho
-from allianceauth.eveonline.models import EveCharacter
+from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
 
 from aadiscordbot.app_settings import aastatistics_active
 from aadiscordbot.cogs.utils.decorators import (
     has_any_perm, in_channels, message_in_channels, sender_has_any_perm,
 )
 
 logger = logging.getLogger(__name__)
@@ -187,51 +187,71 @@
 
     async def search_corps_on_characters(ctx: AutocompleteContext):
         """Returns a list of colors that begin with the characters entered so far."""
         return list(EveCharacter.objects.filter(corporation_name__icontains=ctx.value).values_list('corporation_name', flat=True).distinct()[:10])
 
     def build_altcorp_embeds(self, input_name):
         chars = EveCharacter.objects.filter(corporation_name=input_name)
-        own_ids = [settings.DISCORD_BOT_MEMBER_ALLIANCES]
-        alts_in_corp = []
-        for c in chars:
-            if c.alliance_id not in own_ids:
-                alts_in_corp.append(c)
+        if chars.count():
+            corp_id = 0
+            own_ids = [settings.DISCORD_BOT_MEMBER_ALLIANCES]
+            alts_in_corp = []
+            knowns = 0
+            for c in chars:
+                corp_id = c.corporation_id
+                alliance = c.alliance_name
+                if c.alliance_id not in own_ids:
+                    alts_in_corp.append(c)
 
-        mains = {}
-        for a in alts_in_corp:
-            try:
-                main = a.character_ownership.user.profile.main_character
-                if main.character_id not in mains:
-                    mains[main.character_id] = [main, 0]
-                mains[main.character_id][1] += 1
-                alt_corp_id = a.corporation_id
-            except Exception as e:
-                logger.error(e)
-                pass
-        output = []
-        base_string = "[{}]({}) [ [{}]({}) ] has {} alt{}"
-        for k, m in mains.items():
-            output.append(
-                base_string.format(
-                    m[0],
-                    evewho.character_url(m[0].character_id),
-                    m[0].corporation_ticker,
-                    evewho.corporation_url(m[0].corporation_id),
-                    m[1],
-                    "s" if m[1] > 1 else ""
+            mains = {}
+            for a in alts_in_corp:
+                try:
+                    main = a.character_ownership.user.profile.main_character
+                    if main.character_id not in mains:
+                        mains[main.character_id] = [main, 0]
+                    mains[main.character_id][1] += 1
+                    knowns += 1
+                except Exception as e:
+                    # logger.error(e)
+                    pass
+            output = []
+            base_string = "[{}]({}) [ [{}]({}) ] has {} alt{}"
+            for k, m in mains.items():
+                output.append(
+                    base_string.format(
+                        m[0],
+                        evewho.character_url(m[0].character_id),
+                        m[0].corporation_ticker,
+                        evewho.corporation_url(m[0].corporation_id),
+                        m[1],
+                        "s" if m[1] > 1 else ""
+                    )
                 )
+            embeds = []
+
+            corp_info = EveCorporationInfo.provider.get_corporation(corp_id)
+
+            msg = f"**[ [{corp_info.ticker}]({evewho.corporation_url(corp_id)}) ]** has {corp_info.members} members:\n\n"\
+                f"```diff\n"\
+                f"+Known Members     : {knowns}\n"\
+                f"-Unknowns          : {corp_info.members-knowns}```"
+
+            _header = Embed(
+                title=input_name,
+                description=msg
             )
-        embeds = []
-        for strings in [output[i:i + 10] for i in range(0, len(output), 10)]:
-            embed = Embed(title=input_name)
-            embed.colour = Color.blue()
-            embed.description = "\n".join(strings)
-            embeds.append(embed)
-        return embeds
+
+            embeds.append(_header)
+
+            for strings in [output[i:i + 10] for i in range(0, len(output), 10)]:
+                embed = Embed(title=input_name)
+                embed.colour = Color.blue()
+                embed.description = "\n".join(strings)
+                embeds.append(embed)
+            return embeds
 
     @commands.slash_command(name='altcorp', guild_ids=[int(settings.DISCORD_GUILD_ID)])
     @option("corporation", description="Search for a Character!", autocomplete=search_corps_on_characters)
     async def slash_altcorp(
         self,
         ctx,
         corporation: str,
@@ -239,15 +259,15 @@
         try:
             in_channels(ctx.channel.id, settings.ADMIN_DISCORD_BOT_CHANNELS)
             has_any_perm(ctx.author.id, [
                          'corputils.view_alliance_corpstats', 'corpstats.view_alliance_corpstats'])
             await ctx.defer()
             embeds = self.build_altcorp_embeds(corporation)
             if len(embeds):
-                e = embeds.pop()
+                e = embeds.pop(0)
                 await ctx.respond(embed=e)
                 for e in embeds:
                     await ctx.send(embed=e)
             else:
                 await ctx.respond("No Members Found!")
         except commands.MissingPermissions as e:
             return await ctx.respond(e.missing_permissions[0], ephemeral=True)
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/models.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/price_check.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/price_check.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/quote.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/quote.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/reaction_roles.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/reaction_roles.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/remind.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/remind.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/services.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/services.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/sov.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/sov.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/time.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/timers.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/timers.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/utils/decorators.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/utils/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
 
 
 def has_perm(id, perm: str):
     if id in get_admins():
         return True
     try:
-        has_perm = DiscordUser.objects.get(uid=id).user.has_perm(perm)
+        user = DiscordUser.objects.get(uid=id)
+        has_perm = user.user.has_perm(perm)
+
         if has_perm:
             return True
         else:
             raise commands.MissingPermissions([perm])
-    except Exception as e:
+    except DiscordUser.DoesNotExist as e:
         logger.error(e)
         raise NotAuthenticated
 
 
 def sender_has_perm(perm: str):
     """
     Permission Decorator: Does the user have x Django Permission
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/cogs/welcomegoodbye.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/cogs/welcomegoodbye.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import logging
 
 from discord.ext import commands
 
 from allianceauth.services.modules.discord.models import DiscordUser
 
 from aadiscordbot.models import GoodbyeMessage, WelcomeMessage
+from aadiscordbot.app_settings import get_site_url
 
 logger = logging.getLogger(__name__)
 
 
 class Welcome(commands.Cog):
     """
     Responds to on_member_join events from discord
```

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0001_initial.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0002_reactionrolebinding_reactionrolemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0003_authbotconfiguration.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0003_authbotconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0005_rr_fixes_blank_admins.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0006_goodbyemessage_welcomemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/migrations/0007_quotemessage.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/migrations/0007_quotemessage.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/models.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth-discordbot-3.4.0b2/aadiscordbot/tasks.py` & `allianceauth-discordbot-3.5.0/aadiscordbot/tasks.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             kwargs={"embed": embed},
             countdown=countdown)
 
 # Note these Tasks do not DO anything. They can simply be called by AA to add the tasks to our Queue of choice to be consumed by bot.queueconsumer
 
 
 @shared_task
-def send_channel_message_by_discord_id(channel_id, message_content, embed=False):
+def send_channel_message_by_discord_id(channel_id, message_content, embed=None, view_class: str = None, view_args: list = [], view_kwargs: dict = {}):
     # Queue a message to a Discord Channel
     raise Exception(
         f"This function should be called asynchronously. Failed to queue a message to Channel {channel_id}")
 
 
 @shared_task
 def send_channel_message(channel_id, message_content, embed=False):
```

### Comparing `allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/PKG-INFO` & `allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-discordbot
-Version: 3.4.0b2
+Version: 3.5.0
 Summary: Alliance Auth Discord Bot
 Home-page: https://github.com/pvyParts/allianceauth-discordbot
 Author: ak
 Author-email: ak@ak.auth
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
@@ -136,14 +136,15 @@
   "aadiscordbot.cogs.reaction_roles", # auth group integrated reaction roles
   "aadiscordbot.cogs.services", # service activation data
   "aadiscordbot.cogs.price_check", # Price Checks
   "aadiscordbot.cogs.eightball", # 8ball should i install this cog
   "aadiscordbot.cogs.welcomegoodbye", # Customizable user join/leave messages
   "aadiscordbot.cogs.models", # Populate and Maintain Django Models for Channels and Servers
   "aadiscordbot.cogs.quote", # Save and recall messages
+  "aadiscordbot.cogs.prom_export", # Admin Level Logging cog
   ]
 
 # configure the optional rate limited
 # this is a bot_task function and how many / time period
 # 100/s equates to 100 per second max
 # 10/m equates to 10 per minute or 1 every 6 seconds max
 # 60/h equates to 60 per hour or one per minute max
```

### Comparing `allianceauth-discordbot-3.4.0b2/allianceauth_discordbot.egg-info/SOURCES.txt` & `allianceauth-discordbot-3.5.0/allianceauth_discordbot.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 aadiscordbot/cogs/admin.py
 aadiscordbot/cogs/auth.py
 aadiscordbot/cogs/eastereggs.py
 aadiscordbot/cogs/eightball.py
 aadiscordbot/cogs/members.py
 aadiscordbot/cogs/models.py
 aadiscordbot/cogs/price_check.py
+aadiscordbot/cogs/prom_export.py
 aadiscordbot/cogs/quote.py
 aadiscordbot/cogs/reaction_roles.py
 aadiscordbot/cogs/remind.py
 aadiscordbot/cogs/services.py
 aadiscordbot/cogs/sov.py
 aadiscordbot/cogs/time.py
 aadiscordbot/cogs/timers.py
```

### Comparing `allianceauth-discordbot-3.4.0b2/setup.py` & `allianceauth-discordbot-3.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,10 +37,10 @@
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     python_requires='>=3.8',
     install_requires=[
         "allianceauth>=2.9.0,<4.0.0",
         "py-cord>2.0.0,<3.0.0",
         "pendulum>=2.1.2,<3.0.0",
-        "aioredis<2.0.0"
+        "aioredis>=2.0.0"
     ],
 )
```

