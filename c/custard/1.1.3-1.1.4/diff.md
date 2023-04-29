# Comparing `tmp/custard-1.1.3.tar.gz` & `tmp/custard-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custard-1.1.3.tar", max compression
+gzip compressed data, was "custard-1.1.4.tar", max compression
```

## Comparing `custard-1.1.3.tar` & `custard-1.1.4.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0     5635 2023-04-29 14:23:05.810066 custard-1.1.3/README.md
--rw-r--r--   0        0        0      236 2023-04-29 14:23:05.810066 custard-1.1.3/custard/__init__.py
--rw-r--r--   0        0        0     1242 2023-04-29 14:23:05.810066 custard-1.1.3/custard/core/__init__.py
--rw-r--r--   0        0        0   770290 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/decode.py
--rw-r--r--   0        0        0    28568 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/factory.py
--rw-r--r--   0        0        0    13726 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/functools.py
--rw-r--r--   0        0        0     2976 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/kerberos.py
--rw-r--r--   0        0        0    24995 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/processor.py
--rw-r--r--   0        0        0    20274 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/regular.py
--rw-r--r--   0        0        0     1973 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/snowflake.py
--rw-r--r--   0        0        0    15658 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/system.py
--rw-r--r--   0        0        0    22041 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/useragent.py
--rw-r--r--   0        0        0     1607 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/xml2dict.py
--rw-r--r--   0        0        0     2023 2023-04-29 14:23:05.814066 custard-1.1.3/custard/core/xprint.py
--rw-r--r--   0        0        0      463 2023-04-29 14:23:05.814066 custard-1.1.3/custard/crypto/__init__.py
--rw-r--r--   0        0        0    15654 2023-04-29 14:23:05.814066 custard-1.1.3/custard/crypto/crypto.py
--rw-r--r--   0        0        0     3257 2023-04-29 14:23:05.814066 custard-1.1.3/custard/crypto/streambody.py
--rw-r--r--   0        0        0      323 2023-04-29 14:23:05.814066 custard-1.1.3/custard/curl/__init__.py
--rw-r--r--   0        0        0     5850 2023-04-29 14:23:05.814066 custard-1.1.3/custard/curl/parse.py
--rw-r--r--   0        0        0      291 2023-04-29 14:23:05.814066 custard-1.1.3/custard/hitfilter/__init__.py
--rw-r--r--   0        0        0     2972 2023-04-29 14:23:05.814066 custard-1.1.3/custard/hitfilter/hitfilter.py
--rw-r--r--   0        0        0   761348 2023-04-29 14:23:05.818066 custard-1.1.3/custard/hitfilter/keywords
--rw-r--r--   0        0        0      418 2023-04-29 14:23:05.818066 custard-1.1.3/custard/kaptcha/__init__.py
--rw-r--r--   0        0        0     9386 2023-04-29 14:23:05.818066 custard-1.1.3/custard/kaptcha/captcha.py
--rw-r--r--   0        0        0   171508 2023-04-29 14:23:05.822066 custard-1.1.3/custard/kaptcha/font1.ttf
--rw-r--r--   0        0        0    42452 2023-04-29 14:23:05.822066 custard-1.1.3/custard/kaptcha/font2.ttf
--rw-r--r--   0        0        0    92956 2023-04-29 14:23:05.822066 custard-1.1.3/custard/kaptcha/font3.ttf
--rw-r--r--   0        0        0   314452 2023-04-29 14:23:05.822066 custard-1.1.3/custard/kaptcha/font4.ttf
--rw-r--r--   0        0        0     3411 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/README.md
--rw-r--r--   0        0        0     2584 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/__init__.py
--rw-r--r--   0        0        0     2818 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/depends.py
--rw-r--r--   0        0        0      452 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/enums.py
--rw-r--r--   0        0        0     1705 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/examples/__init__.py
--rw-r--r--   0        0        0     1962 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/examples/test_depends.py
--rw-r--r--   0        0        0      438 2023-04-29 14:23:05.822066 custard-1.1.3/custard/limiter/execres.py
--rw-r--r--   0        0        0     1819 2023-04-29 14:23:05.822066 custard-1.1.3/custard/mock/__init__.py
--rw-r--r--   0        0        0    14336 2023-04-29 14:23:05.822066 custard-1.1.3/custard/mock/mini_racer.py
--rw-r--r--   0        0        0   366292 2023-04-29 14:23:05.826066 custard-1.1.3/custard/mock/mock.min.js
--rw-r--r--   0        0        0   292581 2023-04-29 14:23:05.826066 custard-1.1.3/custard/mock/mock.old.min.js
--rw-r--r--   0        0        0      696 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/__init__.py
--rw-r--r--   0        0        0     4249 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/api.py
--rw-r--r--   0        0        0     1094 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/async_sqlalchemy.py
--rw-r--r--   0        0        0     2741 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/bases.py
--rw-r--r--   0        0        0     1322 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/iterables.py
--rw-r--r--   0        0        0     1437 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/limit_offset.py
--rw-r--r--   0        0        0     1658 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/pagination.py
--rw-r--r--   0        0        0      847 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/paginator.py
--rw-r--r--   0        0        0     1107 2023-04-29 14:23:05.826066 custard-1.1.3/custard/pagination/sync_sqlalchemy.py
--rw-r--r--   0        0        0      998 2023-04-29 14:23:05.826066 custard-1.1.3/custard/swagger/__init__.py
--rw-r--r--   0        0        0      332 2023-04-29 14:23:05.826066 custard-1.1.3/custard/swagger/exception.py
--rw-r--r--   0        0        0     6423 2023-04-29 14:23:05.826066 custard-1.1.3/custard/swagger/swagger.py
--rw-r--r--   0        0        0      584 2023-04-29 14:23:05.826066 custard-1.1.3/custard/swagger/utils.py
--rw-r--r--   0        0        0      234 2023-04-29 14:23:05.826066 custard-1.1.3/custard/time/__init__.py
--rw-r--r--   0        0        0     6299 2023-04-29 14:23:05.826066 custard-1.1.3/custard/time/dafunc.py
--rw-r--r--   0        0        0     1677 2023-04-29 14:23:05.826066 custard-1.1.3/custard/time/exceptions.py
--rw-r--r--   0        0        0     5752 2023-04-29 14:23:05.826066 custard-1.1.3/custard/time/moment.py
--rw-r--r--   0        0        0     1692 2023-04-29 14:23:05.826066 custard-1.1.3/custard/time/stoppable_thread.py
--rw-r--r--   0        0        0      233 2023-04-29 14:23:05.826066 custard-1.1.3/custard/utils/__init__.py
--rw-r--r--   0        0        0   161226 2023-04-29 14:23:05.830066 custard-1.1.3/custard/utils/area_code.py
--rw-r--r--   0        0        0     3895 2023-04-29 14:23:05.830066 custard-1.1.3/custard/utils/configparser.py
--rw-r--r--   0        0        0     3754 2023-04-29 14:23:05.830066 custard-1.1.3/custard/utils/id_cards.py
--rw-r--r--   0        0        0    85077 2023-04-29 14:23:05.830066 custard-1.1.3/custard/utils/jenkins.py
--rw-r--r--   0        0        0    24805 2023-04-29 14:23:05.830066 custard-1.1.3/custard/utils/multi.py
--rw-r--r--   0        0        0     4555 2023-04-29 14:23:05.830066 custard-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     8799 1970-01-01 00:00:00.000000 custard-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     5589 2023-04-29 16:05:45.087851 custard-1.1.4/README.md
+-rw-r--r--   0        0        0      236 2023-04-29 16:05:45.087851 custard-1.1.4/custard/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-29 16:05:45.087851 custard-1.1.4/custard/core/__init__.py
+-rw-r--r--   0        0        0   770290 2023-04-29 16:05:45.087851 custard-1.1.4/custard/core/decode.py
+-rw-r--r--   0        0        0    28635 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/factory.py
+-rw-r--r--   0        0        0    13726 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/functools.py
+-rw-r--r--   0        0        0     2976 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/kerberos.py
+-rw-r--r--   0        0        0    25958 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/processor.py
+-rw-r--r--   0        0        0    20274 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/regular.py
+-rw-r--r--   0        0        0    15684 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/system.py
+-rw-r--r--   0        0        0    22041 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/useragent.py
+-rw-r--r--   0        0        0     1607 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/xml2dict.py
+-rw-r--r--   0        0        0     1853 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/xprint.py
+-rw-r--r--   0        0        0      463 2023-04-29 16:05:45.091851 custard-1.1.4/custard/crypto/__init__.py
+-rw-r--r--   0        0        0    15682 2023-04-29 16:05:45.091851 custard-1.1.4/custard/crypto/crypto.py
+-rw-r--r--   0        0        0     3257 2023-04-29 16:05:45.091851 custard-1.1.4/custard/crypto/streambody.py
+-rw-r--r--   0        0        0      323 2023-04-29 16:05:45.091851 custard-1.1.4/custard/curl/__init__.py
+-rw-r--r--   0        0        0     5936 2023-04-29 16:05:45.091851 custard-1.1.4/custard/curl/parse.py
+-rw-r--r--   0        0        0      291 2023-04-29 16:05:45.091851 custard-1.1.4/custard/hitfilter/__init__.py
+-rw-r--r--   0        0        0     2972 2023-04-29 16:05:45.091851 custard-1.1.4/custard/hitfilter/hitfilter.py
+-rw-r--r--   0        0        0   761348 2023-04-29 16:05:45.095851 custard-1.1.4/custard/hitfilter/keywords
+-rw-r--r--   0        0        0      418 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/__init__.py
+-rw-r--r--   0        0        0     9386 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/captcha.py
+-rw-r--r--   0        0        0   171508 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/font1.ttf
+-rw-r--r--   0        0        0    42452 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/font2.ttf
+-rw-r--r--   0        0        0    92956 2023-04-29 16:05:45.099851 custard-1.1.4/custard/kaptcha/font3.ttf
+-rw-r--r--   0        0        0   314452 2023-04-29 16:05:45.099851 custard-1.1.4/custard/kaptcha/font4.ttf
+-rw-r--r--   0        0        0     3411 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/README.md
+-rw-r--r--   0        0        0     2584 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/__init__.py
+-rw-r--r--   0        0        0     2818 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/depends.py
+-rw-r--r--   0        0        0      452 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/enums.py
+-rw-r--r--   0        0        0     1705 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/examples/__init__.py
+-rw-r--r--   0        0        0     1962 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/examples/test_depends.py
+-rw-r--r--   0        0        0      438 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/execres.py
+-rw-r--r--   0        0        0     1819 2023-04-29 16:05:45.099851 custard-1.1.4/custard/mock/__init__.py
+-rw-r--r--   0        0        0    14336 2023-04-29 16:05:45.099851 custard-1.1.4/custard/mock/mini_racer.py
+-rw-r--r--   0        0        0   366292 2023-04-29 16:05:45.099851 custard-1.1.4/custard/mock/mock.min.js
+-rw-r--r--   0        0        0   292581 2023-04-29 16:05:45.103851 custard-1.1.4/custard/mock/mock.old.min.js
+-rw-r--r--   0        0        0      696 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/__init__.py
+-rw-r--r--   0        0        0     4249 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/api.py
+-rw-r--r--   0        0        0     1094 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/async_sqlalchemy.py
+-rw-r--r--   0        0        0     2741 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/bases.py
+-rw-r--r--   0        0        0     1322 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/iterables.py
+-rw-r--r--   0        0        0     1437 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/limit_offset.py
+-rw-r--r--   0        0        0     1658 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/pagination.py
+-rw-r--r--   0        0        0      847 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/paginator.py
+-rw-r--r--   0        0        0     1107 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/sync_sqlalchemy.py
+-rw-r--r--   0        0        0      998 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/__init__.py
+-rw-r--r--   0        0        0      332 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/exception.py
+-rw-r--r--   0        0        0     6423 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/swagger.py
+-rw-r--r--   0        0        0      584 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/utils.py
+-rw-r--r--   0        0        0      644 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/__init__.py
+-rw-r--r--   0        0        0     6299 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/dafunc.py
+-rw-r--r--   0        0        0     1677 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/exceptions.py
+-rw-r--r--   0        0        0     5752 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/moment.py
+-rw-r--r--   0        0        0     1692 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/stoppable_thread.py
+-rw-r--r--   0        0        0      233 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/__init__.py
+-rw-r--r--   0        0        0   161226 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/area_code.py
+-rw-r--r--   0        0        0     3895 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/configparser.py
+-rw-r--r--   0        0        0     3754 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/id_cards.py
+-rw-r--r--   0        0        0    85077 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/jenkins.py
+-rw-r--r--   0        0        0    24805 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/multi.py
+-rw-r--r--   0        0        0     4555 2023-04-29 16:05:45.107851 custard-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     8753 1970-01-01 00:00:00.000000 custard-1.1.4/PKG-INFO
```

### Comparing `custard-1.1.3/README.md` & `custard-1.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -92,9 +92,9 @@
 ### 📐PR遵照的原则
 
 custard欢迎任何人为custard添砖加瓦，贡献代码，不过维护者是一个强迫症患者，为了照顾病人，需要提交的pr（pull request）符合一些规范，规范如下：
 
 1. 注释完备，尤其每个新增的方法应按照Python文档规范标明方法说明、参数说明、返回值说明等信息，必要时请添加单元测试，如果愿意，也可以加上你的大名。
 2. custard的缩进按照IDEA 默认（tab）缩进，所以请遵守（不要和我争执空格与tab的问题，这是一个病人的习惯）。
 3. 新加的方法不要使用第三方库的方法，custard遵循无依赖原则（除非在extra模块中加方法工具）。
