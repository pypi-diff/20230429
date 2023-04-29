# Comparing `tmp/golem_garden-0.5.2.tar.gz` & `tmp/golem_garden-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_garden-0.5.2.tar", last modified: Sat Apr 29 14:42:32 2023, max compression
+gzip compressed data, was "golem_garden-0.5.3.tar", last modified: Sat Apr 29 14:52:22 2023, max compression
```

## Comparing `golem_garden-0.5.2.tar` & `golem_garden-0.5.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      834 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/workflows/deploy_docs.yml
--rw-r--r--   0        0        0     1123 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1883 2023-04-29 14:42:26.024752 golem_garden-0.5.2/.gitignore
--rw-r--r--   0        0        0     3348 2023-04-29 14:42:26.024752 golem_garden-0.5.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    34523 2023-04-29 14:42:26.024752 golem_garden-0.5.2/LICENSE
--rw-r--r--   0        0        0      190 2023-04-29 14:42:26.024752 golem_garden-0.5.2/README.md
--rw-r--r--   0        0        0       79 2023-04-29 14:42:26.024752 golem_garden-0.5.2/RUN_ME.py
--rw-r--r--   0        0        0     1640 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/Community Guidelines/Code of Conduct.md
--rw-r--r--   0        0        0     3511 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/Contributing guide/Contributing.md
--rw-r--r--   0        0        0     2790 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/Contributing guide/python_style_guide.md
--rw-r--r--   0        0        0      190 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/index.md
--rw-r--r--   0        0        0     2485 2023-04-29 14:42:26.024752 golem_garden-0.5.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      251 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/__init__.py
--rw-r--r--   0        0        0      910 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/__main__.py
--rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/data_loaders/__init__.py
--rw-r--r--   0        0        0      996 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/data_loaders/async_load_url_with_playwright.py
--rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/golems/__init__.py
--rw-r--r--   0        0        0     2125 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/golems/golem.py
--rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/output_parsers/__init__.py
--rw-r--r--   0        0        0     1186 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/output_parsers/output_parser.py
--rw-r--r--   0        0        0        0 2023-04-29 14:42:26.024752 golem_garden-0.5.2/golem_garden/prompts/__init__.py
--rw-r--r--   0        0        0     1777 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/prompts/prompts.py
--rw-r--r--   0        0        0        0 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/__init__.py
--rw-r--r--   0        0        0     3378 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/directory_printer.py
--rw-r--r--   0        0        0     5029 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/grab_all_py_in_one_text_block.py
--rw-r--r--   0        0        0      484 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
--rw-r--r--   0        0        0     3686 2023-04-29 14:42:26.028751 golem_garden-0.5.2/golem_garden/tools/tools.py
--rw-r--r--   0        0        0    29940 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/ask_freemocap_docs.ipynb
--rw-r--r--   0        0        0     8092 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/dog_mailer_auto_gpt.py
--rw-r--r--   0        0        0    20524 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
--rw-r--r--   0        0        0     3890 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/langchain_agent_playground.py
--rw-r--r--   0        0        0    26686 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/autogpt.ipynb
--rw-r--r--   0        0        0    31113 2023-04-29 14:42:26.028751 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
--rw-r--r--   0        0        0    18274 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb
--rw-r--r--   0        0        0    60363 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
--rw-r--r--   0        0        0    44476 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
--rw-r--r--   0        0        0    23377 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
--rw-r--r--   0        0        0      882 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
--rw-r--r--   0        0        0    18760 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
--rw-r--r--   0        0        0    60951 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/marathon_times.ipynb
--rw-r--r--   0        0        0    23334 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
--rw-r--r--   0        0        0    25052 2023-04-29 14:42:26.032752 golem_garden-0.5.2/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
--rw-r--r--   0        0        0      123 2023-04-29 14:42:26.032752 golem_garden-0.5.2/mkdocs.yml
--rw-r--r--   0        0        0      356 2023-04-29 14:42:26.032752 golem_garden-0.5.2/notes/bluesky_todos.md
--rw-r--r--   0        0        0     1296 2023-04-29 14:42:26.032752 golem_garden-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      232 2023-04-29 14:42:26.032752 golem_garden-0.5.2/sample.env
--rw-r--r--   0        0        0       99 2023-04-29 14:42:26.032752 golem_garden-0.5.2/utilities/env_setup.bat
--rw-r--r--   0        0        0     2280 2023-04-29 14:42:26.032752 golem_garden-0.5.2/utilities/pinecone.py
--rw-r--r--   0        0        0      507 2023-04-29 14:42:26.032752 golem_garden-0.5.2/utilities/try_mongo_connection.py
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 golem_garden-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      834 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/workflows/deploy_docs.yml
+-rw-r--r--   0        0        0     1123 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1883 2023-04-29 14:52:16.047027 golem_garden-0.5.3/.gitignore
+-rw-r--r--   0        0        0     3348 2023-04-29 14:52:16.047027 golem_garden-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    34523 2023-04-29 14:52:16.051028 golem_garden-0.5.3/LICENSE
+-rw-r--r--   0        0        0      190 2023-04-29 14:52:16.051028 golem_garden-0.5.3/README.md
+-rw-r--r--   0        0        0       79 2023-04-29 14:52:16.051028 golem_garden-0.5.3/RUN_ME.py
+-rw-r--r--   0        0        0     1640 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/Community Guidelines/Code of Conduct.md
+-rw-r--r--   0        0        0     3511 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/Contributing guide/Contributing.md
+-rw-r--r--   0        0        0     2790 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/Contributing guide/python_style_guide.md
+-rw-r--r--   0        0        0      190 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/index.md
+-rw-r--r--   0        0        0     2485 2023-04-29 14:52:16.051028 golem_garden-0.5.3/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      295 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/__init__.py
+-rw-r--r--   0        0        0      897 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/data_loaders/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/data_loaders/async_load_url_with_playwright.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/golems/__init__.py
+-rw-r--r--   0        0        0     2118 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/golems/golem.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/output_parsers/__init__.py
+-rw-r--r--   0        0        0     1186 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/output_parsers/output_parser.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/prompts/__init__.py
+-rw-r--r--   0        0        0     1777 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/prompts/prompts.py
+-rw-r--r--   0        0        0        0 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/__init__.py
+-rw-r--r--   0        0        0     3378 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/directory_printer.py
+-rw-r--r--   0        0        0     5029 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/grab_all_py_in_one_text_block.py
+-rw-r--r--   0        0        0      484 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/output/copy_of_directories_on_2023-04-22_21_26_57_output.md
+-rw-r--r--   0        0        0     3686 2023-04-29 14:52:16.051028 golem_garden-0.5.3/golem_garden/tools/tools.py
+-rw-r--r--   0        0        0    29940 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/ask_freemocap_docs.ipynb
+-rw-r--r--   0        0        0     8092 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/dog_mailer_auto_gpt.py
+-rw-r--r--   0        0        0    20524 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0     3890 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_agent_playground.py
+-rw-r--r--   0        0        0    26686 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/autogpt.ipynb
+-rw-r--r--   0        0        0    31113 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb
+-rw-r--r--   0        0        0    18274 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb
+-rw-r--r--   0        0        0    60363 2023-04-29 14:52:16.051028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb
+-rw-r--r--   0        0        0    44476 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb
+-rw-r--r--   0        0        0    23377 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb
+-rw-r--r--   0        0        0      882 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_playground.ipynb
+-rw-r--r--   0        0        0    18760 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb
+-rw-r--r--   0        0        0    60951 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/marathon_times.ipynb
+-rw-r--r--   0        0        0    23334 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb
+-rw-r--r--   0        0        0    25052 2023-04-29 14:52:16.055028 golem_garden-0.5.3/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb
+-rw-r--r--   0        0        0      123 2023-04-29 14:52:16.055028 golem_garden-0.5.3/mkdocs.yml
+-rw-r--r--   0        0        0      356 2023-04-29 14:52:16.055028 golem_garden-0.5.3/notes/bluesky_todos.md
+-rw-r--r--   0        0        0     1296 2023-04-29 14:52:16.055028 golem_garden-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-04-29 14:52:16.055028 golem_garden-0.5.3/sample.env
+-rw-r--r--   0        0        0       99 2023-04-29 14:52:16.055028 golem_garden-0.5.3/utilities/env_setup.bat
+-rw-r--r--   0        0        0     2280 2023-04-29 14:52:16.055028 golem_garden-0.5.3/utilities/pinecone.py
+-rw-r--r--   0        0        0      507 2023-04-29 14:52:16.055028 golem_garden-0.5.3/utilities/try_mongo_connection.py
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 golem_garden-0.5.3/PKG-INFO
```

### Comparing `golem_garden-0.5.2/.github/ISSUE_TEMPLATE/bug_report.md` & `golem_garden-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/.github/ISSUE_TEMPLATE/feature_request.md` & `golem_garden-0.5.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/.github/workflows/deploy_docs.yml` & `golem_garden-0.5.3/.github/workflows/deploy_docs.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `golem_garden-0.5.3/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/.gitignore` & `golem_garden-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/CONTRIBUTING.md` & `golem_garden-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/LICENSE` & `golem_garden-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/docs/Community Guidelines/Code of Conduct.md` & `golem_garden-0.5.3/docs/Community Guidelines/Code of Conduct.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/docs/Contributing guide/Contributing.md` & `golem_garden-0.5.3/docs/Contributing guide/Contributing.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/docs/Contributing guide/python_style_guide.md` & `golem_garden-0.5.3/docs/Contributing guide/python_style_guide.md`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/docs/stylesheets/extra.css` & `golem_garden-0.5.3/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/golem_garden/__main__.py` & `golem_garden-0.5.3/golem_garden/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 base_package_path = Path(__file__).parent.parent
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from rich.console import Console
 
 rich_console = Console()
 
