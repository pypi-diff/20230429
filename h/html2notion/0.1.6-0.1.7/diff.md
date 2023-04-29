# Comparing `tmp/html2notion-0.1.6.tar.gz` & `tmp/html2notion-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html2notion-0.1.6.tar", last modified: Fri Apr 28 05:45:28 2023, max compression
+gzip compressed data, was "html2notion-0.1.7.tar", last modified: Sat Apr 29 10:42:28 2023, max compression
```

## Comparing `html2notion-0.1.6.tar` & `html2notion-0.1.7.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.029199 html2notion-0.1.6/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1064 2023-03-22 08:52:55.000000 html2notion-0.1.6/LICENSE
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-28 05:45:28.029345 html2notion-0.1.6/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4111 2023-04-23 03:24:11.000000 html2notion-0.1.6/README.md
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.012364 html2notion-0.1.6/html2notion/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.6/html2notion/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3955 2023-04-23 03:47:45.000000 html2notion-0.1.6/html2notion/main.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.022434 html2notion-0.1.6/html2notion/translate/
--rw-r--r--   0 daemonzhao   (501) staff       (20)        0 2023-03-20 01:38:35.000000 html2notion-0.1.6/html2notion/translate/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4176 2023-04-23 03:24:11.000000 html2notion-0.1.6/html2notion/translate/batch_import.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2724 2023-04-19 01:44:49.000000 html2notion-0.1.6/html2notion/translate/cos_uploader.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3816 2023-04-28 05:32:21.000000 html2notion-0.1.6/html2notion/translate/html2json.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    14207 2023-04-28 05:42:06.000000 html2notion-0.1.6/html2notion/translate/html2json_base.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4119 2023-04-28 05:42:00.000000 html2notion-0.1.6/html2notion/translate/html2json_clipper.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      430 2023-04-20 02:17:23.000000 html2notion-0.1.6/html2notion/translate/html2json_default.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     8744 2023-04-28 03:13:54.000000 html2notion-0.1.6/html2notion/translate/html2json_yinxiang.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     7168 2023-04-23 11:21:17.000000 html2notion-0.1.6/html2notion/translate/notion_export.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2867 2023-04-28 05:18:16.000000 html2notion-0.1.6/html2notion/translate/notion_import.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.025379 html2notion-0.1.6/html2notion/utils/
--rw-r--r--   0 daemonzhao   (501) staff       (20)      427 2023-03-24 02:23:25.000000 html2notion-0.1.6/html2notion/utils/__init__.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      828 2023-03-22 03:05:54.000000 html2notion-0.1.6/html2notion/utils/load_config.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     1579 2023-04-20 06:50:27.000000 html2notion-0.1.6/html2notion/utils/log.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)      437 2023-04-21 02:46:15.000000 html2notion-0.1.6/html2notion/utils/timeutil.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.015441 html2notion-0.1.6/html2notion.egg-info/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     4600 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/PKG-INFO
--rw-r--r--   0 daemonzhao   (501) staff       (20)      918 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/SOURCES.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)        1 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/dependency_links.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       54 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/entry_points.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      170 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/requires.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)       12 2023-04-28 05:45:27.000000 html2notion-0.1.6/html2notion.egg-info/top_level.txt
--rw-r--r--   0 daemonzhao   (501) staff       (20)      103 2023-03-20 01:38:35.000000 html2notion-0.1.6/pyproject.toml
--rw-r--r--   0 daemonzhao   (501) staff       (20)      852 2023-04-28 05:45:28.029919 html2notion-0.1.6/setup.cfg
--rw-r--r--   0 daemonzhao   (501) staff       (20)       38 2023-03-17 05:39:04.000000 html2notion-0.1.6/setup.py
-drwxr-xr-x   0 daemonzhao   (501) staff       (20)        0 2023-04-28 05:45:28.028320 html2notion-0.1.6/tests/
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2892 2023-04-20 03:22:55.000000 html2notion-0.1.6/tests/test_batchimport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     3038 2023-04-20 03:22:52.000000 html2notion-0.1.6/tests/test_cosupload.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)     2698 2023-04-13 05:01:24.000000 html2notion-0.1.6/tests/test_notionexport.py
--rw-r--r--   0 daemonzhao   (501) staff       (20)    31656 2023-04-27 02:03:06.000000 html2notion-0.1.6/tests/test_yinxiang.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.681534 html2notion-0.1.7/
+-rw-r--r--   0 feizhao    (501) staff       (20)     1064 2023-03-22 13:58:21.000000 html2notion-0.1.7/LICENSE
+-rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-04-29 10:42:28.681904 html2notion-0.1.7/PKG-INFO
+-rw-r--r--   0 feizhao    (501) staff       (20)     4111 2023-04-22 07:11:47.000000 html2notion-0.1.7/README.md
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.645708 html2notion-0.1.7/html2notion/
+-rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-03-18 15:41:01.000000 html2notion-0.1.7/html2notion/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     4413 2023-04-29 05:20:41.000000 html2notion-0.1.7/html2notion/main.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.661157 html2notion-0.1.7/html2notion/translate/
+-rw-r--r--   0 feizhao    (501) staff       (20)        0 2023-04-08 10:17:44.000000 html2notion-0.1.7/html2notion/translate/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     4176 2023-04-22 12:42:21.000000 html2notion-0.1.7/html2notion/translate/batch_import.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2724 2023-04-19 14:40:39.000000 html2notion-0.1.7/html2notion/translate/cos_uploader.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3816 2023-04-29 05:20:41.000000 html2notion-0.1.7/html2notion/translate/html2json.py
+-rw-r--r--   0 feizhao    (501) staff       (20)    15643 2023-04-29 09:04:36.000000 html2notion-0.1.7/html2notion/translate/html2json_base.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     5296 2023-04-29 05:20:41.000000 html2notion-0.1.7/html2notion/translate/html2json_clipper.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      430 2023-04-19 23:45:05.000000 html2notion-0.1.7/html2notion/translate/html2json_default.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     7443 2023-04-29 09:04:54.000000 html2notion-0.1.7/html2notion/translate/html2json_yinxiang.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     7168 2023-04-23 14:40:05.000000 html2notion-0.1.7/html2notion/translate/notion_export.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3091 2023-04-29 09:56:47.000000 html2notion-0.1.7/html2notion/translate/notion_import.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.668384 html2notion-0.1.7/html2notion/utils/
+-rw-r--r--   0 feizhao    (501) staff       (20)      453 2023-04-29 09:56:35.000000 html2notion-0.1.7/html2notion/utils/__init__.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      895 2023-04-29 09:55:54.000000 html2notion-0.1.7/html2notion/utils/load_config.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     1579 2023-04-20 14:39:58.000000 html2notion-0.1.7/html2notion/utils/log.py
+-rw-r--r--   0 feizhao    (501) staff       (20)      437 2023-04-21 14:23:32.000000 html2notion-0.1.7/html2notion/utils/timeutil.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.649918 html2notion-0.1.7/html2notion.egg-info/
+-rw-r--r--   0 feizhao    (501) staff       (20)     4600 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/PKG-INFO
+-rw-r--r--   0 feizhao    (501) staff       (20)      941 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/SOURCES.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)        1 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/dependency_links.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)       54 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/entry_points.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)      188 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/requires.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)       12 2023-04-29 10:42:28.000000 html2notion-0.1.7/html2notion.egg-info/top_level.txt
+-rw-r--r--   0 feizhao    (501) staff       (20)      103 2023-03-18 15:06:24.000000 html2notion-0.1.7/pyproject.toml
+-rw-r--r--   0 feizhao    (501) staff       (20)      871 2023-04-29 10:42:28.683316 html2notion-0.1.7/setup.cfg
+-rw-r--r--   0 feizhao    (501) staff       (20)       38 2023-03-18 07:34:12.000000 html2notion-0.1.7/setup.py
+drwxr-xr-x   0 feizhao    (501) staff       (20)        0 2023-04-29 10:42:28.679704 html2notion-0.1.7/tests/
+-rw-r--r--   0 feizhao    (501) staff       (20)     3940 2023-04-29 10:35:21.000000 html2notion-0.1.7/tests/test_batchimport.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     3038 2023-04-20 14:39:58.000000 html2notion-0.1.7/tests/test_cosupload.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     2698 2023-04-13 14:42:38.000000 html2notion-0.1.7/tests/test_notionexport.py
+-rw-r--r--   0 feizhao    (501) staff       (20)     1690 2023-04-29 09:11:49.000000 html2notion-0.1.7/tests/test_reqlimit.py
+-rw-r--r--   0 feizhao    (501) staff       (20)    31656 2023-04-27 14:25:22.000000 html2notion-0.1.7/tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.6/LICENSE` & `html2notion-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/PKG-INFO` & `html2notion-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.6
+Version: 0.1.7
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.6/README.md` & `html2notion-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/html2notion/main.py` & `html2notion-0.1.7/html2notion/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,28 +78,36 @@
     args = parse_args()
     prepare_env(args)
 
     file_path = Path(args.file) if args.file else None
     dir_path = Path(args.dir) if args.dir else None
     max_concurrency = args.batch
     if file_path and file_path.is_file():
