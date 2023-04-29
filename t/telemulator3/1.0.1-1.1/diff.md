# Comparing `tmp/telemulator3-1.0.1.tar.gz` & `tmp/telemulator3-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telemulator3-1.0.1.tar", last modified: Fri Apr 28 10:37:36 2023, max compression
+gzip compressed data, was "telemulator3-1.1.tar", last modified: Sat Apr 29 09:58:59 2023, max compression
```

## Comparing `telemulator3-1.0.1.tar` & `telemulator3-1.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 10:37:36.037724 telemulator3-1.0.1/
--rw-rw-rw-   0        0        0     1094 2023-04-26 12:26:19.000000 telemulator3-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       60 2023-04-28 10:27:40.000000 telemulator3-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3507 2023-04-28 10:37:36.038724 telemulator3-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2917 2023-04-28 10:24:21.000000 telemulator3-1.0.1/README.md
--rw-rw-rw-   0        0        0      110 2023-04-26 12:26:19.000000 telemulator3-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      717 2023-04-28 10:37:36.039726 telemulator3-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-28 10:37:35.918957 telemulator3-1.0.1/telemulator3/
--rw-rw-rw-   0        0        0     5709 2023-04-28 06:15:12.000000 telemulator3-1.0.1/telemulator3/__init__.py
--rw-rw-rw-   0        0        0     7140 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/api.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:37:35.965834 telemulator3-1.0.1/telemulator3/chat/
--rw-rw-rw-   0        0        0      403 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/chat/__init__.py
--rw-rw-rw-   0        0        0     3117 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/chat/base.py
--rw-rw-rw-   0        0        0     2903 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/chat/channel.py
--rw-rw-rw-   0        0        0     1890 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/chat/group.py
--rw-rw-rw-   0        0        0     1330 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/chat/history.py
--rw-rw-rw-   0        0        0     2551 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/chat/keyboard.py
--rw-rw-rw-   0        0        0     3608 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/chat/member.py
--rw-rw-rw-   0        0        0     1268 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/chat/private.py
--rw-rw-rw-   0        0        0     1158 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/dictionaryable.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:37:36.019223 telemulator3-1.0.1/telemulator3/method/
--rw-rw-rw-   0        0        0     3755 2023-04-26 19:16:04.000000 telemulator3-1.0.1/telemulator3/method/__init__.py
--rw-rw-rw-   0        0        0      824 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/answerCallbackQuery.py
--rw-rw-rw-   0        0        0      427 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/deleteMessage.py
--rw-rw-rw-   0        0        0      670 2023-04-26 19:16:04.000000 telemulator3-1.0.1/telemulator3/method/editMessageCaption.py
--rw-rw-rw-   0        0        0      606 2023-04-26 19:16:04.000000 telemulator3-1.0.1/telemulator3/method/editMessageReplyMarkup.py
--rw-rw-rw-   0        0        0      774 2023-04-26 19:16:04.000000 telemulator3-1.0.1/telemulator3/method/editMessageText.py
--rw-rw-rw-   0        0        0      775 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/forwardMessage.py
--rw-rw-rw-   0        0        0      248 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/getChat.py
--rw-rw-rw-   0        0        0      475 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/getChatAdministrators.py
--rw-rw-rw-   0        0        0      606 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/getChatMember.py
--rw-rw-rw-   0        0        0      281 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/method/getChatMemberCount.py
--rw-rw-rw-   0        0        0      552 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/method/getFile.py
--rw-rw-rw-   0        0        0      528 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/method/getMe.py
--rw-rw-rw-   0        0        0      324 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/leaveChat.py
--rw-rw-rw-   0        0        0      568 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/sendAudio.py
--rw-rw-rw-   0        0        0      463 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/sendChatAction.py
--rw-rw-rw-   0        0        0      598 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/sendDocument.py
--rw-rw-rw-   0        0        0      669 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/sendMessage.py
--rw-rw-rw-   0        0        0      607 2023-04-26 17:28:20.000000 telemulator3-1.0.1/telemulator3/method/sendPhoto.py
--rw-rw-rw-   0        0        0      378 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/method/setWebhook.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:37:36.035722 telemulator3-1.0.1/telemulator3/update/
--rw-rw-rw-   0        0        0       49 2023-04-26 12:26:19.000000 telemulator3-1.0.1/telemulator3/update/__init__.py
--rw-rw-rw-   0        0        0      699 2023-04-26 15:39:56.000000 telemulator3-1.0.1/telemulator3/update/callback_query.py
--rw-rw-rw-   0        0        0     4392 2023-04-27 10:54:49.000000 telemulator3-1.0.1/telemulator3/update/markup.py
--rw-rw-rw-   0        0        0     9378 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/update/message.py
--rw-rw-rw-   0        0        0     4353 2023-04-27 12:37:16.000000 telemulator3-1.0.1/telemulator3/user.py
-drwxrwxrwx   0        0        0        0 2023-04-28 10:37:35.934583 telemulator3-1.0.1/telemulator3.egg-info/
--rw-rw-rw-   0        0        0     3507 2023-04-28 10:37:35.000000 telemulator3-1.0.1/telemulator3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1388 2023-04-28 10:37:35.000000 telemulator3-1.0.1/telemulator3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 10:37:35.000000 telemulator3-1.0.1/telemulator3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 10:37:35.000000 telemulator3-1.0.1/telemulator3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 09:58:59.395010 telemulator3-1.1/
+-rw-rw-rw-   0        0        0     1094 2023-04-26 12:26:19.000000 telemulator3-1.1/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-04-28 10:27:40.000000 telemulator3-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3536 2023-04-29 09:58:59.395511 telemulator3-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2948 2023-04-29 09:55:18.000000 telemulator3-1.1/README.md
+-rw-rw-rw-   0        0        0      110 2023-04-26 12:26:19.000000 telemulator3-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      715 2023-04-29 09:58:59.398013 telemulator3-1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 09:58:59.278360 telemulator3-1.1/telemulator3/
+-rw-rw-rw-   0        0        0     5140 2023-04-29 09:55:18.000000 telemulator3-1.1/telemulator3/__init__.py
+-rw-rw-rw-   0        0        0     7140 2023-04-27 12:37:16.000000 telemulator3-1.1/telemulator3/api.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:58:59.316385 telemulator3-1.1/telemulator3/chat/
+-rw-rw-rw-   0        0        0      403 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/chat/__init__.py
+-rw-rw-rw-   0        0        0     3117 2023-04-27 12:37:16.000000 telemulator3-1.1/telemulator3/chat/base.py
+-rw-rw-rw-   0        0        0     2903 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/chat/channel.py
+-rw-rw-rw-   0        0        0     1890 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/chat/group.py
+-rw-rw-rw-   0        0        0     1330 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/chat/history.py
+-rw-rw-rw-   0        0        0     2551 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/chat/keyboard.py
+-rw-rw-rw-   0        0        0     3608 2023-04-27 12:37:16.000000 telemulator3-1.1/telemulator3/chat/member.py
+-rw-rw-rw-   0        0        0     1268 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/chat/private.py
+-rw-rw-rw-   0        0        0     1158 2023-04-27 12:37:16.000000 telemulator3-1.1/telemulator3/dictionaryable.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:58:59.380000 telemulator3-1.1/telemulator3/method/
+-rw-rw-rw-   0        0        0     3755 2023-04-26 19:16:04.000000 telemulator3-1.1/telemulator3/method/__init__.py
+-rw-rw-rw-   0        0        0      792 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/answerCallbackQuery.py
+-rw-rw-rw-   0        0        0      395 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/deleteMessage.py
+-rw-rw-rw-   0        0        0      638 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/editMessageCaption.py
+-rw-rw-rw-   0        0        0      574 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/editMessageReplyMarkup.py
+-rw-rw-rw-   0        0        0      742 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/editMessageText.py
+-rw-rw-rw-   0        0        0      743 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/forwardMessage.py
+-rw-rw-rw-   0        0        0      216 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/getChat.py
+-rw-rw-rw-   0        0        0      443 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/getChatAdministrators.py
+-rw-rw-rw-   0        0        0      574 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/getChatMember.py
+-rw-rw-rw-   0        0        0      249 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/getChatMemberCount.py
+-rw-rw-rw-   0        0        0      520 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/getFile.py
+-rw-rw-rw-   0        0        0      496 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/getMe.py
+-rw-rw-rw-   0        0        0      292 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/leaveChat.py
+-rw-rw-rw-   0        0        0      536 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/sendAudio.py
+-rw-rw-rw-   0        0        0      431 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/sendChatAction.py
+-rw-rw-rw-   0        0        0      566 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/sendDocument.py
+-rw-rw-rw-   0        0        0      637 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/sendMessage.py
+-rw-rw-rw-   0        0        0      575 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/sendPhoto.py
+-rw-rw-rw-   0        0        0      346 2023-04-28 13:58:13.000000 telemulator3-1.1/telemulator3/method/setWebhook.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:58:59.392509 telemulator3-1.1/telemulator3/update/
+-rw-rw-rw-   0        0        0       49 2023-04-26 12:26:19.000000 telemulator3-1.1/telemulator3/update/__init__.py
+-rw-rw-rw-   0        0        0      699 2023-04-26 15:39:56.000000 telemulator3-1.1/telemulator3/update/callback_query.py
+-rw-rw-rw-   0        0        0     4392 2023-04-27 10:54:49.000000 telemulator3-1.1/telemulator3/update/markup.py
+-rw-rw-rw-   0        0        0     9346 2023-04-29 09:55:18.000000 telemulator3-1.1/telemulator3/update/message.py
+-rw-rw-rw-   0        0        0     4353 2023-04-27 12:37:16.000000 telemulator3-1.1/telemulator3/user.py
+drwxrwxrwx   0        0        0        0 2023-04-29 09:58:59.293371 telemulator3-1.1/telemulator3.egg-info/
+-rw-rw-rw-   0        0        0     3536 2023-04-29 09:58:59.000000 telemulator3-1.1/telemulator3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1388 2023-04-29 09:58:59.000000 telemulator3-1.1/telemulator3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 09:58:59.000000 telemulator3-1.1/telemulator3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-29 09:58:59.000000 telemulator3-1.1/telemulator3.egg-info/top_level.txt
```

### Comparing `telemulator3-1.0.1/LICENSE` & `telemulator3-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/PKG-INFO` & `telemulator3-1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemulator3
-Version: 1.0.1
+Version: 1.1
 Summary: Mocked Telegram Bot API elements for unit tests of a bot based on the pyTelegramBotAPI library.
 Home-page: https://github.com/vb64/telemulator3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/telemulator3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,57 +28,72 @@
 
 ```bash
 pip install telemulator3
 ```
 
 ## Usage
 