-4. 请pull request到`dev`分支。custard在5.x版本后使用了新的分支：`master`是主分支，表示已经发布中央库的版本，这个分支不允许pr，也不允许修改。
+4. 请pull request到`dev`分支。`master`是主分支，表示已经发布中央库的版本，这个分支不允许pr，也不允许修改。
 5. 我们如果关闭了你的issue或pr，请不要诧异，这是我们保持问题处理整洁的一种方式，你依旧可以继续讨论，当有讨论结果时我们会重新打开。
```

#### html2text {}

```diff
@@ -49,10 +49,10 @@
 requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ 1.
 æ³¨éå®å¤ï¼å°¤å¶æ¯ä¸ªæ°å¢çæ¹æ³åºæç§Pythonææ¡£è§èæ ææ¹æ³è¯´æãåæ°è¯´æãè¿åå¼è¯´æç­ä¿¡æ¯ï¼å¿è¦æ¶è¯·æ·»å ååæµè¯ï¼å¦ææ¿æï¼ä¹å¯ä»¥å ä¸ä½ çå¤§åã
 2. custardçç¼©è¿æç§IDEA
 é»è®¤ï¼tabï¼ç¼©è¿ï¼æä»¥è¯·éµå®ï¼ä¸è¦åæäºæ§ç©ºæ ¼ä¸tabçé®é¢ï¼è¿æ¯ä¸ä¸ªçäººçä¹ æ¯ï¼ã
 3.
 æ°å çæ¹æ³ä¸è¦ä½¿ç¨ç¬¬ä¸æ¹åºçæ¹æ³ï¼custardéµå¾ªæ ä¾èµååï¼é¤éå¨extraæ¨¡åä¸­å æ¹æ³å·¥å·ï¼ã
 4. è¯·pull
