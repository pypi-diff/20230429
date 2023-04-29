# Comparing `tmp/ProjZ.py-2.3.5.tar.gz` & `tmp/ProjZ.py-2.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.3.5.tar", last modified: Sat Apr 29 12:43:30 2023, max compression
+gzip compressed data, was "ProjZ.py-2.3.6.tar", last modified: Sat Apr 29 13:02:11 2023, max compression
```

## Comparing `ProjZ.py-2.3.5.tar` & `ProjZ.py-2.3.6.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.047732 ProjZ.py-2.3.5/
--rw-rw-rw-   0        0        0     3983 2023-04-29 12:43:30.047732 ProjZ.py-2.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.919162 ProjZ.py-2.3.5/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     3983 2023-04-29 12:43:29.000000 ProjZ.py-2.3.5/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2258 2023-04-29 12:43:29.000000 ProjZ.py-2.3.5/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:43:29.000000 ProjZ.py-2.3.5/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-04-29 12:43:29.000000 ProjZ.py-2.3.5/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-29 12:43:29.000000 ProjZ.py-2.3.5/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.926108 ProjZ.py-2.3.5/projz/
--rw-rw-rw-   0        0        0       63 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/__init__.py
--rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.931041 ProjZ.py-2.3.5/projz/api/
--rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.934037 ProjZ.py-2.3.5/projz/api/control/
--rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/control/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/control/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.938025 ProjZ.py-2.3.5/projz/api/headers/
--rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/headers/__init__.py
--rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.3.5/projz/api/headers/abc_headers_provider.py
--rw-rw-rw-   0        0        0     2057 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/headers/headers_provider.py
--rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/request_manager.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.941018 ProjZ.py-2.3.5/projz/api/secret/
--rw-rw-rw-   0        0        0      290 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/secret/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.944009 ProjZ.py-2.3.5/projz/api/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/util/__init__.py
--rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/api/util/copy_to_buffer_writer.py
--rw-rw-rw-   0        0        0    57254 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/client.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.974931 ProjZ.py-2.3.5/projz/enum/
--rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/__init__.py
--rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/auth_purpose.py
--rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/auth_type.py
--rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/chat_message_type.py
--rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/chat_query_type.py
--rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/chat_thread_type.py
--rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/circle_filter_type.py
--rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/circle_members_query_type.py
--rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/comment_type.py
--rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/content_region.py
--rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/currency_type.py
--rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/gender.py
--rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/object_type.py
--rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/party_query_type.py
--rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/upload_target.py
--rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/user_task_type.py
--rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/enum/ws_event_type.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:29.977927 ProjZ.py-2.3.5/projz/error/
--rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/error/__init__.py
--rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/error/classes.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.024801 ProjZ.py-2.3.5/projz/model/
--rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/__init__.py
--rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/account.py
--rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/blocked_item_wrapper.py
--rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/blog.py
--rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/category.py
--rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/chat.py
--rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/chat_message.py
--rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/circle.py
--rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/comment.py
--rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/currency.py
--rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/default_background_media.py
--rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/dice.py
--rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/gift_box.py
--rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/link_info.py
--rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/media.py
--rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/member_title.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.027784 ProjZ.py-2.3.5/projz/model/parse/
--rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/parse/__init__.py
--rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/parse/parseutils.py
--rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/party.py
--rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/poll.py
--rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/qi_vote_full_info.py
--rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/qi_vote_info.py
--rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/reaction.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.034768 ProjZ.py-2.3.5/projz/model/response/
--rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/response/__init__.py
--rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/response/auth_result.py
--rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/response/member_titles_info.py
--rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/response/multi_invitation_code_info.py
--rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/rich_format.py
--rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/sticker.py
--rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/transfer_order.py
--rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/user.py
--rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/user_task.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.040751 ProjZ.py-2.3.5/projz/model/util/
--rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/util/__init__.py
--rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/util/paginated_list.py
--rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/util/rich_format_builder.py
--rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/util/rich_format_text_builder.py
--rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/model/wallet.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.043742 ProjZ.py-2.3.5/projz/util/
--rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/util/__init__.py
--rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/util/subscription_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-29 12:43:30.045738 ProjZ.py-2.3.5/projz/websocket/
--rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/websocket/__init__.py
--rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.3.5/projz/websocket/websocket_listener.py
--rw-rw-rw-   0        0        0       42 2023-04-29 12:43:30.049726 ProjZ.py-2.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1854 2023-04-29 12:43:26.000000 ProjZ.py-2.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.846856 ProjZ.py-2.3.6/
+-rw-rw-rw-   0        0        0       35 2023-04-29 12:58:20.000000 ProjZ.py-2.3.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3983 2023-04-29 13:02:11.847854 ProjZ.py-2.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.706714 ProjZ.py-2.3.6/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 13:02:11.000000 ProjZ.py-2.3.6/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2298 2023-04-29 13:02:11.000000 ProjZ.py-2.3.6/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:02:11.000000 ProjZ.py-2.3.6/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-04-29 13:02:11.000000 ProjZ.py-2.3.6/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 13:02:11.000000 ProjZ.py-2.3.6/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.712055 ProjZ.py-2.3.6/projz/
+-rw-rw-rw-   0        0        0       63 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/__init__.py
+-rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.717043 ProjZ.py-2.3.6/projz/api/
+-rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.720049 ProjZ.py-2.3.6/projz/api/control/
+-rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/control/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/control/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.725020 ProjZ.py-2.3.6/projz/api/headers/
+-rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/headers/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.3.6/projz/api/headers/abc_headers_provider.py
+-rw-rw-rw-   0        0        0     2057 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/headers/headers_provider.py
+-rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/request_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.728031 ProjZ.py-2.3.6/projz/api/secret/
+-rw-rw-rw-   0        0        0      290 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/secret/__init__.py
+-rw-rw-rw-   0        0        0     8965 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/secret/secret.pyc
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.732999 ProjZ.py-2.3.6/projz/api/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/util/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/api/util/copy_to_buffer_writer.py
+-rw-rw-rw-   0        0        0    57254 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/client.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.763916 ProjZ.py-2.3.6/projz/enum/
+-rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/auth_purpose.py
+-rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/auth_type.py
+-rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/chat_message_type.py
+-rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/chat_query_type.py
+-rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/chat_thread_type.py
+-rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/circle_filter_type.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/circle_members_query_type.py
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/comment_type.py
+-rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/content_region.py
+-rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/currency_type.py
+-rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/gender.py
+-rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/object_type.py
+-rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/party_query_type.py
+-rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/upload_target.py
+-rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/user_task_type.py
+-rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/enum/ws_event_type.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.769928 ProjZ.py-2.3.6/projz/error/
+-rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/error/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/error/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.823184 ProjZ.py-2.3.6/projz/model/
+-rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/account.py
+-rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/blocked_item_wrapper.py
+-rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/blog.py
+-rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/category.py
+-rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/chat.py
+-rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/chat_message.py
+-rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/circle.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/comment.py
+-rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/currency.py
+-rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/default_background_media.py
+-rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/dice.py
+-rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/gift_box.py
+-rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/link_info.py
+-rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/media.py
+-rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/member_title.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.827173 ProjZ.py-2.3.6/projz/model/parse/
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/parse/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/parse/parseutils.py
+-rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/party.py
+-rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/poll.py
+-rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/qi_vote_full_info.py
+-rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/qi_vote_info.py
+-rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.834154 ProjZ.py-2.3.6/projz/model/response/
+-rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/response/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/response/auth_result.py
+-rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/response/member_titles_info.py
+-rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/response/multi_invitation_code_info.py
+-rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/rich_format.py
+-rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/sticker.py
+-rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/transfer_order.py
+-rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/user.py
+-rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/user_task.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.840869 ProjZ.py-2.3.6/projz/model/util/
+-rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/util/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/util/paginated_list.py
+-rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/util/rich_format_builder.py
+-rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/util/rich_format_text_builder.py
+-rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/model/wallet.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.843864 ProjZ.py-2.3.6/projz/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/util/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/util/subscription_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:02:11.845859 ProjZ.py-2.3.6/projz/websocket/
+-rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/websocket/__init__.py
+-rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.3.6/projz/websocket/websocket_listener.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 13:02:11.848862 ProjZ.py-2.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2023-04-29 13:01:55.000000 ProjZ.py-2.3.6/setup.py
```

### Comparing `ProjZ.py-2.3.5/PKG-INFO` & `ProjZ.py-2.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.5
+Version: 2.3.6
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.3.5/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.3.6/ProjZ.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.5
+Version: 2.3.6
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.3.5/ProjZ.py.egg-info/SOURCES.txt` & `ProjZ.py-2.3.6/ProjZ.py.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ProjZ.py.egg-info/PKG-INFO
 ProjZ.py.egg-info/SOURCES.txt
 ProjZ.py.egg-info/dependency_links.txt
 ProjZ.py.egg-info/requires.txt
