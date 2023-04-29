# Comparing `tmp/daisy_llm-0.0.4.tar.gz` & `tmp/daisy_llm-0.0.5.tar.gz`

## Comparing `daisy_llm-0.0.4.tar` & `daisy_llm-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/main.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/.vscode/launch.json
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/examples/configs.yaml
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/examples/main.py
--rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/Chat.py
--rw-r--r--   0        0        0    14804 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/ChatSpeechProcessor.py
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/ConnectionStatus.py
--rw-r--r--   0        0        0    10237 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/ContextHandlers.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/LoadTts.py
--rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/ModuleLoader.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/SoundManager.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/Text.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/__init__.py
--rw-r--r--   0        0        0   323462 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/sounds/alert.wav
--rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/sounds/beep.wav
--rw-r--r--   0        0        0    63654 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/sounds/end.wav
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/sounds/google_tts_test.mp3
--rw-r--r--   0        0        0  2078036 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/src/daisy_llm/sounds/waiting.wav
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/tests/pytests.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/LICENSE
--rw-r--r--   0        0        0     3265 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/README.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 daisy_llm-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/main.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/publish.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/.vscode/launch.json
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/examples/configs.yaml
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/examples/main.py
+-rw-r--r--   0        0        0    12533 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/Chat.py
+-rw-r--r--   0        0        0    14667 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/ChatSpeechProcessor.py
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/ConnectionStatus.py
+-rw-r--r--   0        0        0    14926 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/ContextHandlers.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/LoadTts.py
+-rw-r--r--   0        0        0    10335 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/ModuleLoader.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/SoundManager.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/Text.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/__init__.py
+-rw-r--r--   0        0        0   323462 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/sounds/alert.wav
+-rw-r--r--   0        0        0    11968 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/sounds/beep.wav
+-rw-r--r--   0        0        0    63654 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/sounds/end.wav
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/sounds/google_tts_test.mp3
+-rw-r--r--   0        0        0  2078036 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/src/daisy_llm/sounds/waiting.wav
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/tests/pytests.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 daisy_llm-0.0.5/PKG-INFO
```

### Comparing `daisy_llm-0.0.4/examples/configs.yaml` & `daisy_llm-0.0.5/examples/configs.yaml`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/Chat.py` & `daisy_llm-0.0.5/src/daisy_llm/Chat.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/ChatSpeechProcessor.py` & `daisy_llm-0.0.5/src/daisy_llm/ChatSpeechProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,18 +187,16 @@
 				return
 			time.sleep(0.5) #Wait juuuust a bit to prevent sentence overlap
 				
 
 
 
 	def play_tts_queue(self, arguments_dict):
-		play_tts_queue = arguments_dict['play_tts_queue']
 		tts_queue = arguments_dict['tts_queue']
 		sentence_queue_canceled = arguments_dict.get('sentence_queue_canceled', [False])
-		sentence_queue_complete = arguments_dict.get('sentence_queue_complete', [False])
 		tts_queue_complete = arguments_dict['tts_queue_complete']
 		stop_event = arguments_dict['stop_event']
 		sound_stop_event = arguments_dict['sound_stop_event']
 		
 		tts = []
 
 		# Wait for tts to be generated
```

### Comparing `daisy_llm-0.0.4/src/daisy_llm/ConnectionStatus.py` & `daisy_llm-0.0.5/src/daisy_llm/ConnectionStatus.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/ContextHandlers.py` & `daisy_llm-0.0.5/src/daisy_llm/ContextHandlers.py`

 * *Files 21% similar despite different names*