-requestå°`dev`åæ¯ãcustardå¨5.xçæ¬åä½¿ç¨äºæ°çåæ¯ï¼`master`æ¯ä¸»åæ¯ï¼è¡¨ç¤ºå·²ç»åå¸ä¸­å¤®åºççæ¬ï¼è¿ä¸ªåæ¯ä¸åè®¸prï¼ä¹ä¸åè®¸ä¿®æ¹ã
+requestå°`dev`åæ¯ã`master`æ¯ä¸»åæ¯ï¼è¡¨ç¤ºå·²ç»åå¸ä¸­å¤®åºççæ¬ï¼è¿ä¸ªåæ¯ä¸åè®¸prï¼ä¹ä¸åè®¸ä¿®æ¹ã
 5.
 æä»¬å¦æå³é­äºä½ çissueæprï¼è¯·ä¸è¦è¯§å¼ï¼è¿æ¯æä»¬ä¿æé®é¢å¤çæ´æ´çä¸ç§æ¹å¼ï¼ä½ ä¾æ§å¯ä»¥ç»§ç»­è®¨è®ºï¼å½æè®¨è®ºç»ææ¶æä»¬ä¼éæ°æå¼ã
```

### Comparing `custard-1.1.3/custard/core/__init__.py` & `custard-1.1.4/custard/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,27 +23,25 @@
     sync_redis_lock,
     synchronized_lock,
     singleton_lock,
 )
 from .kerberos import Kerberos
 from .processor import DataKitHelper
 from .regular import RegEx