@@ -13,14 +14,15 @@
 projz/api/request_manager.py
 projz/api/control/__init__.py
 projz/api/control/rpc.py
 projz/api/headers/__init__.py
 projz/api/headers/abc_headers_provider.py
 projz/api/headers/headers_provider.py
 projz/api/secret/__init__.py
+projz/api/secret/secret.pyc
 projz/api/util/__init__.py
 projz/api/util/copy_to_buffer_writer.py
 projz/enum/__init__.py
 projz/enum/auth_purpose.py
 projz/enum/auth_type.py
 projz/enum/chat_message_type.py
 projz/enum/chat_query_type.py
```

### Comparing `ProjZ.py-2.3.5/README.md` & `ProjZ.py-2.3.6/README.md`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/__main__.py` & `ProjZ.py-2.3.6/projz/__main__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/api/control/rpc.py` & `ProjZ.py-2.3.6/projz/api/control/rpc.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/api/headers/abc_headers_provider.py` & `ProjZ.py-2.3.6/projz/api/headers/abc_headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/api/headers/headers_provider.py` & `ProjZ.py-2.3.6/projz/api/headers/headers_provider.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/api/request_manager.py` & `ProjZ.py-2.3.6/projz/api/request_manager.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/client.py` & `ProjZ.py-2.3.6/projz/client.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/enum/__init__.py` & `ProjZ.py-2.3.6/projz/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/error/classes.py` & `ProjZ.py-2.3.6/projz/error/classes.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/__init__.py` & `ProjZ.py-2.3.6/projz/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/account.py` & `ProjZ.py-2.3.6/projz/model/account.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/blocked_item_wrapper.py` & `ProjZ.py-2.3.6/projz/model/blocked_item_wrapper.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/blog.py` & `ProjZ.py-2.3.6/projz/model/blog.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/category.py` & `ProjZ.py-2.3.6/projz/model/category.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/chat.py` & `ProjZ.py-2.3.6/projz/model/chat.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/chat_message.py` & `ProjZ.py-2.3.6/projz/model/chat_message.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/circle.py` & `ProjZ.py-2.3.6/projz/model/circle.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/comment.py` & `ProjZ.py-2.3.6/projz/model/comment.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/currency.py` & `ProjZ.py-2.3.6/projz/model/currency.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/default_background_media.py` & `ProjZ.py-2.3.6/projz/model/default_background_media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/gift_box.py` & `ProjZ.py-2.3.6/projz/model/gift_box.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/media.py` & `ProjZ.py-2.3.6/projz/model/media.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/member_title.py` & `ProjZ.py-2.3.6/projz/model/member_title.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/parse/parseutils.py` & `ProjZ.py-2.3.6/projz/model/parse/parseutils.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/poll.py` & `ProjZ.py-2.3.6/projz/model/poll.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/qi_vote_full_info.py` & `ProjZ.py-2.3.6/projz/model/qi_vote_full_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/qi_vote_info.py` & `ProjZ.py-2.3.6/projz/model/qi_vote_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/reaction.py` & `ProjZ.py-2.3.6/projz/model/reaction.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/response/member_titles_info.py` & `ProjZ.py-2.3.6/projz/model/response/member_titles_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/response/multi_invitation_code_info.py` & `ProjZ.py-2.3.6/projz/model/response/multi_invitation_code_info.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/rich_format.py` & `ProjZ.py-2.3.6/projz/model/rich_format.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/transfer_order.py` & `ProjZ.py-2.3.6/projz/model/transfer_order.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/user.py` & `ProjZ.py-2.3.6/projz/model/user.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/user_task.py` & `ProjZ.py-2.3.6/projz/model/user_task.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/util/rich_format_builder.py` & `ProjZ.py-2.3.6/projz/model/util/rich_format_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/util/rich_format_text_builder.py` & `ProjZ.py-2.3.6/projz/model/util/rich_format_text_builder.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/model/wallet.py` & `ProjZ.py-2.3.6/projz/model/wallet.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/util/subscription_handler.py` & `ProjZ.py-2.3.6/projz/util/subscription_handler.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/projz/websocket/websocket_listener.py` & `ProjZ.py-2.3.6/projz/websocket/websocket_listener.py`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.5/setup.py` & `ProjZ.py-2.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             else:
                 print("Failed to install Sox. The stability of the library is not guaranteed.")
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.3.5",
+        version="2.3.6",
         author="D4krwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
```

