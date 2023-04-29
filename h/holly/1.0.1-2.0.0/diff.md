# Comparing `tmp/holly-1.0.1.tar.gz` & `tmp/holly-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holly-1.0.1.tar", last modified: Wed Nov  3 10:09:14 2021, max compression
+gzip compressed data, was "holly-2.0.0.tar", last modified: Sat Apr 29 12:40:20 2023, max compression
```

## Comparing `holly-1.0.1.tar` & `holly-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2021-11-03 10:09:14.157990 holly-1.0.1/
--rw-r--r--   0 dmulholl   (501) staff       (20)      516 2021-11-03 10:09:14.157769 holly-1.0.1/PKG-INFO
-drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2021-11-03 10:09:14.157465 holly-1.0.1/holly.egg-info/
--rw-r--r--   0 dmulholl   (501) staff       (20)      516 2021-11-03 10:09:13.000000 holly-1.0.1/holly.egg-info/PKG-INFO
--rw-r--r--   0 dmulholl   (501) staff       (20)      133 2021-11-03 10:09:14.000000 holly-1.0.1/holly.egg-info/SOURCES.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        1 2021-11-03 10:09:13.000000 holly-1.0.1/holly.egg-info/dependency_links.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)        6 2021-11-03 10:09:13.000000 holly-1.0.1/holly.egg-info/top_level.txt
--rw-r--r--   0 dmulholl   (501) staff       (20)     6800 2021-11-03 09:58:20.000000 holly-1.0.1/holly.py
--rw-r--r--   0 dmulholl   (501) staff       (20)       38 2021-11-03 10:09:14.158064 holly-1.0.1/setup.cfg
--rwxr-xr-x   0 dmulholl   (501) staff       (20)      607 2021-11-03 10:02:22.000000 holly-1.0.1/setup.py
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-29 12:40:20.651537 holly-2.0.0/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      415 2023-04-29 12:40:20.651350 holly-2.0.0/PKG-INFO
+drwxr-xr-x   0 dmulholl   (501) staff       (20)        0 2023-04-29 12:40:20.651091 holly-2.0.0/holly.egg-info/
+-rw-r--r--   0 dmulholl   (501) staff       (20)      415 2023-04-29 12:40:20.000000 holly-2.0.0/holly.egg-info/PKG-INFO
+-rw-r--r--   0 dmulholl   (501) staff       (20)      133 2023-04-29 12:40:20.000000 holly-2.0.0/holly.egg-info/SOURCES.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        1 2023-04-29 12:40:20.000000 holly-2.0.0/holly.egg-info/dependency_links.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)        6 2023-04-29 12:40:20.000000 holly-2.0.0/holly.egg-info/top_level.txt
+-rw-r--r--   0 dmulholl   (501) staff       (20)     6712 2023-04-29 12:26:48.000000 holly-2.0.0/holly.py
+-rw-r--r--   0 dmulholl   (501) staff       (20)       38 2023-04-29 12:40:20.651608 holly-2.0.0/setup.cfg
+-rwxr-xr-x   0 dmulholl   (501) staff       (20)      607 2023-04-29 12:37:24.000000 holly-2.0.0/setup.py
```

### Comparing `holly-1.0.1/holly.py` & `holly-2.0.0/holly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import ivy
+import ark
 import math
 import datetime
 
 
 # This callback generates the indexes. (An index is an ordered list of nodes
 # attached to a node via an 'index' property.)
-@ivy.events.register('init_build')
+@ark.events.register('init_build')
 def init():
-    if config := ivy.site.config.get('holly'):
+    if config := ark.site.config.get('holly'):
 
         # Generate the homepage index.
         if home := config.get('homepage'):
             root_urls = home.get('root_urls', [])
             sort_func = home.get('sort_func')
             sort_rev = home.get('reverse', True)
             per_page = home.get('per_page', 10)
@@ -21,36 +21,34 @@
         for root in config.get('roots', []):
             root_url = root.get('root_url', '')
             tag_slug = root.get('tag_slug', 'tags')
             sort_func = root.get('sort_func')
             sort_rev = root.get('reverse', True)
             per_page = root.get('per_page', 10)
             per_tag_page = root.get('per_tag_page', 100)
-            if node := ivy.nodes.node(root_url):
+            if node := ark.nodes.node(root_url):
                 make_node_index(node, sort_func, sort_rev, per_page)
                 make_tag_indexes(node, tag_slug, sort_func, sort_rev, per_tag_page)
 
 
 # This callback adds CSS classes to index pages.
