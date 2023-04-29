# Comparing `tmp/turbo_chat-0.3.8.tar.gz` & `tmp/turbo_chat-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_chat-0.3.8.tar", max compression
+gzip compressed data, was "turbo_chat-0.3.9.tar", max compression
```

## Comparing `turbo_chat-0.3.8.tar` & `turbo_chat-0.3.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1075 2023-03-27 06:50:49.642216 turbo_chat-0.3.8/LICENSE
--rw-r--r--   0        0        0    10839 2023-04-12 08:40:24.985314 turbo_chat-0.3.8/README.md
--rw-r--r--   0        0        0     1276 2023-04-18 05:27:54.501699 turbo_chat-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      898 2023-04-05 05:13:21.209711 turbo_chat-0.3.8/turbo_chat/__init__.py
--rw-r--r--   0        0        0      237 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/__init__.py
--rw-r--r--   0        0        0      520 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/qa.py
--rw-r--r--   0        0        0     1377 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/self_ask.py
--rw-r--r--   0        0        0       72 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/subqueries/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/subqueries/bot.py
--rw-r--r--   0        0        0      636 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/subqueries/scratchpad.py
--rw-r--r--   0        0        0     1747 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/subqueries/template.py
--rw-r--r--   0        0        0      422 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/summarize.py
--rw-r--r--   0        0        0       66 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/tool/__init__.py
--rw-r--r--   0        0        0     4270 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/tool/bot.py
--rw-r--r--   0        0        0      426 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/tool/scratchpad.py
--rw-r--r--   0        0        0     2940 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/bots/tool/template.py
--rw-r--r--   0        0        0      154 2023-04-05 05:13:21.209711 turbo_chat-0.3.8/turbo_chat/cache/__init__.py
--rw-r--r--   0        0        0     1489 2023-04-12 03:09:32.852539 turbo_chat-0.3.8/turbo_chat/cache/redis.py
--rw-r--r--   0        0        0      638 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/cache/simple.py
--rw-r--r--   0        0        0     1303 2023-04-12 08:29:36.369017 turbo_chat-0.3.8/turbo_chat/chat.py
--rw-r--r--   0        0        0     1629 2023-04-18 05:26:08.284295 turbo_chat-0.3.8/turbo_chat/completion.py
--rw-r--r--   0        0        0      446 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/config.py
--rw-r--r--   0        0        0      488 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/errors.py
--rw-r--r--   0        0        0      239 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/memory/__init__.py
--rw-r--r--   0        0        0      788 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/memory/local_memory.py
--rw-r--r--   0        0        0     1358 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/memory/summary_memory.py
--rw-r--r--   0        0        0     1604 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/memory/truncated_memory.py
--rw-r--r--   0        0        0      796 2023-04-11 16:57:02.142061 turbo_chat-0.3.8/turbo_chat/runner.py
--rw-r--r--   0        0        0      356 2023-03-27 09:35:21.119756 turbo_chat-0.3.8/turbo_chat/structs/__init__.py
--rw-r--r--   0        0        0     1198 2023-03-30 10:03:00.267473 turbo_chat-0.3.8/turbo_chat/structs/messages.py
--rw-r--r--   0        0        0      968 2023-03-28 17:49:03.767496 turbo_chat-0.3.8/turbo_chat/structs/proxies.py
--rw-r--r--   0        0        0      795 2023-03-29 09:31:03.306136 turbo_chat-0.3.8/turbo_chat/structs/result.py
--rw-r--r--   0        0        0     1567 2023-04-05 05:13:21.209711 turbo_chat-0.3.8/turbo_chat/structs/scratchpad.py
--rw-r--r--   0        0        0      495 2023-03-29 07:56:38.680320 turbo_chat-0.3.8/turbo_chat/structs/signals.py
--rw-r--r--   0        0        0     6300 2023-04-18 05:25:42.419987 turbo_chat-0.3.8/turbo_chat/turbo.py
--rw-r--r--   0        0        0      360 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/types/__init__.py
--rw-r--r--   0        0        0      770 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/types/cache.py
--rw-r--r--   0        0        0      855 2023-04-12 06:52:00.686614 turbo_chat-0.3.8/turbo_chat/types/generators.py
--rw-r--r--   0        0        0     3387 2023-03-30 10:03:00.267473 turbo_chat-0.3.8/turbo_chat/types/memory.py
--rw-r--r--   0        0        0     3029 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/types/messages.py
--rw-r--r--   0        0        0       74 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/types/misc.py
--rw-r--r--   0        0        0      218 2023-04-18 05:20:03.611062 turbo_chat-0.3.8/turbo_chat/types/tools.py
--rw-r--r--   0        0        0      300 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/utils/__init__.py
--rw-r--r--   0        0        0     1111 2023-04-03 13:40:06.231883 turbo_chat-0.3.8/turbo_chat/utils/args.py
--rw-r--r--   0        0        0  1681126 2023-04-12 06:17:06.606268 turbo_chat-0.3.8/turbo_chat/utils/cl100k_base.tiktoken
--rw-r--r--   0        0        0     2589 2023-04-12 08:29:36.373017 turbo_chat-0.3.8/turbo_chat/utils/debug.py
--rw-r--r--   0        0        0      425 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/utils/fn.py
--rw-r--r--   0        0        0      137 2023-03-27 09:38:54.782616 turbo_chat-0.3.8/turbo_chat/utils/lang.py
--rw-r--r--   0        0        0      343 2023-04-12 08:29:36.373017 turbo_chat-0.3.8/turbo_chat/utils/pprint.py
--rw-r--r--   0        0        0     1110 2023-03-27 06:50:49.646216 turbo_chat-0.3.8/turbo_chat/utils/retries.py
--rw-r--r--   0        0        0     1029 2023-04-03 13:40:06.231883 turbo_chat-0.3.8/turbo_chat/utils/template.py
--rw-r--r--   0        0        0     3711 2023-04-12 06:17:06.610268 turbo_chat-0.3.8/turbo_chat/utils/tokens.py
--rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 turbo_chat-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-27 06:50:49.642216 turbo_chat-0.3.9/LICENSE
+-rw-r--r--   0        0        0    11087 2023-04-18 12:26:11.529952 turbo_chat-0.3.9/README.md
+-rw-r--r--   0        0        0     1276 2023-04-18 12:26:11.533952 turbo_chat-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      898 2023-04-05 05:13:21.209711 turbo_chat-0.3.9/turbo_chat/__init__.py
+-rw-r--r--   0        0        0      237 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/__init__.py
+-rw-r--r--   0        0        0      520 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/qa.py
+-rw-r--r--   0        0        0     1377 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/self_ask.py
+-rw-r--r--   0        0        0       72 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/subqueries/__init__.py
+-rw-r--r--   0        0        0     1887 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/subqueries/bot.py
+-rw-r--r--   0        0        0      636 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/subqueries/scratchpad.py
+-rw-r--r--   0        0        0     1747 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/subqueries/template.py
+-rw-r--r--   0        0        0      422 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/summarize.py
+-rw-r--r--   0        0        0       66 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/tool/__init__.py
+-rw-r--r--   0        0        0     4270 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/tool/bot.py
+-rw-r--r--   0        0        0      426 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/tool/scratchpad.py
+-rw-r--r--   0        0        0     2940 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/bots/tool/template.py
+-rw-r--r--   0        0        0      154 2023-04-05 05:13:21.209711 turbo_chat-0.3.9/turbo_chat/cache/__init__.py
+-rw-r--r--   0        0        0     1489 2023-04-12 03:09:32.852539 turbo_chat-0.3.9/turbo_chat/cache/redis.py
+-rw-r--r--   0        0        0      638 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/cache/simple.py
+-rw-r--r--   0        0        0     1303 2023-04-12 08:29:36.369017 turbo_chat-0.3.9/turbo_chat/chat.py
+-rw-r--r--   0        0        0     1629 2023-04-18 11:53:42.338944 turbo_chat-0.3.9/turbo_chat/completion.py
+-rw-r--r--   0        0        0      446 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/config.py
+-rw-r--r--   0        0        0      488 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/errors.py
+-rw-r--r--   0        0        0      239 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/memory/__init__.py
+-rw-r--r--   0        0        0      788 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/memory/local_memory.py
+-rw-r--r--   0        0        0     1358 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/memory/summary_memory.py
+-rw-r--r--   0        0        0     1604 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/memory/truncated_memory.py
+-rw-r--r--   0        0        0      796 2023-04-11 16:57:02.142061 turbo_chat-0.3.9/turbo_chat/runner.py
+-rw-r--r--   0        0        0      356 2023-03-27 09:35:21.119756 turbo_chat-0.3.9/turbo_chat/structs/__init__.py
+-rw-r--r--   0        0        0     1198 2023-03-30 10:03:00.267473 turbo_chat-0.3.9/turbo_chat/structs/messages.py
+-rw-r--r--   0        0        0      968 2023-03-28 17:49:03.767496 turbo_chat-0.3.9/turbo_chat/structs/proxies.py
+-rw-r--r--   0        0        0      795 2023-03-29 09:31:03.306136 turbo_chat-0.3.9/turbo_chat/structs/result.py
+-rw-r--r--   0        0        0     1567 2023-04-05 05:13:21.209711 turbo_chat-0.3.9/turbo_chat/structs/scratchpad.py
+-rw-r--r--   0        0        0      495 2023-03-29 07:56:38.680320 turbo_chat-0.3.9/turbo_chat/structs/signals.py
+-rw-r--r--   0        0        0     6311 2023-04-18 12:26:11.533952 turbo_chat-0.3.9/turbo_chat/turbo.py
+-rw-r--r--   0        0        0      360 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/types/__init__.py
+-rw-r--r--   0        0        0      770 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/types/cache.py
+-rw-r--r--   0        0        0      855 2023-04-12 06:52:00.686614 turbo_chat-0.3.9/turbo_chat/types/generators.py
+-rw-r--r--   0        0        0     3387 2023-03-30 10:03:00.267473 turbo_chat-0.3.9/turbo_chat/types/memory.py
+-rw-r--r--   0        0        0     3029 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/types/messages.py
+-rw-r--r--   0        0        0       74 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/types/misc.py
+-rw-r--r--   0        0        0      218 2023-04-18 05:20:03.611062 turbo_chat-0.3.9/turbo_chat/types/tools.py
+-rw-r--r--   0        0        0      300 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/utils/__init__.py
+-rw-r--r--   0        0        0     1111 2023-04-03 13:40:06.231883 turbo_chat-0.3.9/turbo_chat/utils/args.py
+-rw-r--r--   0        0        0  1681126 2023-04-12 06:17:06.606268 turbo_chat-0.3.9/turbo_chat/utils/cl100k_base.tiktoken
+-rw-r--r--   0        0        0     2589 2023-04-12 08:29:36.373017 turbo_chat-0.3.9/turbo_chat/utils/debug.py
+-rw-r--r--   0        0        0      425 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/utils/fn.py
+-rw-r--r--   0        0        0      137 2023-03-27 09:38:54.782616 turbo_chat-0.3.9/turbo_chat/utils/lang.py
+-rw-r--r--   0        0        0      343 2023-04-12 08:29:36.373017 turbo_chat-0.3.9/turbo_chat/utils/pprint.py
+-rw-r--r--   0        0        0     1110 2023-03-27 06:50:49.646216 turbo_chat-0.3.9/turbo_chat/utils/retries.py
+-rw-r--r--   0        0        0     1029 2023-04-03 13:40:06.231883 turbo_chat-0.3.9/turbo_chat/utils/template.py
+-rw-r--r--   0        0        0     3711 2023-04-12 06:17:06.610268 turbo_chat-0.3.9/turbo_chat/utils/tokens.py
+-rw-r--r--   0        0        0    12378 1970-01-01 00:00:00.000000 turbo_chat-0.3.9/PKG-INFO
```

### Comparing `turbo_chat-0.3.8/LICENSE` & `turbo_chat-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/README.md` & `turbo_chat-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -179,14 +179,16 @@
 
 ```
 
 ---
 
 ### Latest Changes
 
+* version: 0.3.9. PR [#59](https://github.com/creatorrr/turbo-chat/pull/59) by [@creatorrr](https://github.com/creatorrr).
+* x/fix cache args. PR [#58](https://github.com/creatorrr/turbo-chat/pull/58) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.7. PR [#57](https://github.com/creatorrr/turbo-chat/pull/57) by [@creatorrr](https://github.com/creatorrr).
 * f/support multi choice. PR [#56](https://github.com/creatorrr/turbo-chat/pull/56) by [@creatorrr](https://github.com/creatorrr).
 * feat: Support multiple choices selector; n > 1. PR [#55](https://github.com/creatorrr/turbo-chat/pull/55) by [@creatorrr](https://github.com/creatorrr).
 * feat: Support positional arguments for running apps. PR [#54](https://github.com/creatorrr/turbo-chat/pull/54) by [@creatorrr](https://github.com/creatorrr).
 * feat: Make get_encoding faster. PR [#53](https://github.com/creatorrr/turbo-chat/pull/53) by [@creatorrr](https://github.com/creatorrr).
 * feat: Add ttl support to redis_cache. PR [#52](https://github.com/creatorrr/turbo-chat/pull/52) by [@creatorrr](https://github.com/creatorrr).
 * feat: Support for parsing completions. PR [#51](https://github.com/creatorrr/turbo-chat/pull/51) by [@creatorrr](https://github.com/creatorrr).
```

