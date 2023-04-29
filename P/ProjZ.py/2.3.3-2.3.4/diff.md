# Comparing `tmp/ProjZ.py-2.3.3.tar.gz` & `tmp/ProjZ.py-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-2.3.3.tar", last modified: Sat Apr 29 12:28:15 2023, max compression
+gzip compressed data, was "ProjZ.py-2.3.4.tar", last modified: Sat Apr 29 12:38:50 2023, max compression
```

## Comparing `ProjZ.py-2.3.3.tar` & `ProjZ.py-2.3.4.tar`

### file list

```diff
@@ -1,11 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 12:28:15.645702 ProjZ.py-2.3.3/
--rw-rw-rw-   0        0        0     3983 2023-04-29 12:28:15.646664 ProjZ.py-2.3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-29 12:28:15.643690 ProjZ.py-2.3.3/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0     3983 2023-04-29 12:28:15.000000 ProjZ.py-2.3.3/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2023-04-29 12:28:15.000000 ProjZ.py-2.3.3/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:28:15.000000 ProjZ.py-2.3.3/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-04-29 12:28:15.000000 ProjZ.py-2.3.3/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 12:28:15.000000 ProjZ.py-2.3.3/ProjZ.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 12:28:15.647678 ProjZ.py-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2136 2023-04-29 12:28:04.000000 ProjZ.py-2.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.104967 ProjZ.py-2.3.4/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 12:38:50.104967 ProjZ.py-2.3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.975314 ProjZ.py-2.3.4/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     3983 2023-04-29 12:38:49.000000 ProjZ.py-2.3.4/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2258 2023-04-29 12:38:49.000000 ProjZ.py-2.3.4/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:38:49.000000 ProjZ.py-2.3.4/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-29 12:38:49.000000 ProjZ.py-2.3.4/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-29 12:38:49.000000 ProjZ.py-2.3.4/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.980300 ProjZ.py-2.3.4/projz/
+-rw-rw-rw-   0        0        0       63 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/__init__.py
+-rw-rw-rw-   0        0        0     7167 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.983291 ProjZ.py-2.3.4/projz/api/
+-rw-rw-rw-   0        0        0      120 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.988280 ProjZ.py-2.3.4/projz/api/control/
+-rw-rw-rw-   0        0        0       22 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/control/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/control/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.994268 ProjZ.py-2.3.4/projz/api/headers/
+-rw-rw-rw-   0        0        0      101 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/headers/__init__.py
+-rw-rw-rw-   0        0        0      969 2023-04-29 12:23:08.000000 ProjZ.py-2.3.4/projz/api/headers/abc_headers_provider.py
+-rw-rw-rw-   0        0        0     2057 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/headers/headers_provider.py
+-rw-rw-rw-   0        0        0     4789 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/request_manager.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.995260 ProjZ.py-2.3.4/projz/api/secret/
+-rw-rw-rw-   0        0        0      290 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/secret/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:49.999249 ProjZ.py-2.3.4/projz/api/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/util/__init__.py
+-rw-rw-rw-   0        0        0      289 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/api/util/copy_to_buffer_writer.py
+-rw-rw-rw-   0        0        0    57254 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/client.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.028171 ProjZ.py-2.3.4/projz/enum/
+-rw-rw-rw-   0        0        0      641 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/__init__.py
+-rw-rw-rw-   0        0        0      179 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/auth_purpose.py
+-rw-rw-rw-   0        0        0       87 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/auth_type.py
+-rw-rw-rw-   0        0        0      148 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/chat_message_type.py
+-rw-rw-rw-   0        0        0      181 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/chat_query_type.py
+-rw-rw-rw-   0        0        0      109 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/chat_thread_type.py
+-rw-rw-rw-   0        0        0      158 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/circle_filter_type.py
+-rw-rw-rw-   0        0        0      112 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/circle_members_query_type.py
+-rw-rw-rw-   0        0        0       82 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/comment_type.py
+-rw-rw-rw-   0        0        0      221 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/content_region.py
+-rw-rw-rw-   0        0        0      108 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/currency_type.py
+-rw-rw-rw-   0        0        0       95 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/gender.py
+-rw-rw-rw-   0        0        0      149 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/object_type.py
+-rw-rw-rw-   0        0        0       85 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/party_query_type.py
+-rw-rw-rw-   0        0        0      210 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/upload_target.py
+-rw-rw-rw-   0        0        0      212 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/user_task_type.py
+-rw-rw-rw-   0        0        0       98 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/enum/ws_event_type.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.031163 ProjZ.py-2.3.4/projz/error/
+-rw-rw-rw-   0        0        0       24 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/error/__init__.py
+-rw-rw-rw-   0        0        0     1620 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/error/classes.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.078038 ProjZ.py-2.3.4/projz/model/
+-rw-rw-rw-   0        0        0     1102 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/__init__.py
+-rw-rw-rw-   0        0        0      967 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/account.py
+-rw-rw-rw-   0        0        0      577 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/blocked_item_wrapper.py
+-rw-rw-rw-   0        0        0     1388 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/blog.py
+-rw-rw-rw-   0        0        0     1796 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/category.py
+-rw-rw-rw-   0        0        0     2260 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/chat.py
+-rw-rw-rw-   0        0        0      952 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/chat_message.py
+-rw-rw-rw-   0        0        0     2093 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/circle.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/comment.py
+-rw-rw-rw-   0        0        0      584 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/currency.py
+-rw-rw-rw-   0        0        0      663 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/default_background_media.py
+-rw-rw-rw-   0        0        0      433 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/dice.py
+-rw-rw-rw-   0        0        0     1194 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/gift_box.py
+-rw-rw-rw-   0        0        0      415 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/link_info.py
+-rw-rw-rw-   0        0        0      602 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/media.py
+-rw-rw-rw-   0        0        0      540 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/member_title.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.080033 ProjZ.py-2.3.4/projz/model/parse/
+-rw-rw-rw-   0        0        0       27 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/parse/__init__.py
+-rw-rw-rw-   0        0        0     1033 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/parse/parseutils.py
+-rw-rw-rw-   0        0        0      409 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/party.py
+-rw-rw-rw-   0        0        0      840 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/poll.py
+-rw-rw-rw-   0        0        0     1004 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/qi_vote_full_info.py
+-rw-rw-rw-   0        0        0      594 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/qi_vote_info.py
+-rw-rw-rw-   0        0        0      561 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/reaction.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.089009 ProjZ.py-2.3.4/projz/model/response/
+-rw-rw-rw-   0        0        0      152 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/response/__init__.py
+-rw-rw-rw-   0        0        0      447 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/response/auth_result.py
+-rw-rw-rw-   0        0        0      513 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/response/member_titles_info.py
+-rw-rw-rw-   0        0        0      738 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/response/multi_invitation_code_info.py
+-rw-rw-rw-   0        0        0     2872 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/rich_format.py
+-rw-rw-rw-   0        0        0      280 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/sticker.py
+-rw-rw-rw-   0        0        0     1134 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/transfer_order.py
+-rw-rw-rw-   0        0        0     3484 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/user.py
+-rw-rw-rw-   0        0        0      632 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/user_task.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.094992 ProjZ.py-2.3.4/projz/model/util/
+-rw-rw-rw-   0        0        0      156 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/util/__init__.py
+-rw-rw-rw-   0        0        0      339 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/util/paginated_list.py
+-rw-rw-rw-   0        0        0     4330 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/util/rich_format_builder.py
+-rw-rw-rw-   0        0        0     4790 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/util/rich_format_text_builder.py
+-rw-rw-rw-   0        0        0     1685 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/model/wallet.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.098982 ProjZ.py-2.3.4/projz/util/
+-rw-rw-rw-   0        0        0       55 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/util/__init__.py
+-rw-rw-rw-   0        0        0     1492 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/util/subscription_handler.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:38:50.103969 ProjZ.py-2.3.4/projz/websocket/
+-rw-rw-rw-   0        0        0       51 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/websocket/__init__.py
+-rw-rw-rw-   0        0        0     3753 2023-04-29 10:11:44.000000 ProjZ.py-2.3.4/projz/websocket/websocket_listener.py
+-rw-rw-rw-   0        0        0       42 2023-04-29 12:38:50.106961 ProjZ.py-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2136 2023-04-29 12:38:46.000000 ProjZ.py-2.3.4/setup.py
```

### Comparing `ProjZ.py-2.3.3/PKG-INFO` & `ProjZ.py-2.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.3
+Version: 2.3.4
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.3.3/ProjZ.py.egg-info/PKG-INFO` & `ProjZ.py-2.3.4/ProjZ.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProjZ.py
-Version: 2.3.3
+Version: 2.3.4
 Summary: An asynchronous library for creating scripts and chatbots in Project Z.
 Home-page: UNKNOWN
 Author: D4krwat3r
 Author-email: ktoya170214@gmail.com
 License: UNKNOWN
 Keywords: project-z,projectz,projz,bots,api,supersymlab,projz-bot,projz-bots,projz-api
 Platform: UNKNOWN
```

### Comparing `ProjZ.py-2.3.3/README.md` & `ProjZ.py-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ProjZ.py-2.3.3/setup.py` & `ProjZ.py-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                     print("Installation canceled.")
                     return
         else:
             print("Sox found, no installation required.")
 
     setup(
         name="ProjZ.py",
-        version="2.3.3",
+        version="2.3.4",
         author="D4krwat3r",
         description="An asynchronous library for creating scripts and chatbots in Project Z.",
         packages=find_packages(),
         author_email="ktoya170214@gmail.com",
         install_requires=get_requirements(),
         long_description=get_readme(),
         long_description_content_type="text/markdown",
```

