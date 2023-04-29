# Comparing `tmp/bubblemsg-3.0.tar.gz` & `tmp/bubblemsg-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bubblemsg-3.0.tar", last modified: Wed Apr 26 13:56:27 2023, max compression
+gzip compressed data, was "bubblemsg-3.1.tar", last modified: Sat Apr 29 04:07:23 2023, max compression
```

## Comparing `bubblemsg-3.0.tar` & `bubblemsg-3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 13:56:27.794666 bubblemsg-3.0/
--rw-rw-rw-   0        0        0     1091 2023-02-11 07:25:20.000000 bubblemsg-3.0/LICENSE
--rw-rw-rw-   0        0        0      387 2023-04-26 13:56:27.794666 bubblemsg-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2196 2023-03-13 13:17:10.000000 bubblemsg-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 13:56:27.779045 bubblemsg-3.0/bubblemsg/
--rw-rw-rw-   0        0        0     9358 2023-04-26 11:25:53.000000 bubblemsg-3.0/bubblemsg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 13:56:27.794666 bubblemsg-3.0/bubblemsg.egg-info/
--rw-rw-rw-   0        0        0      387 2023-04-26 13:56:27.000000 bubblemsg-3.0/bubblemsg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-04-26 13:56:27.000000 bubblemsg-3.0/bubblemsg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 13:56:27.000000 bubblemsg-3.0/bubblemsg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-26 13:56:27.000000 bubblemsg-3.0/bubblemsg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 13:56:27.794666 bubblemsg-3.0/setup.cfg
--rw-rw-rw-   0        0        0      496 2023-04-26 13:25:42.000000 bubblemsg-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 04:07:23.032014 bubblemsg-3.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 07:25:20.000000 bubblemsg-3.1/LICENSE
+-rw-rw-rw-   0        0        0      387 2023-04-29 04:07:23.016391 bubblemsg-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2196 2023-03-13 13:17:10.000000 bubblemsg-3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 04:07:23.016391 bubblemsg-3.1/bubblemsg/
+-rw-rw-rw-   0        0        0     9326 2023-04-29 04:06:01.000000 bubblemsg-3.1/bubblemsg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 04:07:23.016391 bubblemsg-3.1/bubblemsg.egg-info/
+-rw-rw-rw-   0        0        0      387 2023-04-29 04:07:22.000000 bubblemsg-3.1/bubblemsg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-04-29 04:07:22.000000 bubblemsg-3.1/bubblemsg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 04:07:22.000000 bubblemsg-3.1/bubblemsg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-29 04:07:22.000000 bubblemsg-3.1/bubblemsg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 04:07:23.032014 bubblemsg-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      496 2023-04-29 04:06:50.000000 bubblemsg-3.1/setup.py
```

### Comparing `bubblemsg-3.0/LICENSE` & `bubblemsg-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bubblemsg-3.0/README.md` & `bubblemsg-3.1/README.md`

 * *Files identical despite different names*

### Comparing `bubblemsg-3.0/bubblemsg/__init__.py` & `bubblemsg-3.1/bubblemsg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,8 +189,7 @@
         def show_msg(title,msg):
     	    t = TestTaskbarIcon()
     	    t.showMsg(title, msg)
         show_msg('None','None')
 
     else:
         raise NoTypeError('模式“' + str(nx) + '”被作者炸到天堂去了')
-bubblemsg('测试','测试',4)
```

