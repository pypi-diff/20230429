# Comparing `tmp/selfcord.py-0.1.1.tar.gz` & `tmp/selfcord.py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.1.tar", last modified: Fri Apr 28 16:33:46 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.2.tar", last modified: Sat Apr 29 00:33:42 2023, max compression
```

## Comparing `selfcord.py-0.1.1.tar` & `selfcord.py-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/
--rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     2259 2023-04-24 19:11:53.000000 selfcord.py-0.1.1/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.134728 selfcord.py-0.1.1/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.1.1/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.144728 selfcord.py-0.1.1/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.1.1/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.1.1/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)     9183 2023-04-27 18:19:43.000000 selfcord.py-0.1.1/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    16788 2023-04-27 16:47:37.000000 selfcord.py-0.1.1/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7975 2023-04-27 16:53:31.000000 selfcord.py-0.1.1/selfcord/api/http.py
--rw-r--r--   0 shell     (1000) shell     (1001)    17139 2023-04-28 02:03:57.000000 selfcord.py-0.1.1/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.154729 selfcord.py-0.1.1/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.1.1/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    16434 2023-04-27 15:34:03.000000 selfcord.py-0.1.1/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1052 2023-04-27 15:34:24.000000 selfcord.py-0.1.1/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      901 2023-04-27 15:34:29.000000 selfcord.py-0.1.1/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7323 2023-04-28 16:04:21.000000 selfcord.py-0.1.1/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      933 2023-04-27 15:34:49.000000 selfcord.py-0.1.1/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1868 2023-04-27 15:35:44.000000 selfcord.py-0.1.1/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2130 2023-04-27 15:35:57.000000 selfcord.py-0.1.1/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1556 2023-04-27 15:36:19.000000 selfcord.py-0.1.1/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     3898 2023-04-27 19:15:13.000000 selfcord.py-0.1.1/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1331 2023-04-27 15:44:13.000000 selfcord.py-0.1.1/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.1.1/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    15277 2023-04-27 16:27:44.000000 selfcord.py-0.1.1/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.138062 selfcord.py-0.1.1/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      710 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1004 2023-04-28 16:33:05.000000 selfcord.py-0.1.1/setup.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/tests/
--rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.1/tests/test_commands.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.681921 selfcord.py-0.1.2/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-29 00:33:42.681921 selfcord.py-0.1.2/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)     2259 2023-04-24 19:11:53.000000 selfcord.py-0.1.2/README.md
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.665254 selfcord.py-0.1.2/selfcord/
+-rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.1.2/selfcord/__init__.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.668587 selfcord.py-0.1.2/selfcord/api/
+-rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.1.2/selfcord/api/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.1.2/selfcord/api/errors.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     9183 2023-04-27 18:19:43.000000 selfcord.py-0.1.2/selfcord/api/events.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    16788 2023-04-27 16:47:37.000000 selfcord.py-0.1.2/selfcord/api/gateway.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7975 2023-04-27 16:53:31.000000 selfcord.py-0.1.2/selfcord/api/http.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    17139 2023-04-28 02:03:57.000000 selfcord.py-0.1.2/selfcord/bot.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.678588 selfcord.py-0.1.2/selfcord/models/
+-rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.1.2/selfcord/models/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    16677 2023-04-29 00:12:51.000000 selfcord.py-0.1.2/selfcord/models/channel.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1052 2023-04-27 15:34:24.000000 selfcord.py-0.1.2/selfcord/models/client.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      901 2023-04-27 15:34:29.000000 selfcord.py-0.1.2/selfcord/models/emoji.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7323 2023-04-28 16:04:21.000000 selfcord.py-0.1.2/selfcord/models/guild.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      933 2023-04-27 15:34:49.000000 selfcord.py-0.1.2/selfcord/models/member.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2698 2023-04-29 00:23:26.000000 selfcord.py-0.1.2/selfcord/models/message.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2130 2023-04-27 15:35:57.000000 selfcord.py-0.1.2/selfcord/models/permission.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1556 2023-04-27 15:36:19.000000 selfcord.py-0.1.2/selfcord/models/role.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     3898 2023-04-27 19:15:13.000000 selfcord.py-0.1.2/selfcord/models/user.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1331 2023-04-27 15:44:13.000000 selfcord.py-0.1.2/selfcord/models/webhook.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.678588 selfcord.py-0.1.2/selfcord/utils/
+-rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.1.2/selfcord/utils/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    15588 2023-04-29 00:32:36.000000 selfcord.py-0.1.2/selfcord/utils/command.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.668587 selfcord.py-0.1.2/selfcord.py.egg-info/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)      710 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-04-29 00:33:42.000000 selfcord.py-0.1.2/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-04-29 00:33:42.681921 selfcord.py-0.1.2/setup.cfg
+-rw-r--r--   0 shell     (1000) shell     (1001)     1004 2023-04-29 00:33:34.000000 selfcord.py-0.1.2/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-29 00:33:42.678588 selfcord.py-0.1.2/tests/
+-rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.2/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.1/PKG-INFO` & `selfcord.py-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
```

### Comparing `selfcord.py-0.1.1/README.md` & `selfcord.py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/api/errors.py` & `selfcord.py-0.1.2/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/api/events.py` & `selfcord.py-0.1.2/selfcord/api/events.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/api/gateway.py` & `selfcord.py-0.1.2/selfcord/api/gateway.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/api/http.py` & `selfcord.py-0.1.2/selfcord/api/http.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/bot.py` & `selfcord.py-0.1.2/selfcord/bot.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/channel.py` & `selfcord.py-0.1.2/selfcord/models/channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,55 +91,62 @@
         """
         amount: list[int] = [i + 1 for i in range(amount)]
         for i in range(0, len(amount), 3):
             await asyncio.gather(
                 *(asyncio.create_task(self.send(tts=tts, content=content)) for amoun in amount[i:i + 3]))
             await asyncio.sleep(0.3)
 
-    async def send(self, content=None, tts=False) -> None:
+    async def send(self, content=None, tts=False) -> Message:
         """
         Send a message to the text channel.
 
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
             - tts(bool) : Specify whether message is text-to-speech or not
 
         Returns:
             No return value.
         """
         if hasattr(self, "guild_id"):
-            await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
+            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
                                     json={"content": content, "tts": tts})
+            resp.update({"guild_id": self.guild_id})
+
         else:
-            await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
+            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
                                     json={"content": content, "tts": tts})
 
-    async def reply(self, message: str, content=None, tts=False) -> None:
+        return Message(resp, self.bot, self.http)
+
+
+    async def reply(self, message: str, content=None, tts=False) -> Message:
         """Reply to a specific message
 
         Args:
             message (str): Message to reply to
             content (_type_, optional): Message content to reply with. Defaults to None.
             tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
 
         Returns:
             No return value.
         """
         if hasattr(self, "guild_id"):
-            await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
+            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
                                     json={"content": content, "tts": tts,
                                         "message_reference": {"channel_id": f"{self.id}", "message_id": f"{message.id}"},
                                         "allowed_mentions": {"parse": ["users", "roles", "everyone"],
                                                             "replied_user": False}})
+            resp.update({"guild_id": self.guild_id})
         else:
-            await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
+            resp = await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
                                     json={"content": content, "tts": tts,
                                         "message_reference": {"channel_id": f"{self.id}", "message_id": f"{message.id}"},
                                         "allowed_mentions": {"parse": ["users", "roles", "everyone"],
                                                             "replied_user": False}})
+        return Message(resp, self.bot, self.http)
 
 
 
 
 
 class TextChannel(Messageable):
     """
