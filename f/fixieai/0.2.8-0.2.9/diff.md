# Comparing `tmp/fixieai-0.2.8.tar.gz` & `tmp/fixieai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixieai-0.2.8.tar", max compression
+gzip compressed data, was "fixieai-0.2.9.tar", max compression
```

## Comparing `fixieai-0.2.8.tar` & `fixieai-0.2.9.tar`

### file list

```diff
@@ -1,41 +1,47 @@
--rw-r--r--   0        0        0    11357 2023-02-23 22:50:37.233187 fixieai-0.2.8/LICENSE
--rw-r--r--   0        0        0     1004 2023-03-23 19:55:59.424183 fixieai-0.2.8/fixieai/__init__.py
--rw-r--r--   0        0        0      730 2023-03-23 19:55:59.424744 fixieai-0.2.8/fixieai/agents/__init__.py
--rw-r--r--   0        0        0     2284 2023-03-09 06:10:51.909136 fixieai-0.2.8/fixieai/agents/api.py
--rw-r--r--   0        0        0      863 2023-03-09 06:10:51.909511 fixieai-0.2.8/fixieai/agents/api_test.py
--rw-r--r--   0        0        0    13650 2023-03-28 16:51:27.397705 fixieai-0.2.8/fixieai/agents/code_shot.py
--rw-r--r--   0        0        0     8278 2023-03-28 16:51:27.398008 fixieai-0.2.8/fixieai/agents/code_shot_test.py
--rw-r--r--   0        0        0      392 2023-03-09 06:10:51.910776 fixieai-0.2.8/fixieai/agents/corpora.py
--rw-r--r--   0        0        0     8993 2023-03-03 23:24:37.371114 fixieai-0.2.8/fixieai/agents/oauth.py
--rw-r--r--   0        0        0     4711 2023-03-07 21:18:08.284870 fixieai-0.2.8/fixieai/agents/user_storage.py
--rw-r--r--   0        0        0     3092 2023-02-23 22:50:37.238945 fixieai-0.2.8/fixieai/agents/user_storage_test.py
--rw-r--r--   0        0        0    10808 2023-03-23 19:55:59.426109 fixieai-0.2.8/fixieai/agents/utils.py
--rw-r--r--   0        0        0     5253 2023-03-23 19:55:59.426492 fixieai-0.2.8/fixieai/agents/utils_test.py
--rw-r--r--   0        0        0        0 2023-03-07 21:53:04.349446 fixieai-0.2.8/fixieai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-07 17:08:15.229030 fixieai-0.2.8/fixieai/cli/agent/__init__.py
--rw-r--r--   0        0        0     1958 2023-03-23 19:55:59.427036 fixieai-0.2.8/fixieai/cli/agent/agent_config.py
--rw-r--r--   0        0        0      383 2023-03-07 17:08:15.229614 fixieai-0.2.8/fixieai/cli/agent/agent_config_test.py
--rw-r--r--   0        0        0    19095 2023-03-28 16:51:27.398754 fixieai-0.2.8/fixieai/cli/agent/commands.py
--rw-r--r--   0        0        0      949 2023-03-14 03:29:01.740659 fixieai-0.2.8/fixieai/cli/agent/commands_test.py
--rw-r--r--   0        0        0     2607 2023-03-28 16:51:27.399130 fixieai-0.2.8/fixieai/cli/agent/loader.py
--rw-r--r--   0        0        0     1641 2023-03-27 20:03:17.154129 fixieai-0.2.8/fixieai/cli/agent/tunnel.py
--rw-r--r--   0        0        0        0 2023-03-09 06:10:51.912134 fixieai-0.2.8/fixieai/cli/auth/__init__.py
--rw-r--r--   0        0        0     1753 2023-03-28 16:51:27.399587 fixieai-0.2.8/fixieai/cli/auth/commands.py
--rw-r--r--   0        0        0     1942 2023-03-09 06:10:51.912797 fixieai-0.2.8/fixieai/cli/auth/oauth_flow.py
--rw-r--r--   0        0        0     2667 2023-03-28 16:51:27.399926 fixieai-0.2.8/fixieai/cli/auth/user_config.py
--rw-r--r--   0        0        0     2120 2023-03-28 16:51:27.400303 fixieai-0.2.8/fixieai/cli/auth/user_config_test.py
--rwxr-xr-x   0        0        0     1581 2023-03-11 00:03:34.150504 fixieai-0.2.8/fixieai/cli/cli.py
--rw-r--r--   0        0        0        0 2023-03-07 17:08:15.230356 fixieai-0.2.8/fixieai/cli/session/__init__.py
--rw-r--r--   0        0        0     1731 2023-03-11 00:03:34.150791 fixieai-0.2.8/fixieai/cli/session/commands.py
--rw-r--r--   0        0        0     4720 2023-03-14 03:29:01.741160 fixieai-0.2.8/fixieai/cli/session/console.py
--rw-r--r--   0        0        0     1523 2023-03-28 16:51:27.400549 fixieai-0.2.8/fixieai/cli/utils.py
--rw-r--r--   0        0        0      655 2023-03-14 20:27:29.607865 fixieai-0.2.8/fixieai/cli/utils_test.py
--rw-r--r--   0        0        0      322 2023-03-07 17:08:15.231370 fixieai-0.2.8/fixieai/client/__init__.py
--rw-r--r--   0        0        0    12332 2023-03-14 20:27:29.608238 fixieai-0.2.8/fixieai/client/agent.py
--rwxr-xr-x   0        0        0     6979 2023-03-28 15:52:10.550353 fixieai-0.2.8/fixieai/client/client.py
--rw-r--r--   0        0        0     4987 2023-03-11 00:03:34.152283 fixieai-0.2.8/fixieai/client/client_test.py
--rwxr-xr-x   0        0        0     8750 2023-03-11 00:03:34.152549 fixieai-0.2.8/fixieai/client/session.py
--rw-r--r--   0        0        0     2238 2023-03-28 16:51:27.400784 fixieai-0.2.8/fixieai/constants.py
--rw-r--r--   0        0        0     1874 2023-03-28 16:51:27.402804 fixieai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 fixieai-0.2.8/setup.py
--rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 fixieai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-23 22:50:37.233187 fixieai-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1070 2023-03-30 01:29:50.785632 fixieai-0.2.9/fixieai/__init__.py
+-rw-r--r--   0        0        0      875 2023-03-30 01:29:50.786037 fixieai-0.2.9/fixieai/agents/__init__.py
+-rw-r--r--   0        0        0     9263 2023-03-30 01:29:50.786680 fixieai-0.2.9/fixieai/agents/agent_base.py
+-rw-r--r--   0        0        0     7113 2023-03-30 01:29:50.787128 fixieai-0.2.9/fixieai/agents/agent_base_test.py
+-rw-r--r--   0        0        0     2686 2023-03-30 01:29:50.787476 fixieai-0.2.9/fixieai/agents/api.py
+-rw-r--r--   0        0        0      863 2023-03-09 06:10:51.909511 fixieai-0.2.9/fixieai/agents/api_test.py
+-rw-r--r--   0        0        0     3491 2023-03-30 01:29:50.787837 fixieai-0.2.9/fixieai/agents/code_shot.py
+-rw-r--r--   0        0        0     2943 2023-03-30 01:29:50.788076 fixieai-0.2.9/fixieai/agents/code_shot_test.py
+-rw-r--r--   0        0        0      392 2023-03-09 06:10:51.910776 fixieai-0.2.9/fixieai/agents/corpora.py
+-rw-r--r--   0        0        0     1046 2023-03-30 01:29:50.788247 fixieai-0.2.9/fixieai/agents/llm_settings.py
+-rw-r--r--   0        0        0      839 2023-03-30 01:29:50.788531 fixieai-0.2.9/fixieai/agents/metadata.py
+-rw-r--r--   0        0        0     8993 2023-03-03 23:24:37.371114 fixieai-0.2.9/fixieai/agents/oauth.py
+-rw-r--r--   0        0        0     2127 2023-03-30 01:29:50.788828 fixieai-0.2.9/fixieai/agents/standalone.py
+-rw-r--r--   0        0        0     2154 2023-03-30 01:29:50.789122 fixieai-0.2.9/fixieai/agents/standalone_test.py
+-rw-r--r--   0        0        0     4711 2023-03-29 22:13:30.104697 fixieai-0.2.9/fixieai/agents/user_storage.py
+-rw-r--r--   0        0        0     3092 2023-02-23 22:50:37.238945 fixieai-0.2.9/fixieai/agents/user_storage_test.py
+-rw-r--r--   0        0        0    10844 2023-03-30 01:29:50.789410 fixieai-0.2.9/fixieai/agents/utils.py
+-rw-r--r--   0        0        0     5253 2023-03-23 19:55:59.426492 fixieai-0.2.9/fixieai/agents/utils_test.py
+-rw-r--r--   0        0        0        0 2023-03-07 21:53:04.349446 fixieai-0.2.9/fixieai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-07 17:08:15.229030 fixieai-0.2.9/fixieai/cli/agent/__init__.py
+-rw-r--r--   0        0        0     1958 2023-03-23 19:55:59.427036 fixieai-0.2.9/fixieai/cli/agent/agent_config.py
+-rw-r--r--   0        0        0      383 2023-03-07 17:08:15.229614 fixieai-0.2.9/fixieai/cli/agent/agent_config_test.py
+-rw-r--r--   0        0        0    19402 2023-03-30 01:29:50.789950 fixieai-0.2.9/fixieai/cli/agent/commands.py
+-rw-r--r--   0        0        0      949 2023-03-14 03:29:01.740659 fixieai-0.2.9/fixieai/cli/agent/commands_test.py
+-rw-r--r--   0        0        0     2791 2023-03-30 01:29:50.790201 fixieai-0.2.9/fixieai/cli/agent/loader.py
+-rw-r--r--   0        0        0     1641 2023-03-27 20:03:17.154129 fixieai-0.2.9/fixieai/cli/agent/tunnel.py
+-rw-r--r--   0        0        0        0 2023-03-09 06:10:51.912134 fixieai-0.2.9/fixieai/cli/auth/__init__.py
+-rw-r--r--   0        0        0     1753 2023-03-28 16:51:27.399587 fixieai-0.2.9/fixieai/cli/auth/commands.py
+-rw-r--r--   0        0        0     1942 2023-03-09 06:10:51.912797 fixieai-0.2.9/fixieai/cli/auth/oauth_flow.py
+-rw-r--r--   0        0        0     2667 2023-03-28 16:51:27.399926 fixieai-0.2.9/fixieai/cli/auth/user_config.py
+-rw-r--r--   0        0        0     2120 2023-03-28 16:51:27.400303 fixieai-0.2.9/fixieai/cli/auth/user_config_test.py
+-rwxr-xr-x   0        0        0     1581 2023-03-11 00:03:34.150504 fixieai-0.2.9/fixieai/cli/cli.py
+-rw-r--r--   0        0        0        0 2023-03-07 17:08:15.230356 fixieai-0.2.9/fixieai/cli/session/__init__.py
+-rw-r--r--   0        0        0     1731 2023-03-11 00:03:34.150791 fixieai-0.2.9/fixieai/cli/session/commands.py
+-rw-r--r--   0        0        0     4720 2023-03-14 03:29:01.741160 fixieai-0.2.9/fixieai/cli/session/console.py
+-rw-r--r--   0        0        0     1523 2023-03-28 16:51:27.400549 fixieai-0.2.9/fixieai/cli/utils.py
+-rw-r--r--   0        0        0      655 2023-03-14 20:27:29.607865 fixieai-0.2.9/fixieai/cli/utils_test.py
+-rw-r--r--   0        0        0      322 2023-03-07 17:08:15.231370 fixieai-0.2.9/fixieai/client/__init__.py
+-rw-r--r--   0        0        0    12332 2023-03-14 20:27:29.608238 fixieai-0.2.9/fixieai/client/agent.py
+-rwxr-xr-x   0        0        0     6979 2023-03-28 15:52:10.550353 fixieai-0.2.9/fixieai/client/client.py
+-rw-r--r--   0        0        0     4987 2023-03-11 00:03:34.152283 fixieai-0.2.9/fixieai/client/client_test.py
+-rwxr-xr-x   0        0        0     8750 2023-03-11 00:03:34.152549 fixieai-0.2.9/fixieai/client/session.py
+-rw-r--r--   0        0        0     2238 2023-03-28 16:51:27.400784 fixieai-0.2.9/fixieai/constants.py
+-rw-r--r--   0        0        0     1874 2023-03-30 01:30:27.861585 fixieai-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 fixieai-0.2.9/setup.py
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 fixieai-0.2.9/PKG-INFO
```

### Comparing `fixieai-0.2.8/LICENSE` & `fixieai-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/__init__.py` & `fixieai-0.2.9/fixieai/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 from fixieai.agents import DocumentCorpus
 from fixieai.agents import DocumentLoader
 from fixieai.agents import Embed
 from fixieai.agents import LlmSettings
 from fixieai.agents import Message
 from fixieai.agents import OAuthHandler
 from fixieai.agents import OAuthParams
