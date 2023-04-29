# Comparing `tmp/davtelepot-2.8.9.tar.gz` & `tmp/davtelepot-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davtelepot-2.8.9.tar", last modified: Sat Dec 10 17:46:40 2022, max compression
+gzip compressed data, was "davtelepot-2.9.1.tar", last modified: Sat Apr 29 18:57:16 2023, max compression
```

## Comparing `davtelepot-2.8.9.tar` & `davtelepot-2.9.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2022-12-10 17:46:40.621799 davtelepot-2.8.9/
--rw-r--r--   0 davte     (1000) davte     (1000)       68 2018-10-23 15:20:11.000000 davtelepot-2.8.9/LICENSE
--rw-rw-r--   0 davte     (1000) davte     (1000)      153 2019-07-19 08:07:29.000000 davtelepot-2.8.9/MANIFEST.in
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2022-12-10 17:46:40.621799 davtelepot-2.8.9/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)     2781 2019-07-18 12:44:21.000000 davtelepot-2.8.9/README.md
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2022-12-10 17:46:40.617799 davtelepot-2.8.9/davtelepot/
--rw-rw-r--   0 davte     (1000) davte     (1000)      747 2022-12-10 17:46:29.000000 davtelepot-2.8.9/davtelepot/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    70625 2022-10-12 11:53:43.000000 davtelepot-2.8.9/davtelepot/administration_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    95286 2022-12-08 15:19:45.000000 davtelepot-2.8.9/davtelepot/api.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     9821 2022-12-08 15:19:45.000000 davtelepot-2.8.9/davtelepot/api_helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2022-12-06 21:18:51.000000 davtelepot-2.8.9/davtelepot/authorization.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   141728 2022-12-08 15:19:45.000000 davtelepot-2.8.9/davtelepot/bot.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2022-12-10 17:46:40.617799 davtelepot-2.8.9/davtelepot/data/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-19 07:39:50.000000 davtelepot-2.8.9/davtelepot/data/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2022-12-10 17:46:29.000000 davtelepot-2.8.9/davtelepot/database.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-11-19 14:18:50.000000 davtelepot-2.8.9/davtelepot/helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    16258 2019-07-18 12:44:21.000000 davtelepot-2.8.9/davtelepot/ietf_language_tags.csv
--rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2022-10-12 11:53:43.000000 davtelepot-2.8.9/davtelepot/languages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    46400 2022-12-05 21:10:02.000000 davtelepot-2.8.9/davtelepot/messages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2022-10-12 11:53:43.000000 davtelepot-2.8.9/davtelepot/suggestions.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2022-12-10 17:46:40.617799 davtelepot-2.8.9/davtelepot/tools/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-06-22 20:56:16.000000 davtelepot-2.8.9/davtelepot/tools/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-06-22 20:56:16.000000 davtelepot-2.8.9/davtelepot/tools/merge_files.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2022-10-12 11:53:43.000000 davtelepot-2.8.9/davtelepot/useful_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    49259 2022-10-12 12:04:39.000000 davtelepot-2.8.9/davtelepot/utilities.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2022-12-10 17:46:40.617799 davtelepot-2.8.9/davtelepot.egg-info/
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2022-12-10 17:46:40.000000 davtelepot-2.8.9/davtelepot.egg-info/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)      754 2022-12-10 17:46:40.000000 davtelepot-2.8.9/davtelepot.egg-info/SOURCES.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)        1 2022-12-10 17:46:40.000000 davtelepot-2.8.9/davtelepot.egg-info/dependency_links.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2022-12-10 17:46:40.000000 davtelepot-2.8.9/davtelepot.egg-info/requires.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2022-12-10 17:46:40.000000 davtelepot-2.8.9/davtelepot.egg-info/top_level.txt
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2022-12-10 17:46:40.617799 davtelepot-2.8.9/examples/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-18 12:44:21.000000 davtelepot-2.8.9/examples/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-08-23 12:21:45.000000 davtelepot-2.8.9/examples/a_simple_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-08-23 12:21:45.000000 davtelepot-2.8.9/examples/more_bots_together.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3245 2020-08-23 12:11:09.000000 davtelepot-2.8.9/examples/webhook_powered_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)       38 2022-12-10 17:46:40.621799 davtelepot-2.8.9/setup.cfg
--rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-08-23 12:11:09.000000 davtelepot-2.8.9/setup.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.702412 davtelepot-2.9.1/
+-rw-r--r--   0 davte     (1000) davte     (1000)       68 2018-10-23 15:20:11.000000 davtelepot-2.9.1/LICENSE
+-rw-rw-r--   0 davte     (1000) davte     (1000)      153 2019-07-19 08:07:29.000000 davtelepot-2.9.1/MANIFEST.in
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-04-29 18:57:16.702412 davtelepot-2.9.1/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2781 2019-07-18 12:44:21.000000 davtelepot-2.9.1/README.md
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot/
+-rw-rw-r--   0 davte     (1000) davte     (1000)      747 2023-04-29 11:52:55.000000 davtelepot-2.9.1/davtelepot/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-04-29 15:53:32.000000 davtelepot-2.9.1/davtelepot/__main__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    70625 2022-12-12 21:45:08.000000 davtelepot-2.9.1/davtelepot/administration_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   111657 2023-04-29 15:25:02.000000 davtelepot-2.9.1/davtelepot/api.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-01-06 09:30:24.000000 davtelepot-2.9.1/davtelepot/api_helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2022-12-06 21:18:51.000000 davtelepot-2.9.1/davtelepot/authorization.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   143116 2023-04-29 18:02:59.000000 davtelepot-2.9.1/davtelepot/bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     8455 2023-04-29 18:55:02.000000 davtelepot-2.9.1/davtelepot/cli.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot/data/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-19 07:39:50.000000 davtelepot-2.9.1/davtelepot/data/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2022-12-10 17:46:29.000000 davtelepot-2.9.1/davtelepot/database.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-11-19 14:18:50.000000 davtelepot-2.9.1/davtelepot/helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    16258 2019-07-18 12:44:21.000000 davtelepot-2.9.1/davtelepot/ietf_language_tags.csv
+-rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2022-10-12 11:53:43.000000 davtelepot-2.9.1/davtelepot/languages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    46400 2022-12-05 21:10:02.000000 davtelepot-2.9.1/davtelepot/messages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2022-10-12 11:53:43.000000 davtelepot-2.9.1/davtelepot/suggestions.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot/tools/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-06-22 20:56:16.000000 davtelepot-2.9.1/davtelepot/tools/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-06-22 20:56:16.000000 davtelepot-2.9.1/davtelepot/tools/merge_files.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2022-10-12 11:53:43.000000 davtelepot-2.9.1/davtelepot/useful_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    50174 2023-01-06 09:30:02.000000 davtelepot-2.9.1/davtelepot/utilities.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot.egg-info/
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)      795 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/SOURCES.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)        1 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/dependency_links.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/requires.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/top_level.txt
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.702412 davtelepot-2.9.1/examples/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-18 12:44:21.000000 davtelepot-2.9.1/examples/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-08-23 12:21:45.000000 davtelepot-2.9.1/examples/a_simple_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-08-23 12:21:45.000000 davtelepot-2.9.1/examples/more_bots_together.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3245 2020-08-23 12:11:09.000000 davtelepot-2.9.1/examples/webhook_powered_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)       38 2023-04-29 18:57:16.702412 davtelepot-2.9.1/setup.cfg
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-08-23 12:11:09.000000 davtelepot-2.9.1/setup.py
```

### Comparing `davtelepot-2.8.9/PKG-INFO` & `davtelepot-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.8.9
+Version: 2.9.1
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.8.9/README.md` & `davtelepot-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/__init__.py` & `davtelepot-2.9.1/davtelepot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ```
 """
 
 __author__ = "Davide Testa"
 __email__ = "davide@davte.it"
 __credits__ = ["Marco Origlia", "Nick Lee @Nickoala"]
 __license__ = "GNU General Public License v3.0"
-__version__ = "2.8.9"
+__version__ = "2.9.1"
 __maintainer__ = "Davide Testa"
 __contact__ = "t.me/davte"
 
 from davtelepot import (administration_tools, api, authorization,
                         bot, helper, languages, messages, suggestions,
                         useful_tools, utilities)
```

