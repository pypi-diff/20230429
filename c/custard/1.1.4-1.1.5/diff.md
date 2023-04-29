# Comparing `tmp/custard-1.1.4.tar.gz` & `tmp/custard-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custard-1.1.4.tar", max compression
+gzip compressed data, was "custard-1.1.5.tar", max compression
```

## Comparing `custard-1.1.4.tar` & `custard-1.1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5589 2023-04-29 16:05:45.087851 custard-1.1.4/README.md
--rw-r--r--   0        0        0      236 2023-04-29 16:05:45.087851 custard-1.1.4/custard/__init__.py
--rw-r--r--   0        0        0     1192 2023-04-29 16:05:45.087851 custard-1.1.4/custard/core/__init__.py
--rw-r--r--   0        0        0   770290 2023-04-29 16:05:45.087851 custard-1.1.4/custard/core/decode.py
--rw-r--r--   0        0        0    28635 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/factory.py
--rw-r--r--   0        0        0    13726 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/functools.py
--rw-r--r--   0        0        0     2976 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/kerberos.py
--rw-r--r--   0        0        0    25958 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/processor.py
--rw-r--r--   0        0        0    20274 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/regular.py
--rw-r--r--   0        0        0    15684 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/system.py
--rw-r--r--   0        0        0    22041 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/useragent.py
--rw-r--r--   0        0        0     1607 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/xml2dict.py
--rw-r--r--   0        0        0     1853 2023-04-29 16:05:45.091851 custard-1.1.4/custard/core/xprint.py
--rw-r--r--   0        0        0      463 2023-04-29 16:05:45.091851 custard-1.1.4/custard/crypto/__init__.py
--rw-r--r--   0        0        0    15682 2023-04-29 16:05:45.091851 custard-1.1.4/custard/crypto/crypto.py
--rw-r--r--   0        0        0     3257 2023-04-29 16:05:45.091851 custard-1.1.4/custard/crypto/streambody.py
--rw-r--r--   0        0        0      323 2023-04-29 16:05:45.091851 custard-1.1.4/custard/curl/__init__.py
--rw-r--r--   0        0        0     5936 2023-04-29 16:05:45.091851 custard-1.1.4/custard/curl/parse.py
--rw-r--r--   0        0        0      291 2023-04-29 16:05:45.091851 custard-1.1.4/custard/hitfilter/__init__.py
--rw-r--r--   0        0        0     2972 2023-04-29 16:05:45.091851 custard-1.1.4/custard/hitfilter/hitfilter.py
--rw-r--r--   0        0        0   761348 2023-04-29 16:05:45.095851 custard-1.1.4/custard/hitfilter/keywords
--rw-r--r--   0        0        0      418 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/__init__.py
--rw-r--r--   0        0        0     9386 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/captcha.py
--rw-r--r--   0        0        0   171508 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/font1.ttf
--rw-r--r--   0        0        0    42452 2023-04-29 16:05:45.095851 custard-1.1.4/custard/kaptcha/font2.ttf
--rw-r--r--   0        0        0    92956 2023-04-29 16:05:45.099851 custard-1.1.4/custard/kaptcha/font3.ttf
--rw-r--r--   0        0        0   314452 2023-04-29 16:05:45.099851 custard-1.1.4/custard/kaptcha/font4.ttf
--rw-r--r--   0        0        0     3411 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/README.md
--rw-r--r--   0        0        0     2584 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/__init__.py
--rw-r--r--   0        0        0     2818 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/depends.py
--rw-r--r--   0        0        0      452 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/enums.py
--rw-r--r--   0        0        0     1705 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/examples/__init__.py
--rw-r--r--   0        0        0     1962 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/examples/test_depends.py
--rw-r--r--   0        0        0      438 2023-04-29 16:05:45.099851 custard-1.1.4/custard/limiter/execres.py
--rw-r--r--   0        0        0     1819 2023-04-29 16:05:45.099851 custard-1.1.4/custard/mock/__init__.py
--rw-r--r--   0        0        0    14336 2023-04-29 16:05:45.099851 custard-1.1.4/custard/mock/mini_racer.py
--rw-r--r--   0        0        0   366292 2023-04-29 16:05:45.099851 custard-1.1.4/custard/mock/mock.min.js
--rw-r--r--   0        0        0   292581 2023-04-29 16:05:45.103851 custard-1.1.4/custard/mock/mock.old.min.js
--rw-r--r--   0        0        0      696 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/__init__.py
--rw-r--r--   0        0        0     4249 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/api.py
--rw-r--r--   0        0        0     1094 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/async_sqlalchemy.py
--rw-r--r--   0        0        0     2741 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/bases.py
--rw-r--r--   0        0        0     1322 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/iterables.py
--rw-r--r--   0        0        0     1437 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/limit_offset.py
--rw-r--r--   0        0        0     1658 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/pagination.py
--rw-r--r--   0        0        0      847 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/paginator.py
--rw-r--r--   0        0        0     1107 2023-04-29 16:05:45.103851 custard-1.1.4/custard/pagination/sync_sqlalchemy.py
--rw-r--r--   0        0        0      998 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/__init__.py
--rw-r--r--   0        0        0      332 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/exception.py
--rw-r--r--   0        0        0     6423 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/swagger.py
--rw-r--r--   0        0        0      584 2023-04-29 16:05:45.103851 custard-1.1.4/custard/swagger/utils.py
--rw-r--r--   0        0        0      644 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/__init__.py
--rw-r--r--   0        0        0     6299 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/dafunc.py
--rw-r--r--   0        0        0     1677 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/exceptions.py
--rw-r--r--   0        0        0     5752 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/moment.py
--rw-r--r--   0        0        0     1692 2023-04-29 16:05:45.103851 custard-1.1.4/custard/time/stoppable_thread.py
--rw-r--r--   0        0        0      233 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/__init__.py
--rw-r--r--   0        0        0   161226 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/area_code.py
--rw-r--r--   0        0        0     3895 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/configparser.py
--rw-r--r--   0        0        0     3754 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/id_cards.py
--rw-r--r--   0        0        0    85077 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/jenkins.py
--rw-r--r--   0        0        0    24805 2023-04-29 16:05:45.103851 custard-1.1.4/custard/utils/multi.py
--rw-r--r--   0        0        0     4555 2023-04-29 16:05:45.107851 custard-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     8753 1970-01-01 00:00:00.000000 custard-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     5589 2023-04-29 16:20:12.886455 custard-1.1.5/README.md
+-rw-r--r--   0        0        0      236 2023-04-29 16:20:12.886455 custard-1.1.5/custard/__init__.py
+-rw-r--r--   0        0        0     1192 2023-04-29 16:20:12.886455 custard-1.1.5/custard/core/__init__.py
+-rw-r--r--   0        0        0   770290 2023-04-29 16:20:12.886455 custard-1.1.5/custard/core/decode.py
+-rw-r--r--   0        0        0    28635 2023-04-29 16:20:12.886455 custard-1.1.5/custard/core/factory.py
+-rw-r--r--   0        0        0    13726 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/functools.py
+-rw-r--r--   0        0        0     2976 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/kerberos.py
+-rw-r--r--   0        0        0    25958 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/processor.py
+-rw-r--r--   0        0        0    20274 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/regular.py
+-rw-r--r--   0        0        0    15684 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/system.py
+-rw-r--r--   0        0        0    22041 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/useragent.py
+-rw-r--r--   0        0        0     1607 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/xml2dict.py
+-rw-r--r--   0        0        0     1853 2023-04-29 16:20:12.890456 custard-1.1.5/custard/core/xprint.py
+-rw-r--r--   0        0        0      463 2023-04-29 16:20:12.890456 custard-1.1.5/custard/crypto/__init__.py
+-rw-r--r--   0        0        0    15682 2023-04-29 16:20:12.890456 custard-1.1.5/custard/crypto/crypto.py
+-rw-r--r--   0        0        0     3257 2023-04-29 16:20:12.890456 custard-1.1.5/custard/crypto/streambody.py
+-rw-r--r--   0        0        0      323 2023-04-29 16:20:12.890456 custard-1.1.5/custard/curl/__init__.py
+-rw-r--r--   0        0        0     5936 2023-04-29 16:20:12.890456 custard-1.1.5/custard/curl/parse.py
+-rw-r--r--   0        0        0      291 2023-04-29 16:20:12.890456 custard-1.1.5/custard/hitfilter/__init__.py
+-rw-r--r--   0        0        0     2972 2023-04-29 16:20:12.890456 custard-1.1.5/custard/hitfilter/hitfilter.py
+-rw-r--r--   0        0        0   761348 2023-04-29 16:20:12.894456 custard-1.1.5/custard/hitfilter/keywords
+-rw-r--r--   0        0        0      418 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/__init__.py
+-rw-r--r--   0        0        0     9386 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/captcha.py
+-rw-r--r--   0        0        0   171508 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/font1.ttf
+-rw-r--r--   0        0        0    42452 2023-04-29 16:20:12.894456 custard-1.1.5/custard/kaptcha/font2.ttf
+-rw-r--r--   0        0        0    92956 2023-04-29 16:20:12.898455 custard-1.1.5/custard/kaptcha/font3.ttf
+-rw-r--r--   0        0        0   314452 2023-04-29 16:20:12.898455 custard-1.1.5/custard/kaptcha/font4.ttf
+-rw-r--r--   0        0        0     3411 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/README.md
+-rw-r--r--   0        0        0     2584 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/__init__.py
+-rw-r--r--   0        0        0     2818 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/depends.py
+-rw-r--r--   0        0        0      452 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/enums.py
+-rw-r--r--   0        0        0     1705 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/examples/__init__.py
+-rw-r--r--   0        0        0     1962 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/examples/test_depends.py
+-rw-r--r--   0        0        0      438 2023-04-29 16:20:12.898455 custard-1.1.5/custard/limiter/execres.py
+-rw-r--r--   0        0        0     1819 2023-04-29 16:20:12.898455 custard-1.1.5/custard/mock/__init__.py
+-rw-r--r--   0        0        0    14336 2023-04-29 16:20:12.898455 custard-1.1.5/custard/mock/mini_racer.py
+-rw-r--r--   0        0        0   366292 2023-04-29 16:20:12.902455 custard-1.1.5/custard/mock/mock.min.js
+-rw-r--r--   0        0        0   292581 2023-04-29 16:20:12.902455 custard-1.1.5/custard/mock/mock.old.min.js
+-rw-r--r--   0        0        0      696 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/__init__.py
+-rw-r--r--   0        0        0     4249 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/api.py
+-rw-r--r--   0        0        0     1094 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/async_sqlalchemy.py
+-rw-r--r--   0        0        0     2741 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/bases.py
+-rw-r--r--   0        0        0     1322 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/iterables.py
+-rw-r--r--   0        0        0     1437 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/limit_offset.py
+-rw-r--r--   0        0        0     1658 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/pagination.py
+-rw-r--r--   0        0        0      847 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/paginator.py
+-rw-r--r--   0        0        0     1107 2023-04-29 16:20:12.902455 custard-1.1.5/custard/pagination/sync_sqlalchemy.py
+-rw-r--r--   0        0        0      990 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/__init__.py
+-rw-r--r--   0        0        0      328 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/exception.py
+-rw-r--r--   0        0        0     6423 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/swagger.py
+-rw-r--r--   0        0        0      584 2023-04-29 16:20:12.902455 custard-1.1.5/custard/swagger/utils.py
+-rw-r--r--   0        0        0      644 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/__init__.py
+-rw-r--r--   0        0        0     6299 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/dafunc.py
+-rw-r--r--   0        0        0     1673 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/exceptions.py
+-rw-r--r--   0        0        0     5752 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/moment.py
+-rw-r--r--   0        0        0     1692 2023-04-29 16:20:12.902455 custard-1.1.5/custard/time/stoppable_thread.py
+-rw-r--r--   0        0        0      233 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/__init__.py
+-rw-r--r--   0        0        0   161226 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/area_code.py
+-rw-r--r--   0        0        0     3895 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/configparser.py
+-rw-r--r--   0        0        0     3754 2023-04-29 16:20:12.902455 custard-1.1.5/custard/utils/id_cards.py
+-rw-r--r--   0        0        0    85077 2023-04-29 16:20:12.906455 custard-1.1.5/custard/utils/jenkins.py
+-rw-r--r--   0        0        0    24805 2023-04-29 16:20:12.906455 custard-1.1.5/custard/utils/multi.py
+-rw-r--r--   0        0        0     4555 2023-04-29 16:20:12.906455 custard-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     8753 1970-01-01 00:00:00.000000 custard-1.1.5/PKG-INFO
```

### Comparing `custard-1.1.4/README.md` & `custard-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/__init__.py` & `custard-1.1.5/custard/core/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/decode.py` & `custard-1.1.5/custard/core/decode.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/factory.py` & `custard-1.1.5/custard/core/factory.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/functools.py` & `custard-1.1.5/custard/core/functools.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/kerberos.py` & `custard-1.1.5/custard/core/kerberos.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/processor.py` & `custard-1.1.5/custard/core/processor.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/regular.py` & `custard-1.1.5/custard/core/regular.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/system.py` & `custard-1.1.5/custard/core/system.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/useragent.py` & `custard-1.1.5/custard/core/useragent.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/xml2dict.py` & `custard-1.1.5/custard/core/xml2dict.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/core/xprint.py` & `custard-1.1.5/custard/core/xprint.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/crypto/crypto.py` & `custard-1.1.5/custard/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/crypto/streambody.py` & `custard-1.1.5/custard/crypto/streambody.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/curl/parse.py` & `custard-1.1.5/custard/curl/parse.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/hitfilter/hitfilter.py` & `custard-1.1.5/custard/hitfilter/hitfilter.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/hitfilter/keywords` & `custard-1.1.5/custard/hitfilter/keywords`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/kaptcha/captcha.py` & `custard-1.1.5/custard/kaptcha/captcha.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/kaptcha/font1.ttf` & `custard-1.1.5/custard/kaptcha/font1.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/kaptcha/font2.ttf` & `custard-1.1.5/custard/kaptcha/font2.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/kaptcha/font3.ttf` & `custard-1.1.5/custard/kaptcha/font3.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/kaptcha/font4.ttf` & `custard-1.1.5/custard/kaptcha/font4.ttf`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/limiter/README.md` & `custard-1.1.5/custard/limiter/README.md`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/limiter/__init__.py` & `custard-1.1.5/custard/limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/limiter/depends.py` & `custard-1.1.5/custard/limiter/depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/limiter/examples/__init__.py` & `custard-1.1.5/custard/limiter/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/limiter/examples/test_depends.py` & `custard-1.1.5/custard/limiter/examples/test_depends.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/mock/__init__.py` & `custard-1.1.5/custard/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/mock/mini_racer.py` & `custard-1.1.5/custard/mock/mini_racer.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/mock/mock.min.js` & `custard-1.1.5/custard/mock/mock.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/mock/mock.old.min.js` & `custard-1.1.5/custard/mock/mock.old.min.js`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/__init__.py` & `custard-1.1.5/custard/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/api.py` & `custard-1.1.5/custard/pagination/api.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/async_sqlalchemy.py` & `custard-1.1.5/custard/pagination/async_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/bases.py` & `custard-1.1.5/custard/pagination/bases.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/iterables.py` & `custard-1.1.5/custard/pagination/iterables.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/limit_offset.py` & `custard-1.1.5/custard/pagination/limit_offset.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/pagination.py` & `custard-1.1.5/custard/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/paginator.py` & `custard-1.1.5/custard/pagination/paginator.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/pagination/sync_sqlalchemy.py` & `custard-1.1.5/custard/pagination/sync_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/swagger/__init__.py` & `custard-1.1.5/custard/swagger/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 @Time    :  2022/7/18 10:16
 @Author  :  YuYanQing
 @Version :  1.0
 @Contact :  mryu168@163.com
 @License :  (C)Copyright 2022-2026
 @Desc    :  None
 """
-from urllib import request
-
+from requests import request
 from custard.core.system import SystemHand
-
 from .exception import ParseMethodError
 from .swagger import Swagger2
 
 
 def load_url(url, method="get", **kwargs):
     """
     通过url加载json