```diff
@@ -64,109 +64,42 @@
 
 
 		self.db_path = db_path
 		self.messages = []
 		self.start_prompts = []
 		self.connection_pool = ConnectionPool(db_path)
 
-		self.load_context()
-
-	def update_conversation_name_summary(self):
-		# Get the name of the current conversation from the LLM
-		time.sleep(1)
-		logging.info("Updating conversation name and summary...")
-		messages = self.get_context_without_timestamp()
-		prompt = """
-		Please respond with a name, and summary for this conversation.
-		1. The name should be a single word or short phrase, no more than 5 words."
-		2. The summary should be a short description of the conversation, no more than 2 SHORT sentences.
-		3. The output must follow the following JSON format: {"name": name, "summary": summary}
-		"""
-		messages.append(self.single_message_context('system', prompt, False))
-
-		print_text("Conversation info ("+str(self.conversation_id)+"): ", "yellow")
-		response = self.chat.request(
-			messages=messages, 
-			silent=False, 
-			response_label=False
-			)
-
-		# Extract the JSON response from the string
-		response_match = re.search(r"{.*}", response)
-		if response_match:
-			response_json = response_match.group(0)
-		else:
-			logging.error("Invalid response format while setting conversation name and summary")
-			return
-
-		# Convert the JSON response to an object
-		try:
-			response_obj = json.loads(response_json)
-		except Exception as e:
-			logging.error("Invalid JSON response while setting conversation name and summary: " + str(e))
-			return
-
-		# Update the name and summary of the current conversation in the database
-		with self.connection_pool.get_connection() as conn:
-			cursor = conn.cursor()
-			cursor.execute(
-				'''UPDATE conversations SET name = ?, summary = ? WHERE id = ?''',
-				(response_obj["name"], response_obj["summary"], self.conversation_id)
-			)
-			conn.commit()
-
-		logging.info("Name and summary updated: " + response_obj["name"])
-
-		return
-
 
 	def load_context(self):
 		self.messages = []
 		self.create_conversations_table_if_not_exists()
 		with self.connection_pool.get_connection() as conn:
 
 			cursor = conn.cursor()
 
-			# Get the conversation ID
-			if not self.conversation_id:
-				cursor.execute('''
-				SELECT id FROM conversations ORDER BY id DESC LIMIT 1;
-				''')
-				row = cursor.fetchone()
-				if row:
-					self.conversation_id = str(row[0])
-					logging.info("No conversation id found in configs.yaml, loading latest conversation: " + str(self.conversation_id))
-
-			# If conversation still is not set, create a new conversation ID
+			# If conversation_id is not set, create a new conversation ID
 			if not self.conversation_id:
 				self.conversation_id = str(int(time.time()))
-				logging.info("No conversation found, creating new conversation: " + str(self.conversation_id))
 
-				# Set the new conversation ID in configs.yaml
-				with open("configs.yaml", "r") as f:
-					configs = yaml.load(f)
-				configs['conversation_id'] = self.conversation_id
-				with open("configs.yaml", "w") as f:
-					yaml.dump(configs, f)
+				print_text("Creating new conversation: ", "yellow")
+				print_text(str(self.conversation_id), None, "\n")
 
 			logging.info("Conversation id: " + str(self.conversation_id))
 
 			# Get the messages from the conversation ID
 			cursor.execute('''
 				SELECT * FROM messages WHERE id = ?
 			''', (self.conversation_id,))
 			rows = cursor.fetchall()
 			if rows:
 				for row in rows:
 					message = json.loads(row[1])
 					self.messages.append(message)
 				print_text("Loaded "+ str(len(rows)) + " messages from conversation id: " + str(self.conversation_id), "yellow", "\n")
 
-
-
 	def create_conversations_table_if_not_exists(self):
 		with self.connection_pool.get_connection() as conn:
 			cursor = conn.cursor()
 			cursor.execute('''
 				CREATE TABLE IF NOT EXISTS messages (
 					id TEXT NOT NULL,
 					message TEXT NOT NULL
@@ -194,15 +127,15 @@
 			rows = conn.execute('''
 				SELECT COUNT(*) FROM conversations WHERE id = ?;
 			''', (self.conversation_id,)).fetchone()[0]
 			if rows == 0:
 				conn.execute('''
 					INSERT INTO conversations (id, name, summary)
 					VALUES (?, ?, ?);
-				''', (self.conversation_id, "generic name", "generic summary"))
+				''', (self.conversation_id, "No name", "No summary"))
 
 			# Save messages
 			conn.execute('''
 				DELETE FROM messages WHERE id = ?;
 			''', (self.conversation_id,))
 			for message in self.messages:
 				json_message = json.dumps(message)
@@ -213,57 +146,55 @@
 				COMMIT;
 			''')
 			row_count = conn.execute('''
 				SELECT COUNT(*) FROM messages WHERE id = ?;
 			''', (self.conversation_id,)).fetchone()[0]
 			logging.info(f"Inserted {row_count} rows for conversation {self.conversation_id}.")
 
-
 	def get_context(self):
 		context = []
 		#Append start prompts to messages
 		for start_prompt in self.start_prompts:
 			context.append(start_prompt)
 
 		for message in self.messages:
 			context.append(message)
 		return context
 
-
 	def get_context_without_timestamp(self):
 		messages_without_timestamp = []
 
 		for message in self.get_context():
 			message_without_timestamp = message.copy()
 			del message_without_timestamp['timestamp']
 			messages_without_timestamp.append(message_without_timestamp)
 		return messages_without_timestamp
-	
-	def get_conversation_name_summary(self):
+
+	def get_conversation_name_summary(self, limit=None):
 		with self.connection_pool.get_connection() as conn:
 			cursor = conn.cursor()
-			cursor.execute(
-				'''SELECT name, summary FROM conversations'''
-			)
+			query = '''SELECT id, name, summary FROM conversations ORDER BY id DESC'''
+			if limit:
+				query += f' LIMIT {limit}'
+			cursor.execute(query)
 			rows = cursor.fetchall()
 			if rows:
-				return [(name, summary) for name, summary in rows]
+				return [(id, name, summary) for id, name, summary in rows]
 			else:
 				return None
 
-
 	def single_message_context(self, role, message, incl_timestamp=True):
 		if incl_timestamp:
 			now = datetime.datetime.now()
 			timestamp = now.strftime("%Y-%m-%d %H:%M:%S")
 			return {'role': role, 'timestamp': timestamp, 'content': str(message)}
 		else:
 			return {'role': role, 'content': str(message)}
-		
-	def add_start_propmpt(self, role="system", message=""):
+
+	def add_start_prompt(self, role="system", message=""):
 		start_prompt = self.single_message_context(role, message)
 		self.start_prompts.append(start_prompt)
 
 	def add_message_object(self, role, message):
 		logging.debug("Adding " + role + " message to context")
 		now = datetime.datetime.now()
 		timestamp = now.strftime("%Y-%m-%d %H:%M:%S")
@@ -325,7 +256,214 @@
 				self.messages[index]['content'] = message
 				now = datetime.datetime.now()
 				self.messages[index]['timestamp'] = now.strftime('%Y-%m-%d %H:%M:%S')
 				self.save_context()
 		except ValueError:
 			pass
 		return False
+
+	def update_conversation_name_summary(self, conversation_id=None, update_all=False):
+		conversation_ids = []
+
+		if conversation_id:
+			conversation_ids.append(conversation_id)
+		elif update_all:
+			conversation_ids = self.get_conversation_ids()
+		else:
+			conversation_ids.append(self.conversation_id)
+			# Get conversations with missing name or summary
+			conversations = self.get_conversation_name_summary(limit=None)
+			for conv_id, name, summary in conversations:
+				if name == "No name" or summary == "No summary":
+					if conv_id not in conversation_ids:
+						conversation_ids.append(conv_id)
+
+		for conv_id in conversation_ids:
+			messages = self.get_conversation_context_by_id(conv_id, include_timestamp=False)
+			#If there are no messages in the context, delete it
+			
+			if not messages:
+				self.delete_conversation_by_id(conv_id)
+
+			# Get the name of the current conversation from the LLM
+			time.sleep(1)
+			logging.info("Updating conversation name and summary for: " + conv_id)
+
+			while True:
+				prompt = """
+				Please respond with a name, and summary for this conversation.
+				1. The name should be a single word or short phrase, no more than 5 words."
+				2. The summary should be a fairly verbose summary of the conversation, as short as possible while still containing all of the important topics, names, places, and sentiment of conversation.
+				3. The output must follow the following JSON format: {"name": name, "summary": summary}
+				4. If the conversation is empty, please respond with "Empty"
+				"""
+				if messages:
+					messages.append(self.single_message_context('system', prompt, False))
+
+					print_text("Conversation info (" + str(conv_id) + "): ", "yellow")
+					response = self.chat.request(
+						messages=messages,
+						silent=False,
+						response_label=False
+					)
+				else:
+					response = '{"name": "Empty Conversation", "summary": "None"}'
+
+
+				# Extract the JSON response from the string
+				response_match = re.search(r"{.*}", response)
+				if response_match:
+					response_json = response_match.group(0)
+					break
+				else:
+					logging.error("Invalid response format while setting conversation name and summary. Trying again...")
+
+			# Convert the JSON response to an object
+			try:
+				response_obj = json.loads(response_json)
+			except Exception as e:
+				logging.error("Invalid JSON response while setting conversation name and summary: " + str(e))
+				return
+
+			# Update the name and summary of the current conversation in the database
+			with self.connection_pool.get_connection() as conn:
+				cursor = conn.cursor()
+				cursor.execute(
+					'''UPDATE conversations SET name = ?, summary = ? WHERE id = ?''',
+					(response_obj["name"], response_obj["summary"], conv_id)
+				)
+				conn.commit()
+
+			logging.info("Name and summary updated for conversation " + conv_id + ": " + response_obj["name"])
+
+	def get_conversation_ids(self):
+		with self.connection_pool.get_connection() as conn:
+			cursor = conn.cursor()
+			cursor.execute('''SELECT id FROM conversations;''')
+			rows = cursor.fetchall()
+			return [row[0] for row in rows]
+
+	def new_conversation(self):
+		# Generate a new conversation ID
+		conversation_id = str(int(time.time()))
+		logging.info("Creating a new conversation: " + conversation_id)
+
+		# Set the new conversation ID in configs.yaml
+		with open("configs.yaml", "r") as f:
+			configs = yaml.load(f)
+		configs['conversation_id'] = conversation_id
+		with open("configs.yaml", "w") as f:
+			yaml.dump(configs, f)
+
+		# Update the conversation ID and load the context
+		self.conversation_id = conversation_id
+		self.load_context()
+
+	def get_conversation_name_by_id(self, conversation_id):
+		with self.connection_pool.get_connection() as conn:
+			cursor = conn.cursor()
+			cursor.execute(
+				'''SELECT name FROM conversations WHERE id = ?''',
+				(conversation_id,)
+			)
+			row = cursor.fetchone()
+			if row:
+				return row[0]
+			else:
+				return None
+			
+	def get_conversation_context_by_id(self, conversation_id, include_timestamp=True):
+		# Check if the conversation ID exists in the database
+		with self.connection_pool.get_connection() as conn:
+			cursor = conn.cursor()
+			cursor.execute('''
+				SELECT id FROM conversations WHERE id = ?;
+			''', (conversation_id,))
+			row = cursor.fetchone()
+
+		if row:
+			# Get the messages from the specified conversation ID
+			with self.connection_pool.get_connection() as conn:
+				cursor = conn.cursor()
+				cursor.execute('''
+					SELECT message FROM messages WHERE id = ?;
+				''', (conversation_id,))
+				rows = cursor.fetchall()
+
+			context = []
+			if rows:
+				for row in rows:
+					message = json.loads(row[0])
+					if not include_timestamp:
+						message.pop('timestamp', None)
+					context.append(message)
+
+			return context
+		else:
+			return None
+
+	def set_conversation_by_id(self, conversation_id):
+		if str(conversation_id).isdigit():
+			conversation_id = int(conversation_id)
+		else:
+			return False
+			
+		logging.info("Setting conversation ID: " + str(conversation_id))
+		
+		# Check if the conversation ID exists in the database
+		with self.connection_pool.get_connection() as conn:
+			cursor = conn.cursor()
+			cursor.execute('''
+				SELECT id FROM conversations WHERE id = ?;
+			''', (conversation_id,))
+			row = cursor.fetchone()
+		
+		if row:
+			# Set the conversation ID in configs.yaml
+			with open("configs.yaml", "r") as f:
+				configs = yaml.load(f)
+			configs['conversation_id'] = conversation_id
+			with open("configs.yaml", "w") as f:
+				yaml.dump(configs, f)
+			
+			# Update the conversation ID and load the context
+			self.conversation_id = conversation_id
+			self.load_context()
+			return True
+		else:
+			return False
+		
+	def delete_conversation_by_id(self, conversation_id):
+		logging.info("Deleting conversation ID: " + conversation_id)
+		
+		# Check if the conversation ID exists in the database
+		with self.connection_pool.get_connection() as conn:
+			cursor = conn.cursor()
+			cursor.execute('''
+				SELECT id FROM conversations WHERE id = ?;
+			''', (conversation_id,))
+			row = cursor.fetchone()
+		
+		if row:
+			# Delete the conversation from the database
+			with self.connection_pool.get_connection() as conn:
+				cursor = conn.cursor()
+				cursor.execute('''
+					DELETE FROM conversations WHERE id = ?;
+					DELETE FROM messages WHERE id = ?;
+				''', (conversation_id, conversation_id,))
+				conn.commit()
+			
+			# Clear the conversation ID in configs.yaml if it matches the deleted conversation
+			with open("configs.yaml", "r") as f:
+				configs = yaml.load(f)
+			if configs.get('conversation_id') == conversation_id:
+				configs['conversation_id'] = None
+				with open("configs.yaml", "w") as f:
+					yaml.dump(configs, f)
+			
+			# Reset the conversation ID and reload the context
+			self.conversation_id = None
+			self.load_context()
+			return True
+		else:
+			return False
```

