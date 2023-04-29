# Comparing `tmp/llm_generation_server-0.0.8.tar.gz` & `tmp/llm_generation_server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_generation_server-0.0.8.tar", last modified: Sat Apr 29 15:34:27 2023, max compression
+gzip compressed data, was "llm_generation_server-0.0.9.tar", last modified: Sat Apr 29 15:57:09 2023, max compression
```

## Comparing `llm_generation_server-0.0.8.tar` & `llm_generation_server-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/llm_generation_server/
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/component_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/llm_generation_server/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/llm_generation_server/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/dist/assets/index-0babc66b.css
--rw-r--r--   0 runner    (1001) docker     (123)   200409 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/dist/assets/index-5384adf7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/dist/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/llm_generation_server/elements/
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/elements/barchart_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/elements/element_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/elements/plain_text_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/elements/selector_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/elements/table_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/elements/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/llm_generation_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/llm_generation_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 15:34:27.000000 llm_generation_server-0.0.8/llm_generation_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-29 15:34:27.000000 llm_generation_server-0.0.8/llm_generation_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:34:27.000000 llm_generation_server-0.0.8/llm_generation_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 15:34:27.000000 llm_generation_server-0.0.8/llm_generation_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 15:34:27.000000 llm_generation_server-0.0.8/llm_generation_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 15:34:16.000000 llm_generation_server-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:34:27.294998 llm_generation_server-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/llm_generation_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/component_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/llm_generation_server/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/llm_generation_server/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   200409 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/dist/assets/index-054c6326.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/dist/assets/index-064f0851.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/dist/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/llm_generation_server/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/elements/barchart_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/elements/element_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/elements/plain_text_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/elements/selector_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/elements/table_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/elements/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/llm_generation_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/llm_generation_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-29 15:57:09.000000 llm_generation_server-0.0.9/llm_generation_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-29 15:57:09.000000 llm_generation_server-0.0.9/llm_generation_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:57:09.000000 llm_generation_server-0.0.9/llm_generation_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 15:57:09.000000 llm_generation_server-0.0.9/llm_generation_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-29 15:57:09.000000 llm_generation_server-0.0.9/llm_generation_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 15:56:58.000000 llm_generation_server-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:57:09.149719 llm_generation_server-0.0.9/setup.cfg
```

### Comparing `llm_generation_server-0.0.8/LICENSE` & `llm_generation_server-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/PKG-INFO` & `llm_generation_server-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: llm_generation_server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple full stack app for displaying distribution of next token.
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visualize_llm_generation
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visualize_llm_generation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.8`
+## VERSION: `0.0.9`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.0.8/README.md` & `llm_generation_server-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.8`
+## VERSION: `0.0.9`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.0.8/llm_generation_server/component_base.py` & `llm_generation_server-0.0.9/llm_generation_server/component_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/dist/assets/index-0babc66b.css` & `llm_generation_server-0.0.9/llm_generation_server/dist/assets/index-064f0851.css`

 * *Files 12% similar despite different names*