### Comparing `davtelepot-2.8.9/davtelepot/administration_tools.py` & `davtelepot-2.9.1/davtelepot/administration_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from sqlalchemy.exc import ResourceClosedError
 
 # Project modules
 from davtelepot.messages import default_admin_messages, default_talk_messages
 from davtelepot.bot import Bot
 from davtelepot.utilities import (
     async_wrapper, CachedPage, Confirmator, extract, get_cleaned_text,
-    get_user, escape_html_chars, line_drawing_unordered_list, make_button,
+    get_user, clean_html_string, line_drawing_unordered_list, make_button,
     make_inline_keyboard, remove_html_tags, send_part_of_text_file,
     send_csv_file, make_lines_of_buttons
 )
 
 # Use this parameter in SQL `LIMIT x OFFSET y` clauses
 rows_number_limit = 10
 
@@ -126,15 +126,15 @@
     if len(text) == 0:
         text = (
             bot.get_message(
                 'talk',
                 'help_text',
                 update=update,
                 user_record=user_record,
-                q=escape_html_chars(
+                q=clean_html_string(
                     remove_html_tags(text)
                 )
             )
         )
         reply_markup = make_inline_keyboard(
             [
                 make_button(
@@ -151,15 +151,15 @@
     elif len(users) == 0:
         text = (
             bot.get_message(
                 'talk',
                 'user_not_found',
                 update=update,
                 user_record=user_record,
-                q=escape_html_chars(
+                q=clean_html_string(
                     remove_html_tags(text)
                 )
             )
         )
         reply_markup = make_inline_keyboard(
             [
                 make_button(
```

### Comparing `davtelepot-2.8.9/davtelepot/api.py` & `davtelepot-2.9.1/davtelepot/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # Standard library modules
 import asyncio
 import datetime
 import io
 import json
 import logging
+import os.path
 
 from typing import Dict, Union, List, IO
 
 # Third party modules
 import aiohttp
 import aiohttp.web
 
@@ -266,14 +267,87 @@
             raise TypeError(f"Unknown InlineQueryResult type: `{type}`.")
         super().__init__(self)
         self['type'] = type
         for key, value in kwargs.items():
             self[key] = value
 
 
+class MaskPosition(dict):
+    """This object describes the position on faces where a mask should be placed by default."""
+
+    def __init__(self, point: str, x_shift: float, y_shift: float, scale: float):
+        """This object describes the position on faces where a mask should be placed by default.
+
+        @param point: The part of the face relative to which the mask should
+            be placed. One of “forehead”, “eyes”, “mouth”, or “chin”.
+        @param x_shift: Shift by X-axis measured in widths of the mask scaled
+            to the face size, from left to right. For example, choosing -1.0
+            will place mask just to the left of the default mask position.
+        @param y_shift: Shift by Y-axis measured in heights of the mask scaled
+            to the face size, from top to bottom. For example, 1.0 will place
+            the mask just below the default mask position.
+        @param scale: Mask scaling coefficient.
+            For example, 2.0 means double size.
+        """
+        super().__init__(self)
+        self['point'] = point
+        self['x_shift'] = x_shift
+        self['y_shift'] = y_shift
+        self['scale'] = scale
+
+
+class InputSticker(dict):
+    """This object describes a sticker to be added to a sticker set."""
+
+    def __init__(self, sticker: Union[str, dict, IO], emoji_list: List[str],
+                 mask_position: Union['MaskPosition', None] = None,
+                 keywords: Union[List[str], None] = None):
+        """This object describes a sticker to be added to a sticker set.
+
+        @param sticker: The added sticker. Pass a file_id as a String to send
+            a file that already exists on the Telegram servers,
+            pass an HTTP URL as a String for Telegram to get a file from the
+            Internet, upload a new one using multipart/form-data,
+            or pass “attach://<file_attach_name>” to upload a new one using
+            multipart/form-data under <file_attach_name> name.
+            Animated and video stickers can't be uploaded via HTTP URL.
+            More information on Sending Files: https://core.telegram.org/bots/api#sending-files
+        @param emoji_list: List of 1-20 emoji associated with the sticker
+        @param mask_position: Optional. Position where the mask should be
+            placed on faces. For “mask” stickers only.
+        @param keywords: Optional. List of 0-20 search keywords for the sticker
+            with total length of up to 64 characters.
+            For “regular” and “custom_emoji” stickers only.
+        """
+        super().__init__(self)
+        self['sticker'] = sticker
+        self['emoji_list'] = emoji_list
+        self['mask_position'] = mask_position
+        self['keywords'] = keywords
+
+
+class InlineQueryResultsButton(dict):
+    """Button to be shown above inline query results."""
+
+    def __init__(self,
+                 text: str = None,
+                 web_app: 'WebAppInfo' = None,
+                 start_parameter: str = None):
+        super().__init__(self)
+        if sum(1 for e in (text, web_app, start_parameter) if e) != 1:
+            logging.error("You must provide exactly one parameter (`text` "
+                          "or `web_app` or `start_parameter`).")
+            return
+        self['text'] = text
+        self['web_app'] = web_app
+        self['start_parameter'] = start_parameter
+        return
+
+
+
 # This class needs to mirror Telegram API, so camelCase method are needed
 # noinspection PyPep8Naming
 class TelegramBot:
     """Provide python method having the same signature as Telegram API methods.
 
     All mirrored methods are camelCase.
     """
@@ -378,36 +452,40 @@
         )
         if not response['ok']:
             raise TelegramError(**response)
         return response['result']
 
     @staticmethod
     def adapt_parameters(parameters, exclude=None):
-        """Build a aiohttp.FormData object from given `parameters`.
+        """Build an aiohttp.FormData object from given `parameters`.
 
         Exclude `self`, empty values and parameters in `exclude` list.
         Cast integers to string to avoid TypeError during json serialization.
         """
         if exclude is None:
             exclude = []
-        exclude.append('self')
+        exclude += ['self', 'kwargs']
         # quote_fields=False, otherwise some file names cause troubles
         data = aiohttp.FormData(quote_fields=False)
         for key, value in parameters.items():
             if not (key in exclude or value is None):
                 if (type(value) in (int, list,)
                         or (type(value) is dict and 'file' not in value)):
                     value = json.dumps(value, separators=(',', ':'))
                 data.add_field(key, value)
         return data
 
     @staticmethod
     def prepare_file_object(file: Union[str, IO, dict, None]
-                            ) -> Union[Dict[str, IO], None]:
-        if type(file) is str:
+                            ) -> Union[str, Dict[str, IO], None]:
+        """If `file` is a valid file path, return a dict for multipart/form-data.
+
+        Other valid file identifiers are URLs and Telegram `file_id`s.
+        """
+        if type(file) is str and os.path.isfile(file):
             try:
                 file = open(file, 'r')
             except FileNotFoundError as e:
                 logging.error(f"{e}")
                 file = None
         if isinstance(file, io.IOBase):
             file = dict(file=file)
@@ -439,14 +517,28 @@
             session_must_be_closed = True
         return session, session_must_be_closed
 
     def set_flood_wait(self, flood_wait):
         """Wait `flood_wait` seconds before next request."""
         self._flood_wait = flood_wait
 
+    def make_input_sticker(self,
+                           sticker: Union[dict, str, IO],
+                           emoji_list: Union[List[str], str],
+                           mask_position: Union[MaskPosition, None] = None,
+                           keywords: Union[List[str], None] = None) -> InputSticker:
+        if isinstance(emoji_list, str):
+            emoji_list = [c for c in emoji_list]
+        if isinstance(keywords, str):
+            keywords = [w for w in keywords]
+        if isinstance(sticker, str) and os.path.isfile(sticker):
+            sticker = self.prepare_file_object(sticker)
+        return InputSticker(sticker=sticker, emoji_list=emoji_list,
+                            mask_position=mask_position, keywords=keywords)
+
     async def prevent_flooding(self, chat_id):
         """Await until request may be sent safely.
 
         Telegram flood control won't allow too many API requests in a small
             period.
         Exact limits are unknown, but less than 30 total private chat messages
             per second, less than 1 private message per chat and less than 20
@@ -680,14 +772,15 @@
                         parse_mode: str = None,
                         caption_entities: List[dict] = None,
                         message_thread_id: int = None,
                         protect_content: bool = None,
                         disable_notification: bool = None,
                         reply_to_message_id: int = None,
                         allow_sending_without_reply: bool = None,
+                        has_spoiler: bool = None,
                         reply_markup=None):
         """Send a photo from file_id, HTTP url or file.
 
         See https://core.telegram.org/bots/api#sendphoto for details.
         """
         return await self.api_request(
             'sendPhoto',
@@ -697,93 +790,119 @@
     async def sendAudio(self, chat_id: Union[int, str], audio,
                         caption: str = None,
                         parse_mode: str = None,
                         caption_entities: List[dict] = None,
                         duration: int = None,
                         performer: str = None,
                         title: str = None,
-                        thumb=None,
+                        thumbnail=None,
                         disable_notification: bool = None,
                         reply_to_message_id: int = None,
                         allow_sending_without_reply: bool = None,
                         message_thread_id: int = None,
                         protect_content: bool = None,
-                        reply_markup=None):
+                        reply_markup=None,
+                        **kwargs):
         """Send an audio file from file_id, HTTP url or file.
 
         See https://core.telegram.org/bots/api#sendaudio for details.
         """
+        if 'thumb' in kwargs:
+            thumbnail = kwargs['thumb']
+            logging.error("DEPRECATION WARNING: `thumb` parameter of function"
+                          "`sendAudio` has been deprecated since Bot API 6.6. "
+                          "Use `thumbnail` instead.")
         return await self.api_request(
             'sendAudio',
             parameters=locals()
         )
 
     async def sendDocument(self, chat_id: Union[int, str], document,
-                           thumb=None,
+                           thumbnail=None,
                            caption: str = None,
                            parse_mode: str = None,
                            caption_entities: List[dict] = None,
                            disable_content_type_detection: bool = None,
                            disable_notification: bool = None,
                            reply_to_message_id: int = None,
                            allow_sending_without_reply: bool = None,
                            message_thread_id: int = None,
                            protect_content: bool = None,
-                           reply_markup=None):
+                           reply_markup=None,
+                           **kwargs):
         """Send a document from file_id, HTTP url or file.
 
         See https://core.telegram.org/bots/api#senddocument for details.
         """
+        if 'thumb' in kwargs:
+            thumbnail = kwargs['thumb']
+            logging.error("DEPRECATION WARNING: `thumb` parameter of function"
+                          "`sendDocument` has been deprecated since Bot API 6.6. "
+                          "Use `thumbnail` instead.")
         return await self.api_request(
             'sendDocument',
             parameters=locals()
         )
 
     async def sendVideo(self, chat_id: Union[int, str], video,
                         duration: int = None,
                         width: int = None,
                         height: int = None,
-                        thumb=None,
+                        thumbnail=None,
                         caption: str = None,
                         parse_mode: str = None,
                         caption_entities: List[dict] = None,
                         supports_streaming: bool = None,
                         disable_notification: bool = None,
                         reply_to_message_id: int = None,
                         allow_sending_without_reply: bool = None,
                         message_thread_id: int = None,
                         protect_content: bool = None,
-                        reply_markup=None):
+                        has_spoiler: bool = None,
+                        reply_markup=None,
+                        **kwargs):
         """Send a video from file_id, HTTP url or file.
 
         See https://core.telegram.org/bots/api#sendvideo for details.
         """
+        if 'thumb' in kwargs:
+            thumbnail = kwargs['thumb']
+            logging.error("DEPRECATION WARNING: `thumb` parameter of function"
+                          "`sendVideo` has been deprecated since Bot API 6.6. "
+                          "Use `thumbnail` instead.")
         return await self.api_request(
             'sendVideo',
             parameters=locals()
         )
 
     async def sendAnimation(self, chat_id: Union[int, str], animation,
                             duration: int = None,
                             width: int = None,
                             height: int = None,
-                            thumb=None,
+                            thumbnail=None,
                             caption: str = None,
                             parse_mode: str = None,
                             caption_entities: List[dict] = None,
                             disable_notification: bool = None,
                             reply_to_message_id: int = None,
                             allow_sending_without_reply: bool = None,
                             message_thread_id: int = None,
                             protect_content: bool = None,
-                            reply_markup=None):
+                            has_spoiler: bool = None,
+                            reply_markup=None,
+                            **kwargs):
         """Send animation files (GIF or H.264/MPEG-4 AVC video without sound).
 
         See https://core.telegram.org/bots/api#sendanimation for details.
         """
+        if 'thumb' in kwargs:
+            thumbnail = kwargs['thumb']
+            logging.error("DEPRECATION WARNING: `thumb` parameter of function"
+                          "`sendAnimation` has been deprecated since Bot API 6.6. "
+                          "Use `thumbnail` instead.")
         return await self.api_request(
             'sendAnimation',
             parameters=locals()
         )
 
     async def sendVoice(self, chat_id: Union[int, str], voice,
                         caption: str = None,
@@ -805,25 +924,31 @@
             'sendVoice',
             parameters=locals()
         )
 
     async def sendVideoNote(self, chat_id: Union[int, str], video_note,
                             duration: int = None,
                             length: int = None,
-                            thumb=None,
+                            thumbnail=None,
                             disable_notification: bool = None,
                             reply_to_message_id: int = None,
                             allow_sending_without_reply: bool = None,
                             message_thread_id: int = None,
                             protect_content: bool = None,
-                            reply_markup=None):
+                            reply_markup=None,
+                            **kwargs):
         """Send a rounded square mp4 video message of up to 1 minute long.
 
         See https://core.telegram.org/bots/api#sendvideonote for details.
         """
+        if 'thumb' in kwargs:
+            thumbnail = kwargs['thumb']
+            logging.error("DEPRECATION WARNING: `thumb` parameter of function"
+                          "`sendVideoNote` has been deprecated since Bot API 6.6. "
+                          "Use `thumbnail` instead.")
         return await self.api_request(
             'sendVideoNote',
             parameters=locals()
         )
 
     async def sendMediaGroup(self, chat_id: Union[int, str], media: list,
                              disable_notification: bool = None,
@@ -1006,15 +1131,16 @@
         parameters['type'] = parameters['type_']
         del parameters['type_']
         return await self.api_request(
             'sendPoll',
             parameters=parameters
         )
 
-    async def sendChatAction(self, chat_id: Union[int, str], action):
+    async def sendChatAction(self, chat_id: Union[int, str], action,
+                             message_thread_id: int = None):
         """Fake a typing status or similar.
 
         See https://core.telegram.org/bots/api#sendchataction for details.
         """
         return await self.api_request(
             'sendChatAction',
             parameters=locals()
@@ -1054,15 +1180,15 @@
         """Kick a user from a group, a supergroup or a channel.
 
         In the case of supergroups and channels, the user will not be able to
             return to the group on their own using invite links, etc., unless
             unbanned first.
         Note: In regular groups (non-supergroups), this method will only work
             if the ‘All Members Are Admins’ setting is off in the target group.
-            Otherwise members may only be removed by the group's creator or by
+            Otherwise, members may only be removed by the group's creator or by
             the member that added them.
         See https://core.telegram.org/bots/api#kickchatmember for details.
         """
         return await self.api_request(
             'kickChatMember',
             parameters=locals()
         )
@@ -1083,14 +1209,15 @@
         return await self.api_request(
             'unbanChatMember',
             parameters=locals()
         )
 
     async def restrictChatMember(self, chat_id: Union[int, str], user_id: int,
                                  permissions: Dict[str, bool],
+                                 use_independent_chat_permissions: bool = None,
                                  until_date: Union[datetime.datetime, int] = None):
         """Restrict a user in a supergroup.
 
         The bot must be an administrator in the supergroup for this to work
             and must have the appropriate admin rights.
             Pass True for all boolean parameters to lift restrictions from a
             user.
@@ -1241,15 +1368,15 @@
         """
         return await self.api_request(
             'leaveChat',
             parameters=locals()
         )
 
     async def getChat(self, chat_id: Union[int, str]):
-        """Get up to date information about the chat.
+        """Get up-to-date information about the chat.
 
         Return a Chat object on success.
         See https://core.telegram.org/bots/api#getchat for details.
         """
         return await self.api_request(
             'getChat',
             parameters=locals()
@@ -1457,17 +1584,20 @@
     async def sendSticker(self, chat_id: Union[int, str],
                           sticker: Union[str, dict, IO],
                           disable_notification: bool = None,
                           reply_to_message_id: int = None,
                           allow_sending_without_reply: bool = None,
                           message_thread_id: int = None,
                           protect_content: bool = None,
+                          emoji: str = None,
                           reply_markup=None):
         """Send `.webp` stickers.
 
+        `sticker` must be a file path, a URL, a file handle or a dict
+            {"file": io_file_handle}, to allow multipart/form-data encoding.
         On success, the sent Message is returned.
         See https://core.telegram.org/bots/api#sendsticker for details.
         """
         sticker = self.prepare_file_object(sticker)
         if sticker is None:
             logging.error("Invalid sticker provided!")
             return
@@ -1486,96 +1616,123 @@
         See https://core.telegram.org/bots/api#getstickerset for details.
         """
         return await self.api_request(
             'getStickerSet',
             parameters=locals()
         )
 
-    async def uploadStickerFile(self, user_id, png_sticker):
-        """Upload a .png file as a sticker.
-
-        Use it later via `createNewStickerSet` and `addStickerToSet` methods
-            (can be used multiple times).
-        Return the uploaded File on success.
-        `png_sticker` must be a *.png image up to 512 kilobytes in size,
-            dimensions must not exceed 512px, and either width or height must
-            be exactly 512px.
+    async def uploadStickerFile(self, user_id: int, sticker: Union[str, dict, IO],
+                                sticker_format: str, **kwargs):
+        """Upload an image file for later use in sticker packs.
+
+        Use this method to upload a file with a sticker for later use in the
+            createNewStickerSet and addStickerToSet methods
+            (the file can be used multiple times).
+        `sticker` must be a file path, a file handle or a dict
+            {"file": io_file_handle}, to allow multipart/form-data encoding.
+        Returns the uploaded File on success.
         See https://core.telegram.org/bots/api#uploadstickerfile for details.
         """
-        return await self.api_request(
+        if 'png_sticker' in kwargs:
+            sticker = kwargs['png_sticker']
+            logging.error("DEPRECATION WARNING: `png_sticker` parameter of function"
+                          "`uploadStickerFile` has been deprecated since Bot API 6.6. "
+                          "Use `sticker` instead.")
+        if sticker_format not in ("static", "animated", "video"):
+            logging.error(f"Unknown sticker format `{sticker_format}`.")
+        sticker = self.prepare_file_object(sticker)
+        if sticker is None:
+            logging.error("Invalid sticker provided!")
+            return
+        result = await self.api_request(
             'uploadStickerFile',
             parameters=locals()
         )
+        if type(sticker) is dict:  # Close sticker file, if it was open
+            sticker['file'].close()
+        return result
 
     async def createNewStickerSet(self, user_id: int, name: str, title: str,
-                                  emojis: str,
-                                  png_sticker: Union[str, dict, IO] = None,
-                                  tgs_sticker: Union[str, dict, IO] = None,
-                                  webm_sticker: Union[str, dict, IO] = None,
+                                  stickers: List['InputSticker'],
+                                  sticker_format: str = 'static',
                                   sticker_type: str = 'regular',
-                                  mask_position: dict = None,
+                                  needs_repainting: bool = False,
                                   **kwargs):
         """Create new sticker set owned by a user.
 
         The bot will be able to edit the created sticker set.
         Returns True on success.
         See https://core.telegram.org/bots/api#createnewstickerset for details.
         """
+        if stickers is None:
+            stickers = []
         if 'contains_masks' in kwargs:
             logging.error("Parameter `contains_masks` of method "
                           "`createNewStickerSet` has been deprecated. "
                           "Use `sticker_type = 'mask'` instead.")
             sticker_type = 'mask' if kwargs['contains_masks'] else 'regular'
-        if sticker_type not in ('regular', 'mask'):
-            raise TypeError
-        png_sticker = self.prepare_file_object(png_sticker)
-        tgs_sticker = self.prepare_file_object(tgs_sticker)
-        webm_sticker = self.prepare_file_object(webm_sticker)
-        if png_sticker is None and tgs_sticker is None and webm_sticker is None:
-            logging.error("Invalid sticker provided!")
-            return
+        for old_sticker_format in ('png_sticker', 'tgs_sticker', 'webm_sticker'):
+            if old_sticker_format in kwargs:
+                if 'emojis' not in kwargs:
+                    logging.error(f"No `emojis` provided together with "
+                                  f"`{old_sticker_format}`. To create new "
+                                  f"sticker set with some stickers in it, use "
+                                  f"the new `stickers` parameter.")
+                    return
+                logging.error(f"Parameter `{old_sticker_format}` of method "
+                              "`createNewStickerSet` has been deprecated since"
+                              "Bot API 6.6. "
+                              "Use `stickers` instead.")
+                stickers.append(
+                    self.make_input_sticker(
+                        sticker=kwargs[old_sticker_format],
+                        emoji_list=kwargs['emojis']
+                    )
+                )
+        if sticker_type not in ('regular', 'mask', 'custom_emoji'):
+            raise TypeError(f"Unknown sticker type `{sticker_type}`.")
         result = await self.api_request(
             'createNewStickerSet',
-            parameters=locals()
+            parameters=locals(),
+            exclude=['old_sticker_format']
         )
-        if type(png_sticker) is dict:  # Close png_sticker file, if it was open
-            png_sticker['file'].close()
-        if type(tgs_sticker) is dict:  # Close tgs_sticker file, if it was open
-            tgs_sticker['file'].close()
-        if type(webm_sticker) is dict:  # Close webm_sticker file, if it was open
-            webm_sticker['file'].close()
         return result
 
     async def addStickerToSet(self, user_id: int, name: str,
-                              emojis: str,
-                              png_sticker: Union[str, dict, IO] = None,
-                              tgs_sticker: Union[str, dict, IO] = None,
-                              webm_sticker: Union[str, dict, IO] = None,
-                              mask_position: dict = None):
+                              sticker: InputSticker = None,
+                              **kwargs):
         """Add a new sticker to a set created by the bot.
 
         Returns True on success.
         See https://core.telegram.org/bots/api#addstickertoset for details.
         """
-        png_sticker = self.prepare_file_object(png_sticker)
-        tgs_sticker = self.prepare_file_object(tgs_sticker)
-        webm_sticker = self.prepare_file_object(webm_sticker)
-        if png_sticker is None and tgs_sticker is None and webm_sticker is None:
-            logging.error("Invalid sticker provided!")
+        for old_sticker_format in ('png_sticker', 'tgs_sticker', 'webm_sticker'):
+            if old_sticker_format in kwargs:
+                if 'emojis' not in kwargs:
+                    logging.error(f"No `emojis` provided together with "
+                                  f"`{old_sticker_format}`.")
+                    return
+                logging.error(f"Parameter `{old_sticker_format}` of method "
+                              "`addStickerToSet` has been deprecated since"
+                              "Bot API 6.6. "
+                              "Use `sticker` instead.")
+                sticker = self.make_input_sticker(
+                    sticker=kwargs[old_sticker_format],
+                    emoji_list=kwargs['emojis'],
+                    mask_position=kwargs['mask_position'] if 'mask_position' in kwargs else None
+                )
+        if sticker is None:
+            logging.error("Must provide a sticker of type `InputSticker` to "
+                          "`addStickerToSet` method.")
             return
         result = await self.api_request(
             'addStickerToSet',
-            parameters=locals()
+            parameters=locals(),
+            exclude=['old_sticker_format']
         )
-        if type(png_sticker) is dict:  # Close png_sticker file, if it was open
-            png_sticker['file'].close()
-        if type(tgs_sticker) is dict:  # Close tgs_sticker file, if it was open
-            tgs_sticker['file'].close()
-        if type(webm_sticker) is dict:  # Close webm_sticker file, if it was open
-            webm_sticker['file'].close()
         return result
 
     async def setStickerPositionInSet(self, sticker, position):
         """Move a sticker in a set created by the bot to a specific position .
 
         Position is 0-based.
         Returns True on success.
@@ -1599,22 +1756,26 @@
             parameters=locals()
         )
 
     async def answerInlineQuery(self, inline_query_id, results,
                                 cache_time=None,
                                 is_personal=None,
                                 next_offset=None,
-                                switch_pm_text=None,
-                                switch_pm_parameter=None):
+                                button: Union['InlineQueryResultsButton', None] = None,
+                                **kwargs):
         """Send answers to an inline query.
 
         On success, True is returned.
         No more than 50 results per query are allowed.
         See https://core.telegram.org/bots/api#answerinlinequery for details.
         """
+        if 'switch_pm_text' in kwargs:
+            button = InlineQueryResultsButton(text=kwargs['switch_pm_text'])
+        if 'switch_pm_parameter' in kwargs:
+            button = InlineQueryResultsButton(start_parameter=kwargs['switch_pm_parameter'])
         return await self.api_request(
             'answerInlineQuery',
             parameters=locals()
         )
 
     async def sendInvoice(self, chat_id: int, title: str, description: str,
                           payload: str, provider_token: str,
@@ -1806,15 +1967,16 @@
             'setChatAdministratorCustomTitle',
             parameters=locals()
         )
 
     async def setChatPermissions(self,
                                  chat_id: Union[int, str] = None,
                                  permissions: Union[ChatPermissions,
-                                                    dict] = None):
+                                                    dict] = None,
+                                 use_independent_chat_permissions: bool = None):
         """Set default chat permissions for all members.
 
         Use this method to set default chat permissions for all members.
         The bot must be an administrator in the group or a supergroup for this
             to work and must have the can_restrict_members admin rights.
         Returns True on success.
         See https://core.telegram.org/bots/api#setchatpermissions for details.
@@ -2281,7 +2443,224 @@
         Returns the created invoice link as String on success.
         See https://core.telegram.org/bots/api#createinvoicelink for details.
         """
         return await self.api_request(
             'createInvoiceLink',
             parameters=locals()
         )