+Create TeleBot instance and start emulate Telegram API for bot.
+
 ```python
-import unittest
 from telebot import TeleBot
-from telemulator3 import Telemulator, send_command
+from telemulator3 import Telemulator
+
+bot = TeleBot('xxx-yyy-zzz', threaded=False)
+
+@bot.message_handler(commands=['start', 'help'])
+def send_welcome(message):
+    bot.reply_to(message, "Howdy, how are you doing?")
+
+telemul = Telemulator()
+telemul.set_tested_bot(bot, username='my_bot', name='My Bot')
+```
+
+At start, there are no registered users in emulated API.
 
-class TestCase(unittest.TestCase, Telemulator):
+```python
+assert not telemul.api.users
+```
+
+Make API user, that represent our bot.
+It's a first registered user.
+
+```python
+mybot = telemul.api.get_me()
+assert mybot.is_bot
+assert mybot.username == 'my_bot'
+assert len(telemul.api.users) == 1
+```
 
-    def setUp(self):
-        """Connect your bot to test suite."""
-        super().setUp()
-        self.set_tested_bot(TeleBot('xxx-yyy-zzz', threaded=False))
-
-        # Your bot is available via api property.
-        # Your need to set bot name and username.
-        self.api.bot.username = 'my_bot'
-        self.api.bot.name = 'My Bot'
-
-    def test_api(self):
-        """Play with API calls."""
-        assert not self.api.users
-
-        # create API user for our bot
-        bot = self.api.get_me()
-        assert bot.is_bot
-        assert bot.username == 'my_bot'
-
-        # our bot is a first registered user
-        assert len(self.api.users) == 1
-
-        # new user open private chat with bot
-        user = self.api.create_user('User')
-        chat = user.private()
-        send_command(chat, '/start', user)
-        assert chat.history.contain('/start')
-
-        # user create group and add bot as member
-        group = user.create_group('My group')
-        group.add_members(user, [bot])
-        assert group.history.contain('invite new members:')
-
-        bot.leave(group)
-        assert group.history.contain('My Bot (ID 1) left chat')
-        # group.history.dump()
+New user open private chat with bot and send `/start` command.
+Bot must answer as defined and his answer must be in chat history.
+
+```python
+from telemulator3 import send_command
+
+user = telemul.api.create_user('User')
+chat = user.private()
+send_command(chat, '/start', user)
+assert chat.history.contain('Howdy, how are you doing?')
+```
+
+User create group and add bot as member.
+
+```python
+group = user.create_group('My group')
+group.add_members(user, [mybot])
+assert group.history.contain('invite new members:')
+```
+
+And so on.
+
+```python
+mybot.leave(group)
+assert group.history.contain('My Bot (ID 1) left chat')
+# group.history.dump()
 ```
 
 ## Development
 
 ```
 $ git clone git@github.com:vb64/telemulator3
 $ cd telemulator3
```

