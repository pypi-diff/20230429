# Comparing `tmp/qq.py-1.2.7.tar.gz` & `tmp/qq.py-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qq.py-1.2.7.tar", last modified: Thu May 26 05:31:29 2022, max compression
+gzip compressed data, was "qq.py-1.2.8.tar", last modified: Tue Jun  7 12:42:59 2022, max compression
```

## Comparing `qq.py-1.2.7.tar` & `qq.py-1.2.8.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.358434 qq.py-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-05-26 05:31:19.000000 qq.py-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-26 05:31:19.000000 qq.py-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-05-26 05:31:29.358434 qq.py-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-05-26 05:31:19.000000 qq.py-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.354434 qq.py-1.2.7/qq/
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9803 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21929 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/abc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/api_permission.py
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/asset.py
--rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/backoff.py
--rw-r--r--   0 runner    (1001) docker     (121)    33870 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)    27718 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     9820 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/colour.py
--rw-r--r--   0 runner    (1001) docker     (121)    23560 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/embeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7848 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)     6090 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     6612 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.350434 qq.py-1.2.7/qq/ext/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.358434 qq.py-1.2.7/qq/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (121)    37643 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)    16565 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (121)    13616 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (121)    30786 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/converter.py
--rw-r--r--   0 runner    (1001) docker     (121)    12698 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/cooldowns.py
--rw-r--r--   0 runner    (1001) docker     (121)    72175 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    26713 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    21007 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)    45275 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (121)     6023 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/commands/view.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.358434 qq.py-1.2.7/qq/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)    25175 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/file.py
--rw-r--r--   0 runner    (1001) docker     (121)    10880 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/flags.py
--rw-r--r--   0 runner    (1001) docker     (121)    19481 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)    37874 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/guild.py
--rw-r--r--   0 runner    (1001) docker     (121)    30163 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/http.py
--rw-r--r--   0 runner    (1001) docker     (121)    15486 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)    15214 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/member.py
--rw-r--r--   0 runner    (1001) docker     (121)     5322 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/mention.py
--rw-r--r--   0 runner    (1001) docker     (121)    38808 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/object.py
--rw-r--r--   0 runner    (1001) docker     (121)     5909 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/partial_emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)    12027 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     7040 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/reaction.py
--rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)    16124 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/shard.py
--rw-r--r--   0 runner    (1001) docker     (121)    35864 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.358434 qq.py-1.2.7/qq/types/
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/embed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/guild.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/member.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/permission.py
--rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/raw_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/role.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/types/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    21071 2022-05-26 05:31:19.000000 qq.py-1.2.7/qq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 05:31:29.354434 qq.py-1.2.7/qq.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-05-26 05:31:29.000000 qq.py-1.2.7/qq.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-05-26 05:31:29.000000 qq.py-1.2.7/qq.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 05:31:29.000000 qq.py-1.2.7/qq.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-05-26 05:31:29.000000 qq.py-1.2.7/qq.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-05-26 05:31:29.000000 qq.py-1.2.7/qq.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-05-26 05:31:19.000000 qq.py-1.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-26 05:31:29.358434 qq.py-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-05-26 05:31:19.000000 qq.py-1.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.251878 qq.py-1.2.8/
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-06-07 12:42:50.000000 qq.py-1.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-06-07 12:42:50.000000 qq.py-1.2.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-06-07 12:42:59.251878 qq.py-1.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-06-07 12:42:50.000000 qq.py-1.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.247878 qq.py-1.2.8/qq/
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9803 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21929 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/abc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2948 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/api_permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5138 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/asset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5225 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33870 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27717 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9820 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/colour.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23527 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7848 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6090 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6612 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/error.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.243878 qq.py-1.2.8/qq/ext/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.251878 qq.py-1.2.8/qq/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37643 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16565 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13616 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30786 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/converter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12698 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/cooldowns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    72175 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26713 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21007 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/flags.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45275 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6023 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/commands/view.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.251878 qq.py-1.2.8/qq/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (121)    25175 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/file.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10880 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/flags.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19481 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38024 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/guild.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30293 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15486 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15214 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/member.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5322 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/mention.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38808 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2606 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/object.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5909 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/partial_emoji.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12027 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     7040 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16124 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/shard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35882 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.251878 qq.py-1.2.8/qq/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/audio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/embed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1986 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/guild.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/member.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/permission.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2446 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/raw_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1414 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8503 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21071 2022-06-07 12:42:50.000000 qq.py-1.2.8/qq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 12:42:59.247878 qq.py-1.2.8/qq.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3543 2022-06-07 12:42:59.000000 qq.py-1.2.8/qq.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-06-07 12:42:59.000000 qq.py-1.2.8/qq.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 12:42:59.000000 qq.py-1.2.8/qq.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 12:42:59.000000 qq.py-1.2.8/qq.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-06-07 12:42:59.000000 qq.py-1.2.8/qq.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-07 12:42:50.000000 qq.py-1.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 12:42:59.251878 qq.py-1.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2479 2022-06-07 12:42:50.000000 qq.py-1.2.8/setup.py
```

### Comparing `qq.py-1.2.7/LICENSE` & `qq.py-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/PKG-INFO` & `qq.py-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qq.py
-Version: 1.2.7
+Version: 1.2.8
 Summary: QQ 频道 API 的 Python Wrapper
 Home-page: https://github.com/foxwhite25/qq.py
 Author: foxwhite25
 Author-email: vct.xie@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qq.py-1.2.7/README.md` & `qq.py-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/__init__.py` & `qq.py-1.2.8/qq/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 __title__ = 'qq'
 __author__ = 'Foxwhite'
 __license__ = 'MIT'
