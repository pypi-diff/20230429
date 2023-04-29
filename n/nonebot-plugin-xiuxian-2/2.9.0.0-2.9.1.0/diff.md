# Comparing `tmp/nonebot_plugin_xiuxian_2-2.9.0.0.tar.gz` & `tmp/nonebot_plugin_xiuxian_2-2.9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_xiuxian_2-2.9.0.0.tar", last modified: Tue Apr 25 04:15:56 2023, max compression
+gzip compressed data, was "nonebot_plugin_xiuxian_2-2.9.1.0.tar", last modified: Sat Apr 29 15:10:04 2023, max compression
```

## Comparing `nonebot_plugin_xiuxian_2-2.9.0.0.tar` & `nonebot_plugin_xiuxian_2-2.9.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.240272 nonebot_plugin_xiuxian_2-2.9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-25 04:15:56.240272 nonebot_plugin_xiuxian_2-2.9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.228272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/download_xiuxian_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/item_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/lay_out.py
--rw-r--r--   0 runner    (1001) docker     (123)    54783 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/player_fight.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/read_buff.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49555 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian2_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.232272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/
--rw-r--r--   0 runner    (1001) docker     (123)    72789 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.232272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_bank/
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.232272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_base/
--rw-r--r--   0 runner    (1001) docker     (123)    60905 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.232272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/
--rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.232272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_buff/
--rw-r--r--   0 runner    (1001) docker     (123)    45638 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.236272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/
--rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.236272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/
--rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.236272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.236272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/
--rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mix_elixir_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_opertion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.240272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/
--rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.240272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_sect/
--rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.240272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/
--rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py
--rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 04:15:56.232272 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-04-25 04:15:56.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-25 04:15:56.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 04:15:56.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 04:15:56.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-25 04:15:56.000000 nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 04:15:56.240272 nonebot_plugin_xiuxian_2-2.9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-25 04:15:45.000000 nonebot_plugin_xiuxian_2-2.9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.332736 nonebot_plugin_xiuxian_2-2.9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-29 15:10:04.332736 nonebot_plugin_xiuxian_2-2.9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/download_xiuxian_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/item_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/lay_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54783 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/player_fight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/read_buff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49555 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian2_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/
+-rw-r--r--   0 runner    (1001) docker     (123)    72789 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21934 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_base/
+-rw-r--r--   0 runner    (1001) docker     (123)    60905 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/
+-rw-r--r--   0 runner    (1001) docker     (123)    35642 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/
+-rw-r--r--   0 runner    (1001) docker     (123)    45638 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/
+-rw-r--r--   0 runner    (1001) docker     (123)    18822 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.324736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/
+-rw-r--r--   0 runner    (1001) docker     (123)    19054 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/
+-rw-r--r--   0 runner    (1001) docker     (123)    29072 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mix_elixir_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_opertion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/
+-rw-r--r--   0 runner    (1001) docker     (123)    20739 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/
+-rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.328736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/
+-rw-r--r--   0 runner    (1001) docker     (123)    24909 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:10:04.320736 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-29 15:10:04.000000 nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:10:04.332736 nonebot_plugin_xiuxian_2-2.9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-29 15:09:49.000000 nonebot_plugin_xiuxian_2-2.9.1.0/setup.py
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/PKG-INFO` & `nonebot_plugin_xiuxian_2-2.9.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_xiuxian_2
-Version: 2.9.0.0
+Version: 2.9.1.0
 Summary: 修仙插件
 Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat
 Author-email: 1242550160@qq.com
 Keywords: pip,nonebot2,文游,修仙
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,19 @@
 </p>
 </div>
 
 ## 📖 介绍
 
 一款适用于QQ群的修仙插件,设定征集中，有好的想法可以推送给我哦~~~
 
+
 ## 💿 安装