### Comparing `telemulator3-1.0.1/setup.cfg` & `telemulator3-1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 656c 656d 756c 6174 6f72 330d   = telemulator3.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e31  .version = 1.0.1
-00000030: 0d0a 6175 7468 6f72 203d 2056 6974 616c  ..author = Vital
-00000040: 7920 426f 676f 6d6f 6c6f 760d 0a61 7574  y Bogomolov..aut
-00000050: 686f 725f 656d 6169 6c20 3d20 6d61 696c  hor_email = mail
-00000060: 4076 6974 616c 792d 626f 676f 6d6f 6c6f  @vitaly-bogomolo
-00000070: 762e 7275 0d0a 6465 7363 7269 7074 696f  v.ru..descriptio
-00000080: 6e20 3d20 4d6f 636b 6564 2054 656c 6567  n = Mocked Teleg
-00000090: 7261 6d20 426f 7420 4150 4920 656c 656d  ram Bot API elem
-000000a0: 656e 7473 2066 6f72 2075 6e69 7420 7465  ents for unit te
-000000b0: 7374 7320 6f66 2061 2062 6f74 2062 6173  sts of a bot bas
-000000c0: 6564 206f 6e20 7468 6520 7079 5465 6c65  ed on the pyTele
-000000d0: 6772 616d 426f 7441 5049 206c 6962 7261  gramBotAPI libra
-000000e0: 7279 2e0d 0a6c 6f6e 675f 6465 7363 7269  ry...long_descri
-000000f0: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000100: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
-00000110: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000120: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000130: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
-00000140: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000150: 2f76 6236 342f 7465 6c65 6d75 6c61 746f  /vb64/telemulato
-00000160: 7233 0d0a 7072 6f6a 6563 745f 7572 6c73  r3..project_urls
-00000170: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-00000180: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000190: 7562 2e63 6f6d 2f76 6236 342f 7465 6c65  ub.com/vb64/tele
-000001a0: 6d75 6c61 746f 7233 2f69 7373 7565 730d  mulator3/issues.
-000001b0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-000001c0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000001d0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000001e0: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
-000001f0: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000200: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000210: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000220: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000230: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-00000240: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000250: 0d0a 7061 636b 6167 6573 203d 2074 656c  ..packages = tel
-00000260: 656d 756c 6174 6f72 330d 0a70 7974 686f  emulator3..pytho
-00000270: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000280: 2e37 0d0a 696e 636c 7564 655f 7061 636b  .7..include_pack
-00000290: 6167 655f 6461 7461 203d 2054 7275 650d  age_data = True.
-000002a0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-000002b0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000002c0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e31 0d0a  .version = 1.1..
+00000030: 6175 7468 6f72 203d 2056 6974 616c 7920  author = Vitaly 
+00000040: 426f 676f 6d6f 6c6f 760d 0a61 7574 686f  Bogomolov..autho
+00000050: 725f 656d 6169 6c20 3d20 6d61 696c 4076  r_email = mail@v
+00000060: 6974 616c 792d 626f 676f 6d6f 6c6f 762e  italy-bogomolov.
+00000070: 7275 0d0a 6465 7363 7269 7074 696f 6e20  ru..description 
+00000080: 3d20 4d6f 636b 6564 2054 656c 6567 7261  = Mocked Telegra
+00000090: 6d20 426f 7420 4150 4920 656c 656d 656e  m Bot API elemen
+000000a0: 7473 2066 6f72 2075 6e69 7420 7465 7374  ts for unit test
+000000b0: 7320 6f66 2061 2062 6f74 2062 6173 6564  s of a bot based
+000000c0: 206f 6e20 7468 6520 7079 5465 6c65 6772   on the pyTelegr
+000000d0: 616d 426f 7441 5049 206c 6962 7261 7279  amBotAPI library
+000000e0: 2e0d 0a6c 6f6e 675f 6465 7363 7269 7074  ...long_descript
+000000f0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+00000100: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000110: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000120: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000130: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000140: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
+00000150: 6236 342f 7465 6c65 6d75 6c61 746f 7233  b64/telemulator3
+00000160: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+00000170: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+00000180: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000190: 2e63 6f6d 2f76 6236 342f 7465 6c65 6d75  .com/vb64/telemu
+000001a0: 6c61 746f 7233 2f69 7373 7565 730d 0a63  lator3/issues..c
+000001b0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001e0: 3a20 330d 0a09 4c69 6365 6e73 6520 3a3a  : 3...License ::
+000001f0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000200: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
+00000210: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
+00000220: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
+00000230: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
+00000240: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
+00000250: 7061 636b 6167 6573 203d 2074 656c 656d  packages = telem
+00000260: 756c 6174 6f72 330d 0a70 7974 686f 6e5f  ulator3..python_
+00000270: 7265 7175 6972 6573 203d 203e 3d33 2e37  requires = >=3.7
+00000280: 0d0a 696e 636c 7564 655f 7061 636b 6167  ..include_packag
+00000290: 655f 6461 7461 203d 2054 7275 650d 0a0d  e_data = True...
+000002a0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000002b0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000002c0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `telemulator3-1.0.1/telemulator3/__init__.py` & `telemulator3-1.1/telemulator3/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,33 @@
 """Mocked elements of the Telegram Bot API for unit tests."""
-import os
 
 
 class EmulatorException(Exception):
     """This class represents an Exception thrown when a call to the Emulator fails."""
 
 
 class Telemulator:
     """Class for Telegram API tests."""
 
     api = None
-    teleuser = None
-    private = None
-    group = None
-    tele_message = None
-    group_message = None
-
-    def set_tested_bot(self, bot):
-        """Set bot for testing.
-
-        The bot must have follows properties and methods:
-
-        - name: bot name
-        - username: bot username
-        - token: bot API token
-        - process_new_updates([update]): method for process Telegram API update
-        """
+
+    def set_tested_bot(self, bot, username='tested_bot', name='Test Bot'):
+        """Set telebot.TeleBot instance for testing."""
         from .api import Telegram
 
-        self.clean_proxy()
+        bot.username = username
+        bot.name = name
         self.api = Telegram(bot)
 
     @property
     def bot(self):
         """Shortcut for tested bot."""
         return self.api.bot
 
     @staticmethod
-    def clean_proxy():
-        """Remove system proxy settings.
-
-        Its need for correct proccesing httpretty + requests
-        """
-        for proxy in ['https_proxy', 'http_proxy']:
-            if proxy in os.environ:
-                del os.environ[proxy]
-
-    @staticmethod
     def print_trace(is_on):
         """Switch printing calls to Telegram API."""
         from .api import debug_print
         debug_print(is_on)
 
     @staticmethod
     def create_group(title, from_user, members=None):
```

