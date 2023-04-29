# Comparing `tmp/ipymock-1.0.2.tar.gz` & `tmp/ipymock-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.0.2.tar", last modified: Fri Apr 28 23:35:28 2023, max compression
+gzip compressed data, was "ipymock-1.0.3.tar", last modified: Sat Apr 29 09:27:02 2023, max compression
```

## Comparing `ipymock-1.0.2.tar` & `ipymock-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.481143 ipymock-1.0.2/
--rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.2/LICENSE
--rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.2/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)    10267 2023-04-28 23:35:28.480740 ipymock-1.0.2/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     9517 2023-04-28 23:34:45.000000 ipymock-1.0.2/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.476525 ipymock-1.0.2/ipymock/
--rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/__init__.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2405 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/_nbdev.py
--rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/agi.py
--rw-rw-r--   0 saintway   (501) staff       (20)    12854 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/browser.py
--rw-rw-r--   0 saintway   (501) staff       (20)      977 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/llm.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/reader.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.479222 ipymock-1.0.2/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.480085 ipymock-1.0.2/ipymock.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)    10267 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/PKG-INFO
--rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/SOURCES.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/dependency_links.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.2/ipymock.egg-info/not-zip-safe
--rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/requires.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/top_level.txt
--rw-rw-r--   0 saintway   (501) staff       (20)     2586 2023-04-28 23:33:09.000000 ipymock-1.0.2/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-28 23:35:28.481225 ipymock-1.0.2/setup.cfg
--rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.2/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.326377 ipymock-1.0.3/
+-rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.3/LICENSE
+-rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.3/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)    10620 2023-04-29 09:27:02.325906 ipymock-1.0.3/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     9877 2023-04-29 09:26:04.000000 ipymock-1.0.3/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.322131 ipymock-1.0.3/ipymock/
+-rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/__init__.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2454 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/_nbdev.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/agi.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    15390 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/browser.py
+-rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/llm.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-04-29 09:25:44.000000 ipymock-1.0.3/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.324315 ipymock-1.0.3/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-29 09:27:02.325183 ipymock-1.0.3/ipymock.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.3/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.3/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)    10620 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/PKG-INFO
+-rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/SOURCES.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/dependency_links.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.3/ipymock.egg-info/not-zip-safe
+-rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/requires.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-29 09:27:02.000000 ipymock-1.0.3/ipymock.egg-info/top_level.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)     2610 2023-04-29 09:06:43.000000 ipymock-1.0.3/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-29 09:27:02.326479 ipymock-1.0.3/setup.cfg
+-rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.3/setup.py
```

### Comparing `ipymock-1.0.2/LICENSE` & `ipymock-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.2/PKG-INFO` & `ipymock-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.2
-Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
+Version: 1.0.3
+Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Running PyTest in Jupyter Notebooks
+> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
 