```diff
@@ -1 +1 @@
-.inline-bar-block[data-v-f28118db]{display:flex;padding-top:1px;padding-bottom:1px;margin-left:5px}.inline-bar-block-text[data-v-f28118db]{font-size:small;text-align:center;color:#75757588}.multiline-bar-block[data-v-f28118db]{display:flex;column-gap:10px;margin-top:5px;flex-wrap:wrap}.track[data-v-f28118db]{display:inline-block;background:#ebebeb;width:100%}.track-fill[data-v-f28118db]{background:#666;display:inline-block;height:100%}.prob-text[data-v-f28118db]{color:azure;margin-left:2px}.rounded .track[data-v-f28118db],.rounded .track-fill[data-v-f28118db]{box-shadow:inset 0 0 5px #0003;border-radius:3px}.word-text[data-v-f28118db]{display:inline-block;width:fit-content;overflow:auto;margin-bottom:-7px;margin-right:5px}.context-text[data-v-f28118db]{width:100%;overflow:auto;font-size:large;background-color:#e0e0e0;padding:5px}.single-bar-wrapper[data-v-f28118db]{width:200px;flex-grow:1}.input-radio[data-v-1a24ee3a]{margin-right:10px}.progress-bar[data-v-1a24ee3a]{margin-top:10px;display:flex}.selectorWrapper[data-v-30377ad5]{width:fit-content;display:inline-block}.checkbox-text[data-v-9f0e25b2]{margin-right:5px}[data-v-764daa31] .sample-selector{font-family:sans-serif;font-weight:400;padding:5px}[data-v-764daa31] .button{display:inline-block;padding:5px 10px;margin-left:5px}[data-v-764daa31] .descr{margin-right:5px}.subSelectorsWrapper[data-v-764daa31]{display:flex;flex-wrap:wrap;justify-content:space-evenly}.buttonWrapper[data-v-764daa31]{text-align:center}.table-wrapper h3[data-v-cc0331df]{text-align:center;margin-top:0}.table-wrapper[data-v-cc0331df]{width:fit-content;background-color:#00000020;border-style:dashed;border-width:1px;padding:5px;border-radius:5px;box-shadow:0 35px 50px #0003;flex:none}.table-style-0[data-v-cc0331df]{border-radius:5px;font-size:12px;font-weight:400;border:none;border-collapse:collapse;max-width:100%;white-space:nowrap;background-color:#fff}.table-style-0 td[data-v-cc0331df],.table-style-0 th[data-v-cc0331df]{text-align:left;padding:8px}.table-style-0 td[data-v-cc0331df]{border-right:1px solid #f8f8f8;font-size:12px}.table-style-0 thead th[data-v-cc0331df]{color:#fff;background:#7c7c7c;padding-right:10px;padding-left:10px}.table-style-0 thead th[data-v-cc0331df]:nth-child(odd){color:#fff;background:#6d6d6d;padding-right:10px;padding-left:10px}.table-style-0 tr[data-v-cc0331df]:nth-child(even){background:#efeeee;padding-right:10px;padding-left:10px}.table-style-0 .active[data-v-cc0331df]{background:#fbd0d0!important}.spacedTables[data-v-cc0331df]{display:flex;flex-direction:column;row-gap:5px;align-items:center}nav[data-v-32f10cfc]{margin-bottom:10px;background-color:silver;margin-top:-2rem;margin-right:-2rem;margin-left:-2rem}.notLoaded[data-v-32f10cfc]{text-align:center}.router-link-active[data-v-32f10cfc]{color:#000}:root{--vt-c-white: #ffffff;--vt-c-white-soft: #f8f8f8;--vt-c-white-mute: #f2f2f2;--vt-c-black: #181818;--vt-c-black-soft: #222222;--vt-c-black-mute: #282828;--vt-c-indigo: #2c3e50;--vt-c-divider-light-1: rgba(60, 60, 60, .29);--vt-c-divider-light-2: rgba(60, 60, 60, .12);--vt-c-divider-dark-1: rgba(84, 84, 84, .65);--vt-c-divider-dark-2: rgba(84, 84, 84, .48);--vt-c-text-light-1: var(--vt-c-indigo);--vt-c-text-light-2: rgba(60, 60, 60, .66);--vt-c-text-dark-1: var(--vt-c-white);--vt-c-text-dark-2: rgba(235, 235, 235, .64)}:root{--color-background: var(--vt-c-white);--color-background-soft: var(--vt-c-white-soft);--color-background-mute: var(--vt-c-white-mute);--color-border: var(--vt-c-divider-light-2);--color-border-hover: var(--vt-c-divider-light-1);--color-heading: var(--vt-c-text-light-1);--color-text: var(--vt-c-text-light-1);--section-gap: 160px}@media (prefers-color-scheme: dark){:root{--color-background: var(--vt-c-black);--color-background-soft: var(--vt-c-black-soft);--color-background-mute: var(--vt-c-black-mute);--color-border: var(--vt-c-divider-dark-2);--color-border-hover: var(--vt-c-divider-dark-1);--color-heading: var(--vt-c-text-dark-1);--color-text: var(--vt-c-text-dark-2)}}*,*:before,*:after{box-sizing:border-box;margin:0;position:relative;font-weight:400}body{min-height:100vh;color:var(--color-text);background:var(--color-background);transition:color .5s,background-color .5s;line-height:1.6;font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;font-size:15px;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}#app{margin:0 auto;padding:2rem;font-weight:400}h2{border-bottom:1px solid #999;font-family:sans-serif;font-weight:400;color:#333}h3{border-bottom:1px solid #999;font-family:sans-serif;font-weight:lighter;margin-top:10px}.button{background-color:#00000068;padding:20px;font-family:sans-serif;font-weight:400;text-decoration:none;font-size:large;color:#3b3b3b;margin-right:2px;display:inline-block;box-shadow:inset 0 0 5px #0003}.button:hover{background-color:#0000004d}.wrapElement{box-shadow:#00000029 0 10px 36px,#0000000f 0 0 0 1px;padding:5px;margin:5px}
+.inline-bar-block[data-v-f28118db]{display:flex;padding-top:1px;padding-bottom:1px;margin-left:5px}.inline-bar-block-text[data-v-f28118db]{font-size:small;text-align:center;color:#75757588}.multiline-bar-block[data-v-f28118db]{display:flex;column-gap:10px;margin-top:5px;flex-wrap:wrap}.track[data-v-f28118db]{display:inline-block;background:#ebebeb;width:100%}.track-fill[data-v-f28118db]{background:#666;display:inline-block;height:100%}.prob-text[data-v-f28118db]{color:azure;margin-left:2px}.rounded .track[data-v-f28118db],.rounded .track-fill[data-v-f28118db]{box-shadow:inset 0 0 5px #0003;border-radius:3px}.word-text[data-v-f28118db]{display:inline-block;width:fit-content;overflow:auto;margin-bottom:-7px;margin-right:5px}.context-text[data-v-f28118db]{width:100%;overflow:auto;font-size:large;background-color:#e0e0e0;padding:5px}.single-bar-wrapper[data-v-f28118db]{width:200px;flex-grow:1}.input-radio[data-v-1a24ee3a]{margin-right:10px}.progress-bar[data-v-1a24ee3a]{margin-top:10px;display:flex}.selectorWrapper[data-v-30377ad5]{width:fit-content;display:inline-block}.checkbox-text[data-v-9f0e25b2]{margin-right:5px}[data-v-764daa31] .sample-selector{font-family:sans-serif;font-weight:400;padding:5px}[data-v-764daa31] .button{display:inline-block;padding:5px 10px;margin-left:5px}[data-v-764daa31] .descr{margin-right:5px}.subSelectorsWrapper[data-v-764daa31]{display:flex;flex-wrap:wrap;justify-content:space-evenly}.buttonWrapper[data-v-764daa31]{text-align:center}.table-wrapper h3[data-v-6527bbd4]{text-align:center;margin-top:0}.table-wrapper[data-v-6527bbd4]{display:flex;justify-content:center;align-items:center;flex-direction:column;width:fit-content;background-color:#00000020;border-style:dashed;border-width:1px;padding:5px;border-radius:5px;box-shadow:0 35px 50px #0003}.table-style-0[data-v-6527bbd4]{border-radius:5px;font-size:12px;font-weight:400;border:none;border-collapse:collapse;max-width:100%;white-space:nowrap;background-color:#fff}.table-style-0 td[data-v-6527bbd4],.table-style-0 th[data-v-6527bbd4]{text-align:left;padding:8px}.table-style-0 td[data-v-6527bbd4]{border-right:1px solid #f8f8f8;font-size:12px}.table-style-0 thead th[data-v-6527bbd4]{color:#fff;background:#7c7c7c;padding-right:10px;padding-left:10px}.table-style-0 thead th[data-v-6527bbd4]:nth-child(odd){color:#fff;background:#6d6d6d;padding-right:10px;padding-left:10px}.table-style-0 tr[data-v-6527bbd4]:nth-child(even){background:#efeeee;padding-right:10px;padding-left:10px}.table-style-0 .active[data-v-6527bbd4]{background:#fbd0d0!important}.spacedTables[data-v-6527bbd4]{display:flex;flex-direction:column;row-gap:5px;align-items:center}nav[data-v-32f10cfc]{margin-bottom:10px;background-color:silver;margin-top:-2rem;margin-right:-2rem;margin-left:-2rem}.notLoaded[data-v-32f10cfc]{text-align:center}.router-link-active[data-v-32f10cfc]{color:#000}:root{--vt-c-white: #ffffff;--vt-c-white-soft: #f8f8f8;--vt-c-white-mute: #f2f2f2;--vt-c-black: #181818;--vt-c-black-soft: #222222;--vt-c-black-mute: #282828;--vt-c-indigo: #2c3e50;--vt-c-divider-light-1: rgba(60, 60, 60, .29);--vt-c-divider-light-2: rgba(60, 60, 60, .12);--vt-c-divider-dark-1: rgba(84, 84, 84, .65);--vt-c-divider-dark-2: rgba(84, 84, 84, .48);--vt-c-text-light-1: var(--vt-c-indigo);--vt-c-text-light-2: rgba(60, 60, 60, .66);--vt-c-text-dark-1: var(--vt-c-white);--vt-c-text-dark-2: rgba(235, 235, 235, .64)}:root{--color-background: var(--vt-c-white);--color-background-soft: var(--vt-c-white-soft);--color-background-mute: var(--vt-c-white-mute);--color-border: var(--vt-c-divider-light-2);--color-border-hover: var(--vt-c-divider-light-1);--color-heading: var(--vt-c-text-light-1);--color-text: var(--vt-c-text-light-1);--section-gap: 160px}@media (prefers-color-scheme: dark){:root{--color-background: var(--vt-c-black);--color-background-soft: var(--vt-c-black-soft);--color-background-mute: var(--vt-c-black-mute);--color-border: var(--vt-c-divider-dark-2);--color-border-hover: var(--vt-c-divider-dark-1);--color-heading: var(--vt-c-text-dark-1);--color-text: var(--vt-c-text-dark-2)}}*,*:before,*:after{box-sizing:border-box;margin:0;position:relative;font-weight:400}body{min-height:100vh;color:var(--color-text);background:var(--color-background);transition:color .5s,background-color .5s;line-height:1.6;font-family:Inter,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Oxygen,Ubuntu,Cantarell,Fira Sans,Droid Sans,Helvetica Neue,sans-serif;font-size:15px;text-rendering:optimizeLegibility;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}#app{margin:0 auto;padding:2rem;font-weight:400}h2{border-bottom:1px solid #999;font-family:sans-serif;font-weight:400;color:#333}h3{border-bottom:1px solid #999;font-family:sans-serif;font-weight:lighter;margin-top:10px}.button{background-color:#00000068;padding:20px;font-family:sans-serif;font-weight:400;text-decoration:none;font-size:large;color:#3b3b3b;margin-right:2px;display:inline-block;box-shadow:inset 0 0 5px #0003}.button:hover{background-color:#0000004d}.wrapElement{box-shadow:#00000029 0 10px 36px,#0000000f 0 0 0 1px;padding:5px;margin:5px}
```