+
+    async def editGeneralForumTopic(self, chat_id: Union[int, str], name: str):
+        """Edit the name of the 'General' topic in a forum supergroup chat.
+
+        The bot must be an administrator in the chat for this to work and must
+            have can_manage_topics administrator rights.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#editgeneralforumtopic for details.
+        """
+        return await self.api_request(
+            'editGeneralForumTopic',
+            parameters=locals()
+        )
+
+    async def closeGeneralForumTopic(self, chat_id: Union[int, str]):
+        """Close an open 'General' topic in a forum supergroup chat.
+
+        The bot must be an administrator in the chat for this to work and must
+            have the can_manage_topics administrator rights.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#closegeneralforumtopic for details.
+        """
+        return await self.api_request(
+            'closeGeneralForumTopic',
+            parameters=locals()
+        )
+
+    async def reopenGeneralForumTopic(self, chat_id: Union[int, str]):
+        """Reopen a closed 'General' topic in a forum supergroup chat.
+
+        The bot must be an administrator in the chat for this to work and must
+            have the can_manage_topics administrator rights.
+            The topic will be automatically unhidden if it was hidden.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#reopengeneralforumtopic for details.
+        """
+        return await self.api_request(
+            'reopenGeneralForumTopic',
+            parameters=locals()
+        )
+
+    async def hideGeneralForumTopic(self, chat_id: Union[int, str]):
+        """Hide the 'General' topic in a forum supergroup chat.
+
+        The bot must be an administrator in the chat for this to work and
+            must have the can_manage_topics administrator rights.
+            The topic will be automatically closed if it was open.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#hidegeneralforumtopic for details.
+        """
+        return await self.api_request(
+            'hideGeneralForumTopic',
+            parameters=locals()
+        )
+
+    async def unhideGeneralForumTopic(self, chat_id: Union[int, str]):
+        """Unhide the 'General' topic in a forum supergroup chat.
+
+        The bot must be an administrator in the chat for this to work and must
+            have the can_manage_topics administrator rights.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#unhidegeneralforumtopic for details.
+        """
+        return await self.api_request(
+            'unhideGeneralForumTopic',
+            parameters=locals()
+        )
+
+    async def setMyName(self, name: str, language_code: str):
+        """Change the bot's name.
+
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setmyname for details.
+        """
+        return await self.api_request(
+            'setMyName',
+            parameters=locals()
+        )
+
+    async def getMyName(self, language_code: str):
+        """Get the current bot name for the given user language.
+
+        Returns BotName on success.
+        See https://core.telegram.org/bots/api#getmyname for details.
+        """
+        return await self.api_request(
+            'getMyName',
+            parameters=locals()
+        )
+
+    async def setMyDescription(self, description: str, language_code: str):
+        """Change the bot's description, which is shown in the chat with the bot if
+            the chat is empty.
+
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setmydescription for details.
+        """
+        return await self.api_request(
+            'setMyDescription',
+            parameters=locals()
+        )
+
+    async def getMyDescription(self, language_code: str):
+        """Get the current bot description for the given user language.
+
+        Returns BotDescription on success.
+        See https://core.telegram.org/bots/api#getmydescription for details.
+        """
+        return await self.api_request(
+            'getMyDescription',
+            parameters=locals()
+        )
+
+    async def setMyShortDescription(self, short_description: str, language_code: str):
+        """Change the bot's short description, which is shown on the bot's profile
+            page and is sent together with the link when users share the bot.
+
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setmyshortdescription for details.
+        """
+        return await self.api_request(
+            'setMyShortDescription',
+            parameters=locals()
+        )
+
+    async def getMyShortDescription(self, language_code: str):
+        """Get the current bot short description for the given user language.
+
+        Returns BotShortDescription on success.
+        See https://core.telegram.org/bots/api#getmyshortdescription for details.
+        """
+        return await self.api_request(
+            'getMyShortDescription',
+            parameters=locals()
+        )
+
+    async def setStickerEmojiList(self, sticker: str, emoji_list: List[str]):
+        """Change the list of emoji assigned to a regular or custom emoji sticker.
+
+        The sticker must belong to a sticker set created by the bot.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setstickeremojilist for details.
+        """
+        return await self.api_request(
+            'setStickerEmojiList',
+            parameters=locals()
+        )
+
+    async def setStickerKeywords(self, sticker: str, keywords: List[str]):
+        """Change search keywords assigned to a regular or custom emoji sticker.
+
+        The sticker must belong to a sticker set created by the bot.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setstickerkeywords for details.
+        """
+        return await self.api_request(
+            'setStickerKeywords',
+            parameters=locals()
+        )
+
+    async def setStickerMaskPosition(self, sticker: str, mask_position: 'MaskPosition'):
+        """Change the mask position of a mask sticker.
+
+        The sticker must belong to a sticker set that was created by the bot.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setstickermaskposition for details.
+        """
+        return await self.api_request(
+            'setStickerMaskPosition',
+            parameters=locals()
+        )
+
+    async def setStickerSetTitle(self, name: str, title: str):
+        """Set the title of a created sticker set.
+
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setstickersettitle for details.
+        """
+        return await self.api_request(
+            'setStickerSetTitle',
+            parameters=locals()
+        )
+
+    async def setStickerSetThumbnail(self, name: str, user_id: int, thumbnail: 'InputFile or String'):
+        """Set the thumbnail of a regular or mask sticker set.
+
+        The format of the thumbnail file must match the format of the stickers
+            in the set.
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setstickersetthumbnail for details.
+        """
+        return await self.api_request(
+            'setStickerSetThumbnail',
+            parameters=locals()
+        )
+
+    async def setCustomEmojiStickerSetThumbnail(self, name: str, custom_emoji_id: str):
+        """Set the thumbnail of a custom emoji sticker set.
+
+        Returns True on success.
+        See https://core.telegram.org/bots/api#setcustomemojistickersetthumbnail for details.
+        """
+        return await self.api_request(
+            'setCustomEmojiStickerSetThumbnail',
+            parameters=locals()
+        )
+
+    async def deleteStickerSet(self, name: str):
+        """Delete a sticker set that was created by the bot.
+
+        Returns True on success.
+        See https://core.telegram.org/bots/api#deletestickerset for details.
+        """
+        return await self.api_request(
+            'deleteStickerSet',
+            parameters=locals()
+        )
```

### Comparing `davtelepot-2.8.9/davtelepot/api_helper.py` & `davtelepot-2.9.1/davtelepot/api_helper.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,14 +43,37 @@
 
     @property
     def description(self):
         """Return method description."""
         return self._description
 
     @property