### Comparing `telemulator3-1.0.1/telemulator3/api.py` & `telemulator3-1.1/telemulator3/api.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/base.py` & `telemulator3-1.1/telemulator3/chat/base.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/channel.py` & `telemulator3-1.1/telemulator3/chat/channel.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/group.py` & `telemulator3-1.1/telemulator3/chat/group.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/history.py` & `telemulator3-1.1/telemulator3/chat/history.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/keyboard.py` & `telemulator3-1.1/telemulator3/chat/keyboard.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/member.py` & `telemulator3-1.1/telemulator3/chat/member.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/chat/private.py` & `telemulator3-1.1/telemulator3/chat/private.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/dictionaryable.py` & `telemulator3-1.1/telemulator3/dictionaryable.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/method/__init__.py` & `telemulator3-1.1/telemulator3/method/__init__.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/method/answerCallbackQuery.py` & `telemulator3-1.1/telemulator3/method/answerCallbackQuery.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=invalid-name
 """Module for answerCallbackQuery method emulator."""
 from . import get_int, get, error
 
 
 def response(api, _uri, params):
     """Notify origin user of callback query."""
     # print "#answerCallbackQuery uri", uri
```

### Comparing `telemulator3-1.0.1/telemulator3/method/editMessageCaption.py` & `telemulator3-1.1/telemulator3/method/editMessageCaption.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=invalid-name
 """Module for editMessageCaption method emulator."""
 from telebot.types import InlineKeyboardMarkup
 
 from ..update import markup
 from . import with_chat, get_int, get, get_reply_markup