### Comparing `daisy_llm-0.0.4/src/daisy_llm/LoadTts.py` & `daisy_llm-0.0.5/src/daisy_llm/LoadTts.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/ModuleLoader.py` & `daisy_llm-0.0.5/src/daisy_llm/ModuleLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 			ModuleLoader.initialized = True
 
 			self.start_prompts = []
 			self.hook_instances = {}
 			self.loaded = False
 
 			self.stop_event = threading.Event()
-			self.thread = threading.Thread(target=self.update_modules_loop)
+			self.thread = threading.Thread(target=self.update_configs_loop)
 
 			# Load modules
 			self.available_modules = []
 
 
 			# Load enabled modules from config file
 			with open(self.configs_yaml, 'r') as f:
@@ -203,32 +203,32 @@
 
 					if hasattr(instance, 'close') and callable(getattr(instance, 'close')):
 						instance.close()
 
 		#Replace existing object with the new one
 		self.hook_instances = updated_hook_instances
 
-	def update_modules_loop(self):
+	def update_configs_loop(self):
 		last_modified_time = 0
 		while True:
 			current_modified_time = os.path.getmtime("configs.yaml")
 			if current_modified_time > last_modified_time:
 				self.loaded = False
 				self.get_available_modules()
 
 				last_modified_time = current_modified_time
 
 			time.sleep(1)
 