-        logger.info(f"Begin save single html file: {file_path}.")
+        logger.debug(f"Begin save single html file: {file_path}.")
         result = asyncio.run(import_single_file(file_path))
-        logger.info(f"Finish save single html file: {file_path}.\n{result}")
-        console.print(f"File {file_path} saved.", style="green")
+        logger.debug(f"Finish save single html file: {file_path}.\n{result}")
+        text = Text("Single file ", style="default")
+        text.append(f"{file_path} ", style="cyan")
+        text.append("save to notion success.", style="default")
+        console.print(text)
     elif dir_path and dir_path.is_dir():
         logger.info(f"Begin save all html files in the dir: {dir_path}.")
         batch_import = BatchImport(dir_path, max_concurrency)
         result = asyncio.run(batch_import.process_directory())
         logger.info(f"Finish save all html files in the dir: {dir_path}.\n{result}")
 
         if len(batch_import.success_files) == len(batch_import.all_files):
             console.print(f"All files processed success.", style="green")
 
         print_fail_details(batch_import.failed_files)
     else:
-        console.print("No impossible.", style="red")
+        text = Text("The parameters provided are incorrect, please check.", style="red")
+        text.append("\nIf you need help, please submit an ", style="default")
+        link = Text("issue", style="cyan underline link https://github.com/selfboot/html2notion/issues")
+        text.append(link)
+        text.append(" on gitHub.", style="default")
+        console.print(text)
     return
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `html2notion-0.1.6/html2notion/translate/batch_import.py` & `html2notion-0.1.7/html2notion/translate/batch_import.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/html2notion/translate/cos_uploader.py` & `html2notion-0.1.7/html2notion/translate/cos_uploader.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/html2notion/translate/html2json.py` & `html2notion-0.1.7/html2notion/translate/html2json.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/html2notion/translate/html2json_base.py` & `html2notion-0.1.7/html2notion/translate/html2json_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "underline": bool,
         "code": bool,
         "color": str,
     }
 
     _color_tuple = namedtuple("Color", "name r g b")
     _notion_color = [
+        _color_tuple("default", 0, 0, 0),
         _color_tuple("gray", 128, 128, 128),
         _color_tuple("brown", 165, 42, 42),
         _color_tuple("orange", 255, 165, 0),
         _color_tuple("yellow", 255, 255, 0),
         _color_tuple("green", 0, 128, 0),
         _color_tuple("blue", 0, 0, 255),
         _color_tuple("purple", 128, 0, 128),
@@ -112,35 +113,39 @@
         if tag_name == 'a':
             href = tag_soup.get('href', "")
             if not href:
                 logger.warning("Link href is empty")
             text_params["url"] = href
         return
 
+    # https://developers.notion.com/reference/request-limits
     # Process one tag and return a list of objects
     # <b><u>unlineline and bold</u></b>
     # <div><font color="#ff2600">Red color4</font></div>
     # <div> Code in super note</div>
     @staticmethod
     def generate_inline_obj(tag: PageElement):
         res_obj = []
         text_with_parents = Html2JsonBase.extract_text_and_parents(tag)
         for (text, parent_tags) in text_with_parents:
-            text_params = {"plain_text": text}
-            for parent in parent_tags:
-                Html2JsonBase.parse_one_style(parent, text_params)
+            # Split the text into chunks of 2000 characters
+            text_chunks = [text[i:i+2000] for i in range(0, len(text), 2000)]
+            for chunk in text_chunks:
+                text_params = {"plain_text": chunk}
+                for parent in parent_tags:
+                    Html2JsonBase.parse_one_style(parent, text_params)
 
-            if text_params.get("url", ""):
-                text_obj = Html2JsonBase.generate_link(**text_params)
-            else:
-                text_obj = Html2JsonBase.generate_text(**text_params)
-            if text_obj:
-                res_obj.append(text_obj)
+                if text_params.get("url", ""):
+                    text_obj = Html2JsonBase.generate_link(**text_params)
+                else:
+                    text_obj = Html2JsonBase.generate_text(**text_params)
+                if text_obj:
+                    res_obj.append(text_obj)
         return res_obj
-    
+
     @staticmethod
     def generate_link(**kwargs):
         if not kwargs.get("plain_text", ""):
             return
         return {
             "href": kwargs.get("url", ""),
             "plain_text": kwargs.get("plain_text", ""),
@@ -300,14 +305,16 @@
         if color.startswith("rgb"):
             color_values = [int(x.strip()) for x in re.findall(r'\d+', color)]
             if len(color_values) >= 3:
                 r, g, b = color_values[:3]
                 return Html2JsonBase._closest_color(r, g, b)
         # Check if color is in hexadecimal format
         elif re.match(r'^#(?:[0-9a-fA-F]{3}){1,2}$', color):
+            if len(color) == 4:  # Short form like #abc -> #aabbcc
+                color = '#' + ''.join([c*2 for c in color[1:]])
             r, g, b = Html2JsonBase._hex_to_rgb(color)
             return Html2JsonBase._closest_color(r, g, b)
 
         return "default"
 
     def convert_paragraph(self, soup):
         json_obj = {
@@ -389,22 +396,55 @@
         rich_text = json_obj[list_type]["rich_text"]
         text_obj = Html2JsonBase.generate_inline_obj(soup)
         if text_obj:
             rich_text.extend(text_obj)
 
         return json_obj
 
-    # def convert_fail(self, soup):
-    #     return {
-    #         "object": "block",
-    #         "type": "paragraph",
-    #         "paragraph": {
-    #             "rich_text": []
-    #         }
-    #     }
+    """
+    <div>
+    <div><br /></div>
+    <table> <tbody> <tr> <td> </td> </tr> </tbody>
+    <div><br /></div>
+    </div>
+    """
+    # ../examples/insert_table.ipynb
+    def convert_table(self, soup):
+        table_rows = []
+        tr_tags = soup.find_all('tr')
+        if not tr_tags:
+            logger.error(f"No tr found in {soup}")
+            return
+        
+        table_width = len(tr_tags[0].find_all('td'))
+        for tr in tr_tags:
+            td_tags = tr.find_all('td')
+            if not td_tags:
+                continue
+            table_width = max(table_width, len(td_tags))
+            one_row = {
+                "type": "table_row",
+                "table_row": {
+                    "cells": []
+                }
+            }
+            for td in td_tags:
+                col = Html2JsonBase.generate_inline_obj(td)
+                one_row["table_row"]["cells"].append(col)
+            table_rows.append(one_row)
+
+        table_obj = {
+            "table": {
+                "has_row_header": False,
+                "has_column_header": False,
+                "table_width": table_width,
+                "children": table_rows,
+            }
+        }
+        return table_obj
 
     @classmethod
     def register(cls, input_type, subclass):
         cls._registry[input_type] = subclass
 
     @classmethod
     def create(cls, input_type, html_content):
```