```

### Comparing `telemulator3-1.0.1/telemulator3/method/editMessageReplyMarkup.py` & `telemulator3-1.1/telemulator3/method/sendMessage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# pylint: disable=invalid-name
-"""Module for editMessageReplyMarkup method emulator."""
-from ..update import markup
-from . import with_chat, get_int, get_reply_markup
+"""Module for sendMessage method emulator."""
+from ..update.message import Text
+from . import EmulatorException, message_for_chat, get
 
 
-@with_chat
-def response(_api, params, chat):
-    """Replace text and markup for given chat message."""
-    # print "#editMessageReplyMarkup.py params", params
-    message_id = get_int(params, 'message_id')
-    reply_markup = markup.from_dict(get_reply_markup(params))
+@message_for_chat
+def response(api, params, chat, reply_to_message, reply_markup):
+    """Send text to chat and return result message."""
+    # print "#sendMessage params", params
+    if 'text' not in params:
+        raise EmulatorException(402, "Wrong request no text: {}".format(params))
 
-    message = chat.history.messages.get(message_id, None)
-    if message:
-        reply_markup.attach(message)
-        return True
-
-    return False
+    return chat.send(
+      Text(
+        chat,
+        api.get_me(),
+        get(params, 'text'),
+        reply_to_message=reply_to_message
+      ),
+      reply_markup=reply_markup
+    )
```

### Comparing `telemulator3-1.0.1/telemulator3/method/editMessageText.py` & `telemulator3-1.1/telemulator3/method/editMessageText.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=invalid-name
 """Module for editMessageText method emulator."""
 from telebot.types import InlineKeyboardMarkup
 from ..update.message import Text
 from ..update import markup
 from . import with_chat, get_reply_markup, get_int, get
