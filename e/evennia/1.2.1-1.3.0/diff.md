# Comparing `tmp/evennia-1.2.1.tar.gz` & `tmp/evennia-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evennia-1.2.1.tar", last modified: Sun Feb 26 19:23:20 2023, max compression
+gzip compressed data, was "evennia-1.3.0.tar", last modified: Sat Apr 29 06:52:56 2023, max compression
```

## Comparing `evennia-1.2.1.tar` & `evennia-1.3.0.tar`

### file list

```diff
@@ -1,953 +1,953 @@
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.528069 evennia-1.2.1/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2022-12-17 18:42:26.000000 evennia-1.2.1/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-02-26 19:23:20.524069 evennia-1.2.1/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3027 2022-12-21 16:00:31.000000 evennia-1.2.1/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.468069 evennia-1.2.1/bin/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/bin/unix/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2022-12-17 18:42:26.000000 evennia-1.2.1/bin/unix/evennia
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2023-02-26 19:19:48.000000 evennia-1.2.1/evennia/VERSION.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      438 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/VERSION_REQS.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12647 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/__main__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.476069 evennia-1.2.1/evennia/accounts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    67784 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26733 2023-01-25 17:38:44.000000 evennia-1.2.1/evennia/accounts/bots.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.476069 evennia-1.2.1/evennia/accounts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0002_move_defaults.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0003_auto_20150209_2234.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0004_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0005_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0007_copy_player_to_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0008_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0009_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0010_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16624 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/accounts/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.476069 evennia-1.2.1/evennia/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.476069 evennia-1.2.1/evennia/commands/_trial_temp/
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/_trial_temp/_trial_marker
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31705 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/cmdhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27219 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/cmdset.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26152 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/cmdsethandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29198 2023-02-26 19:05:50.000000 evennia-1.2.1/evennia/commands/command.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.476069 evennia-1.2.1/evennia/commands/default/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37421 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/commands/default/account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19595 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/commands/default/admin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23003 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/batchprocess.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   167200 2023-02-26 13:59:37.000000 evennia-1.2.1/evennia/commands/default/building.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/cmdset_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/cmdset_character.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/cmdset_session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/cmdset_unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    76171 2023-02-25 08:05:28.000000 evennia-1.2.1/evennia/commands/default/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22494 2023-01-25 17:38:34.000000 evennia-1.2.1/evennia/commands/default/general.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39551 2023-02-26 15:55:33.000000 evennia-1.2.1/evennia/commands/default/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12788 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/muxcommand.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/syscommands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41884 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/commands/default/system.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    81813 2023-02-25 23:10:03.000000 evennia-1.2.1/evennia/commands/default/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17440 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/commands/default/unloggedin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46641 2023-02-26 19:06:44.000000 evennia-1.2.1/evennia/commands/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.476069 evennia-1.2.1/evennia/comms/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32556 2023-02-25 23:09:58.000000 evennia-1.2.1/evennia/comms/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2023-01-15 12:57:07.000000 evennia-1.2.1/evennia/comms/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/comms/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0003_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0004_auto_20150118_1631.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0005_auto_20150223_1517.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0007_msg_db_tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0008_auto_20160905_0902.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0009_auto_20160921_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0010_auto_20161206_1912.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0011_auto_20170217_2039.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0011_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0012_merge_20170617_2017.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0013_auto_20170705_1726.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0014_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0015_auto_20170706_2041.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0016_auto_20180925_1735.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0017_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0018_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0019_auto_20210514_2032.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0020_auto_20210514_2210.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0021_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22638 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/comms/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2023-02-25 23:09:58.000000 evennia-1.2.1/evennia/comms/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/awsstorage/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2023-01-15 12:43:20.000000 evennia-1.2.1/evennia/contrib/base_systems/awsstorage/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/awsstorage/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/awsstorage/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/building_menu/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/building_menu/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/building_menu/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42659 2023-02-26 11:16:24.000000 evennia-1.2.1/evennia/contrib/base_systems/building_menu/building_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6878 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/building_menu/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/color_markups/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/color_markups/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/color_markups/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/color_markups/color_markups.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/color_markups/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/components/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6344 2022-12-23 15:43:18.000000 evennia-1.2.1/evennia/contrib/base_systems/components/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/components/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3915 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/components/component.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3762 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/components/dbfield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11021 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/components/holder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7237 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/components/signals.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14129 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/components/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/email_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/email_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/email_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/email_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10264 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/email_login/email_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/email_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.480069 evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8938 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/webclient.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40308 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/callbackhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/eventfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/ingame_python/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/base_systems/menu_login/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/menu_login/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/menu_login/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/menu_login/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8781 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/menu_login/menu_login.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/menu_login/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/base_systems/unixcommand/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/unixcommand/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/unixcommand/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/unixcommand/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/base_systems/unixcommand/unixcommand.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/full_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22699 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10565 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34348 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      753 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/state.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/states/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/states/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10461 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/barter/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/barter/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/barter/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/barter/barter.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/barter/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/clothing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4249 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/clothing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/clothing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24573 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/clothing/clothing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4816 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/clothing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/cooldowns/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/cooldowns/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/cooldowns/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/cooldowns/cooldowns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/cooldowns/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/crafting/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2022-12-23 15:43:18.000000 evennia-1.2.1/evennia/contrib/game_systems/crafting/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/crafting/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41599 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/contrib/game_systems/crafting/crafting.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17892 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/crafting/example_recipes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/crafting/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/gendersub/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/gendersub/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/gendersub/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5096 2023-01-15 22:08:02.000000 evennia-1.2.1/evennia/contrib/game_systems/gendersub/gendersub.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1091 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/gendersub/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/mail/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/mail/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/mail/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/mail/mail.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/mail/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/multidescer/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      932 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/multidescer/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/multidescer/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/multidescer/multidescer.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/multidescer/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.484069 evennia-1.2.1/evennia/contrib/game_systems/puzzles/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/puzzles/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/puzzles/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27837 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/puzzles/puzzles.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41328 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/puzzles/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28734 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_basic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_equip.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37446 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_items.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_magic.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_range.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29682 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/extended_room/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3172 2022-12-21 16:00:35.000000 evennia-1.2.1/evennia/contrib/grid/extended_room/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      384 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/extended_room/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/contrib/grid/extended_room/extended_room.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4793 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/contrib/grid/extended_room/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/ingame_map_display/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2022-12-23 15:43:18.000000 evennia-1.2.1/evennia/contrib/grid/ingame_map_display/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/ingame_map_display/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/ingame_map_display/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/mapbuilder/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/mapbuilder/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/mapbuilder/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/mapbuilder/mapbuilder.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/mapbuilder/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/simpledoor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/simpledoor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/simpledoor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/simpledoor/simpledoor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/simpledoor/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/slow_exit/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/slow_exit/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/slow_exit/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/slow_exit/slow_exit.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/slow_exit/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/wilderness/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4567 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/wilderness/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/wilderness/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6026 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/wilderness/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28578 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/wilderness/wilderness.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/grid/xyzgrid/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54690 2023-01-28 17:46:43.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      202 2022-12-23 15:44:29.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20837 2023-01-28 17:46:43.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7822 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13723 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/launchcmd.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42072 2023-01-28 17:46:43.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    40413 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/xymap.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    52070 2023-02-25 19:48:13.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/xymap_legend.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2023-01-28 21:36:35.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/xyzgrid.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24616 2023-01-28 17:46:43.000000 evennia-1.2.1/evennia/contrib/grid/xyzgrid/xyzroom.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/rpg/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.488069 evennia-1.2.1/evennia/contrib/rpg/buffs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/buffs/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/buffs/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    45607 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/buffs/buff.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/buffs/samplebuffs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/buffs/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/rpg/character_creator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/character_creator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/character_creator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/character_creator/character_creator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/character_creator/example_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1552 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/character_creator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/rpg/dice/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/dice/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/dice/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10272 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/dice/dice.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      901 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/dice/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/rpg/health_bar/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/health_bar/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/health_bar/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/health_bar/health_bar.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/health_bar/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/rpg/rpsystem/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9938 2022-12-23 15:43:18.000000 evennia-1.2.1/evennia/contrib/rpg/rpsystem/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/rpsystem/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/rpsystem/rplanguage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65825 2023-02-26 11:08:59.000000 evennia-1.2.1/evennia/contrib/rpg/rpsystem/rpsystem.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14981 2023-02-26 11:08:52.000000 evennia-1.2.1/evennia/contrib/rpg/rpsystem/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/rpg/traits/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14246 2023-01-15 12:47:59.000000 evennia-1.2.1/evennia/contrib/rpg/traits/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/traits/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/traits/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    54252 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/rpg/traits/traits.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/tutorials/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/tutorials/evadventure/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1183 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/build_techdemo.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/build_world.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12557 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11187 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    48197 2023-01-28 21:30:36.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/combat_turnbased.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13739 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17844 2022-12-21 16:23:28.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1533 2023-01-28 21:30:36.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/enums.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14381 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11894 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/npcs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6614 2023-01-28 21:30:36.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/random_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2983 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13120 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/shops.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2151 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12871 2023-01-28 21:30:36.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_combat.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4159 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_commands.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_quests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_rules.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      712 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/evadventure/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.492069 evennia-1.2.1/evennia/contrib/tutorials/mirror/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/mirror/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/mirror/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/mirror/mirror.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/tutorials/red_button/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2022-12-23 15:43:18.000000 evennia-1.2.1/evennia/contrib/tutorials/red_button/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/red_button/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/red_button/red_button.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/tutorials/talking_npc/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/talking_npc/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/talking_npc/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/talking_npc/talking_npc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/talking_npc/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2022-12-23 15:43:18.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/build.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25293 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/intro_menu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/mob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7342 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/auditing/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/auditing/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/auditing/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/auditing/outputs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/auditing/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6023 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/auditing/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/fieldfill/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/fieldfill/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/fieldfill/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26404 2023-01-06 18:10:32.000000 evennia-1.2.1/evennia/contrib/utils/fieldfill/fieldfill.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/git_integration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2023-01-15 12:45:26.000000 evennia-1.2.1/evennia/contrib/utils/git_integration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/git_integration/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7743 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/git_integration/git_integration.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/git_integration/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/name_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/name_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/name_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/name_generator/btn_givennames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/name_generator/btn_surnames.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/name_generator/namegen.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/name_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/random_string_generator/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/random_string_generator/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/random_string_generator/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/random_string_generator/random_string_generator.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/random_string_generator/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/contrib/utils/tree_select/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/tree_select/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/tree_select/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/tree_select/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/contrib/utils/tree_select/tree_select.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/game_template/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/game_template/commands/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/commands/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/commands/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/commands/command.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/commands/default_cmdsets.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/gitignore
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.496069 evennia-1.2.1/evennia/game_template/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/server/conf/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/at_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/at_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/at_server_startstop.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/cmdparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/connection_screens.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/inlinefuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4009 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/portal_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/secret_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/server_services_plugins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/conf/web_plugins.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/server/logs/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/server/logs/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1525 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/exits.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/rooms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/typeclasses/scripts.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      297 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/admin/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/admin/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/api/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/game_template/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/rest_framework/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/rest_framework/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/game_template/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/webclient/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/webclient/js/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/game_template/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/website/css/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/static/website/images/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/templates/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/templates/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/templates/rest_framework/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/templates/webclient/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/templates/website/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/templates/website/flatpages/README.md
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/templates/website/registration/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1105 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/webclient/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/webclient/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/website/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/web/website/views/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/game_template/world/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/world/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/world/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/world/batch_cmds.ev
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2186 2022-12-21 16:00:35.000000 evennia-1.2.1/evennia/game_template/world/help_entries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/game_template/world/prototypes.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/help/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/filehelp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/help/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/0002_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/0003_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/0004_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/0005_auto_20210530_1818.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/0006_alter_helpentry_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7673 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/help/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.500069 evennia-1.2.1/evennia/locale/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/README
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/de/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/de/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/de/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/es/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/es/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/es/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/fr/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2022-12-23 15:32:25.000000 evennia-1.2.1/evennia/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2022-12-23 15:31:00.000000 evennia-1.2.1/evennia/locale/fr/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/it/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/it/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/it/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/ko/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/ko/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/ko/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/ko/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/la/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/la/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/la/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/la/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/pl/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/pt/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/pt/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/pt/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/pt/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/ru/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/sv/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/sv/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/sv/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/sv/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/locale/zh/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locale/zh/LC_MESSAGES/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/zh/LC_MESSAGES/django.mo
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locale/zh/LC_MESSAGES/django.po
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/locks/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locks/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21852 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locks/lockfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    26966 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locks/lockhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/locks/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/objects/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29704 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.504069 evennia-1.2.1/evennia/objects/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0002_auto_20140917_0756.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0004_auto_20150118_1622.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0005_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0006_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0007_objectdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0008_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0009_remove_objectdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0010_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0011_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13399 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   119132 2023-02-25 18:01:10.000000 evennia-1.2.1/evennia/objects/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14391 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/objects/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.508069 evennia-1.2.1/evennia/prototypes/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/prototypes/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/prototypes/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    92110 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/prototypes/menus.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2023-02-26 09:41:36.000000 evennia-1.2.1/evennia/prototypes/protfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    46545 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/prototypes/prototypes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    42860 2023-02-26 14:15:03.000000 evennia-1.2.1/evennia/prototypes/spawner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    39636 2023-02-26 13:58:53.000000 evennia-1.2.1/evennia/prototypes/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.508069 evennia-1.2.1/evennia/scripts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.508069 evennia-1.2.1/evennia/scripts/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0002_auto_20150118_1625.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0004_auto_20150306_1354.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0005_auto_20150306_1441.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0006_auto_20150310_2249.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0007_auto_20150403_2339.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0008_auto_20170606_1731.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0009_scriptdb_db_account.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0010_auto_20170705_1736.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0012_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0013_auto_20191025_0831.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0014_auto_20210520_2137.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0015_convert_contrib_paths.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8746 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/monitorhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4987 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/scripthandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27442 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20801 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/taskhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3133 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24704 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/scripts/tickerhandler.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.508069 evennia-1.2.1/evennia/server/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8697 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/amp_client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16629 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/connection_wizard.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7955 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/deprecations.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    79833 2022-12-23 16:12:03.000000 evennia-1.2.1/evennia/server/evennia_launcher.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.508069 evennia-1.2.1/evennia/server/game_index_client/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/game_index_client/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/game_index_client/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6277 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/game_index_client/client.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1990 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/game_index_client/service.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7647 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    19709 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/inputfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1708 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/manager.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.508069 evennia-1.2.1/evennia/server/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/migrations/0002_auto_20190128_2311.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/migrations/0003_alter_serverconfig_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/models.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.512069 evennia-1.2.1/evennia/server/portal/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/amp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17520 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/amp_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18478 2023-01-28 17:46:43.000000 evennia-1.2.1/evennia/server/portal/discord.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11345 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/grapevine.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/irc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/mccp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/mssp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/mxp.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/naws.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    16002 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/portal.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17231 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/portalsessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/rss.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15788 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/ssh.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/suppress_ga.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2023-02-26 15:53:58.000000 evennia-1.2.1/evennia/server/portal/telnet.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/telnet_oob.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4861 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/telnet_ssl.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14725 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6991 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/ttype.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11265 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/webclient.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/portal/webclient_ajax.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.512069 evennia-1.2.1/evennia/server/profiling/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    20881 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/dummyrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/dummyrunner_settings.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/memplot.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/settings_mixin.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1095 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/test_queries.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/profiling/timetrace.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28629 2023-02-25 08:05:28.000000 evennia-1.2.1/evennia/server/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14599 2023-02-26 13:41:06.000000 evennia-1.2.1/evennia/server/serversession.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/session.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30190 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/sessionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4962 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/signals.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.512069 evennia-1.2.1/evennia/server/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/tests/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4721 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/tests/test_amp_connection.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/tests/test_initial_setup.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2022-12-21 16:00:31.000000 evennia-1.2.1/evennia/server/tests/test_launcher.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4444 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/tests/test_misc.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9256 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/tests/test_server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/tests/testrunner.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/throttle.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2776 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/validators.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/server/webserver.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    60835 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/settings_default.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.512069 evennia-1.2.1/evennia/typeclasses/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    64065 2023-02-25 19:19:18.000000 evennia-1.2.1/evennia/typeclasses/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/managers.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.512069 evennia-1.2.1/evennia/typeclasses/migrations/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0001_initial.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0015_alter_attribute_options.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/migrations/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    37091 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/typeclasses/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    25077 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/typeclasses/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    17813 2023-02-25 07:45:02.000000 evennia-1.2.1/evennia/typeclasses/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.516069 evennia-1.2.1/evennia/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    50819 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8077 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/create.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    32502 2022-12-21 16:00:31.000000 evennia-1.2.1/evennia/utils/dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/evennia-mode.el
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21081 2023-01-07 19:57:45.000000 evennia-1.2.1/evennia/utils/evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    78095 2022-12-21 16:00:31.000000 evennia-1.2.1/evennia/utils/evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18330 2023-02-26 16:32:12.000000 evennia-1.2.1/evennia/utils/evmore.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    65173 2023-02-26 18:02:20.000000 evennia-1.2.1/evennia/utils/evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    53244 2023-01-25 17:38:44.000000 evennia-1.2.1/evennia/utils/funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8779 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/gametime.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.516069 evennia-1.2.1/evennia/utils/idmapper/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/LICENSE.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/README_evennia.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/README_orig.rst
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/manager.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/models.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2876 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/idmapper/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18787 2023-02-25 08:06:48.000000 evennia-1.2.1/evennia/utils/logger.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10265 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/optionclasses.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6455 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/optionhandler.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/picklefield.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    24450 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/test_resources.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.516069 evennia-1.2.1/evennia/utils/tests/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.516069 evennia-1.2.1/evennia/utils/tests/data/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/data/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/data/broken_script.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/data/evform_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/data/evmenu_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/data/prototypes_example.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_ansi.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_batchprocessors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_containers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7032 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_create_functions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7543 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_dbserialize.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_eveditor.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12172 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_evform.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11767 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_evmenu.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12101 2023-02-26 18:31:37.000000 evennia-1.2.1/evennia/utils/tests/test_evtable.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    30844 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_funcparser.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_gametime.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_search.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_tagparsing.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    29939 2023-01-06 18:10:32.000000 evennia-1.2.1/evennia/utils/tests/test_utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6371 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/tests/test_validatorfuncs.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/text2html.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    97196 2023-01-06 18:10:32.000000 evennia-1.2.1/evennia/utils/utils.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/validatorfuncs.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.516069 evennia-1.2.1/evennia/utils/verb_conjugation/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/verb_conjugation/LICENSE.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/verb_conjugation/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9885 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/verb_conjugation/conjugate.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/verb_conjugation/pronouns.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/verb_conjugation/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/utils/verb_conjugation/verbs.txt
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/__init__.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/attributes.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/comms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/frontpage.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11915 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/objects.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4499 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/scripts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/server.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/tags.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/admin/utils.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/api/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/filters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/permissions.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/root.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/serializers.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/api/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/web/static/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/web/static/rest_framework/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/rest_framework/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/rest_framework/css/api.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/rest_framework/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/rest_framework/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/web/static/webclient/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/webclient/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/css/goldenlayout.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/css/webclient.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/webclient/fonts/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/fonts/DejaVuSansMono.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/webclient/js/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    18546 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/evennia.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/webclient/js/plugins/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/clienthelp.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/default_in.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1958 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/default_out.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/default_unload.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/font.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    28903 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/goldenlayout.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/history.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/hotbuttons.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/iframe.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/message_routing.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/multimedia.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/notifications.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/oob.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/options2.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/popups.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/plugins/text2html.js
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9705 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/js/webclient_gui.js
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.520069 evennia-1.2.1/evennia/web/static/webclient/media/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/webclient/media/notification.wav
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/web/static/website/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/static/website/css/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/website/css/custom.css
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/website/css/website.css
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/static/website/images/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/website/images/LICENCE
--rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/website/images/evennia_logo.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/website/images/evennia_logo_festive.png
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/static/website/images/favicon.ico
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia/web/templates/
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templates/admin/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/admin/app_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/admin/frontpage.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templates/rest_framework/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/rest_framework/api.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/rest_framework/redoc.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templates/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     7691 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/webclient/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/webclient/webclient.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templates/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/404.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/500.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4078 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/web/templates/website/_menu.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/base.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/channel_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/channel_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/character_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/character_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/character_manage_list.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templates/website/flatpages/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/flatpages/default.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/generic_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/help_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/help_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5367 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/index.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/messages.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/object_confirm_delete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/object_detail.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/object_list.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/pagination.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templates/website/registration/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/logged_out.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/login.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_change_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_change_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_reset_complete.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_reset_confirm.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_reset_done.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_reset_email.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/registration/password_reset_form.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/web/templates/website/registration/register.html
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templates/website/tbi.html
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/templatetags/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templatetags/README.md
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templatetags/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/templatetags/addclass.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/utils/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1256 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/adminsite.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/apache_wsgi.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/backends.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/evennia_modpy_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/evennia_wsgi_apache.conf
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4137 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/web/utils/general_context.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2712 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/utils/middleware.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2443 2023-01-06 19:58:52.000000 evennia-1.2.1/evennia/web/utils/tests.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/webclient/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/webclient/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/webclient/urls.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/webclient/views.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/website/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/forms.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    12503 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/tests.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/urls.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.524069 evennia-1.2.1/evennia/web/website/views/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/__init__.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2168 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/accounts.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/channels.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     8330 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/characters.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/errors.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    11796 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/help.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     4624 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/index.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/mixins.py
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2022-12-17 18:42:26.000000 evennia-1.2.1/evennia/web/website/views/objects.py
-drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-02-26 19:23:20.472069 evennia-1.2.1/evennia.egg-info/
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-02-26 19:23:20.000000 evennia-1.2.1/evennia.egg-info/PKG-INFO
--rw-rw-r--   0 griatch   (1000) griatch   (1000)    34356 2023-02-26 19:23:20.000000 evennia-1.2.1/evennia.egg-info/SOURCES.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2023-02-26 19:23:20.000000 evennia-1.2.1/evennia.egg-info/dependency_links.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-02-26 19:23:20.000000 evennia-1.2.1/evennia.egg-info/requires.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2023-02-26 19:23:20.000000 evennia-1.2.1/evennia.egg-info/top_level.txt
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     3961 2023-02-26 19:19:58.000000 evennia-1.2.1/pyproject.toml
--rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2023-02-26 19:23:20.528069 evennia-1.2.1/setup.cfg
--rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2022-12-17 18:42:26.000000 evennia-1.2.1/setup.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1531 2023-04-10 11:44:01.000000 evennia-1.3.0/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-04-29 06:52:56.532944 evennia-1.3.0/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3027 2023-04-10 11:44:01.000000 evennia-1.3.0/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.436944 evennia-1.3.0/bin/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/bin/unix/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)      210 2023-04-10 11:44:01.000000 evennia-1.3.0/bin/unix/evennia
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        6 2023-04-29 06:31:26.000000 evennia-1.3.0/evennia/VERSION.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      438 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/VERSION_REQS.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12647 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1839 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/__main__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia/accounts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      214 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    67757 2023-04-20 21:48:41.000000 evennia-1.3.0/evennia/accounts/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26733 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/bots.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9574 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia/accounts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7211 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0002_move_defaults.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0003_auto_20150209_2234.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2158 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0004_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1010 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0005_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1488 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1927 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0007_copy_player_to_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3944 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0008_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      867 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0009_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0010_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4017 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      490 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/0012_defaultaccount_alter_accountdb_id_account_bot_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5740 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16624 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/accounts/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      304 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/commands/_trial_temp/
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/_trial_temp/_trial_marker
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8287 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27219 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdset.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26152 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/cmdsethandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29198 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/command.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/commands/default/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37421 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19595 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/admin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23003 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/batchprocess.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   167200 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/building.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2358 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3032 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_character.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      371 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      872 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/cmdset_unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    76302 2023-04-29 06:12:49.000000 evennia-1.3.0/evennia/commands/default/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22494 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/general.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39551 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12788 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/muxcommand.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3152 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/syscommands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41884 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/system.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    81813 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17440 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/default/unloggedin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46641 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/commands/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.448944 evennia-1.3.0/evennia/comms/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      207 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32556 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16863 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/comms/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3523 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      500 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0002_msg_db_hide_from_objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3784 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0003_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      504 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0004_auto_20150118_1631.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      641 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0005_auto_20150223_1517.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      615 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0007_msg_db_tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0008_auto_20160905_0902.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3872 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0009_auto_20160921_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0010_auto_20161206_1912.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1029 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0011_auto_20170217_2039.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4563 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0011_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      267 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0012_merge_20170617_2017.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4778 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0013_auto_20170705_1726.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0014_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      943 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0015_auto_20170706_2041.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      462 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0016_auto_20180925_1735.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7069 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0017_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      665 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0018_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1713 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0019_auto_20210514_2032.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      916 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0020_auto_20210514_2210.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3635 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0021_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      711 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22638 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3166 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/comms/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      198 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7695 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32480 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22503 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/awsstorage/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/building_menu/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46012 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      148 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42659 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/building_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6878 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/building_menu/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/color_markups/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2641 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8605 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/color_markups.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/color_markups/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/components/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6397 2023-04-29 05:57:10.000000 evennia-1.3.0/evennia/contrib/base_systems/components/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      952 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3915 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/component.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3762 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/dbfield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11201 2023-04-20 16:46:53.000000 evennia-1.3.0/evennia/contrib/base_systems/components/holder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7237 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/components/signals.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14575 2023-04-20 16:46:53.000000 evennia-1.3.0/evennia/contrib/base_systems/components/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1549 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      439 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10390 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2017 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/email_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1022 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      136 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1445 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10264 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/email_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1200 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/email_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.452944 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8938 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      703 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3074 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27602 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/webclient.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40300 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      128 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6777 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21872 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3048 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23990 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21618 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34963 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8151 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/ingame_python/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/menu_login/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      787 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1206 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8781 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/menu_login.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/menu_login/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1936 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16012 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2298 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2241 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1654 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9989 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/base_systems/unixcommand/unixcommand.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/full_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       75 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       48 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5210 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22699 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10565 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34348 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7942 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      753 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9582 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/state.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4168 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10461 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6112 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      269 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/barter/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4322 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       80 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29726 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/barter.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5976 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/barter/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/clothing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4249 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      199 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24574 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/clothing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4816 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/clothing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2084 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       88 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7580 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/cooldowns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6135 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/cooldowns/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.456944 evennia-1.3.0/evennia/contrib/game_systems/crafting/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11186 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      233 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41599 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/crafting.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17892 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/example_recipes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24911 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/crafting/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/gendersub/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1986 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      123 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5096 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/gendersub.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1091 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/gendersub/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/mail/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      115 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14841 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/mail.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1852 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/mail/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/multidescer/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      932 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9951 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/multidescer.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/multidescer/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/puzzles/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2181 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27837 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/puzzles.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41328 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/puzzles/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2940 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28762 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_basic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    23139 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_equip.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37446 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_items.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_magic.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38339 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_range.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29682 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       84 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/extended_room/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3172 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      384 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/extended_room.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4793 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/extended_room/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1358 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       92 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10572 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1404 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/ingame_map_display/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/mapbuilder/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9672 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       87 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17398 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/mapbuilder.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6435 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/mapbuilder/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/simpledoor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1356 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5838 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/simpledoor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1079 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/simpledoor/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/slow_exit/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1730 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      203 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5046 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/slow_exit.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      824 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/slow_exit/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.460944 evennia-1.3.0/evennia/contrib/grid/wilderness/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4932 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      394 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6026 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28916 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/wilderness/wilderness.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/grid/xyzgrid/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54690 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      202 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20837 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7822 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13723 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/launchcmd.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1145 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42072 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1043 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    40413 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    52070 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap_legend.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10484 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzgrid.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24616 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzroom.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      406 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/buffs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22364 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    45607 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/buff.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3893 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/samplebuffs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16470 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/buffs/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/character_creator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      176 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/character_creator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21006 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/example_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1552 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/character_creator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/dice/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1442 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      177 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10272 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/dice.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      901 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/dice/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/health_bar/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1264 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4913 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/health_bar.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1634 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/health_bar/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/rpsystem/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9938 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      793 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24722 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/rplanguage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65825 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/rpsystem.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14981 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/rpsystem/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/rpg/traits/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14246 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      294 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37184 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    54252 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/rpg/traits/traits.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/tutorials/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      151 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       81 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1623 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       50 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1567 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3618 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.464944 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      471 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      104 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2311 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3324 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/evadventure/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1183 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      164 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3996 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/build_techdemo.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/build_world.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12557 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11187 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    48197 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13739 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17844 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1533 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/enums.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14381 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11894 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/npcs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6614 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8743 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11708 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/random_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2983 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13120 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17153 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/shops.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1389 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2151 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12871 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4159 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3356 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7811 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8083 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      712 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1485 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/evadventure/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/mirror/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      429 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/mirror/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       83 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/mirror/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2235 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/mirror/mirror.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/red_button/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1344 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/red_button/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       94 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/red_button/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18609 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/red_button/red_button.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      124 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3697 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/talking_npc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      449 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/talking_npc/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4302 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      125 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    50297 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/build.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25293 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16130 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/mob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42155 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42922 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7342 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.468944 evennia-1.3.0/evennia/contrib/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       67 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/auditing/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3303 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2065 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/outputs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8515 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6023 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/auditing/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/fieldfill/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5816 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/fieldfill/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      288 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/fieldfill/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26404 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/fieldfill/fieldfill.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/git_integration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3139 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       86 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7743 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/git_integration.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2828 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/git_integration/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/name_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9815 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   232619 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/btn_givennames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    56503 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/btn_surnames.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14447 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/namegen.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4914 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/name_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/random_string_generator/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2165 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      268 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12595 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/random_string_generator.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      737 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/random_string_generator/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/contrib/utils/tree_select/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5935 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      109 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2199 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20930 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/contrib/utils/tree_select/tree_select.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/game_template/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1521 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/game_template/commands/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      676 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7738 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/command.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2636 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/commands/default_cmdsets.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/gitignore
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.472944 evennia-1.3.0/evennia/game_template/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1718 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/server/conf/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/at_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2154 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/at_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/at_server_startstop.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2174 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/cmdparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/connection_screens.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1159 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/inlinefuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1419 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1065 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4009 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      709 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/portal_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      714 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/secret_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/server_services_plugins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1347 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1500 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/conf/web_plugins.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/server/logs/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      839 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/server/logs/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      733 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3774 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2920 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1525 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2044 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/exits.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8847 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      551 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/rooms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4394 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/typeclasses/scripts.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2939 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      296 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/admin/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      520 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/admin/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/api/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      849 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/game_template/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       53 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/rest_framework/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       47 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/rest_framework/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/game_template/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      132 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/webclient/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      143 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/webclient/js/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/game_template/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      129 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/website/css/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      135 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/static/website/images/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      760 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       58 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/rest_framework/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      223 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/webclient/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/website/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/website/flatpages/README.md
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.476944 evennia-1.3.0/evennia/game_template/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      152 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/templates/website/registration/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1099 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1102 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/webclient/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      539 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/webclient/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1262 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      509 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/web/website/views/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/game_template/world/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      467 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      999 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/batch_cmds.ev
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2186 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/help_entries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3646 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/game_template/world/prototypes.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/help/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      217 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8013 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/filehelp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6229 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/help/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2222 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      577 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0002_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1688 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0003_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      540 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0004_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1166 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0005_auto_20210530_1818.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      473 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/0006_alter_helpentry_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9729 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3736 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7673 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/help/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/locale/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2686 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/README
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/de/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10764 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14475 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/es/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.480944 evennia-1.3.0/evennia/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3821 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30981 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/fr/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26255 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    38581 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/it/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6944 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    35844 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/ko/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3569 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30924 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/la/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/la/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6537 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32786 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/pl/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28236 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/pt/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.484944 evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25584 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42122 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/ru/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2281 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29419 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/sv/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29036 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    43353 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/locale/zh/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3300 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.mo
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30540 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.po
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/locks/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      240 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22093 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/lockfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    26966 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/lockhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13732 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/locks/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.488944 evennia-1.3.0/evennia/objects/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      120 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29704 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/objects/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4315 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1193 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0002_auto_20140917_0756.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      810 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      530 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0004_auto_20150118_1622.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      410 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0005_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1599 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0006_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1203 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0007_objectdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0008_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      643 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5028 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0010_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1351 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0011_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4011 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      488 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/0013_defaultobject_alter_objectdb_id_defaultcharacter_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13399 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   119132 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14391 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/objects/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/prototypes/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6567 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    92110 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/menus.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2912 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/protfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    46545 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/prototypes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    42860 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/spawner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    39636 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/prototypes/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/scripts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      229 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11275 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.492944 evennia-1.3.0/evennia/scripts/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4762 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      675 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0002_auto_20150118_1625.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1507 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      861 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0004_auto_20150306_1354.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      430 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0005_auto_20150306_1441.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      710 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0006_auto_20150310_2249.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      396 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0007_auto_20150403_2339.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      913 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0008_auto_20170606_1731.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1271 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0009_scriptdb_db_account.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      757 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0010_auto_20170705_1736.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4655 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0012_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      666 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0013_auto_20191025_0831.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      752 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0014_auto_20210520_2137.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3329 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0015_convert_contrib_paths.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/0016_scriptbase_alter_scriptdb_id_defaultscript_and_more.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6311 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8746 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/monitorhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4987 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/scripts/scripthandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27442 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/scripts/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20801 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/taskhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10678 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24704 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/scripts/tickerhandler.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      234 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8697 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/amp_client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/connection_wizard.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7955 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/deprecations.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    79833 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/evennia_launcher.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/game_index_client/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4321 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       45 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6277 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/client.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1990 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/game_index_client/service.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7647 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    19709 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/inputfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1708 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/manager.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      812 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1363 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/0002_auto_20190128_2311.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      478 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/0003_alter_serverconfig_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3818 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/models.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.496944 evennia-1.3.0/evennia/server/portal/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17922 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/amp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17520 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/amp_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18478 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/discord.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11345 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/grapevine.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14242 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/irc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2571 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/mccp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3882 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/mssp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2341 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/mxp.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2359 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/naws.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    16002 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/portal.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17231 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/portalsessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4450 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/rss.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15788 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/ssh.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3319 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1785 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/suppress_ga.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17379 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/telnet.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15609 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/telnet_oob.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4861 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/telnet_ssl.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14725 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6991 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/ttype.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/webclient.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15897 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/portal/webclient_ajax.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.500944 evennia-1.3.0/evennia/server/profiling/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      212 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    20881 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/dummyrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9427 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/dummyrunner_settings.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3924 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/memplot.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1375 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/settings_mixin.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1095 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/test_queries.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5371 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1345 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/profiling/timetrace.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28629 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14599 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/serversession.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5616 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/session.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30190 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/sessionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4935 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/signals.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.500944 evennia-1.3.0/evennia/server/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4721 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_amp_connection.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      521 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_initial_setup.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7305 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_launcher.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4444 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_misc.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9256 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/test_server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1369 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/tests/testrunner.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7101 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/throttle.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2763 2023-04-20 22:23:08.000000 evennia-1.3.0/evennia/server/validators.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8653 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/server/webserver.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    60833 2023-04-20 21:45:02.000000 evennia-1.3.0/evennia/settings_default.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.500944 evennia-1.3.0/evennia/typeclasses/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      434 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    64065 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    31304 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/managers.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.504944 evennia-1.3.0/evennia/typeclasses/migrations/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6101 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0001_initial.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      768 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      833 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      922 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1444 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3899 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1699 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4230 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1993 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      821 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      592 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      362 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0015_alter_attribute_options.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      722 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/migrations/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    37091 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    25077 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    17813 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/typeclasses/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.504944 evennia-1.3.0/evennia/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      320 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    51381 2023-04-20 16:46:53.000000 evennia-1.3.0/evennia/utils/ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    15392 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8077 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10242 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/create.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    32941 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    41419 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2734 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evennia-mode.el
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21081 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    78095 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/utils/evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18330 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evmore.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    65173 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    53244 2023-04-20 16:49:57.000000 evennia-1.3.0/evennia/utils/funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8779 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/gametime.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.504944 evennia-1.3.0/evennia/utils/idmapper/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1309 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/LICENSE.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1097 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/README_evennia.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1992 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/README_orig.rst
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       64 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1181 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/manager.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24820 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/models.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2876 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/idmapper/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18789 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/logger.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10265 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/optionclasses.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6455 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/optionhandler.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11093 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/picklefield.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14179 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    24929 2023-04-29 05:55:25.000000 evennia-1.3.0/evennia/utils/test_resources.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/utils/tests/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/utils/tests/data/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      274 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/broken_script.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1125 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/evform_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6245 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/evmenu_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      382 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/data/prototypes_example.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1608 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_ansi.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7052 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_batchprocessors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3463 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_containers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7032 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_create_functions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7888 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_dbserialize.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11752 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_eveditor.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12172 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_evform.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11767 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_evmenu.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12101 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_evtable.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    30844 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_funcparser.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3942 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_gametime.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4460 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_search.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    13564 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_tagparsing.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5509 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    29939 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6371 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/tests/test_validatorfuncs.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12235 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/text2html.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    97251 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/utils.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9489 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/validatorfuncs.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/utils/verb_conjugation/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18011 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/LICENSE.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9885 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/conjugate.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11298 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/pronouns.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10493 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)   554408 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/utils/verb_conjugation/verbs.txt
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.508944 evennia-1.3.0/evennia/web/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1150 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      127 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/__init__.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      428 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    14125 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8627 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/attributes.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8508 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/comms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      593 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/frontpage.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1889 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11915 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/objects.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4499 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/scripts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      508 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/server.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8955 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/tags.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      878 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2884 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/admin/utils.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/api/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7674 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4268 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/filters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3949 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/permissions.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      277 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/root.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9905 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/serializers.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8148 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2293 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5828 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/api/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/rest_framework/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/static/rest_framework/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      298 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/rest_framework/css/api.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.512944 evennia-1.3.0/evennia/web/static/rest_framework/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/rest_framework/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/webclient/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.516944 evennia-1.3.0/evennia/web/static/webclient/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2104 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/css/goldenlayout.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    27268 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/css/webclient.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.516944 evennia-1.3.0/evennia/web/static/webclient/fonts/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    22208 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/fonts/DejaVuSansMono.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.516944 evennia-1.3.0/evennia/web/static/webclient/js/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    18546 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/evennia.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.520943 evennia-1.3.0/evennia/web/static/webclient/js/plugins/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      563 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/clienthelp.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3914 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_in.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1958 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_out.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      345 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_unload.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3785 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/font.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    28903 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2114 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2981 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/history.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5031 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/hotbuttons.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1969 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1912 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/iframe.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4666 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/message_routing.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4611 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/multimedia.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2842 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/notifications.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      909 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/oob.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6262 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/options2.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2790 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/popups.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    10949 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/plugins/text2html.js
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9705 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/js/webclient_gui.js
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.520943 evennia-1.3.0/evennia/web/static/webclient/media/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3624 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/webclient/media/notification.wav
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/static/website/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/static/website/css/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/css/custom.css
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2013 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/css/website.css
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/static/website/images/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      266 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/LICENCE
+-rwxrwxr-x   0 griatch   (1000) griatch   (1000)    17938 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/evennia_logo.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    21167 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/evennia_logo_festive.png
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1406 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/static/website/images/favicon.ico
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.440944 evennia-1.3.0/evennia/web/templates/
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/templates/admin/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1621 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/admin/app_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     6462 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/admin/frontpage.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/templates/rest_framework/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      903 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/rest_framework/api.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      417 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/rest_framework/redoc.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.524943 evennia-1.3.0/evennia/web/templates/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     7691 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/webclient/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1058 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/webclient/webclient.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templates/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      510 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/404.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      614 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/500.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4078 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/_menu.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3132 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/base.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2858 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/channel_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2667 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/channel_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1402 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/character_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/character_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1139 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/character_manage_list.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templates/website/flatpages/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      341 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/flatpages/default.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1501 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/generic_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2715 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/help_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5052 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/help_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5367 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/index.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      180 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/messages.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      900 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/object_confirm_delete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1034 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/object_detail.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      546 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/object_list.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1484 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/pagination.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templates/website/registration/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      942 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/logged_out.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1957 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/login.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      612 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_change_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1422 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_change_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      813 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_complete.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1747 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_confirm.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1185 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_done.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      566 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_email.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1577 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/password_reset_form.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1895 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/registration/register.html
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      671 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templates/website/tbi.html
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/templatetags/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      287 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templatetags/README.md
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templatetags/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/templatetags/addclass.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1631 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.528943 evennia-1.3.0/evennia/web/utils/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1256 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/adminsite.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      596 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/apache_wsgi.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1815 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/backends.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2035 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/evennia_modpy_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1819 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/evennia_wsgi_apache.conf
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4137 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/general_context.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2712 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/middleware.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2443 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/utils/tests.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/evennia/web/webclient/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        0 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/webclient/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      209 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/webclient/urls.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      795 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/webclient/views.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/evennia/web/website/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       31 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5736 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/forms.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    12503 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/tests.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2575 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/urls.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.532944 evennia-1.3.0/evennia/web/website/views/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       24 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/__init__.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2120 2023-04-20 22:20:57.000000 evennia-1.3.0/evennia/web/website/views/accounts.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5329 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/channels.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     8330 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/characters.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      311 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/errors.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    11796 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/help.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     4624 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/index.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     2353 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/mixins.py
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     9037 2023-04-10 11:44:01.000000 evennia-1.3.0/evennia/web/website/views/objects.py
+drwxrwxr-x   0 griatch   (1000) griatch   (1000)        0 2023-04-29 06:52:56.444944 evennia-1.3.0/evennia.egg-info/
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     5239 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/PKG-INFO
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)    34356 2023-04-29 06:52:56.000000 evennia-1.3.0/evennia.egg-info/SOURCES.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        1 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/dependency_links.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)      550 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/requires.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)        8 2023-04-29 06:52:55.000000 evennia-1.3.0/evennia.egg-info/top_level.txt
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     3961 2023-04-29 06:31:51.000000 evennia-1.3.0/pyproject.toml
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)       38 2023-04-29 06:52:56.532944 evennia-1.3.0/setup.cfg
+-rw-rw-r--   0 griatch   (1000) griatch   (1000)     1388 2023-04-10 11:44:01.000000 evennia-1.3.0/setup.py
```

### Comparing `evennia-1.2.1/LICENSE.txt` & `evennia-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/PKG-INFO` & `evennia-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 1.2.1
+Version: 1.3.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-1.2.1/README.md` & `evennia-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/__init__.py` & `evennia-1.3.0/evennia/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/__main__.py` & `evennia-1.3.0/evennia/__main__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/accounts.py` & `evennia-1.3.0/evennia/accounts/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 from django.conf import settings
 from django.contrib.auth import authenticate, password_validation
 from django.core.exceptions import ImproperlyConfigured, ValidationError
 from django.utils import timezone
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext as _
-
 from evennia.accounts.manager import AccountManager
 from evennia.accounts.models import AccountDB
 from evennia.commands.cmdsethandler import CmdSetHandler
 from evennia.comms.models import ChannelDB
 from evennia.objects.models import ObjectDB
 from evennia.scripts.scripthandler import ScriptHandler
 from evennia.server.models import ServerConfig