### Comparing `html2notion-0.1.6/html2notion/translate/html2json_clipper.py` & `html2notion-0.1.7/html2notion/translate/html2json_clipper.py`

 * *Files 20% similar despite different names*

```diff
@@ -45,26 +45,30 @@
         self.properties = self.generate_properties(**properties)
         return
 
     def get_block_type(self, element):
         tag_name = element.name
         if tag_name == "p":
             return Block.PARAGRAPH.value
+        elif tag_name == "table":
+            return Block.TABLE.value
         elif tag_name in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
             return Block.HEADING.value
         elif tag_name == 'hr':
             return Block.DIVIDER.value
         elif tag_name == 'ol':
             return Block.NUMBERED_LIST.value
         elif tag_name == 'ul':
             return Block.BULLETED_LIST.value
         elif tag_name == 'p':
             return Block.PARAGRAPH.value
         elif element.name == 'pre' and element.code:
             return Block.CODE.value
+        elif self._check_is_block(element):
+            return Block.QUOTE.value
 
         return Block.FAIL.value
 
     def convert_children(self, soup):
         processed_tags = set()
         for element in soup.descendants:
             if isinstance(element, NavigableString):
@@ -105,9 +109,44 @@
                 continue
             text_obj = self.generate_inline_obj(child)
             if text_obj:
                 rich_text.extend(text_obj)
         json_obj["code"]["rich_text"] = self.merge_rich_text(rich_text)
         return json_obj
 
-        
+    def convert_quote(self, soup):
+        json_obj = {
+            "object": "block",
+            "type": "quote",
+            "quote": {
+                "rich_text": []
+            }
+        }
+        rich_text = json_obj["quote"]["rich_text"]
+        text_obj = self.generate_inline_obj(soup)
+        if text_obj:
+            rich_text.extend(text_obj)
+
+        # Merge tags has same anotions
+        return json_obj
+
+    def _check_is_block(self, element):
+        quote_elements = {'blockquote', 'q', 'cite'}
+        if element.name in quote_elements:
+            return True
+
+        if element.name != 'div':
+            return False
+
+        # if 'class' in element.attrs:
+        #     if any('quote' in class_name.lower() for class_name in element.attrs['class']):
+        #         return True
+
+        # if 'style' in element.attrs:
+        #     style_attrs = element.attrs['style'].lower()
+        #     if 'border:' in style_attrs or 'padding:' in style_attrs:
+        #         return True
+
+        return False
+
+    
 Html2JsonBase.register(YinXiangClipper_Type, Html2JsonYinXiang)
```

