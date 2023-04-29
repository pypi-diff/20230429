# Comparing `tmp/ProjZ.py-1.8.3.tar.gz` & `tmp/ProjZ.py-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProjZ.py-1.8.3.tar", last modified: Mon Jan 31 13:37:01 2022, max compression
+gzip compressed data, was "ProjZ.py-2.3.1.tar", last modified: Sat Apr 29 12:18:35 2023, max compression
```

## Comparing `ProjZ.py-1.8.3.tar` & `ProjZ.py-2.3.1.tar`

### file list

```diff
@@ -1,74 +1,11 @@
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.716260 ProjZ.py-1.8.3/
--rw-rw-rw-   0        0        0      194 2022-01-31 13:37:01.716260 ProjZ.py-1.8.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.623555 ProjZ.py-1.8.3/ProjZ.py.egg-info/
--rw-rw-rw-   0        0        0      194 2022-01-31 13:37:01.000000 ProjZ.py-1.8.3/ProjZ.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2472 2022-01-31 13:37:01.000000 ProjZ.py-1.8.3/ProjZ.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-31 13:37:01.000000 ProjZ.py-1.8.3/ProjZ.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-31 13:37:01.000000 ProjZ.py-1.8.3/ProjZ.py.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       53 2022-01-31 13:37:01.000000 ProjZ.py-1.8.3/ProjZ.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-01-31 13:37:01.000000 ProjZ.py-1.8.3/ProjZ.py.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.626735 ProjZ.py-1.8.3/projz/
--rw-rw-rw-   0        0        0      510 2022-01-31 13:36:32.000000 ProjZ.py-1.8.3/projz/__init__.py
--rw-rw-rw-   0        0        0    15300 2022-01-31 13:36:39.000000 ProjZ.py-1.8.3/projz/client.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.628729 ProjZ.py-1.8.3/projz/internal/
--rw-rw-rw-   0        0        0        0 2022-01-13 13:05:39.000000 ProjZ.py-1.8.3/projz/internal/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.638270 ProjZ.py-1.8.3/projz/internal/api/
--rw-rw-rw-   0        0        0        0 2022-01-13 13:05:47.000000 ProjZ.py-1.8.3/projz/internal/api/__init__.py
--rw-rw-rw-   0        0        0     2052 2022-01-22 13:52:43.000000 ProjZ.py-1.8.3/projz/internal/api/z_api_request.py
--rw-rw-rw-   0        0        0      688 2022-01-22 13:47:46.000000 ProjZ.py-1.8.3/projz/internal/api/z_api_response.py
--rw-rw-rw-   0        0        0     2763 2022-01-23 07:46:35.000000 ProjZ.py-1.8.3/projz/internal/api/z_headers_composer.py
--rw-rw-rw-   0        0        0     1437 2022-01-26 07:52:45.000000 ProjZ.py-1.8.3/projz/internal/api/z_http_api.py
--rw-rw-rw-   0        0        0     1403 2022-01-22 13:58:05.000000 ProjZ.py-1.8.3/projz/internal/api/z_media_api.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.642295 ProjZ.py-1.8.3/projz/internal/exceptions/
--rw-rw-rw-   0        0        0        0 2022-01-18 18:04:27.000000 ProjZ.py-1.8.3/projz/internal/exceptions/__init__.py
--rw-rw-rw-   0        0        0      183 2022-01-18 19:15:16.000000 ProjZ.py-1.8.3/projz/internal/exceptions/api_exception.py
--rw-rw-rw-   0        0        0     1327 2022-01-26 09:01:27.000000 ProjZ.py-1.8.3/projz/internal/exceptions/finder.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.659243 ProjZ.py-1.8.3/projz/internal/exceptions/objects/
--rw-rw-rw-   0        0        0        0 2022-01-18 18:48:52.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/__init__.py
--rw-rw-rw-   0        0        0      234 2022-01-18 19:27:20.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/bad_device_id.py
--rw-rw-rw-   0        0        0      279 2022-01-26 08:53:48.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/captcha_caught.py
--rw-rw-rw-   0        0        0      241 2022-01-18 19:16:56.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/email_not_registered.py
--rw-rw-rw-   0        0        0      241 2022-01-21 20:07:53.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/file_uploading_error.py
--rw-rw-rw-   0        0        0      227 2022-01-18 19:15:16.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/incorrect_password.py
--rw-rw-rw-   0        0        0      248 2022-01-22 08:20:30.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/incorrect_verification_code.py
--rw-rw-rw-   0        0        0      235 2022-01-18 19:15:15.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/invalid_email.py
--rw-rw-rw-   0        0        0      241 2022-01-18 19:28:28.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/unsupported_service.py
--rw-rw-rw-   0        0        0      241 2022-01-22 08:21:45.000000 ProjZ.py-1.8.3/projz/internal/exceptions/objects/you_cant_register_now.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.670348 ProjZ.py-1.8.3/projz/internal/exceptions/other/
--rw-rw-rw-   0        0        0        0 2022-01-19 14:07:34.000000 ProjZ.py-1.8.3/projz/internal/exceptions/other/__init__.py
--rw-rw-rw-   0        0        0      131 2022-01-20 14:08:37.000000 ProjZ.py-1.8.3/projz/internal/exceptions/other/circle_client_initializing_error.py
--rw-rw-rw-   0        0        0      242 2022-01-24 15:55:14.000000 ProjZ.py-1.8.3/projz/internal/exceptions/other/message_sending_error.py
--rw-rw-rw-   0        0        0      126 2022-01-19 14:12:47.000000 ProjZ.py-1.8.3/projz/internal/exceptions/other/request_initializing_error.py
--rw-rw-rw-   0        0        0      124 2022-01-19 15:12:54.000000 ProjZ.py-1.8.3/projz/internal/exceptions/other/response_received_error.py
--rw-rw-rw-   0        0        0      114 2022-01-19 19:48:09.000000 ProjZ.py-1.8.3/projz/internal/exceptions/other/unauthorized.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.700835 ProjZ.py-1.8.3/projz/internal/models/
--rw-rw-rw-   0        0        0        0 2022-01-13 13:41:25.000000 ProjZ.py-1.8.3/projz/internal/models/__init__.py
--rw-rw-rw-   0        0        0      485 2022-01-21 08:53:17.000000 ProjZ.py-1.8.3/projz/internal/models/account.py
--rw-rw-rw-   0        0        0      785 2022-01-22 16:56:54.000000 ProjZ.py-1.8.3/projz/internal/models/chat.py
--rw-rw-rw-   0        0        0      284 2022-01-23 19:39:08.000000 ProjZ.py-1.8.3/projz/internal/models/chat_list.py
--rw-rw-rw-   0        0        0      517 2022-01-21 08:37:34.000000 ProjZ.py-1.8.3/projz/internal/models/circle.py
--rw-rw-rw-   0        0        0      288 2022-01-21 08:37:34.000000 ProjZ.py-1.8.3/projz/internal/models/circle_list.py
--rw-rw-rw-   0        0        0      146 2022-01-21 09:18:07.000000 ProjZ.py-1.8.3/projz/internal/models/link_info.py
--rw-rw-rw-   0        0        0      190 2022-01-22 08:52:39.000000 ProjZ.py-1.8.3/projz/internal/models/media.py
--rw-rw-rw-   0        0        0      263 2022-01-22 16:55:13.000000 ProjZ.py-1.8.3/projz/internal/models/message.py
--rw-rw-rw-   0        0        0      290 2022-01-24 13:55:14.000000 ProjZ.py-1.8.3/projz/internal/models/message_list.py
--rw-rw-rw-   0        0        0      233 2022-01-24 14:04:39.000000 ProjZ.py-1.8.3/projz/internal/models/old_chat_list.py
--rw-rw-rw-   0        0        0      112 2022-01-21 09:25:35.000000 ProjZ.py-1.8.3/projz/internal/models/pagination.py
--rw-rw-rw-   0        0        0      105 2022-01-21 09:25:35.000000 ProjZ.py-1.8.3/projz/internal/models/push_message.py
--rw-rw-rw-   0        0        0      139 2022-01-21 09:18:07.000000 ProjZ.py-1.8.3/projz/internal/models/resource.py
--rw-rw-rw-   0        0        0      104 2022-01-21 08:43:48.000000 ProjZ.py-1.8.3/projz/internal/models/user_mood.py
--rw-rw-rw-   0        0        0      999 2022-01-22 17:11:48.000000 ProjZ.py-1.8.3/projz/internal/models/user_profile.py
--rw-rw-rw-   0        0        0      375 2022-01-22 15:28:57.000000 ProjZ.py-1.8.3/projz/internal/models/user_profile_extensions.py
--rw-rw-rw-   0        0        0      299 2022-01-22 15:47:30.000000 ProjZ.py-1.8.3/projz/internal/models/user_profile_list.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.705037 ProjZ.py-1.8.3/projz/internal/utils/
--rw-rw-rw-   0        0        0        0 2022-01-18 18:24:32.000000 ProjZ.py-1.8.3/projz/internal/utils/__init__.py
--rw-rw-rw-   0        0        0     8257 2022-01-24 14:05:13.000000 ProjZ.py-1.8.3/projz/internal/utils/objectification.py
--rw-rw-rw-   0        0        0      254 2022-01-22 09:13:12.000000 ProjZ.py-1.8.3/projz/internal/utils/other.py
-drwxrwxrwx   0        0        0        0 2022-01-31 13:37:01.714016 ProjZ.py-1.8.3/projz/internal/websockets/
--rw-rw-rw-   0        0        0        0 2022-01-20 14:08:06.000000 ProjZ.py-1.8.3/projz/internal/websockets/__init__.py
--rw-rw-rw-   0        0        0     2942 2022-01-25 09:26:42.000000 ProjZ.py-1.8.3/projz/internal/websockets/base_websockets_listener.py
--rw-rw-rw-   0        0        0      307 2022-01-20 16:31:18.000000 ProjZ.py-1.8.3/projz/internal/websockets/callback_type.py
--rw-rw-rw-   0        0        0      515 2022-01-23 18:17:18.000000 ProjZ.py-1.8.3/projz/internal/websockets/custom_executor.py
--rw-rw-rw-   0        0        0     2970 2022-01-25 08:44:16.000000 ProjZ.py-1.8.3/projz/internal/websockets/z_websocket_listener.py
--rw-rw-rw-   0        0        0       42 2022-01-31 13:37:01.720284 ProjZ.py-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0      414 2022-01-31 13:36:25.000000 ProjZ.py-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 12:18:35.312546 ProjZ.py-2.3.1/
+-rw-rw-rw-   0        0        0     3981 2023-04-29 12:18:35.313509 ProjZ.py-2.3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-29 12:18:35.311530 ProjZ.py-2.3.1/ProjZ.py.egg-info/
+-rw-rw-rw-   0        0        0     3981 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 12:18:35.000000 ProjZ.py-2.3.1/ProjZ.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3574 2023-04-29 10:08:26.000000 ProjZ.py-2.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 12:18:35.315160 ProjZ.py-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2021 2023-04-29 12:18:31.000000 ProjZ.py-2.3.1/setup.py
```

