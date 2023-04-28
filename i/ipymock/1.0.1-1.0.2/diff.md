# Comparing `tmp/ipymock-1.0.1.tar.gz` & `tmp/ipymock-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.0.1.tar", last modified: Thu Apr 27 01:16:12 2023, max compression
+gzip compressed data, was "ipymock-1.0.2.tar", last modified: Fri Apr 28 23:35:28 2023, max compression
```

## Comparing `ipymock-1.0.1.tar` & `ipymock-1.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.132060 ipymock-1.0.1/
--rw-r--r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.1/LICENSE
--rw-r--r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.1/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-27 01:16:12.131773 ipymock-1.0.1/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     6783 2023-04-27 01:15:05.000000 ipymock-1.0.1/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.128148 ipymock-1.0.1/ipymock/
--rw-r--r--   0 saintway   (501) staff       (20)     1605 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/__init__.py
--rw-r--r--   0 saintway   (501) staff       (20)     2405 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/_nbdev.py
--rw-r--r--   0 saintway   (501) staff       (20)    18088 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/agi.py
--rw-r--r--   0 saintway   (501) staff       (20)    12854 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/browser.py
--rw-r--r--   0 saintway   (501) staff       (20)      977 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/llm.py
--rw-r--r--   0 saintway   (501) staff       (20)     2974 2023-04-27 01:10:48.000000 ipymock-1.0.1/ipymock/reader.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.130286 ipymock-1.0.1/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-27 01:16:12.131154 ipymock-1.0.1/ipymock.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.1/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.1/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 saintway   (501) staff       (20)     7533 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)      460 2023-04-27 01:16:12.000000 ipymock-1.0.1/ipymock.egg-info/SOURCES.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/dependency_links.txt
--rw-r--r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.1/ipymock.egg-info/not-zip-safe
--rw-r--r--   0 saintway   (501) staff       (20)       62 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/requires.txt
--rw-r--r--   0 saintway   (501) staff       (20)        8 2023-04-27 01:16:11.000000 ipymock-1.0.1/ipymock.egg-info/top_level.txt
--rw-r--r--   0 saintway   (501) staff       (20)     2519 2023-04-27 01:14:32.000000 ipymock-1.0.1/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-27 01:16:12.132146 ipymock-1.0.1/setup.cfg
--rw-r--r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.1/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.481143 ipymock-1.0.2/
+-rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.0.2/LICENSE
+-rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.0.2/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)    10267 2023-04-28 23:35:28.480740 ipymock-1.0.2/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)     9517 2023-04-28 23:34:45.000000 ipymock-1.0.2/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.476525 ipymock-1.0.2/ipymock/
+-rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/__init__.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2405 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/_nbdev.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/agi.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    12854 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/browser.py
+-rw-rw-r--   0 saintway   (501) staff       (20)      977 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/llm.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-04-28 23:34:20.000000 ipymock-1.0.2/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.479222 ipymock-1.0.2/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-04-28 23:35:28.480085 ipymock-1.0.2/ipymock.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.0.2/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.0.2/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)    10267 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/PKG-INFO
+-rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/SOURCES.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/dependency_links.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.0.2/ipymock.egg-info/not-zip-safe
+-rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/requires.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-28 23:35:28.000000 ipymock-1.0.2/ipymock.egg-info/top_level.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)     2586 2023-04-28 23:33:09.000000 ipymock-1.0.2/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-04-28 23:35:28.481225 ipymock-1.0.2/setup.cfg
+-rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.0.2/setup.py
```

### Comparing `ipymock-1.0.1/LICENSE` & `ipymock-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.1/PKG-INFO` & `ipymock-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,118 @@
-Metadata-Version: 2.1
-Name: ipymock
-Version: 1.0.1
-Summary: A pytest plugin that let you run pytest within Jupyter Notebook cells.
-Home-page: https://github.com/seii-saintway/ipymock/tree/main/
-Author: andrew
-Author-email: andrew.saintway@gmail.com
-License: Apache Software License 2.0
-Keywords: pytest interactive jupyter
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# Running PyTest in Jupyter Notebooks
 
-# A Jupyter Notebook Runtime Pytest Plugin
-> This pytest plugin project is created by the <a href='https://youtu.be/ZJTop5uqC2U'>NbDev Template</a>.
 
 
-## Troubleshooting Tips
+## Setup iPyMock
 
--  Make sure you are using the latest version of nbdev with `pip install -U nbdev`
--  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
--  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
--  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
--  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
+Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
+
+```bash
+mkdir -p ~/.config/ipymock
+
+cat << EOF > ~/.config/ipymock/config.json
+{
+  "access_token": "<access_token>",
+  "conversation_id": "<conversation_id>"
+}
+EOF
 
-## Pytest the Python Testfiles
+pip install --upgrade ipymock
+```
+
+## Using the Browser Side API in Jupyter Notebooks
+
+```python
+from ipymock.browser import start_conversation
+import IPython
 
+def ask(prompt):
+    for response in start_conversation(prompt):
+        IPython.display.display(IPython.core.display.Markdown(response))
+        IPython.display.clear_output(wait=True)
+
+import ipymock.browser
+# if the proxy is deployed locally
+ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
+# otherwise using a third party proxy
+ipymock.browser.common.chat_gpt_base_url = 'https://.../api'
+# the conversation_id which is set in config.json
+print(ipymock.browser.common.conversation_id)
+
+ask('''
+what is the meaning of getting patched?
+''')
 ```