@@ -34,21 +33,15 @@
     SIGNAL_OBJECT_POST_UNPUPPET,
 )
 from evennia.server.throttle import Throttle
 from evennia.typeclasses.attributes import ModelAttributeBackend, NickHandler
 from evennia.typeclasses.models import TypeclassBase
 from evennia.utils import class_from_module, create, logger
 from evennia.utils.optionhandler import OptionHandler
-from evennia.utils.utils import (
-    is_iter,
-    lazy_property,
-    make_iter,
-    to_str,
-    variable_from_module,
-)
+from evennia.utils.utils import is_iter, lazy_property, make_iter, to_str, variable_from_module
 
 __all__ = ("DefaultAccount", "DefaultGuest")
 
 _SESSIONS = None
 
 _AT_SEARCH_RESULT = variable_from_module(*settings.SEARCH_AT_RESULT.rsplit(".", 1))
 _MULTISESSION_MODE = settings.MULTISESSION_MODE
@@ -505,15 +498,14 @@
         Args:
             validator_config (list): List of dicts comprising the battery of
                 validators to apply to a username.
 
         Returns:
             validators (list): List of instantiated Validator objects.
         """
-
         objs = []
         for validator in validator_config:
             try:
                 klass = import_string(validator["NAME"])
             except ImportError:
                 msg = (
                     f"The module in NAME could not be imported: {validator['NAME']}. "
```

### Comparing `evennia-1.2.1/evennia/accounts/bots.py` & `evennia-1.3.0/evennia/accounts/bots.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/manager.py` & `evennia-1.3.0/evennia/accounts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0001_initial.py` & `evennia-1.3.0/evennia/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0003_auto_20150209_2234.py` & `evennia-1.3.0/evennia/accounts/migrations/0003_auto_20150209_2234.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0004_auto_20150403_2339.py` & `evennia-1.3.0/evennia/accounts/migrations/0004_auto_20150403_2339.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0005_auto_20160905_0902.py` & `evennia-1.3.0/evennia/accounts/migrations/0005_auto_20160905_0902.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0006_auto_20170606_1731.py` & `evennia-1.3.0/evennia/accounts/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0007_copy_player_to_account.py` & `evennia-1.3.0/evennia/accounts/migrations/0007_copy_player_to_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0008_auto_20190128_1820.py` & `evennia-1.3.0/evennia/accounts/migrations/0008_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0009_auto_20191025_0831.py` & `evennia-1.3.0/evennia/accounts/migrations/0009_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py` & `evennia-1.3.0/evennia/accounts/migrations/0011_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/models.py` & `evennia-1.3.0/evennia/accounts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/accounts/tests.py` & `evennia-1.3.0/evennia/accounts/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/cmdhandler.py` & `evennia-1.3.0/evennia/commands/cmdhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/cmdparser.py` & `evennia-1.3.0/evennia/commands/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/cmdset.py` & `evennia-1.3.0/evennia/commands/cmdset.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/cmdsethandler.py` & `evennia-1.3.0/evennia/commands/cmdsethandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/command.py` & `evennia-1.3.0/evennia/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/account.py` & `evennia-1.3.0/evennia/commands/default/account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/admin.py` & `evennia-1.3.0/evennia/commands/default/admin.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/batchprocess.py` & `evennia-1.3.0/evennia/commands/default/batchprocess.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/building.py` & `evennia-1.3.0/evennia/commands/default/building.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/cmdset_account.py` & `evennia-1.3.0/evennia/commands/default/cmdset_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/cmdset_character.py` & `evennia-1.3.0/evennia/commands/default/cmdset_character.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/cmdset_unloggedin.py` & `evennia-1.3.0/evennia/commands/default/cmdset_unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/comms.py` & `evennia-1.3.0/evennia/commands/default/comms.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 - channel
 - page
 - irc/rss/grapevine/discord linking
 
 """
 
 from django.conf import settings
