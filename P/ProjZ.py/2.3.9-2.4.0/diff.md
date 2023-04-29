# Comparing `tmp/ProjZ.py-2.3.9.tar.gz` & `tmp/ProjZ.py-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.3.9.tar", last modified: Sat Apr 29 15:22:00 2023, max compression
+gzip compressed data, was "ProjZ.py-2.4.0.tar", last modified: Sat Apr 29 15:35:55 2023, max compression
```

## Comparing `ProjZ.py-2.3.9.tar` & `ProjZ.py-2.4.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.599010 ProjZ.py-2.3.9/
--rw-rw-rw-   0        0        0     3983 2023-04-29 15:22:00.599010 ProjZ.py-2.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.461537 ProjZ.py-2.3.9/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     3983 2023-04-29 15:22:00.000000 ProjZ.py-2.3.9/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2284 2023-04-29 15:22:00.000000 ProjZ.py-2.3.9/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 15:22:00.000000 ProjZ.py-2.3.9/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-29 15:22:00.000000 ProjZ.py-2.3.9/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 15:22:00.000000 ProjZ.py-2.3.9/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.466484 ProjZ.py-2.3.9/projz/
--rw-rw-rw-   0        0        0      112 2023-04-29 14:18:02.000000 ProjZ.py-2.3.9/projz/__init__.py
--rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.471507 ProjZ.py-2.3.9/projz/api/
--rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.475458 ProjZ.py-2.3.9/projz/api/control/
--rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/control/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/control/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.480330 ProjZ.py-2.3.9/projz/api/headers/
--rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/headers/__init__.py
--rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.3.9/projz/api/headers/abc_headers_provider.py
--rw-rw-rw-   0        0        0     2057 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/headers/headers_provider.py
--rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/request_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.484364 ProjZ.py-2.3.9/projz/api/secret/
--rw-rw-rw-   0        0        0      315 2023-04-29 15:21:00.000000 ProjZ.py-2.3.9/projz/api/secret/__init__.py
--rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.3.9/projz/api/secret/data.txt
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.488309 ProjZ.py-2.3.9/projz/api/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/util/__init__.py
--rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/api/util/copy_to_buffer_writer.py
--rw-rw-rw-   0        0        0    57254 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/client.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.518150 ProjZ.py-2.3.9/projz/enum/
--rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/__init__.py
--rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/auth_purpose.py
--rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/auth_type.py
--rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/chat_message_type.py
--rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/chat_query_type.py
--rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/chat_thread_type.py
--rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/circle_filter_type.py
--rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/circle_members_query_type.py
--rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/comment_type.py
--rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/content_region.py
--rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/currency_type.py
--rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/gender.py
--rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/object_type.py
--rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/party_query_type.py
--rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/upload_target.py
--rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/user_task_type.py
--rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/enum/ws_event_type.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.522139 ProjZ.py-2.3.9/projz/error/
--rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/error/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/error/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.571153 ProjZ.py-2.3.9/projz/model/
--rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/__init__.py
--rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/account.py
--rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/blocked_item_wrapper.py
--rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/blog.py
--rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/category.py
--rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/chat.py
--rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/chat_message.py
--rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/circle.py
--rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/comment.py
--rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/currency.py
--rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/default_background_media.py
--rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/dice.py
--rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/gift_box.py
--rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/link_info.py
--rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/media.py
--rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/member_title.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.574138 ProjZ.py-2.3.9/projz/model/parse/
--rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/parse/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/parse/parseutils.py
--rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/party.py
--rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/poll.py
--rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/qi_vote_full_info.py
--rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/qi_vote_info.py
--rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.582116 ProjZ.py-2.3.9/projz/model/response/
--rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/response/__init__.py
--rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/response/auth_result.py
--rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/response/member_titles_info.py
--rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/response/multi_invitation_code_info.py
--rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/rich_format.py
--rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/sticker.py
--rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/transfer_order.py
--rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/user.py
--rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/user_task.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.590028 ProjZ.py-2.3.9/projz/model/util/
--rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/util/__init__.py
--rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/util/paginated_list.py
--rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/util/rich_format_builder.py
--rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/util/rich_format_text_builder.py
--rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/model/wallet.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.593044 ProjZ.py-2.3.9/projz/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/util/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/util/subscription_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-29 15:22:00.597041 ProjZ.py-2.3.9/projz/websocket/
--rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/websocket/__init__.py
--rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.3.9/projz/websocket/websocket_listener.py
--rw-rw-rw-   0        0        0       42 2023-04-29 15:22:00.601294 ProjZ.py-2.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1929 2023-04-29 15:21:56.000000 ProjZ.py-2.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.173584 ProjZ.py-2.4.0/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 15:35:55.173584 ProjZ.py-2.4.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.945577 ProjZ.py-2.4.0/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 15:35:54.000000 ProjZ.py-2.4.0/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2284 2023-04-29 15:35:54.000000 ProjZ.py-2.4.0/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 15:35:54.000000 ProjZ.py-2.4.0/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-29 15:35:54.000000 ProjZ.py-2.4.0/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 15:35:54.000000 ProjZ.py-2.4.0/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.954635 ProjZ.py-2.4.0/projz/
+-rw-rw-rw-   0        0        0      112 2023-04-29 14:18:02.000000 ProjZ.py-2.4.0/projz/__init__.py
+-rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.963470 ProjZ.py-2.4.0/projz/api/
+-rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.969604 ProjZ.py-2.4.0/projz/api/control/
+-rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/control/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/control/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.978585 ProjZ.py-2.4.0/projz/api/headers/
+-rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/headers/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.4.0/projz/api/headers/abc_headers_provider.py
+-rw-rw-rw-   0        0        0     2328 2023-04-29 15:34:51.000000 ProjZ.py-2.4.0/projz/api/headers/headers_provider.py
+-rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/request_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.985599 ProjZ.py-2.4.0/projz/api/secret/
+-rw-rw-rw-   0        0        0      657 2023-04-29 15:34:51.000000 ProjZ.py-2.4.0/projz/api/secret/__init__.py
+-rw-rw-rw-   0        0        0    11964 2023-04-29 15:20:01.000000 ProjZ.py-2.4.0/projz/api/secret/data.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:54.993203 ProjZ.py-2.4.0/projz/api/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/util/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/api/util/copy_to_buffer_writer.py
+-rw-rw-rw-   0        0        0    57254 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/client.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.050735 ProjZ.py-2.4.0/projz/enum/
+-rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/auth_purpose.py
+-rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/auth_type.py
+-rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/chat_message_type.py
+-rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/chat_query_type.py
+-rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/chat_thread_type.py
+-rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/circle_filter_type.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/circle_members_query_type.py
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/comment_type.py
+-rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/content_region.py
+-rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/currency_type.py
+-rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/gender.py
+-rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/object_type.py
+-rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/party_query_type.py
+-rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/upload_target.py
+-rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/user_task_type.py
+-rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/enum/ws_event_type.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.061370 ProjZ.py-2.4.0/projz/error/
+-rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/error/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/error/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.139242 ProjZ.py-2.4.0/projz/model/
+-rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/account.py
+-rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/blocked_item_wrapper.py
+-rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/blog.py
+-rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/category.py
+-rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/chat.py
+-rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/chat_message.py
+-rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/circle.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/comment.py
+-rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/currency.py
+-rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/default_background_media.py
+-rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/dice.py
+-rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/gift_box.py
+-rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/link_info.py
+-rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/media.py
+-rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/member_title.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.141236 ProjZ.py-2.4.0/projz/model/parse/
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/parse/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/parse/parseutils.py
+-rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/party.py
+-rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/poll.py
+-rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/qi_vote_full_info.py
+-rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/qi_vote_info.py
+-rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.154811 ProjZ.py-2.4.0/projz/model/response/
+-rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/response/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/response/auth_result.py
+-rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/response/member_titles_info.py
+-rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/response/multi_invitation_code_info.py
+-rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/rich_format.py
+-rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/sticker.py
+-rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/transfer_order.py
+-rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/user.py
+-rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/user_task.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.164932 ProjZ.py-2.4.0/projz/model/util/
+-rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/util/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/util/paginated_list.py
+-rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/util/rich_format_builder.py
+-rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/util/rich_format_text_builder.py
+-rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/model/wallet.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.169594 ProjZ.py-2.4.0/projz/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/util/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/util/subscription_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-29 15:35:55.172586 ProjZ.py-2.4.0/projz/websocket/
+-rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/websocket/__init__.py
+-rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.4.0/projz/websocket/websocket_listener.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 15:35:55.186577 ProjZ.py-2.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1929 2023-04-29 15:35:51.000000 ProjZ.py-2.4.0/setup.py
```

### Comparing `ProjZ.py-2.3.9/PKG-INFO` & `ProjZ.py-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.9
+Version: 2.4.0
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.3.9/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.4.0/ProjZ.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.9
+Version: 2.4.0
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.3.9/ProjZ.py.egg-info/SOURCES.txt` & `ProjZ.py-2.4.0/ProjZ.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/README.md` & `ProjZ.py-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/__main__.py` & `ProjZ.py-2.4.0/projz/__main__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/api/control/rpc.py` & `ProjZ.py-2.4.0/projz/api/control/rpc.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/api/headers/abc_headers_provider.py` & `ProjZ.py-2.4.0/projz/api/headers/abc_headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/api/headers/headers_provider.py` & `ProjZ.py-2.4.0/projz/api/headers/headers_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .abc_headers_provider import ABCHeadersProvider
 from ..secret import secret_functions
