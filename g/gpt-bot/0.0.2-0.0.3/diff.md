# Comparing `tmp/gpt_bot-0.0.2-py3-none-any.whl.zip` & `tmp/gpt_bot-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4676 bytes, number of entries: 7
+Zip file size: 5995 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 05:12 gpt_bot/__init__.py
--rw-r--r--  2.0 unx     4849 b- defN 23-Apr-25 05:12 gpt_bot/__main__.py
+-rw-r--r--  2.0 unx     6599 b- defN 23-Apr-29 15:16 gpt_bot/__main__.py
 -rw-r--r--  2.0 unx     2318 b- defN 23-Apr-22 13:21 gpt_bot/record.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      520 b- defN 23-Apr-25 05:38 gpt_bot-0.0.2.dist-info/RECORD
-7 files, 8866 bytes uncompressed, 3756 bytes compressed:  57.6%
+-rw-r--r--  2.0 unx     2153 b- defN 23-Apr-29 15:16 gpt_bot/speak.py
+-rw-r--r--  2.0 unx     1059 b- defN 23-Apr-29 15:23 gpt_bot-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 15:23 gpt_bot-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 15:23 gpt_bot-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 23-Apr-29 15:23 gpt_bot-0.0.3.dist-info/RECORD
+8 files, 12822 bytes uncompressed, 4967 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: gpt_bot/__main__.py
 Comment: 
 
 Filename: gpt_bot/record.py
 Comment: 
 
-Filename: gpt_bot-0.0.2.dist-info/METADATA
+Filename: gpt_bot/speak.py
 Comment: 
 
-Filename: gpt_bot-0.0.2.dist-info/WHEEL
+Filename: gpt_bot-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: gpt_bot-0.0.2.dist-info/top_level.txt
+Filename: gpt_bot-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: gpt_bot-0.0.2.dist-info/RECORD
+Filename: gpt_bot-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: gpt_bot-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gpt_bot/__main__.py