-
 from evennia.accounts import bots
 from evennia.accounts.models import AccountDB
 from evennia.comms.comms import DefaultChannel
 from evennia.comms.models import Msg
 from evennia.locks.lockhandler import LockException
 from evennia.utils import create, logger, search, utils
 from evennia.utils.evmenu import ask_yes_no
@@ -773,15 +772,14 @@
             "my aliases",
             "locks",
             "description",
             align="l",
             maxwidth=_DEFAULT_WIDTH,
         )
         for chan in subscribed:
-
             locks = "-"
             chanid = "-"
             if chan.access(self.caller, "control"):
                 locks = chan.locks
                 chanid = chan.id
 
             my_aliases = ", ".join(self.get_channel_aliases(chan))
@@ -1154,15 +1152,14 @@
                 self.msg("Usage: channel/boot channel[,channel,...] = username [:reason]")
                 return
 
             target_str, *reason = self.rhs.rsplit(":", 1)
             reason = reason[0].strip() if reason else ""
 
             for chan in channels:
-
                 if not chan.access(caller, "control"):
                     self.msg(f"You need 'control'-access to boot a user from {chan.key}.")
                     return
 
                 # the target must be a member of all given channels
                 target = caller.search(target_str, candidates=chan.subscriptions.all())
                 if not target:
@@ -1241,17 +1238,19 @@
 
             channames = ", ".join(chan.key for chan in channels)
             reasonwarn = (
                 ". Also note that your reason will be echoed to the channel" if reason else ""
             )
             ask_yes_no(
                 caller,
-                f"Are you sure you want to ban user {target.key} from "
-                f"channel(s) {channames} (make sure name/channels are correct{reasonwarn}) "
-                "{options}?",
+                (
+                    f"Are you sure you want to ban user {target.key} from "
+                    f"channel(s) {channames} (make sure name/channels are correct{reasonwarn}) "
+                    "{options}?"
+                ),
                 _ban_user,
                 "Aborted.",
             )
             return
 
         if "unban" in switches:
             # unban a previously banned user from channel
@@ -1356,15 +1355,15 @@
                 for target in self.lhslist:
                     target_obj = self.caller.search(target)
                     if not target_obj:
                         return
                     targets.append(target_obj)
                 message = self.rhs.strip()
             else:
-                target, *message = self.args.split(" ", 4)
+                target, *message = self.args.split(" ", 1)
                 if target and target.isnumeric():
                     # a number to specify a historic page
                     number = int(target)
                 elif target:
                     target_obj = self.caller.search(target, quiet=True)
                     if target_obj:
                         # a proper target