```

### Comparing `telemulator3-1.0.1/telemulator3/method/forwardMessage.py` & `telemulator3-1.1/telemulator3/method/forwardMessage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=invalid-name
 """Module for forwardMessage method emulator."""
 from . import get_chat, get_int, message_to_dic, EmulatorException, error
 
 
 def response(api, _uri, params):
     """Forward message from the from_chat_id to chat_id and return True."""
     # print "#forwardMessage params", params
```

### Comparing `telemulator3-1.0.1/telemulator3/method/getFile.py` & `telemulator3-1.1/telemulator3/method/getFile.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=invalid-name
 """Module for getFile method emulator."""
 
 
 def response(_api, _uri, _params):
     """Return data for passed file_id."""
     # print "#getFile uri", uri
     # print "#getFile params", _params
```

### Comparing `telemulator3-1.0.1/telemulator3/method/sendAudio.py` & `telemulator3-1.1/telemulator3/method/sendAudio.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=invalid-name
 """Module for sendAudio method emulator."""
 from ..update.message import Audio
 from . import message_for_chat, get
 
 
 @message_for_chat
 def response(api, params, chat, reply_to_message, reply_markup):
```

### Comparing `telemulator3-1.0.1/telemulator3/method/sendDocument.py` & `telemulator3-1.1/telemulator3/method/sendPhoto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# pylint: disable=invalid-name
-"""Module for sendDocument method emulator."""
-from ..update.message import Document
+"""Module for sendPhoto method emulator."""
+from ..update.message import Photo
 from . import message_for_chat, get
 
 
 @message_for_chat
 def response(api, params, chat, reply_to_message, reply_markup):