-from .snowflake import generator
 from .system import SystemHand
 from .useragent import firefox, internet_explorer, opera, safari
 from .xprint import xprint
 
 __all__ = [
     "text_type",
     "unidecode",
     "MockHelper",
     "Kerberos",
     "DataKitHelper",
     "RegEx",
-    "generator",
     "SystemHand",
     "firefox",
     "safari",
     "internet_explorer",
     "opera",
     "xprint",
     "ExcContextManager",
```

### Comparing `custard-1.1.3/custard/core/decode.py` & `custard-1.1.4/custard/core/decode.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/core/factory.py` & `custard-1.1.4/custard/core/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from urllib.parse import quote
 
 import pypinyin
 from faker import Faker
 from requests.exceptions import InvalidURL
 from urllib3.exceptions import LocationParseError
 from urllib3.util import parse_url
+from custard.core.processor import DataKitHelper
 
 from custard.time.moment import Moment
 from custard.utils.id_cards import IdNumber
 
 fake = Faker(["zh_CN"])
 logger = logging.getLogger(__name__)
 
@@ -777,15 +778,15 @@
         try:
             return dict.__getitem__(self, item)
         except KeyError:
             value = self[item] = type(self)()
         return value
 
 
-class MsHelper(object):
+class MsHelper(DataKitHelper):
     GLOBAL_PAGE_INDEX = ["page_index", "pageindex"]
     GLOBAL_PAGE_SIZE = ["page_size", "pagesize"]
 
     @classmethod
     def __property__(cls, prop):
         """
         数据转换
@@ -818,15 +819,15 @@
         """
         support_type = (list, float, int, tuple)
         type_err = TypeError("类型错误、仅支持dict")
         if isinstance(data, support_type):
             raise type_err
         if isinstance(data, str):
             try:
-                return json.loads(data)
+                return cls.safely_json_loads(data)
             except json.decoder.JSONDecodeError as decoder_err:
                 raise Exception(decoder_err)
         if isinstance(data, dict):
             return data
         return None
 
     @classmethod
```

### Comparing `custard-1.1.3/custard/core/functools.py` & `custard-1.1.4/custard/core/functools.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/core/kerberos.py` & `custard-1.1.4/custard/core/kerberos.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/core/processor.py` & `custard-1.1.4/custard/core/processor.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,56 +3,56 @@
 """
 @File    :  processor.py
 @Time    :  2022/5/1 8:21 PM
 @Author  :  YuYanQing
 @Version :  1.0
 @Contact :  mryu168@163.com
 @License :  (C)Copyright 2022-2026
-@Desc    :  An XPath for JSON 后置处理
+@Desc    :  数据处理器
 """
 import base64
 import difflib
 import hashlib
 import json
 import logging
 import operator
 import re
+import time
 import xml.dom.minidom
 import xml.etree.ElementTree
 from collections import Counter
 from functools import reduce
 from itertools import zip_longest
 from typing import Any, Dict, Tuple
 from urllib.parse import unquote
 
 from dicttoxml import dicttoxml
 from six import binary_type, text_type
 
-from custard.core.system import SystemHand
 from custard.core.xml2dict import Xml2Dict
 
 logger = logging.getLogger(__name__)
 
 
 SINGLE_UPLOAD_LENGTH = 5 * 1024 * 1024 * 1024  # 单次上传文件最大为5GB
 DEFAULT_CHUNK_SIZE = 1024 * 1024  # 计算MD5值时,文件单次读取的块大小为1MB
 
 
 class DataKitHelper:
     @classmethod
-    def add_dicts(cls, *args: Tuple[Dict, ...]) -> Dict:
+    def sub_dict_value(cls, *args: Tuple[Dict, ...]) -> Dict:
         """
         Adds two or more dicts together. Common keys will have their values added.
 
         Returns:
         Example:
             >>> t1 = {'a':1, 'b':2}
             >>> t2 = {'b':1, 'c':3}
             >>> t3 = {'d':5}
-            >>> DataKit.add_dicts(t1, t2, t3)
+            >>> DataKit.sub_dict_value(t1, t2, t3)
             {'a': 1, 'c': 3, 'b': 3, 'd': 5}
         """
 
         counters = [Counter(arg) for arg in args]
         return dict(reduce(operator.add, counters))
 
     @classmethod
@@ -104,17 +104,15 @@
                         dict_map[key][i] = cls.convert_type(dict_map=dict_map[key][i], disable_data=disable_data)
                 elif isinstance(dict_map[key], dict):
                     dict_map[key] = cls.convert_type(dict_map=dict_map[key], disable_data=disable_data)
                 elif str(dict_map[key]).isdigit() and str(key) not in disable_data:
                     dict_map[key] = int(dict_map[key])
                 elif str(dict_map[key]) == "null":  # 统一处理str无法转化None
                     dict_map[key] = None
-            return (
-                json.dumps(dict_map, ensure_ascii=False).replace('\\"', '"').replace('"{', "{").replace('}"', "}")
-            )  # 临时打个补丁 后续若报错则需再次做兼容
+            return dict_map
         else:
             raise TypeError("传入的参数不是dict类型 %s" % (type(dict_map)))
 
     @classmethod
     def dict_to_from(cls, post_data):
         """
         字典转xwww-from格式
@@ -142,111 +140,14 @@
                     raise Exception(err)
                 converted_dict[key] = unquote(value)
             return converted_dict
         else:
             return post_data
 
     @classmethod
-    def list_sub_dict(cls, origin_list):
-        """
-        list转dict
-        :param origin_list: (list) [{"name": "v", "value": "1"},{"name": "w", "value": "2"}]
-        :return: dict:{"v": "1", "w": "2"}
-        """
-        return {item["name"]: item.get("value") for item in origin_list}
-
-    @classmethod
-    def dict_capital_to_lower(cls, dict_map):
-        """
-        dict中的key转换小写
-        :param dict_map:
-        :return:
-        """
-        new_dict = {}
-        for key in list(dict_map.keys()):
-            new_dict[key.lower()] = dict_map[key]
-        return new_dict
-
-    @classmethod
-    def capital_lower_to_dict(cls, dict_map):
-        """
-        dict中的key转换大写
-        :param dict_map:
-        :return:
-        """
-        new_dict = {}
-        for key in list(dict_map.keys()):
-            new_dict[str(key).upper()] = dict_map[key]
-        return new_dict
-
-    @classmethod
-    def diff_json(cls, filename1, filename2, targetPath):
-        """
-        比较两个文件内容的md5值并输出到html文件中
-        :param filename1:
-        :param filename2:
-        :param targetPath:
-        :return:
-        """
-        file1Md5 = hashlib.md5.new(filename1.read()).digest()
-        file2Md5 = hashlib.md5.new(filename2.read()).digest()
-        if file1Md5 != file2Md5:
-            text1_lines = SystemHand.load_file(filename1, "json")
-            text2_lines = SystemHand.load_file(filename2, "json")
-            d = difflib.HtmlDiff()
-            result = d.make_file(text1_lines, text2_lines, filename1, filename2, context=True)
-            # 内容保存到result.html文件中
-            try:
-                with open(targetPath, "a", encoding="utf-8") as result_file:
-                    result_file.write(result)
-            except Exception as e:
-                logger.error("写入文件失败:" + e)
-
-    @classmethod
-    def is_json_format(cls, raw_data):
-        """
-        用于判断一个字符串是否符合Json格式
-        :param raw_data:
-        :return:
-        """
-        if isinstance(raw_data, str):
-            try:
-                json.loads(raw_data, encoding="utf-8")
-            except ValueError:
-                return False
-            else:
-                return True
-        else:
-            return False
-
-    @classmethod
-    def json_to_dict(cls, data):
-        """
-        Json转字典
-        :param data: 数据来源
-        :return:
-        """
-        return json.loads(data)
-
-    @classmethod
-    def dict_to_json(cls, data, sort_keys=False, ensure_ascii=False, indent=4, separators=(",", ": ")):
-        """
-        字典转Json
-        :param data: 数据来源
-        :return:
-        """
-        return json.dumps(
-            data,
-            ensure_ascii=ensure_ascii,
-            sort_keys=sort_keys,
-            indent=indent,
-            separators=separators,
-        )
-
-    @classmethod
     def json_to_schema(cls, data, result=None):
         """
         json递归生成schema
         :param data:
         :param result:
         :return:
         Example::
@@ -371,15 +272,15 @@
         Examples:
             >>> origin_dict = { "Name": "", "Request": "", "URL": "", "METHOD": "", "Headers": "", "Data": ""}
             >>> DataKitHelper.lower_dict_keys(origin_dict)
         """
         if not origin_dict or not isinstance(origin_dict, dict):
             return origin_dict
 
-        return {key.lower(): value for key, value in origin_dict.items()}
+        return {str(key).lower(): value for key, value in origin_dict.items()}
 
     @classmethod
     def upper_dict_keys(cls, origin_dict: Dict):
         """
         convert keys in dict to lower case
         Args:
             origin_dict: mapping data structure
@@ -390,15 +291,15 @@
         Examples:
             >>> origin_dict = {'name': '', 'request': '', 'url': '', 'method': '', 'headers': '', 'data': ''}
             >>> DataKitHelper.upper_dict_keys(origin_dict)
         """
         if not origin_dict or not isinstance(origin_dict, dict):
             return origin_dict
 
-        return {key.upper(): value for key, value in origin_dict.items()}
+        return {str(key).upper(): value for key, value in origin_dict.items()}
 
     @classmethod
     def omit_long_data(cls, body, omit_len=512):
         """omit too long str/bytes"""
         if not isinstance(body, (str, bytes)):
             return body
 
@@ -522,27 +423,27 @@
     def format_values(cls, data):
         """格式化headers和params中的values为bytes"""
         for i in data:
             data[i] = cls.to_bytes(data[i])
         return data
 
     @classmethod
-    def is_json(cls, target_data):
+    def is_json(cls, raw_data, encoding="utf-8"):
         """
         判断目标源是否为json类型
         Args:
             target_data:
         Returns:
         Examples:
             >>> list = ["1235678",{"key1":"value", "key2":"value"}]
             >>> DataKitHelper.is_json()
         """
-        if isinstance(target_data, str):
+        if isinstance(raw_data, str):
             try:
-                json.loads(target_data)
+                json.loads(raw_data, encoding=encoding)
             except ValueError:
                 return False
             return True
         else:
             return False
 
     @classmethod
@@ -598,29 +499,83 @@
             for i in iter:
                 result.update(i)
         else:
             result = reduce(lambda x, y: list(x) + list(y), iter)
         return result
 
     @classmethod
-    def safely_json_loads(cls, json_str, default_type=dict, escape=True):
+    def safely_json_loads(
+        cls,
+        value,
+        object_hook: dict = None,
+        parse_float=None,
+        parse_int=None,
+        parse_constant=None,
+        object_pairs_hook=None,
+        err_detail="解析JSON字符串并将其转换为Python字典失败",
+    ):
         """
         返回安全的json类型
         Args:
-            json_str: 要被loads的字符串
-            default_type: 若load失败希望得到的对象类型
-            escape: 是否将单引号变成双引号
-        Returns:
-        """
-        if not json_str:
-            return default_type()
-        elif escape:
-            return json.loads(default_type(json_str))
-        else:
-            return json.loads(json_str)
+            value (_type_): _description_
+            object_hook (_type_, optional): _description_. Defaults to None.
+            parse_float (_type_, optional): _description_. Defaults to None.
+            parse_int (_type_, optional): _description_. Defaults to None.
+            parse_constant (_type_, optional): _description_. Defaults to None.
+            object_pairs_hook (_type_, optional): _description_. Defaults to None.
+            err_detail (str, optional): _description_. Defaults to "解析JSON字符串并将其转换为Python字典失败".
+
+        Raises:
+            Exception: _description_
+
+        Returns:
+            _type_: _description_
+        """
+        try:
+            value = json.loads(
+                value,
+                object_hook=object_hook,
+                parse_float=parse_float,
+                parse_int=parse_int,
+                parse_constant=parse_constant,
+                object_pairs_hook=object_pairs_hook,
+            )
+        except Exception as e:
+            raise Exception(f"{err_detail}: {e}")
+        return value
+
+    @classmethod
+    def safely_json_dumps(
+        cls,
+        obj,
+        skipkeys=False,
+        ensure_ascii=True,
+        check_circular=True,
+        allow_nan=True,
+        indent=None,
+        separators=None,
+        default=None,
+        sort_keys=False,
+        err_detail="解析obj序列化为JSON格式字符串失败",
+    ):
+        try:
+            value = json.dumps(
+                obj,
+                skipkeys=skipkeys,
+                ensure_ascii=ensure_ascii,
+                check_circular=check_circular,
+                allow_nan=allow_nan,
+                indent=indent,
+                separators=separators,
+                default=default,
+                sort_keys=sort_keys,
+            )
+        except Exception as e:
+            raise Exception(f"{err_detail}: {e}")
+        return value
 
     @classmethod
     def format_html_string(cls, html):
         """
         格式化html, 去掉多余的字符,类,script等。
         Args:
             html:
@@ -655,19 +610,19 @@
         Returns:
         Examples:
             # 将两个相同长度的列表转换成字典
             >>> print(DataKitHelper.data_type_convert(original=(["key1","key2"],["value1","value2"]), target_type="dict"))
             # 将两个不同长度的列表转换成字典
             >>> print(DataKitHelper.data_type_convert(original=(["key1","key2","key3"],["value1","value2"]), target_type="dict"))
             # 将json转化为字典
-            >>> print(DataKitHelper.data_type_convert(original='{"errcode": 401,"errmsg": "[POST]","data": null}', target_type="dict"))
+            >>> print(DataKitHelper.data_type_convert(original='{"errcode": 401,"errs": "[POST]","data": null}', target_type="dict"))
             # 将dict转化为json
-            >>> print(DataKitHelper.data_type_convert(original={'errcode': 401,'errmsg': 'POST','data': True}, target_type="json"))
+            >>> print(DataKitHelper.data_type_convert(original={'errcode': 401,'errs': 'POST','data': True}, target_type="json"))
             # 将字典列表转换为单个字典
-            >>> print(DataKitHelper.data_type_convert(original=[{"errcode": 401},{"errmsg": "[POST]","data": True}], target_type="dict"))
+            >>> print(DataKitHelper.data_type_convert(original=[{"errcode": 401},{"errs": "[POST]","data": True}], target_type="dict"))
         """
         if isinstance(original, dict) and target_type == "json":
             return json.dumps(original)
         elif isinstance(original, tuple) and target_type == "dict":
             is_equal_bool = len(original[0]) == len(original[1])
             if is_equal_bool:
                 return dict(original)
@@ -675,15 +630,15 @@
                 return dict(zip_longest(original[0], original[1]))
         elif isinstance(original, list) and target_type == "dict":
             temp = {}
             for index in original:
                 temp.update(index)
             return temp
         elif cls.is_json(original) and target_type == "dict":
-            return json.loads(original)
+            return cls.safely_json_loads(original)
         return None
 
     @classmethod
     def parser(cls, keyword):
         """
         获取后续的字符对应前面出现过的字符的下标
         Args:
@@ -729,7 +684,74 @@
             last_num = pay_num - money
             if last_num < 0:
                 continue
             try:
                 yield cls.charged(last_num, money_num)
             except ValueError:
                 continue
+
+
+class Snowflake:
+    epoch = 1292978355588
+    worker_id_bits = 5
+    data_center_id_bits = 5
+    max_worker_id = -1 ^ (-1 << worker_id_bits)
+    max_data_center_id = -1 ^ (-1 << data_center_id_bits)
+    sequence_bits = 12
+    worker_id_shift = sequence_bits
+    data_center_id_shift = sequence_bits + worker_id_bits
+    timestamp_left_shift = sequence_bits + worker_id_bits + data_center_id_bits
+    sequence_mask = -1 ^ (-1 << sequence_bits)
+
+    @classmethod
+    def snowflake_to_timestamp(cls, _id):
+        _id = _id >> 22  # strip the lower 22 bits
+        _id += cls.epoch  # adjust for twitter epoch
+        _id = _id / 1000  # convert from milliseconds to seconds
+        return _id
+
+    @classmethod
+    def generator(cls, worker_id, data_center_id, sleep=lambda x: time.sleep(x / 1000.0)):
+        """
+        生成器
+        Args:
+            worker_id (_type_): _description_
+            data_center_id (_type_): _description_
+            sleep (_type_, optional): _description_. Defaults to lambda x:time.sleep(x / 1000.0).
+        Examples:
+            >>> s = generator(1, 1)
+            >>> for _i in range(1000000):
+            ...     print(s.__next__())
+        Yields:
+            _type_: _description_
+        """
+        assert 0 <= worker_id <= cls.max_worker_id
+        assert 0 <= data_center_id <= cls.max_data_center_id
+
+        last_timestamp = -1
+        sequence = 0
+
+        while True:
+            timestamp = int(time.time() * 1000)
+
+            if last_timestamp > timestamp:
+                print("clock is moving backwards. waiting until %i" % last_timestamp)
+                sleep(last_timestamp - timestamp)
+                continue
+
+            if last_timestamp == timestamp:
+                sequence = (sequence + 1) & cls.sequence_mask
+                if sequence == 0:
+                    print("sequence overrun")
+                    sequence = -1 & cls.sequence_mask
+                    sleep(1)
+                    continue
+            else:
+                sequence = 0
+
+            last_timestamp = timestamp
+            yield (
+                ((timestamp - cls.epoch) << cls.timestamp_left_shift)
+                | (data_center_id << cls.data_center_id_shift)
+                | (worker_id << cls.worker_id_shift)
+                | sequence
+            )
```

### Comparing `custard-1.1.3/custard/core/regular.py` & `custard-1.1.4/custard/core/regular.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/core/system.py` & `custard-1.1.4/custard/core/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     # PyYAML version >= 5.1
     yaml.warnings({"YAMLLoadWarning": False})
 
 
 logger = logging.getLogger(__name__)
 
 
-class SystemHand:
+class SystemHand(DataKitHelper):
     @classmethod
     def shell(cls, command):
         output, errors = subprocess.Popen(
             command,
             shell=True,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
@@ -416,15 +416,15 @@
     @classmethod
     def json_to_yaml(cls, json_file):
         """
         json文件格式转yaml
         """
         if json_file.endswith("json"):
             with open(json_file, "r") as pf:
-                json_to_dict = json.loads(pf.read())
+                json_to_dict = cls.safely_json_loads(pf.read())
             yaml_file = json_file.replace(".json", ".yaml")
             with open(yaml_file, "w") as fp:
                 yaml.safe_dump(json_to_dict, stream=fp, default_flow_style=False)
                 return True
         return False
 
     @classmethod
```

### Comparing `custard-1.1.3/custard/core/useragent.py` & `custard-1.1.4/custard/core/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/core/xml2dict.py` & `custard-1.1.4/custard/core/xml2dict.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/core/xprint.py` & `custard-1.1.4/custard/core/xprint.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,16 +64,7 @@
                 f'\033[35m{time.strftime("%H:%M:%S")}{single_space}"{file_name}:{line}"{single_space}'
                 f"{sep.join(args)}{single_space}{end}\033[0m",
             )
         else:
             stdout_write(f'{time.strftime("%H:%M:%S")}\t"{file_name}:{line}"{single_space}{sep.join(args)}{end}')
     else:
         print_raw(*args, sep=sep, end=end, file=file)
-
-
-if __name__ == "__main__":
-    xprint(156, "def")
-    try:
-        with open("a") as file:
-            file.read()
-    except FileNotFoundError as e:
-        xprint(e)
```

### Comparing `custard-1.1.3/custard/crypto/crypto.py` & `custard-1.1.4/custard/crypto/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,16 @@
     Returns:
 
     """
     if isinstance(str_, text_type):
         try:
             return str_.encode("utf-8")
         except UnicodeEncodeError:
-            raise CryptoException("your unicode strings can not encoded in utf8, utf8 support only!")
+            detail = "your unicode strings can not encoded in utf8, utf8 support only!"
+            raise CryptoException(detail)
     return str_
 
 
 def random_key(key_len):
     """
 
     Args:
```

### Comparing `custard-1.1.3/custard/crypto/streambody.py` & `custard-1.1.4/custard/crypto/streambody.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/curl/parse.py` & `custard-1.1.4/custard/curl/parse.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import warnings
 from http.cookies import SimpleCookie
 from shlex import split
 from urllib.parse import urlparse
 
 from w3lib.http import basic_auth_header
 
+from custard.core.processor import DataKitHelper
 
-class CurlParser(argparse.ArgumentParser):
+
+class CurlParser(argparse.ArgumentParser, DataKitHelper):
     def error(self, message):
         error_msg = "There was an error parsing the curl command: {}".format(message)
         raise ValueError(error_msg)
 
 
 # 自定义解析的内容
 curl_parser = CurlParser()
@@ -93,15 +95,15 @@
         user, password = parsed_args.auth.split(":", 1)
         headers.append(("Authorization", basic_auth_header(user, password)))
     if headers:
         result["headers"] = headers
     if cookies:
         result["cookies"] = cookies
     if parsed_args.data:
-        body_ = json.loads(parsed_args.data)
+        body_ = DataKitHelper.safely_json_loads(parsed_args.data)
         result["body"] = body_
     if forms:
         if content_type == "application/x-www-form-urlencoded":
             result["data-urlencode"] = forms
         else:
             result["form"] = forms
     # print("---parsed_curl_dumps---", json.dumps(result))
```

### Comparing `custard-1.1.3/custard/hitfilter/hitfilter.py` & `custard-1.1.4/custard/hitfilter/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/hitfilter/keywords` & `custard-1.1.4/custard/hitfilter/keywords`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/kaptcha/captcha.py` & `custard-1.1.4/custard/kaptcha/captcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/kaptcha/font1.ttf` & `custard-1.1.4/custard/kaptcha/font1.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/kaptcha/font2.ttf` & `custard-1.1.4/custard/kaptcha/font2.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/kaptcha/font3.ttf` & `custard-1.1.4/custard/kaptcha/font3.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/kaptcha/font4.ttf` & `custard-1.1.4/custard/kaptcha/font4.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/limiter/README.md` & `custard-1.1.4/custard/limiter/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/limiter/__init__.py` & `custard-1.1.4/custard/limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/limiter/depends.py` & `custard-1.1.4/custard/limiter/depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/limiter/examples/__init__.py` & `custard-1.1.4/custard/limiter/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/limiter/examples/test_depends.py` & `custard-1.1.4/custard/limiter/examples/test_depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/mock/__init__.py` & `custard-1.1.4/custard/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/mock/mini_racer.py` & `custard-1.1.4/custard/mock/mini_racer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/mock/mock.min.js` & `custard-1.1.4/custard/mock/mock.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/mock/mock.old.min.js` & `custard-1.1.4/custard/mock/mock.old.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/__init__.py` & `custard-1.1.4/custard/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/api.py` & `custard-1.1.4/custard/pagination/api.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/async_sqlalchemy.py` & `custard-1.1.4/custard/pagination/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/bases.py` & `custard-1.1.4/custard/pagination/bases.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/iterables.py` & `custard-1.1.4/custard/pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/limit_offset.py` & `custard-1.1.4/custard/pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/pagination.py` & `custard-1.1.4/custard/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/paginator.py` & `custard-1.1.4/custard/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/pagination/sync_sqlalchemy.py` & `custard-1.1.4/custard/pagination/sync_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/swagger/__init__.py` & `custard-1.1.4/custard/swagger/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/swagger/swagger.py` & `custard-1.1.4/custard/swagger/swagger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/swagger/utils.py` & `custard-1.1.4/custard/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/time/dafunc.py` & `custard-1.1.4/custard/time/dafunc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/time/exceptions.py` & `custard-1.1.4/custard/time/exceptions.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/time/moment.py` & `custard-1.1.4/custard/time/moment.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/time/stoppable_thread.py` & `custard-1.1.4/custard/time/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/utils/area_code.py` & `custard-1.1.4/custard/utils/area_code.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/utils/configparser.py` & `custard-1.1.4/custard/utils/configparser.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/utils/id_cards.py` & `custard-1.1.4/custard/utils/id_cards.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/utils/jenkins.py` & `custard-1.1.4/custard/utils/jenkins.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/custard/utils/multi.py` & `custard-1.1.4/custard/utils/multi.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.3/pyproject.toml` & `custard-1.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "custard"
-version = "1.1.3"
+version = "1.1.4"
 description = "custard easy to learn, fast to code, ready for production"
 readme = "README.md"
 license = "MIT"
 authors = ["Kamalyes <mryu168@163.com>",]
 
 repository = "https://github.com/kamalyes/custard"
```

### Comparing `custard-1.1.3/PKG-INFO` & `custard-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custard
-Version: 1.1.3
+Version: 1.1.4
 Summary: custard easy to learn, fast to code, ready for production
 Home-page: https://github.com/kamalyes/custard
 License: MIT
 Author: Kamalyes
 Author-email: mryu168@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -159,10 +159,10 @@
 ### 📐PR遵照的原则
 
 custard欢迎任何人为custard添砖加瓦，贡献代码，不过维护者是一个强迫症患者，为了照顾病人，需要提交的pr（pull request）符合一些规范，规范如下：
 
 1. 注释完备，尤其每个新增的方法应按照Python文档规范标明方法说明、参数说明、返回值说明等信息，必要时请添加单元测试，如果愿意，也可以加上你的大名。
 2. custard的缩进按照IDEA 默认（tab）缩进，所以请遵守（不要和我争执空格与tab的问题，这是一个病人的习惯）。
 3. 新加的方法不要使用第三方库的方法，custard遵循无依赖原则（除非在extra模块中加方法工具）。
-4. 请pull request到`dev`分支。custard在5.x版本后使用了新的分支：`master`是主分支，表示已经发布中央库的版本，这个分支不允许pr，也不允许修改。
+4. 请pull request到`dev`分支。`master`是主分支，表示已经发布中央库的版本，这个分支不允许pr，也不允许修改。
 5. 我们如果关闭了你的issue或pr，请不要诧异，这是我们保持问题处理整洁的一种方式，你依旧可以继续讨论，当有讨论结果时我们会重新打开。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custard Version: 1.1.3 Summary: custard easy to
+Metadata-Version: 2.1 Name: custard Version: 1.1.4 Summary: custard easy to
 learn, fast to code, ready for production Home-page: https://github.com/
 kamalyes/custard License: MIT Author: Kamalyes Author-email: mryu168@163.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
@@ -91,10 +91,10 @@
 requestï¼ç¬¦åä¸äºè§èï¼è§èå¦ä¸ï¼ 1.
 æ³¨éå®å¤ï¼å°¤å¶æ¯ä¸ªæ°å¢çæ¹æ³åºæç§Pythonææ¡£è§èæ ææ¹æ³è¯´æãåæ°è¯´æãè¿åå¼è¯´æç­ä¿¡æ¯ï¼å¿è¦æ¶è¯·æ·»å ååæµè¯ï¼å¦ææ¿æï¼ä¹å¯ä»¥å ä¸ä½ çå¤§åã
 2. custardçç¼©è¿æç§IDEA
 é»è®¤ï¼tabï¼ç¼©è¿ï¼æä»¥è¯·éµå®ï¼ä¸è¦åæäºæ§ç©ºæ ¼ä¸tabçé®é¢ï¼è¿æ¯ä¸ä¸ªçäººçä¹ æ¯ï¼ã
 3.
 æ°å çæ¹æ³ä¸è¦ä½¿ç¨ç¬¬ä¸æ¹åºçæ¹æ³ï¼custardéµå¾ªæ ä¾èµååï¼é¤éå¨extraæ¨¡åä¸­å æ¹æ³å·¥å·ï¼ã
 4. è¯·pull
-requestå°`dev`åæ¯ãcustardå¨5.xçæ¬åä½¿ç¨äºæ°çåæ¯ï¼`master`æ¯ä¸»åæ¯ï¼è¡¨ç¤ºå·²ç»åå¸ä¸­å¤®åºççæ¬ï¼è¿ä¸ªåæ¯ä¸åè®¸prï¼ä¹ä¸åè®¸ä¿®æ¹ã
+requestå°`dev`åæ¯ã`master`æ¯ä¸»åæ¯ï¼è¡¨ç¤ºå·²ç»åå¸ä¸­å¤®åºççæ¬ï¼è¿ä¸ªåæ¯ä¸åè®¸prï¼ä¹ä¸åè®¸ä¿®æ¹ã
 5.
 æä»¬å¦æå³é­äºä½ çissueæprï¼è¯·ä¸è¦è¯§å¼ï¼è¿æ¯æä»¬ä¿æé®é¢å¤çæ´æ´çä¸ç§æ¹å¼ï¼ä½ ä¾æ§å¯ä»¥ç»§ç»­è®¨è®ºï¼å½æè®¨è®ºç»ææ¶æä»¬ä¼éæ°æå¼ã
```

