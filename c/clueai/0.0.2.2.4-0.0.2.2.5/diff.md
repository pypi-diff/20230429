# Comparing `tmp/clueai-0.0.2.2.4.tar.gz` & `tmp/clueai-0.0.2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clueai-0.0.2.2.4.tar", last modified: Wed Feb 15 03:28:37 2023, max compression
+gzip compressed data, was "clueai-0.0.2.2.5.tar", last modified: Sat Apr 29 06:34:49 2023, max compression
```

## Comparing `clueai-0.0.2.2.4.tar` & `clueai-0.0.2.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-02-15 03:28:37.012485 clueai-0.0.2.2.4/
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1063 2022-08-18 02:23:35.000000 clueai-0.0.2.2.4/LICENSE
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    50773 2023-02-15 03:28:37.012085 clueai-0.0.2.2.4/PKG-INFO
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    41384 2023-02-15 03:11:47.000000 clueai-0.0.2.2.4/README.md
-drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-02-15 03:28:37.001843 clueai-0.0.2.2.4/clueai/
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      409 2022-11-24 03:00:20.000000 clueai-0.0.2.2.4/clueai/__init__.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1010 2022-08-18 02:13:51.000000 clueai-0.0.2.2.4/clueai/classify.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    20795 2023-02-14 12:41:58.000000 clueai-0.0.2.2.4/clueai/client.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      371 2022-08-18 02:13:51.000000 clueai-0.0.2.2.4/clueai/embeddings.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      591 2022-08-19 06:26:56.000000 clueai-0.0.2.2.4/clueai/error.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     2791 2022-08-18 02:13:51.000000 clueai-0.0.2.2.4/clueai/extract.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1007 2022-08-18 02:13:51.000000 clueai-0.0.2.2.4/clueai/generation.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      771 2022-09-26 12:05:13.000000 clueai-0.0.2.2.4/clueai/match.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      685 2022-11-25 06:40:19.000000 clueai-0.0.2.2.4/clueai/qa.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      337 2022-08-18 02:13:51.000000 clueai-0.0.2.2.4/clueai/response.py
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      434 2022-08-18 02:13:51.000000 clueai-0.0.2.2.4/clueai/tokenize.py
-drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-02-15 03:28:37.010125 clueai-0.0.2.2.4/clueai.egg-info/
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)    50773 2023-02-15 03:28:36.000000 clueai-0.0.2.2.4/clueai.egg-info/PKG-INFO
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)      373 2023-02-15 03:28:36.000000 clueai-0.0.2.2.4/clueai.egg-info/SOURCES.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)        1 2023-02-15 03:28:36.000000 clueai-0.0.2.2.4/clueai.egg-info/dependency_links.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)       16 2023-02-15 03:28:36.000000 clueai-0.0.2.2.4/clueai.egg-info/requires.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)        7 2023-02-15 03:28:36.000000 clueai-0.0.2.2.4/clueai.egg-info/top_level.txt
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)       38 2023-02-15 03:28:37.012661 clueai-0.0.2.2.4/setup.cfg
--rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1256 2023-02-15 03:28:25.000000 clueai-0.0.2.2.4/setup.py
+drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:34:49.933634 clueai-0.0.2.2.5/
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1063 2022-08-18 02:23:35.000000 clueai-0.0.2.2.5/LICENSE
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    53110 2023-04-29 06:34:49.931882 clueai-0.0.2.2.5/PKG-INFO
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    43545 2023-04-29 06:33:53.000000 clueai-0.0.2.2.5/README.md
+drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:34:49.875434 clueai-0.0.2.2.5/clueai/
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      409 2022-11-24 03:00:20.000000 clueai-0.0.2.2.5/clueai/__init__.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1010 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/classify.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    20817 2023-04-29 06:34:10.000000 clueai-0.0.2.2.5/clueai/client.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      371 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/embeddings.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      591 2022-08-19 06:26:56.000000 clueai-0.0.2.2.5/clueai/error.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     2791 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/extract.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1007 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/generation.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      771 2022-09-26 12:05:13.000000 clueai-0.0.2.2.5/clueai/match.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      685 2022-11-25 06:40:19.000000 clueai-0.0.2.2.5/clueai/qa.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      337 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/response.py
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      434 2022-08-18 02:13:51.000000 clueai-0.0.2.2.5/clueai/tokenize.py
+drwxr-xr-x   0 zhangxuanwei   (501) staff       (20)        0 2023-04-29 06:34:49.923195 clueai-0.0.2.2.5/clueai.egg-info/
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)    53110 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/PKG-INFO
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)      373 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)        1 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)       16 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/requires.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)        7 2023-04-29 06:34:49.000000 clueai-0.0.2.2.5/clueai.egg-info/top_level.txt
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)       38 2023-04-29 06:34:49.933846 clueai-0.0.2.2.5/setup.cfg
+-rw-r--r--   0 zhangxuanwei   (501) staff       (20)     1256 2023-04-29 06:34:34.000000 clueai-0.0.2.2.5/setup.py
```

### Comparing `clueai-0.0.2.2.4/LICENSE` & `clueai-0.0.2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/PKG-INFO` & `clueai-0.0.2.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clueai
-Version: 0.0.2.2.4
+Version: 0.0.2.2.5
 Summary: A Python library for the ClueAI API
 Home-page: https://github.com/clue-ai/clueai-python
 Author: matrix
 Author-email: brightmart@hotmail.com
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -54,18 +54,24 @@
             - [文本分类](#文本分类)
             - [文本生成](#文本生成-1)
         - [生成参数说明](#生成参数说明)
         - [查看调用使用量](#查看调用使用量)
         - [模型介绍](#模型介绍)
         - [返回结果](#返回结果)
         - [问题反馈和技术交流](#问题反馈和技术交流)
-        
-        ### 更新 Update 2023-02-03(新)
+        ### 更新 Update 2023-03-23(新)
+        [ChatYuan开源模型](https://github.com/clue-ai/ChatYuan)大升级
+        ### 更新 Update 2023-02-15
+        新增模型ChatYuan微调功能：[模型微调](#模型微调) [上传库-启动-调用](#上传库-启动-调用)  
+        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=jctvm0fxMwEY)
+        ### 更新 Update 2023-02-03
         新增ChatYuan功能对话：  [ChatYuan功能对话](#ChatYuan功能对话)
-        ### 更新 Update 2022-11-25(新)
+        ### 更新 Update 2023-01-15
+        [ChatYuan开源模型](https://github.com/clue-ai/ChatYuan)
+        ### 更新 Update 2022-11-25
         新增智能文档问答生成：  [智能文档问答生成](#智能文档问答生成)
         #### 更新 Update 2022-11-09
         新增模型微调功能：[模型微调](#模型微调) [上传库-启动-调用](#上传库-启动-调用)
         #### 更新 Update 2022-09-29
         PromptCLUE: 中文多任务Prompt预训练模型，已经开源！<a href='https://github.com/clue-ai/PromptCLUE'>github项目地址</a> | <a href='https://huggingface.co/ClueAI/PromptCLUE'>模型下载</a>
         
         ## Python 软件包
@@ -125,16 +131,22 @@
         
         ##### 单轮对话
         ```python
         import clueai
         
         # initialize the Clueai Client with an API Key
         cl = clueai.Client('YOUR_API_KEY', check_api_key=True)
+        # 注意'''的用法，如果换行后，下一行前不要加空格，要顶格写, （不需要和上文对齐），不熟悉'''的用法，请使用"的字符串
+        """
         prompt= '''用户：介绍一下亚马逊云的历史
         小元：'''
+        """
+        # "用法的示例，使用\n来拼成一行
+        prompt = "用户：介绍一下亚马逊云的历史\n小元："
+        
         
         # generate a prediction for a prompt 
         # 需要返回得分的话，指定return_likelihoods="GENERATION"
         prediction = cl.generate(
                     model_name='ChatYuan-large',
                     prompt=prompt)
                     
@@ -144,20 +156,26 @@
         
         ##### 多轮对话
         ```python
         import clueai
         
         # initialize the Clueai Client with an API Key
         cl = clueai.Client('YOUR_API_KEY', check_api_key=True)
+        # 注意'''的用法，如果换行后，下一行前不要加空格，要顶格写, （不需要和上文对齐）, 不熟悉'''的用法，请使用"的字符串
+        """
         prompt= '''用户：新冠什么症状？
         小元：新冠是指新型冠状病毒，其症状包括发热、干咳、乏力、嗅味觉减退、呼吸困难等。
         用户：可以吃什么药？
         小元：根据您提供的病史，目前没有明确的抗新冠病毒的药物，建议您在家进行自我隔离，避免与他人接触，多喝开水，清淡易消化饮食，避免熬夜和过度劳累，适当进行户外活动。
         用户：帮我写一个2023年工作规划
         小元：'''
+        """
+        # "用法的示例，使用\n来拼成一行
+        prompt = "用户：新冠什么症状？\n小元：新冠是指新型冠状病毒，其症状包括发热、干咳、乏力、嗅味觉减退、呼吸困难等。\n用户：可以吃什么药？\n小元：根据您提供的病史，目前没有明确的抗新冠病毒的药物，建议您在家进行自我隔离，避免与他人接触，多喝开水，清淡易消化饮食，避免熬夜和过度劳累，适当进行户外活动。\n用户：帮我写一个2023年工作规划\n小元："
+        
         
         # generate a prediction for a prompt 
         # 需要返回得分的话，指定return_likelihoods="GENERATION"
         prediction = cl.generate(
                     model_name='ChatYuan-large',
                     prompt=prompt)
                     
@@ -349,20 +367,24 @@
         </tr>
         </table>
         
         ### 模型微调
         #### 上传库-启动-调用
         说明：
         1. 上传需要微调的数据，自动训练微调/部署模型，提供接口使用
-        2. 上传的数据为json格式，参考./examples/finetune_train_examples.json
+        2. 上传的数据为json格式，PromptCLUE参考./examples/finetune_train_examples.json, ChatYuan参考./examples/qa_test.json
         3. 基于promptCLUE模型微调，建议参考prompt提示的格式构建数据集，效果会更好，prompt格式可以参考下面[示例输入](#示例输入)的形式
-        4. 需要有个API key， 并且在创建`clueai.Client`对象时需要指定这个API key. API key 可以通过这个[平台](https://www.clueai.cn/)获得，方法： 点击[官网](https://www.clueai.cn/)右上角立即使用-注册登陆后-右上角有创建apikey-创建apikey
-        5. 微调数据数量限制1w条，超过会被采样，如果需要微调更大数量请与我们联系，联系方式见最下方
-        6. 完整代码可参考：[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9)
-        7. 默认启动模型推理服务后，会保持10分钟，超时会断开
+        4. 如果是基于ChatYuan微调的话，可以参考[示例格式](https://github.com/clue-ai/clueai-python/blob/main/examples/qa_test.json)，也可以参考[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=jctvm0fxMwEY)  
+           a. 输入为json格式, 包含两个字段input和output（字段名字可以自己指定）   
+           b. input的内容可以是"用户：+内容+\n小元："的格式，也可以直接是"内容"的格式  
+           c. output的内容直接是你想模型输出的结果内容即可
+        5. 需要有个API key， 并且在创建`clueai.Client`对象时需要指定这个API key. API key 可以通过这个[平台](https://www.clueai.cn/)获得，方法： 点击[官网](https://www.clueai.cn/)右上角立即使用-注册登陆后-右上角有创建apikey-创建apikey
+        6. 微调数据数量限制1w条，超过会被采样，如果需要微调更大数量请与我们联系，联系方式见最下方
+        7. 完整代码可参考：[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9)
+        8. 默认启动模型推理服务后，会保持10分钟，超时会断开
         <table>
         <tr>
         <td> 上传文件 🔐 </td>
         <td> 启动模型 🔐 </td>
         <td> 调用模型 🔐 </td>
         </tr>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.4 Summary: A Python library
+Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.5 Summary: A Python library
 for the ClueAI API Home-page: https://github.com/clue-ai/clueai-python Author:
 matrix Author-email: brightmart@hotmail.com License: UNKNOWN Description:
 
 
 
            [CLUEAI_logo:_The_data_structure_for_unstructured_data]_
 
@@ -26,17 +26,24 @@
 [æå»ºå¼ææå¡ï¼æ¨è/é®ç­/æç´¢ï¼]
 (#æå»ºå¼ææå¡æ¨èé®ç­æç´¢) - [ä¸ä¼ åº--\>è°ç¨](#ä¸ä¼ åº--
 è°ç¨) - [ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥) - [æ´å¤§æ¨¡åæ´å¥½ææ]
 (#æ´å¤§æ¨¡åæ´å¥½ææ) - [ææ¬åç±»](#ææ¬åç±») - [ææ¬çæ]
 (#ææ¬çæ-1) - [çæåæ°è¯´æ](#çæåæ°è¯´æ) -
 [æ¥çè°ç¨ä½¿ç¨é](#æ¥çè°ç¨ä½¿ç¨é) - [æ¨¡åä»ç»](#æ¨¡åä»ç»)
 - [è¿åç»æ](#è¿åç»æ) - [é®é¢åé¦åææ¯äº¤æµ]
-(#é®é¢åé¦åææ¯äº¤æµ) ### æ´æ° Update 2023-02-03(æ°)
+(#é®é¢åé¦åææ¯äº¤æµ) ### æ´æ° Update 2023-03-23(æ°)
+[ChatYuanå¼æºæ¨¡å](https://github.com/clue-ai/ChatYuan)å¤§åçº§ ### æ´æ°
+Update 2023-02-15 æ°å¢æ¨¡åChatYuanå¾®è°åè½ï¼[æ¨¡åå¾®è°]
+(#æ¨¡åå¾®è°) [ä¸ä¼ åº-å¯å¨-è°ç¨](#ä¸ä¼ åº-å¯å¨-è°ç¨) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-
+y0JyRo1mIXN#scrollTo=jctvm0fxMwEY) ### æ´æ° Update 2023-02-03
 æ°å¢ChatYuanåè½å¯¹è¯ï¼ [ChatYuanåè½å¯¹è¯](#ChatYuanåè½å¯¹è¯) ###
-æ´æ° Update 2022-11-25(æ°) æ°å¢æºè½ææ¡£é®ç­çæï¼
+æ´æ° Update 2023-01-15 [ChatYuanå¼æºæ¨¡å](https://github.com/clue-ai/
+ChatYuan) ### æ´æ° Update 2022-11-25 æ°å¢æºè½ææ¡£é®ç­çæï¼
 [æºè½ææ¡£é®ç­çæ](#æºè½ææ¡£é®ç­çæ) #### æ´æ° Update 2022-
 11-09 æ°å¢æ¨¡åå¾®è°åè½ï¼[æ¨¡åå¾®è°](#æ¨¡åå¾®è°) [ä¸ä¼ åº-
 å¯å¨-è°ç¨](#ä¸ä¼ åº-å¯å¨-è°ç¨) #### æ´æ° Update 2022-09-29
 PromptCLUE:
 ä¸­æå¤ä»»å¡Prompté¢è®­ç»æ¨¡åï¼å·²ç»å¼æºï¼githubé¡¹ç®å°å |
 æ¨¡åä¸è½½ ## Python è½¯ä»¶å
 è¯¥è½¯ä»¶åæä¾äºå¼åçåè½ï¼ä»¥ç®åå¨python3ä¸­ä¸clueai
@@ -56,28 +63,36 @@
 ä¿¡æ¯æ½å ner | 63.02 | 70.09 | | ç¥è¯å¾è°±é®ç­ knowledge_graph | - |
 53.11 | | ä¸­å¿è¯æå Keyword_extraction | 66.50 |71.50 | |
 **çæä»»å¡**ï¼rougeï¼6ç±»ï¼ | | | | ç¿»è¯ï¼è±ä¸­ãä¸­è±ï¼ nmt |
 55.92 | 59.67 | | æè¦ summary | 31.71 | 34.48| | é®ç­ qa | 21.18 | 27.05 |
 | çæï¼æç« ãé®é¢çæï¼ | 35.86 | 39.87 | | æ¹å paraphrase | - |
 57.68 | | çº é correct | - | 93.35 | ### ChatYuanåè½å¯¹è¯ #####
 åè½®å¯¹è¯ ```python import clueai # initialize the Clueai Client with an API
-Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) prompt=
-'''ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå² å°åï¼''' # generate a
-prediction for a prompt #
-éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" prediction =
-cl.generate( model_name='ChatYuan-large', prompt=prompt) # print the predicted
-text print('prediction: {}'.format(prediction.generations[0].text)) ``` #####
-å¤è½®å¯¹è¯ ```python import clueai # initialize the Clueai Client with an API
-Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) prompt=
-'''ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼
+Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) #
+æ³¨æ'''çç¨æ³ï¼å¦ææ¢è¡åï¼ä¸ä¸è¡åä¸è¦å ç©ºæ ¼ï¼è¦é¡¶æ ¼å,
+ï¼ä¸éè¦åä¸æå¯¹é½ï¼ï¼ä¸çæ'''çç¨æ³ï¼è¯·ä½¿ç¨"çå­ç¬¦ä¸²
+""" prompt= '''ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå² å°åï¼''' """ #
+"ç¨æ³çç¤ºä¾ï¼ä½¿ç¨\næ¥æ¼æä¸è¡ prompt =
+"ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå²\nå°åï¼" # generate a prediction
+for a prompt # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION"
+prediction = cl.generate( model_name='ChatYuan-large', prompt=prompt) # print
+the predicted text print('prediction: {}'.format(prediction.generations
+[0].text)) ``` ##### å¤è½®å¯¹è¯ ```python import clueai # initialize the
+Clueai Client with an API Key cl = clueai.Client('YOUR_API_KEY',
+check_api_key=True) #
+æ³¨æ'''çç¨æ³ï¼å¦ææ¢è¡åï¼ä¸ä¸è¡åä¸è¦å ç©ºæ ¼ï¼è¦é¡¶æ ¼å,
+ï¼ä¸éè¦åä¸æå¯¹é½ï¼, ä¸çæ'''çç¨æ³ï¼è¯·ä½¿ç¨"çå­ç¬¦ä¸²
+""" prompt= '''ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼
 å°åï¼æ°å æ¯ææ°åå ç¶çæ¯ï¼å¶çç¶åæ¬åç­ãå¹²å³ãä¹åãåå³è§åéãå¼å¸å°é¾ç­ã
 ç¨æ·ï¼å¯ä»¥åä»ä¹è¯ï¼
 å°åï¼æ ¹æ®æ¨æä¾ççå²ï¼ç®åæ²¡ææç¡®çææ°å çæ¯çè¯ç©ï¼å»ºè®®æ¨å¨å®¶è¿è¡èªæéç¦»ï¼é¿åä¸ä»äººæ¥è§¦ï¼å¤åå¼æ°´ï¼æ¸æ·¡ææ¶åé¥®é£ï¼é¿åç¬å¤åè¿åº¦å³ç´¯ï¼éå½è¿è¡æ·å¤æ´»å¨ã
-ç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å å°åï¼''' # generate a
-prediction for a prompt #
+ç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å å°åï¼''' """ #
+"ç¨æ³çç¤ºä¾ï¼ä½¿ç¨\næ¥æ¼æä¸è¡ prompt =
+"ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼\nå°åï¼æ°å æ¯ææ°åå ç¶çæ¯ï¼å¶çç¶åæ¬åç­ãå¹²å³ãä¹åãåå³è§åéãå¼å¸å°é¾ç­ã\nç¨æ·ï¼å¯ä»¥åä»ä¹è¯ï¼\nå°åï¼æ ¹æ®æ¨æä¾ççå²ï¼ç®åæ²¡ææç¡®çææ°å çæ¯çè¯ç©ï¼å»ºè®®æ¨å¨å®¶è¿è¡èªæéç¦»ï¼é¿åä¸ä»äººæ¥è§¦ï¼å¤åå¼æ°´ï¼æ¸æ·¡ææ¶åé¥®é£ï¼é¿åç¬å¤åè¿åº¦å³ç´¯ï¼éå½è¿è¡æ·å¤æ´»å¨ã\nç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å\nå°åï¼"
+# generate a prediction for a prompt #
 éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" prediction =
 cl.generate( model_name='ChatYuan-large', prompt=prompt) # print the predicted
 text print('prediction: {}'.format(prediction.generations[0].text)) ``` ###
 æºè½ææ¡£é®ç­çæ è¯´æï¼ 1.
 å¯ä»¥æ ¹æ®ä½ çææ¡£ï¼èªå¨çæé®é¢åç­æ¡å¯¹ 2. éè¦æä¸ªAPI
 keyï¼ å¹¶ä¸å¨åå»º`clueai.Client`å¯¹è±¡æ¶éè¦æå®è¿ä¸ªAPI key. API
 key å¯ä»¥éè¿è¿ä¸ª[å¹³å°](https://www.clueai.cn/)è·å¾ï¼æ¹æ³ï¼ ç¹å»
@@ -97,26 +112,37 @@
 ( model_name='clueai-base', prompt=prompt) # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" # print the predicted text print('prediction: {}'.format(prediction.generations[0].text)) ```
 ### ææ¬çæ
 python ð                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    curl ðâ¡â¡
 ```python import clueai # initialize the Clueai Client with an API Key cl = clueai.Client("", check_api_key=False) prompt= ''' æè¦ï¼ æ¬ææ»ç»äºåä¸ªå¯ç©¿æ´äº§åçè®¾è®¡ååï¼èè¿äºååï¼åæ ·ä¹æ¯ç¬èè®¤ä¸ºæ¯è¿ä¸ªè¡ä¸æå¸å¼äººçå°æ¹ï¼1.ä¸ºäººä»¬è§£å³éå¤æ§é®é¢ï¼2.ä»äººå¼å§ï¼èä¸æ¯ä»æºå¨å¼å§ï¼3.è¦�```python curl --location --request POST 'https://www.modelfun.cn/modelfun/api/serving_api' \ --header 'Content-Type: application/json' \ --header 'Model-name: clueai-base' \ --data '{ "task_type": "generate", "task_name": "æè¦", "input_data": ["æè¦ï¼\næ¬ææ»ç»äºåä¸ªå¯ç©¿æ´äº§åçè®¾è®¡ååï¼èè¿äºååï¼åæ ·ä¹æ¯ç¬èè®¤ä¸ºæ¯è¿ä¸ªè¡ä¸æå¸å¼äººçå°æ¹ï¼1.ä¸ºäººä»¬è§£å³éå¤æ§é®é¢ï¼2.ä»äººå¼å§ï¼èä¸æ¯ä»æºå¨å¼å§ï¼3.è¦å¼èµ·æ³¨æï¼ä½ä¸è¦å»æï¼4.æåç¨æ·è½åï¼èä¸æ¯åä»£äºº\nç­æ¡ï¼"] }' ```
 "length_penalty": 1.0, "num_beams": 1 } # å¦æéè¦èªç±è°æ´åæ°èªç±éæ ·çæï¼æ·»å é¢å¤åæ°ä¿¡æ¯è®¾ç½®æ¹å¼ï¼generate_config=generate_config prediction = cl.generate( model_name='clueai-base', prompt=prompt) # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" # print the predicted text print('prediction: {}'.format(prediction.generations[0].text)) ```
 ### æ¨¡åå¾®è° #### ä¸ä¼ åº-å¯å¨-è°ç¨ è¯´æï¼ 1.
 ä¸ä¼ éè¦å¾®è°çæ°æ®ï¼èªå¨è®­ç»å¾®è°/
-é¨ç½²æ¨¡åï¼æä¾æ¥å£ä½¿ç¨ 2. ä¸ä¼ çæ°æ®ä¸ºjsonæ ¼å¼ï¼åè./
-examples/finetune_train_examples.json 3.
+é¨ç½²æ¨¡åï¼æä¾æ¥å£ä½¿ç¨ 2.
+ä¸ä¼ çæ°æ®ä¸ºjsonæ ¼å¼ï¼PromptCLUEåè./examples/
+finetune_train_examples.json, ChatYuanåè./examples/qa_test.json 3.
 åºäºpromptCLUEæ¨¡åå¾®è°ï¼å»ºè®®åèpromptæç¤ºçæ ¼å¼æå»ºæ°æ®éï¼ææä¼æ´å¥½ï¼promptæ ¼å¼å¯ä»¥åèä¸é¢
-[ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥)çå½¢å¼ 4. éè¦æä¸ªAPI keyï¼
+[ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥)çå½¢å¼ 4.
+å¦ææ¯åºäºChatYuanå¾®è°çè¯ï¼å¯ä»¥åè[ç¤ºä¾æ ¼å¼](https://
+github.com/clue-ai/clueai-python/blob/main/examples/
+qa_test.json)ï¼ä¹å¯ä»¥åè[![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-
+y0JyRo1mIXN#scrollTo=jctvm0fxMwEY) a. è¾å¥ä¸ºjsonæ ¼å¼,
+åå«ä¸¤ä¸ªå­æ®µinputåoutputï¼å­æ®µåå­å¯ä»¥èªå·±æå®ï¼ b.
+inputçåå®¹å¯ä»¥æ¯"ç¨æ·ï¼+åå®¹+\nå°åï¼"çæ ¼å¼ï¼ä¹å¯ä»¥ç´æ¥æ¯"åå®¹"çæ ¼å¼
+c. outputçåå®¹ç´æ¥æ¯ä½ æ³æ¨¡åè¾åºçç»æåå®¹å³å¯ 5.
+éè¦æä¸ªAPI keyï¼
 å¹¶ä¸å¨åå»º`clueai.Client`å¯¹è±¡æ¶éè¦æå®è¿ä¸ªAPI key. API key
 å¯ä»¥éè¿è¿ä¸ª[å¹³å°](https://www.clueai.cn/)è·å¾ï¼æ¹æ³ï¼ ç¹å»
 [å®ç½](https://www.clueai.cn/)å³ä¸è§ç«å³ä½¿ç¨-æ³¨åç»éå-
-å³ä¸è§æåå»ºapikey-åå»ºapikey 5.
+å³ä¸è§æåå»ºapikey-åå»ºapikey 6.
 å¾®è°æ°æ®æ°ééå¶1wæ¡ï¼è¶è¿ä¼è¢«éæ ·ï¼å¦æéè¦å¾®è°æ´å¤§æ°éè¯·ä¸æä»¬èç³»ï¼èç³»æ¹å¼è§æä¸æ¹
-6. å®æ´ä»£ç å¯åèï¼[![Open In Colab](https://colab.research.google.com/
+7. å®æ´ä»£ç å¯åèï¼[![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9) 7.
+1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9) 8.
 é»è®¤å¯å¨æ¨¡åæ¨çæå¡åï¼ä¼ä¿æ10åéï¼è¶æ¶ä¼æ­å¼
 ä¸ä¼ æä»¶ ð                                                                                                å¯å¨æ¨¡å ð                                                                                             è°ç¨æ¨¡å ð
 ```python # ä¸ä¼ å°éå¾®è°æ°æ®ï¼æå®è¾å¥åè¾åºå­æ®µï¼                                                                                                                                 ```python import clueai # initialize the Clueai Client with an API Key cl = clueai.Client(api_key) chatyuan_prompt= '''ç¨æ·ï¼ä½ è½å¹²ä»ä¹ï¼ å°åï¼''' clueai_prompt=
 input_fieldåtarget_fieldåå«æä½ éè¦å¾®è°çè¾å¥åè¾åºå­æ®µ # �```python import clueai cl = clueai.Client(api_key) # engine_key æå®ä½ è®­ç»æ¨¡åçkey # æ�'''ä»¥ä¸ä¸¤å¥è¯çææç¸åçåï¼ âè±åå·²ç»éè¿ å¯æ¯æè¿æ²¡æ¶å°âï¼âæçè±åæè¿è¿æ¬¾æ¯å å·âã éé¡¹ï¼æ¯çï¼ä¸æ¯ã ç­æ¡ï¼''' prompt = chatyuan_prompt # generate
 åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡å import clueai ClueAI, ChatYuan:åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡�a prediction for a prompt generate_config = { "do_sample": True, "top_p": 0.8, "max_length": 128, "min_length": 10, "length_penalty": 1.0, "num_beams": 1 } #
 cl.upload_finetune_corpus( file_path="finetune_train_examples.json", input_field="input", target_field="target",                 ( engine_key=engine_key, base_model_name="ChatYuan") print(response) ```                                                      å¦æéè¦èªç±è°æ´åæ°èªç±éæ ·çæï¼æ·»å é¢å¤åæ°ä¿¡æ¯è®¾ç½®æ¹å¼ï¼generate_config=generate_config # æå®åºç¡æ¨¡åChatYuan/ClueAI, ChatYuan:
 base_model_name="ChatYuan" ) if "engine_key" in response: engine_key = response["engine_key"] print("engine key: ", engine_key)                                                                                                                                åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡å prediction = cl.finetune_generate( engine_key=engine_key, prompt=prompt, base_model_name="ChatYuan") # print the predicted text print('prediction:
```

### Comparing `clueai-0.0.2.2.4/README.md` & `clueai-0.0.2.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -46,18 +46,24 @@
     - [文本分类](#文本分类)
     - [文本生成](#文本生成-1)
 - [生成参数说明](#生成参数说明)
 - [查看调用使用量](#查看调用使用量)
 - [模型介绍](#模型介绍)
 - [返回结果](#返回结果)
 - [问题反馈和技术交流](#问题反馈和技术交流)
-
-### 更新 Update 2023-02-03(新)
+### 更新 Update 2023-03-23(新)
+[ChatYuan开源模型](https://github.com/clue-ai/ChatYuan)大升级
+### 更新 Update 2023-02-15
+新增模型ChatYuan微调功能：[模型微调](#模型微调) [上传库-启动-调用](#上传库-启动-调用)  
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=jctvm0fxMwEY)
+### 更新 Update 2023-02-03
 新增ChatYuan功能对话：  [ChatYuan功能对话](#ChatYuan功能对话)
-### 更新 Update 2022-11-25(新)
+### 更新 Update 2023-01-15
+[ChatYuan开源模型](https://github.com/clue-ai/ChatYuan)
+### 更新 Update 2022-11-25
 新增智能文档问答生成：  [智能文档问答生成](#智能文档问答生成)
 #### 更新 Update 2022-11-09
 新增模型微调功能：[模型微调](#模型微调) [上传库-启动-调用](#上传库-启动-调用)
 #### 更新 Update 2022-09-29
 PromptCLUE: 中文多任务Prompt预训练模型，已经开源！<a href='https://github.com/clue-ai/PromptCLUE'>github项目地址</a> | <a href='https://huggingface.co/ClueAI/PromptCLUE'>模型下载</a>
 
 ## Python 软件包
@@ -117,16 +123,22 @@
 
 ##### 单轮对话
 ```python
 import clueai
 
 # initialize the Clueai Client with an API Key
 cl = clueai.Client('YOUR_API_KEY', check_api_key=True)
+# 注意'''的用法，如果换行后，下一行前不要加空格，要顶格写, （不需要和上文对齐），不熟悉'''的用法，请使用"的字符串
+"""
 prompt= '''用户：介绍一下亚马逊云的历史
 小元：'''
+"""
+# "用法的示例，使用\n来拼成一行
+prompt = "用户：介绍一下亚马逊云的历史\n小元："
+
 
 # generate a prediction for a prompt 
 # 需要返回得分的话，指定return_likelihoods="GENERATION"
 prediction = cl.generate(
             model_name='ChatYuan-large',
             prompt=prompt)
             
@@ -136,20 +148,26 @@
 
 ##### 多轮对话
 ```python
 import clueai
 
 # initialize the Clueai Client with an API Key
 cl = clueai.Client('YOUR_API_KEY', check_api_key=True)
+# 注意'''的用法，如果换行后，下一行前不要加空格，要顶格写, （不需要和上文对齐）, 不熟悉'''的用法，请使用"的字符串
+"""
 prompt= '''用户：新冠什么症状？
 小元：新冠是指新型冠状病毒，其症状包括发热、干咳、乏力、嗅味觉减退、呼吸困难等。
 用户：可以吃什么药？
 小元：根据您提供的病史，目前没有明确的抗新冠病毒的药物，建议您在家进行自我隔离，避免与他人接触，多喝开水，清淡易消化饮食，避免熬夜和过度劳累，适当进行户外活动。
 用户：帮我写一个2023年工作规划
 小元：'''
+"""
+# "用法的示例，使用\n来拼成一行
+prompt = "用户：新冠什么症状？\n小元：新冠是指新型冠状病毒，其症状包括发热、干咳、乏力、嗅味觉减退、呼吸困难等。\n用户：可以吃什么药？\n小元：根据您提供的病史，目前没有明确的抗新冠病毒的药物，建议您在家进行自我隔离，避免与他人接触，多喝开水，清淡易消化饮食，避免熬夜和过度劳累，适当进行户外活动。\n用户：帮我写一个2023年工作规划\n小元："
+
 
 # generate a prediction for a prompt 
 # 需要返回得分的话，指定return_likelihoods="GENERATION"
 prediction = cl.generate(
             model_name='ChatYuan-large',
             prompt=prompt)
             
@@ -341,20 +359,24 @@
 </tr>
 </table>
 
 ### 模型微调
 #### 上传库-启动-调用
 说明：
 1. 上传需要微调的数据，自动训练微调/部署模型，提供接口使用
-2. 上传的数据为json格式，参考./examples/finetune_train_examples.json
+2. 上传的数据为json格式，PromptCLUE参考./examples/finetune_train_examples.json, ChatYuan参考./examples/qa_test.json
 3. 基于promptCLUE模型微调，建议参考prompt提示的格式构建数据集，效果会更好，prompt格式可以参考下面[示例输入](#示例输入)的形式
-4. 需要有个API key， 并且在创建`clueai.Client`对象时需要指定这个API key. API key 可以通过这个[平台](https://www.clueai.cn/)获得，方法： 点击[官网](https://www.clueai.cn/)右上角立即使用-注册登陆后-右上角有创建apikey-创建apikey
-5. 微调数据数量限制1w条，超过会被采样，如果需要微调更大数量请与我们联系，联系方式见最下方
-6. 完整代码可参考：[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9)
-7. 默认启动模型推理服务后，会保持10分钟，超时会断开
+4. 如果是基于ChatYuan微调的话，可以参考[示例格式](https://github.com/clue-ai/clueai-python/blob/main/examples/qa_test.json)，也可以参考[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=jctvm0fxMwEY)  
+   a. 输入为json格式, 包含两个字段input和output（字段名字可以自己指定）   
+   b. input的内容可以是"用户：+内容+\n小元："的格式，也可以直接是"内容"的格式  
+   c. output的内容直接是你想模型输出的结果内容即可
+5. 需要有个API key， 并且在创建`clueai.Client`对象时需要指定这个API key. API key 可以通过这个[平台](https://www.clueai.cn/)获得，方法： 点击[官网](https://www.clueai.cn/)右上角立即使用-注册登陆后-右上角有创建apikey-创建apikey
+6. 微调数据数量限制1w条，超过会被采样，如果需要微调更大数量请与我们联系，联系方式见最下方
+7. 完整代码可参考：[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9)
+8. 默认启动模型推理服务后，会保持10分钟，超时会断开
 <table>
 <tr>
 <td> 上传文件 🔐 </td>
 <td> 启动模型 🔐 </td>
 <td> 调用模型 🔐 </td>
 </tr>
```

#### html2text {}

```diff
@@ -23,17 +23,24 @@
 [æå»ºå¼ææå¡ï¼æ¨è/é®ç­/æç´¢ï¼]
 (#æå»ºå¼ææå¡æ¨èé®ç­æç´¢) - [ä¸ä¼ åº--\>è°ç¨](#ä¸ä¼ åº--
 è°ç¨) - [ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥) - [æ´å¤§æ¨¡åæ´å¥½ææ]
 (#æ´å¤§æ¨¡åæ´å¥½ææ) - [ææ¬åç±»](#ææ¬åç±») - [ææ¬çæ]
 (#ææ¬çæ-1) - [çæåæ°è¯´æ](#çæåæ°è¯´æ) -
 [æ¥çè°ç¨ä½¿ç¨é](#æ¥çè°ç¨ä½¿ç¨é) - [æ¨¡åä»ç»](#æ¨¡åä»ç»)
 - [è¿åç»æ](#è¿åç»æ) - [é®é¢åé¦åææ¯äº¤æµ]
-(#é®é¢åé¦åææ¯äº¤æµ) ### æ´æ° Update 2023-02-03(æ°)
+(#é®é¢åé¦åææ¯äº¤æµ) ### æ´æ° Update 2023-03-23(æ°)
+[ChatYuanå¼æºæ¨¡å](https://github.com/clue-ai/ChatYuan)å¤§åçº§ ### æ´æ°
+Update 2023-02-15 æ°å¢æ¨¡åChatYuanå¾®è°åè½ï¼[æ¨¡åå¾®è°]
+(#æ¨¡åå¾®è°) [ä¸ä¼ åº-å¯å¨-è°ç¨](#ä¸ä¼ åº-å¯å¨-è°ç¨) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-
+y0JyRo1mIXN#scrollTo=jctvm0fxMwEY) ### æ´æ° Update 2023-02-03
 æ°å¢ChatYuanåè½å¯¹è¯ï¼ [ChatYuanåè½å¯¹è¯](#ChatYuanåè½å¯¹è¯) ###
-æ´æ° Update 2022-11-25(æ°) æ°å¢æºè½ææ¡£é®ç­çæï¼
+æ´æ° Update 2023-01-15 [ChatYuanå¼æºæ¨¡å](https://github.com/clue-ai/
+ChatYuan) ### æ´æ° Update 2022-11-25 æ°å¢æºè½ææ¡£é®ç­çæï¼
 [æºè½ææ¡£é®ç­çæ](#æºè½ææ¡£é®ç­çæ) #### æ´æ° Update 2022-
 11-09 æ°å¢æ¨¡åå¾®è°åè½ï¼[æ¨¡åå¾®è°](#æ¨¡åå¾®è°) [ä¸ä¼ åº-
 å¯å¨-è°ç¨](#ä¸ä¼ åº-å¯å¨-è°ç¨) #### æ´æ° Update 2022-09-29
 PromptCLUE:
 ä¸­æå¤ä»»å¡Prompté¢è®­ç»æ¨¡åï¼å·²ç»å¼æºï¼githubé¡¹ç®å°å |
 æ¨¡åä¸è½½ ## Python è½¯ä»¶å
 è¯¥è½¯ä»¶åæä¾äºå¼åçåè½ï¼ä»¥ç®åå¨python3ä¸­ä¸clueai
@@ -53,28 +60,36 @@
 ä¿¡æ¯æ½å ner | 63.02 | 70.09 | | ç¥è¯å¾è°±é®ç­ knowledge_graph | - |
 53.11 | | ä¸­å¿è¯æå Keyword_extraction | 66.50 |71.50 | |
 **çæä»»å¡**ï¼rougeï¼6ç±»ï¼ | | | | ç¿»è¯ï¼è±ä¸­ãä¸­è±ï¼ nmt |
 55.92 | 59.67 | | æè¦ summary | 31.71 | 34.48| | é®ç­ qa | 21.18 | 27.05 |
 | çæï¼æç« ãé®é¢çæï¼ | 35.86 | 39.87 | | æ¹å paraphrase | - |
 57.68 | | çº é correct | - | 93.35 | ### ChatYuanåè½å¯¹è¯ #####
 åè½®å¯¹è¯ ```python import clueai # initialize the Clueai Client with an API
-Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) prompt=
-'''ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå² å°åï¼''' # generate a
-prediction for a prompt #
-éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" prediction =
-cl.generate( model_name='ChatYuan-large', prompt=prompt) # print the predicted
-text print('prediction: {}'.format(prediction.generations[0].text)) ``` #####
-å¤è½®å¯¹è¯ ```python import clueai # initialize the Clueai Client with an API
-Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) prompt=
-'''ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼
+Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) #
+æ³¨æ'''çç¨æ³ï¼å¦ææ¢è¡åï¼ä¸ä¸è¡åä¸è¦å ç©ºæ ¼ï¼è¦é¡¶æ ¼å,
+ï¼ä¸éè¦åä¸æå¯¹é½ï¼ï¼ä¸çæ'''çç¨æ³ï¼è¯·ä½¿ç¨"çå­ç¬¦ä¸²
+""" prompt= '''ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå² å°åï¼''' """ #
+"ç¨æ³çç¤ºä¾ï¼ä½¿ç¨\næ¥æ¼æä¸è¡ prompt =
+"ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå²\nå°åï¼" # generate a prediction
+for a prompt # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION"
+prediction = cl.generate( model_name='ChatYuan-large', prompt=prompt) # print
+the predicted text print('prediction: {}'.format(prediction.generations
+[0].text)) ``` ##### å¤è½®å¯¹è¯ ```python import clueai # initialize the
+Clueai Client with an API Key cl = clueai.Client('YOUR_API_KEY',
+check_api_key=True) #
+æ³¨æ'''çç¨æ³ï¼å¦ææ¢è¡åï¼ä¸ä¸è¡åä¸è¦å ç©ºæ ¼ï¼è¦é¡¶æ ¼å,
+ï¼ä¸éè¦åä¸æå¯¹é½ï¼, ä¸çæ'''çç¨æ³ï¼è¯·ä½¿ç¨"çå­ç¬¦ä¸²
+""" prompt= '''ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼
 å°åï¼æ°å æ¯ææ°åå ç¶çæ¯ï¼å¶çç¶åæ¬åç­ãå¹²å³ãä¹åãåå³è§åéãå¼å¸å°é¾ç­ã
 ç¨æ·ï¼å¯ä»¥åä»ä¹è¯ï¼
 å°åï¼æ ¹æ®æ¨æä¾ççå²ï¼ç®åæ²¡ææç¡®çææ°å çæ¯çè¯ç©ï¼å»ºè®®æ¨å¨å®¶è¿è¡èªæéç¦»ï¼é¿åä¸ä»äººæ¥è§¦ï¼å¤åå¼æ°´ï¼æ¸æ·¡ææ¶åé¥®é£ï¼é¿åç¬å¤åè¿åº¦å³ç´¯ï¼éå½è¿è¡æ·å¤æ´»å¨ã
-ç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å å°åï¼''' # generate a
-prediction for a prompt #
+ç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å å°åï¼''' """ #
+"ç¨æ³çç¤ºä¾ï¼ä½¿ç¨\næ¥æ¼æä¸è¡ prompt =
+"ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼\nå°åï¼æ°å æ¯ææ°åå ç¶çæ¯ï¼å¶çç¶åæ¬åç­ãå¹²å³ãä¹åãåå³è§åéãå¼å¸å°é¾ç­ã\nç¨æ·ï¼å¯ä»¥åä»ä¹è¯ï¼\nå°åï¼æ ¹æ®æ¨æä¾ççå²ï¼ç®åæ²¡ææç¡®çææ°å çæ¯çè¯ç©ï¼å»ºè®®æ¨å¨å®¶è¿è¡èªæéç¦»ï¼é¿åä¸ä»äººæ¥è§¦ï¼å¤åå¼æ°´ï¼æ¸æ·¡ææ¶åé¥®é£ï¼é¿åç¬å¤åè¿åº¦å³ç´¯ï¼éå½è¿è¡æ·å¤æ´»å¨ã\nç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å\nå°åï¼"
+# generate a prediction for a prompt #
 éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" prediction =
 cl.generate( model_name='ChatYuan-large', prompt=prompt) # print the predicted
 text print('prediction: {}'.format(prediction.generations[0].text)) ``` ###
 æºè½ææ¡£é®ç­çæ è¯´æï¼ 1.
 å¯ä»¥æ ¹æ®ä½ çææ¡£ï¼èªå¨çæé®é¢åç­æ¡å¯¹ 2. éè¦æä¸ªAPI
 keyï¼ å¹¶ä¸å¨åå»º`clueai.Client`å¯¹è±¡æ¶éè¦æå®è¿ä¸ªAPI key. API
 key å¯ä»¥éè¿è¿ä¸ª[å¹³å°](https://www.clueai.cn/)è·å¾ï¼æ¹æ³ï¼ ç¹å»
@@ -94,26 +109,37 @@
 ( model_name='clueai-base', prompt=prompt) # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" # print the predicted text print('prediction: {}'.format(prediction.generations[0].text)) ```
 ### ææ¬çæ
 python ð                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    curl ðâ¡â¡
 ```python import clueai # initialize the Clueai Client with an API Key cl = clueai.Client("", check_api_key=False) prompt= ''' æè¦ï¼ æ¬ææ»ç»äºåä¸ªå¯ç©¿æ´äº§åçè®¾è®¡ååï¼èè¿äºååï¼åæ ·ä¹æ¯ç¬èè®¤ä¸ºæ¯è¿ä¸ªè¡ä¸æå¸å¼äººçå°æ¹ï¼1.ä¸ºäººä»¬è§£å³éå¤æ§é®é¢ï¼2.ä»äººå¼å§ï¼èä¸æ¯ä»æºå¨å¼å§ï¼3.è¦�```python curl --location --request POST 'https://www.modelfun.cn/modelfun/api/serving_api' \ --header 'Content-Type: application/json' \ --header 'Model-name: clueai-base' \ --data '{ "task_type": "generate", "task_name": "æè¦", "input_data": ["æè¦ï¼\næ¬ææ»ç»äºåä¸ªå¯ç©¿æ´äº§åçè®¾è®¡ååï¼èè¿äºååï¼åæ ·ä¹æ¯ç¬èè®¤ä¸ºæ¯è¿ä¸ªè¡ä¸æå¸å¼äººçå°æ¹ï¼1.ä¸ºäººä»¬è§£å³éå¤æ§é®é¢ï¼2.ä»äººå¼å§ï¼èä¸æ¯ä»æºå¨å¼å§ï¼3.è¦å¼èµ·æ³¨æï¼ä½ä¸è¦å»æï¼4.æåç¨æ·è½åï¼èä¸æ¯åä»£äºº\nç­æ¡ï¼"] }' ```
 "length_penalty": 1.0, "num_beams": 1 } # å¦æéè¦èªç±è°æ´åæ°èªç±éæ ·çæï¼æ·»å é¢å¤åæ°ä¿¡æ¯è®¾ç½®æ¹å¼ï¼generate_config=generate_config prediction = cl.generate( model_name='clueai-base', prompt=prompt) # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" # print the predicted text print('prediction: {}'.format(prediction.generations[0].text)) ```
 ### æ¨¡åå¾®è° #### ä¸ä¼ åº-å¯å¨-è°ç¨ è¯´æï¼ 1.
 ä¸ä¼ éè¦å¾®è°çæ°æ®ï¼èªå¨è®­ç»å¾®è°/
-é¨ç½²æ¨¡åï¼æä¾æ¥å£ä½¿ç¨ 2. ä¸ä¼ çæ°æ®ä¸ºjsonæ ¼å¼ï¼åè./
-examples/finetune_train_examples.json 3.
+é¨ç½²æ¨¡åï¼æä¾æ¥å£ä½¿ç¨ 2.
+ä¸ä¼ çæ°æ®ä¸ºjsonæ ¼å¼ï¼PromptCLUEåè./examples/
+finetune_train_examples.json, ChatYuanåè./examples/qa_test.json 3.
 åºäºpromptCLUEæ¨¡åå¾®è°ï¼å»ºè®®åèpromptæç¤ºçæ ¼å¼æå»ºæ°æ®éï¼ææä¼æ´å¥½ï¼promptæ ¼å¼å¯ä»¥åèä¸é¢
-[ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥)çå½¢å¼ 4. éè¦æä¸ªAPI keyï¼
+[ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥)çå½¢å¼ 4.
+å¦ææ¯åºäºChatYuanå¾®è°çè¯ï¼å¯ä»¥åè[ç¤ºä¾æ ¼å¼](https://
+github.com/clue-ai/clueai-python/blob/main/examples/
+qa_test.json)ï¼ä¹å¯ä»¥åè[![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-
+y0JyRo1mIXN#scrollTo=jctvm0fxMwEY) a. è¾å¥ä¸ºjsonæ ¼å¼,
+åå«ä¸¤ä¸ªå­æ®µinputåoutputï¼å­æ®µåå­å¯ä»¥èªå·±æå®ï¼ b.
+inputçåå®¹å¯ä»¥æ¯"ç¨æ·ï¼+åå®¹+\nå°åï¼"çæ ¼å¼ï¼ä¹å¯ä»¥ç´æ¥æ¯"åå®¹"çæ ¼å¼
+c. outputçåå®¹ç´æ¥æ¯ä½ æ³æ¨¡åè¾åºçç»æåå®¹å³å¯ 5.
+éè¦æä¸ªAPI keyï¼
 å¹¶ä¸å¨åå»º`clueai.Client`å¯¹è±¡æ¶éè¦æå®è¿ä¸ªAPI key. API key
 å¯ä»¥éè¿è¿ä¸ª[å¹³å°](https://www.clueai.cn/)è·å¾ï¼æ¹æ³ï¼ ç¹å»
 [å®ç½](https://www.clueai.cn/)å³ä¸è§ç«å³ä½¿ç¨-æ³¨åç»éå-
-å³ä¸è§æåå»ºapikey-åå»ºapikey 5.
+å³ä¸è§æåå»ºapikey-åå»ºapikey 6.
 å¾®è°æ°æ®æ°ééå¶1wæ¡ï¼è¶è¿ä¼è¢«éæ ·ï¼å¦æéè¦å¾®è°æ´å¤§æ°éè¯·ä¸æä»¬èç³»ï¼èç³»æ¹å¼è§æä¸æ¹
-6. å®æ´ä»£ç å¯åèï¼[![Open In Colab](https://colab.research.google.com/
+7. å®æ´ä»£ç å¯åèï¼[![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9) 7.
+1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9) 8.
 é»è®¤å¯å¨æ¨¡åæ¨çæå¡åï¼ä¼ä¿æ10åéï¼è¶æ¶ä¼æ­å¼
 ä¸ä¼ æä»¶ ð                                                                                                å¯å¨æ¨¡å ð                                                                                             è°ç¨æ¨¡å ð
 ```python # ä¸ä¼ å°éå¾®è°æ°æ®ï¼æå®è¾å¥åè¾åºå­æ®µï¼                                                                                                                                 ```python import clueai # initialize the Clueai Client with an API Key cl = clueai.Client(api_key) chatyuan_prompt= '''ç¨æ·ï¼ä½ è½å¹²ä»ä¹ï¼ å°åï¼''' clueai_prompt=
 input_fieldåtarget_fieldåå«æä½ éè¦å¾®è°çè¾å¥åè¾åºå­æ®µ # �```python import clueai cl = clueai.Client(api_key) # engine_key æå®ä½ è®­ç»æ¨¡åçkey # æ�'''ä»¥ä¸ä¸¤å¥è¯çææç¸åçåï¼ âè±åå·²ç»éè¿ å¯æ¯æè¿æ²¡æ¶å°âï¼âæçè±åæè¿è¿æ¬¾æ¯å å·âã éé¡¹ï¼æ¯çï¼ä¸æ¯ã ç­æ¡ï¼''' prompt = chatyuan_prompt # generate
 åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡å import clueai ClueAI, ChatYuan:åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡�a prediction for a prompt generate_config = { "do_sample": True, "top_p": 0.8, "max_length": 128, "min_length": 10, "length_penalty": 1.0, "num_beams": 1 } #
 cl.upload_finetune_corpus( file_path="finetune_train_examples.json", input_field="input", target_field="target",                 ( engine_key=engine_key, base_model_name="ChatYuan") print(response) ```                                                      å¦æéè¦èªç±è°æ´åæ°èªç±éæ ·çæï¼æ·»å é¢å¤åæ°ä¿¡æ¯è®¾ç½®æ¹å¼ï¼generate_config=generate_config # æå®åºç¡æ¨¡åChatYuan/ClueAI, ChatYuan:
 base_model_name="ChatYuan" ) if "engine_key" in response: engine_key = response["engine_key"] print("engine key: ", engine_key)                                                                                                                                åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡å prediction = cl.finetune_generate( engine_key=engine_key, prompt=prompt, base_model_name="ChatYuan") # print the predicted text print('prediction:
```

### Comparing `clueai-0.0.2.2.4/clueai/classify.py` & `clueai-0.0.2.2.5/clueai/classify.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/clueai/client.py` & `clueai-0.0.2.2.5/clueai/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,15 +557,15 @@
         tmp_headers.update(headers)
         url = urljoin(self.api_url, endpoint)
         #print(json_body)
         if use_xhr_client:
             response = self.__pyfetch(url, tmp_headers, json_body)
             return response
         else:
-            response = requests.post(url, json=json.loads(json_body), headers=tmp_headers)
+            response = requests.post(url, json=json.loads(json_body), headers=tmp_headers, timeout=self.timeout)
             try:
                 res = json.loads(response.text)
             except Exception:
                 raise ClueaiError(
                     message=response.text,
                     http_status=response.status_code,
                     headers=response.headers)
```

### Comparing `clueai-0.0.2.2.4/clueai/error.py` & `clueai-0.0.2.2.5/clueai/error.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/clueai/extract.py` & `clueai-0.0.2.2.5/clueai/extract.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/clueai/generation.py` & `clueai-0.0.2.2.5/clueai/generation.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/clueai/match.py` & `clueai-0.0.2.2.5/clueai/match.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/clueai/qa.py` & `clueai-0.0.2.2.5/clueai/qa.py`

 * *Files identical despite different names*

### Comparing `clueai-0.0.2.2.4/clueai.egg-info/PKG-INFO` & `clueai-0.0.2.2.5/clueai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clueai
-Version: 0.0.2.2.4
+Version: 0.0.2.2.5
 Summary: A Python library for the ClueAI API
 Home-page: https://github.com/clue-ai/clueai-python
 Author: matrix
 Author-email: brightmart@hotmail.com
 License: UNKNOWN
 Description: 
         <p align="center">
@@ -54,18 +54,24 @@
             - [文本分类](#文本分类)
             - [文本生成](#文本生成-1)
         - [生成参数说明](#生成参数说明)
         - [查看调用使用量](#查看调用使用量)
         - [模型介绍](#模型介绍)
         - [返回结果](#返回结果)
         - [问题反馈和技术交流](#问题反馈和技术交流)
-        
-        ### 更新 Update 2023-02-03(新)
+        ### 更新 Update 2023-03-23(新)
+        [ChatYuan开源模型](https://github.com/clue-ai/ChatYuan)大升级
+        ### 更新 Update 2023-02-15
+        新增模型ChatYuan微调功能：[模型微调](#模型微调) [上传库-启动-调用](#上传库-启动-调用)  
+        [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=jctvm0fxMwEY)
+        ### 更新 Update 2023-02-03
         新增ChatYuan功能对话：  [ChatYuan功能对话](#ChatYuan功能对话)
-        ### 更新 Update 2022-11-25(新)
+        ### 更新 Update 2023-01-15
+        [ChatYuan开源模型](https://github.com/clue-ai/ChatYuan)
+        ### 更新 Update 2022-11-25
         新增智能文档问答生成：  [智能文档问答生成](#智能文档问答生成)
         #### 更新 Update 2022-11-09
         新增模型微调功能：[模型微调](#模型微调) [上传库-启动-调用](#上传库-启动-调用)
         #### 更新 Update 2022-09-29
         PromptCLUE: 中文多任务Prompt预训练模型，已经开源！<a href='https://github.com/clue-ai/PromptCLUE'>github项目地址</a> | <a href='https://huggingface.co/ClueAI/PromptCLUE'>模型下载</a>
         
         ## Python 软件包
@@ -125,16 +131,22 @@
         
         ##### 单轮对话
         ```python
         import clueai
         
         # initialize the Clueai Client with an API Key
         cl = clueai.Client('YOUR_API_KEY', check_api_key=True)
+        # 注意'''的用法，如果换行后，下一行前不要加空格，要顶格写, （不需要和上文对齐），不熟悉'''的用法，请使用"的字符串
+        """
         prompt= '''用户：介绍一下亚马逊云的历史
         小元：'''
+        """
+        # "用法的示例，使用\n来拼成一行
+        prompt = "用户：介绍一下亚马逊云的历史\n小元："
+        
         
         # generate a prediction for a prompt 
         # 需要返回得分的话，指定return_likelihoods="GENERATION"
         prediction = cl.generate(
                     model_name='ChatYuan-large',
                     prompt=prompt)
                     
@@ -144,20 +156,26 @@
         
         ##### 多轮对话
         ```python
         import clueai
         
         # initialize the Clueai Client with an API Key
         cl = clueai.Client('YOUR_API_KEY', check_api_key=True)
+        # 注意'''的用法，如果换行后，下一行前不要加空格，要顶格写, （不需要和上文对齐）, 不熟悉'''的用法，请使用"的字符串
+        """
         prompt= '''用户：新冠什么症状？
         小元：新冠是指新型冠状病毒，其症状包括发热、干咳、乏力、嗅味觉减退、呼吸困难等。
         用户：可以吃什么药？
         小元：根据您提供的病史，目前没有明确的抗新冠病毒的药物，建议您在家进行自我隔离，避免与他人接触，多喝开水，清淡易消化饮食，避免熬夜和过度劳累，适当进行户外活动。
         用户：帮我写一个2023年工作规划
         小元：'''
+        """
+        # "用法的示例，使用\n来拼成一行
+        prompt = "用户：新冠什么症状？\n小元：新冠是指新型冠状病毒，其症状包括发热、干咳、乏力、嗅味觉减退、呼吸困难等。\n用户：可以吃什么药？\n小元：根据您提供的病史，目前没有明确的抗新冠病毒的药物，建议您在家进行自我隔离，避免与他人接触，多喝开水，清淡易消化饮食，避免熬夜和过度劳累，适当进行户外活动。\n用户：帮我写一个2023年工作规划\n小元："
+        
         
         # generate a prediction for a prompt 
         # 需要返回得分的话，指定return_likelihoods="GENERATION"
         prediction = cl.generate(
                     model_name='ChatYuan-large',
                     prompt=prompt)
                     
@@ -349,20 +367,24 @@
         </tr>
         </table>
         
         ### 模型微调
         #### 上传库-启动-调用
         说明：
         1. 上传需要微调的数据，自动训练微调/部署模型，提供接口使用
-        2. 上传的数据为json格式，参考./examples/finetune_train_examples.json
+        2. 上传的数据为json格式，PromptCLUE参考./examples/finetune_train_examples.json, ChatYuan参考./examples/qa_test.json
         3. 基于promptCLUE模型微调，建议参考prompt提示的格式构建数据集，效果会更好，prompt格式可以参考下面[示例输入](#示例输入)的形式
-        4. 需要有个API key， 并且在创建`clueai.Client`对象时需要指定这个API key. API key 可以通过这个[平台](https://www.clueai.cn/)获得，方法： 点击[官网](https://www.clueai.cn/)右上角立即使用-注册登陆后-右上角有创建apikey-创建apikey
-        5. 微调数据数量限制1w条，超过会被采样，如果需要微调更大数量请与我们联系，联系方式见最下方
-        6. 完整代码可参考：[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9)
-        7. 默认启动模型推理服务后，会保持10分钟，超时会断开
+        4. 如果是基于ChatYuan微调的话，可以参考[示例格式](https://github.com/clue-ai/clueai-python/blob/main/examples/qa_test.json)，也可以参考[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=jctvm0fxMwEY)  
+           a. 输入为json格式, 包含两个字段input和output（字段名字可以自己指定）   
+           b. input的内容可以是"用户：+内容+\n小元："的格式，也可以直接是"内容"的格式  
+           c. output的内容直接是你想模型输出的结果内容即可
+        5. 需要有个API key， 并且在创建`clueai.Client`对象时需要指定这个API key. API key 可以通过这个[平台](https://www.clueai.cn/)获得，方法： 点击[官网](https://www.clueai.cn/)右上角立即使用-注册登陆后-右上角有创建apikey-创建apikey
+        6. 微调数据数量限制1w条，超过会被采样，如果需要微调更大数量请与我们联系，联系方式见最下方
+        7. 完整代码可参考：[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9)
+        8. 默认启动模型推理服务后，会保持10分钟，超时会断开
         <table>
         <tr>
         <td> 上传文件 🔐 </td>
         <td> 启动模型 🔐 </td>
         <td> 调用模型 🔐 </td>
         </tr>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.4 Summary: A Python library
+Metadata-Version: 2.1 Name: clueai Version: 0.0.2.2.5 Summary: A Python library
 for the ClueAI API Home-page: https://github.com/clue-ai/clueai-python Author:
 matrix Author-email: brightmart@hotmail.com License: UNKNOWN Description:
 
 
 
            [CLUEAI_logo:_The_data_structure_for_unstructured_data]_
 
@@ -26,17 +26,24 @@
 [æå»ºå¼ææå¡ï¼æ¨è/é®ç­/æç´¢ï¼]
 (#æå»ºå¼ææå¡æ¨èé®ç­æç´¢) - [ä¸ä¼ åº--\>è°ç¨](#ä¸ä¼ åº--
 è°ç¨) - [ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥) - [æ´å¤§æ¨¡åæ´å¥½ææ]
 (#æ´å¤§æ¨¡åæ´å¥½ææ) - [ææ¬åç±»](#ææ¬åç±») - [ææ¬çæ]
 (#ææ¬çæ-1) - [çæåæ°è¯´æ](#çæåæ°è¯´æ) -
 [æ¥çè°ç¨ä½¿ç¨é](#æ¥çè°ç¨ä½¿ç¨é) - [æ¨¡åä»ç»](#æ¨¡åä»ç»)
 - [è¿åç»æ](#è¿åç»æ) - [é®é¢åé¦åææ¯äº¤æµ]
-(#é®é¢åé¦åææ¯äº¤æµ) ### æ´æ° Update 2023-02-03(æ°)
+(#é®é¢åé¦åææ¯äº¤æµ) ### æ´æ° Update 2023-03-23(æ°)
+[ChatYuanå¼æºæ¨¡å](https://github.com/clue-ai/ChatYuan)å¤§åçº§ ### æ´æ°
+Update 2023-02-15 æ°å¢æ¨¡åChatYuanå¾®è°åè½ï¼[æ¨¡åå¾®è°]
+(#æ¨¡åå¾®è°) [ä¸ä¼ åº-å¯å¨-è°ç¨](#ä¸ä¼ åº-å¯å¨-è°ç¨) [![Open In
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-
+y0JyRo1mIXN#scrollTo=jctvm0fxMwEY) ### æ´æ° Update 2023-02-03
 æ°å¢ChatYuanåè½å¯¹è¯ï¼ [ChatYuanåè½å¯¹è¯](#ChatYuanåè½å¯¹è¯) ###
-æ´æ° Update 2022-11-25(æ°) æ°å¢æºè½ææ¡£é®ç­çæï¼
+æ´æ° Update 2023-01-15 [ChatYuanå¼æºæ¨¡å](https://github.com/clue-ai/
+ChatYuan) ### æ´æ° Update 2022-11-25 æ°å¢æºè½ææ¡£é®ç­çæï¼
 [æºè½ææ¡£é®ç­çæ](#æºè½ææ¡£é®ç­çæ) #### æ´æ° Update 2022-
 11-09 æ°å¢æ¨¡åå¾®è°åè½ï¼[æ¨¡åå¾®è°](#æ¨¡åå¾®è°) [ä¸ä¼ åº-
 å¯å¨-è°ç¨](#ä¸ä¼ åº-å¯å¨-è°ç¨) #### æ´æ° Update 2022-09-29
 PromptCLUE:
 ä¸­æå¤ä»»å¡Prompté¢è®­ç»æ¨¡åï¼å·²ç»å¼æºï¼githubé¡¹ç®å°å |
 æ¨¡åä¸è½½ ## Python è½¯ä»¶å
 è¯¥è½¯ä»¶åæä¾äºå¼åçåè½ï¼ä»¥ç®åå¨python3ä¸­ä¸clueai
@@ -56,28 +63,36 @@
 ä¿¡æ¯æ½å ner | 63.02 | 70.09 | | ç¥è¯å¾è°±é®ç­ knowledge_graph | - |
 53.11 | | ä¸­å¿è¯æå Keyword_extraction | 66.50 |71.50 | |
 **çæä»»å¡**ï¼rougeï¼6ç±»ï¼ | | | | ç¿»è¯ï¼è±ä¸­ãä¸­è±ï¼ nmt |
 55.92 | 59.67 | | æè¦ summary | 31.71 | 34.48| | é®ç­ qa | 21.18 | 27.05 |
 | çæï¼æç« ãé®é¢çæï¼ | 35.86 | 39.87 | | æ¹å paraphrase | - |
 57.68 | | çº é correct | - | 93.35 | ### ChatYuanåè½å¯¹è¯ #####
 åè½®å¯¹è¯ ```python import clueai # initialize the Clueai Client with an API
-Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) prompt=
-'''ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå² å°åï¼''' # generate a
-prediction for a prompt #
-éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" prediction =
-cl.generate( model_name='ChatYuan-large', prompt=prompt) # print the predicted
-text print('prediction: {}'.format(prediction.generations[0].text)) ``` #####
-å¤è½®å¯¹è¯ ```python import clueai # initialize the Clueai Client with an API
-Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) prompt=
-'''ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼
+Key cl = clueai.Client('YOUR_API_KEY', check_api_key=True) #
+æ³¨æ'''çç¨æ³ï¼å¦ææ¢è¡åï¼ä¸ä¸è¡åä¸è¦å ç©ºæ ¼ï¼è¦é¡¶æ ¼å,
+ï¼ä¸éè¦åä¸æå¯¹é½ï¼ï¼ä¸çæ'''çç¨æ³ï¼è¯·ä½¿ç¨"çå­ç¬¦ä¸²
+""" prompt= '''ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå² å°åï¼''' """ #
+"ç¨æ³çç¤ºä¾ï¼ä½¿ç¨\næ¥æ¼æä¸è¡ prompt =
+"ç¨æ·ï¼ä»ç»ä¸ä¸äºé©¬éäºçåå²\nå°åï¼" # generate a prediction
+for a prompt # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION"
+prediction = cl.generate( model_name='ChatYuan-large', prompt=prompt) # print
+the predicted text print('prediction: {}'.format(prediction.generations
+[0].text)) ``` ##### å¤è½®å¯¹è¯ ```python import clueai # initialize the
+Clueai Client with an API Key cl = clueai.Client('YOUR_API_KEY',
+check_api_key=True) #
+æ³¨æ'''çç¨æ³ï¼å¦ææ¢è¡åï¼ä¸ä¸è¡åä¸è¦å ç©ºæ ¼ï¼è¦é¡¶æ ¼å,
+ï¼ä¸éè¦åä¸æå¯¹é½ï¼, ä¸çæ'''çç¨æ³ï¼è¯·ä½¿ç¨"çå­ç¬¦ä¸²
+""" prompt= '''ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼
 å°åï¼æ°å æ¯ææ°åå ç¶çæ¯ï¼å¶çç¶åæ¬åç­ãå¹²å³ãä¹åãåå³è§åéãå¼å¸å°é¾ç­ã
 ç¨æ·ï¼å¯ä»¥åä»ä¹è¯ï¼
 å°åï¼æ ¹æ®æ¨æä¾ççå²ï¼ç®åæ²¡ææç¡®çææ°å çæ¯çè¯ç©ï¼å»ºè®®æ¨å¨å®¶è¿è¡èªæéç¦»ï¼é¿åä¸ä»äººæ¥è§¦ï¼å¤åå¼æ°´ï¼æ¸æ·¡ææ¶åé¥®é£ï¼é¿åç¬å¤åè¿åº¦å³ç´¯ï¼éå½è¿è¡æ·å¤æ´»å¨ã
-ç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å å°åï¼''' # generate a
-prediction for a prompt #
+ç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å å°åï¼''' """ #
+"ç¨æ³çç¤ºä¾ï¼ä½¿ç¨\næ¥æ¼æä¸è¡ prompt =
+"ç¨æ·ï¼æ°å ä»ä¹çç¶ï¼\nå°åï¼æ°å æ¯ææ°åå ç¶çæ¯ï¼å¶çç¶åæ¬åç­ãå¹²å³ãä¹åãåå³è§åéãå¼å¸å°é¾ç­ã\nç¨æ·ï¼å¯ä»¥åä»ä¹è¯ï¼\nå°åï¼æ ¹æ®æ¨æä¾ççå²ï¼ç®åæ²¡ææç¡®çææ°å çæ¯çè¯ç©ï¼å»ºè®®æ¨å¨å®¶è¿è¡èªæéç¦»ï¼é¿åä¸ä»äººæ¥è§¦ï¼å¤åå¼æ°´ï¼æ¸æ·¡ææ¶åé¥®é£ï¼é¿åç¬å¤åè¿åº¦å³ç´¯ï¼éå½è¿è¡æ·å¤æ´»å¨ã\nç¨æ·ï¼å¸®æåä¸ä¸ª2023å¹´å·¥ä½è§å\nå°åï¼"
+# generate a prediction for a prompt #
 éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" prediction =
 cl.generate( model_name='ChatYuan-large', prompt=prompt) # print the predicted
 text print('prediction: {}'.format(prediction.generations[0].text)) ``` ###
 æºè½ææ¡£é®ç­çæ è¯´æï¼ 1.
 å¯ä»¥æ ¹æ®ä½ çææ¡£ï¼èªå¨çæé®é¢åç­æ¡å¯¹ 2. éè¦æä¸ªAPI
 keyï¼ å¹¶ä¸å¨åå»º`clueai.Client`å¯¹è±¡æ¶éè¦æå®è¿ä¸ªAPI key. API
 key å¯ä»¥éè¿è¿ä¸ª[å¹³å°](https://www.clueai.cn/)è·å¾ï¼æ¹æ³ï¼ ç¹å»
@@ -97,26 +112,37 @@
 ( model_name='clueai-base', prompt=prompt) # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" # print the predicted text print('prediction: {}'.format(prediction.generations[0].text)) ```
 ### ææ¬çæ
 python ð                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    curl ðâ¡â¡
 ```python import clueai # initialize the Clueai Client with an API Key cl = clueai.Client("", check_api_key=False) prompt= ''' æè¦ï¼ æ¬ææ»ç»äºåä¸ªå¯ç©¿æ´äº§åçè®¾è®¡ååï¼èè¿äºååï¼åæ ·ä¹æ¯ç¬èè®¤ä¸ºæ¯è¿ä¸ªè¡ä¸æå¸å¼äººçå°æ¹ï¼1.ä¸ºäººä»¬è§£å³éå¤æ§é®é¢ï¼2.ä»äººå¼å§ï¼èä¸æ¯ä»æºå¨å¼å§ï¼3.è¦�```python curl --location --request POST 'https://www.modelfun.cn/modelfun/api/serving_api' \ --header 'Content-Type: application/json' \ --header 'Model-name: clueai-base' \ --data '{ "task_type": "generate", "task_name": "æè¦", "input_data": ["æè¦ï¼\næ¬ææ»ç»äºåä¸ªå¯ç©¿æ´äº§åçè®¾è®¡ååï¼èè¿äºååï¼åæ ·ä¹æ¯ç¬èè®¤ä¸ºæ¯è¿ä¸ªè¡ä¸æå¸å¼äººçå°æ¹ï¼1.ä¸ºäººä»¬è§£å³éå¤æ§é®é¢ï¼2.ä»äººå¼å§ï¼èä¸æ¯ä»æºå¨å¼å§ï¼3.è¦å¼èµ·æ³¨æï¼ä½ä¸è¦å»æï¼4.æåç¨æ·è½åï¼èä¸æ¯åä»£äºº\nç­æ¡ï¼"] }' ```
 "length_penalty": 1.0, "num_beams": 1 } # å¦æéè¦èªç±è°æ´åæ°èªç±éæ ·çæï¼æ·»å é¢å¤åæ°ä¿¡æ¯è®¾ç½®æ¹å¼ï¼generate_config=generate_config prediction = cl.generate( model_name='clueai-base', prompt=prompt) # éè¦è¿åå¾åçè¯ï¼æå®return_likelihoods="GENERATION" # print the predicted text print('prediction: {}'.format(prediction.generations[0].text)) ```
 ### æ¨¡åå¾®è° #### ä¸ä¼ åº-å¯å¨-è°ç¨ è¯´æï¼ 1.
 ä¸ä¼ éè¦å¾®è°çæ°æ®ï¼èªå¨è®­ç»å¾®è°/
-é¨ç½²æ¨¡åï¼æä¾æ¥å£ä½¿ç¨ 2. ä¸ä¼ çæ°æ®ä¸ºjsonæ ¼å¼ï¼åè./
-examples/finetune_train_examples.json 3.
+é¨ç½²æ¨¡åï¼æä¾æ¥å£ä½¿ç¨ 2.
+ä¸ä¼ çæ°æ®ä¸ºjsonæ ¼å¼ï¼PromptCLUEåè./examples/
+finetune_train_examples.json, ChatYuanåè./examples/qa_test.json 3.
 åºäºpromptCLUEæ¨¡åå¾®è°ï¼å»ºè®®åèpromptæç¤ºçæ ¼å¼æå»ºæ°æ®éï¼ææä¼æ´å¥½ï¼promptæ ¼å¼å¯ä»¥åèä¸é¢
-[ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥)çå½¢å¼ 4. éè¦æä¸ªAPI keyï¼
+[ç¤ºä¾è¾å¥](#ç¤ºä¾è¾å¥)çå½¢å¼ 4.
+å¦ææ¯åºäºChatYuanå¾®è°çè¯ï¼å¯ä»¥åè[ç¤ºä¾æ ¼å¼](https://
+github.com/clue-ai/clueai-python/blob/main/examples/
+qa_test.json)ï¼ä¹å¯ä»¥åè[![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/drive/1H5J03ek3kpKschQ32mhX-
+y0JyRo1mIXN#scrollTo=jctvm0fxMwEY) a. è¾å¥ä¸ºjsonæ ¼å¼,
+åå«ä¸¤ä¸ªå­æ®µinputåoutputï¼å­æ®µåå­å¯ä»¥èªå·±æå®ï¼ b.
+inputçåå®¹å¯ä»¥æ¯"ç¨æ·ï¼+åå®¹+\nå°åï¼"çæ ¼å¼ï¼ä¹å¯ä»¥ç´æ¥æ¯"åå®¹"çæ ¼å¼
+c. outputçåå®¹ç´æ¥æ¯ä½ æ³æ¨¡åè¾åºçç»æåå®¹å³å¯ 5.
+éè¦æä¸ªAPI keyï¼
 å¹¶ä¸å¨åå»º`clueai.Client`å¯¹è±¡æ¶éè¦æå®è¿ä¸ªAPI key. API key
 å¯ä»¥éè¿è¿ä¸ª[å¹³å°](https://www.clueai.cn/)è·å¾ï¼æ¹æ³ï¼ ç¹å»
 [å®ç½](https://www.clueai.cn/)å³ä¸è§ç«å³ä½¿ç¨-æ³¨åç»éå-
-å³ä¸è§æåå»ºapikey-åå»ºapikey 5.
+å³ä¸è§æåå»ºapikey-åå»ºapikey 6.
 å¾®è°æ°æ®æ°ééå¶1wæ¡ï¼è¶è¿ä¼è¢«éæ ·ï¼å¦æéè¦å¾®è°æ´å¤§æ°éè¯·ä¸æä»¬èç³»ï¼èç³»æ¹å¼è§æä¸æ¹
-6. å®æ´ä»£ç å¯åèï¼[![Open In Colab](https://colab.research.google.com/
+7. å®æ´ä»£ç å¯åèï¼[![Open In Colab](https://colab.research.google.com/
 assets/colab-badge.svg)](https://colab.research.google.com/drive/
-1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9) 7.
+1H5J03ek3kpKschQ32mhX-y0JyRo1mIXN#scrollTo=zMSp1naSL8X9) 8.
 é»è®¤å¯å¨æ¨¡åæ¨çæå¡åï¼ä¼ä¿æ10åéï¼è¶æ¶ä¼æ­å¼
 ä¸ä¼ æä»¶ ð                                                                                                å¯å¨æ¨¡å ð                                                                                             è°ç¨æ¨¡å ð
 ```python # ä¸ä¼ å°éå¾®è°æ°æ®ï¼æå®è¾å¥åè¾åºå­æ®µï¼                                                                                                                                 ```python import clueai # initialize the Clueai Client with an API Key cl = clueai.Client(api_key) chatyuan_prompt= '''ç¨æ·ï¼ä½ è½å¹²ä»ä¹ï¼ å°åï¼''' clueai_prompt=
 input_fieldåtarget_fieldåå«æä½ éè¦å¾®è°çè¾å¥åè¾åºå­æ®µ # �```python import clueai cl = clueai.Client(api_key) # engine_key æå®ä½ è®­ç»æ¨¡åçkey # æ�'''ä»¥ä¸ä¸¤å¥è¯çææç¸åçåï¼ âè±åå·²ç»éè¿ å¯æ¯æè¿æ²¡æ¶å°âï¼âæçè±åæè¿è¿æ¬¾æ¯å å·âã éé¡¹ï¼æ¯çï¼ä¸æ¯ã ç­æ¡ï¼''' prompt = chatyuan_prompt # generate
 åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡å import clueai ClueAI, ChatYuan:åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡�a prediction for a prompt generate_config = { "do_sample": True, "top_p": 0.8, "max_length": 128, "min_length": 10, "length_penalty": 1.0, "num_beams": 1 } #
 cl.upload_finetune_corpus( file_path="finetune_train_examples.json", input_field="input", target_field="target",                 ( engine_key=engine_key, base_model_name="ChatYuan") print(response) ```                                                      å¦æéè¦èªç±è°æ´åæ°èªç±éæ ·çæï¼æ·»å é¢å¤åæ°ä¿¡æ¯è®¾ç½®æ¹å¼ï¼generate_config=generate_config # æå®åºç¡æ¨¡åChatYuan/ClueAI, ChatYuan:
 base_model_name="ChatYuan" ) if "engine_key" in response: engine_key = response["engine_key"] print("engine key: ", engine_key)                                                                                                                                åè½å¯¹è¯å¤§æ¨¡åï¼ClueAIï¼åæ¨¡åå¤ä»»å¡å¤§æ¨¡å prediction = cl.finetune_generate( engine_key=engine_key, prompt=prompt, base_model_name="ChatYuan") # print the predicted text print('prediction:
```

### Comparing `clueai-0.0.2.2.4/setup.py` & `clueai-0.0.2.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return False
 
     def has_ext_modules(foo) -> bool:
         return True
 
 setuptools.setup(
     name='clueai',
-    version='0.0.2.2.4',
+    version='0.0.2.2.5',
     author='matrix',
     author_email='brightmart@hotmail.com',
     description='A Python library for the ClueAI API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/clue-ai/clueai-python',
     packages=setuptools.find_packages(),
```