-from golem_garden.golems.golem import Golem
+from golem_garden import Golem
 
 
 
 class GolemGarden:
     def __init__(self):
 
         self._golem = Golem()
```

### Comparing `golem_garden-0.5.2/golem_garden/data_loaders/async_load_url_with_playwright.py` & `golem_garden-0.5.3/golem_garden/data_loaders/async_load_url_with_playwright.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/golem_garden/golems/golem.py` & `golem_garden-0.5.3/golem_garden/golems/golem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+import logging
 import os
 
 from dotenv import load_dotenv
 from langchain.agents import Tool, initialize_agent, AgentType
 from langchain.chat_models import ChatOpenAI
 from langchain.memory import ConversationBufferMemory
 
-from golem_garden.__main__ import rich_console
+
 
 load_dotenv()
 
 from langchain import SerpAPIWrapper, WikipediaAPIWrapper, WolframAlphaAPIWrapper
 
+logger = logging.getLogger(__name__)
+
 class Golem:
     def __init__(self):
-        rich_console.print("Initializing Golem...")
+        logger.info("Initializing Golem...")
         self._serper_search = SerpAPIWrapper(serpapi_api_key=os.environ["SERPER_API_KEY"])
         self._wikipedia_search = WikipediaAPIWrapper()
         self._wolfram_alpha = WolframAlphaAPIWrapper(wolfram_alpha_appid=os.environ["WOLFRAM_ALPHA_APPID"])
         self._tools = [
             Tool(
                 name="Current Search",
                 func=self._serper_search.run,
@@ -40,10 +43,10 @@
         self._chain = initialize_agent(self._tools,
                                        self._llm,
                                        agent=AgentType.CHAT_CONVERSATIONAL_REACT_DESCRIPTION,
                                        verbose=True,
                                        memory=self._memory)
 
     def intake_message(self, message: str):
-        rich_console.print(f"Received message: {message}")
+        logger.info(f"Received message: {message}")
         response = self._chain.run(message)
         return response
```

### Comparing `golem_garden-0.5.2/golem_garden/output_parsers/output_parser.py` & `golem_garden-0.5.3/golem_garden/output_parsers/output_parser.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/golem_garden/prompts/prompts.py` & `golem_garden-0.5.3/golem_garden/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/golem_garden/tools/directory_printer.py` & `golem_garden-0.5.3/golem_garden/tools/directory_printer.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/golem_garden/tools/grab_all_py_in_one_text_block.py` & `golem_garden-0.5.3/golem_garden/tools/grab_all_py_in_one_text_block.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/golem_garden/tools/tools.py` & `golem_garden-0.5.3/golem_garden/tools/tools.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/ask_freemocap_docs.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/ask_freemocap_docs.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/dog_mailer_auto_gpt.py` & `golem_garden-0.5.3/jupyter_notebooks/dog_mailer_auto_gpt.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/dog_mailer_baby_agi_with_agent.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_agent_playground.py` & `golem_garden-0.5.3/jupyter_notebooks/langchain_agent_playground.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/autogpt.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/autogpt.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/camel_role_playing.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/custom_agent_with_plugin_retrieval_using_plugnplai.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_baby_agi_old.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_docs_baby_agi_with_agent.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_playground.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_playground.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/langchain_semantic_search.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/marathon_times.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/marathon_times.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/multi_player_dnd.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb` & `golem_garden-0.5.3/jupyter_notebooks/langchain_docs/sharedmemory_for_tools.ipynb`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/pyproject.toml` & `golem_garden-0.5.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/jonmatthis/golem_garden"
 
 [tool.bumpver]
-current_version = "v0.5.2"
+current_version = "v0.5.3"
 
 version_pattern = "vMAJOR.MINOR.PATCH[-TAG]"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
```

### Comparing `golem_garden-0.5.2/utilities/pinecone.py` & `golem_garden-0.5.3/utilities/pinecone.py`

 * *Files identical despite different names*

### Comparing `golem_garden-0.5.2/PKG-INFO` & `golem_garden-0.5.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golem_garden
-Version: 0.5.2
+Version: 0.5.3
 Summary: Welcome to the Garden - We're so glad you're here <3 
 Keywords: chat
 Author: Jonathan Samir Matthis
 Requires-Python: >=3.9 , <4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: python-dotenv
```