+    def description_80chars(self):
+        """Return method description, breaking lines at 80 characters."""
+        result, current_line = '', ''
+        indentation = 8
+        redundant_string = "Use this method to "
+        for n, paragraph in enumerate(self.description.replace('.', '.\n').split('\n')):
+            additional_indentation = 0
+            if n == 0 and paragraph.startswith(redundant_string):
+                paragraph = paragraph[len(redundant_string)].upper() + paragraph[len(redundant_string)+1:]
+            for word in paragraph.split(' '):
+                if len(current_line) + len(word) > 80 - indentation - additional_indentation:
+                    additional_indentation = max(additional_indentation, 4)
+                    result += f"{current_line.strip()}\n{' ' * additional_indentation}"
+                    current_line = ""
+                current_line += f"{word} "
+            if len(current_line):
+                result += f"{current_line.strip()}\n"
+                current_line = ""
+            if n == 0:
+                result += '\n'
+        return result.strip()
+
+    @property
     def table(self):
         """Return method parameters table."""
         return self._table
 
     @property
     def parameters(self):
         return self._parameters
@@ -189,15 +212,15 @@
                     "class Bot(TelegramBot):\n\n"
                 )
             file.writelines(
                 f"    async def {method.name}("
                 f"{', '.join(['self'] + method.parameters_with_types)}"
                 f"):\n"
                 f"        \"\"\""
-                f"{method.description.replace(new_line, new_line + ' ' * 4)}\n"
+                f"{method.description_80chars.replace(new_line, new_line + ' ' * 8)}\n"
                 f"        See https://core.telegram.org/bots/api#"
                 f"{method.name.lower()} for details.\n"
                 f"        \"\"\"\n"
                 f"        return await self.api_request(\n"
                 f"            '{method.name}',\n"
                 f"            parameters=locals()\n"
                 f"        )\n\n"
```

### Comparing `davtelepot-2.8.9/davtelepot/authorization.py` & `davtelepot-2.9.1/davtelepot/authorization.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/bot.py` & `davtelepot-2.9.1/davtelepot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,30 +50,30 @@
 
 # Project modules
 from davtelepot.api import TelegramBot, TelegramError
 from davtelepot.database import ObjectWithDatabase
 from davtelepot.languages import MultiLanguageObject
 from davtelepot.messages import davtelepot_messages
 from davtelepot.utilities import (
-    async_get, escape_html_chars, extract, get_secure_key,
+    async_get, clean_html_string, extract, get_secure_key,
     make_inline_query_answer, make_lines_of_buttons, remove_html_tags
 )
 
 # Do not log aiohttp `INFO` and `DEBUG` levels
 logging.getLogger('aiohttp').setLevel(logging.WARNING)
 # Same with chardet
 logging.getLogger('chardet').setLevel(logging.WARNING)
 
 
 # Some methods are not implemented yet: that's the reason behind the following statement
 # noinspection PyUnusedLocal,PyMethodMayBeStatic,PyMethodMayBeStatic
 class Bot(TelegramBot, ObjectWithDatabase, MultiLanguageObject):
     """Simple Bot object, providing methods corresponding to Telegram bot API.
 
-    Multiple Bot() instances may be run together, along with a aiohttp web app.
+    Multiple Bot() instances may be run together, along with an aiohttp web app.
     """
 
     bots = []
     _path = '.'
     runner = None
     server = None
     # TODO: find a way to choose port automatically by default
@@ -95,15 +95,17 @@
             input_message_content=dict(
                 message_text="I'm sorry "
                 "but I could not find an answer for your query."
             )
         )
     ]
     _log_file_name = None