-	def start_update_modules_loop_thread(self):
-		self.update_modules_loop_thread = threading.Thread(target=self.update_modules_loop)
-		self.update_modules_loop_thread.start()
+	def start_update_configs_loop_thread(self):
+		self.update_configs_loop_thread = threading.Thread(target=self.update_configs_loop)
+		self.update_configs_loop_thread.start()
 
-	def stop_update_modules_loop_thread(self):
-		self.update_modules_loop_thread.stop()
+	def stop_update_configs_loop_thread(self):
+		self.update_configs_loop_thread.stop()
 
 	def enable_module(self, module_name):
 		logging.info("Enabling module: " + module_name)
 		with open(self.configs_yaml, 'r') as f:
 			config = yaml.load(f)
 
 		if module_name not in config['enabled_modules']:
```

### Comparing `daisy_llm-0.0.4/src/daisy_llm/SoundManager.py` & `daisy_llm-0.0.5/src/daisy_llm/SoundManager.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/Text.py` & `daisy_llm-0.0.5/src/daisy_llm/Text.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/__init__.py` & `daisy_llm-0.0.5/src/daisy_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/sounds/alert.wav` & `daisy_llm-0.0.5/src/daisy_llm/sounds/alert.wav`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/sounds/beep.wav` & `daisy_llm-0.0.5/src/daisy_llm/sounds/beep.wav`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/sounds/end.wav` & `daisy_llm-0.0.5/src/daisy_llm/sounds/end.wav`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/sounds/google_tts_test.mp3` & `daisy_llm-0.0.5/src/daisy_llm/sounds/google_tts_test.mp3`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/src/daisy_llm/sounds/waiting.wav` & `daisy_llm-0.0.5/src/daisy_llm/sounds/waiting.wav`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/tests/pytests.py` & `daisy_llm-0.0.5/tests/pytests.py`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/LICENSE` & `daisy_llm-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `daisy_llm-0.0.4/README.md` & `daisy_llm-0.0.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 ### 🏁 Getting Started
 Install package
 ```
 pip install daisy_llm
 ```
 
+Import into your project and use. See main-example.py
+
 
 Create ```config.py``` in your project with necessary information and enable desired modules to be loaded. See [Daisy-openai-chat](https://github.com/myrakrusemark/Daisy-openAI-chat) for sample project and a collection of modules to get started
 
 ### 🧰 Capabilities
 Daisy accepts different types of user-developed "modules". A voice assistant module comes with [Daisy-openai-chat](https://github.com/myrakrusemark/Daisy-openAI-chat) as a "proof-of-concept". Possible configurations and apps built using Daisy could include:
   - Web apps
   - Conversational processing APIs
```