+from ..secret import local_secrets_initialized
+from ..control import RPC
 from time import time
 
 
 class HeadersProvider(ABCHeadersProvider):
     def __init__(self):
         self.sid = ""
 
@@ -38,18 +40,20 @@
     def get_sid(self) -> str: return self.sid
 
     def set_sid(self, sid: str) -> None: self.sid = sid
 
     def remove_sid(self) -> None: self.sid = ""
 
     async def generate_request_signature(self, path: str, headers: dict, body: bytes) -> str:
-        return secret_functions.s(path, headers, body)
+        return secret_functions.s(path, headers, body) if local_secrets_initialized \
+            else RPC.generate_request_signature(path, headers, body)
 
     async def generate_device_id(self, installation_id: str):
-        return secret_functions.di(installation_id)
+        return secret_functions.di(installation_id) if local_secrets_initialized \
+            else await RPC.generate_device_id(installation_id)
 
     async def generate_device_id_three(
         self,
         organization: str,
         platform: str,
         version: str,
         model: str,
```

### Comparing `ProjZ.py-2.3.9/projz/api/request_manager.py` & `ProjZ.py-2.4.0/projz/api/request_manager.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/api/secret/data.txt` & `ProjZ.py-2.4.0/projz/api/secret/data.txt`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/client.py` & `ProjZ.py-2.4.0/projz/client.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/enum/__init__.py` & `ProjZ.py-2.4.0/projz/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/error/classes.py` & `ProjZ.py-2.4.0/projz/error/classes.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/__init__.py` & `ProjZ.py-2.4.0/projz/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/account.py` & `ProjZ.py-2.4.0/projz/model/account.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/blocked_item_wrapper.py` & `ProjZ.py-2.4.0/projz/model/blocked_item_wrapper.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/blog.py` & `ProjZ.py-2.4.0/projz/model/blog.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/category.py` & `ProjZ.py-2.4.0/projz/model/category.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/chat.py` & `ProjZ.py-2.4.0/projz/model/chat.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/chat_message.py` & `ProjZ.py-2.4.0/projz/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/circle.py` & `ProjZ.py-2.4.0/projz/model/circle.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/comment.py` & `ProjZ.py-2.4.0/projz/model/comment.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/currency.py` & `ProjZ.py-2.4.0/projz/model/currency.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/default_background_media.py` & `ProjZ.py-2.4.0/projz/model/default_background_media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/gift_box.py` & `ProjZ.py-2.4.0/projz/model/gift_box.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/media.py` & `ProjZ.py-2.4.0/projz/model/media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/member_title.py` & `ProjZ.py-2.4.0/projz/model/member_title.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/parse/parseutils.py` & `ProjZ.py-2.4.0/projz/model/parse/parseutils.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/poll.py` & `ProjZ.py-2.4.0/projz/model/poll.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/qi_vote_full_info.py` & `ProjZ.py-2.4.0/projz/model/qi_vote_full_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/qi_vote_info.py` & `ProjZ.py-2.4.0/projz/model/qi_vote_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/reaction.py` & `ProjZ.py-2.4.0/projz/model/reaction.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/response/member_titles_info.py` & `ProjZ.py-2.4.0/projz/model/response/member_titles_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/response/multi_invitation_code_info.py` & `ProjZ.py-2.4.0/projz/model/response/multi_invitation_code_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/rich_format.py` & `ProjZ.py-2.4.0/projz/model/rich_format.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/transfer_order.py` & `ProjZ.py-2.4.0/projz/model/transfer_order.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/user.py` & `ProjZ.py-2.4.0/projz/model/user.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/user_task.py` & `ProjZ.py-2.4.0/projz/model/user_task.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/util/rich_format_builder.py` & `ProjZ.py-2.4.0/projz/model/util/rich_format_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/util/rich_format_text_builder.py` & `ProjZ.py-2.4.0/projz/model/util/rich_format_text_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/model/wallet.py` & `ProjZ.py-2.4.0/projz/model/wallet.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/util/subscription_handler.py` & `ProjZ.py-2.4.0/projz/util/subscription_handler.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/projz/websocket/websocket_listener.py` & `ProjZ.py-2.4.0/projz/websocket/websocket_listener.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.9/setup.py` & `ProjZ.py-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             else:
                 print("Failed to install Sox. The stability of the library is not guaranteed.")
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.3.9",
+        version="2.4.0",
         author="D4krwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
```