```diff
@@ -1,26 +1,26 @@
 import asyncio
-import fire
 import openai
 import os
 import prompt_toolkit
 import tiktoken
 
+# Some static configuration
+MODEL = "gpt-3.5-turbo"  # Choose the ID of the model to use
+PROMPT = "You are ChatGPT, a large language model trained by OpenAI. Answer as concisely as possible."
+MAX_TOKENS = 4096
+
 # Authenticate with OpenAI API
 assert "OPENAI_API_KEY" in os.environ, "OPENAI_API_KEY environment variable not set."
 openai.api_key = os.environ["OPENAI_API_KEY"]
 if "OPENAI_PROXY" in os.environ:
     openai.proxy = os.environ["OPENAI_PROXY"]
 
-MODEL = "gpt-3.5-turbo"  # Choose the ID of the model to use
-PROMPT = "You are ChatGPT, a large language model trained by OpenAI. Answer as concisely as possible."
-MAX_TOKENS = 4096
 
-
-def num_tokens_from_messages(messages, model=MODEL):
+def num_tokens_from_messages(messages, model):
     encoding = tiktoken.encoding_for_model(model)
     if model == MODEL:  # note: future models may deviate from this
         num_tokens = 0
         for message in messages:
             num_tokens += 4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
             for key, value in message.items():
                 num_tokens += len(encoding.encode(value))
@@ -63,70 +63,151 @@
             yield obj['delta']['content']
 
 
 def prompt_continuation(width, line_number, is_soft_wrap):
     return '.' * (width - 1) + ' '
 
 
-async def driver(model, prompt):
-    print(f"Welcome to the chatbot({model})! PROMPT is")
-    print(prompt)
-    print()
-
-    multiline = False
-    chat_history = []
-    session = prompt_toolkit.PromptSession(history=prompt_toolkit.history.FileHistory(os.path.expanduser("~/.gpt_history")))
-    while True:
-        user_input = await session.prompt_async(
-            "You: ",
-            multiline=multiline,
-            prompt_continuation=prompt_continuation,
-        )
-        if user_input.startswith("/multiline"):
-            multiline = not multiline
-            print(f"{multiline=}")
-            continue
-        if user_input.startswith("/prompt"):
-            prompt = user_input[7:]
-            print("Update prompt to: ", prompt)
-            continue
-        if user_input.startswith("/rollback"):
-            chat_history = chat_history[:-2]
-            print("Rollback the history")
-            continue
-        if user_input.startswith("/history"):
-            print(chat_history)
-            continue
-        if user_input.startswith("/edit"):
-            last_chat = chat_history[-1]
-            user_edit = await session.prompt_async(
-                "Bot: ",
-                multiline=multiline,
-                prompt_continuation=prompt_continuation,
-                default=last_chat,
-            )
-            chat_history[-1] = user_edit
-            continue
-        if user_input.startswith("/record"):
-            from .record import record_and_transcribe
-            user_input = await record_and_transcribe()
-            print("You:", user_input)
-        if user_input.startswith("/quit"):
-            break
-
-        chat_history.append(user_input)
-        print("Bot: ", end="", flush=True)
-        bot_response = ""
-        # Get response from OpenAI's GPT-3 model
-        async for message in completion(chat_history, model, prompt):
-            print(message, end="", flush=True)
-            bot_response += message
+class App:
+
+    def __init__(self, model=MODEL, prompt=PROMPT, history="~/.gpt_history"):
+        self.model = model
+        self.prompt = prompt
+
+        self.middleware = {}
+
+        self.multiline = False
+        self.chat_history = []
+        self.session = prompt_toolkit.PromptSession(history=prompt_toolkit.history.FileHistory(os.path.expanduser(history)))
+        self.speak = False
+
+    async def driver(self):
+        print(f"Welcome to the chatbot({self.model})! PROMPT is")
+        print(self.prompt)
         print()
-        chat_history.append(bot_response)
 
+        while True:
+            user_input = await self.session.prompt_async(
+                "You: ",
+                multiline=self.multiline,
+                prompt_continuation=prompt_continuation,
+            )
 
-def main(model=MODEL, prompt=PROMPT):
-    asyncio.run(driver(model, prompt))
+            do_quit = False
+            do_continue = False
+            for prefix, function in self.middleware.items():
+                if user_input.startswith(prefix):
+                    try:
+                        line = user_input[len(prefix):]
+                        if asyncio.iscoroutinefunction(function):
+                            user_input = await function(self, line)
+                        else:
+                            user_input = function(self, line)
+                        break
+                    except self.Exit:
+                        do_quit = True
+                        break
+                    except self.Continue:
+                        do_continue = True
+                        break
+            if do_quit:
+                break
+            if do_continue:
+                continue
+
+            self.chat_history.append(user_input)
+            print("Bot: ", end="", flush=True)
+            bot_response = ""
+            # Get response from OpenAI's GPT-3 model
+            async for message in completion(self.chat_history, self.model, self.prompt):
+                print(message, end="", flush=True)
+                bot_response += message
+            print()
+            if self.speak:
+                from .speak import speak
+                await speak(bot_response)
+            self.chat_history.append(bot_response)
+
+    def handle(self, prefix):
+
+        def handle_for_prefix(function):
+            self.middleware[prefix] = function
+            return function
+
+        return handle_for_prefix
+
+    class Exit(BaseException):
+        pass
+
+    class Continue(BaseException):
+        pass
+
+
+app = App()
+
+
+@app.handle("/quit")
+@app.handle("/exit")
+def _(self, line):
+    raise self.Exit()
+
+
+@app.handle("/multiline")
+def _(self, line):
+    self.multiline = not self.multiline
+    print(f"{self.multiline=}")
+    raise self.Continue()
+
+
+@app.handle("/prompt")
+def _(self, line):
+    self.prompt = line
+    print("Update prompt to:", self.prompt)
+    raise self.Continue()
+
+
+@app.handle("/record")
+async def _(self, line):
+    from .record import record_and_transcribe
+    user_input = await record_and_transcribe()
+    print("You:", user_input)
+    return user_input
+
+
+@app.handle("/history")
+def _(self, line):
+    print("History:")
+    print("Sys:", self.prompt)
+    for i, content in enumerate(self.chat_history):
+        print("You:" if i % 2 == 0 else "Bot:", content)
+    raise self.Continue()
+
+
+@app.handle("/rollback")
+def _(self, line):
+    self.chat_history = self.chat_history[:-2]
+    print("Rollback the history")
+    raise self.Continue()
+
+
+@app.handle("/edit")
+async def _(self, line):
+    last_chat = self.chat_history[-1]
+    user_edit = await self.session.prompt_async(
+        "Bot: ",
+        multiline=self.multiline,
+        prompt_continuation=prompt_continuation,
+        default=last_chat,
+    )
+    self.chat_history[-1] = user_edit
+    raise self.Continue()
+
+
+@app.handle("/speak")
+def _(self, line):
+    self.speak = not self.speak
+    print(f"{self.speak=}")
+    raise self.Continue()
 
 
 if __name__ == "__main__":
-    fire.Fire(main)
+    asyncio.run(app.driver())
```

## Comparing `gpt_bot-0.0.2.dist-info/METADATA` & `gpt_bot-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gpt-bot
-Version: 0.0.2
+Version: 0.0.3
 Summary: GPT Commandline interface bot
 Home-page: https://github.com/hzhangxyz/gpt-bot
 Author: Hao Zhang
 Author-email: zh970205@mail.ustc.edu.cn
 License: GPLv3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: fire
 Requires-Dist: numpy
 Requires-Dist: openai
 Requires-Dist: prompt-toolkit
 Requires-Dist: pyaudio
 Requires-Dist: tiktoken
 
 # gpt-bot
```

