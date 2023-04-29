# Comparing `tmp/dpytest-0.6.4.tar.gz` & `tmp/dpytest-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpytest-0.6.4.tar", last modified: Mon Apr  3 11:58:05 2023, max compression
+gzip compressed data, was "dpytest-0.6.5.tar", last modified: Sat Apr 29 10:40:53 2023, max compression
```

## Comparing `dpytest-0.6.4.tar` & `dpytest-0.6.5.tar`

### file list

```diff
@@ -1,72 +1,75 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:05.950693 dpytest-0.6.4/
--rw-rw-rw-   0        0        0     1685 2023-04-03 11:55:58.000000 dpytest-0.6.4/HISTORY.md
--rw-rw-rw-   0        0        0     1102 2022-11-29 17:57:13.000000 dpytest-0.6.4/LICENSE
--rw-rw-rw-   0        0        0      228 2022-11-30 13:48:52.000000 dpytest-0.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3562 2023-04-03 11:58:05.950693 dpytest-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2022-12-11 11:03:48.000000 dpytest-0.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:04.056197 dpytest-0.6.4/discord/
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:04.057199 dpytest-0.6.4/discord/ext/
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:04.383915 dpytest-0.6.4/discord/ext/test/
--rw-rw-rw-   0        0        0      586 2023-04-03 11:57:46.000000 dpytest-0.6.4/discord/ext/test/__init__.py
--rw-rw-rw-   0        0        0      541 2023-01-13 14:54:07.000000 dpytest-0.6.4/discord/ext/test/_types.py
--rw-rw-rw-   0        0        0    40491 2023-04-03 09:36:38.000000 dpytest-0.6.4/discord/ext/test/backend.py
--rw-rw-rw-   0        0        0     1992 2022-11-29 17:57:13.000000 dpytest-0.6.4/discord/ext/test/callbacks.py
--rw-rw-rw-   0        0        0    19932 2023-03-01 08:27:49.000000 dpytest-0.6.4/discord/ext/test/factories.py
--rw-rw-rw-   0        0        0    13433 2023-01-13 14:57:38.000000 dpytest-0.6.4/discord/ext/test/runner.py
--rw-rw-rw-   0        0        0     2754 2023-01-13 15:00:31.000000 dpytest-0.6.4/discord/ext/test/state.py
--rw-rw-rw-   0        0        0     1870 2023-02-24 14:30:23.000000 dpytest-0.6.4/discord/ext/test/utils.py
--rw-rw-rw-   0        0        0    10242 2022-11-29 17:57:13.000000 dpytest-0.6.4/discord/ext/test/verify.py
--rw-rw-rw-   0        0        0     1605 2022-11-30 13:48:52.000000 dpytest-0.6.4/discord/ext/test/websocket.py
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:04.397453 dpytest-0.6.4/docs/
--rw-rw-rw-   0        0        0     2957 2023-04-03 11:57:46.000000 dpytest-0.6.4/docs/conf.py
--rw-rw-rw-   0        0        0      796 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:04.588994 dpytest-0.6.4/docs/modules/
--rw-rw-rw-   0        0        0       64 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/backend.rst
--rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/callbacks.rst
--rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/factories.rst
--rw-rw-rw-   0        0        0      171 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/index.rst
--rw-rw-rw-   0        0        0       61 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/runner.rst
--rw-rw-rw-   0        0        0       58 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/state.rst
--rw-rw-rw-   0        0        0       58 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/utils.rst
--rw-rw-rw-   0        0        0       61 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/verify.rst
--rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/modules/websocket.rst
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:04.845653 dpytest-0.6.4/docs/tutorials/
--rw-rw-rw-   0        0        0     1707 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/tutorials/getting_started.rst
--rw-rw-rw-   0        0        0      310 2022-11-29 17:57:13.000000 dpytest-0.6.4/docs/tutorials/index.rst
--rw-rw-rw-   0        0        0     5008 2022-11-30 13:48:52.000000 dpytest-0.6.4/docs/tutorials/using_pytest.rst
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:05.003752 dpytest-0.6.4/dpytest.egg-info/
--rw-rw-rw-   0        0        0     3562 2023-04-03 11:58:03.000000 dpytest-0.6.4/dpytest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-04-03 11:58:04.000000 dpytest-0.6.4/dpytest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 11:58:03.000000 dpytest-0.6.4/dpytest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-04-03 11:58:03.000000 dpytest-0.6.4/dpytest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 11:58:03.000000 dpytest-0.6.4/dpytest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      552 2023-04-03 11:58:05.953693 dpytest-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1944 2022-11-30 13:48:52.000000 dpytest-0.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:05.772565 dpytest-0.6.4/tests/
--rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.4/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2023-02-28 14:20:17.000000 dpytest-0.6.4/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:05.936694 dpytest-0.6.4/tests/data/
--rw-rw-rw-   0        0        0     3561 2022-11-29 17:57:13.000000 dpytest-0.6.4/tests/data/loremimpsum.txt
--rw-rw-rw-   0        0        0    48027 2022-11-29 17:57:13.000000 dpytest-0.6.4/tests/data/unit-tests.jpg
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:05.940696 dpytest-0.6.4/tests/internal/
--rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.4/tests/internal/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 11:58:05.948692 dpytest-0.6.4/tests/internal/cogs/
--rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.4/tests/internal/cogs/__init__.py
--rw-rw-rw-   0        0        0      330 2022-11-30 13:48:52.000000 dpytest-0.6.4/tests/internal/cogs/echo.py
--rw-rw-rw-   0        0        0      352 2022-11-30 13:48:52.000000 dpytest-0.6.4/tests/internal/cogs/greeting.py
--rw-rw-rw-   0        0        0      809 2022-11-30 10:51:57.000000 dpytest-0.6.4/tests/test_activity.py
--rw-rw-rw-   0        0        0      508 2022-11-30 11:00:30.000000 dpytest-0.6.4/tests/test_dmchannel.py
--rw-rw-rw-   0        0        0      552 2023-04-03 09:36:38.000000 dpytest-0.6.4/tests/test_edit.py
--rw-rw-rw-   0        0        0      442 2022-12-11 11:08:54.000000 dpytest-0.6.4/tests/test_fetch_message.py
--rw-rw-rw-   0        0        0     1800 2022-11-30 13:48:52.000000 dpytest-0.6.4/tests/test_get.py
--rw-rw-rw-   0        0        0      783 2022-11-30 10:51:13.000000 dpytest-0.6.4/tests/test_member.py
--rw-rw-rw-   0        0        0     1386 2022-11-30 11:00:21.000000 dpytest-0.6.4/tests/test_mentions.py
--rw-rw-rw-   0        0        0     1192 2023-01-13 15:03:51.000000 dpytest-0.6.4/tests/test_message.py
--rw-rw-rw-   0        0        0     2333 2022-12-05 09:09:54.000000 dpytest-0.6.4/tests/test_permissions.py
--rw-rw-rw-   0        0        0     1789 2022-11-30 10:51:19.000000 dpytest-0.6.4/tests/test_reactions.py
--rw-rw-rw-   0        0        0     1926 2023-01-13 14:55:26.000000 dpytest-0.6.4/tests/test_role.py
--rw-rw-rw-   0        0        0      509 2022-12-11 11:06:57.000000 dpytest-0.6.4/tests/test_send.py
--rw-rw-rw-   0        0        0     3102 2023-02-24 14:30:23.000000 dpytest-0.6.4/tests/test_utils.py
--rw-rw-rw-   0        0        0     1684 2022-11-30 13:48:52.000000 dpytest-0.6.4/tests/test_verify_embed.py
--rw-rw-rw-   0        0        0     1146 2022-11-30 10:51:30.000000 dpytest-0.6.4/tests/test_verify_file.py
--rw-rw-rw-   0        0        0     1675 2023-02-24 14:38:30.000000 dpytest-0.6.4/tests/test_verify_message.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.195425 dpytest-0.6.5/
+-rw-rw-rw-   0        0        0     1906 2023-04-29 10:38:51.000000 dpytest-0.6.5/HISTORY.md
+-rw-rw-rw-   0        0        0     1102 2022-11-29 17:57:13.000000 dpytest-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0      228 2022-11-30 13:48:52.000000 dpytest-0.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     5380 2023-04-29 10:40:53.197427 dpytest-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-04-20 13:50:15.000000 dpytest-0.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.825855 dpytest-0.6.5/discord/
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.826869 dpytest-0.6.5/discord/ext/
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.885619 dpytest-0.6.5/discord/ext/test/
+-rw-rw-rw-   0        0        0      586 2023-04-29 10:39:11.000000 dpytest-0.6.5/discord/ext/test/__init__.py
+-rw-rw-rw-   0        0        0      541 2023-01-13 14:54:07.000000 dpytest-0.6.5/discord/ext/test/_types.py
+-rw-rw-rw-   0        0        0    41717 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/backend.py
+-rw-rw-rw-   0        0        0     1992 2022-11-29 17:57:13.000000 dpytest-0.6.5/discord/ext/test/callbacks.py
+-rw-rw-rw-   0        0        0    20502 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/factories.py
+-rw-rw-rw-   0        0        0    14511 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/runner.py
+-rw-rw-rw-   0        0        0     3873 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/state.py
+-rw-rw-rw-   0        0        0     1870 2023-02-24 14:30:23.000000 dpytest-0.6.5/discord/ext/test/utils.py
+-rw-rw-rw-   0        0        0    10242 2022-11-29 17:57:13.000000 dpytest-0.6.5/discord/ext/test/verify.py
+-rw-rw-rw-   0        0        0     1355 2023-04-29 10:26:18.000000 dpytest-0.6.5/discord/ext/test/voice.py
+-rw-rw-rw-   0        0        0     1605 2022-11-30 13:48:52.000000 dpytest-0.6.5/discord/ext/test/websocket.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.897711 dpytest-0.6.5/docs/
+-rw-rw-rw-   0        0        0     2957 2023-04-29 10:39:11.000000 dpytest-0.6.5/docs/conf.py
+-rw-rw-rw-   0        0        0      796 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:52.978948 dpytest-0.6.5/docs/modules/
+-rw-rw-rw-   0        0        0       64 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/backend.rst
+-rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/callbacks.rst
+-rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/factories.rst
+-rw-rw-rw-   0        0        0      171 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/index.rst
+-rw-rw-rw-   0        0        0       61 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/runner.rst
+-rw-rw-rw-   0        0        0       58 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/state.rst
+-rw-rw-rw-   0        0        0       58 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/utils.rst
+-rw-rw-rw-   0        0        0       61 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/verify.rst
+-rw-rw-rw-   0        0        0       70 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/modules/websocket.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.016080 dpytest-0.6.5/docs/tutorials/
+-rw-rw-rw-   0        0        0     1707 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/tutorials/getting_started.rst
+-rw-rw-rw-   0        0        0      310 2022-11-29 17:57:13.000000 dpytest-0.6.5/docs/tutorials/index.rst
+-rw-rw-rw-   0        0        0     5008 2022-11-30 13:48:52.000000 dpytest-0.6.5/docs/tutorials/using_pytest.rst
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.080889 dpytest-0.6.5/dpytest.egg-info/
+-rw-rw-rw-   0        0        0     5380 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1493 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      111 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 10:40:52.000000 dpytest-0.6.5/dpytest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1534 2023-04-20 13:50:51.000000 dpytest-0.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0      514 2023-04-29 10:40:53.202427 dpytest-0.6.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.161428 dpytest-0.6.5/tests/
+-rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2023-02-28 14:20:17.000000 dpytest-0.6.5/tests/conftest.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.164428 dpytest-0.6.5/tests/data/
+-rw-rw-rw-   0        0        0     3561 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/data/loremimpsum.txt
+-rw-rw-rw-   0        0        0    48027 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/data/unit-tests.jpg
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.169467 dpytest-0.6.5/tests/internal/
+-rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/internal/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 10:40:53.194429 dpytest-0.6.5/tests/internal/cogs/
+-rw-rw-rw-   0        0        0        0 2022-11-29 17:57:13.000000 dpytest-0.6.5/tests/internal/cogs/__init__.py
+-rw-rw-rw-   0        0        0      330 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/internal/cogs/echo.py
+-rw-rw-rw-   0        0        0      352 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/internal/cogs/greeting.py
+-rw-rw-rw-   0        0        0      809 2022-11-30 10:51:57.000000 dpytest-0.6.5/tests/test_activity.py
+-rw-rw-rw-   0        0        0      948 2023-04-29 10:26:18.000000 dpytest-0.6.5/tests/test_create_channel.py
+-rw-rw-rw-   0        0        0      508 2022-11-30 11:00:30.000000 dpytest-0.6.5/tests/test_dmchannel.py
+-rw-rw-rw-   0        0        0      552 2023-04-03 09:36:38.000000 dpytest-0.6.5/tests/test_edit.py
+-rw-rw-rw-   0        0        0      442 2022-12-11 11:08:54.000000 dpytest-0.6.5/tests/test_fetch_message.py
+-rw-rw-rw-   0        0        0     1800 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/test_get.py
+-rw-rw-rw-   0        0        0      783 2022-11-30 10:51:13.000000 dpytest-0.6.5/tests/test_member.py
+-rw-rw-rw-   0        0        0     1386 2022-11-30 11:00:21.000000 dpytest-0.6.5/tests/test_mentions.py
+-rw-rw-rw-   0        0        0     1192 2023-01-13 15:03:51.000000 dpytest-0.6.5/tests/test_message.py
+-rw-rw-rw-   0        0        0     2333 2022-12-05 09:09:54.000000 dpytest-0.6.5/tests/test_permissions.py
+-rw-rw-rw-   0        0        0     1789 2022-11-30 10:51:19.000000 dpytest-0.6.5/tests/test_reactions.py
+-rw-rw-rw-   0        0        0     1926 2023-01-13 14:55:26.000000 dpytest-0.6.5/tests/test_role.py
+-rw-rw-rw-   0        0        0      509 2022-12-11 11:06:57.000000 dpytest-0.6.5/tests/test_send.py
+-rw-rw-rw-   0        0        0     3102 2023-02-24 14:30:23.000000 dpytest-0.6.5/tests/test_utils.py
+-rw-rw-rw-   0        0        0     1684 2022-11-30 13:48:52.000000 dpytest-0.6.5/tests/test_verify_embed.py
+-rw-rw-rw-   0        0        0     1146 2022-11-30 10:51:30.000000 dpytest-0.6.5/tests/test_verify_file.py
+-rw-rw-rw-   0        0        0     1675 2023-02-24 14:38:30.000000 dpytest-0.6.5/tests/test_verify_message.py
+-rw-rw-rw-   0        0        0      754 2023-04-29 10:26:18.000000 dpytest-0.6.5/tests/test_voice.py
```

### Comparing `dpytest-0.6.4/HISTORY.md` & `dpytest-0.6.5/HISTORY.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # History
 