```

### Comparing `selfcord.py-0.1.1/selfcord/models/client.py` & `selfcord.py-0.1.2/selfcord/models/client.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/emoji.py` & `selfcord.py-0.1.2/selfcord/models/emoji.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/guild.py` & `selfcord.py-0.1.2/selfcord/models/guild.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/member.py` & `selfcord.py-0.1.2/selfcord/models/member.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/message.py` & `selfcord.py-0.1.2/selfcord/models/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -41,14 +41,27 @@
         self.guild = self.bot.get_guild(self.guild_id)
 
     async def delete(self):
         """Delete the Message Object
         """
         await self.http.request(method="delete", endpoint=f"/channels/{self.channel_id}/messages/{self.id}")
 
+    async def edit(self, content: str):
+        """Edits the specified message
+
+        Args:
+            content (str): Content to edit message to.
+        """
+        if self.guild_id != None:
+            resp = await self.http.request(method="patch", endpoint=f"/channels/{self.channel_id}/messages/{self.id}", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.channel_id}/{self.guild_id}"}, json={"content":content})
+            resp.update({"guild_id" : self.guild_id})
+        else:
+            resp = await self.http.request(method="patch", endpoint=f"/channels/{self.channel_id}/messages/{self.id}", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.channel_id}"}, json={"content":content})
+        return Message(resp, self.bot, self.http)
+
 
     async def react(self, emoji: str):
         """React to a message with an emoji
 
         Args:
             emoji (str): The emoji
         """
```

### Comparing `selfcord.py-0.1.1/selfcord/models/permission.py` & `selfcord.py-0.1.2/selfcord/models/permission.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/role.py` & `selfcord.py-0.1.2/selfcord/models/role.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/user.py` & `selfcord.py-0.1.2/selfcord/models/user.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/models/webhook.py` & `selfcord.py-0.1.2/selfcord/models/webhook.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/selfcord/utils/command.py` & `selfcord.py-0.1.2/selfcord/utils/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -483,24 +483,26 @@
     async def reply(self, content: str, tts=False):
         """Helper function to reply to your own message containing the command
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        await self.channel.reply(self.message, content, tts)
+        message = await self.channel.reply(self.message, content, tts)
+        return message
 
     async def send(self, content: str, tts=False):
         """Helper function to send message to the current channel
 
         Args:
             content (str): The message you would like to send
             tts (bool, optional): Whether message should be tts or not. Defaults to False.
         """
-        await self.channel.send( content=content, tts=tts)
+        message = await self.channel.send( content=content, tts=tts)
+        return message
 
     async def spam(self, amount: int, content: str):
         """Helper function to spam messages in the current channel (uses asyncio.gather !!!!)
 
         Args:
             amount (int): Amount of messages to spam
             content (str): The message you would like to send
@@ -511,10 +513,20 @@
         """Helper function to purge messages in the current channel, uses asyncio gather.
 
         Args:
             amount (int): The amount of messages to purge, defaults to All.
         """
         await self.channel.purge(amount)
 
+    async def edit(self, content: str):
+        """Helper function to edit the message you sent
+
+        Args:
+            content (str): Content to edit to
+        """
+        message = await self.message.edit(content)
+        return message
+
+
```

### Comparing `selfcord.py-0.1.1/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.2/selfcord.py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
```

### Comparing `selfcord.py-0.1.1/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.2/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.1/setup.py` & `selfcord.py-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models']),
-        version="0.1.1",
+        version="0.1.2",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
         install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
```