-@ivy.filters.register('class_list')
+@ark.filters.register('class_list')
 def add_classes(class_list, node):
     if node.get('is_index'):
         class_list.append('index')
     if node.get('is_dir_index'):
         class_list.append('dir-index')
     if node.get('is_tag_index'):
         class_list.append('tag-index')
     if node.get('is_homepage_index'):
         class_list.append('homepage-index')
     if node.get('is_paged'):
         class_list.append('paged')
     if node.get('is_tag_base'):
         class_list.append('tag-base')
-    if node.get('is_node_index'): # Deprecated.
-        class_list.append('node-index')
     return class_list
 
 
 # Returns a list of all the node's descendant leaf nodes, i.e nodes with no children.
 def get_leaf_nodes(node):
     leaf_nodes = []
     for child in node.children:
@@ -61,18 +59,18 @@
     return leaf_nodes
 
 
 # Assembles a composite index for the homepage.
 def make_homepage_index(root_urls, sort_func, sort_rev, per_page):
     entries = []
     for url in root_urls:
-        if node := ivy.nodes.node(url):
+        if node := ark.nodes.node(url):
             entries.extend(get_leaf_nodes(node))
     sort_index(entries, sort_func, sort_rev)
-    node = ivy.nodes.root()
+    node = ark.nodes.root()
     node['index'] = entries
     node['is_index'] = True
     node['is_homepage_index'] = True
     split_index(node, per_page)
 
 
 # Assembles an index of all the node's descendant leaf nodes. Attaches this index to the node.
@@ -94,37 +92,37 @@
 
 
 # Checks all descendant nodes of the root node for tag strings. Parses tags, converts them into
 # Tag objects, assembles a set of tag index pages and attaches them to the root node.
 def make_tag_indexes(root_node, tag_slug, sort_func, sort_rev, per_tag_page):
     tag_base = root_node.child(tag_slug)
     if tag_base is None:
-        tag_base = ivy.nodes.Node()
+        tag_base = ark.nodes.Node()
         root_node.children.append(tag_base)
         tag_base.parent = root_node
         tag_base['slug'] = tag_slug
         tag_base['title'] = 'Tags'
 
     tag_map = {}
     url_base = root_node.url.rstrip('/') + f'/{tag_slug}/'
     def tag_parser(node):
         if (tagstring := node.get('tags')) is None:
             return
         node['tags'] = []
         for tag in (t.strip() for t in tagstring.split(',') if t.strip()):
             tag_map.setdefault(tag, []).append(node)
-            node['tags'].append(Tag(tag, url_base + ivy.utils.slugify(tag) + '//'))
+            node['tags'].append(Tag(tag, url_base + ark.utils.slugify(tag) + '//'))
     root_node.walk(tag_parser)
 
     for tag, node_list in tag_map.items():
-        slug = ivy.utils.slugify(tag)
+        slug = ark.utils.slugify(tag)
         if tag_node := tag_base.child(slug):
             tag_node.meta.setdefault('index', []).extend(node_list)
         else:
-            tag_node = ivy.nodes.Node()
+            tag_node = ark.nodes.Node()
             tag_base.children.append(tag_node)
             tag_node.parent = tag_base
             tag_node['title'] = tag
             tag_node['slug'] = slug
             tag_node['index'] = node_list
         sort_index(tag_node['index'], sort_func, sort_rev)
         tag_node['is_index'] = True
@@ -154,15 +152,15 @@
         node['is_paged'] = True
         node['page_num'] = 1
         node['total_pages'] = total_pages
         node['prev_url'] = ''
         node['next_url'] = next_url(node.url, 1, total_pages)
 
         for page in range(2, total_pages + 1):
-            page_node = ivy.nodes.Node()
+            page_node = ark.nodes.Node()
             node.children.append(page_node)
             page_node.parent = node
             page_node.meta = node.meta.copy()
             page_node['slug'] = f'{page}'
             page_node['index'] = entries[per_page * (page-1):per_page * page]
             page_node['page_num'] = page
             page_node['prev_url'] = prev_url(node.url, page)
```

### Comparing `holly-1.0.1/setup.py` & `holly-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 #!/usr/bin/env python3
 """
 Holly
 =====
 
-A blog-engine plugin for Ivy.
+A blog-engine plugin for Ark.
 
 """
 
 from setuptools import setup
 
 setup(
     name = 'holly',
-    version = '1.0.1',
+    version = '2.0.0',
     py_modules = ['holly'],
     author = 'Darren Mulholland',
     url = 'https://github.com/dmulholl/holly',
     license = 'Public Domain',
     description = (
-        'A blog-engine plugin for Ivy.'
+        'A blog-engine plugin for Ark.'
     ),
     long_description = __doc__,
     classifiers = [
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
         'License :: Public Domain',
         'Topic :: Text Processing :: Markup :: HTML',
```