+## 0.6.5
+
+This release allows testing with Voice Channels.
+
+New :
+
+- `FakeVoiceChannel` and `FakeVoiceClient` classes implemetation
+- New tests
+
+Changes :
+
+- `create_channel` method can create voice channel
+
 ## 0.6.4
 
 - Fix: edit message doesn't update message queue
 - Refactor __init__.py import to be explicit exports as per PEP 484
 
 ## 0.6.3
```

### Comparing `dpytest-0.6.4/LICENSE` & `dpytest-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/README.md` & `dpytest-0.6.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # dpytest
 
 [![Test CI](https://github.com/CraftSpider/dpytest/actions/workflows/test-ci.yml/badge.svg)](https://github.com/CraftSpider/dpytest/actions/workflows/test-ci.yml)
 [![Lint](https://github.com/CraftSpider/dpytest/actions/workflows/lint-ci.yml/badge.svg)](https://github.com/CraftSpider/dpytest/actions/workflows/lint-ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/dpytest/badge/?version=latest)](https://dpytest.readthedocs.io/en/latest/?badge=latest)
 [![Discord Server](https://img.shields.io/discord/523301176309972993.svg?label=Support%20Discord)](https://discord.gg/aNe8DqAuxd)
 
-
 This is a package to allow testing of discord.py.
 It is only compatible with the rewrite version, and is still in alpha.
 If using pytest, it is suggested to use pytest-asyncio for test running, otherwise the user will need
 to provide their own async test runner.
 
-# Notice
+## Notice
 
 For discord.py 1.7.X, use `dpytest 0.5.3`
 
 For discord.py 2.X.X, use `dpytest>=0.6`
 
-# Documentation
+## Documentation
 
 Documentation can be found at [dpytest.readthedocs.io](https://dpytest.readthedocs.io/en/latest/), including examples and tutorials
```

### Comparing `dpytest-0.6.4/discord/ext/test/__init__.py` & `dpytest-0.6.5/discord/ext/test/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 __title__ = "dpytest"
 __author__ = "Rune Tynan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2018-2019 CraftSpider"
-__version__ = "0.6.4"
+__version__ = "0.6.5"
 
 from . import backend as backend
 
 from .runner import *
 
 from .utils import embed_eq as embed_eq
 from .utils import activity_eq as activity_eq
```

### Comparing `dpytest-0.6.4/discord/ext/test/_types.py` & `dpytest-0.6.5/discord/ext/test/_types.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/discord/ext/test/backend.py` & `dpytest-0.6.5/discord/ext/test/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import asyncio
 import sys
 import logging
 import re
 import typing
 import datetime
+
 import discord
 import discord.http as dhttp
 import pathlib
 import urllib.parse
 import urllib.request
 
 from . import factories as facts, state as dstate, callbacks, websocket, _types
@@ -104,14 +105,17 @@
         perms = options.get("permission_overwrites", None)
         parent_id = options.get("parent_id", None)
 
         if channel_type == discord.ChannelType.text.value:
             channel = make_text_channel(name, guild, permission_overwrites=perms, parent_id=parent_id)
         elif channel_type == discord.ChannelType.category.value:
             channel = make_category_channel(name, guild, permission_overwrites=perms)
+        elif channel_type == discord.ChannelType.voice.value:
+            channel = make_voice_channel(name, guild, permission_overwrites=perms)
+
         else:
             raise NotImplementedError(
                 "Operation occurred that isn't captured by the tests framework. This is dpytest's fault, please report"
                 "an issue on github. Debug Info: only TextChannels and CategoryChannels are currently supported."
             )
         return facts.dict_from_channel(channel)
 
@@ -120,14 +124,16 @@
         channel = locs.get("self", None)
         if channel.type.value == discord.ChannelType.text.value:
             delete_channel(channel)
         if channel.type.value == discord.ChannelType.category.value:
             for sub_channel in channel.text_channels:
                 delete_channel(sub_channel)
             delete_channel(channel)
+        if channel.type.value == discord.ChannelType.voice.value:
+            delete_channel(channel)
 
     async def get_channel(self, channel_id: int) -> _types.JsonDict:
         await callbacks.dispatch_event("get_channel", channel_id)
 
         find = None
         for guild in _cur_config.state.guilds:
             for channel in guild.channels:
@@ -326,19 +332,21 @@
         me.nick = nickname
 
         await callbacks.dispatch_event("change_nickname", nickname, me, reason=reason)
 
         return {"nick": nickname}
 
     async def edit_member(self, guild_id: int, user_id: int, *, reason: typing.Optional[str] = None,
-                          **fields: typing.Any) -> None:
+                          **fields: typing.Any) -> _types.JsonDict:
         locs = _get_higher_locs(1)
         member = locs.get("self", None)
 
         await callbacks.dispatch_event("edit_member", fields, member, reason=reason)
+        member = update_member(member, nick=fields.get('nick'), roles=fields.get('roles'))
+        return facts.dict_from_member(member)
 
     async def get_member(self, guild_id: int, member_id: int) -> _types.JsonDict:
         locs = _get_higher_locs(1)
         guild = locs.get("self", None)
         member = discord.utils.get(guild.members, id=member_id)
 
         return facts.dict_from_member(member)
@@ -731,14 +739,36 @@
                                               permission_overwrites=permission_overwrites)
     state = get_state()
     state.parse_channel_create(c_dict)
 
     return guild.get_channel(c_dict["id"])
 
 
+def make_voice_channel(
+        name: str,
+        guild: discord.Guild,
+        position: int = -1,
+        id_num: int = -1,
+        permission_overwrites: typing.Optional[_types.JsonDict] = None,
+        parent_id: typing.Optional[int] = None,
+        bitrate: int = 192,
+        user_limit: int = 0
+
+) -> discord.VoiceChannel:
+    if position == -1:
+        position = len(guild.voice_channels) + 1
+    c_dict = facts.make_voice_channel_dict(name, id_num, position=position, guild_id=guild.id,
+                                           permission_overwrites=permission_overwrites, parent_id=parent_id,
+                                           bitrate=bitrate, user_limit=user_limit)
+    state = get_state()
+    state.parse_channel_create(c_dict)
+
+    return guild.get_channel(c_dict["id"])
+
+
 def delete_channel(channel: _types.AnyChannel) -> None:
     c_dict = facts.make_text_channel_dict(channel.name, id_num=channel.id, guild_id=channel.guild.id)
 
     state = get_state()
     state.parse_channel_delete(c_dict)
```

### Comparing `dpytest-0.6.4/discord/ext/test/callbacks.py` & `dpytest-0.6.5/discord/ext/test/callbacks.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/discord/ext/test/factories.py` & `dpytest-0.6.5/discord/ext/test/factories.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import typing
 import datetime as dt
 import discord
 from . import _types
 
+
 generated_ids: int = 0
 
 
 def make_id() -> int:
     global generated_ids
     # timestamp
     discord_epoch = str(bin(int(dt.datetime.now().timestamp() * 1000) - 1420070400000))[2:]
@@ -261,14 +262,18 @@
     return make_channel_dict(discord.ChannelType.category.value, id_num, name=name, **kwargs)
 
 
 def make_dm_channel_dict(user: discord.User, id_num: int = -1, **kwargs: typing.Any) -> _types.JsonDict:
     return make_channel_dict(discord.ChannelType.private, id_num, recipients=[dict_from_user(user)], **kwargs)
 
 
+def make_voice_channel_dict(name: str, id_num: int = -1, **kwargs: typing.Any) -> _types.JsonDict:
+    return make_channel_dict(discord.ChannelType.voice.value, id_num, name=name, **kwargs)
+
+
 def dict_from_overwrite(target: typing.Union[discord.Member, discord.Role],
                         overwrite: discord.PermissionOverwrite) -> _types.JsonDict:
     allow, deny = overwrite.pair()
     ovr = {
         'id': target.id,
         'allow': allow.value,
         'deny': deny.value,
@@ -298,14 +303,23 @@
         return {
             'name': channel.name,
             'position': channel.position,
             'id': channel.id,
             'guild_id': channel.guild.id,
             'permission_overwrites': [dict_from_overwrite(k, v) for k, v in channel.overwrites.items()],
             'type': channel.type
+        }
+    if isinstance(channel, discord.VoiceChannel):
+        return {
+            'name': channel.name,
+            'position': channel.position,
+            'id': channel.id,
+            'guild_id': channel.guild.id,
+            'permission_overwrites': [dict_from_overwrite(k, v) for k, v in channel.overwrites.items()],
+            'type': channel.type
         }
 
 
 @typing.overload
 def make_message_dict(
         channel: _types.AnyChannel,
         author: discord.user.BaseUser,
```

### Comparing `dpytest-0.6.4/discord/ext/test/runner.py` & `dpytest-0.6.5/discord/ext/test/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
     All public functions in this module are re-exported at ``discord.ext.test``, this is the primary
     entry point for users of the library and most of what they should interact with
 
     See also:
         :mod:`discord.ext.test.verify`
 """
 
-
 import sys
 import asyncio
 import logging
 import discord
 import typing
 import pathlib
 
@@ -45,19 +44,21 @@
     """
         Decorator to enforce that configuration is completed before the decorated function is
         called.
 
     :param func: Function to decorate
     :return: Function with added check for configuration being setup
     """
+
     def wrapper(*args, **kwargs):
         if _cur_config is None:
             log.error("Attempted to make call before runner configured")
             raise RuntimeError(f"Configure runner before calling {func.__name__}")
         return func(*args, **kwargs)
+
     wrapper.__wrapped__ = func
     wrapper.__annotations__ = func.__annotations__
     wrapper.__doc__ = func.__doc__
     return wrapper
 
 
 async def run_all_events() -> None:
@@ -137,14 +138,30 @@
         Internal callback, on a message being sent (in any channel) adds it to the queue
 
     :param message: Message sent on discord
     """
     await sent_queue.put(message)
 
 
+async def _edit_member_callback(fields: typing.Any, member: discord.Member, reason: typing.Optional[str]):
+    """
+        Internal callback. Updates a guild's voice states to reflect the given Member connecting to the given channel.
+        Other updates to members are handled in http.edit_member().
+
+    :param fields: Fields passed in from Member.edit().
+    :param member: The Member to edit.
+    :param reason: The reason for editing. Not used.
+    """
+    data = {'user_id': member.id}
+    guild = member.guild
+    channel = fields.get('channel_id')
+    if not fields.get('nick') and not fields.get('roles'):
+        guild._update_voice_state(data, channel)
+
+
 counter = count(0)
 
 
 @require_config
 async def message(
         content: str,
         channel: typing.Union[_types.AnyChannel, int] = 0,
@@ -327,21 +344,23 @@
         Get the current runner configuration
 
     :return: Current runner config
     """
     return _cur_config
 
 
-def configure(client: discord.Client, num_guilds: int = 1, num_channels: int = 1, num_members: int = 1) -> None:
+def configure(client: discord.Client, num_guilds: int = 1, num_text_channels: int = 1,
+              num_voice_channels: int = 1, num_members: int = 1) -> None:
     """
         Set up the runner configuration. This should be done before any tests are run.
 
     :param client: Client to configure with. Should be the bot/client that is going to be tested.
     :param num_guilds: Number of guilds to start the configuration with. Default is 1
-    :param num_channels: Number of text channels in each guild to start with. Default is 1
+    :param num_text_channels: Number of text channels in each guild to start with. Default is 1
+    :param num_voice_channels: Number of voice channels in each guild to start with. Default is 1.
     :param num_members: Number of members in each guild (other than the client) to start with. Default is 1.
     """
 
     global _cur_config
 
     if not isinstance(client, discord.Client):
         raise TypeError("Runner client must be an instance of discord.Client")
@@ -363,30 +382,34 @@
             await error_queue.put((ctx, error))
 
     on_command_error.__old__ = old_error
     client.on_command_error = on_command_error
 
     # Configure global callbacks
     callbacks.set_callback(_message_callback, "send_message")
+    callbacks.set_callback(_edit_member_callback, "edit_member")
 
     back.get_state().stop_dispatch()
 
     guilds = []
     for num in range(num_guilds):
         guild = back.make_guild(f"Test Guild {num}")
         guilds.append(guild)
 
     channels = []
     members = []
     for guild in guilds:
-        for num in range(num_channels):
-            channel = back.make_text_channel(f"Channel_{num}", guild)
+        for num in range(num_text_channels):
+            channel = back.make_text_channel(f"TextChannel_{num}", guild)
+            channels.append(channel)
+        for num in range(num_voice_channels):
+            channel = back.make_voice_channel(f"VoiceChannel_{num}", guild)
             channels.append(channel)
         for num in range(num_members):
-            user = back.make_user(f"TestUser{str(num)}", f"{num+1:04}")
+            user = back.make_user(f"TestUser{str(num)}", f"{num + 1:04}")
             member = back.make_member(user, guild, nick=user.name + f"_{str(num)}_nick")
             members.append(member)
         back.make_member(back.get_state().user, guild, nick=client.user.name + "_nick")
 
     back.get_state().start_dispatch()
 
     _cur_config = RunnerConfig(client, guilds, channels, members)
```

### Comparing `dpytest-0.6.4/discord/ext/test/state.py` & `dpytest-0.6.5/discord/ext/test/state.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import typing
 import discord
 import discord.http as dhttp
 import discord.state as dstate
 
 from . import factories as facts
 from . import backend as back
+from .voice import FakeVoiceChannel
 
 
 class FakeState(dstate.ConnectionState):
     """
         A mock implementation of a ``ConnectionState``. Overrides methods that would otherwise cause issues, and
         implements functionality such as disabling dispatch temporarily.
     """
@@ -33,14 +34,15 @@
         if user is None:
             user = discord.ClientUser(state=self, data=facts.make_user_dict("FakeApp", "0001", None))
             user.bot = True
         self.user = user
         self.shard_count = client.shard_count
         self._get_websocket = lambda x: client.ws
         self._do_dispatch = True
+        self._get_client = lambda: client
 
         real_disp = self.dispatch
 
         def dispatch(*args, **kwargs):
             if not self._do_dispatch:
                 return
             return real_disp(*args, **kwargs)
@@ -69,7 +71,32 @@
         pass
 
     def _guild_needs_chunking(self, guild: discord.Guild):
         """
         Prevents chunking which can throw asyncio wait_for errors with tests under 60 seconds
         """
         return False
+
+    def parse_channel_create(self, data) -> None:
+        """
+        Need to make sure that FakeVoiceChannels are created when this is called to create VoiceChannels. Otherwise,
+        guilds would not be set up correctly.
+
+        :param data: info to use in channel creation.
+        """
+        if data['type'] == discord.ChannelType.voice.value:
+            factory, ch_type = FakeVoiceChannel, discord.ChannelType.voice.value
+        else:
+            factory, ch_type = discord.channel._channel_factory(data['type'])
+
+        if factory is None:
+            return
+
+        guild_id = discord.utils._get_as_snowflake(data, 'guild_id')
+        guild = self._get_guild(guild_id)
+        if guild is not None:
+            # the factory can't be a DMChannel or GroupChannel here
+            channel = factory(guild=guild, state=self, data=data)  # type: ignore
+            guild._add_channel(channel)  # type: ignore
+            self.dispatch('guild_channel_create', channel)
+        else:
+            return
```

### Comparing `dpytest-0.6.4/discord/ext/test/utils.py` & `dpytest-0.6.5/discord/ext/test/utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/discord/ext/test/verify.py` & `dpytest-0.6.5/discord/ext/test/verify.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/discord/ext/test/websocket.py` & `dpytest-0.6.5/discord/ext/test/websocket.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/docs/conf.py` & `dpytest-0.6.5/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'dpytest'
 copyright = '2020, CraftSpider'
 author = 'CraftSpider'
 
 # The full version, including alpha/beta/rc tags
-release = '0.6.4'
+release = '0.6.5'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `dpytest-0.6.4/docs/index.rst` & `dpytest-0.6.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/docs/tutorials/getting_started.rst` & `dpytest-0.6.5/docs/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/docs/tutorials/using_pytest.rst` & `dpytest-0.6.5/docs/tutorials/using_pytest.rst`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/dpytest.egg-info/SOURCES.txt` & `dpytest-0.6.5/dpytest.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
-setup.py
 discord/ext/test/__init__.py
 discord/ext/test/_types.py
 discord/ext/test/backend.py
 discord/ext/test/callbacks.py
 discord/ext/test/factories.py
 discord/ext/test/runner.py
 discord/ext/test/state.py
 discord/ext/test/utils.py
 discord/ext/test/verify.py
+discord/ext/test/voice.py
 discord/ext/test/websocket.py
 docs/conf.py
 docs/index.rst
 docs/modules/backend.rst
 docs/modules/callbacks.rst
 docs/modules/factories.rst
 docs/modules/index.rst
@@ -32,14 +33,15 @@
 dpytest.egg-info/SOURCES.txt
 dpytest.egg-info/dependency_links.txt
 dpytest.egg-info/requires.txt
 dpytest.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_activity.py
+tests/test_create_channel.py
 tests/test_dmchannel.py
 tests/test_edit.py
 tests/test_fetch_message.py
 tests/test_get.py
 tests/test_member.py
 tests/test_mentions.py
 tests/test_message.py
@@ -47,13 +49,14 @@
 tests/test_reactions.py
 tests/test_role.py
 tests/test_send.py
 tests/test_utils.py
 tests/test_verify_embed.py
 tests/test_verify_file.py
 tests/test_verify_message.py
+tests/test_voice.py
 tests/data/loremimpsum.txt
 tests/data/unit-tests.jpg
 tests/internal/__init__.py
 tests/internal/cogs/__init__.py
 tests/internal/cogs/echo.py
 tests/internal/cogs/greeting.py
```

### Comparing `dpytest-0.6.4/setup.py` & `dpytest-0.6.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-
-import setuptools
-import re
-
-with open("discord/ext/test/__init__.py", "r") as file:
-    try:
-        version = re.search(r"^__version__\s*=\s*[\"']([^\"']*)[\"']", file.read(), re.MULTILINE).group(1)
-    except Exception as e:
-        raise RuntimeError("Version isn't set")
-
-if version.endswith(("a", "b")):
-    try:
-        import subprocess as sp
-        p = sp.Popen(["git", "rev-list", "--count", "HEAD"], stdout=sp.PIPE, stderr=sp.PIPE)
-        out, err = p.communicate()
-        if out:
-            version += out.decode("utf-8").strip()
-        p = sp.Popen(["git", "rev-parse", "--short", "HEAD"], stdout=sp.PIPE, stderr=sp.PIPE)
-        out, err = p.communicate()
-        if out:
-            version += "+g" + out.decode("utf-8").strip()
-    except Exception as e:
-        raise RuntimeError("Failure to get current git commit")
-
-with open("README.md", "r") as readme_file:
-    readme = readme_file.read()
-
-with open('HISTORY.md', "r") as history_file:
-    history = history_file.read()
-
-setuptools.setup(
-    name="dpytest",
-    version=version,
-    author="Rune Tynan",
-    author_email="runetynan@gmail.com",
-    description="A package that assists in writing tests for discord.py",
-    long_description=readme + '\n\n' + history,
-    long_description_content_type="text/markdown",
-    url="https://github.com/CraftSpider/dpytest",
-    packages=["discord.ext.test"],
-    classifiers=[
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Development Status :: 3 - Alpha",
-        "Topic :: Software Development :: Testing"
-    ],
-    keywords="discord discord.py test",
-    install_requires=["discord.py", "pytest-asyncio"]
-)
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "dpytest"
+authors = [{name = "Rune Tynan", email = "runetynan@gmail.com"},]
+maintainers = [{name = "CraftSpider"},
+               {name = "Sergeileduc"}]
+description = "A package that assists in writing tests for discord.py"
+dynamic = ["readme", "version"]
+license = {file = "LICENSE"}
+requires-python = ">=3.8"
+keywords = ["discord", "discord.py", "test"]
+classifiers = [
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Development Status :: 3 - Alpha",
+    "Topic :: Software Development :: Testing",
+]
+
+dependencies = [
+    "discord.py == 2.2.2",
+    "pytest",
+    "pytest-asyncio",
+]
+
+[project.optional-dependencies]
+test = ["pytest", "pytest-asyncio"]
+doc = ["sphinx"]
+dev = ["flake8", "invoke", "build"]
+
+[project.urls]
+"Homepage" = "https://github.com/CraftSpider/dpytest"
+"Source" = "https://github.com/CraftSpider/dpytest"
+"Bug Tracker" = "https://github.com/CraftSpider/dpytest/issues"
+"Documentation" = "https://dpytest.readthedocs.io/"
+
+[tool.setuptools]
+packages = ["discord.ext.test"]
+
+[tool.setuptools.dynamic]
+readme = {file = ["README.md", "HISTORY.md"], content-type = "text/markdown"}
+version = {attr = "discord.ext.test.__version__"}
```

### Comparing `dpytest-0.6.4/tests/conftest.py` & `dpytest-0.6.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/data/loremimpsum.txt` & `dpytest-0.6.5/tests/data/loremimpsum.txt`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/data/unit-tests.jpg` & `dpytest-0.6.5/tests/data/unit-tests.jpg`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_activity.py` & `dpytest-0.6.5/tests/test_activity.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_edit.py` & `dpytest-0.6.5/tests/test_edit.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_get.py` & `dpytest-0.6.5/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_member.py` & `dpytest-0.6.5/tests/test_member.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_mentions.py` & `dpytest-0.6.5/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_message.py` & `dpytest-0.6.5/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_permissions.py` & `dpytest-0.6.5/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_reactions.py` & `dpytest-0.6.5/tests/test_reactions.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_role.py` & `dpytest-0.6.5/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_utils.py` & `dpytest-0.6.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_verify_embed.py` & `dpytest-0.6.5/tests/test_verify_embed.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_verify_file.py` & `dpytest-0.6.5/tests/test_verify_file.py`

 * *Files identical despite different names*

### Comparing `dpytest-0.6.4/tests/test_verify_message.py` & `dpytest-0.6.5/tests/test_verify_message.py`

 * *Files identical despite different names*