-__version__ = '1.2.7'
+__version__ = '1.2.8'
 
 #  The MIT License (MIT)
 #  Copyright (c) 2021-present foxwhite25
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a
 #  copy of this software and associated documentation files (the "Software"),
 #  to deal in the Software without restriction, including without limitation
@@ -57,8 +57,8 @@
     major: int
     minor: int
     micro: int
     releaselevel: Literal["alpha", "beta", "candidate", "final"]
     serial: int
 
 
-version_info: VersionInfo = VersionInfo(major=1, minor=2, micro=7, releaselevel='beta', serial=0)
+version_info: VersionInfo = VersionInfo(major=1, minor=2, micro=8, releaselevel='beta', serial=0)
```

### Comparing `qq.py-1.2.7/qq/__main__.py` & `qq.py-1.2.8/qq/__main__.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/abc.py` & `qq.py-1.2.8/qq/abc.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/api_permission.py` & `qq.py-1.2.8/qq/api_permission.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/asset.py` & `qq.py-1.2.8/qq/asset.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/audio.py` & `qq.py-1.2.8/qq/audio.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/backoff.py` & `qq.py-1.2.8/qq/backoff.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/channel.py` & `qq.py-1.2.8/qq/channel.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/client.py` & `qq.py-1.2.8/qq/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,15 +686,15 @@
         asyncio.TimeoutError
             如果提供超时并且已达到。
 
         Returns
         --------
         Any
             不返回任何参数、单个参数或多个参数的元组，
-            这些参数反映在 :ref:`事件指南 <qq-api-events>` 中传递的参数。
+            这些参数反映在 :ref:`事件指南`<qq-api-events> 中传递的参数。
         """
 
         future = self.loop.create_future()
         if check is None:
             def _check(*args):
                 return True
```

### Comparing `qq.py-1.2.7/qq/colour.py` & `qq.py-1.2.8/qq/colour.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/embeds.py` & `qq.py-1.2.8/qq/embeds.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,18 +322,17 @@
 
         if timestamp:
             self.timestamp = timestamp
 
     @classmethod
     def from_dict(cls: Type[E], data: Mapping[str, Any]) -> E:
         """将 :class:`dict` 转换为 :class:`Embed`，前提是它采用 QQ 期望的格式。
-        你可以在 ``官方 QQ 文档``__ 中找到有关此格式的信息。
+        你可以在 ``官方 QQ 文档`` 中找到有关此格式的信息。
 