@@ -1966,35 +1965,38 @@
             discord_bot.start()
             self.msg("Created and initialized a new Discord relay bot.")
         else:
             discord_bot = discord_bot[0]
 
         if not discord_bot.is_typeclass(settings.DISCORD_BOT_CLASS, exact=True):
             self.msg(
-                f"WARNING: The Discord bot's typeclass is '{discord_bot.typeclass_path}'. This does not match {settings.DISCORD_BOT_CLASS} in settings!"
+                f"WARNING: The Discord bot's typeclass is '{discord_bot.typeclass_path}'. This does"
+                f" not match {settings.DISCORD_BOT_CLASS} in settings!"
             )
 
         if "start" in self.switches:
             if discord_bot.sessions.all():
                 self.msg("The Discord bot is already running.")
             else:
                 discord_bot.start()
                 self.msg("Starting the Discord bot session.")
             return
 
         if "guild" in self.switches:
             discord_bot.db.tag_guild = not discord_bot.db.tag_guild
             self.msg(
-                f"Messages to Evennia |wwill {'' if discord_bot.db.tag_guild else 'not '}|ninclude the Discord server."
+                f"Messages to Evennia |wwill {'' if discord_bot.db.tag_guild else 'not '}|ninclude"
+                " the Discord server."
             )
             return
         if "channel" in self.switches:
             discord_bot.db.tag_channel = not discord_bot.db.tag_channel
             self.msg(
-                f"Relayed messages |wwill {'' if discord_bot.db.tag_channel else 'not '}|ninclude the originating channel."
+                f"Relayed messages |wwill {'' if discord_bot.db.tag_channel else 'not '}|ninclude"
+                " the originating channel."
             )
             return
 
         if "list" in self.switches or not self.args:
             # show all connections
             if channel_list := discord_bot.db.channels:
                 table = self.styled_table(
@@ -2025,15 +2027,16 @@
                     self.msg("Usage: discord2chan/remove <link id>")
                     return
                 if lid < len(channel_list):
                     ev_chan, dc_chan = discord_bot.db.channels.pop(lid)
                     dc_chan_names = discord_bot.attributes.get("discord_channels", {})
                     dc_info = dc_chan_names.get(dc_chan, {"name": "unknown", "guild": "unknown"})
                     self.msg(
-                        f"Removed link between {ev_chan} and #{dc_info.get('name','?')}@{dc_info.get('guild','?')}"
+                        f"Removed link between {ev_chan} and"
+                        f" #{dc_info.get('name','?')}@{dc_info.get('guild','?')}"
                     )
                     return
             else:
                 self.msg("There are no active connections to Discord.")
                 return
 
         ev_channel = self.lhs
```

### Comparing `evennia-1.2.1/evennia/commands/default/general.py` & `evennia-1.3.0/evennia/commands/default/general.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/help.py` & `evennia-1.3.0/evennia/commands/default/help.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/muxcommand.py` & `evennia-1.3.0/evennia/commands/default/muxcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/syscommands.py` & `evennia-1.3.0/evennia/commands/default/syscommands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/system.py` & `evennia-1.3.0/evennia/commands/default/system.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/tests.py` & `evennia-1.3.0/evennia/commands/default/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/default/unloggedin.py` & `evennia-1.3.0/evennia/commands/default/unloggedin.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/commands/tests.py` & `evennia-1.3.0/evennia/commands/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/comms.py` & `evennia-1.3.0/evennia/comms/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/managers.py` & `evennia-1.3.0/evennia/comms/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0001_initial.py` & `evennia-1.3.0/evennia/comms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0003_auto_20140917_0756.py` & `evennia-1.3.0/evennia/comms/migrations/0003_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0005_auto_20150223_1517.py` & `evennia-1.3.0/evennia/comms/migrations/0005_auto_20150223_1517.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py` & `evennia-1.3.0/evennia/comms/migrations/0006_channeldb_db_object_subscriptions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0007_msg_db_tags.py` & `evennia-1.3.0/evennia/comms/migrations/0007_msg_db_tags.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0009_auto_20160921_1731.py` & `evennia-1.3.0/evennia/comms/migrations/0009_auto_20160921_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0010_auto_20161206_1912.py` & `evennia-1.3.0/evennia/comms/migrations/0010_auto_20161206_1912.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0011_auto_20170217_2039.py` & `evennia-1.3.0/evennia/comms/migrations/0011_auto_20170217_2039.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0011_auto_20170606_1731.py` & `evennia-1.3.0/evennia/comms/migrations/0011_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0013_auto_20170705_1726.py` & `evennia-1.3.0/evennia/comms/migrations/0013_auto_20170705_1726.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0014_auto_20170705_1736.py` & `evennia-1.3.0/evennia/comms/migrations/0014_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0015_auto_20170706_2041.py` & `evennia-1.3.0/evennia/comms/migrations/0015_auto_20170706_2041.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0017_auto_20190128_1820.py` & `evennia-1.3.0/evennia/comms/migrations/0017_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0018_auto_20191025_0831.py` & `evennia-1.3.0/evennia/comms/migrations/0018_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0019_auto_20210514_2032.py` & `evennia-1.3.0/evennia/comms/migrations/0019_auto_20210514_2032.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0020_auto_20210514_2210.py` & `evennia-1.3.0/evennia/comms/migrations/0020_auto_20210514_2210.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0021_auto_20210520_2137.py` & `evennia-1.3.0/evennia/comms/migrations/0021_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py` & `evennia-1.3.0/evennia/comms/migrations/0022_defaultchannel_alter_channeldb_id_alter_msg_id_and_more.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/models.py` & `evennia-1.3.0/evennia/comms/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/comms/tests.py` & `evennia-1.3.0/evennia/comms/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/README.md` & `evennia-1.3.0/evennia/contrib/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/awsstorage/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/awsstorage/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 For example, when Evennia (or Django), tries to save a file permanently (say, an
 image uploaded by a user), the save (or load) communication follows the path:
 
     Evennia -> Django
     Django -> Storage backend
     Storage backend -> file storage location (e.g. hard drive)
 
-[django docs](https://docs.djangoproject.com/en/3.0/ref/settings/#std:setting-STATICFILES_STORAGE)
+[django docs](https://docs.djangoproject.com/en/4.1/ref/settings/#std:setting-STATICFILES_STORAGE)
 
 This plugin, when enabled, overrides the default storage backend,
 which defaults to saving files at mygame/website/, instead,
 sending the files to S3 via the storage backend defined herein.
 
 There is no way (or need) to directly access or use the functions here with
 other contributions or custom code. Simply work how you would normally, Django
```

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py` & `evennia-1.3.0/evennia/contrib/base_systems/awsstorage/aws_s3_cdn.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/awsstorage/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/awsstorage/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/building_menu/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/building_menu/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/building_menu/building_menu.py` & `evennia-1.3.0/evennia/contrib/base_systems/building_menu/building_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/building_menu/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/building_menu/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/color_markups/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/color_markups/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/color_markups/color_markups.py` & `evennia-1.3.0/evennia/contrib/base_systems/color_markups/color_markups.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/color_markups/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/color_markups/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/components/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Components
 
-_Contrib by ChrisLR 2021_
+Contrib by ChrisLR, 2021
 
-# The Components Contrib
+Expand typeclasses using a components/composition approach.
+
+## The Components Contrib
 
 This contrib introduces Components and Composition to Evennia.
 Each 'Component' class represents a feature that will be 'enabled' on a typeclass instance.
 You can register these components on an entire typeclass or a single object at runtime.
 It supports both persisted attributes and in-memory attributes by using Evennia's AttributeHandler.
 
-# Pros
+## Pros
 - You can reuse a feature across multiple typeclasses without inheritance
 - You can cleanly organize each feature into a self-contained class.
 - You can check if your object supports a feature without checking its instance.
 
-# Cons
+## Cons
 - It introduces additional complexity.
 - A host typeclass instance is required.
 
-# How to install
+## How to install
 
 To enable component support for a typeclass,
 import and inherit the ComponentHolderMixin, similar to this
 ```python
 from evennia.contrib.base_systems.components import ComponentHolderMixin
 class Character(ComponentHolderMixin, DefaultCharacter):
 # ...
@@ -122,23 +124,23 @@
 from typeclasses.components.health import Health
 ```
 ```python
 from typeclasses.components import health
 ```
 Both of the above examples will work.
 
-# Full Example
+## Full Example
 ```python
 from evennia.contrib.base_systems import components
 
 
 # This is the Component class
 class Health(components.Component):
     name = "health"
-    
+
     # Stores the current and max values as Attributes on the host, defaulting to 100
     current = components.DBField(default=100)
     max = components.DBField(default=100)
 
     def damage(self, value):
         if self.current <= 0:
             return
@@ -181,12 +183,12 @@
         caller = self.caller
         targets = self.caller.search(args, quiet=True)
         valid_target = None
         for target in targets:
             # Attempt to retrieve the component, None is obtained if it does not exist.
             if target.components.health:
                 valid_target = target
-        
+
         if not valid_target:
             caller.msg("You can't attack that!")
             return True
 ```
```

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/__init__.py` & `evennia-1.3.0/evennia/contrib/base_systems/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/component.py` & `evennia-1.3.0/evennia/contrib/base_systems/components/component.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/dbfield.py` & `evennia-1.3.0/evennia/contrib/base_systems/components/dbfield.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/holder.py` & `evennia-1.3.0/evennia/contrib/base_systems/components/holder.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,19 @@
         component = instance.components.get(self.component_name)
         return component
 
     def __set__(self, instance, value):
         raise Exception("Cannot set a class property")
 
     def __set_name__(self, owner, name):
-        class_components = getattr(owner, "_class_components", None)
+        # Retrieve the class_components set on the direct class only
+        class_components = owner.__dict__.get("_class_components")
         if not class_components:
-            class_components = []
+            # Create a new list, including inherited class components
+            class_components = list(getattr(owner, "_class_components", []))
             setattr(owner, "_class_components", class_components)
 
         class_components.append((self.component_name, self.values))
 
 
 class ComponentHandler:
     """
```

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/signals.py` & `evennia-1.3.0/evennia/contrib/base_systems/components/signals.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/components/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/components/tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,21 +38,33 @@
 
 
 class CharacterWithComponents(ComponentHolderMixin, DefaultCharacter):
     test_a = ComponentProperty("test_a")
     test_b = ComponentProperty("test_b", my_int=3, my_list=[1, 2, 3])
 
 
+class InheritedTCWithComponents(CharacterWithComponents):
+    test_c = ComponentProperty("test_c")
+
+
 class TestComponents(EvenniaTest):
     character_typeclass = CharacterWithComponents
 
     def test_character_has_class_components(self):
         assert self.char1.test_a
         assert self.char1.test_b
 
+    def test_inherited_typeclass_does_not_include_child_class_components(self):
+        char_with_c = create.create_object(
+            InheritedTCWithComponents, key="char_with_c", location=self.room1, home=self.room1
+        )
+        assert self.char1.test_a
+        assert not self.char1.cmp.get('test_c')
+        assert char_with_c.test_c
+
     def test_character_instances_components_properly(self):
         assert isinstance(self.char1.test_a, ComponentTestA)
         assert isinstance(self.char1.test_b, ComponentTestB)
 
     def test_character_assigns_default_value(self):
         assert self.char1.test_a.my_int == 1
         assert self.char1.test_a.my_list == []
```

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/custom_gametime.py` & `evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/custom_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/custom_gametime/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/custom_gametime/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/email_login/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/email_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/email_login/connection_screens.py` & `evennia-1.3.0/evennia/contrib/base_systems/email_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/email_login/email_login.py` & `evennia-1.3.0/evennia/contrib/base_systems/email_login/email_login.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/email_login/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/email_login/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/__init__.py` & `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py` & `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/test_text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py` & `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/text2bbcode.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/godotwebsocket/webclient.py` & `evennia-1.3.0/evennia/contrib/base_systems/godotwebsocket/webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 ## Basic structure and vocabulary
 
 - At the basis of the in-game Python system are **events**.  An **event**
   defines the context in which we would like to call some arbitrary code.  For
 instance, one event is defined on exits and will fire every time a character
 traverses through this exit.  Events are described on a [typeclass](Typeclasses)
-([exits](Objects#exits) in our example).  All objects inheriting from this
+([exits](Exits) in our example).  All objects inheriting from this
 typeclass will have access to this event.
 - **Callbacks** can be set on individual objects, on events defined in code.
   These **callbacks** can contain arbitrary code and describe a specific
 behavior for an object.  When the event fires, all callbacks connected to this
 object's event are executed.
 
 To see the system in context, when an object is picked up (using the default
```

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/callbackhandler.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/callbackhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/commands.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/eventfuncs.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/eventfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/scripts.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/typeclasses.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/ingame_python/utils.py` & `evennia-1.3.0/evennia/contrib/base_systems/ingame_python/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/menu_login/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/menu_login/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/menu_login/connection_screens.py` & `evennia-1.3.0/evennia/contrib/base_systems/menu_login/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/menu_login/menu_login.py` & `evennia-1.3.0/evennia/contrib/base_systems/menu_login/menu_login.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py` & `evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/mux_comms_cmds.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/mux_comms_cmds/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/mux_comms_cmds/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/unixcommand/README.md` & `evennia-1.3.0/evennia/contrib/base_systems/unixcommand/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/unixcommand/tests.py` & `evennia-1.3.0/evennia/contrib/base_systems/unixcommand/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/base_systems/unixcommand/unixcommand.py` & `evennia-1.3.0/evennia/contrib/base_systems/unixcommand/unixcommand.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/README.md` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/commands.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/menu.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/objects.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/room.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/room.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/scripts.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/state.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/state.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/states/README.md` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/states/state_001_start.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/tests.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/full_systems/evscaperoom/utils.py` & `evennia-1.3.0/evennia/contrib/full_systems/evscaperoom/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/barter/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/barter/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/barter/barter.py` & `evennia-1.3.0/evennia/contrib/game_systems/barter/barter.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/barter/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/barter/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/clothing/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/clothing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/clothing/clothing.py` & `evennia-1.3.0/evennia/contrib/game_systems/clothing/clothing.py`

 * *Files 0% similar despite different names*

```diff
@@ -273,15 +273,15 @@
         # Echo a message to the room
         if not quiet:
             if type(wearstyle) is str:
                 message = f"$You() $conj(wear) {self.name} {wearstyle}"
             else:
                 message = f"$You() $conj(put) on {self.name}"
             if to_cover:
-                message += ", covering {iter_to_str(to_cover)}"
+                message += f", covering {iter_to_str(to_cover)}"
             wearer.location.msg_contents(message + ".", from_obj=wearer)
 
     def remove(self, wearer, quiet=False):
         """
         Removes worn clothes and optionally echoes to the room.
 
         Args:
```

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/clothing/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/clothing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/cooldowns/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/cooldowns/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/cooldowns/cooldowns.py` & `evennia-1.3.0/evennia/contrib/game_systems/cooldowns/cooldowns.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/cooldowns/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/cooldowns/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/crafting/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/crafting/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/crafting/crafting.py` & `evennia-1.3.0/evennia/contrib/game_systems/crafting/crafting.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/crafting/example_recipes.py` & `evennia-1.3.0/evennia/contrib/game_systems/crafting/example_recipes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/crafting/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/crafting/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/gendersub/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/gendersub/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/gendersub/gendersub.py` & `evennia-1.3.0/evennia/contrib/game_systems/gendersub/gendersub.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/gendersub/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/gendersub/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/mail/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/mail/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/mail/mail.py` & `evennia-1.3.0/evennia/contrib/game_systems/mail/mail.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/mail/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/mail/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/multidescer/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/multidescer/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/multidescer/multidescer.py` & `evennia-1.3.0/evennia/contrib/game_systems/multidescer/multidescer.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/multidescer/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/multidescer/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/puzzles/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/puzzles/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/puzzles/puzzles.py` & `evennia-1.3.0/evennia/contrib/game_systems/puzzles/puzzles.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/puzzles/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/puzzles/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/README.md` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_basic.py` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_basic.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         Adds attributes for a character's current and maximum HP.
         We're just going to set this value at '100' by default.
 
         You may want to expand this to include various 'stats' that
         can be changed at creation and factor into combat calculations.
         """
 
-    def at_pre_move(self, destination):
+    def at_pre_move(self, destination, move_type='move', **kwargs):
         """
         Called just before starting to move this object to
         destination.
 
         Args:
             destination (Object): The object we are moving to
```

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_equip.py` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_equip.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_items.py` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_items.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_magic.py` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_magic.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tb_range.py` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tb_range.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/game_systems/turnbattle/tests.py` & `evennia-1.3.0/evennia/contrib/game_systems/turnbattle/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/extended_room/README.md` & `evennia-1.3.0/evennia/contrib/grid/extended_room/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/extended_room/extended_room.py` & `evennia-1.3.0/evennia/contrib/grid/extended_room/extended_room.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/extended_room/tests.py` & `evennia-1.3.0/evennia/contrib/grid/extended_room/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/ingame_map_display/README.md` & `evennia-1.3.0/evennia/contrib/grid/ingame_map_display/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/ingame_map_display/ingame_map_display.py` & `evennia-1.3.0/evennia/contrib/grid/ingame_map_display/ingame_map_display.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/ingame_map_display/tests.py` & `evennia-1.3.0/evennia/contrib/grid/ingame_map_display/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/mapbuilder/README.md` & `evennia-1.3.0/evennia/contrib/grid/mapbuilder/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/mapbuilder/mapbuilder.py` & `evennia-1.3.0/evennia/contrib/grid/mapbuilder/mapbuilder.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/mapbuilder/tests.py` & `evennia-1.3.0/evennia/contrib/grid/mapbuilder/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/simpledoor/README.md` & `evennia-1.3.0/evennia/contrib/grid/simpledoor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/simpledoor/simpledoor.py` & `evennia-1.3.0/evennia/contrib/grid/simpledoor/simpledoor.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/simpledoor/tests.py` & `evennia-1.3.0/evennia/contrib/grid/simpledoor/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/slow_exit/README.md` & `evennia-1.3.0/evennia/contrib/grid/slow_exit/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/slow_exit/slow_exit.py` & `evennia-1.3.0/evennia/contrib/grid/slow_exit/slow_exit.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/slow_exit/tests.py` & `evennia-1.3.0/evennia/contrib/grid/slow_exit/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/wilderness/README.md` & `evennia-1.3.0/evennia/contrib/grid/wilderness/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Wilderness system
 
 Contribution by titeuf87, 2017
 
 This contrib provides a wilderness map without actually creating a large number
-of rooms - as you move, you instead end up back in the same room but its description 
+of rooms - as you move, you instead end up back in the same room but its description
 changes. This means you can make huge areas with little database use as
 long as the rooms are relatively similar (e.g. only the names/descs changing).
 
 ## Installation
 
 This contrib does not provide any new commands. Instead the default `py` command
 is used to call functions/classes in this contrib directly.
@@ -15,19 +15,19 @@
 ## Usage
 
 A wilderness map needs to created first. There can be different maps, all
 with their own name. If no name is provided, then a default one is used. Internally,
 the wilderness is stored as a Script with the name you specify. If you don't
 specify the name, a script named "default" will be created and used.
 
-    @py from evennia.contrib.grid import wilderness; wilderness.create_wilderness()
+    py from evennia.contrib.grid import wilderness; wilderness.create_wilderness()
 
 Once created, it is possible to move into that wilderness map:
 
-    @py from evennia.contrib.grid import wilderness; wilderness.enter_wilderness(me)
+    py from evennia.contrib.grid import wilderness; wilderness.enter_wilderness(me)
 
 All coordinates used by the wilderness map are in the format of `(x, y)`
 tuples. x goes from left to right and y goes from bottom to top. So `(0, 0)`
 is the bottom left corner of the map.
 
 > You can also add a wilderness by defining a WildernessScript in your GLOBAL_SCRIPT
 > settings. If you do, make sure define the map provider.
@@ -98,22 +98,29 @@
 
     def at_prepare_room(self, coordinates, caller, room):
         "Any other changes done to the room before showing it"
         x, y = coordinates
         desc = "This is a room in the pyramid."
         if y == 3 :
             desc = "You can see far and wide from the top of the pyramid."
-        room.ndb.desc = desc
+        room.ndb.active_desc = desc
 ```
 
+Note that the currently active description is stored as `.ndb.active_desc`. When
+looking at the room, this is what will be pulled and shown.
+
+> Exits on a room are always present, but locks hide those not used for a
+> location. So make sure to `quell` if you are a superuser (since the superuser ignores
+> locks, those exits will otherwise not be hidden)
+
 Now we can use our new pyramid-shaped wilderness map. From inside Evennia we
 create a new wilderness (with the name "default") but using our new map provider:
 
     py from world import pyramid as p; p.wilderness.create_wilderness(mapprovider=p.PyramidMapProvider())
-    py from evennia.contrib import wilderness; wilderness.enter_wilderness(me, coordinates=(4, 1))
+    py from evennia.contrib.grid import wilderness; wilderness.enter_wilderness(me, coordinates=(4, 1))
 
 ## Implementation details
 
 When a character moves into the wilderness, they get their own room. If
 they move, instead of moving the character, the room changes to match the
 new coordinates.
```

### Comparing `evennia-1.2.1/evennia/contrib/grid/wilderness/tests.py` & `evennia-1.3.0/evennia/contrib/grid/wilderness/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/wilderness/wilderness.py` & `evennia-1.3.0/evennia/contrib/grid/wilderness/wilderness.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,24 @@
 
     def at_prepare_room(self, coordinates, caller, room):
         "Any other changes done to the room before showing it"
         x, y = coordinates
         desc = "This is a room in the pyramid."
         if y == 3 :
             desc = "You can see far and wide from the top of the pyramid."
-        room.ndb.desc = desc
+        room.ndb.active_desc = desc
 ```
 
+Note that the currently active description is stored as `.ndb.active_desc`. When
+looking at the room, this is what will be pulled and shown.
+
+> Exits on a room are always present, but locks hide those not used for a
+> location. So make sure to `quell` if you are a superuser (since the superuser ignores
+> locks, those exits will otherwise not be hidden)
+
 Now we can use our new pyramid-shaped wilderness map. From inside Evennia we
 create a new wilderness (with the name "default") but using our new map provider:
 
     py from world import pyramid as p; p.wilderness.create_wilderness(mapprovider=p.PyramidMapProvider())
     py from evennia.contrib import wilderness; wilderness.enter_wilderness(me, coordinates=(4, 1))
 
 ## Implementation details
@@ -112,21 +119,15 @@
     separate rooms.
 
     Rooms are created as needed. Unneeded rooms are stored away to avoid the
     overhead cost of creating new rooms again in the future.
 
 """
 
-from evennia import (
-    DefaultExit,
-    DefaultRoom,
-    DefaultScript,
-    create_object,
-    create_script,
-)
+from evennia import DefaultExit, DefaultRoom, DefaultScript, create_object, create_script
 from evennia.typeclasses.attributes import AttributeProperty
 from evennia.utils import inherits_from
 
 
 def create_wilderness(name="default", mapprovider=None, preserve_items=False):
     """
     Creates a new wilderness map. Does nothing if a wilderness map already
```

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/README.md` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/commands.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/example.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/example.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/launchcmd.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/launchcmd.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/prototypes.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/tests.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/utils.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/xymap.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/xymap_legend.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xymap_legend.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/xyzgrid.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzgrid.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/grid/xyzgrid/xyzroom.py` & `evennia-1.3.0/evennia/contrib/grid/xyzgrid/xyzroom.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/buffs/README.md` & `evennia-1.3.0/evennia/contrib/rpg/buffs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/buffs/buff.py` & `evennia-1.3.0/evennia/contrib/rpg/buffs/buff.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/buffs/samplebuffs.py` & `evennia-1.3.0/evennia/contrib/rpg/buffs/samplebuffs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/buffs/tests.py` & `evennia-1.3.0/evennia/contrib/rpg/buffs/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/character_creator/README.md` & `evennia-1.3.0/evennia/contrib/rpg/character_creator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/character_creator/character_creator.py` & `evennia-1.3.0/evennia/contrib/rpg/character_creator/character_creator.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/character_creator/example_menu.py` & `evennia-1.3.0/evennia/contrib/rpg/character_creator/example_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/character_creator/tests.py` & `evennia-1.3.0/evennia/contrib/rpg/character_creator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/dice/README.md` & `evennia-1.3.0/evennia/contrib/rpg/dice/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/dice/dice.py` & `evennia-1.3.0/evennia/contrib/rpg/dice/dice.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/dice/tests.py` & `evennia-1.3.0/evennia/contrib/rpg/dice/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/health_bar/README.md` & `evennia-1.3.0/evennia/contrib/rpg/health_bar/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/health_bar/health_bar.py` & `evennia-1.3.0/evennia/contrib/rpg/health_bar/health_bar.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/health_bar/tests.py` & `evennia-1.3.0/evennia/contrib/rpg/health_bar/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/rpsystem/README.md` & `evennia-1.3.0/evennia/contrib/rpg/rpsystem/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/rpsystem/__init__.py` & `evennia-1.3.0/evennia/contrib/rpg/rpsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/rpsystem/rplanguage.py` & `evennia-1.3.0/evennia/contrib/rpg/rpsystem/rplanguage.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/rpsystem/rpsystem.py` & `evennia-1.3.0/evennia/contrib/rpg/rpsystem/rpsystem.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/rpsystem/tests.py` & `evennia-1.3.0/evennia/contrib/rpg/rpsystem/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/traits/README.md` & `evennia-1.3.0/evennia/contrib/rpg/traits/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/traits/tests.py` & `evennia-1.3.0/evennia/contrib/rpg/traits/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/rpg/traits/traits.py` & `evennia-1.3.0/evennia/contrib/rpg/traits/traits.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/README.md` & `evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev` & `evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/batchprocessor/example_batch_code.py` & `evennia-1.3.0/evennia/contrib/tutorials/batchprocessor/example_batch_code.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py` & `evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/bodyfunctions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/bodyfunctions/tests.py` & `evennia-1.3.0/evennia/contrib/tutorials/bodyfunctions/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/README.md` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/build_techdemo.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/build_techdemo.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/characters.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/chargen.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/combat_turnbased.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/combat_turnbased.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/commands.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/dungeon.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/enums.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/enums.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/equipment.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/npcs.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/npcs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/objects.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/quests.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/quests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/random_tables.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/random_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/rooms.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/rules.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/rules.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/shops.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/shops.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/mixins.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_characters.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_chargen.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_chargen.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_combat.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_combat.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_commands.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_dungeon.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_equipment.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_equipment.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_quests.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_quests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_rules.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/tests/test_utils.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/evadventure/utils.py` & `evennia-1.3.0/evennia/contrib/tutorials/evadventure/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/mirror/mirror.py` & `evennia-1.3.0/evennia/contrib/tutorials/mirror/mirror.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/red_button/README.md` & `evennia-1.3.0/evennia/contrib/tutorials/red_button/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/red_button/red_button.py` & `evennia-1.3.0/evennia/contrib/tutorials/red_button/red_button.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/talking_npc/README.md` & `evennia-1.3.0/evennia/contrib/tutorials/talking_npc/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/talking_npc/talking_npc.py` & `evennia-1.3.0/evennia/contrib/tutorials/talking_npc/talking_npc.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/README.md` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/build.ev` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/build.ev`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/intro_menu.py` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/intro_menu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/mob.py` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/mob.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/objects.py` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/rooms.py` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/tutorials/tutorial_world/tests.py` & `evennia-1.3.0/evennia/contrib/tutorials/tutorial_world/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/auditing/README.md` & `evennia-1.3.0/evennia/contrib/utils/auditing/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/auditing/outputs.py` & `evennia-1.3.0/evennia/contrib/utils/auditing/outputs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/auditing/server.py` & `evennia-1.3.0/evennia/contrib/utils/auditing/server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/auditing/tests.py` & `evennia-1.3.0/evennia/contrib/utils/auditing/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/fieldfill/README.md` & `evennia-1.3.0/evennia/contrib/utils/fieldfill/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/fieldfill/fieldfill.py` & `evennia-1.3.0/evennia/contrib/utils/fieldfill/fieldfill.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/git_integration/README.md` & `evennia-1.3.0/evennia/contrib/utils/git_integration/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/git_integration/git_integration.py` & `evennia-1.3.0/evennia/contrib/utils/git_integration/git_integration.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/git_integration/tests.py` & `evennia-1.3.0/evennia/contrib/utils/git_integration/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/name_generator/README.md` & `evennia-1.3.0/evennia/contrib/utils/name_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/name_generator/btn_givennames.txt` & `evennia-1.3.0/evennia/contrib/utils/name_generator/btn_givennames.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/name_generator/btn_surnames.txt` & `evennia-1.3.0/evennia/contrib/utils/name_generator/btn_surnames.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/name_generator/namegen.py` & `evennia-1.3.0/evennia/contrib/utils/name_generator/namegen.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/name_generator/tests.py` & `evennia-1.3.0/evennia/contrib/utils/name_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/random_string_generator/README.md` & `evennia-1.3.0/evennia/contrib/utils/random_string_generator/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/random_string_generator/random_string_generator.py` & `evennia-1.3.0/evennia/contrib/utils/random_string_generator/random_string_generator.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/random_string_generator/tests.py` & `evennia-1.3.0/evennia/contrib/utils/random_string_generator/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/tree_select/README.md` & `evennia-1.3.0/evennia/contrib/utils/tree_select/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/tree_select/tests.py` & `evennia-1.3.0/evennia/contrib/utils/tree_select/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/contrib/utils/tree_select/tree_select.py` & `evennia-1.3.0/evennia/contrib/utils/tree_select/tree_select.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/README.md` & `evennia-1.3.0/evennia/game_template/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/commands/README.md` & `evennia-1.3.0/evennia/game_template/commands/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/commands/command.py` & `evennia-1.3.0/evennia/game_template/commands/command.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/commands/default_cmdsets.py` & `evennia-1.3.0/evennia/game_template/commands/default_cmdsets.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/gitignore` & `evennia-1.3.0/evennia/game_template/gitignore`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/README.md` & `evennia-1.3.0/evennia/game_template/server/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/at_initial_setup.py` & `evennia-1.3.0/evennia/game_template/server/conf/at_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/at_search.py` & `evennia-1.3.0/evennia/game_template/server/conf/at_search.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/at_server_startstop.py` & `evennia-1.3.0/evennia/game_template/server/conf/at_server_startstop.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/cmdparser.py` & `evennia-1.3.0/evennia/game_template/server/conf/cmdparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/connection_screens.py` & `evennia-1.3.0/evennia/game_template/server/conf/connection_screens.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/inlinefuncs.py` & `evennia-1.3.0/evennia/game_template/server/conf/inlinefuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/inputfuncs.py` & `evennia-1.3.0/evennia/game_template/server/conf/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/lockfuncs.py` & `evennia-1.3.0/evennia/game_template/server/conf/lockfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/mssp.py` & `evennia-1.3.0/evennia/game_template/server/conf/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/portal_services_plugins.py` & `evennia-1.3.0/evennia/game_template/server/conf/portal_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/secret_settings.py` & `evennia-1.3.0/evennia/game_template/server/conf/secret_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/server_services_plugins.py` & `evennia-1.3.0/evennia/game_template/server/conf/server_services_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/serversession.py` & `evennia-1.3.0/evennia/game_template/server/conf/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/settings.py` & `evennia-1.3.0/evennia/game_template/server/conf/settings.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/conf/web_plugins.py` & `evennia-1.3.0/evennia/game_template/server/conf/web_plugins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/server/logs/README.md` & `evennia-1.3.0/evennia/game_template/server/logs/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/README.md` & `evennia-1.3.0/evennia/game_template/typeclasses/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/accounts.py` & `evennia-1.3.0/evennia/game_template/typeclasses/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/channels.py` & `evennia-1.3.0/evennia/game_template/typeclasses/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/characters.py` & `evennia-1.3.0/evennia/game_template/typeclasses/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/exits.py` & `evennia-1.3.0/evennia/game_template/typeclasses/exits.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/objects.py` & `evennia-1.3.0/evennia/game_template/typeclasses/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/rooms.py` & `evennia-1.3.0/evennia/game_template/typeclasses/rooms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/typeclasses/scripts.py` & `evennia-1.3.0/evennia/game_template/typeclasses/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/README.md` & `evennia-1.3.0/evennia/game_template/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/admin/urls.py` & `evennia-1.3.0/evennia/game_template/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/static/README.md` & `evennia-1.3.0/evennia/game_template/web/static/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/templates/README.md` & `evennia-1.3.0/evennia/game_template/web/templates/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/urls.py` & `evennia-1.3.0/evennia/game_template/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/webclient/README.md` & `evennia-1.3.0/evennia/game_template/web/webclient/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# Webclient Views 
+# Webclient Views
 
 The webclient is mainly controlled by Javascript directly in the browser, so
 you usually customize it via `mygame/web/static/webclient/js/` - files instead.
 
-There is very little you can change from here, unless you want to implement 
+There is very little you can change from here, unless you want to implement
 your very own client from scratch.
 
 ## On views
 
 A 'view' is python code (a function or callable class) responsible for
 producing a HTML page for a user to view in response for going to a given URL
 in their browser. In Evennia lingo, it's similar in function to a Command, with
@@ -15,9 +15,9 @@
 
 The urls.py file contains regular expressions that are run against the provided
 URL - when a match is found, the execution is passed to a view which is then
 responsible (usually) for producing the web page by filling in a _template_ - a
 HTML document that can have special tags in it that are replaced for dynamic
 content. It then returns the finished HTML page for the user to view.
 
-See the [Django docs on Views](https://docs.djangoproject.com/en/3.2/topics/http/views/) for 
+See the [Django docs on Views](https://docs.djangoproject.com/en/4.1/topics/http/views/) for
 more information.
```

### Comparing `evennia-1.2.1/evennia/game_template/web/webclient/urls.py` & `evennia-1.3.0/evennia/game_template/web/webclient/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/web/website/README.md` & `evennia-1.3.0/evennia/game_template/web/website/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-# Website views and other code 
+# Website views and other code
 
 A 'view' is python code (a function or callable class) responsible for
 producing a HTML page for a user to view in response for going to a given URL
 in their browser. In Evennia lingo, it's similar in function to a Command, with
 the input/args being the URL/request and the output being a new web-page.
 
 The urls.py file contains regular expressions that are run against the provided
 URL - when a match is found, the execution is passed to a view which is then
 responsible (usually) for producing the web page by filling in a _template_ - a
 HTML document that can have special tags in it that are replaced for dynamic
 content. It then returns the finished HTML page for the user to view.
 
-See the [Django docs on Views](https://docs.djangoproject.com/en/3.2/topics/http/views/) for 
+See the [Django docs on Views](https://docs.djangoproject.com/en/4.1/topics/http/views/) for
 more information.
 
 ## Overriding a view
 
-1. Copy the original code you want to change from `evennia/web/website/views/` into 
+1. Copy the original code you want to change from `evennia/web/website/views/` into
 `mygame/web/website/views/` and edit it as you like.
-2. Look at `evennia/web/website/urls.py` and find the regex pointing to the view. Add this regex 
+2. Look at `evennia/web/website/urls.py` and find the regex pointing to the view. Add this regex
 to your own `mygam/website/urls.pye` but change it to import and point to your
 changed version instead.
 3. Reload the server and the page now uses your version of the view.
```

### Comparing `evennia-1.2.1/evennia/game_template/world/batch_cmds.ev` & `evennia-1.3.0/evennia/game_template/world/batch_cmds.ev`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/world/help_entries.py` & `evennia-1.3.0/evennia/game_template/world/help_entries.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/game_template/world/prototypes.py` & `evennia-1.3.0/evennia/game_template/world/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/filehelp.py` & `evennia-1.3.0/evennia/help/filehelp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/manager.py` & `evennia-1.3.0/evennia/help/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/migrations/0001_initial.py` & `evennia-1.3.0/evennia/help/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/migrations/0002_auto_20170606_1731.py` & `evennia-1.3.0/evennia/help/migrations/0002_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/migrations/0003_auto_20190128_1820.py` & `evennia-1.3.0/evennia/help/migrations/0003_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/migrations/0004_auto_20210520_2137.py` & `evennia-1.3.0/evennia/help/migrations/0004_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/migrations/0005_auto_20210530_1818.py` & `evennia-1.3.0/evennia/help/migrations/0005_auto_20210530_1818.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/models.py` & `evennia-1.3.0/evennia/help/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/tests.py` & `evennia-1.3.0/evennia/help/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/help/utils.py` & `evennia-1.3.0/evennia/help/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/README` & `evennia-1.3.0/evennia/locale/README`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/de/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/de/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/es/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/es/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/fr/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/fr/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/it/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/it/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/ko/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/ko/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/la/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/la/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/pl/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/pl/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/pt/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/pt/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/ru/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/ru/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/sv/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/sv/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/zh/LC_MESSAGES/django.mo` & `evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locale/zh/LC_MESSAGES/django.po` & `evennia-1.3.0/evennia/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locks/lockfuncs.py` & `evennia-1.3.0/evennia/locks/lockfuncs.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,26 +507,32 @@
 
 def is_ooc(accessing_obj, accessed_obj, *args, **kwargs):
     """
     Usage:
         is_ooc()
 
     This is normally used to lock a Command, so it can be used
-    only when out of character.
+    only when out of character. When not logged in at all, this
+    function will still return True.
     """
     obj = accessed_obj.obj if hasattr(accessed_obj, "obj") else accessed_obj
     account = obj.account if hasattr(obj, "account") else obj
     if not account:
         return True
     try:
         session = accessed_obj.session
     except AttributeError:
-        session = account.sessions.get()[0]  # note-this doesn't work well
+        # note-this doesn't work well
         # for high multisession mode. We may need
         # to change to sessiondb to resolve this
+        sessions = session = account.sessions.get()
+        session = sessions[0] if sessions else None
+    if not session:
+        # this suggests we are not even logged in; treat as ooc.
+        return True
     try:
         return not account.get_puppet(session)
     except TypeError:
         return not session.get_puppet()
 
 
 def objtag(accessing_obj, accessed_obj, *args, **kwargs):
```

### Comparing `evennia-1.2.1/evennia/locks/lockhandler.py` & `evennia-1.3.0/evennia/locks/lockhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/locks/tests.py` & `evennia-1.3.0/evennia/locks/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/manager.py` & `evennia-1.3.0/evennia/objects/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0001_initial.py` & `evennia-1.3.0/evennia/objects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0002_auto_20140917_0756.py` & `evennia-1.3.0/evennia/objects/migrations/0002_auto_20140917_0756.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py` & `evennia-1.3.0/evennia/objects/migrations/0003_defaultcharacter_defaultexit_defaultobject_defaultroom.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0004_auto_20150118_1622.py` & `evennia-1.3.0/evennia/objects/migrations/0004_auto_20150118_1622.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0006_auto_20170606_1731.py` & `evennia-1.3.0/evennia/objects/migrations/0006_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0007_objectdb_db_account.py` & `evennia-1.3.0/evennia/objects/migrations/0007_objectdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0008_auto_20170705_1736.py` & `evennia-1.3.0/evennia/objects/migrations/0008_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0009_remove_objectdb_db_player.py` & `evennia-1.3.0/evennia/objects/migrations/0009_remove_objectdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0010_auto_20190128_1820.py` & `evennia-1.3.0/evennia/objects/migrations/0010_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0011_auto_20191025_0831.py` & `evennia-1.3.0/evennia/objects/migrations/0011_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py` & `evennia-1.3.0/evennia/objects/migrations/0012_convert_contrib_typeclass_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/models.py` & `evennia-1.3.0/evennia/objects/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/objects.py` & `evennia-1.3.0/evennia/objects/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/objects/tests.py` & `evennia-1.3.0/evennia/objects/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/prototypes/README.md` & `evennia-1.3.0/evennia/prototypes/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/prototypes/menus.py` & `evennia-1.3.0/evennia/prototypes/menus.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/prototypes/protfuncs.py` & `evennia-1.3.0/evennia/prototypes/protfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/prototypes/prototypes.py` & `evennia-1.3.0/evennia/prototypes/prototypes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/prototypes/spawner.py` & `evennia-1.3.0/evennia/prototypes/spawner.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/prototypes/tests.py` & `evennia-1.3.0/evennia/prototypes/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/manager.py` & `evennia-1.3.0/evennia/scripts/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0001_initial.py` & `evennia-1.3.0/evennia/scripts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0002_auto_20150118_1625.py` & `evennia-1.3.0/evennia/scripts/migrations/0002_auto_20150118_1625.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py` & `evennia-1.3.0/evennia/scripts/migrations/0003_checksessions_defaultscript_donothing_scriptbase_store_validatechannelhandler_validateidmappercache_.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0004_auto_20150306_1354.py` & `evennia-1.3.0/evennia/scripts/migrations/0004_auto_20150306_1354.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0006_auto_20150310_2249.py` & `evennia-1.3.0/evennia/scripts/migrations/0006_auto_20150310_2249.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0008_auto_20170606_1731.py` & `evennia-1.3.0/evennia/scripts/migrations/0008_auto_20170606_1731.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0009_scriptdb_db_account.py` & `evennia-1.3.0/evennia/scripts/migrations/0009_scriptdb_db_account.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0010_auto_20170705_1736.py` & `evennia-1.3.0/evennia/scripts/migrations/0010_auto_20170705_1736.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py` & `evennia-1.3.0/evennia/scripts/migrations/0011_remove_scriptdb_db_player.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0012_auto_20190128_1820.py` & `evennia-1.3.0/evennia/scripts/migrations/0012_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0013_auto_20191025_0831.py` & `evennia-1.3.0/evennia/scripts/migrations/0013_auto_20191025_0831.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0014_auto_20210520_2137.py` & `evennia-1.3.0/evennia/scripts/migrations/0014_auto_20210520_2137.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/migrations/0015_convert_contrib_paths.py` & `evennia-1.3.0/evennia/scripts/migrations/0015_convert_contrib_paths.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/models.py` & `evennia-1.3.0/evennia/scripts/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/monitorhandler.py` & `evennia-1.3.0/evennia/scripts/monitorhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/scripthandler.py` & `evennia-1.3.0/evennia/scripts/scripthandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/scripts.py` & `evennia-1.3.0/evennia/scripts/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/taskhandler.py` & `evennia-1.3.0/evennia/scripts/taskhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/scripts/tickerhandler.py` & `evennia-1.3.0/evennia/scripts/tickerhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/amp_client.py` & `evennia-1.3.0/evennia/server/amp_client.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/connection_wizard.py` & `evennia-1.3.0/evennia/server/connection_wizard.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/deprecations.py` & `evennia-1.3.0/evennia/server/deprecations.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/evennia_launcher.py` & `evennia-1.3.0/evennia/server/evennia_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/game_index_client/README.md` & `evennia-1.3.0/evennia/server/game_index_client/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/game_index_client/client.py` & `evennia-1.3.0/evennia/server/game_index_client/client.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/game_index_client/service.py` & `evennia-1.3.0/evennia/server/game_index_client/service.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/initial_setup.py` & `evennia-1.3.0/evennia/server/initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/inputfuncs.py` & `evennia-1.3.0/evennia/server/inputfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/manager.py` & `evennia-1.3.0/evennia/server/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/migrations/0001_initial.py` & `evennia-1.3.0/evennia/server/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/migrations/0002_auto_20190128_2311.py` & `evennia-1.3.0/evennia/server/migrations/0002_auto_20190128_2311.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/models.py` & `evennia-1.3.0/evennia/server/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/amp.py` & `evennia-1.3.0/evennia/server/portal/amp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/amp_server.py` & `evennia-1.3.0/evennia/server/portal/amp_server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/discord.py` & `evennia-1.3.0/evennia/server/portal/discord.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/grapevine.py` & `evennia-1.3.0/evennia/server/portal/grapevine.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/irc.py` & `evennia-1.3.0/evennia/server/portal/irc.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/mccp.py` & `evennia-1.3.0/evennia/server/portal/mccp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/mssp.py` & `evennia-1.3.0/evennia/server/portal/mssp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/mxp.py` & `evennia-1.3.0/evennia/server/portal/mxp.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/naws.py` & `evennia-1.3.0/evennia/server/portal/naws.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/portal.py` & `evennia-1.3.0/evennia/server/portal/portal.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/portalsessionhandler.py` & `evennia-1.3.0/evennia/server/portal/portalsessionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/rss.py` & `evennia-1.3.0/evennia/server/portal/rss.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/ssh.py` & `evennia-1.3.0/evennia/server/portal/ssh.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/ssl.py` & `evennia-1.3.0/evennia/server/portal/ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/suppress_ga.py` & `evennia-1.3.0/evennia/server/portal/suppress_ga.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/telnet.py` & `evennia-1.3.0/evennia/server/portal/telnet.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/telnet_oob.py` & `evennia-1.3.0/evennia/server/portal/telnet_oob.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/telnet_ssl.py` & `evennia-1.3.0/evennia/server/portal/telnet_ssl.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/tests.py` & `evennia-1.3.0/evennia/server/portal/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/ttype.py` & `evennia-1.3.0/evennia/server/portal/ttype.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/webclient.py` & `evennia-1.3.0/evennia/server/portal/webclient.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/portal/webclient_ajax.py` & `evennia-1.3.0/evennia/server/portal/webclient_ajax.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/dummyrunner.py` & `evennia-1.3.0/evennia/server/profiling/dummyrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/dummyrunner_settings.py` & `evennia-1.3.0/evennia/server/profiling/dummyrunner_settings.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/memplot.py` & `evennia-1.3.0/evennia/server/profiling/memplot.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/settings_mixin.py` & `evennia-1.3.0/evennia/server/profiling/settings_mixin.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/test_queries.py` & `evennia-1.3.0/evennia/server/profiling/test_queries.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/tests.py` & `evennia-1.3.0/evennia/server/profiling/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/profiling/timetrace.py` & `evennia-1.3.0/evennia/server/profiling/timetrace.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/server.py` & `evennia-1.3.0/evennia/server/server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/serversession.py` & `evennia-1.3.0/evennia/server/serversession.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/session.py` & `evennia-1.3.0/evennia/server/session.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/sessionhandler.py` & `evennia-1.3.0/evennia/server/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/signals.py` & `evennia-1.3.0/evennia/server/signals.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,33 +87,27 @@
 # first created, after all hooks.
 SIGNAL_CHANNEL_POST_CREATE = Signal()
 
 # The sender is the exit used when traversing, as well as 'traverser', for the one traversing
 # Called just after at_traverse hook.
 SIGNAL_EXIT_TRAVERSED = Signal()
 
-# Django default signals (https://docs.djangoproject.com/en/2.2/topics/signals/)
+# Django default signals (https://docs.djangoproject.com/en/4.1/topics/signals/)
 
 from django.core.signals import request_finished  # "             ends.
 from django.core.signals import request_started  # Sent when HTTP request begins.
-from django.db.backends.signals import (  # Sent when making initial connection to database
+from django.db.backends.signals import (
     connection_created,
-)
+)  # Sent when making initial connection to database
 from django.db.models.signals import m2m_changed  # Sent when a ManyToManyField changes.
 from django.db.models.signals import post_delete  # after         "
 from django.db.models.signals import post_init  # end
 from django.db.models.signals import post_migrate  # after     "
 from django.db.models.signals import post_save  # after            "
 from django.db.models.signals import pre_delete  # Sent before an object is deleted.
 from django.db.models.signals import pre_migrate  # Sent before migration starts
+from django.db.models.signals import pre_save  # Sent before a typeclass' .save is called.
 from django.db.models.signals import (
-    pre_save,  # Sent before a typeclass' .save is called.
-)
-from django.db.models.signals import (  # Sent at start of typeclass __init__ (before at_init)
     pre_init,
-)
-from django.test.signals import (
-    setting_changed,  # Sent when setting changes from override
-)
-from django.test.signals import (
-    template_rendered,  # Sent when test system renders template
-)
+)  # Sent at start of typeclass __init__ (before at_init)
+from django.test.signals import setting_changed  # Sent when setting changes from override
+from django.test.signals import template_rendered  # Sent when test system renders template
```

### Comparing `evennia-1.2.1/evennia/server/tests/test_amp_connection.py` & `evennia-1.3.0/evennia/server/tests/test_amp_connection.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/tests/test_initial_setup.py` & `evennia-1.3.0/evennia/server/tests/test_initial_setup.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/tests/test_launcher.py` & `evennia-1.3.0/evennia/server/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/tests/test_misc.py` & `evennia-1.3.0/evennia/server/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/tests/test_server.py` & `evennia-1.3.0/evennia/server/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/tests/testrunner.py` & `evennia-1.3.0/evennia/server/tests/testrunner.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/throttle.py` & `evennia-1.3.0/evennia/server/throttle.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/server/validators.py` & `evennia-1.3.0/evennia/server/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.utils.translation import gettext as _
-
 from evennia.accounts.models import AccountDB
 
 
 class EvenniaUsernameAvailabilityValidator:
     """
     Checks to make sure a given username is not taken or otherwise reserved.
     """
@@ -20,15 +19,14 @@
             username (str): Username to validate
 
         Returns:
             None (None): None if password successfully validated,
                 raises ValidationError otherwise.
 
         """
-
         # Check guest list
         if settings.GUEST_LIST and username.lower() in (
             guest.lower() for guest in settings.GUEST_LIST
         ):
             raise ValidationError(
                 _("Sorry, that username is reserved."), code="evennia_username_reserved"
             )
@@ -41,16 +39,15 @@
             )
 
 
 class EvenniaPasswordValidator:
     def __init__(
         self,
         regex=r"^[\w. @+\-',]+$",
-        policy="Password should contain a mix of letters, "
-        "spaces, digits and @/./+/-/_/'/, only.",
+        policy="Password should contain a mix of letters, spaces, digits and @/./+/-/_/'/, only.",
     ):
         """
         Constructs a standard Django password validator.
 
         Args:
             regex (str): Regex pattern of valid characters to allow.
             policy (str): Brief explanation of what the defined regex permits.
```

### Comparing `evennia-1.2.1/evennia/server/webserver.py` & `evennia-1.3.0/evennia/server/webserver.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/settings_default.py` & `evennia-1.3.0/evennia/settings_default.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # visible location. This is used e.g. on the web site to show how you connect to the
 # game over telnet. Default is localhost (only on your machine).
 SERVER_HOSTNAME = "localhost"
 # Lockdown mode will cut off the game from any external connections
 # and only allow connections from localhost. Requires a cold reboot.
 LOCKDOWN_MODE = False
 # Controls whether new account registration is available.
-# Set to False to lock down the registration page and the create account command. 
+# Set to False to lock down the registration page and the create account command.
 NEW_ACCOUNT_REGISTRATION_ENABLED = True
 # Activate telnet service
 TELNET_ENABLED = True
 # A list of ports the Evennia telnet server listens on Can be one or many.
 TELNET_PORTS = [4000]
 # Interface addresses to listen to. If 0.0.0.0, listen to all. Use :: for IPv6.
 TELNET_INTERFACES = ["0.0.0.0"]
@@ -994,15 +994,15 @@
             ],
             # While true, show "pretty" error messages for template syntax errors.
             "debug": DEBUG,
         },
     }
 ]
 # Django cache settings
-# https://docs.djangoproject.com/en/dev/topics/cache/#setting-up-the-cache
+# https://docs.djangoproject.com/en/4.1/topics/cache/#setting-up-the-cache
 CACHES = {
     "default": {
         "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
     },
     "throttle": {
         "BACKEND": "django.core.cache.backends.locmem.LocMemCache",
         "TIMEOUT": 60 * 5,
@@ -1053,15 +1053,15 @@
     "evennia.web",
 ]
 # The user profile extends the User object with more functionality;
 # This should usually not be changed.
 AUTH_USER_MODEL = "accounts.AccountDB"
 
 # Password validation plugins
-# https://docs.djangoproject.com/en/1.11/ref/settings/#auth-password-validators
+# https://docs.djangoproject.com/en/4.1/ref/settings/#auth-password-validators
 AUTH_PASSWORD_VALIDATORS = [
     {"NAME": "django.contrib.auth.password_validation.UserAttributeSimilarityValidator"},
     {
         "NAME": "django.contrib.auth.password_validation.MinimumLengthValidator",
         "OPTIONS": {"min_length": 8},
     },
     {"NAME": "django.contrib.auth.password_validation.CommonPasswordValidator"},
```

### Comparing `evennia-1.2.1/evennia/typeclasses/attributes.py` & `evennia-1.3.0/evennia/typeclasses/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/managers.py` & `evennia-1.3.0/evennia/typeclasses/managers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0001_initial.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0002_auto_20150109_0913.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0002_auto_20150109_0913.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0003_defaultcharacter_defaultexit_defaultguest_defaultobject_defaultplayer_defaultroom_defaultscript_dono.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0004_auto_20151101_1759.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0004_auto_20151101_1759.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0005_auto_20160625_1812.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0005_auto_20160625_1812.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0006_auto_add_dbmodel_value_for_tags_attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0007_tag_migrations_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0008_lock_and_perm_rename.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0009_rename_player_cmdsets_typeclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0010_delete_old_player_tables.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0010_delete_old_player_tables.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0011_auto_20190128_1820.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0011_auto_20190128_1820.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0012_attrs_to_picklev4_may_be_slow.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0013_auto_20191015_1922.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0013_auto_20191015_1922.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0014_alter_tag_db_category.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0014_alter_tag_db_category.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py` & `evennia-1.3.0/evennia/typeclasses/migrations/0016_alter_attribute_id_alter_tag_id.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/models.py` & `evennia-1.3.0/evennia/typeclasses/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/tags.py` & `evennia-1.3.0/evennia/typeclasses/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/typeclasses/tests.py` & `evennia-1.3.0/evennia/typeclasses/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/ansi.py` & `evennia-1.3.0/evennia/utils/ansi.py`

 * *Files 6% similar despite different names*

```diff
@@ -328,85 +328,80 @@
             elif letter == "z":
                 colval = 231  # pure white @ index 231 (last color cube entry)
             else:
                 # letter in range [b..y] (exactly 24 values!)
                 colval = 134 + ord(letter)
 
             # ansi fallback logic expects r,g,b values in [0..5] range
-            gray = (ord(letter) - 97) / 5.0
+            gray = round((ord(letter) - 97) / 5.0)
             red, green, blue = gray, gray, gray
 
         if use_xterm256:
 
             if not grayscale:
                 colval = 16 + (red * 36) + (green * 6) + blue
 
             return "\033[%s8;5;%sm" % (3 + int(background), colval)
             # replaced since some clients (like Potato) does not accept codes with leading zeroes,
             # see issue #1024.
             # return "\033[%s8;5;%s%s%sm" % (3 + int(background), colval // 100, (colval % 100) // 10, colval%10)  # noqa
 
         else:
             # xterm256 not supported, convert the rgb value to ansi instead
-            if red == green == blue and red < 3:
-                if background:
-                    return ANSI_BACK_BLACK
-                elif red >= 1:
-                    return ANSI_HILITE + ANSI_BLACK
-                else:
-                    return ANSI_NORMAL + ANSI_BLACK
-            elif red == green == blue:
-                if background:
-                    return ANSI_BACK_WHITE
-                elif red >= 4:
-                    return ANSI_HILITE + ANSI_WHITE
-                else:
-                    return ANSI_NORMAL + ANSI_WHITE
-            elif red > green and red > blue:
-                if background:
-                    return ANSI_BACK_RED
-                elif red >= 3:
-                    return ANSI_HILITE + ANSI_RED
-                else:
-                    return ANSI_NORMAL + ANSI_RED
-            elif red == green and red > blue:
-                if background:
-                    return ANSI_BACK_YELLOW
-                elif red >= 3:
-                    return ANSI_HILITE + ANSI_YELLOW
-                else:
-                    return ANSI_NORMAL + ANSI_YELLOW
-            elif red == blue and red > green:
-                if background:
-                    return ANSI_BACK_MAGENTA
-                elif red >= 3:
-                    return ANSI_HILITE + ANSI_MAGENTA
-                else:
-                    return ANSI_NORMAL + ANSI_MAGENTA
-            elif green > blue:
-                if background:
-                    return ANSI_BACK_GREEN
-                elif green >= 3:
-                    return ANSI_HILITE + ANSI_GREEN
-                else:
-                    return ANSI_NORMAL + ANSI_GREEN
-            elif green == blue:
-                if background:
-                    return ANSI_BACK_CYAN
-                elif green >= 3:
-                    return ANSI_HILITE + ANSI_CYAN
-                else:
-                    return ANSI_NORMAL + ANSI_CYAN
-            else:  # mostly blue
-                if background:
-                    return ANSI_BACK_BLUE
-                elif blue >= 3:
-                    return ANSI_HILITE + ANSI_BLUE
-                else:
-                    return ANSI_NORMAL + ANSI_BLUE
+            rgb = (red, green, blue)
+	
+            def _convert_for_ansi(val):
+                return int((val+1)//2)
+
+            # greys
+            if (max(rgb) - min(rgb)) <= 1:
+                match rgb:
+                    case (0,0,0):
+                        return ANSI_BACK_BLACK if background else ANSI_NORMAL + ANSI_BLACK
+                    case ((1|2), (1|2), (1|2)):
+                        return ANSI_BACK_BLACK if background else ANSI_HILITE + ANSI_BLACK
+                    case ((2|3), (2|3), (2|3)):
+                        return ANSI_BACK_WHITE if background else ANSI_NORMAL + ANSI_WHITE
+                    case ((3|4), (3|4), (3|4)):
+                        return ANSI_BACK_WHITE if background else ANSI_NORMAL + ANSI_WHITE
+                    case ((4|5), (4|5), (4|5)):
+                        return ANSI_BACK_WHITE if background else ANSI_HILITE + ANSI_WHITE
+
+            match tuple(_convert_for_ansi(c) for c in rgb):
+                # red
+                case ((2|3), (0|1), (0|1)):
+                    return ANSI_BACK_RED if background else ANSI_HILITE + ANSI_RED
+                case ((1|2), 0, 0):
+                    return ANSI_BACK_RED if background else ANSI_NORMAL + ANSI_RED
+                # green
+                case ((0|1), (2|3), (0|1)):
+                    return ANSI_BACK_GREEN if background else ANSI_HILITE + ANSI_GREEN
+                case ((0 | 1), 1, 0) if green > red:
+                    return ANSI_BACK_GREEN if background else ANSI_NORMAL + ANSI_GREEN
+                # blue
+                case ((0|1), (0|1), (2|3)):
+                    return ANSI_BACK_BLUE if background else ANSI_HILITE + ANSI_BLUE
+                case (0, 0, 1):
+                    return ANSI_BACK_BLUE if background else ANSI_NORMAL + ANSI_BLUE
+                # cyan
+                case ((0|1|2), (2|3), (2|3)) if red == min(rgb):
+                    return ANSI_BACK_CYAN if background else ANSI_HILITE + ANSI_CYAN
+                case (0, (1|2), (1|2)):
+                    return ANSI_BACK_CYAN if background else ANSI_NORMAL + ANSI_CYAN
+                # yellow
+                case ((2|3), (2|3), (0|1|2)) if blue == min(rgb):
+                    return ANSI_BACK_YELLOW if background else ANSI_HILITE + ANSI_YELLOW
+                case ((2|1), (2|1), (0|1)):
+                    return ANSI_BACK_YELLOW if background else ANSI_NORMAL + ANSI_YELLOW
+                # magenta
+                case ((2|3), (0|1|2), (2|3)) if green == min(rgb):
+                    return ANSI_BACK_MAGENTA if background else ANSI_HILITE + ANSI_MAGENTA
+                case ((1|2), 0, (1|2)):
+                    return ANSI_BACK_MAGENTA if background else ANSI_NORMAL + ANSI_MAGENTA
+                
 
     def strip_raw_codes(self, string):
         """
         Strips raw ANSI codes from a string.
 
         Args:
             string (str): The string to strip.
```

### Comparing `evennia-1.2.1/evennia/utils/batchprocessors.py` & `evennia-1.3.0/evennia/utils/batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/containers.py` & `evennia-1.3.0/evennia/utils/containers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/create.py` & `evennia-1.3.0/evennia/utils/create.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/dbserialize.py` & `evennia-1.3.0/evennia/utils/dbserialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     from pickle import UnpicklingError, dumps, loads
 except ImportError:
     from pickle import dumps, loads
 
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ObjectDoesNotExist
 from django.utils.safestring import SafeString
-
 from evennia.utils import logger
 from evennia.utils.utils import is_iter, to_bytes, uses_database
 
 __all__ = ("to_pickle", "from_pickle", "do_pickle", "do_unpickle", "dbserialize", "dbunserialize")
 
 PICKLE_PROTOCOL = 2
 
@@ -205,14 +204,16 @@
                 dat = _SaverDict(_parent=parent)
                 dat._data.update((key, process_tree(val, dat)) for key, val in item.items())
                 return dat
             elif dtype == defaultdict:
                 dat = _SaverDefaultDict(item.default_factory, _parent=parent)
                 dat._data.update((key, process_tree(val, dat)) for key, val in item.items())
                 return dat
+            elif dtype == deque:
+                dat = _SaverDeque(_parent=parent, maxlen=item.maxlen)
             elif dtype == set:
                 dat = _SaverSet(_parent=parent)
                 dat._data.update(process_tree(val, dat) for val in item)
                 return dat
             return item
 
         return process_tree(data, self)
@@ -427,17 +428,17 @@
 
 
 class _SaverDeque(_SaverMutable):
     """
     A deque that can be saved and operated on.
     """
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, maxlen=None, **kwargs):
         super().__init__(*args, **kwargs)
-        self._data = deque()
+        self._data = deque((), maxlen=maxlen)
 
     @_save
     def append(self, *args, **kwargs):
         self._data.append(*args, **kwargs)
 
     @_save
     def appendleft(self, *args, **kwargs):
@@ -509,14 +510,16 @@
             return {_iter(key): _iter(val) for key, val in obj.items()}
         elif tname in ("_SaverOrderedDict", "OrderedDict"):
             return OrderedDict([(_iter(key), _iter(val)) for key, val in obj.items()])
         elif tname in ("_SaverDefaultDict", "defaultdict"):
             return defaultdict(
                 obj.default_factory, {_iter(key): _iter(val) for key, val in obj.items()}
             )
+        elif tname in ("_SaverDeque", deque):
+            return deque((_iter(val) for val in obj), maxlen=obj.maxlen)
         elif tname in _DESERIALIZE_MAPPING:
             return _DESERIALIZE_MAPPING[tname](_iter(val) for val in obj)
         elif is_iter(obj):
             return typ(_iter(val) for val in obj)
         return obj
 
     return _iter(obj)
@@ -676,14 +679,16 @@
         elif dtype in (dict, _SaverDict):
             return dict((process_item(key), process_item(val)) for key, val in item.items())
         elif dtype in (defaultdict, _SaverDefaultDict):
             return defaultdict(
                 item.default_factory,
                 ((process_item(key), process_item(val)) for key, val in item.items()),
             )
+        elif dtype in (deque, _SaverDeque):
+            return deque((process_item(val) for val in item), maxlen=item.maxlen)
         elif dtype in (set, _SaverSet):
             return set(process_item(val) for val in item)
         elif dtype in (OrderedDict, _SaverOrderedDict):
             return OrderedDict((process_item(key), process_item(val)) for key, val in item.items())
         elif dtype in (deque, _SaverDeque):
             return deque(process_item(val) for val in item)
 
@@ -772,15 +777,15 @@
                 ((process_item(key), process_item(val)) for key, val in item.items()),
             )
         elif dtype == set:
             return set(process_item(val) for val in item)
         elif dtype == OrderedDict:
             return OrderedDict((process_item(key), process_item(val)) for key, val in item.items())
         elif dtype == deque:
-            return deque(process_item(val) for val in item)
+            return deque((process_item(val) for val in item), maxlen=item.maxlen)
         elif hasattr(item, "__iter__"):
             try:
                 # we try to conserve the iterable class, if not convert to dict
                 try:
                     return item.__class__(
                         (process_item(key), process_item(val)) for key, val in item.items()
                     )
@@ -845,15 +850,15 @@
         elif dtype == OrderedDict:
             dat = _SaverOrderedDict(_parent=parent)
             dat._data.update(
                 (process_item(key), process_tree(val, dat)) for key, val in item.items()
             )
             return dat
         elif dtype == deque:
-            dat = _SaverDeque(_parent=parent)
+            dat = _SaverDeque(_parent=parent, maxlen=item.maxlen)
             dat._data.extend(process_item(val) for val in item)
             return dat
         elif hasattr(item, "__iter__"):
             try:
                 # we try to conserve the iterable class, if not convert to dict
                 try:
                     dat = _SaverDict(_parent=parent, _class=item.__class__)
@@ -916,15 +921,15 @@
         elif dtype == OrderedDict:
             dat = _SaverOrderedDict(_db_obj=db_obj)
             dat._data.update(
                 (process_item(key), process_tree(val, dat)) for key, val in data.items()
             )
             return dat
         elif dtype == deque:
-            dat = _SaverDeque(_db_obj=db_obj)
+            dat = _SaverDeque(_db_obj=db_obj, maxlen=data.maxlen)
             dat._data.extend(process_item(val) for val in data)
             return dat
         elif hasattr(data, "__iter__"):
             try:
                 # we try to conserve the iterable class, if not convert to dict
                 try:
                     dat = _SaverDict(_db_obj=db_obj, _class=data.__class__)
```

### Comparing `evennia-1.2.1/evennia/utils/eveditor.py` & `evennia-1.3.0/evennia/utils/eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/evennia-mode.el` & `evennia-1.3.0/evennia/utils/evennia-mode.el`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/evform.py` & `evennia-1.3.0/evennia/utils/evform.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/evmenu.py` & `evennia-1.3.0/evennia/utils/evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/evmore.py` & `evennia-1.3.0/evennia/utils/evmore.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/evtable.py` & `evennia-1.3.0/evennia/utils/evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/funcparser.py` & `evennia-1.3.0/evennia/utils/funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/gametime.py` & `evennia-1.3.0/evennia/utils/gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/idmapper/LICENSE.md` & `evennia-1.3.0/evennia/utils/idmapper/LICENSE.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/idmapper/README_evennia.md` & `evennia-1.3.0/evennia/utils/idmapper/README_evennia.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/idmapper/README_orig.rst` & `evennia-1.3.0/evennia/utils/idmapper/README_orig.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 This fork of django-idmapper fixes some bugs that prevented the
 idmapper from being used in many instances. In particular, the caching
 manager is now inherited by SharedMemoryManager subclasses, and it is
 used when Django uses an automatic manager (see
-http://docs.djangoproject.com/en/dev/topics/db/managers/#controlling-automatic-manager-types).
+http://docs.djangoproject.com/en/4.1/topics/db/managers/#controlling-automatic-manager-types).
 This means access through foreign keys now uses identity mapping.
 
 Tested with Django version 1.2 alpha 1 SVN-12375.
 
 My modifications are usually accompanied by comments marked with "CL:".
 
 Django Identity Mapper
```

### Comparing `evennia-1.2.1/evennia/utils/idmapper/manager.py` & `evennia-1.3.0/evennia/utils/idmapper/manager.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/idmapper/models.py` & `evennia-1.3.0/evennia/utils/idmapper/models.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/idmapper/tests.py` & `evennia-1.3.0/evennia/utils/idmapper/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/logger.py` & `evennia-1.3.0/evennia/utils/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 _TIME_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 
 def _log(msg, logfunc, prefix="", **kwargs):
     try:
         msg = str(msg)
     except Exception as err:
-        msg = str(e)
+        msg = str(err)
     if kwargs:
         logfunc(msg, **kwargs)
     else:
         try:
             for line in msg.splitlines():
                 logfunc("{line}", prefix=prefix, line=line)
         except Exception as err:
```

### Comparing `evennia-1.2.1/evennia/utils/optionclasses.py` & `evennia-1.3.0/evennia/utils/optionclasses.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/optionhandler.py` & `evennia-1.3.0/evennia/utils/optionhandler.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/picklefield.py` & `evennia-1.3.0/evennia/utils/picklefield.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/search.py` & `evennia-1.3.0/evennia/utils/search.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/test_resources.py` & `evennia-1.3.0/evennia/utils/test_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -554,17 +554,27 @@
     """
 
 
 class EvenniaTestCase(TestCase):
     """
     For use with gamedir settings; Just like the normal test case, only for naming consistency.
 
+    Notes:
+
+    -   Inheriting from this class will bypass EvenniaTestMixin, and therefore
+        not setup some default objects. This can result in faster tests.
+
+    -   If you do inherit from this class for your unit tests, and have
+        overridden the tearDown() method, please also call flush_cache(). Not
+        doing so will result in flakey and order-dependent tests due to the
+        Django ID cache not being flushed.
     """
 
-    pass
+    def tearDown(self) -> None:
+        flush_cache()
 
 
 @override_settings(**DEFAULT_SETTINGS)
 class BaseEvenniaTest(EvenniaTestMixin, TestCase):
     """
     This class parent has all default objects and uses only default settings.
```

### Comparing `evennia-1.2.1/evennia/utils/tests/data/evform_example.py` & `evennia-1.3.0/evennia/utils/tests/data/evform_example.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/data/evmenu_example.py` & `evennia-1.3.0/evennia/utils/tests/data/evmenu_example.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_ansi.py` & `evennia-1.3.0/evennia/utils/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_batchprocessors.py` & `evennia-1.3.0/evennia/utils/tests/test_batchprocessors.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_containers.py` & `evennia-1.3.0/evennia/utils/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_create_functions.py` & `evennia-1.3.0/evennia/utils/tests/test_create_functions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_dbserialize.py` & `evennia-1.3.0/evennia/utils/tests/test_dbserialize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """
 Tests for dbserialize module
 """
 
 from collections import defaultdict, deque
 
 from django.test import TestCase
-from parameterized import parameterized
-
 from evennia.objects.objects import DefaultObject
 from evennia.utils import dbserialize
+from parameterized import parameterized
 
 
 class TestDbSerialize(TestCase):
     """
     Database serialization operations.
     """
 
@@ -112,14 +111,26 @@
         self.obj.db.test["a"].append(2)
         self.assertEqual(self.obj.db.test, {"a": [1, 2]})
         self.obj.db.test["a"].append(3)
         self.assertEqual(self.obj.db.test, {"a": [1, 2, 3]})
         self.obj.db.test |= {"b": [5, 6]}
         self.assertEqual(self.obj.db.test, {"a": [1, 2, 3], "b": [5, 6]})
 
+    def test_deque_with_maxlen(self):
+        _dd = deque((), maxlen=1)
+        _dd.append(1)
+        _dd.append(2)
+        self.assertEqual(list(_dd), [2])
+
+        dd = deque((), maxlen=1)
+        self.obj.db.test = dd
+        self.obj.db.test.append(1)
+        self.obj.db.test.append(2)
+        self.assertEqual(list(self.obj.db.test), [2])
+
 
 class _InvalidContainer:
     """Container not saveable in Attribute (if obj is dbobj, it 'hides' it)"""
 
     def __init__(self, obj):
         self.hidden_obj = obj
```

### Comparing `evennia-1.2.1/evennia/utils/tests/test_eveditor.py` & `evennia-1.3.0/evennia/utils/tests/test_eveditor.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_evform.py` & `evennia-1.3.0/evennia/utils/tests/test_evform.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_evmenu.py` & `evennia-1.3.0/evennia/utils/tests/test_evmenu.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_evtable.py` & `evennia-1.3.0/evennia/utils/tests/test_evtable.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_funcparser.py` & `evennia-1.3.0/evennia/utils/tests/test_funcparser.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_gametime.py` & `evennia-1.3.0/evennia/utils/tests/test_gametime.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_search.py` & `evennia-1.3.0/evennia/utils/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_tagparsing.py` & `evennia-1.3.0/evennia/utils/tests/test_tagparsing.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_text2html.py` & `evennia-1.3.0/evennia/utils/tests/test_text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_utils.py` & `evennia-1.3.0/evennia/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/tests/test_validatorfuncs.py` & `evennia-1.3.0/evennia/utils/tests/test_validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/text2html.py` & `evennia-1.3.0/evennia/utils/text2html.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/utils.py` & `evennia-1.3.0/evennia/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,20 @@
 from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.core.validators import validate_email as django_validate_email
 from django.utils import timezone
 from django.utils.html import strip_tags
 from django.utils.translation import gettext as _
+from evennia.utils import logger
 from simpleeval import simple_eval
 from twisted.internet import reactor, threads
 from twisted.internet.defer import returnValue  # noqa - used as import target
 from twisted.internet.task import deferLater
 
-from evennia.utils import logger
-
 _MULTIMATCH_TEMPLATE = settings.SEARCH_MULTIMATCH_TEMPLATE
 _EVENNIA_DIR = settings.EVENNIA_DIR
 _GAME_DIR = settings.GAME_DIR
 _IS_MAIN_THREAD = threading.current_thread().name == "MainThread"
 
 ENCODINGS = settings.ENCODINGS
 
@@ -2552,20 +2551,22 @@
             pass
         else:
             if isinstance(value, (int, float)):
                 delay(value, _iterate, generator, caller=caller)
             elif isinstance(value, str):
                 if not caller:
                     raise ValueError(
-                        "To retrieve input from a @pausable method, that method "
-                        "must be called with a 'caller' argument)"
+                        "To use `result yield('prompt')` in an @interactive method, that "
+                        "method must have an argument named `caller`.)"
                     )
                 get_input(caller, value, _process_input, generator=generator)
             else:
-                raise ValueError("yield(val) in a @pausable method must have an int/float as arg.")
+                raise ValueError(
+                    "yield(val) in an @interactive method must have an int/float as arg."
+                )
 
     def decorator(*args, **kwargs):
         argnames = inspect.getfullargspec(func).args
         caller = None
         if "caller" in argnames:
             # we assume this is an object
             caller = args[argnames.index("caller")]
```

### Comparing `evennia-1.2.1/evennia/utils/validatorfuncs.py` & `evennia-1.3.0/evennia/utils/validatorfuncs.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/verb_conjugation/LICENSE.txt` & `evennia-1.3.0/evennia/utils/verb_conjugation/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/verb_conjugation/conjugate.py` & `evennia-1.3.0/evennia/utils/verb_conjugation/conjugate.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/verb_conjugation/pronouns.py` & `evennia-1.3.0/evennia/utils/verb_conjugation/pronouns.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/verb_conjugation/tests.py` & `evennia-1.3.0/evennia/utils/verb_conjugation/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/utils/verb_conjugation/verbs.txt` & `evennia-1.3.0/evennia/utils/verb_conjugation/verbs.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/README.md` & `evennia-1.3.0/evennia/web/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/accounts.py` & `evennia-1.3.0/evennia/web/admin/accounts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/attributes.py` & `evennia-1.3.0/evennia/web/admin/attributes.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/comms.py` & `evennia-1.3.0/evennia/web/admin/comms.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/frontpage.py` & `evennia-1.3.0/evennia/web/admin/frontpage.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/help.py` & `evennia-1.3.0/evennia/web/admin/help.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/objects.py` & `evennia-1.3.0/evennia/web/admin/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/scripts.py` & `evennia-1.3.0/evennia/web/admin/scripts.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/tags.py` & `evennia-1.3.0/evennia/web/admin/tags.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/urls.py` & `evennia-1.3.0/evennia/web/admin/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/admin/utils.py` & `evennia-1.3.0/evennia/web/admin/utils.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/README.md` & `evennia-1.3.0/evennia/web/api/README.md`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/filters.py` & `evennia-1.3.0/evennia/web/api/filters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/permissions.py` & `evennia-1.3.0/evennia/web/api/permissions.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/serializers.py` & `evennia-1.3.0/evennia/web/api/serializers.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/tests.py` & `evennia-1.3.0/evennia/web/api/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/urls.py` & `evennia-1.3.0/evennia/web/api/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/api/views.py` & `evennia-1.3.0/evennia/web/api/views.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/rest_framework/images/favicon.ico` & `evennia-1.3.0/evennia/web/static/rest_framework/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/css/goldenlayout.css` & `evennia-1.3.0/evennia/web/static/webclient/css/goldenlayout.css`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/css/webclient.css` & `evennia-1.3.0/evennia/web/static/webclient/css/webclient.css`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff` & `evennia-1.3.0/evennia/web/static/webclient/fonts/DejaVuSansMono-webfont.woff`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/evennia.js` & `evennia-1.3.0/evennia/web/static/webclient/js/evennia.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/clienthelp.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/clienthelp.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/default_in.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_in.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/default_out.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/default_out.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/font.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/font.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/goldenlayout.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/goldenlayout_default_config.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/history.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/history.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/hotbuttons.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/hotbuttons.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/html.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/html.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/iframe.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/iframe.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/message_routing.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/message_routing.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/multimedia.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/multimedia.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/notifications.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/notifications.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/oob.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/oob.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/options2.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/options2.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/popups.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/popups.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/plugins/text2html.js` & `evennia-1.3.0/evennia/web/static/webclient/js/plugins/text2html.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/js/webclient_gui.js` & `evennia-1.3.0/evennia/web/static/webclient/js/webclient_gui.js`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/webclient/media/notification.wav` & `evennia-1.3.0/evennia/web/static/webclient/media/notification.wav`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/website/css/website.css` & `evennia-1.3.0/evennia/web/static/website/css/website.css`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/website/images/evennia_logo.png` & `evennia-1.3.0/evennia/web/static/website/images/evennia_logo.png`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/website/images/evennia_logo_festive.png` & `evennia-1.3.0/evennia/web/static/website/images/evennia_logo_festive.png`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/static/website/images/favicon.ico` & `evennia-1.3.0/evennia/web/static/website/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/admin/app_list.html` & `evennia-1.3.0/evennia/web/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/admin/frontpage.html` & `evennia-1.3.0/evennia/web/templates/admin/frontpage.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/rest_framework/api.html` & `evennia-1.3.0/evennia/web/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/webclient/base.html` & `evennia-1.3.0/evennia/web/templates/webclient/base.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/webclient/webclient.html` & `evennia-1.3.0/evennia/web/templates/webclient/webclient.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/500.html` & `evennia-1.3.0/evennia/web/templates/website/500.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/_menu.html` & `evennia-1.3.0/evennia/web/templates/website/_menu.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/base.html` & `evennia-1.3.0/evennia/web/templates/website/base.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/channel_detail.html` & `evennia-1.3.0/evennia/web/templates/website/channel_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/channel_list.html` & `evennia-1.3.0/evennia/web/templates/website/channel_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/character_form.html` & `evennia-1.3.0/evennia/web/templates/website/character_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/character_list.html` & `evennia-1.3.0/evennia/web/templates/website/character_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/character_manage_list.html` & `evennia-1.3.0/evennia/web/templates/website/character_manage_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/generic_form.html` & `evennia-1.3.0/evennia/web/templates/website/generic_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/help_detail.html` & `evennia-1.3.0/evennia/web/templates/website/help_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/help_list.html` & `evennia-1.3.0/evennia/web/templates/website/help_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/index.html` & `evennia-1.3.0/evennia/web/templates/website/index.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/object_confirm_delete.html` & `evennia-1.3.0/evennia/web/templates/website/object_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/object_detail.html` & `evennia-1.3.0/evennia/web/templates/website/object_detail.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/object_list.html` & `evennia-1.3.0/evennia/web/templates/website/object_list.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/pagination.html` & `evennia-1.3.0/evennia/web/templates/website/pagination.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/logged_out.html` & `evennia-1.3.0/evennia/web/templates/website/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/login.html` & `evennia-1.3.0/evennia/web/templates/website/registration/login.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_change_done.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_change_form.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_reset_complete.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_reset_confirm.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_reset_done.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_reset_email.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/password_reset_form.html` & `evennia-1.3.0/evennia/web/templates/website/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/registration/register.html` & `evennia-1.3.0/evennia/web/templates/website/registration/register.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templates/website/tbi.html` & `evennia-1.3.0/evennia/web/templates/website/tbi.html`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/templatetags/addclass.py` & `evennia-1.3.0/evennia/web/templatetags/addclass.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/urls.py` & `evennia-1.3.0/evennia/web/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/adminsite.py` & `evennia-1.3.0/evennia/web/utils/adminsite.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/apache_wsgi.conf` & `evennia-1.3.0/evennia/web/utils/apache_wsgi.conf`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/backends.py` & `evennia-1.3.0/evennia/web/utils/backends.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/evennia_modpy_apache.conf` & `evennia-1.3.0/evennia/web/utils/evennia_modpy_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/evennia_wsgi_apache.conf` & `evennia-1.3.0/evennia/web/utils/evennia_wsgi_apache.conf`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/general_context.py` & `evennia-1.3.0/evennia/web/utils/general_context.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/middleware.py` & `evennia-1.3.0/evennia/web/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/utils/tests.py` & `evennia-1.3.0/evennia/web/utils/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/webclient/views.py` & `evennia-1.3.0/evennia/web/webclient/views.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/forms.py` & `evennia-1.3.0/evennia/web/website/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from django import forms
 from django.conf import settings
 from django.contrib.auth.forms import UserCreationForm, UsernameField
 from django.forms import ModelForm
 from django.utils.html import escape
-
 from evennia.utils import class_from_module
 
 
 class EvenniaForm(forms.Form):
     """
     This is a stock Django form, but modified so that all values provided
     through it are escaped (sanitized). Validation is performed by the fields
@@ -123,21 +122,21 @@
         help_text="Years since your birth.")
 
     Default input fields are generic single-line text boxes. You can control what
     sort of input field users will see by specifying a "widget." An example of
     this is used for the 'desc' field to show a Textarea box instead of a Textbox.
 
     For help in building out your form, please see:
-    https://docs.djangoproject.com/en/1.11/topics/forms/#building-a-form-in-django
+    https://docs.djangoproject.com/en/4.1/topics/forms/#building-a-form-in-django
 
     For more information on fields and their capabilities, see:
-    https://docs.djangoproject.com/en/1.11/ref/forms/fields/
+    https://docs.djangoproject.com/en/4.1/ref/forms/fields/
 
     For more on widgets, see:
-    https://docs.djangoproject.com/en/1.11/ref/forms/widgets/
+    https://docs.djangoproject.com/en/4.1/ref/forms/widgets/
 
     """
 
     class Meta:
         """
         This is a Django construct that provides additional configuration to
         the form.
```

### Comparing `evennia-1.2.1/evennia/web/website/tests.py` & `evennia-1.3.0/evennia/web/website/tests.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/urls.py` & `evennia-1.3.0/evennia/web/website/urls.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/views/accounts.py` & `evennia-1.3.0/evennia/web/website/views/accounts.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 
 
 from django.conf import settings
 from django.contrib import messages
 from django.http import HttpResponseRedirect
 from django.urls import reverse_lazy
-
 from evennia.utils import class_from_module
 from evennia.web.website import forms
 
 from .mixins import EvenniaCreateView, TypeclassMixin
 
 
 class AccountMixin(TypeclassMixin):
@@ -52,26 +51,20 @@
 
         """
         # Get values provided
         username = form.cleaned_data["username"]
         password = form.cleaned_data["password1"]
         email = form.cleaned_data.get("email", "")
 
-        # Create account
+        # Create account. This also runs all validations on the username/password.
         account, errs = self.typeclass.create(username=username, password=password, email=email)
 
-        # If unsuccessful, display error messages to user
         if not account:
-            [messages.error(self.request, err) for err in errs]
-
-            # Call the Django "form failure" hook
+            # password validation happens earlier, only username checks appear here.
+            form.add_error("username", ", ".join(errs))
             return self.form_invalid(form)
-
-        # Inform user of success
-        messages.success(
-            self.request,
-            "Your account '%s' was successfully created! "
-            "You may log in using it now." % account.name,
-        )
-
-        # Redirect the user to the login page
-        return HttpResponseRedirect(self.success_url)
+        else:
+            # Inform user of success
+            messages.success(
+                self.request, f"Your account '{account.name}' was successfully created!"
+            )
+            return HttpResponseRedirect(self.success_url)
```

### Comparing `evennia-1.2.1/evennia/web/website/views/channels.py` & `evennia-1.3.0/evennia/web/website/views/channels.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/views/characters.py` & `evennia-1.3.0/evennia/web/website/views/characters.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/views/help.py` & `evennia-1.3.0/evennia/web/website/views/help.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/views/index.py` & `evennia-1.3.0/evennia/web/website/views/index.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/views/mixins.py` & `evennia-1.3.0/evennia/web/website/views/mixins.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia/web/website/views/objects.py` & `evennia-1.3.0/evennia/web/website/views/objects.py`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia.egg-info/PKG-INFO` & `evennia-1.3.0/evennia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evennia
-Version: 1.2.1
+Version: 1.3.0
 Summary: A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc).
 Maintainer-email: Griatch <griatch@gmail.com>
 License: BSD
 Project-URL: Homepage, https://www.evennia.com
 Project-URL: Github, https://github.com/evennia/evennia
 Project-URL: Documentation, https://www.evennia.com/docs/latest/index.html
 Project-URL: Live Demo, https://demo.evennia.com/
```

### Comparing `evennia-1.2.1/evennia.egg-info/SOURCES.txt` & `evennia-1.3.0/evennia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/evennia.egg-info/requires.txt` & `evennia-1.3.0/evennia.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evennia-1.2.1/pyproject.toml` & `evennia-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evennia"
-version = "1.2.1"
+version = "1.3.0"
 maintainers = [{ name = "Griatch", email = "griatch@gmail.com" }]
 description = "A full-featured toolkit and server for text-based multiplayer games (MUDs, MU*, etc)."
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { text = "BSD" }
 keywords = [
   "MUD",
```

### Comparing `evennia-1.2.1/setup.py` & `evennia-1.3.0/setup.py`

 * *Files identical despite different names*