### Comparing `html2notion-0.1.6/html2notion/translate/html2json_yinxiang.py` & `html2notion-0.1.7/html2notion/translate/html2json_yinxiang.py`

 * *Files 11% similar despite different names*

```diff
@@ -107,59 +107,14 @@
                 rich_text.append(self.generate_text(plain_text='\n'))
 
         # Merge tags has same anotions
         logger.debug(f'before merge: {rich_text}')
         json_obj["quote"]["rich_text"] = self.merge_rich_text(rich_text)
         return json_obj
 
-    """
-    <div>
-    <div><br /></div>
-    <table> <tbody> <tr> <td> </td> </tr> </tbody>
-    <div><br /></div>
-    </div>
-    """
-    # ../examples/insert_table.ipynb
-    def convert_table(self, soup):
-        # logger.debug(f'Convert table: {soup}')
-        # Assert: only one table in table div
-        table_rows = []
-        tr_tags = soup.find_all('tr')
-        if not tr_tags:
-            logger.error(f"No tr found in {soup}")
-            return
-        
-        table_width = len(tr_tags[0].find_all('td'))
-        if table_width == 0:
-            logger.error(f"No td found in {soup}")
-            return
-        
-        for tr in tr_tags:
-            td_tags = tr.find_all('td')
-            one_row = {
-                "type": "table_row",
-                "table_row": {
-                    "cells": []
-                }
-            }
-            for td in td_tags:
-                col = Html2JsonBase.generate_inline_obj(td)
-                one_row["table_row"]["cells"].append(col)
-            table_rows.append(one_row)
-
-        table_obj = {
-            "table": {
-                "has_row_header": False,
-                "has_column_header": False,
-                "table_width": table_width,
-                "children": table_rows,
-            }
-        }
-        return table_obj
-
     def convert_to_do(self, soup: Tag):
         # Compatible with the situation where input is under li tag(super note).
         li_tags = soup.find_all('li', recursive=True)
         childs = li_tags if li_tags else [soup]
         to_do_blocks = []
         for child in childs:
             json_obj = {
```