+    _log_file_path = None
     _errors_file_name = None
+    _errors_file_path = None
     _documents_max_dimension = 50 * 1000 * 1000  # 50 MB
 
     def __init__(
         self, token, hostname='', certificate=None, max_connections=40,
         allowed_updates=None, database_url='bot.db'
     ):
         """Init a bot instance.
@@ -233,15 +235,17 @@
         # Default authorization function (always return True)
         self.authorization_function = (
             lambda update, user_record=None, authorization_level='user': True
         )
         self.default_reply_keyboard_elements = []
         self.recent_users = OrderedDict()
         self._log_file_name = None
+        self._log_file_path = None
         self._errors_file_name = None
+        self._errors_file_path = None
         self.placeholder_requests = dict()
         self.shared_data = dict()
         self.Role = None
         self.packages = [sys.modules['davtelepot']]
         self._documents_max_dimension = None
         # Add `users` table with its fields if missing
         if 'users' not in self.db.tables:
@@ -317,56 +321,88 @@
 
         Fallback to class file name if set, otherwise return None.
         """
         return self._log_file_name or self.__class__._log_file_name
 
     @property
     def log_file_path(self):
-        """Return log file path basing on self.path and `_log_file_name`.
+        """Return log file path.
 
+        If an instance file path is set, return it.
+        If not and a class file path is set, return that.
+        Otherwise, generate a file path basing on `self.path` and `_log_file_name`
         Fallback to class file if set, otherwise return None.
         """
+        if self._log_file_path:
+            return self._log_file_path
+        if self.__class__._log_file_path:
+            return self.__class__._log_file_path
         if self.log_file_name:
             return f"{self.path}/data/{self.log_file_name}"
 
     def set_log_file_name(self, file_name):
         """Set log file name."""
         self._log_file_name = file_name
 
     @classmethod
     def set_class_log_file_name(cls, file_name):
         """Set class log file name."""
         cls._log_file_name = file_name
 
+    def set_log_file_path(self, file_path):
+        """Set log file path."""
+        self._log_file_path = file_path
+
+    @classmethod
+    def set_class_log_file_path(cls, file_path):
+        """Set class log file path."""
+        cls._log_file_path = file_path
+
     @property
     def errors_file_name(self):
         """Return errors file name.
 
         Fallback to class file name if set, otherwise return None.
         """
         return self._errors_file_name or self.__class__._errors_file_name
 
     @property
     def errors_file_path(self):
-        """Return errors file path basing on self.path and `_errors_file_name`.
+        """Return errors file path.
 
+        If an instance file path is set, return it.
+        If not and a class file path is set, return that.
+        Otherwise, generate a file path basing on `self.path` and `_errors_file_name`
         Fallback to class file if set, otherwise return None.
         """