### Comparing `turbo_chat-0.3.8/pyproject.toml` & `turbo_chat-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "turbo-chat"
-version = "0.3.8"
+version = "0.3.9"
 description = "Idiomatic way to build chatgpt apps using async generators in python"
 authors = ["Diwank Singh Tomer <singh@diwank.name>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "turbo_chat"}]
 
 [tool.poetry.dependencies]
```

### Comparing `turbo_chat-0.3.8/turbo_chat/__init__.py` & `turbo_chat-0.3.9/turbo_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/qa.py` & `turbo_chat-0.3.9/turbo_chat/bots/qa.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/self_ask.py` & `turbo_chat-0.3.9/turbo_chat/bots/self_ask.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/subqueries/bot.py` & `turbo_chat-0.3.9/turbo_chat/bots/subqueries/bot.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/subqueries/scratchpad.py` & `turbo_chat-0.3.9/turbo_chat/bots/subqueries/scratchpad.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/subqueries/template.py` & `turbo_chat-0.3.9/turbo_chat/bots/subqueries/template.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/tool/bot.py` & `turbo_chat-0.3.9/turbo_chat/bots/tool/bot.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/bots/tool/template.py` & `turbo_chat-0.3.9/turbo_chat/bots/tool/template.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/cache/redis.py` & `turbo_chat-0.3.9/turbo_chat/cache/redis.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/cache/simple.py` & `turbo_chat-0.3.9/turbo_chat/cache/simple.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/chat.py` & `turbo_chat-0.3.9/turbo_chat/chat.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/completion.py` & `turbo_chat-0.3.9/turbo_chat/completion.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/memory/local_memory.py` & `turbo_chat-0.3.9/turbo_chat/memory/local_memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/memory/summary_memory.py` & `turbo_chat-0.3.9/turbo_chat/memory/summary_memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/memory/truncated_memory.py` & `turbo_chat-0.3.9/turbo_chat/memory/truncated_memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/runner.py` & `turbo_chat-0.3.9/turbo_chat/runner.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/structs/messages.py` & `turbo_chat-0.3.9/turbo_chat/structs/messages.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/structs/proxies.py` & `turbo_chat-0.3.9/turbo_chat/structs/proxies.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/structs/result.py` & `turbo_chat-0.3.9/turbo_chat/structs/result.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/structs/scratchpad.py` & `turbo_chat-0.3.9/turbo_chat/structs/scratchpad.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/turbo.py` & `turbo_chat-0.3.9/turbo_chat/turbo.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,39 +92,40 @@
         async def turbo_gen_fn(*args, **kwargs) -> TurboGenWrapper:
             """Wrapped chatml app from an async generator"""
 
             # Get cache and memory args
             cache_args = kwargs.pop("cache_args", {})
             memory_args = kwargs.pop("memory_args", {})
 
-            params = inspect.signature(original_fn or gen_fn).bind(*args, **kwargs)
-            context = params.arguments
+            # Prepare kwargs
+            signature = inspect.signature(original_fn or gen_fn)
+            arg_names = [k for k in signature.parameters.keys()]
 
             # Init memory
             memory = memory_class(model=model)
             assert ensure_args(memory.setup, memory_args)
             await memory.setup(**memory_args)
 
             # Init cache
             cache = None
             if cache_class:
                 cache = cache_class()
                 assert ensure_args(cache.setup, cache_args)
                 await cache.setup(**cache_args)
 
-            # Init generator
-            signature = inspect.signature(gen_fn)
-            arg_names = [k for k in signature.parameters.keys()]
-
             if "memory" in arg_names:
-                context["memory"] = memory
+                kwargs["memory"] = memory
 
             if "cache" in arg_names:
-                context["cache"] = cache
+                kwargs["cache"] = cache
+
+            params = signature.bind(*args, **kwargs)
+            context = params.arguments
 
+            # Init generator
             turbo_gen = gen_fn(**context)
 
             # Parameters
             payload: Any = None
 
             # Yield Start() to indicate start
             yield Start()
```

### Comparing `turbo_chat-0.3.8/turbo_chat/types/cache.py` & `turbo_chat-0.3.9/turbo_chat/types/cache.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/types/generators.py` & `turbo_chat-0.3.9/turbo_chat/types/generators.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/types/memory.py` & `turbo_chat-0.3.9/turbo_chat/types/memory.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/types/messages.py` & `turbo_chat-0.3.9/turbo_chat/types/messages.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/utils/args.py` & `turbo_chat-0.3.9/turbo_chat/utils/args.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/utils/cl100k_base.tiktoken` & `turbo_chat-0.3.9/turbo_chat/utils/cl100k_base.tiktoken`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/utils/debug.py` & `turbo_chat-0.3.9/turbo_chat/utils/debug.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/utils/retries.py` & `turbo_chat-0.3.9/turbo_chat/utils/retries.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/utils/template.py` & `turbo_chat-0.3.9/turbo_chat/utils/template.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/turbo_chat/utils/tokens.py` & `turbo_chat-0.3.9/turbo_chat/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `turbo_chat-0.3.8/PKG-INFO` & `turbo_chat-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-chat
-Version: 0.3.8
+Version: 0.3.9
 Summary: Idiomatic way to build chatgpt apps using async generators in python
 License: MIT
 Author: Diwank Singh Tomer
 Author-email: singh@diwank.name
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -212,14 +212,16 @@
 
 ```
 
 ---
 
 ### Latest Changes
 
+* version: 0.3.9. PR [#59](https://github.com/creatorrr/turbo-chat/pull/59) by [@creatorrr](https://github.com/creatorrr).
+* x/fix cache args. PR [#58](https://github.com/creatorrr/turbo-chat/pull/58) by [@creatorrr](https://github.com/creatorrr).
 * version: 0.3.7. PR [#57](https://github.com/creatorrr/turbo-chat/pull/57) by [@creatorrr](https://github.com/creatorrr).
 * f/support multi choice. PR [#56](https://github.com/creatorrr/turbo-chat/pull/56) by [@creatorrr](https://github.com/creatorrr).
 * feat: Support multiple choices selector; n > 1. PR [#55](https://github.com/creatorrr/turbo-chat/pull/55) by [@creatorrr](https://github.com/creatorrr).
 * feat: Support positional arguments for running apps. PR [#54](https://github.com/creatorrr/turbo-chat/pull/54) by [@creatorrr](https://github.com/creatorrr).
 * feat: Make get_encoding faster. PR [#53](https://github.com/creatorrr/turbo-chat/pull/53) by [@creatorrr](https://github.com/creatorrr).
 * feat: Add ttl support to redis_cache. PR [#52](https://github.com/creatorrr/turbo-chat/pull/52) by [@creatorrr](https://github.com/creatorrr).
 * feat: Support for parsing completions. PR [#51](https://github.com/creatorrr/turbo-chat/pull/51) by [@creatorrr](https://github.com/creatorrr).
```

