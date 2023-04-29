# Comparing `tmp/bulrush-0.6.2.tar.gz` & `tmp/bulrush-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulrush-0.6.2.tar", last modified: Sat Apr 29 14:27:15 2023, max compression
+gzip compressed data, was "bulrush-0.6.3.tar", last modified: Sat Apr 29 16:25:51 2023, max compression
```

## Comparing `bulrush-0.6.2.tar` & `bulrush-0.6.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.974168 bulrush-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-29 14:26:50.000000 bulrush-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 14:27:15.974168 bulrush-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-04-29 14:26:50.000000 bulrush-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/image_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/license_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/schema_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.966168 bulrush-0.6.2/bulrush/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush/static/css/main.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/analytics.html
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/archives.html
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/article.html
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/article_infos.html
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/article_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/category.html
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/comments.html
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/disqus_script.html
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/github.html
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/mailchimp.html
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/mermaid.html
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/meta_tags.html
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/page.html
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/period_archives.html
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/social.html
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/tag.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/taglist.html
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/tags.html
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 14:26:50.000000 bulrush-0.6.2/bulrush/templates/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 14:27:15.970168 bulrush-0.6.2/bulrush.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 14:27:15.000000 bulrush-0.6.2/bulrush.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 14:27:15.974168 bulrush-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-29 14:26:50.000000 bulrush-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:25:51.923214 bulrush-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-29 16:25:17.000000 bulrush-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-29 16:25:51.923214 bulrush-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-04-29 16:25:17.000000 bulrush-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:25:51.919214 bulrush-0.6.3/bulrush/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/image_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/license_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/schema_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:25:51.919214 bulrush-0.6.3/bulrush/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:25:51.919214 bulrush-0.6.3/bulrush/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-29 16:25:51.000000 bulrush-0.6.3/bulrush/static/css/main.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:25:51.923214 bulrush-0.6.3/bulrush/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/analytics.html
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/archives.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/article.html
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/article_infos.html
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/article_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/category.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/comments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/disqus_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/github.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/mailchimp.html
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/mermaid.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/meta_tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/period_archives.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/social.html
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/tag.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/taglist.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/tags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 16:25:17.000000 bulrush-0.6.3/bulrush/templates/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:25:51.919214 bulrush-0.6.3/bulrush.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-29 16:25:51.000000 bulrush-0.6.3/bulrush.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-29 16:25:51.000000 bulrush-0.6.3/bulrush.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:25:51.000000 bulrush-0.6.3/bulrush.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 16:25:51.000000 bulrush-0.6.3/bulrush.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 16:25:51.000000 bulrush-0.6.3/bulrush.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:25:51.923214 bulrush-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-29 16:25:17.000000 bulrush-0.6.3/setup.py
```

### Comparing `bulrush-0.6.2/LICENSE` & `bulrush-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/PKG-INFO` & `bulrush-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulrush
-Version: 0.6.2
+Version: 0.6.3
 Summary: Bulrush theme for Pelican
 Home-page: https://github.com/textbook/bulrush
 Author: Jonathan Sharpe
 Author-email: mail@jonrshar.pe
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pelican :: Themes
@@ -203,15 +203,15 @@
 
 ### Mermaid Configuration
 
 Enables [Mermaid][25] diagram generation on your site, allowing diagrams to be
 written in a Markdown-ish syntax. Simply wrap the code in a `pre` element
 with the `mermaid` class:
 
-```markdown
+```html
 <pre class="mermaid">
 graph TD;
     A-->B;
     A-->C;
     B-->D;
     C-->D;
 </pre>
```

### Comparing `bulrush-0.6.2/README.md` & `bulrush-0.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
 ### Mermaid Configuration
 
 Enables [Mermaid][25] diagram generation on your site, allowing diagrams to be
 written in a Markdown-ish syntax. Simply wrap the code in a `pre` element
 with the `mermaid` class:
 
-```markdown
+```html
 <pre class="mermaid">
 graph TD;
     A-->B;
     A-->C;
     B-->D;
     C-->D;
 </pre>
```

### Comparing `bulrush-0.6.2/bulrush/__init__.py` & `bulrush-0.6.3/bulrush/__init__.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/image_extractor.py` & `bulrush-0.6.3/bulrush/image_extractor.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/license_generator.py` & `bulrush-0.6.3/bulrush/license_generator.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/schema_generator.py` & `bulrush-0.6.3/bulrush/schema_generator.py`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/static/css/main.css` & `bulrush-0.6.3/bulrush/static/css/main.css`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/analytics.html` & `bulrush-0.6.3/bulrush/templates/analytics.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/archives.html` & `bulrush-0.6.3/bulrush/templates/archives.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/article.html` & `bulrush-0.6.3/bulrush/templates/article.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/article_infos.html` & `bulrush-0.6.3/bulrush/templates/article_infos.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/article_list.html` & `bulrush-0.6.3/bulrush/templates/article_list.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/base.html` & `bulrush-0.6.3/bulrush/templates/base.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/index.html` & `bulrush-0.6.3/bulrush/templates/index.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/mailchimp.html` & `bulrush-0.6.3/bulrush/templates/mailchimp.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/meta_tags.html` & `bulrush-0.6.3/bulrush/templates/meta_tags.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/page.html` & `bulrush-0.6.3/bulrush/templates/page.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/pagination.html` & `bulrush-0.6.3/bulrush/templates/pagination.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/period_archives.html` & `bulrush-0.6.3/bulrush/templates/period_archives.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush/templates/social.html` & `bulrush-0.6.3/bulrush/templates/social.html`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/bulrush.egg-info/PKG-INFO` & `bulrush-0.6.3/bulrush.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulrush
-Version: 0.6.2
+Version: 0.6.3
 Summary: Bulrush theme for Pelican
 Home-page: https://github.com/textbook/bulrush
 Author: Jonathan Sharpe
 Author-email: mail@jonrshar.pe
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pelican :: Themes
@@ -203,15 +203,15 @@
 
 ### Mermaid Configuration
 
 Enables [Mermaid][25] diagram generation on your site, allowing diagrams to be
 written in a Markdown-ish syntax. Simply wrap the code in a `pre` element
 with the `mermaid` class:
 
-```markdown
+```html
 <pre class="mermaid">
 graph TD;
     A-->B;
     A-->C;
     B-->D;
     C-->D;
 </pre>
```

### Comparing `bulrush-0.6.2/bulrush.egg-info/SOURCES.txt` & `bulrush-0.6.3/bulrush.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bulrush-0.6.2/setup.py` & `bulrush-0.6.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,9 +26,9 @@
             'static/css/*.css',
         ]
     },
     packages=['bulrush'],
     test_suite='tests',
     tests_require=['pelican'],
     url='https://github.com/textbook/bulrush',
-    version='0.6.2',
+    version='0.6.3',
 )
```