@@ -24,15 +22,15 @@
         url:
         method:
         **kwargs:
 
     Returns:
 
     """
-    return request.request(url=url, method=method, **kwargs).json()
+    return request(url=url, method=method, **kwargs).json()
 
 
 def swagger_parse(url=None, file=None, deep=5, **kwargs):
     """
     解析swagger
     Args:
         url:
```

### Comparing `custard-1.1.4/custard/swagger/swagger.py` & `custard-1.1.5/custard/swagger/swagger.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/swagger/utils.py` & `custard-1.1.5/custard/swagger/utils.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/time/__init__.py` & `custard-1.1.5/custard/time/__init__.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/time/dafunc.py` & `custard-1.1.5/custard/time/dafunc.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/time/exceptions.py` & `custard-1.1.5/custard/time/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class TimeOutError(Exception):
     """
     An operation timed out
     """
 
 
-class FunctionTimedOut(BaseException):
+class FunctionTimedOut(Exception):
     def __init__(
         self,
         msg="",
         timed_out_after=None,
         timed_out_function=None,
         timed_out_args=None,
         timed_out_kwargs=None,
```

### Comparing `custard-1.1.4/custard/time/moment.py` & `custard-1.1.5/custard/time/moment.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/time/stoppable_thread.py` & `custard-1.1.5/custard/time/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/utils/area_code.py` & `custard-1.1.5/custard/utils/area_code.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/utils/configparser.py` & `custard-1.1.5/custard/utils/configparser.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/utils/id_cards.py` & `custard-1.1.5/custard/utils/id_cards.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/utils/jenkins.py` & `custard-1.1.5/custard/utils/jenkins.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/custard/utils/multi.py` & `custard-1.1.5/custard/utils/multi.py`

 * *Files identical despite different names*

### Comparing `custard-1.1.4/pyproject.toml` & `custard-1.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "custard"
-version = "1.1.4"
+version = "1.1.5"
 description = "custard easy to learn, fast to code, ready for production"
 readme = "README.md"
 license = "MIT"
 authors = ["Kamalyes <mryu168@163.com>",]
 
 repository = "https://github.com/kamalyes/custard"
```

### Comparing `custard-1.1.4/PKG-INFO` & `custard-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: custard
-Version: 1.1.4
+Version: 1.1.5
 Summary: custard easy to learn, fast to code, ready for production
 Home-page: https://github.com/kamalyes/custard
 License: MIT
 Author: Kamalyes
 Author-email: mryu168@163.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: custard Version: 1.1.4 Summary: custard easy to
+Metadata-Version: 2.1 Name: custard Version: 1.1.5 Summary: custard easy to
 learn, fast to code, ready for production Home-page: https://github.com/
 kamalyes/custard License: MIT Author: Kamalyes Author-email: mryu168@163.com
 Requires-Python: >=3.9,<4.0 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 System Administrators Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
```