-        .. _QQDocs: https://bot.q.qq.com/wiki/develop/api/openapi/message/model.html#messageembed
-        __ QQDocs_
+        https://bot.q.qq.com/wiki/develop/api/openapi/message/model.html#messageembed
 
         Parameters
         -----------
         data: :class:`dict`
             要转换为嵌入的字典。
         """
         # we are bypassing __init__ here since it doesn't apply here
```

### Comparing `qq.py-1.2.7/qq/emoji.py` & `qq.py-1.2.8/qq/emoji.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/enum.py` & `qq.py-1.2.8/qq/enum.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/error.py` & `qq.py-1.2.8/qq/error.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/__init__.py` & `qq.py-1.2.8/qq/ext/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/_types.py` & `qq.py-1.2.8/qq/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/bot.py` & `qq.py-1.2.8/qq/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/cog.py` & `qq.py-1.2.8/qq/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/context.py` & `qq.py-1.2.8/qq/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/converter.py` & `qq.py-1.2.8/qq/ext/commands/converter.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/cooldowns.py` & `qq.py-1.2.8/qq/ext/commands/cooldowns.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/core.py` & `qq.py-1.2.8/qq/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/errors.py` & `qq.py-1.2.8/qq/ext/commands/errors.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/flags.py` & `qq.py-1.2.8/qq/ext/commands/flags.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/help.py` & `qq.py-1.2.8/qq/ext/commands/help.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/commands/view.py` & `qq.py-1.2.8/qq/ext/commands/view.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/ext/tasks/__init__.py` & `qq.py-1.2.8/qq/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/file.py` & `qq.py-1.2.8/qq/file.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/flags.py` & `qq.py-1.2.8/qq/flags.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/gateway.py` & `qq.py-1.2.8/qq/gateway.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/guild.py` & `qq.py-1.2.8/qq/guild.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,20 +167,27 @@
             ('name', self.name),
             ('member_count', getattr(self, '_member_count', None)),
         )
         inner = ' '.join('%s=%r' % t for t in attrs)
         return f'<Guild {inner}>'
 
     async def fill_in(self):
-        channels = await self._state.http.get_guild_channels(self.id)
-        result = await self._state.http.get_member(self.id, self._state.user.id)
+        try:
+            channels = await self._state.http.get_guild_channels(self.id)
+        except HTTPException:
+            channels = []
+
+        try:
+            result = await self._state.http.get_member(self.id, self._state.user.id)
 
-        member = Member(data=result,
-                        guild=self, state=self._state)
-        self._add_member(member)
+            member = Member(data=result,
+                            guild=self, state=self._state)
+            self._add_member(member)
+        except HTTPException:
+            pass
 
         try:
 
             permissions = await self._state.http.get_permission(self.id)
             for permission in permissions['apis']:
                 permission = Permission(data=permission, state=self._state, guild=self)
                 self._permission.append(permission)
```

### Comparing `qq.py-1.2.7/qq/http.py` & `qq.py-1.2.8/qq/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,16 +274,19 @@
                 if form:
                     form_data = aiohttp.FormData()
                     for key, value in form.items():
                         form_data.add_field(key, value)
                     kwargs['data'] = form_data
                 try:
                     async with self.__session.request(method, url, **kwargs) as response:
-                        _log.debug('%s %s 与 %s 已返回 %s Trace ID: %s', method, url, kwargs.get('data'),
-                                   response.status, response.headers['X-Tps-trace-ID'])
+                        _log.debug(
+                            '%s %s 与 %s 已返回 %s Trace ID: %s', method, url, kwargs.get('data'),
+                            response.status,
+                            response.headers['X-Tps-trace-ID'] if 'X-Tps-trace-ID' in response.headers else "Missing"
+                        )
 
                         # even errors have text involved in them so this is safe to call
                         data = await json_or_text(response)
 
                         # the request was successful so just return the text/json
                         if 300 > response.status >= 200:
                             if response.status != 204:
```

### Comparing `qq.py-1.2.7/qq/iterators.py` & `qq.py-1.2.8/qq/iterators.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/member.py` & `qq.py-1.2.8/qq/member.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/mention.py` & `qq.py-1.2.8/qq/mention.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/message.py` & `qq.py-1.2.8/qq/message.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/mixins.py` & `qq.py-1.2.8/qq/mixins.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/object.py` & `qq.py-1.2.8/qq/object.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/partial_emoji.py` & `qq.py-1.2.8/qq/partial_emoji.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/permissions.py` & `qq.py-1.2.8/qq/permissions.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/raw_models.py` & `qq.py-1.2.8/qq/raw_models.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/reaction.py` & `qq.py-1.2.8/qq/reaction.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/role.py` & `qq.py-1.2.8/qq/role.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/schedule.py` & `qq.py-1.2.8/qq/schedule.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/shard.py` & `qq.py-1.2.8/qq/shard.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/state.py` & `qq.py-1.2.8/qq/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,15 +461,15 @@
         self._ready_task = asyncio.create_task(self._delay_ready())
 
     def parse_resumed(self, data) -> None:
         self.dispatch('resumed')
 
     def parse_at_message_create(self, data) -> None:
         channel, guild = self._get_guild_channel(data)
-        direct = True if 'direct_message' in data else False
+        direct = data['direct_message'] if 'direct_message' in data else False
         # channel would be the correct type here
         message = Message(channel=channel, data=data, state=self, direct=direct)  # type: ignore
         self.dispatch('message', message)
         if self._messages is not None:
             self._messages.append(message)
         # we ensure that the channel is either a TextChannel or Thread
         if channel and channel.__class__ in (TextChannel,):
```

### Comparing `qq.py-1.2.7/qq/types/audio.py` & `qq.py-1.2.8/qq/types/audio.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/channel.py` & `qq.py-1.2.8/qq/types/channel.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/embed.py` & `qq.py-1.2.8/qq/types/embed.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/emoji.py` & `qq.py-1.2.8/qq/types/emoji.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/guild.py` & `qq.py-1.2.8/qq/types/guild.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/member.py` & `qq.py-1.2.8/qq/types/member.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/message.py` & `qq.py-1.2.8/qq/types/message.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/permission.py` & `qq.py-1.2.8/qq/types/permission.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/raw_models.py` & `qq.py-1.2.8/qq/types/raw_models.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/role.py` & `qq.py-1.2.8/qq/types/role.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/schedule.py` & `qq.py-1.2.8/qq/types/schedule.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/types/user.py` & `qq.py-1.2.8/qq/types/user.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/user.py` & `qq.py-1.2.8/qq/user.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq/utils.py` & `qq.py-1.2.8/qq/utils.py`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/qq.py.egg-info/PKG-INFO` & `qq.py-1.2.8/qq.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qq.py
-Version: 1.2.7
+Version: 1.2.8
 Summary: QQ 频道 API 的 Python Wrapper
 Home-page: https://github.com/foxwhite25/qq.py
 Author: foxwhite25
 Author-email: vct.xie@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qq.py-1.2.7/qq.py.egg-info/SOURCES.txt` & `qq.py-1.2.8/qq.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qq.py-1.2.7/setup.py` & `qq.py-1.2.8/setup.py`

 * *Files identical despite different names*