-    """Send document to chat and return result message."""
-    # print "#sendDocument params", params
+    """Send photo to chat and return result message.
+
+    How access to file upload data?
+    """
+    # print "#sendPhoto params", params
     return chat.send(
-      Document(
+      Photo(
         chat,
         api.get_me(),
-        'readme.txt',
-        500,
-        caption=get(params, 'caption'),
+        get(params, 'caption'),
+        100, 100, 500,
         reply_to_message=reply_to_message
       ),
       reply_markup=reply_markup
     )
```

### Comparing `telemulator3-1.0.1/telemulator3/method/sendMessage.py` & `telemulator3-1.1/telemulator3/method/sendDocument.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# pylint: disable=invalid-name
-"""Module for sendMessage method emulator."""
-from ..update.message import Text
-from . import EmulatorException, message_for_chat, get
+"""Module for sendDocument method emulator."""
+from ..update.message import Document
+from . import message_for_chat, get
 
 
 @message_for_chat
 def response(api, params, chat, reply_to_message, reply_markup):
-    """Send text to chat and return result message."""
-    # print "#sendMessage params", params
-    if 'text' not in params:
-        raise EmulatorException(402, "Wrong request no text: {}".format(params))
-
+    """Send document to chat and return result message."""
+    # print "#sendDocument params", params
     return chat.send(
-      Text(
+      Document(
         chat,
         api.get_me(),
-        get(params, 'text'),
+        'readme.txt',
+        500,
+        caption=get(params, 'caption'),
         reply_to_message=reply_to_message
       ),
       reply_markup=reply_markup
     )
```

### Comparing `telemulator3-1.0.1/telemulator3/update/callback_query.py` & `telemulator3-1.1/telemulator3/update/callback_query.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/update/markup.py` & `telemulator3-1.1/telemulator3/update/markup.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3/update/message.py` & `telemulator3-1.1/telemulator3/update/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Telegram types with specialized constructors and text representation."""
 from telebot.types import (
-  Message as MessageBase, MessageEntity, PhotoSize as PhotoSizeBase, Audio as AudioBase,
+  Message as MessageBase, PhotoSize as PhotoSizeBase, Audio as AudioBase,
   Document as DocumentBase, Contact as ContactBase, Voice as VoiceBase,
 )
 from ..dictionaryable import Dictionaryable
 
 
 class Message(MessageBase, Dictionaryable):
     """Base class with message_id generator."""
@@ -87,16 +87,16 @@
 
 
 class Command(Text):
     """Command message."""
 
     def __init__(self, chat, from_user, text, **kwargs):
         """Create command message."""
-        entities = MessageEntity("bot_command", 0, len(text))
-        Text.__init__(self, chat, from_user, text=text, entities=entities, **kwargs)
+        # entities = MessageEntity("bot_command", 0, len(text))
+        Text.__init__(self, chat, from_user, text=text, **kwargs)
 
 
 class PhotoSize(PhotoSizeBase, Dictionaryable):
     """Dictionaryable PhotoSize class."""
 
     attr_list = ['file_id', 'file_unique_id', 'width', 'height', 'file_size']
```

### Comparing `telemulator3-1.0.1/telemulator3/user.py` & `telemulator3-1.1/telemulator3/user.py`

 * *Files identical despite different names*

### Comparing `telemulator3-1.0.1/telemulator3.egg-info/PKG-INFO` & `telemulator3-1.1/telemulator3.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telemulator3
-Version: 1.0.1
+Version: 1.1
 Summary: Mocked Telegram Bot API elements for unit tests of a bot based on the pyTelegramBotAPI library.
 Home-page: https://github.com/vb64/telemulator3
 Author: Vitaly Bogomolov
 Author-email: mail@vitaly-bogomolov.ru
 Project-URL: Bug Tracker, https://github.com/vb64/telemulator3/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,57 +28,72 @@
 
 ```bash
 pip install telemulator3
 ```
 
 ## Usage
 
+Create TeleBot instance and start emulate Telegram API for bot.
+
 ```python
-import unittest
 from telebot import TeleBot
-from telemulator3 import Telemulator, send_command
+from telemulator3 import Telemulator
+
+bot = TeleBot('xxx-yyy-zzz', threaded=False)
+
+@bot.message_handler(commands=['start', 'help'])
+def send_welcome(message):
+    bot.reply_to(message, "Howdy, how are you doing?")
+
+telemul = Telemulator()
+telemul.set_tested_bot(bot, username='my_bot', name='My Bot')
+```
+
+At start, there are no registered users in emulated API.
 
-class TestCase(unittest.TestCase, Telemulator):
+```python
+assert not telemul.api.users
+```
+
+Make API user, that represent our bot.
+It's a first registered user.
+
+```python
+mybot = telemul.api.get_me()
+assert mybot.is_bot
+assert mybot.username == 'my_bot'
+assert len(telemul.api.users) == 1
+```
 
-    def setUp(self):
-        """Connect your bot to test suite."""
-        super().setUp()
-        self.set_tested_bot(TeleBot('xxx-yyy-zzz', threaded=False))
-
-        # Your bot is available via api property.
-        # Your need to set bot name and username.
-        self.api.bot.username = 'my_bot'
-        self.api.bot.name = 'My Bot'
-
-    def test_api(self):
-        """Play with API calls."""
-        assert not self.api.users
-
-        # create API user for our bot
-        bot = self.api.get_me()
-        assert bot.is_bot
-        assert bot.username == 'my_bot'
-
-        # our bot is a first registered user
-        assert len(self.api.users) == 1
-
-        # new user open private chat with bot
-        user = self.api.create_user('User')
-        chat = user.private()
-        send_command(chat, '/start', user)
-        assert chat.history.contain('/start')
-
-        # user create group and add bot as member
-        group = user.create_group('My group')
-        group.add_members(user, [bot])
-        assert group.history.contain('invite new members:')
-
-        bot.leave(group)
-        assert group.history.contain('My Bot (ID 1) left chat')
-        # group.history.dump()
+New user open private chat with bot and send `/start` command.
+Bot must answer as defined and his answer must be in chat history.
+
+```python
+from telemulator3 import send_command
+
+user = telemul.api.create_user('User')
+chat = user.private()
+send_command(chat, '/start', user)
+assert chat.history.contain('Howdy, how are you doing?')
+```
+
+User create group and add bot as member.
+
+```python
+group = user.create_group('My group')
+group.add_members(user, [mybot])
+assert group.history.contain('invite new members:')
+```
+
+And so on.
+
+```python
+mybot.leave(group)
+assert group.history.contain('My Bot (ID 1) left chat')
+# group.history.dump()
 ```
 
 ## Development
 
 ```
 $ git clone git@github.com:vb64/telemulator3
 $ cd telemulator3
```

### Comparing `telemulator3-1.0.1/telemulator3.egg-info/SOURCES.txt` & `telemulator3-1.1/telemulator3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