+
+## Testing AutoGPT
+
+This is the test function for AutoGPT.
+
+```python
+import os, sys
+os.chdir(os.path.expanduser('~/Auto-GPT'))
+sys.path.append(os.path.expanduser('~/Auto-GPT'))
+
+def test_auto_gpt(
+    mock_openai,
+    mock_openai_embed,
+    reset_embed_dimension,
+):
+    from autogpt.main import run_auto_gpt
+    run_auto_gpt(
+        continuous = True,
+        continuous_limit = 10000,
+        ai_settings = None,
+        skip_reprompt = False,
+        speak = True,
+        debug = False,
+        gpt3only = False,
+        gpt4only = True,
+        memory_type = 'local',
+        browser_name = 'safari',
+        allow_downloads = True,
+        skip_news = True,
+        workspace_directory = os.path.expanduser('~/Auto-GPT/andrew_space'),
+        install_plugin_deps = True,
+    )
+    assert True
+```
+
+It actually run AutoGPT by pytest mock and browser automation.
+
+```python
+import ipymock
+import ipymock.browser
+import ipymock.llm
+import pytest
+
+ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
+# reset conversation_id to empty to start a new chat
+ipymock.browser.common.conversation_id = ''
+
+@pytest.fixture
+def reset_embed_dimension(monkeypatch):
+    import autogpt.memory.local
+    monkeypatch.setattr(autogpt.memory.local, 'EMBED_DIM', 1024)
+
+ipymock.do(
+    mock_openai = ipymock.browser.mock_openai,
+    mock_openai_embed = ipymock.llm.mock_openai_embed,
+    reset_embed_dimension = reset_embed_dimension,
+    test_auto_gpt = test_auto_gpt,
+)
+```
+
+This project is still under development and lack of documentation.
+
+This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
+
+## The Mechanism of PyTesting the Python Testfiles
+
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -44,24 +120,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
-## Pytest the Python Testcases within IPyNb Runtimes
+### PyTesting the Python Testcases within iPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -107,15 +183,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -124,22 +200,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -182,42 +258,50 @@
 ```python
 for i, f in enumerate(m.collect()):
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
-### How to use the do-pytest?
+### How to Use the Do-PyTest?
 
-```
+```python
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
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
 
     
     => no.0  nbs::test_fixture  setup  passed
     
     => no.0  nbs::test_fixture  runtest  passed
     
 
+
+## Troubleshooting Tips of NbDev
+
+-  Make sure you are using the latest version of nbdev with `pip install -U nbdev`
+-  If you are using an older version of this template, see the instructions above on how to upgrade your template. 
+-  It is important for you to spell the name of your user and repo correctly in `settings.ini` or the website will not have the correct address from which to source assets like CSS for your site.  When in doubt, you can open your browser's developer console and see if there are any errors related to fetching assets for your website due to an incorrect URL generated by misspelled values from `settings.ini`.
+-  If you change the name of your repo, you have to make the appropriate changes in `settings.ini`
+-  After you make changes to `settings.ini`, run `nbdev_build_lib && nbdev_clean_nbs && nbdev_build_docs` to make sure all changes are propagated appropriately.
```

### Comparing `ipymock-1.0.1/ipymock/__init__.py` & `ipymock-1.0.2/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.1/ipymock/_nbdev.py` & `ipymock-1.0.2/ipymock/_nbdev.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.1/ipymock/agi.py` & `ipymock-1.0.2/ipymock/agi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/4_agi.ipynb (unless otherwise specified).
 
 __all__ = ['BabyAGI', 'tools', 'ZeroRoundAgent', 'llm', 'FORMAT_INSTRUCTIONS', 'llm_chain', 'ChineseOutputParser',
            'FINAL_ANSWER_ACTION', 'agent_executor', 'baby_agi', 'common', 'mock_baby_agi']
 
-# Internal Cell
+# Cell
 import time
 from collections import deque
 from typing import Dict, List, Optional, Any
 
 # Internal Cell
 from langchain import LLMChain, OpenAI, PromptTemplate
 from langchain.llms import BaseLLM
```

### Comparing `ipymock-1.0.1/ipymock/browser.py` & `ipymock-1.0.2/ipymock/browser.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.1/ipymock/llm.py` & `ipymock-1.0.2/ipymock/llm.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.1/ipymock/reader.py` & `ipymock-1.0.2/ipymock/reader.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.0.1/settings.ini` & `ipymock-1.0.2/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 user = seii-saintway
 description = A pytest plugin that let you run pytest within Jupyter Notebook cells.
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = Neuro Spirit, DAO.
 branch = main
-version = 1.0.1
+version = 1.0.2
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
 status = 2
 
 # Optional. Same format as setuptools requirements
-requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.*
+requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.* pydantic==1.* langchain==0.* faiss-cpu==1.* duckduckgo_search==2.*
 # Optional. Same format as setuptools console_scripts
 # console_scripts = 
 # Optional. Same format as setuptools dependency-links
 # dep_links = 
 
 ###
 # You probably won't need to change anything under here,
```

### Comparing `ipymock-1.0.1/setup.py` & `ipymock-1.0.2/setup.py`

 * *Files identical despite different names*