### Comparing `daisy_llm-0.0.4/pyproject.toml` & `daisy_llm-0.0.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "daisy_llm"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Myra Krusemark", email = "daisy_llm@myrakrusemark.com" }
 ]
-description = "A toolkit for working and conversing with large language models."
+description = "A toolkit for working and conversing with large language models. Featuring tokenized sentence queueing for TTS."
 readme = "README.md"
 requires-python = ">=3.11.1"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
```

### Comparing `daisy_llm-0.0.4/PKG-INFO` & `daisy_llm-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: daisy_llm
-Version: 0.0.4
-Summary: A toolkit for working and conversing with large language models.
+Version: 0.0.5
+Summary: A toolkit for working and conversing with large language models. Featuring tokenized sentence queueing for TTS.
 Project-URL: Homepage, https://github.com/myrakrusemark/daisy_llm
 Project-URL: Bug Tracker, https://github.com/myrakrusemark/daisy_llm/issues
 Author-email: Myra Krusemark <daisy_llm@myrakrusemark.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -49,14 +49,16 @@
 
 ### 🏁 Getting Started
 Install package
 ```
 pip install daisy_llm
 ```
 
+Import into your project and use. See main-example.py
+
 
 Create ```config.py``` in your project with necessary information and enable desired modules to be loaded. See [Daisy-openai-chat](https://github.com/myrakrusemark/Daisy-openAI-chat) for sample project and a collection of modules to get started
 
 ### 🧰 Capabilities
 Daisy accepts different types of user-developed "modules". A voice assistant module comes with [Daisy-openai-chat](https://github.com/myrakrusemark/Daisy-openAI-chat) as a "proof-of-concept". Possible configurations and apps built using Daisy could include:
   - Web apps
   - Conversational processing APIs
```