+from fixieai.agents import StandaloneAgent
 from fixieai.agents import UserStorage
 from fixieai.client import FixieClient
 from fixieai.client import get_agents
 from fixieai.client import get_client
 from fixieai.client import get_embeds
 from fixieai.client import query
 
 __all__ = [
     "AgentQuery",
     "AgentResponse",
     "Embed",
     "Message",
     "CodeShotAgent",
+    "StandaloneAgent",
     "DocumentCorpus",
     "DocumentLoader",
     "LlmSettings",
     "OAuthParams",
     "OAuthHandler",
     "UserStorage",
     "FixieClient",
```

### Comparing `fixieai-0.2.8/fixieai/agents/__init__.py` & `fixieai-0.2.9/fixieai/agents/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
+from fixieai.agents.agent_base import AgentBase
 from fixieai.agents.api import AgentQuery
 from fixieai.agents.api import AgentResponse
 from fixieai.agents.api import Embed
 from fixieai.agents.api import Message
 from fixieai.agents.code_shot import CodeShotAgent
-from fixieai.agents.code_shot import LlmSettings
 from fixieai.agents.corpora import DocumentCorpus
 from fixieai.agents.corpora import DocumentLoader
+from fixieai.agents.llm_settings import LlmSettings
 from fixieai.agents.oauth import OAuthHandler
 from fixieai.agents.oauth import OAuthParams
+from fixieai.agents.standalone import StandaloneAgent
 from fixieai.agents.user_storage import UserStorage
 
 __all__ = [
+    "AgentBase",
     "AgentQuery",
     "AgentResponse",
     "CodeShotAgent",
     "DocumentCorpus",
     "DocumentLoader",
     "Embed",
     "LlmSettings",
     "Message",
+    "StandaloneAgent",
     "OAuthHandler",
     "OAuthParams",
     "UserStorage",
 ]
```

### Comparing `fixieai-0.2.8/fixieai/agents/api.py` & `fixieai-0.2.9/fixieai/agents/api.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """This module holds objects that represent the API interface by which Agents talk to
 Fixie ecosystem."""
 
 from __future__ import annotations
 
 import base64
 import dataclasses
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 import requests
 from pydantic import dataclasses as pydantic_dataclasses
 
 
 @pydantic_dataclasses.dataclass
 class Embed:
@@ -71,7 +71,18 @@
 
 @pydantic_dataclasses.dataclass
 class AgentResponse:
     """A response message from an Agent."""
 
     # The text of the response message.
     message: Message
+
+    @classmethod
+    def from_value(cls, value: Union[str, Message, AgentResponse]) -> AgentResponse:
+        if isinstance(value, str):
+            return cls(Message(value))
+        elif isinstance(value, Message):
+            return cls(value)
+        elif isinstance(value, cls):
+            return value
+        else:
+            raise TypeError(f"Unexpected type to wrap: {type(value)}")
```

### Comparing `fixieai-0.2.8/fixieai/agents/api_test.py` & `fixieai-0.2.9/fixieai/agents/api_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/agents/code_shot.py` & `fixieai-0.2.9/fixieai/agents/agent_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from __future__ import annotations
 
+import abc
 import dataclasses
 import functools
 import inspect
 import json
 import logging
 import os
 import re
 import warnings
-from typing import Any, Callable, Dict, Iterable, List, Optional, Union
+from typing import Any, Callable, Dict, Iterable, Optional
 
 import fastapi
 import fastapi.security
 import jwt
 import starlette.responses
 import uvicorn
 import yaml
 from pydantic import dataclasses as pydantic_dataclasses
 
 from fixieai import constants
 from fixieai.agents import api
-from fixieai.agents import corpora
+from fixieai.agents import metadata as agent_metadata
 from fixieai.agents import oauth
 from fixieai.agents import user_storage
 from fixieai.agents import utils
 
 # Regex that controls what Func names are allowed.
 ACCEPTED_FUNC_NAMES = re.compile(r"^\w+$")
 
@@ -32,144 +33,57 @@
 _AGENT_ID_JWT_CLAIM = "aid"
 
 _RESPONSE_CHUNK_SIZE = 1024
 
 logger = logging.getLogger(__file__)
 
 
-@pydantic_dataclasses.dataclass
-class LlmSettings:
-    """LLM settings for agents.
-
-    These settings influence how agent responses are generated by the underlying LLM.
-
-    Args:
-        model Optional[str]: The name of the LLM to use.
-            See https://docs.fixie.ai/agents/#agent-default-model-and-model-params for supported
-            values.
-        temperature Optional[float]: The sampling temperature to use, between 0 and 2.
-            Higher values like 0.8 will make the output more random, while lower values like
-            0.2 will make it more focused and deterministic. The precise behavior is
-            model-specific.
-        maximum_tokens Optional[int]: The maximum number of tokens to generate in responses.
-            One token is typically a subword. The exact token definition depends on the model.
-    """
-
-    model: Optional[str] = None
-    temperature: Optional[float] = None
-    maximum_tokens: Optional[int] = None
-
-
-@pydantic_dataclasses.dataclass
-class AgentMetadata:
-    """Metadata for a Fixie CodeShot Agent.
-
-    This will get sent to the Fixie platform upon handshake.
-    """
-
-    base_prompt: str
-    few_shots: List[str]
-    corpora: Optional[List[corpora.DocumentCorpus]] = None
-    conversational: bool = False
-    response_model: Optional[LlmSettings] = None
-
-
-class CodeShotAgent:
-    """A CodeShot agent.
-
-    To make a CodeShot agent, simply pass a BASE_PROMPT and FEW_SHOTS:
-
-        BASE_PROMPT = "A summary of what this agent does; how it does it; and its
-        personality"
-
-        FEW_SHOTS = '''
-        Q: <Sample query that this agent supports>
-        A: <Desired response for this query>
-
-        Q: <Another sample query>
-        A: <Desired response for this query>
-        '''
-
-        agent = CodeShotAgent(BASE_PROMPT, FEW_SHOTS)
-
-    You can have FEW_SHOTS as a single string of all your few-shots separated by 2 new
-    lines, or as an explicit list of one few-shot per index.
-
-    Your few-shots may reach out to other Agents in the fixie ecosystem by
-    "Ask Agent[agent_id]: <query to pass>", or reach out to some python functions
-    by "Ask Func[func_name]: <query to pass>".
-
-    There are a series of default runtime `Func`s provided by the platform available for
-    your agents to consume. For a full list of default runtime `Func`s, refer to:
-        http://docs.fixie.ai/XXX
-
-    You may also need to write your own python functions here to be consumed by your
-    agent. To make a function accessible by an agent, you'd need to register it by
-    `@agent.register_func`. Example:
-
-        @agent.register_func
-        def func_name(query: fixieai.Message) -> ReturnType:
-            ...
-
-        , where ReturnType is one of `str`, `fixieai.Message`, or `fixie.AgentResponse`.
-
-    Note that in the above, we are using the decorator `@agent.register_func` to
-    register this function with the agent instance we just created.
-
-    To check out the default `Func`s that are provided in Fixie, see:
-        http://docs.fixie.ai/XXX
-
-    """
+class AgentBase(abc.ABC):
+    """Base class for Fixie agents."""
 
     def __init__(
         self,
-        base_prompt: str,
-        few_shots: Union[str, List[str]],
-        corpora: Optional[List[corpora.DocumentCorpus]] = None,
-        conversational: bool = False,
         oauth_params: Optional[oauth.OAuthParams] = None,
-        llm_settings: Optional[LlmSettings] = None,
     ):
-        if isinstance(few_shots, str):
-            few_shots = _split_few_shots(few_shots)
-
-        self.base_prompt = base_prompt
-        self.few_shots = few_shots
-        self.corpora = corpora
-        self.conversational = conversational
         self.oauth_params = oauth_params
-        self.llm_settings = llm_settings
         self._funcs: Dict[str, Callable] = {}
         self._jwks_client = jwt.PyJWKClient(constants.FIXIE_JWKS_URL)
         self._allowed_agent_id = os.getenv("FIXIE_ALLOWED_AGENT_ID")
         if self._allowed_agent_id is None:
             warnings.warn(
                 "No allowed agent ID was specified, so your agent will accept requests intended for any agent. "
                 "Ensure that the FIXIE_ALLOWED_AGENT_ID variable is set to correct this."
             )
 
         if oauth_params is not None:
             # Register default Funcs.
             self.register_func(_oauth)
 
-        utils.strip_prompt_lines(self)
+    @abc.abstractmethod
+    def metadata(self) -> agent_metadata.Metadata:
+        """Returns metadata about how the agent should be interacted with."""
+
+    @abc.abstractmethod
+    def validate(self):
+        """Performs any validation after all funcs are registered."""
 
     def serve(self, host: str = "0.0.0.0", port: int = 8181):
         """Starts serving the current agent at `{host}:{port}` via uvicorn.
 
         Args:
             host: The address to start listening at.
             port: The port number to start listening at.
         """
         uvicorn.run(self.app(), host=host, port=port)
 
     def app(self) -> fastapi.FastAPI:
         """Returns a fastapi.FastAPI application that serves the agent."""
         fast_api = fastapi.FastAPI()
         fast_api.include_router(self.api_router())
+
         return fast_api
 
     def api_router(self) -> fastapi.APIRouter:
         """Returns a fastapi.APIRouter object that serves the agent."""
         router = fastapi.APIRouter()
         router.add_api_route("/", self._handshake, methods=["GET"])
         router.add_api_route("/{func_name}", self._serve_func, methods=["POST"])
@@ -222,84 +136,78 @@
     def _handshake(
         self,
         credentials: fastapi.security.HTTPAuthorizationCredentials = fastapi.Depends(
             fastapi.security.HTTPBearer()
         ),
     ) -> fastapi.Response:
         """Returns the agent's metadata in YAML format."""
-        token_claims = _VerifiedTokenClaims.from_token(
+        token_claims = VerifiedTokenClaims.from_token(
             credentials.credentials, self._jwks_client, self._allowed_agent_id
         )
         if token_claims is None:
             raise fastapi.HTTPException(status_code=403, detail="Invalid token")
 
-        metadata = AgentMetadata(
-            self.base_prompt,
-            self.few_shots,
-            self.corpora,
-            self.conversational,
-            self.llm_settings,
-        )
+        metadata = self.metadata()
         yaml_content = yaml.dump(dataclasses.asdict(metadata))
 
-        # Use a streaming response because prompts/fewshots can be very large.
+        # Use a streaming response because metadata can be very large.
         chunks = (
             yaml_content[start : start + _RESPONSE_CHUNK_SIZE]
             for start in range(0, len(yaml_content), _RESPONSE_CHUNK_SIZE)
         )
         return starlette.responses.StreamingResponse(
             chunks,
             media_type="application/yaml",
         )
 
+    def validate_token(
+        self, credentials: fastapi.security.HTTPAuthorizationCredentials
+    ):
+        token_claims = VerifiedTokenClaims.from_token(
+            credentials.credentials, self._jwks_client, self._allowed_agent_id
+        )
+        if token_claims is None:
+            raise fastapi.HTTPException(status_code=403, detail="Invalid token")
+
+        return token_claims
+
     def _serve_func(
         self,
         func_name: str,
         query: api.AgentQuery,
         credentials: fastapi.security.HTTPAuthorizationCredentials = fastapi.Depends(
             fastapi.security.HTTPBearer()
         ),
     ) -> api.AgentResponse:
         """Verifies the request is a valid request from Fixie, and dispatches it to
         the appropriate function.
         """
-        token_claims = _VerifiedTokenClaims.from_token(
-            credentials.credentials, self._jwks_client, self._allowed_agent_id
-        )
-        if token_claims is None:
-            raise fastapi.HTTPException(status_code=403, detail="Invalid token")
-        elif (
-            query.access_token is not None
-            and query.access_token != credentials.credentials
-        ):
-            raise fastapi.HTTPException(status_code=403, detail="Mismatched tokens")
-        else:
-            query.access_token = credentials.credentials
+        token_claims = self.validate_token(credentials)
 
         try:
             pyfunc = self._funcs[func_name]
         except KeyError:
             raise fastapi.HTTPException(
                 status_code=404, detail=f"Func[{func_name}] doesn't exist"
             )
-        kwargs = self._get_func_kwargs(
+        kwargs = self.get_func_kwargs(
             query, token_claims, inspect.signature(pyfunc).parameters.keys()
         )
         output = pyfunc(**kwargs)
         try:
-            return _wrap_with_agent_response(output)
+            return api.AgentResponse.from_value(output)
         except TypeError:
             raise TypeError(
                 f"Func[{func_name}] returned unexpected output of type {type(output)}."
             )
 
-    def _get_func_kwargs(
+    def get_func_kwargs(
         self,
         query: api.AgentQuery,
-        token_claims: _VerifiedTokenClaims,
+        token_claims: VerifiedTokenClaims,
         arg_names: Iterable[str],
     ) -> Dict[str, Any]:
         kwargs: Dict[str, Any] = {}
         for arg_name in arg_names:
             if arg_name == "query":
                 kwargs[arg_name] = query.message
             elif arg_name == "user_storage":
@@ -313,25 +221,25 @@
                 )
             else:
                 raise ValueError(f"Found unknown argument {arg_name!r}.")
         return kwargs
 
 
 @pydantic_dataclasses.dataclass
-class _VerifiedTokenClaims:
+class VerifiedTokenClaims:
     """Verified claims from an agent token."""
 
     agent_id: str
 
     @staticmethod
     def from_token(
         token: str,
         jwks_client: jwt.PyJWKClient,
         expected_agent_id: Optional[str],
-    ) -> Optional[_VerifiedTokenClaims]:
+    ) -> Optional[VerifiedTokenClaims]:
         try:
             public_key = jwks_client.get_signing_key_from_jwt(token)
             claims = jwt.decode(
                 token,
                 public_key.key,
                 algorithms=["EdDSA"],
                 audience=constants.FIXIE_AGENT_API_AUDIENCES,
@@ -348,42 +256,17 @@
         if expected_agent_id is not None and token_agent_id != expected_agent_id:
             # The agent ID in the token did not match the allowed value.
             logger.warning(
                 f"Rejecting valid JWT because agent ID in token ({token_agent_id!r}) did not match {expected_agent_id!r}"
             )
             return None
 
-        return _VerifiedTokenClaims(agent_id=token_agent_id)
+        return VerifiedTokenClaims(agent_id=token_agent_id)
 
 
 def _oauth(query: api.Message, oauth_handler: oauth.OAuthHandler) -> str:
     """Serves Func[_oauth] which is used upon auth redirect callback."""
     auth_request = json.loads(query.text)
     state = auth_request["state"]
     code = auth_request["code"]
     oauth_handler.authorize(state, code)
     return "Authorization successful!"
-
-
-def _wrap_with_agent_response(
-    value: Union[str, api.Message, api.AgentResponse]
-) -> api.AgentResponse:
-    if isinstance(value, str):
-        return api.AgentResponse(api.Message(value))
-    elif isinstance(value, api.Message):
-        return api.AgentResponse(value)
-    elif isinstance(value, api.AgentResponse):
-        return value
-    else:
-        raise TypeError(f"Unexpected type to wrap: {type(value)}")
-
-
-def _split_few_shots(few_shots: str) -> List[str]:
-    """Split a long string of all few-shots into a list of few-shot strings."""
-    # First, strip all lines to remove bad spaces.
-    few_shots = "\n".join(line.strip() for line in few_shots.splitlines())
-    # Then, split by "\n\nQ:".
-    few_shot_splits = few_shots.split("\n\nQ:")
-    few_shot_splits = [few_shot_splits[0]] + [
-        "Q:" + few_shot for few_shot in few_shot_splits[1:]
-    ]
-    return few_shot_splits
```

### Comparing `fixieai-0.2.8/fixieai/agents/oauth.py` & `fixieai-0.2.9/fixieai/agents/oauth.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/agents/user_storage.py` & `fixieai-0.2.9/fixieai/agents/user_storage.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/agents/user_storage_test.py` & `fixieai-0.2.9/fixieai/agents/user_storage_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/agents/utils.py` & `fixieai-0.2.9/fixieai/agents/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import enum
 import inspect
 import re
 from typing import TYPE_CHECKING, Callable, Optional, Set, get_type_hints
 from unittest import mock
 
+from fixieai.agents import agent_base
+
 if TYPE_CHECKING:
     from fixieai.agents import api
     from fixieai.agents import code_shot
 else:
     api = mock.MagicMock()
     code_shot = mock.MagicMock()
 
@@ -29,15 +31,15 @@
     _validate_base_prompt(agent.base_prompt)
     for fewshot in agent.few_shots:
         _validate_few_shot_prompt(
             fewshot, agent.conversational, agent.is_valid_func_name
         )
 
 
-def validate_registered_pyfunc(func: Callable, agent: code_shot.CodeShotAgent):
+def validate_registered_pyfunc(func: Callable, agent: agent_base.AgentBase):
     """Validates `func`'s signature to be a valid CodeShot Func.
 
     Args:
         func: The function to be validated.
         agent: The CodeShotAgent that this func is going to be registered for.
     """
     # Delayed import to avoid circular dependency
```

### Comparing `fixieai-0.2.8/fixieai/agents/utils_test.py` & `fixieai-0.2.9/fixieai/agents/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/agent/agent_config.py` & `fixieai-0.2.9/fixieai/cli/agent/agent_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/agent/commands.py` & `fixieai-0.2.9/fixieai/cli/agent/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -477,21 +477,27 @@
         console.print(f":white_check_mark: {text}")
     except:
         console.print(f":cross_mark: {text}")
         raise
 
 
 def _tarinfo_filter(
-    console: rich_console.Console, root: str, tarinfo: tarfile.TarInfo
+    console: rich_console.Console, root: str, tar_prefix: str, tarinfo: tarfile.TarInfo
 ) -> Optional[tarfile.TarInfo]:
     """Filters out hidden files from being included in a tarball."""
 
-    if os.path.basename(tarinfo.name).startswith("."):
+    basename = os.path.basename(tarinfo.name)
+    if basename.startswith(".") and basename != ".env":
+        original_path = tarinfo.name
+        if original_path.startswith(tar_prefix):
+            original_path = original_path[len(tar_prefix) :]
+
+        original_path = os.path.join(root, original_path)
         console.print(
-            f"Ignoring hidden {'directory' if tarinfo.isdir() else 'file'} {os.path.join(root, tarinfo.name)}",
+            f"Ignoring hidden {'directory' if tarinfo.isdir() else 'file'} {original_path}",
             style="grey53",
         )
         return None
     else:
         return tarinfo
 
 
@@ -537,15 +543,17 @@
     if config.deployment_url is None and not metadata_only:
         # Deploy the agent to fixie with some bootstrapping code.
         with tempfile.TemporaryFile() as tarball_file:
             with tarfile.open(fileobj=tarball_file, mode="w:gz") as tarball:
                 tarball.add(
                     agent_dir,
                     arcname="agent",
-                    filter=functools.partial(_tarinfo_filter, console, agent_dir),
+                    filter=functools.partial(
+                        _tarinfo_filter, console, agent_dir, "agent/"
+                    ),
                 )
 
                 # Add the bootstrapping code and environment variables
                 _add_text_file_to_tarfile(
                     "main.py", _DEPLOYMENT_BOOTSTRAP_SOURCE, tarball
                 )
                 _add_text_file_to_tarfile(
```

### Comparing `fixieai-0.2.8/fixieai/cli/agent/commands_test.py` & `fixieai-0.2.9/fixieai/cli/agent/commands_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/agent/loader.py` & `fixieai-0.2.9/fixieai/cli/agent/loader.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,56 +3,64 @@
 import importlib
 import os
 import sys
 import threading
 import time
 from typing import Tuple
 
+import dotenv
+
 import fixieai
 from fixieai import agents
-from fixieai.agents import utils
 from fixieai.cli.agent import agent_config
 
 
 @contextlib.contextmanager
 def _ensure_serving_disabled():
-    original_serve = agents.CodeShotAgent.serve
+    original_serve = agents.AgentBase.serve
 
     def _fail(*_, **__):
         raise RuntimeError(
             "agent.serve() must not be called while your agent is being imported."
         )
 
-    agents.CodeShotAgent.serve = _fail  # type: ignore[assignment]
+    agents.AgentBase.serve = _fail  # type: ignore[assignment]
     try:
         yield
     finally:
-        agents.CodeShotAgent.serve = original_serve  # type: ignore[assignment]
+        agents.AgentBase.serve = original_serve  # type: ignore[assignment]
 
 
 def load_agent_from_path(
     path: str,
-) -> Tuple[agent_config.AgentConfig, agents.CodeShotAgent]:
+) -> Tuple[agent_config.AgentConfig, agents.AgentBase]:
     """Loads an Agent and its config from a path."""
 
     path = agent_config.normalize_path(path)
     config = agent_config.load_config(path)
     agent_dir = os.path.dirname(path) or "."
 
+    dotenv_path = os.path.join(agent_dir, ".env")
+    if os.path.exists(dotenv_path):
+        dotenv.load_dotenv(dotenv_path)
+
     # Inject the agent directory into PYTHONPATH
     sys.path.insert(0, agent_dir)
 
     entry_point_parts = config.entry_point.split(":", 1)
     module_name = entry_point_parts[0]
     attr = entry_point_parts[1] if len(entry_point_parts) == 2 else "agent"
 
     with _ensure_serving_disabled():
         module = importlib.import_module(module_name)
     agent_impl = getattr(module, attr)
-    utils.validate_code_shot_agent(agent_impl)
+    assert isinstance(
+        agent_impl, agents.AgentBase
+    ), "Entrypoint must refer to an agent instance"
+    agent_impl.validate()
     return config, agent_impl
 
 
 def _refresh_agent_async(agent_handle: str):
     """Asynchronously pings Fixie to refresh the given agent_id."""
 
     def _refresh_agent_sync():
```

### Comparing `fixieai-0.2.8/fixieai/cli/agent/tunnel.py` & `fixieai-0.2.9/fixieai/cli/agent/tunnel.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/auth/commands.py` & `fixieai-0.2.9/fixieai/cli/auth/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/auth/oauth_flow.py` & `fixieai-0.2.9/fixieai/cli/auth/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/auth/user_config.py` & `fixieai-0.2.9/fixieai/cli/auth/user_config.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/auth/user_config_test.py` & `fixieai-0.2.9/fixieai/cli/auth/user_config_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/cli.py` & `fixieai-0.2.9/fixieai/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/session/commands.py` & `fixieai-0.2.9/fixieai/cli/session/commands.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/session/console.py` & `fixieai-0.2.9/fixieai/cli/session/console.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/utils.py` & `fixieai-0.2.9/fixieai/cli/utils.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/cli/utils_test.py` & `fixieai-0.2.9/fixieai/cli/utils_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/client/agent.py` & `fixieai-0.2.9/fixieai/client/agent.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/client/client.py` & `fixieai-0.2.9/fixieai/client/client.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/client/client_test.py` & `fixieai-0.2.9/fixieai/client/client_test.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/client/session.py` & `fixieai-0.2.9/fixieai/client/session.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/fixieai/constants.py` & `fixieai-0.2.9/fixieai/constants.py`

 * *Files identical despite different names*

### Comparing `fixieai-0.2.8/pyproject.toml` & `fixieai-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fixieai"
-version = "0.2.8"
+version = "0.2.9"
 description = "SDK for the Fixie.ai platform. See: https://fixie.ai"
 authors = ["Fixie.ai Team <hello@fixie.ai>"]
 packages = [
     { include = "fixieai/" },
 ]
 
 [build-system]
```

### Comparing `fixieai-0.2.8/setup.py` & `fixieai-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 entry_points = \
 {'console_scripts': ['fixie = fixieai.cli.cli:fixie',
                      'fixieai = fixieai.cli.cli:fixie']}
 
 setup_kwargs = {
     'name': 'fixieai',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'SDK for the Fixie.ai platform. See: https://fixie.ai',
     'long_description': 'None',
     'author': 'Fixie.ai Team',
     'author_email': 'hello@fixie.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `fixieai-0.2.8/PKG-INFO` & `fixieai-0.2.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixieai
-Version: 0.2.8
+Version: 0.2.9
 Summary: SDK for the Fixie.ai platform. See: https://fixie.ai
 Author: Fixie.ai Team
 Author-email: hello@fixie.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

