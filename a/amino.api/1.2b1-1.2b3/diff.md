# Comparing `tmp/amino.api-1.2b1.tar.gz` & `tmp/amino.api-1.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amino.api-1.2b1.tar", last modified: Sat Apr 22 09:29:50 2023, max compression
+gzip compressed data, was "amino.api-1.2b3.tar", last modified: Fri Apr 28 15:41:06 2023, max compression
```

## Comparing `amino.api-1.2b1.tar` & `amino.api-1.2b3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-22 09:29:50.819896 amino.api-1.2b1/
--rw-rw-rw-   0        0        0      606 2023-04-22 09:29:50.820896 amino.api-1.2b1/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-04-21 23:53:10.000000 amino.api-1.2b1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-22 09:29:50.812897 amino.api-1.2b1/amino/
--rw-rw-rw-   0        0        0      855 2023-04-21 21:48:51.000000 amino.api-1.2b1/amino/__init__.py
--rw-rw-rw-   0        0        0    19822 2023-04-22 00:21:50.000000 amino.api-1.2b1/amino/client.py
--rw-rw-rw-   0        0        0    14991 2023-04-22 00:21:32.000000 amino.api-1.2b1/amino/full_client.py
--rw-rw-rw-   0        0        0     8429 2023-04-22 00:21:28.000000 amino.api-1.2b1/amino/local_client.py
--rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b1/amino/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:29:50.819896 amino.api-1.2b1/amino/utils/
--rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b1/amino/utils/__init__.py
--rw-rw-rw-   0        0        0      980 2023-04-21 21:48:51.000000 amino.api-1.2b1/amino/utils/exceptions.py
--rw-rw-rw-   0        0        0     7421 2023-04-22 00:13:53.000000 amino.api-1.2b1/amino/utils/helpers.py
--rw-rw-rw-   0        0        0    10795 2023-04-21 21:48:51.000000 amino.api-1.2b1/amino/utils/objects.py
--rw-rw-rw-   0        0        0     2267 2023-04-22 00:18:06.000000 amino.api-1.2b1/amino/utils/requester.py
-drwxrwxrwx   0        0        0        0 2023-04-22 09:29:50.815896 amino.api-1.2b1/amino.api.egg-info/
--rw-rw-rw-   0        0        0      606 2023-04-22 09:29:50.000000 amino.api-1.2b1/amino.api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-04-22 09:29:50.000000 amino.api-1.2b1/amino.api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-22 09:29:50.000000 amino.api-1.2b1/amino.api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-22 09:29:50.000000 amino.api-1.2b1/amino.api.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-22 09:29:50.000000 amino.api-1.2b1/amino.api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-22 09:29:50.820896 amino.api-1.2b1/setup.cfg
--rw-rw-rw-   0        0        0     1603 2023-04-21 23:54:10.000000 amino.api-1.2b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:41:06.126717 amino.api-1.2b3/
+-rw-rw-rw-   0        0        0      773 2023-04-28 15:41:06.126717 amino.api-1.2b3/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-04-22 10:17:55.000000 amino.api-1.2b3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 15:41:06.081745 amino.api-1.2b3/amino/
+-rw-rw-rw-   0        0        0      883 2023-04-28 13:51:48.000000 amino.api-1.2b3/amino/__init__.py
+-rw-rw-rw-   0        0        0    36475 2023-04-28 13:47:41.000000 amino.api-1.2b3/amino/client.py
+-rw-rw-rw-   0        0        0    18007 2023-04-28 15:34:22.000000 amino.api-1.2b3/amino/full_client.py
+-rw-rw-rw-   0        0        0    10964 2023-04-28 15:34:50.000000 amino.api-1.2b3/amino/local_client.py
+-rw-rw-rw-   0        0        0    11535 2023-04-21 23:43:16.000000 amino.api-1.2b3/amino/socket.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:41:06.125717 amino.api-1.2b3/amino/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-21 21:48:51.000000 amino.api-1.2b3/amino/utils/__init__.py
+-rw-rw-rw-   0        0        0     1099 2023-04-28 13:22:02.000000 amino.api-1.2b3/amino/utils/exceptions.py
+-rw-rw-rw-   0        0        0     7429 2023-04-22 10:56:39.000000 amino.api-1.2b3/amino/utils/helpers.py
+-rw-rw-rw-   0        0        0    11896 2023-04-28 15:15:41.000000 amino.api-1.2b3/amino/utils/objects.py
+-rw-rw-rw-   0        0        0     2270 2023-04-22 10:51:46.000000 amino.api-1.2b3/amino/utils/requester.py
+-rw-rw-rw-   0        0        0     3660 2023-04-26 13:04:41.000000 amino.api-1.2b3/amino/utils/snippetTools.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:41:06.101739 amino.api-1.2b3/amino.api.egg-info/
+-rw-rw-rw-   0        0        0      773 2023-04-28 15:41:04.000000 amino.api-1.2b3/amino.api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2023-04-28 15:41:04.000000 amino.api-1.2b3/amino.api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:41:04.000000 amino.api-1.2b3/amino.api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-28 15:41:04.000000 amino.api-1.2b3/amino.api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-28 15:41:04.000000 amino.api-1.2b3/amino.api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:41:06.127726 amino.api-1.2b3/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2023-04-28 13:50:16.000000 amino.api-1.2b3/setup.py
```

### Comparing `amino.api-1.2b1/amino/__init__.py` & `amino.api-1.2b3/amino/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 Author: Xsarz
+Сo-author: imperialwool
 
 Enjoy using!
 """
 
 
 
 from .utils import helpers, exceptions, objects, requester
@@ -19,15 +20,15 @@
 from json import loads
 from requests import get
 
 __title__ = 'amino.api'
 __author__ = 'Xsarz'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Xsarz'
-__version__ = '1.1'
+__version__ = '1.2b3'
 __newest__ = loads(get("https://pypi.org/pypi/amino.api/json").text)["info"]["version"]
 
 
 
 if __version__ != __newest__:
 	s('cls || clear')
 	print(f'\033[38;5;214m{__title__} made by {__author__}\nPlease update the library. Your version: {__version__}  A new version:{__newest__}\033[0m')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `amino.api-1.2b1/amino/client.py` & `amino.api-1.2b3/amino/full_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from .socket import SocketHandler, Callbacks
 
 from time import time as timestamp
 from json import loads, dumps
 from requests import Session
 from typing import Union, BinaryIO
 from base64 import b64encode
-from json_minify import json_minify
 from uuid import uuid4
 from io import BytesIO
 
-class Client(SocketHandler, Callbacks):
+class FullClient(SocketHandler, Callbacks):
 	def __init__(self, socket_enabled: bool = True, socket_debug: bool = False, socket_trace: bool = False,  auto_device: bool = False, deviceId: str = None, proxies: dict = None, certificatePath = None):
 		self.session = Session()
 		self.profile = objects.profile()
 		self.req = Requester(session=self.session, deviceId=deviceId, auto_device=auto_device, proxies=proxies, verify=certificatePath)
 		self.socket_enabled = socket_enabled
 
 		SocketHandler.__init__(self, self.req, socket_trace, socket_debug)
@@ -31,14 +30,23 @@
 
 	def set_device_id(self, deviceId: str):
 		self.req._set(2, deviceId)
 
 	def set_sid(self, sid: str):
 		self.req._set(1, sid)
 
+	def upload_media(self, file: BinaryIO, fileType: str):
+
+		if fileType == "audio":fileType = "audio/aac"
+		elif fileType == "image":fileType = "image/jpg" 
+		else: raise exceptions.IncorrectType(fileType)
+		data = file.read()
+
+		response = self.req.make_request(method="POST", endpoint="/g/s/media/upload", body=data, type=fileType)
+		return loads(response.text)["mediaValue"]
 
 
 	def login(self, email: str, password: str = None, secret: str = None):
 		data = dumps({
 			"email": email,
 			"v": 2,
 			"secret": secret if secret else f"0 {password}",
@@ -72,21 +80,14 @@
 		json = loads(response.text)
 		self.profile = objects.profile(json)
 		self.req._set(1, self.profile.sid)
 		if self.socket_enabled:self.connect()
 		return self.profile
 
 
-	def login_sid(self, sid: str):
-		self.profile = objects.profile({"sid": sid, "auid": self.req.gen.sid_to_uid(sid)})
-		self.req._set(1, self.profile.sid)		
-		if self.socket_enabled:self.connect()
-		return self.profile
-
-
 
 	def logout(self):
 
 		data = dumps({
 		"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID"),
 		"clientType": 100,
 		"timestamp": int(timestamp() * 1000)
@@ -153,26 +154,33 @@
 
 
 	def leave_community(self, comId: Union[int, str]):
 
 		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/community/leave")
 		return response.status_code
 
-	def join_chat(self, chatId: str):
+	def join_chat(self, chatId: str, comId: Union[int, str] = None):
+		if comId:
+			response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/chat/thread/{chatId}/member/{self.profile.userId}", type="application/x-www-form-urlencoded")
+			return response.status_code		
 
 		response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/member/{self.profile.userId}", type="application/x-www-form-urlencoded")
 		return response.status_code
 
-	def leave_chat(self, chatId: str):
+	def leave_chat(self, chatId: str, comId: Union[int, str] = None):
+		if comId:
+			response = self.req.make_request(method="DELETE", endpoint=f"{self.api}/x{comId}/s/chat/thread/{chatId}/member/{self.profile.userId}")
+			return response.status_code		
 
 		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/chat/thread/{chatId}/member/{self.profile.userId}")
 		return response.status_code
 
 
-	def send_message(self, chatId: str, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
+
+	def send_message(self, chatId: str, comId: Union[int, str] = None, message: str = None, messageType: int = 0, file: BinaryIO = None, fileType: str = None, replyTo: str = None, mentionUserIds: list = None, stickerId: str = None, embedId: str = None, embedType: int = None, embedLink: str = None, embedTitle: str = None, embedContent: str = None, embedImage: BinaryIO = None):
 
 		if message and file is None:
 			message = message.replace("<@", "‎‏").replace("@>", "‬‭")
 		mentions = list()
 		if mentionUserIds:
 			for uid in mentionUserIds:
 				mentions.append({"uid": uid})
@@ -218,69 +226,37 @@
 				data["mediaUhqEnabled"] = True
 
 			else: raise exceptions.IncorrectType(f"fileType: {fileType}")
 
 			data["mediaUploadValue"] = b64encode(file.read()).decode()
 
 
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/message", body=dumps(data))
-		return response.status_code
-
-	def send_video(self, chatId: str, message: str = None, videoFile: BytesIO = None, imageFile: BytesIO = None, mediaUhqEnabled: bool = False):
-		
-		filename = str(uuid4()).upper()
-		сover, video = f"{filename}_thumb.jpg", f"{filename}.mp4"
-		
-		data = {
-			"clientRefId": int(timestamp() / 10 % 1000000000),
-			"content": message,
-			"mediaType": 123,
-			"videoUpload":
-			{
-				"contentType": "video/mp4",
-				"cover": сover,
-				"video": video
-			},
-			"type": 4,
-			"timestamp": int(timestamp() * 1000),
-			"mediaUhqEnabled": mediaUhqEnabled,
-			"extensions": {}	
-		}
-		
-		files = {
-			video: (video, videoFile.read(), 'video/mp4'),
-			сover: (сover, imageFile.read(), 'application/octet-stream'),
-			'payload': (None, data, 'application/octet-stream')
-		}
-		
 		response = self.req.make_request(
-			method="POST",
-			endpoint=f"/g/s/chat/thread/{chatId}/message",
-			payload=dumps(data),
-			files=files
-		)
-		
+				method="POST",
+				endpoint=f"/x{comId}/s/chat/thread/{chatId}/message" if comId else f"/g/s/chat/thread/{chatId}/message",
+				body=dumps(data)
+			)
 		return response.status_code
 
-	def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
+
+	def delete_message(self, chatId: str, messageId: str, comId: Union[int, str] = None, asStaff: bool = False, reason: str = None):
 
 		if asStaff:
 			data = dumps({
 				"adminOpName": 102,
 				"adminOpNote": {"content": reason},
 				"timestamp": int(timestamp() * 1000)
 			})
 
-			response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/message/{messageId}/admin", body=data)
+			response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/chat/thread/{chatId}/message/{messageId}/admin" if comId else f"/g/s/chat/thread/{chatId}/message/{messageId}/admin", body=data)
 			return response.status_code			
 
-		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/chat/thread/{chatId}/message/{messageId}")
+		response = self.req.make_request(method="DELETE", endpoint=f"/x{comId}/s/chat/thread/{chatId}/message/{messageId}" if comId else f"/g/s/chat/thread/{chatId}/message/{messageId}")
 		return response.status_code
 
-
 	def get_public_communities(self, language: str = "en", size: int = 25):
 
 		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&size={size}&pagingType=t")
 		return objects.communityList(loads(response.text))
 
 	def get_all_users(self, start: int = 0, size: int = 25):
 
@@ -299,295 +275,221 @@
 
 
 	def watch_ad(self, userId: str = None):
 		data = dumps(self.req.gen.tapjoy_data(userId if userId else self.profile.userId))
 		response = self.req.session.request("POST", "https://ads.tapdaq.com/v4/analytics/reward", proxies=self.req.proxies, verify=self.req.verify, data=data, headers=self.req.gen.tapjoy_headers)
 		return exceptions.check_exceptions(response.text) if response.status_code != 204 else response.status_code
 
-
-	def send_active_obj(self, comId: str, tz: int = None, timers: list = None):
-		#TODO
-		data = json_minify(dumps({"userActiveTimeChunkList": timers if timers else self.req.gen.timers(), "timestamp": int(timestamp() * 1000), "optInAdsFlags": 2147483647, "timezone": tz if tz else self.req.gen.timezone()}))
-		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/community/stats/user-active-time", body=data)
-		return response.status_code
-
-
-	def request_verify_code(self, email: str, resetPassword: bool = False):
-
-		data = {
-			"identity": email,
-			"type": 1,
-			"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID")
-		}
-
-		if resetPassword:
-			data["level"] = 2
-			data["purpose"] = "reset-password"
-
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/auth/request-security-validation", body=dumps(data))
-		return response.status_code
-
-
-	def register(self, nickname: str, email: str, password: str, verificationCode: str, deviceId: str = None):
+	def send_video(self, chatId: str, comId: Union[str,int] = None, message: str = None, videoFile: BytesIO = None, imageFile: BytesIO = None, mediaUhqEnabled: bool = False):
+		
+		filename = str(uuid4()).upper()
+		сover, video = f"{filename}_thumb.jpg", f"{filename}.mp4"
 
 		data = dumps({
-			"secret": f"0 {password}",
-			"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID"),
-			"email": email,
-			"clientType": 100,
-			"nickname": nickname,
-			"latitude": 0,
-			"longitude": 0,
-			"address": None,
-			"clientCallbackURL": "narviiapp://relogin",
-			"validationContext": {
-				"data": {
-					"code": verificationCode
-				},
-				"type": 1,
-				"identity": email
+			"clientRefId": int(timestamp() / 10 % 1000000000),
+			"content": message,
+			"mediaType": 123,
+			"videoUpload":
+			{
+				"contentType": "video/mp4",
+				"cover": сover,
+				"video": video
 			},
-			"type": 1,
-			"identity": email,
-			"timestamp": int(timestamp() * 1000)
-		})
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/auth/register", body=data)
-		return loads(response.text)
-
-
-
-	def verify_account(self, email: str, code: str):
-
-		data = dumps({
-			"validationContext": {
-				"type": 1,
-				"identity": email,
-				"data": {"code": code}},
-			"deviceID": self.device_id,
-			"timestamp": int(timestamp() * 1000)
-		})
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/auth/check-security-validation", body=data)
-		return response.status_code
-
-
-	def delete_account(self, password: str):
-
-		data = dumps({
-			"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID"),
-			"secret": f"0 {password}"
-		})
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/account/delete-request", body=data)
-		return response.status_code
-
-
-
-
-	def restore_account(self, email: str, password: str):
-
-		data = dumps({
-			"secret": f"0 {password}",
-			"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID"),
-			"email": email,
-			"timestamp": int(timestamp() * 1000)
-		})
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/account/delete-request/cancel", body=data)
-		return response.status_code
-
-
-	def activate_account(self, email: str, code: str):
-
-		data = dumps({
-			"type": 1,
-			"identity": email,
-			"data": {"code": code},
-			"deviceID": self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID")
-		})
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/auth/activate-email", body=data)
-		return response.status_code
-
-
-	def configure_gender(self, age: int, gender: str):
-
-		if gender.lower() == "male": gender = 1
-		elif gender.lower() == "female": gender = 2
-		elif gender.lower() == "non-binary": gender = 255
-		else: raise exceptions.IncorrectType(gender)
-		if age <= 12: raise exceptions.AgeTooLow(age)
-
-		data = dumps({
-			"age": age,
-			"gender": gender,
-			"timestamp": int(timestamp() * 1000)
+			"type": 4,
+			"timestamp": int(timestamp() * 1000),
+			"mediaUhqEnabled": mediaUhqEnabled,
+			"extensions": {}	
 		})
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/persona/profile/basic", body=data)
+		
+		files = {
+			video: (video, videoFile.read(), 'video/mp4'),
+			сover: (сover, imageFile.read(), 'application/octet-stream'),
+			'payload': (None, data, 'application/octet-stream')
+		}
+		
+		nId = f"x{comId}" or "g"
+		response = self.req.make_request(method="POST", endpoint=f"/{nId}/s/chat/thread/{chatId}/message", payload=data, files=files)
 		return response.status_code
+		
+	def post_poll(self, comId: Union[str, int], title: str, content: str, pollVariants: list, duration: int = 7, backgroundColor: str = None, imageForPollOptions: str = None) -> int:
 
-
-	def change_password(self, email: str, password: str, code: str):
-		deviceId = self.req.gen.get_headers(deviceId=self.req.deviceId).get("NDCDEVICEID")
-
-		data = dumps({
-			"updateSecret": f"0 {password}",
-			"emailValidationContext": {
-				"data": {
-					"code": code
+		data = {
+			"taggedBlogCategoryIdList": [],
+			"content": content,
+			"mediaList": None,
+			"keywords": None,
+			"eventSource": "GlobalComposeMenu",
+			"title": title,
+			"timestamp": int(timestamp() * 1000),
+			"type": 4,
+			"durationInDays": duration,
+			"polloptList": [],
+			"extensions": {
+				"featuredType": 0,
+				"style": {
+					"coverMediaIndexList": None
 				},
-				"type": 1,
-				"identity": email,
-				"level": 2,
-				"deviceID": deviceId
-			},
-			"phoneNumberValidationContext": None,
-			"deviceID": deviceId
-		})
-
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/auth/reset-password", body=data)
+				"fansOnly": False,
+				"pageSnippet": None,
+				"quizPlayedTimes": 0,
+				"__disabledLevel__": 0,
+				"headlineStyle": None,
+				"privilegeOfCommentOnPost": 0,
+				"promotedTo": None,
+				"quizTotalQuestionCount": 0,
+				"promoteInfo": None,
+				"promotedFrom": None,
+				"pollSettings": {
+					"polloptType": 0,
+					"joinEnabled": False
+				},
+				"quizInBestQuizzes": False
+			}
+		}
+		
+		if len(pollVariants) < 2: raise Exception("2 poll options or bigger")
+		for pollVariant in pollVariants:
+			pollOpt = {
+				"status": 0,
+				"mediaList": [
+					[
+						100,
+						imageForPollOptions,
+						None,
+						None,
+						None,
+						None
+					]
+				],
+				"votedValue": 0,
+				"globalVotedValue": 0,
+				"parentType": 0,
+				"title": str(pollVariant),
+				"globalVotesCount": 0,
+				"type": 0,
+				"votesCount": 0,
+				"refObjectType": 0,
+				"votesSum": 0
+			}
+			if imageForPollOptions == None: pollOpt.pop("mediaList")
+			data['polloptList'].append(pollOpt)
+		
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/blog", body=dumps(data))
 		return response.status_code
 
 
-	def get_eventlog(self, language: str = "en"):
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/eventlog/profile?language={language.lower()}")
-		return loads(response.text)
-
-
-	def get_my_communities(self, start: int = 0, size: int = 25):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/community/joined?v=1&start={start}&size={size}")
-		return objects.communityList(loads(response.text)["communityList"])
-
-
-	def get_profile_in_communities(self, start: int = 0, size: int = 25):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/community/joined?v=1&start={start}&size={size}")
-		return loads(response.text)["userInfoInCommunities"]
-
-
-	def get_user_info(self, userId: str):
-
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/user-profile/{userId}")
-		return objects.UserProfile(loads(response.text)["userProfile"])
-
-
-	def get_chat_threads(self, start: int = 0, size: int = 25):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread?type=joined-me&start={start}&size={size}")
-		return objects.ThreadList(loads(response.text)["threadList"])
-
-
-	def get_chat_thread(self, chatId: str):
+	def post_blog(self, comId: Union[str, int], title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False):
+		mediaList = []
 
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread/{chatId}")
-		return objects.ThreadList(loads(response.text)["thread"])
+		if captionList is not None:
+			for image, caption in zip(imageList, captionList):
+				mediaList.append([100, self.upload_media(image, "image"), caption])
 
-
-	def get_chat_members(self, chatId: str, start: int = 0, size: int = 25, type: str = "default"):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread/{chatId}/member?start={start}&size={size}&type={type}&cv=1.2")
-		return objects.userProfileList(loads(response.text)["memberList"])
-
-
-
-	def start_chat(self, userId: Union[str, list], message: str, title: str = None, content: str = None, isGlobal: bool = False, publishToGlobal: bool = False):
-
-		if isinstance(userId, str): userIds = [userId]
-		elif isinstance(userId, list): userIds = userId
-		else: raise exceptions.IncorrectType(type(userId))
+		else:
+			if imageList is not None:
+				for image in imageList:
+					print(self.upload_media(image, "image"))
+					mediaList.append([100, self.upload_media(image, "image"), None])
 
 		data = {
-			"title": title,
-			"inviteeUids": userIds,
-			"initialMessageContent": message,
+			"address": None,
 			"content": content,
+			"title": title,
+			"mediaList": mediaList,
+			"extensions": extensions,
+			"latitude": 0,
+			"longitude": 0,
+			"eventSource": "GlobalComposeMenu",
 			"timestamp": int(timestamp() * 1000)
 		}
 
-		if isGlobal: data["type"] = 2; data["eventSource"] = "GlobalComposeMenu"
-		else: data["type"] = 0
-
-		if publishToGlobal: data["publishToGlobal"] = 1
-		else: data["publishToGlobal"] = 0
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread", body=dumps(data))
-		return objects.Thread(loads(response.text)["thread"])
+		if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+		if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+		if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/blog", body=dumps(data))
+		return response.status_code
 
 
-	def invite_to_chat(self, userId: Union[str, list], chatId: str):
+	def post_wiki(self, comId: Union[str, int], title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False):
+		mediaList = []
 
-		if isinstance(userId, str): userIds = [userId]
-		elif isinstance(userId, list): userIds = userId
-		else: raise exceptions.IncorrectType(type(userId))
+		for image in imageList:
+			mediaList.append([100, self.upload_media(image, "image"), None])
 
-		data = dumps({
-			"uids": userIds,
+		data = {
+			"label": title,
+			"content": content,
+			"mediaList": mediaList,
+			"eventSource": "GlobalComposeMenu",
 			"timestamp": int(timestamp() * 1000)
-		})
-
-		response = self.req.make_request(method="POST", endpoint=f"/g/s/chat/thread/{chatId}/member/invite", body=data)
-		return response.status_code
-
-
-
-	def kick(self, userId: str, chatId: str, allowRejoin: bool = True):
+		}
 
-		response = self.req.make_request(method="DELETE", endpoint=f"/g/s/chat/thread/{chatId}/member/{userId}?allowRejoin={1 if allowRejoin else 0}")
+		if icon: data["icon"] = icon
+		if keywords: data["keywords"] = keywords
+		if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
+		if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
+		
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/item", body=dumps(data))
 		return response.status_code
+	
 
-
-	def get_chat_messages(self, chatId: str, size: int = 25, pageToken: str = None):
-
-		response = self.req.make_request(method="GET",
-			endpoint=f"/g/s/chat/thread/{chatId}/message?v=2&pagingType=t&size={size}{f'&pageToken={pageToken}' if pageToken else ''}")
-		return objects.MessageList(loads(response.text))
-
-
-	def get_message_info(self, chatId: str, messageId: str):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/chat/thread/{chatId}/message/{messageId}")
-		return objects.Message(loads(response.text)["message"])
-
-
-	def get_community_info(self, comId: str):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s-x{comId}/community/info?withInfluencerList=1&withTopicList=true&influencerListOrderStrategy=fansCount")
-		return objects.CommunityInfo(loads(response.text)["community"])
-
-
-	def search_community(self, aminoId: str):
-		#TODO
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/search/amino-id-and-link?q={aminoId}")
-		return response.text
-
-
-	def get_user_following(self, userId: str, start: int = 0, size: int = 25):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/user-profile/{userId}/joined?start={start}&size={size}")
-		return objects.userProfileList(loads(response.text))
-
-
-	def get_user_followers(self, userId: str, start: int = 0, size: int = 25):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/user-profile/{userId}/member?start={start}&size={size}")
-		return objects.userProfileList(loads(response.text))
-
-
-
-	def get_user_visitors(self, userId: str, start: int = 0, size: int = 25):
-		#TODO
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/user-profile/{userId}/visitors?start={start}&size={size}")
-		return loads(response.text)
-
-
-	def get_blocked_users(self, start: int = 0, size: int = 25):
-
-		response = self.req.make_request(method="GET", endpoint=f"/g/s/block?start={start}&size={size}")
-		return objects.userProfileList(loads(response.text))
+	def get_wiki_folders(self, comId: Union[str, int], folderId: str = None):
+		fId = f"/{folderId}/item-previews" if folderId else ""
+		
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item-category{fId}")
+		return self.objects.WikiFoldes(response.json())
+	
+
+	def get_all_approved_wikis(self, comId: Union[str, int], size: int = 10):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item?type=catalog-all&pagingType=t&size={size}")
+		return response.json()
+
+
+	def get_community_stickers(self, comId: Union[str, int], size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/store/items?size={size}&sectionGroupId=sticker&storeGroupId=community-shared&pagingType=t")
+		return response.json()
+	
+
+	def get_community_stickerpack(self, comId: Union[str, int], stickerId: str):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/sticker-collection/{stickerId}?includeStickers=1")
+		return response.json()
+	
+
+	def get_pending_wikis(self, comId: Union[str, int], size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/knowledge-base-request?pagingType=t&size={size}&type=pending")
+		return response.json()
+	
+
+	def reject_wiki(self, comId: Union[str, int], requestId: str):
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/knowledge-base-request/{requestId}/reject", body=dumps({ "timestamp": int(timestamp() * 1000) }))
+		return response.status_code
+	
+
+	def approve_wiki(self, comId: Union[str, int], requestId: str, method: str = "replace"):
+		base = { "timestamp": int(timestamp() * 1000) }
+		if method in ['create', 'new']:
+			base.update({"actionType": "create", "destinationCategoryIdList": []})
+		elif method in ['replace', 'update']:
+			base.update({"actionType": "replace"})
+		else: raise Exception("invalid value of method")
+
+		response = self.req.make_request(method="POST",endpoint=f"/x{comId}/s/knowledge-base-request/{requestId}/approve", body=dumps({ "timestamp": int(timestamp() * 1000) }))
+		return response.status_code
+
+	def get_flags(self, comId: Union[str, int], size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/flag?size={size}&status=pending&type=all&pagingType=t")
+		return response.json()
+	
+
+	def view_wiki(self, comId: Union[str, int], wikiId: str):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item/{wikiId}")
+		return response.json()
+	
+
+	def get_hall_of_fame(self, size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?size={size}&categoryKey=customized&type=discover&pagingType=t&moduleId=23ce695c-c4da-4da5-a6c4-7777ba23b7aa")
+		return response.json()
+	
+	def get_recommended_communities(self, size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/g/s/topic/0/feed/community?size={size}&categoryKey=recommendation&type=discover&pagingType=t")
+		return response.json()
```

### Comparing `amino.api-1.2b1/amino/local_client.py` & `amino.api-1.2b3/amino/local_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -83,40 +83,40 @@
 		return response.status_code
 
 	def send_video(self, chatId: str, message: str = None, videoFile: BytesIO = None, imageFile: BytesIO = None, mediaUhqEnabled: bool = False):
 		
 		filename = str(uuid4()).upper()
 		сover, video = f"{filename}_thumb.jpg", f"{filename}.mp4"
 		
-		data = {
+		data = dumps({
 			"clientRefId": int(timestamp() / 10 % 1000000000),
 			"content": message,
 			"mediaType": 123,
 			"videoUpload":
 			{
 				"contentType": "video/mp4",
 				"cover": сover,
 				"video": video
 			},
 			"type": 4,
 			"timestamp": int(timestamp() * 1000),
 			"mediaUhqEnabled": mediaUhqEnabled,
 			"extensions": {}	
-		}
+		})
 		
 		files = {
 			video: (video, videoFile.read(), 'video/mp4'),
 			сover: (сover, imageFile.read(), 'application/octet-stream'),
 			'payload': (None, data, 'application/octet-stream')
 		}
 		
 		response = self.req.make_request(
 			method="POST",
 			endpoint=f"/x{self.comId}/s/chat/thread/{chatId}/message",
-			payload=dumps(data),
+			payload=data,
 			files=files
 		)
 		
 		return response.status_code
 
 	def delete_message(self, chatId: str, messageId: str, asStaff: bool = False, reason: str = None):
 
@@ -129,15 +129,17 @@
 
 			response = self.req.make_request(method="POST", endpoint=f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}/admin", body=data)
 			return response.status_code			
 
 		response = self.req.make_request(method="DELETE", endpoint=f"/x{self.comId}/s/chat/thread/{chatId}/message/{messageId}")
 		return response.status_code
 		
-	def post_poll(self, title: str, content: str, pollVariants: list, duration: int = 7, backgroundColor: str = None, imageForPollOptions: str = None) -> int:
+		
+	def post_poll(self, comId: Union[str, int], title: str, content: str, pollVariants: list, duration: int = 7, backgroundColor: str = None, imageForPollOptions: str = None) -> int:
+
 		data = {
 			"taggedBlogCategoryIdList": [],
 			"content": content,
 			"mediaList": None,
 			"keywords": None,
 			"eventSource": "GlobalComposeMenu",
 			"title": title,
@@ -190,24 +192,20 @@
 				"type": 0,
 				"votesCount": 0,
 				"refObjectType": 0,
 				"votesSum": 0
 			}
 			if imageForPollOptions == None: pollOpt.pop("mediaList")
 			data['polloptList'].append(pollOpt)
-
-		response = self.req.make_request(
-			method="POST",
-			endpoint=f"/x{self.comId}/s/blog",
-			body=dumps(data)
-		)
 		
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/blog", body=dumps(data))
 		return response.status_code
-		
-	def post_blog(self, title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False):
+
+
+	def post_blog(self, comId: Union[str, int], title: str, content: str, imageList: list = None, captionList: list = None, categoriesList: list = None, backgroundColor: str = None, fansOnly: bool = False, extensions: dict = None, crash: bool = False):
 		mediaList = []
 
 		if captionList is not None:
 			for image, caption in zip(imageList, captionList):
 				mediaList.append([100, self.upload_media(image, "image"), caption])
 
 		else:
@@ -228,23 +226,19 @@
 			"timestamp": int(timestamp() * 1000)
 		}
 
 		if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
 		if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
 		if categoriesList: data["taggedBlogCategoryIdList"] = categoriesList
 
-		response = self.req.make_request(
-			method="POST",
-			endpoint=f"/x{self.comId}/s/blog",
-			body=dumps(data)
-		)
-		
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/blog", body=dumps(data))
 		return response.status_code
 
-	def post_wiki(self, title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False):
+
+	def post_wiki(self, comId: Union[str, int], title: str, content: str, icon: str = None, imageList: list = None, keywords: str = None, backgroundColor: str = None, fansOnly: bool = False):
 		mediaList = []
 
 		for image in imageList:
 			mediaList.append([100, self.upload_media(image, "image"), None])
 
 		data = {
 			"label": title,
@@ -255,14 +249,62 @@
 		}
 
 		if icon: data["icon"] = icon
 		if keywords: data["keywords"] = keywords
 		if fansOnly: data["extensions"] = {"fansOnly": fansOnly}
 		if backgroundColor: data["extensions"] = {"style": {"backgroundColor": backgroundColor}}
 		
-		response = self.req.make_request(
-			method="POST",
-			endpoint=f"/x{self.comId}/s/item",
-			body=dumps(data)
-		)
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/item", body=dumps(data))
+		return response.status_code
+	
+
+	def get_wiki_folders(self, comId: Union[str, int], folderId: str = None):
+		fId = f"/{folderId}/item-previews" if folderId else ""
 		
-		return response.status_code
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item-category{fId}")
+		return self.objects.WikiFoldes(response.json())
+	
+
+	def get_all_approved_wikis(self, comId: Union[str, int], size: int = 10):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item?type=catalog-all&pagingType=t&size={size}")
+		return response.json()
+
+
+	def get_community_stickers(self, comId: Union[str, int], size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/store/items?size={size}&sectionGroupId=sticker&storeGroupId=community-shared&pagingType=t")
+		return response.json()
+	
+
+	def get_community_stickerpack(self, comId: Union[str, int], stickerId: str):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/sticker-collection/{stickerId}?includeStickers=1")
+		return response.json()
+	
+
+	def get_pending_wikis(self, comId: Union[str, int], size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/knowledge-base-request?pagingType=t&size={size}&type=pending")
+		return response.json()
+	
+
+	def reject_wiki(self, comId: Union[str, int], requestId: str):
+		response = self.req.make_request(method="POST", endpoint=f"/x{comId}/s/knowledge-base-request/{requestId}/reject", body=dumps({ "timestamp": int(timestamp() * 1000) }))
+		return response.status_code
+	
+
+	def approve_wiki(self, comId: Union[str, int], requestId: str, method: str = "replace"):
+		base = { "timestamp": int(timestamp() * 1000) }
+		if method in ['create', 'new']:
+			base.update({"actionType": "create", "destinationCategoryIdList": []})
+		elif method in ['replace', 'update']:
+			base.update({"actionType": "replace"})
+		else: raise Exception("invalid value of method")
+
+		response = self.req.make_request(method="POST",endpoint=f"/x{comId}/s/knowledge-base-request/{requestId}/approve", body=dumps({ "timestamp": int(timestamp() * 1000) }))
+		return response.status_code
+
+	def get_flags(self, comId: Union[str, int], size: int = 25):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/flag?size={size}&status=pending&type=all&pagingType=t")
+		return response.json()
+	
+
+	def view_wiki(self, comId: Union[str, int], wikiId: str):
+		response = self.req.make_request(method="GET", endpoint=f"/x{comId}/s/item/{wikiId}")
+		return response.json()
```

### Comparing `amino.api-1.2b1/amino/socket.py` & `amino.api-1.2b3/amino/socket.py`

 * *Files identical despite different names*

### Comparing `amino.api-1.2b1/amino/utils/exceptions.py` & `amino.api-1.2b3/amino/utils/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 	def __init__(*args, **kwargs):
 		Exception.__init__(*args, **kwargs)
 
 class AgeTooLow(Exception):
 	def __init__(*args, **kwargs):
 		Exception.__init__(*args, **kwargs)
 
+
+class UnsupportedLanguage(Exception):
+	def __init__(*args, **kwargs):
+		Exception.__init__(*args, **kwargs)
+
+
+
 errors = {
 }
 
 def check_exceptions(data):
 	try:
 		data = loads(data)
 		try:code = data["api:statuscode"]
```

### Comparing `amino.api-1.2b1/amino/utils/helpers.py` & `amino.api-1.2b3/amino/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 			"Connection": "Upgrade"
 		}
 		if data:
 			headers["Content-Length"] = str(len(data))
 			headers["NDC-MSG-SIG"] = self.signature(data=data)
 		if sid:          headers["NDCAUTH"] = f"sid={sid}"
 		if content_type: headers["Content-Type"] = content_type
-		if type == "==PAYLOAD==": headers.pop("Content-Type")
+		if content_type == "==PAYLOAD==": headers.pop("Content-Type")
 		
 		return headers
 
 	def get_ws_headers(self, final: str, sid: str = None, deviceId: str = None):
 		return {
 				"NDCDEVICEID": self.generate_deviceId() if self.auto_device else deviceId if deviceId else self.get_device().get("deviceId"),
 				"NDCAUTH": f"sid={sid}",
```

### Comparing `amino.api-1.2b1/amino/utils/objects.py` & `amino.api-1.2b3/amino/utils/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,19 +73,20 @@
 		self.blogsCount = self.json.get("blogsCount")
 
 
 class linkInfo:
 	def __init__(self, data: dict = {}):
 		self.json = data
 		linkInfo = self.json.get("extensions", {}).get("linkInfo", {})
+		self.community = CommunityInfo(self.json.get("extensions", {}).get("community"))
 
 		self.path = self.json.get("path")
 		self.objectId = linkInfo.get("objectId")
 		self.targetCode = linkInfo.get("targetCode")
-		self.comId = linkInfo.get("ndcId")
+		self.comId = linkInfo.get("ndcId") if linkInfo.get("ndcId") else self.community.comId
 		self.fullPath = linkInfo.get("fullPath")
 		self.shortCode = linkInfo.get("shortCode")
 		self.objectType = linkInfo.get("objectType")
 
 
 class Event:
 	def __init__(self, data: dict = {}):
@@ -268,8 +269,35 @@
 		self.json = data
 		paging = self.json.get("paging", {})
 		
 		self.messages = list()
 		self.nextPageToken = paging.get("nextPageToken")
 		self.prevPageToken = paging.get("prevPageToken")
 		for message in self.json.get("messageList", []):
-			self.messages.append(Message(message))
+			self.messages.append(Message(message))
+
+
+
+class WikiFoldes:
+	def __init__(self, data: dict = []):
+		self.json = data
+		self.folders = list
+		self.allFolders = self.Folder(self.json.get("allEntriesItemCategory"))
+		for folder in self.json.get("itemCategoryList"):
+			self.folders.append(self.Folder(folder))
+
+
+	class Folder:
+		def __init__(self, data: dict = []):
+			self.json = data
+			self.itemsCount = self.json.get("itemsCount")
+			self.parentCategoryId = self.json.get("parentCategoryId")
+			self.categoryId = self.json.get("categoryId")
+			self.content = self.json.get("itemsCount")
+			self.itemsCount = self.json.get("content")
+			self.extensions = self.json.get("extensions")
+			self.createdTime = self.json.get("createdTime")
+			self.subcategoriesCount = self.json.get("subcategoriesCount")
+			self.label = self.json.get("label")
+			self.mediaList = self.json.get("mediaList")
+			self.icon = self.json.get("icon")
+			self.author = UserProfile(self.json.get("author"))
```

### Comparing `amino.api-1.2b1/amino/utils/requester.py` & `amino.api-1.2b3/amino/utils/requester.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .helpers import Generator
 from .exceptions import InvalidFunctionСall, InvalidSessionType
 from .exceptions import check_exceptions
 
 class Requester:
 	def __init__(self, session: Union[ClientSession, Session], deviceId: str = None, auto_device: bool = False, proxies: dict = None, verify = None):
-		self.api = "https://service.narvii.com/api/v1"
+		self.api = "https://service.aminoapps.com/api/v1"
 		self.sid = None
 		self.deviceId = deviceId
 		self.gen = Generator(auto_device)
 		self.session = session
 		self.proxies = proxies
 		self.verify = verify
```

### Comparing `amino.api-1.2b1/setup.py` & `amino.api-1.2b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 info = {
 	"name": "amino.api",
-	"version": "1.2b1",
+	"version": "1.2b3",
 	"github_page": "https://github.com/xXxCLOTIxXx/amino.api",
 	"download_link": "https://github.com/xXxCLOTIxXx/amino.api/archive/refs/heads/main.zip",
 	"license": "MIT",
 	"author": "Xsarz",
 	"author_email": "xsarzy@gmail.com",
 	"description": "Library for creating amino bots and scripts.",
 	"long_description": None,
```

