# Comparing `tmp/scribber-0.1.17.tar.gz` & `tmp/scribber-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribber-0.1.17.tar", last modified: Sat Apr 29 11:45:45 2023, max compression
+gzip compressed data, was "scribber-0.1.18.tar", last modified: Sat Apr 29 12:02:02 2023, max compression
```

## Comparing `scribber-0.1.17.tar` & `scribber-0.1.18.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/
--rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.17/LICENSE
--rw-rw-r--   0 sem       (1000) sem       (1000)     3616 2023-04-29 11:45:45.701084 scribber-0.1.17/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)     2997 2023-04-29 10:51:26.000000 scribber-0.1.17/README.md
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/
--rw-rw-r--   0 sem       (1000) sem       (1000)      380 2023-04-29 10:43:17.000000 scribber-0.1.17/scribber/__init__.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/core/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.17/scribber/core/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3472 2023-04-29 11:36:25.000000 scribber-0.1.17/scribber/core/document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/examples/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.17/scribber/examples/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2315 2023-04-29 11:26:35.000000 scribber-0.1.17/scribber/examples/usage.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/formats/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.17/scribber/formats/__init__.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/formats/excel/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.17/scribber/formats/excel/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2227 2023-04-29 10:32:51.000000 scribber-0.1.17/scribber/formats/excel/excel_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/formats/markdown/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.17/scribber/formats/markdown/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     3941 2023-04-29 11:06:26.000000 scribber-0.1.17/scribber/formats/markdown/markdown_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/formats/text/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.17/scribber/formats/text/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     2946 2023-04-29 10:32:33.000000 scribber-0.1.17/scribber/formats/text/text_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber/formats/word/
--rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.17/scribber/formats/word/__init__.py
--rw-rw-r--   0 sem       (1000) sem       (1000)     1878 2023-04-29 11:44:52.000000 scribber-0.1.17/scribber/formats/word/word_document.py
-drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 11:45:45.701084 scribber-0.1.17/scribber.egg-info/
--rw-rw-r--   0 sem       (1000) sem       (1000)     3616 2023-04-29 11:45:45.000000 scribber-0.1.17/scribber.egg-info/PKG-INFO
--rw-rw-r--   0 sem       (1000) sem       (1000)      651 2023-04-29 11:45:45.000000 scribber-0.1.17/scribber.egg-info/SOURCES.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-04-29 11:45:45.000000 scribber-0.1.17/scribber.egg-info/dependency_links.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)      147 2023-04-29 11:45:45.000000 scribber-0.1.17/scribber.egg-info/requires.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)        9 2023-04-29 11:45:45.000000 scribber-0.1.17/scribber.egg-info/top_level.txt
--rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-04-29 11:45:45.701084 scribber-0.1.17/setup.cfg
--rw-rw-r--   0 sem       (1000) sem       (1000)     1185 2023-04-29 11:07:42.000000 scribber-0.1.17/setup.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1072 2023-04-23 07:58:01.000000 scribber-0.1.18/LICENSE
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3624 2023-04-29 12:02:02.055511 scribber-0.1.18/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3005 2023-04-29 11:50:33.000000 scribber-0.1.18/README.md
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/
+-rw-rw-r--   0 sem       (1000) sem       (1000)      380 2023-04-29 10:43:17.000000 scribber-0.1.18/scribber/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/core/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:19:56.000000 scribber-0.1.18/scribber/core/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3472 2023-04-29 11:36:25.000000 scribber-0.1.18/scribber/core/document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/examples/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2023-04-23 07:28:29.000000 scribber-0.1.18/scribber/examples/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2315 2023-04-29 11:26:35.000000 scribber-0.1.18/scribber/examples/usage.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:25:48.000000 scribber-0.1.18/scribber/formats/__init__.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/excel/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:12.000000 scribber-0.1.18/scribber/formats/excel/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2227 2023-04-29 10:32:51.000000 scribber-0.1.18/scribber/formats/excel/excel_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/markdown/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:59:05.000000 scribber-0.1.18/scribber/formats/markdown/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3941 2023-04-29 11:06:26.000000 scribber-0.1.18/scribber/formats/markdown/markdown_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/text/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:02.000000 scribber-0.1.18/scribber/formats/text/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     2946 2023-04-29 10:32:33.000000 scribber-0.1.18/scribber/formats/text/text_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber/formats/word/
+-rw-rw-r--   0 sem       (1000) sem       (1000)        0 2022-11-20 07:26:50.000000 scribber-0.1.18/scribber/formats/word/__init__.py
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1878 2023-04-29 11:44:52.000000 scribber-0.1.18/scribber/formats/word/word_document.py
+drwxrwxr-x   0 sem       (1000) sem       (1000)        0 2023-04-29 12:02:02.055511 scribber-0.1.18/scribber.egg-info/
+-rw-rw-r--   0 sem       (1000) sem       (1000)     3624 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/PKG-INFO
+-rw-rw-r--   0 sem       (1000) sem       (1000)      651 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/SOURCES.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        1 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/dependency_links.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)      147 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/requires.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)        9 2023-04-29 12:02:02.000000 scribber-0.1.18/scribber.egg-info/top_level.txt
+-rw-rw-r--   0 sem       (1000) sem       (1000)       38 2023-04-29 12:02:02.055511 scribber-0.1.18/setup.cfg
+-rw-rw-r--   0 sem       (1000) sem       (1000)     1185 2023-04-29 12:00:10.000000 scribber-0.1.18/setup.py
```

### Comparing `scribber-0.1.17/LICENSE` & `scribber-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/PKG-INFO` & `scribber-0.1.18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.1.17
+Version: 0.1.18
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
@@ -79,18 +79,18 @@
     doc.add(EmptyLine())
     doc.add(Title(title="Code block", level=2))
     doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
     doc.add(CodeBlock(style="console", code=CODE_RESULT))
     doc.add(Paragraph(text="It's Ok!"))
 
     director = Director()