+
+详情可见 [文档](https://xiuxian.netlify.app/)
+
 ### 下载
 
 1. 通过包管理器安装，可以通过nb，pip，或者poetry等方式安装，以pip为例
 
 ```
 pip install nonebot_plugin_xiuxian_2 -U
 ```
@@ -52,15 +56,15 @@
 
 ```
 git clone https://ghproxy.com/https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 ```
 
 2、如果遇到问题，请先百度和查看下方的 【一些问题】
 
-3、如解决不了进交流群：760517008 提问，提问请贴上完整的日志
+3、如解决不了进交流群：[760517008](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008) 提问，提问请贴上完整的日志
 
 
 ## 配置文件
 1、配置文件一般在data/xiuxian文件夹下，自行按照json格式修改即可，一些字段的含义可以进群交流<br>
 2、子插件的配置会在插件运行后在子插件文件中生成config.json文件，该文件字段含义在同级目录的xxxconfig.py有备注。注意：修改配置只需要修改json即可，修改.py文件的话需要删除json文件才会生效，任何修改都需要重启bot<br>
 3.卡图下载地址：[卡图](https://cowtransfer.com/s/82b90d2b879d43):口令：k3jzr5，文件放置于data/xiuxian目录下<br>
 
@@ -75,15 +79,15 @@
 示例： {<br>
     "群123群号" : "对应发送消息的qq号"<br>
     "群456群号" ： ["对应发送消息的qq号1","对应发送消息的qq号2"]<br>
 }
 当后面qq号为一个字符串时为一对一，为列表时为多对一<br>
 ```
 ## 一些问题
-- 当为放置为plugins目录使用时，请修改根目录下__init__.py文件中的42行：src=''中的内容，填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
+
 - pip install的填这个
   ```
      plugins = ["nonebot_plugin_xiuxian_2"]
   ```
 - 手动安装的填这个
   ```
     plugin_dirs = ["nonebot_plugin_xiuxian_2"]
@@ -108,12 +112,12 @@
 
 
 # 🎉支持
 
 - 大家喜欢的话可以给这个项目点个star
 
 - 有bug、意见和建议都欢迎提交 [Issues](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2.0/issues) 
-- 或者联系进入QQ交流群：760517008
+- 或者联系进入QQ交流群：[760517008](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 - 3.0版本正在路上，敬请期待
 
 # 许可证
 本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_xiuxian_2 Version: 2.9.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_xiuxian_2 Version: 2.9.1.0 Summary:
 ä¿®ä»æä»¶ Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat Author-email: 1242550160@qq.com Keywords:
 pip,nonebot2,ææ¸¸,ä¿®ä» Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified) Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»2.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
                            [Python] [NoneBot] [pypi]
 ## ð ä»ç»
 ä¸æ¬¾éç¨äºQQç¾¤çä¿®ä»æä»¶,è®¾å®å¾éä¸­ï¼æå¥½çæ³æ³å¯ä»¥æ¨éç»æå¦~~~
-## ð¿ å®è£ ### ä¸è½½ 1.
+## ð¿ å®è£ è¯¦æå¯è§ [ææ¡£](https://xiuxian.netlify.app/) ### ä¸è½½
+1.
 éè¿åç®¡çå¨å®è£ï¼å¯ä»¥éè¿nbï¼pipï¼æèpoetryç­æ¹å¼å®è£ï¼ä»¥pipä¸ºä¾
 ``` pip install nonebot_plugin_xiuxian_2 -U ``` 2. æå¨å®è£(å»ºè®®) ``` git
 clone https://ghproxy.com/https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 ``` 2ãå¦æéå°é®é¢ï¼è¯·åç¾åº¦åæ¥çä¸æ¹ç ãä¸äºé®é¢ã
-3ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
+3ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼[760517008](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 æé®ï¼æé®è¯·è´´ä¸å®æ´çæ¥å¿ ## éç½®æä»¶
 1ãéç½®æä»¶ä¸è¬å¨data/
 xiuxianæä»¶å¤¹ä¸ï¼èªè¡æç§jsonæ ¼å¼ä¿®æ¹å³å¯ï¼ä¸äºå­æ®µçå«ä¹å¯ä»¥è¿ç¾¤äº¤æµ
 2ãå­æä»¶çéç½®ä¼å¨æä»¶è¿è¡åå¨å­æä»¶æä»¶ä¸­çæconfig.jsonæä»¶ï¼è¯¥æä»¶å­æ®µå«ä¹å¨åçº§ç®å½çxxxconfig.pyæå¤æ³¨ãæ³¨æï¼ä¿®æ¹éç½®åªéè¦ä¿®æ¹jsonå³å¯ï¼ä¿®æ¹.pyæä»¶çè¯éè¦å é¤jsonæä»¶æä¼çæï¼ä»»ä½ä¿®æ¹é½éè¦éå¯bot
 3.å¡å¾ä¸è½½å°åï¼[å¡å¾](https://cowtransfer.com/s/82b90d2b879d43):
 å£ä»¤ï¼k3jzr5ï¼æä»¶æ¾ç½®äºdata/xiuxianç®å½ä¸
 ## é£æ§éç½® ``` éç½®å°å:ä¿®ä»æä»¶ä¸xiuxian_config.py
@@ -34,25 +36,25 @@
 self.layout_bot_dict = {{}} # QQæè´è´£çç¾¤è{{ç¾¤ :bot}} å¶ä¸­ botç±»å
 []æstr
 ç¤ºä¾ï¼ {
 "ç¾¤123ç¾¤å·" : "å¯¹åºåéæ¶æ¯çqqå·"
 "ç¾¤456ç¾¤å·" ï¼
 ["å¯¹åºåéæ¶æ¯çqqå·1","å¯¹åºåéæ¶æ¯çqqå·2"]
 } å½åé¢qqå·ä¸ºä¸ä¸ªå­ç¬¦ä¸²æ¶ä¸ºä¸å¯¹ä¸ï¼ä¸ºåè¡¨æ¶ä¸ºå¤å¯¹ä¸
-``` ## ä¸äºé®é¢ -
-å½ä¸ºæ¾ç½®ä¸ºpluginsç®å½ä½¿ç¨æ¶ï¼è¯·ä¿®æ¹æ ¹ç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹ï¼å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸
-src='src.plugins.' å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ - pip installçå¡«è¿ä¸ª
-``` plugins = ["nonebot_plugin_xiuxian_2"] ``` - æå¨å®è£çå¡«è¿ä¸ª ```
-plugin_dirs = ["nonebot_plugin_xiuxian_2"] ``` æ `bot.py`ä¸­æ·»å  - pip
+``` ## ä¸äºé®é¢ - pip installçå¡«è¿ä¸ª ``` plugins =
+["nonebot_plugin_xiuxian_2"] ``` - æå¨å®è£çå¡«è¿ä¸ª ``` plugin_dirs =
+["nonebot_plugin_xiuxian_2"] ``` æ `bot.py`ä¸­æ·»å  - pip
 installçå¡«è¿ä¸ª ``` nonebot.load_plugin("nonebot_plugin_xiuxian_2") ``` -
 æå¨å®è£çå¡«è¿ä¸ª ``` nonebot.load_plugins("src/plugins",
 "nonebot_plugin_xiuxian_2") ``` # ð ç¹å«æè°¢ - [NoneBot2](https://
 github.com/nonebot/
 nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ï¼NBå¤©ä¸ç¬¬ä¸å¯ç±ã - [go-
 cqhttp](https://github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã
 - [nonebot_plugin_xiuxian](https://github.com/s52047qwas/
 nonebot_plugin_xiuxian)ï¼åçä¿®ä» # ðæ¯æ -
 å¤§å®¶åæ¬¢çè¯å¯ä»¥ç»è¿ä¸ªé¡¹ç®ç¹ä¸ªstar -
 æbugãæè§åå»ºè®®é½æ¬¢è¿æäº¤ [Issues](https://github.com/QingMuCat/
-nonebot_plugin_xiuxian_2.0/issues) - æèèç³»è¿å¥QQäº¤æµç¾¤ï¼760517008
+nonebot_plugin_xiuxian_2.0/issues) - æèèç³»è¿å¥QQäº¤æµç¾¤ï¼
+[760517008](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 - 3.0çæ¬æ­£å¨è·¯ä¸ï¼æ¬è¯·æå¾ # è®¸å¯è¯ æ¬é¡¹ç®ä½¿ç¨ [MIT](https:
 //choosealicense.com/licenses/mit/) ä½ä¸ºå¼æºè®¸å¯è¯
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/README.md` & `nonebot_plugin_xiuxian_2-2.9.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 </p>
 </div>
 
 ## 📖 介绍
 
 一款适用于QQ群的修仙插件,设定征集中，有好的想法可以推送给我哦~~~
 
+
 ## 💿 安装
+
+详情可见 [文档](https://xiuxian.netlify.app/)
+
 ### 下载
 
 1. 通过包管理器安装，可以通过nb，pip，或者poetry等方式安装，以pip为例
 
 ```
 pip install nonebot_plugin_xiuxian_2 -U
 ```
@@ -38,15 +42,15 @@
 
 ```
 git clone https://ghproxy.com/https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 ```
 
 2、如果遇到问题，请先百度和查看下方的 【一些问题】
 
-3、如解决不了进交流群：760517008 提问，提问请贴上完整的日志
+3、如解决不了进交流群：[760517008](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008) 提问，提问请贴上完整的日志
 
 
 ## 配置文件
 1、配置文件一般在data/xiuxian文件夹下，自行按照json格式修改即可，一些字段的含义可以进群交流<br>
 2、子插件的配置会在插件运行后在子插件文件中生成config.json文件，该文件字段含义在同级目录的xxxconfig.py有备注。注意：修改配置只需要修改json即可，修改.py文件的话需要删除json文件才会生效，任何修改都需要重启bot<br>
 3.卡图下载地址：[卡图](https://cowtransfer.com/s/82b90d2b879d43):口令：k3jzr5，文件放置于data/xiuxian目录下<br>
 
@@ -61,15 +65,15 @@
 示例： {<br>
     "群123群号" : "对应发送消息的qq号"<br>
     "群456群号" ： ["对应发送消息的qq号1","对应发送消息的qq号2"]<br>
 }
 当后面qq号为一个字符串时为一对一，为列表时为多对一<br>
 ```
 ## 一些问题
-- 当为放置为plugins目录使用时，请修改根目录下__init__.py文件中的42行：src=''中的内容，填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
+
 - pip install的填这个
   ```
      plugins = ["nonebot_plugin_xiuxian_2"]
   ```
 - 手动安装的填这个
   ```
     plugin_dirs = ["nonebot_plugin_xiuxian_2"]
@@ -94,12 +98,12 @@
 
 
 # 🎉支持
 
 - 大家喜欢的话可以给这个项目点个star
 
 - 有bug、意见和建议都欢迎提交 [Issues](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2.0/issues) 
-- 或者联系进入QQ交流群：760517008
+- 或者联系进入QQ交流群：[760517008](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 - 3.0版本正在路上，敬请期待
 
 # 许可证
 本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
```

#### html2text {}

```diff
@@ -1,20 +1,22 @@
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»2.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
                            [Python] [NoneBot] [pypi]
 ## ð ä»ç»
 ä¸æ¬¾éç¨äºQQç¾¤çä¿®ä»æä»¶,è®¾å®å¾éä¸­ï¼æå¥½çæ³æ³å¯ä»¥æ¨éç»æå¦~~~
-## ð¿ å®è£ ### ä¸è½½ 1.
+## ð¿ å®è£ è¯¦æå¯è§ [ææ¡£](https://xiuxian.netlify.app/) ### ä¸è½½
+1.
 éè¿åç®¡çå¨å®è£ï¼å¯ä»¥éè¿nbï¼pipï¼æèpoetryç­æ¹å¼å®è£ï¼ä»¥pipä¸ºä¾
 ``` pip install nonebot_plugin_xiuxian_2 -U ``` 2. æå¨å®è£(å»ºè®®) ``` git
 clone https://ghproxy.com/https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 ``` 2ãå¦æéå°é®é¢ï¼è¯·åç¾åº¦åæ¥çä¸æ¹ç ãä¸äºé®é¢ã
-3ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
+3ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼[760517008](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 æé®ï¼æé®è¯·è´´ä¸å®æ´çæ¥å¿ ## éç½®æä»¶
 1ãéç½®æä»¶ä¸è¬å¨data/
 xiuxianæä»¶å¤¹ä¸ï¼èªè¡æç§jsonæ ¼å¼ä¿®æ¹å³å¯ï¼ä¸äºå­æ®µçå«ä¹å¯ä»¥è¿ç¾¤äº¤æµ
 2ãå­æä»¶çéç½®ä¼å¨æä»¶è¿è¡åå¨å­æä»¶æä»¶ä¸­çæconfig.jsonæä»¶ï¼è¯¥æä»¶å­æ®µå«ä¹å¨åçº§ç®å½çxxxconfig.pyæå¤æ³¨ãæ³¨æï¼ä¿®æ¹éç½®åªéè¦ä¿®æ¹jsonå³å¯ï¼ä¿®æ¹.pyæä»¶çè¯éè¦å é¤jsonæä»¶æä¼çæï¼ä»»ä½ä¿®æ¹é½éè¦éå¯bot
 3.å¡å¾ä¸è½½å°åï¼[å¡å¾](https://cowtransfer.com/s/82b90d2b879d43):
 å£ä»¤ï¼k3jzr5ï¼æä»¶æ¾ç½®äºdata/xiuxianç®å½ä¸
 ## é£æ§éç½® ``` éç½®å°å:ä¿®ä»æä»¶ä¸xiuxian_config.py
@@ -27,25 +29,25 @@
 self.layout_bot_dict = {{}} # QQæè´è´£çç¾¤è{{ç¾¤ :bot}} å¶ä¸­ botç±»å
 []æstr
 ç¤ºä¾ï¼ {
 "ç¾¤123ç¾¤å·" : "å¯¹åºåéæ¶æ¯çqqå·"
 "ç¾¤456ç¾¤å·" ï¼
 ["å¯¹åºåéæ¶æ¯çqqå·1","å¯¹åºåéæ¶æ¯çqqå·2"]
 } å½åé¢qqå·ä¸ºä¸ä¸ªå­ç¬¦ä¸²æ¶ä¸ºä¸å¯¹ä¸ï¼ä¸ºåè¡¨æ¶ä¸ºå¤å¯¹ä¸
-``` ## ä¸äºé®é¢ -
-å½ä¸ºæ¾ç½®ä¸ºpluginsç®å½ä½¿ç¨æ¶ï¼è¯·ä¿®æ¹æ ¹ç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹ï¼å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸
-src='src.plugins.' å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ - pip installçå¡«è¿ä¸ª
-``` plugins = ["nonebot_plugin_xiuxian_2"] ``` - æå¨å®è£çå¡«è¿ä¸ª ```
-plugin_dirs = ["nonebot_plugin_xiuxian_2"] ``` æ `bot.py`ä¸­æ·»å  - pip
+``` ## ä¸äºé®é¢ - pip installçå¡«è¿ä¸ª ``` plugins =
+["nonebot_plugin_xiuxian_2"] ``` - æå¨å®è£çå¡«è¿ä¸ª ``` plugin_dirs =
+["nonebot_plugin_xiuxian_2"] ``` æ `bot.py`ä¸­æ·»å  - pip
 installçå¡«è¿ä¸ª ``` nonebot.load_plugin("nonebot_plugin_xiuxian_2") ``` -
 æå¨å®è£çå¡«è¿ä¸ª ``` nonebot.load_plugins("src/plugins",
 "nonebot_plugin_xiuxian_2") ``` # ð ç¹å«æè°¢ - [NoneBot2](https://
 github.com/nonebot/
 nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ï¼NBå¤©ä¸ç¬¬ä¸å¯ç±ã - [go-
 cqhttp](https://github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã
 - [nonebot_plugin_xiuxian](https://github.com/s52047qwas/
 nonebot_plugin_xiuxian)ï¼åçä¿®ä» # ðæ¯æ -
 å¤§å®¶åæ¬¢çè¯å¯ä»¥ç»è¿ä¸ªé¡¹ç®ç¹ä¸ªstar -
 æbugãæè§åå»ºè®®é½æ¬¢è¿æäº¤ [Issues](https://github.com/QingMuCat/
-nonebot_plugin_xiuxian_2.0/issues) - æèèç³»è¿å¥QQäº¤æµç¾¤ï¼760517008
+nonebot_plugin_xiuxian_2.0/issues) - æèèç³»è¿å¥QQäº¤æµç¾¤ï¼
+[760517008](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 - 3.0çæ¬æ­£å¨è·¯ä¸ï¼æ¬è¯·æå¾ # è®¸å¯è¯ æ¬é¡¹ç®ä½¿ç¨ [MIT](https:
 //choosealicense.com/licenses/mit/) ä½ä¸ºå¼æºè®¸å¯è¯
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/data_source.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/download_xiuxian_data.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/download_xiuxian_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/item_json.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/item_json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/lay_out.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/lay_out.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/player_fight.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/player_fight.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/read_buff.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/read_buff.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/utils.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian2_handle.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian2_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/back_util.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_back/backconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_bank/bankconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_base/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/bossconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/makeboss.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_boss/old_boss_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_buff/two_exp_cd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_config.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_all.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart/impart_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/impart_pk_uitls.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_impart_pk/xu_world.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/download.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/draw_user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_info/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_mixelixir/mixelixirutil.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_opertion.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_opertion.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/jsondata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/old_rift_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_rift/riftmake.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_sect/sectconfig.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/reward_data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/work_handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xiuxian_work/workmake.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2/xn_xiuxian_impart_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-xiuxian-2
-Version: 2.9.0.0
+Version: 2.9.1.0
 Summary: 修仙插件
 Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat
 Author-email: 1242550160@qq.com
 Keywords: pip,nonebot2,文游,修仙
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -35,15 +35,19 @@
 </p>
 </div>
 
 ## 📖 介绍
 
 一款适用于QQ群的修仙插件,设定征集中，有好的想法可以推送给我哦~~~
 
+
 ## 💿 安装
+
+详情可见 [文档](https://xiuxian.netlify.app/)
+
 ### 下载
 
 1. 通过包管理器安装，可以通过nb，pip，或者poetry等方式安装，以pip为例
 
 ```
 pip install nonebot_plugin_xiuxian_2 -U
 ```
@@ -52,15 +56,15 @@
 
 ```
 git clone https://ghproxy.com/https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 ```
 
 2、如果遇到问题，请先百度和查看下方的 【一些问题】
 
-3、如解决不了进交流群：760517008 提问，提问请贴上完整的日志
+3、如解决不了进交流群：[760517008](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008) 提问，提问请贴上完整的日志
 
 
 ## 配置文件
 1、配置文件一般在data/xiuxian文件夹下，自行按照json格式修改即可，一些字段的含义可以进群交流<br>
 2、子插件的配置会在插件运行后在子插件文件中生成config.json文件，该文件字段含义在同级目录的xxxconfig.py有备注。注意：修改配置只需要修改json即可，修改.py文件的话需要删除json文件才会生效，任何修改都需要重启bot<br>
 3.卡图下载地址：[卡图](https://cowtransfer.com/s/82b90d2b879d43):口令：k3jzr5，文件放置于data/xiuxian目录下<br>
 
@@ -75,15 +79,15 @@
 示例： {<br>
     "群123群号" : "对应发送消息的qq号"<br>
     "群456群号" ： ["对应发送消息的qq号1","对应发送消息的qq号2"]<br>
 }
 当后面qq号为一个字符串时为一对一，为列表时为多对一<br>
 ```
 ## 一些问题
-- 当为放置为plugins目录使用时，请修改根目录下__init__.py文件中的42行：src=''中的内容，填写的是存放插件的目录，一般情况下 src='src.plugins.'  如有不同请按照格式修改
+
 - pip install的填这个
   ```
      plugins = ["nonebot_plugin_xiuxian_2"]
   ```
 - 手动安装的填这个
   ```
     plugin_dirs = ["nonebot_plugin_xiuxian_2"]
@@ -108,12 +112,12 @@
 
 
 # 🎉支持
 
 - 大家喜欢的话可以给这个项目点个star
 
 - 有bug、意见和建议都欢迎提交 [Issues](https://github.com/QingMuCat/nonebot_plugin_xiuxian_2.0/issues) 
-- 或者联系进入QQ交流群：760517008
+- 或者联系进入QQ交流群：[760517008](http://qm.qq.com/cgi-bin/qm/qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 - 3.0版本正在路上，敬请期待
 
 # 许可证
 本项目使用 [MIT](https://choosealicense.com/licenses/mit/) 作为开源许可证
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-xiuxian-2 Version: 2.9.0.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-xiuxian-2 Version: 2.9.1.0 Summary:
 ä¿®ä»æä»¶ Home-page: https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 Author: QingmuCat Author-email: 1242550160@qq.com Keywords:
 pip,nonebot2,ææ¸¸,ä¿®ä» Platform: any Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: GNU General Public License
 v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified) Description-
 Content-Type: text/markdown
                              [NoneBotPluginLogo]
                               [NoneBotPluginText]
              # ä¿®ä»2.0 _â¨ QQç¾¤èä¿®ä»æå­æ¸¸æâ¨_ ð§¬
                 æä»¶ä¸»è¦ä¸ºå®ç°ç¾¤èä¿®ä»åè½ï¼ð
                            [Python] [NoneBot] [pypi]
 ## ð ä»ç»
 ä¸æ¬¾éç¨äºQQç¾¤çä¿®ä»æä»¶,è®¾å®å¾éä¸­ï¼æå¥½çæ³æ³å¯ä»¥æ¨éç»æå¦~~~
-## ð¿ å®è£ ### ä¸è½½ 1.
+## ð¿ å®è£ è¯¦æå¯è§ [ææ¡£](https://xiuxian.netlify.app/) ### ä¸è½½
+1.
 éè¿åç®¡çå¨å®è£ï¼å¯ä»¥éè¿nbï¼pipï¼æèpoetryç­æ¹å¼å®è£ï¼ä»¥pipä¸ºä¾
 ``` pip install nonebot_plugin_xiuxian_2 -U ``` 2. æå¨å®è£(å»ºè®®) ``` git
 clone https://ghproxy.com/https://github.com/QingMuCat/nonebot_plugin_xiuxian_2
 ``` 2ãå¦æéå°é®é¢ï¼è¯·åç¾åº¦åæ¥çä¸æ¹ç ãä¸äºé®é¢ã
-3ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼760517008
+3ãå¦è§£å³ä¸äºè¿äº¤æµç¾¤ï¼[760517008](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 æé®ï¼æé®è¯·è´´ä¸å®æ´çæ¥å¿ ## éç½®æä»¶
 1ãéç½®æä»¶ä¸è¬å¨data/
 xiuxianæä»¶å¤¹ä¸ï¼èªè¡æç§jsonæ ¼å¼ä¿®æ¹å³å¯ï¼ä¸äºå­æ®µçå«ä¹å¯ä»¥è¿ç¾¤äº¤æµ
 2ãå­æä»¶çéç½®ä¼å¨æä»¶è¿è¡åå¨å­æä»¶æä»¶ä¸­çæconfig.jsonæä»¶ï¼è¯¥æä»¶å­æ®µå«ä¹å¨åçº§ç®å½çxxxconfig.pyæå¤æ³¨ãæ³¨æï¼ä¿®æ¹éç½®åªéè¦ä¿®æ¹jsonå³å¯ï¼ä¿®æ¹.pyæä»¶çè¯éè¦å é¤jsonæä»¶æä¼çæï¼ä»»ä½ä¿®æ¹é½éè¦éå¯bot
 3.å¡å¾ä¸è½½å°åï¼[å¡å¾](https://cowtransfer.com/s/82b90d2b879d43):
 å£ä»¤ï¼k3jzr5ï¼æä»¶æ¾ç½®äºdata/xiuxianç®å½ä¸
 ## é£æ§éç½® ``` éç½®å°å:ä¿®ä»æä»¶ä¸xiuxian_config.py
@@ -34,25 +36,25 @@
 self.layout_bot_dict = {{}} # QQæè´è´£çç¾¤è{{ç¾¤ :bot}} å¶ä¸­ botç±»å
 []æstr
 ç¤ºä¾ï¼ {
 "ç¾¤123ç¾¤å·" : "å¯¹åºåéæ¶æ¯çqqå·"
 "ç¾¤456ç¾¤å·" ï¼
 ["å¯¹åºåéæ¶æ¯çqqå·1","å¯¹åºåéæ¶æ¯çqqå·2"]
 } å½åé¢qqå·ä¸ºä¸ä¸ªå­ç¬¦ä¸²æ¶ä¸ºä¸å¯¹ä¸ï¼ä¸ºåè¡¨æ¶ä¸ºå¤å¯¹ä¸
-``` ## ä¸äºé®é¢ -
-å½ä¸ºæ¾ç½®ä¸ºpluginsç®å½ä½¿ç¨æ¶ï¼è¯·ä¿®æ¹æ ¹ç®å½ä¸__init__.pyæä»¶ä¸­ç42è¡ï¼src=''ä¸­çåå®¹ï¼å¡«åçæ¯å­æ¾æä»¶çç®å½ï¼ä¸è¬æåµä¸
-src='src.plugins.' å¦æä¸åè¯·æç§æ ¼å¼ä¿®æ¹ - pip installçå¡«è¿ä¸ª
-``` plugins = ["nonebot_plugin_xiuxian_2"] ``` - æå¨å®è£çå¡«è¿ä¸ª ```
-plugin_dirs = ["nonebot_plugin_xiuxian_2"] ``` æ `bot.py`ä¸­æ·»å  - pip
+``` ## ä¸äºé®é¢ - pip installçå¡«è¿ä¸ª ``` plugins =
+["nonebot_plugin_xiuxian_2"] ``` - æå¨å®è£çå¡«è¿ä¸ª ``` plugin_dirs =
+["nonebot_plugin_xiuxian_2"] ``` æ `bot.py`ä¸­æ·»å  - pip
 installçå¡«è¿ä¸ª ``` nonebot.load_plugin("nonebot_plugin_xiuxian_2") ``` -
 æå¨å®è£çå¡«è¿ä¸ª ``` nonebot.load_plugins("src/plugins",
 "nonebot_plugin_xiuxian_2") ``` # ð ç¹å«æè°¢ - [NoneBot2](https://
 github.com/nonebot/
 nonebot2)ï¼æ¬æä»¶å®è£çå¼åæ¡æ¶ï¼NBå¤©ä¸ç¬¬ä¸å¯ç±ã - [go-
 cqhttp](https://github.com/Mrs4s/go-cqhttp)ï¼ç¨³å®å®åç CQHTTP å®ç°ã
 - [nonebot_plugin_xiuxian](https://github.com/s52047qwas/
 nonebot_plugin_xiuxian)ï¼åçä¿®ä» # ðæ¯æ -
 å¤§å®¶åæ¬¢çè¯å¯ä»¥ç»è¿ä¸ªé¡¹ç®ç¹ä¸ªstar -
 æbugãæè§åå»ºè®®é½æ¬¢è¿æäº¤ [Issues](https://github.com/QingMuCat/
-nonebot_plugin_xiuxian_2.0/issues) - æèèç³»è¿å¥QQäº¤æµç¾¤ï¼760517008
+nonebot_plugin_xiuxian_2.0/issues) - æèèç³»è¿å¥QQäº¤æµç¾¤ï¼
+[760517008](http://qm.qq.com/cgi-bin/qm/
+qr?_wv=1027&k=zIKrPPqNStgZnRtuLhiOv9woBQSMQurq&authKey=Nrqm0zDxYKP2Fon2MskbNRmZ588Rqm79lJvQyVYWtkh9vDFK1RGBK0UhqzehVyDw&noverify=0&group_code=760517008)
 - 3.0çæ¬æ­£å¨è·¯ä¸ï¼æ¬è¯·æå¾ # è®¸å¯è¯ æ¬é¡¹ç®ä½¿ç¨ [MIT](https:
 //choosealicense.com/licenses/mit/) ä½ä¸ºå¼æºè®¸å¯è¯
```

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt` & `nonebot_plugin_xiuxian_2-2.9.1.0/nonebot_plugin_xiuxian_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_xiuxian_2-2.9.0.0/setup.py` & `nonebot_plugin_xiuxian_2-2.9.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
     setuptools.setup(
     name='nonebot_plugin_xiuxian_2',
-    version='2.9.0.0',
+    version='2.9.1.0',
     author='QingmuCat',
     author_email='1242550160@qq.com',
     keywords=["pip", "nonebot2", "文游", "修仙"],
     url='https://github.com/QingMuCat/nonebot_plugin_xiuxian_2',
     description='''修仙插件''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