### Comparing `html2notion-0.1.6/html2notion/translate/notion_export.py` & `html2notion-0.1.7/html2notion/translate/notion_export.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/html2notion/translate/notion_import.py` & `html2notion-0.1.7/html2notion/translate/notion_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import os
 from aiohttp import ClientSession
 from pathlib import Path
 from notion_client import AsyncClient
 from notion_client.errors import RequestTimeoutError
 from tenacity import retry, stop_after_attempt, wait_exponential, retry_if_exception_type
-from ..utils import logger, test_prepare_conf, config
+from ..utils import logger, test_prepare_conf, config, rate_limit
 from ..translate.html2json import html2json_process
 
 
 class NotionImporter:
     def __init__(self, session: ClientSession, notion_client):
         self.session = session
         self.notion_client = notion_client
@@ -30,31 +30,34 @@
         notion_data, html_type = html2json_process(file_path)
         logger.info(f"path: {file_path}, html type: {html_type}")
 
         create_result = await self.create_new_page(notion_data)
         logger.info(f"Create notion page: {create_result}")
         return "succ"
 
+    # https://developers.notion.com/reference/request-limits
+    # The rate limit for incoming requests per integration is an average of three requests per second. 
     # Doc of create page: https://developers.notion.com/reference/post-page
     @retry(stop=stop_after_attempt(5),
            wait=wait_exponential(multiplier=1, min=3, max=30),
            retry=retry_if_exception_type(RequestTimeoutError))
     async def create_new_page(self, notion_data):
         # logger.debug(f'Create new page: {notion_data["parent"]}, {notion_data["properties"]}')
         # body.children.length should be ≤ `100`,
         blocks = notion_data.get("children", [])
         limit_size = 100
         chunks = [blocks[i: i + limit_size] for i in range(0, len(blocks), limit_size)]
         if blocks:
             notion_data.pop("children")
         first_chunk = chunks[0] if chunks else []