-    text_report_builder = DocumentBuilder(doc=TextDocument)
-    word_report_builder = DocumentBuilder(doc=WordDocument)
-    excel_report_builder = DocumentBuilder(doc=ExcelDocument)
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument)
+    text_report_builder = DocumentBuilder(doc=TextDocument())
+    word_report_builder = DocumentBuilder(doc=WordDocument())
+    excel_report_builder = DocumentBuilder(doc=ExcelDocument())
+    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
```

### Comparing `scribber-0.1.17/README.md` & `scribber-0.1.18/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,18 @@
     doc.add(EmptyLine())
     doc.add(Title(title="Code block", level=2))
     doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
     doc.add(CodeBlock(style="console", code=CODE_RESULT))
     doc.add(Paragraph(text="It's Ok!"))
 
     director = Director()
-    text_report_builder = DocumentBuilder(doc=TextDocument)
-    word_report_builder = DocumentBuilder(doc=WordDocument)
-    excel_report_builder = DocumentBuilder(doc=ExcelDocument)
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument)
+    text_report_builder = DocumentBuilder(doc=TextDocument())
+    word_report_builder = DocumentBuilder(doc=WordDocument())
+    excel_report_builder = DocumentBuilder(doc=ExcelDocument())
+    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
```

### Comparing `scribber-0.1.17/scribber/core/document.py` & `scribber-0.1.18/scribber/core/document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/scribber/examples/usage.py` & `scribber-0.1.18/scribber/examples/usage.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/scribber/formats/excel/excel_document.py` & `scribber-0.1.18/scribber/formats/excel/excel_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/scribber/formats/markdown/markdown_document.py` & `scribber-0.1.18/scribber/formats/markdown/markdown_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/scribber/formats/text/text_document.py` & `scribber-0.1.18/scribber/formats/text/text_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/scribber/formats/word/word_document.py` & `scribber-0.1.18/scribber/formats/word/word_document.py`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/scribber.egg-info/PKG-INFO` & `scribber-0.1.18/scribber.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scribber
-Version: 0.1.17
+Version: 0.1.18
 Summary: A simple document generator with not very rich functionality that can export a document to some formats such as text, docx, xlsx and markdown.
 Home-page: https://github.com/edelwi/scribber
 Author: Evgeniy Semenov
 Author-email: edelwi@yandex.ru
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python :: 3
@@ -79,18 +79,18 @@
     doc.add(EmptyLine())
     doc.add(Title(title="Code block", level=2))
     doc.add(CodeBlock(style="python", code=CODE_EXAMPLE))
     doc.add(CodeBlock(style="console", code=CODE_RESULT))
     doc.add(Paragraph(text="It's Ok!"))
 
     director = Director()
-    text_report_builder = DocumentBuilder(doc=TextDocument)
-    word_report_builder = DocumentBuilder(doc=WordDocument)
-    excel_report_builder = DocumentBuilder(doc=ExcelDocument)
-    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument)
+    text_report_builder = DocumentBuilder(doc=TextDocument())
+    word_report_builder = DocumentBuilder(doc=WordDocument())
+    excel_report_builder = DocumentBuilder(doc=ExcelDocument())
+    marckdown_report_builder = DocumentBuilder(doc=MarkdownDocument())
 
     print("Make a Text Document")
     director.builder = text_report_builder
     director.build_report_from_doc(doc)
     text_report_builder.parts.save("test.txt")
 
     print("Make a Word Document")
```

### Comparing `scribber-0.1.17/scribber.egg-info/SOURCES.txt` & `scribber-0.1.18/scribber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scribber-0.1.17/setup.py` & `scribber-0.1.18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scribber",
-    version="v0.1.17",
+    version="v0.1.18",
     author="Evgeniy Semenov",
     author_email="edelwi@yandex.ru",
     license="MIT",
     description="A simple document generator with not very rich functionality "
                 "that can export a document to some formats such as text, docx, "
                 "xlsx and markdown.",
     long_description=long_description,
```