+        if self.__class__._errors_file_path:
+            return self.__class__._errors_file_path
+        if self._errors_file_path:
+            return self._errors_file_path
         if self.errors_file_name:
             return f"{self.path}/data/{self.errors_file_name}"
 
     def set_errors_file_name(self, file_name):
         """Set errors file name."""
         self._errors_file_name = file_name
 
     @classmethod
     def set_class_errors_file_name(cls, file_name):
         """Set class errors file name."""
         cls._errors_file_name = file_name
 
+    def set_errors_file_path(self, file_path):
+        """Set errors file path."""
+        self._errors_file_path = file_path
+
+    @classmethod
+    def set_class_errors_file_path(cls, file_path):
+        """Set class errors file path."""
+        cls._errors_file_path = file_path
+
     @classmethod
     def get(cls, token, *args, **kwargs):
         """Given a `token`, return class instance with that token.
 
         If no instance is found, instantiate it.
         Positional and keyword arguments may be passed as well.
         """
@@ -413,15 +449,15 @@
         return self._certificate
 
     @property
     def max_connections(self):
         """Maximum number of simultaneous HTTPS connections allowed.
 
         Telegram will open as many connections as possible to boost bot’s
-            throughput, lower values limit the load on bot‘s server.
+            throughput, lower values limit the load on bot's server.
         """
         return self._max_connections
 
     @property
     def allowed_updates(self):
         """List of update types to be retrieved.
 
@@ -473,15 +509,15 @@
         """
         return self._under_maintenance
 
     @property
     def allowed_during_maintenance(self):
         """Return the list of criteria to allow an update during maintenance.
 
-        If any of this criteria returns True on an update, that update will be
+        If any of these criteria returns True on an update, that update will be
             handled even during maintenance.
         """
         return self._allowed_during_maintenance
 
     @property
     def maintenance_message(self):
         """Message to be returned if bot is under maintenance.
@@ -854,15 +890,15 @@
                     if 'language_labelled_commands' in description
                        and language in description['language_labelled_commands']
                        and command == description['language_labelled_commands'][language]
                 ][0]
             elif 'chat' in update and update['chat']['id'] > 0:
                 reply = dict(text=self.unknown_command_message)
         else:  # Handle command aliases and text parsers
-            # Aliases are case insensitive: text and alias are both .lower()
+            # Aliases are case-insensitive: text and alias are both .lower()
             for alias, function in self.command_aliases.items():
                 if lowered_text.startswith(alias.lower()):
                     replier = function
                     break
             # Text message update parsers
             for check_function, parser in self.text_message_parsers.items():
                 if check_function(
@@ -1218,15 +1254,15 @@
         r"""Split text if it hits telegram limits for text messages.
 
         Split at `\n` if possible.
         Add a `[...]` at the end and beginning of split messages,
         with proper code markdown.
         """
         if parse_mode == 'HTML':
-            text = escape_html_chars(text)
+            text = clean_html_string(text)
         tags = (
             ('`', '`')
             if parse_mode == 'Markdown'
             else ('<code>', '</code>')
             if parse_mode.lower() == 'html'
             else ('', '')
         )
@@ -1587,15 +1623,15 @@
             else:
                 already_sent = False
                 if not any(
                     [
                             photo.startswith(url_starter)
                             for url_starter in ('http', 'www',)
                         ]
-                ):  # If `photo` is not a url but a local file path
+                ):  # If `photo` is not a URL but a local file path
                     try:
                         with io.BytesIO() as buffered_picture:
                             with open(
                                 os.path.join(self.path, photo_path),
                                 'rb'  # Read bytes
                             ) as photo_file:
                                 buffered_picture.write(photo_file.read())
@@ -1654,15 +1690,15 @@
     async def send_audio(self, chat_id: Union[int, str], audio,
                          caption: str = None,
                          parse_mode: str = None,
                          caption_entities: List[dict] = None,
                          duration: int = None,
                          performer: str = None,
                          title: str = None,
-                         thumb=None,
+                         thumbnail=None,
                          disable_notification: bool = None,
                          reply_to_message_id: int = None,
                          allow_sending_without_reply: bool = None,
                          reply_markup=None,
                          update: dict = None,
                          reply_to_update: bool = False,
                          send_default_keyboard: bool = True,
@@ -1712,15 +1748,15 @@
             else:
                 already_sent = False
                 if not any(
                     [
                             audio.startswith(url_starter)
                             for url_starter in ('http', 'www',)
                         ]
-                ):  # If `audio` is not a url but a local file path
+                ):  # If `audio` is not a URL but a local file path
                     try:
                         with io.BytesIO() as buffered_picture:
                             with open(
                                 os.path.join(self.path, audio_path),
                                 'rb'  # Read bytes
                             ) as audio_file:
                                 buffered_picture.write(audio_file.read())
@@ -1739,15 +1775,15 @@
                 audio=audio,
                 caption=caption,
                 parse_mode=parse_mode,
                 caption_entities=caption_entities,
                 duration=duration,
                 performer=performer,
                 title=title,
-                thumb=thumb,
+                thumbnail=thumbnail,
                 disable_notification=disable_notification,
                 reply_to_message_id=reply_to_message_id,
                 allow_sending_without_reply=allow_sending_without_reply,
                 reply_markup=reply_markup
             )
             if isinstance(sent_update, Exception):
                 raise Exception("sendAudio API call failed!")
@@ -1837,15 +1873,15 @@
             else:
                 already_sent = False
                 if not any(
                     [
                             voice.startswith(url_starter)
                             for url_starter in ('http', 'www',)
                         ]
-                ):  # If `voice` is not a url but a local file path
+                ):  # If `voice` is not a URL but a local file path
                     try:
                         with io.BytesIO() as buffered_picture:
                             with open(
                                 os.path.join(self.path, voice_path),
                                 'rb'  # Read bytes
                             ) as voice_file:
                                 buffered_picture.write(voice_file.read())
@@ -1898,15 +1934,15 @@
                         file_id=sent_update['voice']['file_id'],
                         errors=False
                     )
                 )
         return sent_update
 
     async def send_document(self, chat_id: Union[int, str] = None, document=None,
-                            thumb=None,
+                            thumbnail=None,
                             caption: str = None,
                             parse_mode: str = None,
                             caption_entities: List[dict] = None,
                             disable_content_type_detection: bool = None,
                             disable_notification: bool = None,
                             reply_to_message_id: int = None,
                             allow_sending_without_reply: bool = None,
@@ -1973,15 +2009,15 @@
             else:
                 already_sent = False
                 if not any(
                     [
                             document_path.startswith(url_starter)
                             for url_starter in ('http', 'www',)
                         ]
-                ):  # If `document_path` is not a url but a local file path
+                ):  # If `document_path` is not a URL but a local file path
                     try:
                         with open(
                             document_path.format(
                                 path=self.path
                             ),
                             'rb'  # Read bytes
                         ) as file_:
@@ -2017,15 +2053,15 @@
                                         f"{part} {i + 1}"
                                     )
                                 else:
                                     buffered_file.name = original_document_name
                                 sent_document = await self.send_document(
                                     chat_id=chat_id,
                                     document=buffered_file,
-                                    thumb=thumb,
+                                    thumbnail=thumbnail,
                                     caption=caption,
                                     parse_mode=parse_mode,
                                     disable_notification=disable_notification,
                                     reply_to_message_id=reply_to_message_id,
                                     reply_markup=reply_markup,
                                     update=update,
                                     reply_to_update=reply_to_update,
@@ -2046,15 +2082,15 @@
             )
             return Exception("No `document` provided")
         sent_update = None
         try:
             sent_update = await self.sendDocument(
                 chat_id=chat_id,
                 document=document,
-                thumb=thumb,
+                thumbnail=thumbnail,
                 caption=caption,
                 parse_mode=parse_mode,
                 caption_entities=caption_entities,
                 disable_content_type_detection=disable_content_type_detection,
                 disable_notification=disable_notification,
                 reply_to_message_id=reply_to_message_id,
                 allow_sending_without_reply=allow_sending_without_reply,
@@ -3107,16 +3143,17 @@
     async def close_sessions(self):
         """Close open sessions."""
         for session_name, session in self.sessions.items():
             if not session.closed:
                 await session.close()
 
     async def send_one_message(self, *args, **kwargs):
-        await self.send_message(*args, **kwargs)
+        sent_message = await self.send_message(*args, **kwargs)
         await self.close_sessions()
+        return sent_message
 
     async def set_webhook(self, url=None, certificate=None,
                           max_connections=None, allowed_updates=None):
         """Set a webhook if token is valid."""
         # Return if token is invalid
         await self.get_me()
         if self.name is None:
@@ -3158,15 +3195,15 @@
             Timeout set for Telegram servers. Make sure that connection timeout
             is greater than `timeout`.
         limit : int (1 - 100)
             Max number of updates to be retrieved.
         allowed_updates : List(str)
             List of update types to be retrieved.
             Empty list to allow all updates.
-            None to fallback to class default.
+            None to fall back to class default.
         """
         # Return if token is invalid
         await self.get_me()
         if self.name is None:
             return
         # Set custom list of allowed updates or fallback to class default list
         if allowed_updates is None:
```

### Comparing `davtelepot-2.8.9/davtelepot/database.py` & `davtelepot-2.9.1/davtelepot/database.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/helper.py` & `davtelepot-2.9.1/davtelepot/helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/ietf_language_tags.csv` & `davtelepot-2.9.1/davtelepot/ietf_language_tags.csv`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/languages.py` & `davtelepot-2.9.1/davtelepot/languages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/messages.py` & `davtelepot-2.9.1/davtelepot/messages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/suggestions.py` & `davtelepot-2.9.1/davtelepot/suggestions.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/tools/merge_files.py` & `davtelepot-2.9.1/davtelepot/tools/merge_files.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/useful_tools.py` & `davtelepot-2.9.1/davtelepot/useful_tools.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/davtelepot/utilities.py` & `davtelepot-2.9.1/davtelepot/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import os
 import random
 import re
 import string
 import time
 
 from difflib import SequenceMatcher
+from typing import Tuple, Union
 
 # Third party modules
-from typing import Tuple, Union
 
 import aiohttp
 from bs4 import BeautifulSoup
 
 
 weekdays = collections.OrderedDict()
 weekdays[0] = {
@@ -1247,15 +1247,15 @@
                     type_=TIME_WORDS[word]['type_']
                 )
             )
         if succeeded:
             result_text.pop()
             if len(result_text) > 0 and result_text[-1].lower() in TIME_WORDS:
                 result_text.pop()
-    result_text = escape_html_chars(
+    result_text = clean_html_string(
         ' '.join(result_text)
     )
     parsers = list(
         filter(
             lambda x: 'result' in x and x['result'],
             parsers
         )
@@ -1326,14 +1326,30 @@
 MONTH_NAMES_ITA[7] = "luglio"
 MONTH_NAMES_ITA[8] = "agosto"
 MONTH_NAMES_ITA[9] = "settembre"
 MONTH_NAMES_ITA[10] = "ottobre"
 MONTH_NAMES_ITA[11] = "novembre"
 MONTH_NAMES_ITA[12] = "dicembre"
 
+allowed_html_tags = ['b', 'strong',
+                     'i', 'em',
+                     'u', 'ins',
+                     's', 'strike', 'del',
+                     'span', 'tg-spoiler',
+                     'a',
+                     'code', 'pre']
+
+HTML_SYMBOLS = collections.OrderedDict()
+HTML_SYMBOLS["&"] = "&amp;"
+HTML_SYMBOLS["<"] = "&lt;"
+HTML_SYMBOLS[">"] = "&gt;"
+HTML_SYMBOLS["\""] = "&quot;"
+
+html_numeric_code_regex = re.compile(r'&amp;(?P<code>#\d{2,3};)')
+
 
 def beautytd(td):
     """Format properly timedeltas."""
     result = ''
     if type(td) is int:
         td = datetime.timedelta(seconds=td)
     assert isinstance(
@@ -1406,75 +1422,65 @@
                     else " {}".format(dt.year)
                 )
             )
         )
     return result
 
 
-HTML_SYMBOLS = MyOD()
-HTML_SYMBOLS["&"] = "&amp;"
-HTML_SYMBOLS["<"] = "&lt;"
-HTML_SYMBOLS[">"] = "&gt;"
-HTML_SYMBOLS["\""] = "&quot;"
-HTML_SYMBOLS["&lt;b&gt;"] = "<b>"
-HTML_SYMBOLS["&lt;/b&gt;"] = "</b>"
-HTML_SYMBOLS["&lt;i&gt;"] = "<i>"
-HTML_SYMBOLS["&lt;/i&gt;"] = "</i>"
-HTML_SYMBOLS["&lt;code&gt;"] = "<code>"
-HTML_SYMBOLS["&lt;/code&gt;"] = "</code>"
-HTML_SYMBOLS["&lt;pre&gt;"] = "<pre>"
-HTML_SYMBOLS["&lt;/pre&gt;"] = "</pre>"
-HTML_SYMBOLS["&lt;a href=&quot;"] = "<a href=\""
-HTML_SYMBOLS["&quot;&gt;"] = "\">"
-HTML_SYMBOLS["&lt;/a&gt;"] = "</a>"
-
-HTML_TAGS = [
-    None, "<b>", "</b>",
-    None, "<i>", "</i>",
-    None, "<code>", "</code>",
-    None, "<pre>", "</pre>",
-    None, "<a href=\"", "\">", "</a>",
-    None
-]
-
+def clean_html_string(text: str) -> str:
+    """Escape HTML symbols, unless part of a valid tag or numeric code character.
 
-def remove_html_tags(text):
-    """Remove HTML tags from `text`."""
-    for tag in HTML_TAGS:
-        if tag is None:
-            continue
-        text = text.replace(tag, '')
+    Find valid HTML tags;
+    if there are any, choose the first occurring and call the function
+        recursively on what comes before the tag, inside the tag and after the
+        tag, preserving the tag opening and close as they are;
+    if there aren't any, escape HTML symbols except for `&` in HTML numeric code
+        characters (`&#` followed by 2 or 3 digits followed by `;`).
+    """
+    first_match = None
+    for tag in allowed_html_tags:
+        if tag in ('a', ):  # <a> must have href attribute
+            attribute = r" href=\".*\""
+        elif tag in ('span', ):  # <span> must have class attribute with "tg-spoiler" value
+            attribute = r" class=\"tg-spoiler\""
+        elif tag in ('code',):  # <code> may have a class with a programming language as value
+            attribute = r"( class=\".*\")?"
+        else:
+            attribute = ""
+        match = re.search(
+            rf'(?P<opening><{tag}{attribute}>)'
+            rf'(?P<body>.*?)'
+            rf'(?P<close></{tag}>)',
+            text,
+            flags=re.DOTALL
+        )
+        if match and (first_match is None or match.start() < first_match.start()):
+            first_match = match
+    if first_match is not None:
+        groups = first_match.groupdict()
+        text = (f"{clean_html_string(text[:first_match.start()])}"
+                f"{groups['opening']}{clean_html_string(groups['body'])}{groups['close']}"
+                f"{clean_html_string(text[first_match.end():])}")
+    else:
+        for key, value in HTML_SYMBOLS.items():
+            text = text.replace(key, value)
+        if re.search(html_numeric_code_regex, text):
+            text = re.sub(html_numeric_code_regex, r'&\g<code>', text)
     return text
 
 
 def escape_html_chars(text):
-    """Escape HTML chars if not part of a tag."""
-    for s, r in HTML_SYMBOLS.items():
-        text = text.replace(s, r)
-    copy = text
-    expected_tag = None
-    while copy:
-        min_ = min(
-            (
-                dict(
-                    position=copy.find(tag) if tag in copy else len(copy),
-                    tag=tag
-                )
-                for tag in HTML_TAGS
-                if tag
-            ),
-            key=lambda x: x['position'],
-            default=0
-        )
-        if min_['position'] == len(copy):
-            break
-        if expected_tag and min_['tag'] != expected_tag:
-            return text.replace('<', '_').replace('>', '_')
-        expected_tag = HTML_TAGS[HTML_TAGS.index(min_['tag'])+1]
-        copy = extract(copy, min_['tag'])
+    logging.error("`escape_html_chars` function deprecated, use `clean_html_string` instead.")
+    return clean_html_string(text)
+
+
+def remove_html_tags(text):
+    """Remove HTML tags from `text`."""
+    for tag in allowed_html_tags:
+        text = re.sub(rf'</?{tag}( (href|class)=\".*\")?>', '', text)
     return text
 
 
 def accents_to_jolly(text, lower=True):
     """Replace letters with Italian accents with SQL jolly character."""
     to_be_replaced = ('à', 'è', 'é', 'ì', 'ò', 'ù')
     if lower:
```

### Comparing `davtelepot-2.8.9/davtelepot.egg-info/PKG-INFO` & `davtelepot-2.9.1/davtelepot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.8.9
+Version: 2.9.1
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.8.9/davtelepot.egg-info/SOURCES.txt` & `davtelepot-2.9.1/davtelepot.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 davtelepot/__init__.py
+davtelepot/__main__.py
 davtelepot/administration_tools.py
 davtelepot/api.py
 davtelepot/api_helper.py
 davtelepot/authorization.py
 davtelepot/bot.py
+davtelepot/cli.py
 davtelepot/database.py
 davtelepot/helper.py
 davtelepot/ietf_language_tags.csv
 davtelepot/languages.py
 davtelepot/messages.py
 davtelepot/suggestions.py
 davtelepot/useful_tools.py
```

### Comparing `davtelepot-2.8.9/examples/a_simple_bot.py` & `davtelepot-2.9.1/examples/a_simple_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/examples/more_bots_together.py` & `davtelepot-2.9.1/examples/more_bots_together.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/examples/webhook_powered_bot.py` & `davtelepot-2.9.1/examples/webhook_powered_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.8.9/setup.py` & `davtelepot-2.9.1/setup.py`

 * *Files identical despite different names*