-        created_page = await self.notion_client.pages.create(**notion_data, children=first_chunk)
-        page_id = created_page["id"]
-        for chunk in chunks[1:]:
-            await self.notion_client.blocks.children.append(page_id, children=chunk)
+        async with rate_limit:
+            created_page = await self.notion_client.pages.create(**notion_data, children=first_chunk)
+            page_id = created_page["id"]
+            for chunk in chunks[1:]:
+                await self.notion_client.blocks.children.append(page_id, children=chunk)
         return created_page
 
 
 async def main(file_path, notion_api_key):
     async with ClientSession() as session:
         async with AsyncClient(auth=notion_api_key) as notion_client:
             importer = NotionImporter(session, notion_client)
```

### Comparing `html2notion-0.1.6/html2notion/utils/log.py` & `html2notion-0.1.7/html2notion/utils/log.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/html2notion.egg-info/PKG-INFO` & `html2notion-0.1.7/html2notion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html2notion
-Version: 0.1.6
+Version: 0.1.7
 Summary: This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 Home-page: https://github.com/selfboot/html2notion
 Author: selfboot
 Author-email: xuezaigds@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `html2notion-0.1.6/html2notion.egg-info/SOURCES.txt` & `html2notion-0.1.7/html2notion.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 html2notion/utils/__init__.py
 html2notion/utils/load_config.py
 html2notion/utils/log.py
 html2notion/utils/timeutil.py
 tests/test_batchimport.py
 tests/test_cosupload.py
 tests/test_notionexport.py
+tests/test_reqlimit.py
 tests/test_yinxiang.py
```