+[![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
+[![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
 Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
 
 ```bash
 mkdir -p ~/.config/ipymock
@@ -124,15 +127,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -140,24 +143,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -203,15 +206,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -220,22 +223,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -280,34 +283,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
 
@@ -316,12 +319,12 @@
     
     => no.0  nbs::test_fixture  runtest  passed
     
 
 
 ## Troubleshooting Tips of NbDev
 
--  Make sure you are using the latest version of nbdev with `pip install -U nbdev`
+-  Make sure you are using the latest version of nbdev with `pip install --upgrade nbdev`
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
```

### Comparing `ipymock-1.0.2/README.md` & `ipymock-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # Running PyTest in Jupyter Notebooks
+> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
 
+[![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
+[![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
 Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
 
 ```bash
 mkdir -p ~/.config/ipymock
@@ -104,15 +107,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -120,24 +123,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -183,15 +186,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -200,22 +203,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -260,34 +263,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
 
@@ -296,12 +299,12 @@
     
     => no.0  nbs::test_fixture  runtest  passed
     
 
 
 ## Troubleshooting Tips of NbDev
 
--  Make sure you are using the latest version of nbdev with `pip install -U nbdev`
+-  Make sure you are using the latest version of nbdev with `pip install --upgrade nbdev`
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
```

### Comparing `ipymock-1.0.2/ipymock/__init__.py` & `ipymock-1.0.3/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.2/ipymock/_nbdev.py` & `ipymock-1.0.3/ipymock/_nbdev.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,20 @@
          "rename_title": "2_browser.ipynb",
          "delete_conversation": "2_browser.ipynb",
          "recover_conversation": "2_browser.ipynb",
          "clear_conversations": "2_browser.ipynb",
          "attrdict": "2_browser.ipynb",
          "attributize": "2_browser.ipynb",
          "delta": "2_browser.ipynb",
-         "mock_create": "3_llm.ipynb",
+         "mock_create": "2_browser.ipynb",
          "chat_delta": "2_browser.ipynb",
          "mock_chat_create": "2_browser.ipynb",
          "mock_openai": "2_browser.ipynb",
          "embeddings_model": "4_agi.ipynb",
+         "mock_embed_create": "3_llm.ipynb",
          "mock_openai_embed": "3_llm.ipynb",
          "embedding_size": "4_agi.ipynb",
          "index": "4_agi.ipynb",
          "vectorstore": "4_agi.ipynb",
          "TaskCreationChain": "4_agi.ipynb",
          "TaskPrioritizationChain": "4_agi.ipynb",
          "ExecutionChain": "4_agi.ipynb",
```

### Comparing `ipymock-1.0.2/ipymock/agi.py` & `ipymock-1.0.3/ipymock/agi.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.2/ipymock/browser.py` & `ipymock-1.0.3/ipymock/browser.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,46 +53,61 @@
     return current_node
 
 def handle_conversation_detail(current_node, mapping):
     conversation_detail = mapping[current_node]
     parent_id = conversation_detail.get('parent', '')
     if parent_id != '':
         handle_conversation_detail(parent_id, mapping)
-        common.question_answer_map[parent_id] = conversation_detail['message']['content']['parts'][0].strip()
+        common.question_answer_map[parent_id] = ''.join(conversation_detail['message']['content']['parts']).strip()
     if 'message' not in conversation_detail:
         return
     message = conversation_detail['message']
     parts = message['content']['parts']
     if len(parts) > 0 and parts[0] != '' and message['author']['role'] == common.role_user:
         common.message_channel.put(message)
 
-def start_conversation(content):
+def start_conversation(prompt):
     if common.conversation_id != '' and common.parent_message_id == '':
         try:
             common.parent_message_id = get_conversation(common.conversation_id)
         except requests.exceptions.ConnectionError as errc:
             sys.stderr.write(f'Error Connecting: {errc}\n')
 
     if common.conversation_id == '' or common.parent_message_id == '':
         common.conversation_id = ''
         common.parent_message_id = str(uuid.uuid4())
 
+    if isinstance(prompt, str):
+        prompt = [{'role': common.role_user, 'parts': [prompt]}]
+    if isinstance(prompt, dict):
+        prompt = [prompt]
+    if isinstance(prompt, list):
+        raw_prompt = prompt
+        prompt = []
+        parts = []
+        for item in raw_prompt:
+            if isinstance(item, dict):
+                prompt.append(item)
+            else:
+                parts.append(str(item))
+        prompt.append({'role': common.role_user, 'parts': parts})
+
     post_data = {
         'action': 'next',
         'messages': [{
             'id': str(uuid.uuid4()),
             'author': {
-                'role': common.role_user,
+                'role': msg['role'],
             },
-            'role': common.role_user,
+            'role': msg['role'],
             'content': {
                 'content_type': 'text',
-                'parts': [content],
+                'parts': msg['parts'],
             },
-        }],
+        } for msg in prompt],
         'model': common.chat_gpt_model,
         'continue_text': '',
     }
     if common.conversation_id != '':
         post_data['conversation_id'] = common.conversation_id
     if common.parent_message_id != '':
         post_data['parent_message_id'] = common.parent_message_id
@@ -224,26 +239,55 @@
     return obj
 
 def delta(prompt):
     id = ''.join(
         random.choices(string.ascii_letters + string.digits, k = 29)
     )
     res = ''
-    for response in start_conversation(prompt):
-        yield attributize({
-            'choices': [
-                {
-                    'index': 0,
-                    'logprobs': None,
-                    'text': response[len(res):],
-                }
-            ],
-            'id': f'cmpl-{id}',
-        })
-        res = response
+    wait_second = 1
+    while True:
+        try:
+            for response in start_conversation(prompt):
+                yield attributize({
+                    'choices': [
+                        {
+                            'index': 0,
+                            'logprobs': None,
+                            'text': response[len(res):],
+                        }
+                    ],
+                    'id': f'cmpl-{id}',
+                })
+                res = response
+        except requests.exceptions.HTTPError as err:
+            sys.stderr.write(
+                f'{err}\n'
+                f'response = {repr(response)}\n'
+                f'Retrying...\n'
+            )
+            status_code = err.response.status_code
+            if status_code == 413:
+                # caller should split the prompt
+                break
+            # if status_code == 429:
+            #     break
+            if status_code >= 400 and status_code != 500:
+                time.sleep(wait_second)
+                wait_second *= 2
+                continue
+            break
+        if response == '':
+            sys.stderr.write(
+                f'Error Responding: response = {repr(response)}\n'
+                f'Retrying...\n'
+            )
+            time.sleep(wait_second)
+            wait_second *= 2
+            continue
+        break
 
 def mock_create(*args, **kwargs):
     prompts = []
     if isinstance(kwargs['prompt'], str):
         prompts = [kwargs['prompt']]
     if isinstance(kwargs['prompt'], list):
         prompts = kwargs['prompt']
@@ -264,15 +308,15 @@
                 sys.stderr.write(
                     f'{err}\n'
                     f'response = {repr(response)}\n'
                     f'Retrying...\n'
                 )
                 status_code = err.response.status_code
                 if status_code == 413:
-                    # todo: split the prompt
+                    # caller should split the prompt
                     break
                 # if status_code == 429:
                 #     break
                 if status_code >= 400 and status_code != 500:
                     time.sleep(wait_second)
                     wait_second *= 2
                     continue
@@ -306,33 +350,61 @@
     })
 
 def chat_delta(prompt):
     id = ''.join(
         random.choices(string.ascii_letters + string.digits, k = 29)
     )
     res = ''
-    for response in start_conversation(prompt):
-        yield attributize({
-            'choices': [
-                {
-                    'index': 0,
-                    'delta': {
-                        'content': response[len(res):],
-                    }
-                }
-            ],
-            'id': f'chatcmpl-{id}',
-        })
-        res = response
+    wait_second = 1
+    while True:
+        try:
+            for response in start_conversation(prompt):
+                yield attributize({
+                    'choices': [
+                        {
+                            'index': 0,
+                            'delta': {
+                                'content': response[len(res):],
+                            }
+                        }
+                    ],
+                    'id': f'chatcmpl-{id}',
+                })
+                res = response
+        except requests.exceptions.HTTPError as err:
+            sys.stderr.write(
+                f'{err}\n'
+                f'response = {repr(response)}\n'
+                f'Retrying...\n'
+            )
+            status_code = err.response.status_code
+            if status_code == 413:
+                # caller should split the prompt
+                break
+            # if status_code == 429:
+            #     break
+            if status_code >= 400 and status_code != 500:
+                time.sleep(wait_second)
+                wait_second *= 2
+                continue
+            break
+        if response == '':
+            sys.stderr.write(
+                f'Error Responding: response = {repr(response)}\n'
+                f'Retrying...\n'
+            )
+            time.sleep(wait_second)
+            wait_second *= 2
+            continue
+        break
 
 def mock_chat_create(*args, **kwargs):
-    summarized_prompt = ''
+    summarized_prompt = []
     for message in kwargs['messages']:
-        summarized_prompt += f"{message['role']}:\n\n{message['content']}\n\n\n"
-    summarized_prompt.strip()
+        summarized_prompt.append({'role': message['role'], 'parts': [message['content']]})
 
     if kwargs.get('stream', False):
         return chat_delta(summarized_prompt)
 
     response = ''
     wait_second = 1
     while True:
@@ -343,15 +415,15 @@
             sys.stderr.write(
                 f'{err}\n'
                 f'response = {repr(response)}\n'
                 f'Retrying...\n'
             )
             status_code = err.response.status_code
             if status_code == 413:
-                # todo: split the prompt
+                # caller should split the prompt
                 break
             # if status_code == 429:
             #     break
             if status_code >= 400 and status_code != 500:
                 time.sleep(wait_second)
                 wait_second *= 2
                 continue
```

### Comparing `ipymock-1.0.2/ipymock/llm.py` & `ipymock-1.0.3/ipymock/llm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/3_llm.ipynb (unless otherwise specified).
 
-__all__ = ['mock_create', 'mock_openai_embed']
+__all__ = ['mock_embed_create', 'mock_openai_embed']
 
 # Internal Cell
 from sentence_transformers import SentenceTransformer
 embeddings_model = SentenceTransformer('GanymedeNil/text2vec-large-chinese')
 
 # Cell
 import ipymock.browser
 
-def mock_create(**kwargs):
+def mock_embed_create(**kwargs):
     texts = kwargs['input']
     if isinstance(texts, str):
         texts = [texts]
     data = []
     for idx, embedding in enumerate(embeddings_model.encode(texts)):
         data.append({
             'object': 'embedding',
@@ -30,8 +30,8 @@
     })
 
 # Cell
 import openai, pytest
 
 @pytest.fixture
 def mock_openai_embed(monkeypatch):
-    monkeypatch.setattr(openai.Embedding, 'create', mock_create)
+    monkeypatch.setattr(openai.Embedding, 'create', mock_embed_create)
```

### Comparing `ipymock-1.0.2/ipymock/reader.py` & `ipymock-1.0.3/ipymock/reader.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.2/ipymock.egg-info/PKG-INFO` & `ipymock-1.0.3/ipymock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.0.2
-Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
+Version: 1.0.3
+Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -15,16 +15,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Running PyTest in Jupyter Notebooks
+> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
 
+[![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
+[![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
 Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
 
 ```bash
 mkdir -p ~/.config/ipymock
@@ -124,15 +127,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```python
+```
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -140,24 +143,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```python
+```
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -203,15 +206,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```python
+```
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -220,22 +223,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```python
+```
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```python
+```
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -280,34 +283,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```python
+```
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```python
+```
 from ipymock import do
 ```
 
-```python
+```
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
 
@@ -316,12 +319,12 @@
     
     => no.0  nbs::test_fixture  runtest  passed
     
 
 
 ## Troubleshooting Tips of NbDev
 
--  Make sure you are using the latest version of nbdev with `pip install -U nbdev`
+-  Make sure you are using the latest version of nbdev with `pip install --upgrade nbdev`
 -  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
 -  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
 -  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
 -  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
```

### Comparing `ipymock-1.0.2/settings.ini` & `ipymock-1.0.3/settings.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified
 host = github
 lib_name = ipymock
 # For Enterprise Git add variable repo_name and company name
 # repo_name = analytics
-# company_name = nike
+organization_name = Neuro Spirit, DAO.
 
 user = seii-saintway
-description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
+description = A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
-copyright = Neuro Spirit, DAO.
+copyright = 2023 onwards, Neuro Spirit, DAO.
 branch = main
-version = 1.0.2
+version = 1.0.3
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
@@ -37,19 +37,19 @@
 ###
 
 # Change to, e.g. "nbs", to put your notebooks in nbs dir instead of repo root
 nbs_path = nbs
 doc_path = docs
 
 # Whether to look for library notebooks recursively in the `nbs_path` dir
-recursive = False
+recursive = True
 
 # Anything shown as '%(...)s' is substituted with that setting automatically
 doc_host =  https://%(user)s.github.io
-#For Enterprise Git pages use:  
+# For Enterprise Git pages use:  
 #doc_host = https://pages.github.%(company_name)s.com.  
 
 
 doc_baseurl = /%(lib_name)s/
 # For Enterprise Github pages docs use:
 # doc_baseurl = /%(repo_name)s/%(lib_name)s/
```

### Comparing `ipymock-1.0.2/setup.py` & `ipymock-1.0.3/setup.py`

 * *Files identical despite different names*