### Comparing `llm_generation_server-0.0.8/llm_generation_server/dist/assets/index-5384adf7.js` & `llm_generation_server-0.0.9/llm_generation_server/dist/assets/index-054c6326.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -8413,15 +8413,15 @@
         class: So({
             active: e.displayedLinksRowID == `${c.id}_${h}`
         })
     }, [(Pe(!0), Ne(St, null, mn(d, S => (Pe(), Ne("td", null, mt(S), 1))), 256))], 10, uh))), 256))])])]))), 256))])
 }
 const fh = yn(aa, [
     ["render", ch],
-    ["__scopeId", "data-v-cc0331df"]
+    ["__scopeId", "data-v-6527bbd4"]
 ]);
 async function dh(e, t, s, o) {
     var d;
     let i = e.$router.currentRoute.value.name;
     if (i == null) throw TypeError();
     let a = i.toString(),
         c = e.$default_fetch_paths[a];
```

### Comparing `llm_generation_server-0.0.8/llm_generation_server/dist/favicon.ico` & `llm_generation_server-0.0.9/llm_generation_server/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/elements/barchart_element.py` & `llm_generation_server-0.0.9/llm_generation_server/elements/barchart_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/elements/element_base.py` & `llm_generation_server-0.0.9/llm_generation_server/elements/element_base.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/elements/plain_text_element.py` & `llm_generation_server-0.0.9/llm_generation_server/elements/plain_text_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/elements/selector_element.py` & `llm_generation_server-0.0.9/llm_generation_server/elements/selector_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/elements/table_element.py` & `llm_generation_server-0.0.9/llm_generation_server/elements/table_element.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/elements/utils.py` & `llm_generation_server-0.0.9/llm_generation_server/elements/utils.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server/server.py` & `llm_generation_server-0.0.9/llm_generation_server/server.py`

 * *Files identical despite different names*

### Comparing `llm_generation_server-0.0.8/llm_generation_server.egg-info/PKG-INFO` & `llm_generation_server-0.0.9/llm_generation_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: llm-generation-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple full stack app for displaying distribution of next token.
 Author-email: "Frantisek Trebuna (gortibaldik)" <ferotre@gmail.com>
 Project-URL: Homepage, https://github.com/gortibaldik/visualize_llm_generation
 Project-URL: Bug Tracker, https://github.com/gortibaldik/visualize_llm_generation/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Conditional Language Model Generation Visualization
 
-## VERSION: `0.0.8`
+## VERSION: `0.0.9`
 
 - when evaluating language models it is often pain to see what is generated and why
 - this little package is a `vue.js` frontend together with `flask` backend and it is designed to easily show some interesting visualizations on conditional generation models
 - it handles frontend-backend communication as well as frontend rendering
 - hence the developper can focus only on ML aspects of his work!
 
 ## Installation
```

### Comparing `llm_generation_server-0.0.8/llm_generation_server.egg-info/SOURCES.txt` & `llm_generation_server-0.0.9/llm_generation_server.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 llm_generation_server.egg-info/PKG-INFO
 llm_generation_server.egg-info/SOURCES.txt
 llm_generation_server.egg-info/dependency_links.txt
 llm_generation_server.egg-info/requires.txt
 llm_generation_server.egg-info/top_level.txt
 llm_generation_server/dist/favicon.ico
 llm_generation_server/dist/index.html
-llm_generation_server/dist/assets/index-0babc66b.css
-llm_generation_server/dist/assets/index-5384adf7.js
+llm_generation_server/dist/assets/index-054c6326.js
+llm_generation_server/dist/assets/index-064f0851.css
 llm_generation_server/elements/barchart_element.py
 llm_generation_server/elements/element_base.py
 llm_generation_server/elements/plain_text_element.py
 llm_generation_server/elements/selector_element.py
 llm_generation_server/elements/table_element.py
 llm_generation_server/elements/utils.py
```

### Comparing `llm_generation_server-0.0.8/pyproject.toml` & `llm_generation_server-0.0.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "llm_generation_server"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Frantisek Trebuna (gortibaldik)", email="ferotre@gmail.com" },
 ]
 description = "Simple full stack app for displaying distribution of next token."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -31,15 +31,15 @@
 [tool.setuptools.package-dir]
 llm_generation_server = "llm_generation_server"
 
 [tool.isort]
 profile = "black"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