### Comparing `html2notion-0.1.6/setup.cfg` & `html2notion-0.1.7/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = html2notion
-version = 0.1.6
+version = 0.1.7
 author = selfboot
 author_email = xuezaigds@gmail.com
 description = This tool can accurately convert HTML to Notion notes and is also useful for exporting Evernote notes to Notion.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/selfboot/html2notion
 license_files = LICENSE
@@ -22,14 +22,15 @@
 	notion-client>=2.0.0
 	PyYAML>=6.0
 	aiohttp>=3.8.4
 	anyio>=3.6.2
 	rich>=13.3.4
 	cos-python-sdk-v5>=1.9.23
 	tenacity>=8.2.2
+	aiolimiter>=1.0.0
 
 [options.entry_points]
 console_scripts = 
 	html2notion = html2notion.main:main
 
 [egg_info]
 tag_build =
```

### Comparing `html2notion-0.1.6/tests/test_batchimport.py` & `html2notion-0.1.7/tests/test_batchimport.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import time
 import os
 from pathlib import Path
 from unittest.mock import patch
 from tempfile import TemporaryDirectory
 from http import HTTPStatus
 from html2notion.translate.batch_import import BatchImport
+from html2notion.utils import rate_limit
 from html2notion.utils.log import log_only_local
 
 process_once_time = 0.5
 
 
 @pytest.fixture(scope="session", autouse=True)
 def prepare_conf_fixture():
@@ -37,14 +38,20 @@
         logger.debug(f"mock_notion_api_request: {file_path}")
     await asyncio.sleep(process_once_time)
     end_time = time.perf_counter()
     elapsed_time = end_time - start_time
     return MockResponse(HTTPStatus.OK, content, elapsed_time)
 
 
+async def mock_notion_create_page(notion_data, *args, **kwargs):
+    async with rate_limit:
+        await asyncio.sleep(0.01)
+        log_only_local(f"mock_notion_create_page")
+    return "succ"
+
 @pytest.fixture(params=[10, 20])
 def temp_dir_fixture(request):
     num_files = request.param
     with TemporaryDirectory() as temp_dir:
         dir_path = Path(temp_dir)
         temp_files = []
         for i in range(num_files):
@@ -74,7 +81,24 @@
     total_time = end_time-start_time
     sync_time = sum(res.json()["elapsed_time"] for res in responses)
     least_time = min(res.json()["elapsed_time"] for res in responses)
     log_only_local(
         f"total_time: {total_time}, sync_time: {sync_time}, least_time: {least_time}")
     assert total_time >= least_time
     assert total_time <= sync_time
+
+
+@pytest.mark.parametrize("concurrent_limit", [5, 10, 20])
+@pytest.mark.asyncio
+async def test_reqlimit(temp_dir_fixture, concurrent_limit):
+    dir_path = temp_dir_fixture
+    start_time = time.perf_counter()
+    with patch("html2notion.translate.notion_import.NotionImporter.create_new_page", side_effect=mock_notion_create_page):
+        batch_processor = BatchImport(dir_path, concurrent_limit=concurrent_limit)
+        responses = await batch_processor.process_directory()
+
+    end_time = time.perf_counter()
+    total_time = end_time-start_time
+    num_files = len(list(dir_path.glob('*.html')))
+    log_only_local(f"file nums: {num_files}, concurrent {concurrent_limit}, total_time: {total_time}")
+    # The time deviation within 1 second is acceptable here.
+    assert (total_time >= num_files / 3 - 1)
```

### Comparing `html2notion-0.1.6/tests/test_cosupload.py` & `html2notion-0.1.7/tests/test_cosupload.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/tests/test_notionexport.py` & `html2notion-0.1.7/tests/test_notionexport.py`

 * *Files identical despite different names*

### Comparing `html2notion-0.1.6/tests/test_yinxiang.py` & `html2notion-0.1.7/tests/test_yinxiang.py`

 * *Files identical despite different names*

