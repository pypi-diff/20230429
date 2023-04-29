# Comparing `tmp/curriculum_analysis-0.2.5.tar.gz` & `tmp/curriculum_analysis-0.2.6.tar.gz`

## Comparing `curriculum_analysis-0.2.5.tar` & `curriculum_analysis-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/analysis.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/config.cfg.default
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/corpus.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/csv_exporter.py
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/js_exporter.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/json_exporter.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/keywords.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/keywords.txt
--rw-r--r--   0        0        0     2529 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/main.py
--rw-r--r--   0        0        0     8805 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/txt_parser.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/data.js
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/index.html
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/index.js
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/module.html
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/module.js
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/curriculum_analysis/html/style.css
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/LICENCE
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/README.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/analysis.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/config.cfg.default
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/corpus.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/csv_exporter.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/js_exporter.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/json_exporter.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/keywords.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/keywords.txt
+-rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/main.py
+-rw-r--r--   0        0        0     8806 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/txt_parser.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/html/data.js
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/html/index.html
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/html/index.js
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/html/module.html
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/curriculum_analysis/html/module.js
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/LICENCE
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/README.md
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 curriculum_analysis-0.2.6/PKG-INFO
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/analysis.py` & `curriculum_analysis-0.2.6/curriculum_analysis/analysis.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,26 +6,44 @@
 log = logging.getLogger(__name__)
 
 class Analysis:
     def __init__(self, obj):
         self.name = str(obj)
         self.corpora = {section: Corpus(section, text) for section, text in obj.corpora().items()}
         self.results = {}
+        self.alternative = {}
         self.summary = defaultdict(int)
+        self.total = 0
 
     def analyse(self, keywords, **kwargs):
+        self.keywords = keywords
         for kw in keywords:
             result = self.check_for_keyword(kw, **kwargs)
             self.results[kw] = result
             for section in result:
                 self.summary[kw] += len(result[section])
-        if sum(self.summary.values()):
-            log.debug(f"found '{sum(self.summary.values())}' keywords in {self.name}")
+        self.total = sum(self.summary.values())
+        if self.total:
+            log.debug(f"found '{self.total}' keywords in {self.name}")
+
+    def analyse_alternative(self, keywords):
+        for section, corpus in self.corpora.items():
+            keyword_indices = {
+                keyword: corpus.find_indices(keyword) for keyword in keywords
+            }
+            total = sum([len(indices) for _, indices in keyword_indices.items()])
+            self.alternative[section] = {
+                "tokens": corpus.tokens,
+                "keywords": keyword_indices,
+                "total": total,
+            }
+            self.total += total 
+
 
     def check_for_keyword(self, keyword, **kwargs):
         return {
             section: c.delemmatized_concordance_list(keyword, **kwargs) 
             for section, c in self.corpora.items()
         }
-    
+
     def raw(self):
         return {section: self.corpora[section].raw_string for section in self.corpora.keys()}
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/corpus.py` & `curriculum_analysis-0.2.6/curriculum_analysis/corpus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Corpus instances are initialised with text and can calculate everything we need"""
 
 import nltk
 from nltk.stem import WordNetLemmatizer
 
 nltk.download('wordnet', quiet=True)
+nltk.download('punkt', quiet=True)
+
 lemmatizer = WordNetLemmatizer()
 
 def slice_from_concordance(con):
     return slice(
         con.offset - len(con.left),
         con.offset + len(con.right) + 1
     )
@@ -25,14 +27,20 @@
         self.tokens = [word.lower() for sent in nltk.sent_tokenize(text) for word in nltk.word_tokenize(sent)]
         self.lemmatized_tokens = [lemmatizer.lemmatize(t) for t in self.tokens]
         self.text = nltk.text.Text(self.tokens)
         self.lemmatized_text = nltk.text.Text(self.lemmatized_tokens)
         self.vocab = self.text.vocab()
         self.lemmatized_vocab = self.lemmatized_text.vocab()
 
+    def find_indices(self, keyword):
+        if keyword not in self.lemmatized_vocab:
+            return []
+        return [i for i, token in enumerate(self.lemmatized_tokens) if token == keyword]
+
+
     def delemmatized_concordance_list(self, kw, **kwargs):
         lemmatized = self.lemmatized_text.concordance_list(kw, **kwargs)
         return [delemmatize(l, self.tokens) for l in lemmatized]
 
     def __repr__(self):
         return f"Corpus({self.label})"
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/csv_exporter.py` & `curriculum_analysis-0.2.6/curriculum_analysis/csv_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/js_exporter.py` & `curriculum_analysis-0.2.6/curriculum_analysis/js_exporter.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,35 +8,54 @@
 log = logging.getLogger(__name__)
 
 class JSExporter:
     def __init__(self, file, output_path):
         self.file = file
         self.output_path = output_path / file.path.stem
         self.output_path.mkdir(parents=True, exist_ok=True)
-        self.code_header = f"{self.file.type} code"
-        self.name_header = f"{self.file.type} full title"
         self.data_path = self.output_path / 'data.js'
+        self.pages_path = output_path / 'pages.js'
 
     def export(self, keywords):
         result = []
         for obj in self.file:
             analysis = Analysis(obj)
-            analysis.analyse(keywords)
+            analysis.analyse_alternative(keywords)
             record = {
                 "code": obj.code,
                 "title": obj.full_title,
-                "data": analysis.results,
-                "summary": analysis.summary,
-                "raw": analysis.raw()
+                "results": analysis.alternative,
+                "total": analysis.total,
             }
             result.append(record)
         json_string = json.dumps(result)
         js_string = f"""
         async function loadJSON() {{ 
             return {json_string}; 
         }}
         """
         log.info(f"exporting results as HTML to {self.output_path.absolute()}")
         log.setLevel(logging.WARN)
         copy_tree(str(Path(__file__).parent / 'html'), str(self.output_path), update=True)
         with self.data_path.open('w') as data_script:
-            data_script.write(js_string)
+            data_script.write(js_string)
+        self.recreate_index()
+    
+    def recreate_index(self):
+        result = []
+        folders = [folder for folder in self.output_path.parent.iterdir() if folder.is_dir()]
+        for folder in folders:
+            if (folder / 'index.html').exists():
+                page = {
+                    'title': folder.name,
+                    'url': str(Path(folder.name) / 'index.html')
+                }
+                result.append(page)
+        json_string = json.dumps(result)
+        js_string = f"""
+        async function loadJSON() {{
+            return {json_string}
+        }}
+        """
+        copy_tree(str(Path(__file__).parent / 'top-level'), str(self.output_path.parent), update=True)
+        with self.pages_path.open('w') as pages_script:
+            pages_script.write(js_string)
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/json_exporter.py` & `curriculum_analysis-0.2.6/curriculum_analysis/json_exporter.py`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/main.py` & `curriculum_analysis-0.2.6/curriculum_analysis/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 def main(filename, conf):
     # check the provided config file exists
     conf_path = Path(conf).expanduser()
     conf_path.parent.mkdir(exist_ok=True)
     if not conf_path.exists():
         print(f"Wait! We are missing the configuration file at {conf_path}")
         default = (Path(__file__).parent / 'config.cfg.default').read_text()
-        conf_path.write_text(default);
+        conf_path.write_text(default)
         print(f"We added this configuration to the file for you.\n")
         print(default)
         print(f"For now, we are aborting.")
         print(f"Please check/edit the configuration before running again.")
         exit()
 
     # load the config file
@@ -40,15 +40,15 @@
     log.info(f"reading config from {conf_path}")
     config.read(conf_path)
 
     # Load keywords
     keyword_path = Path(config.get("curriculumAnalysis", "keywords_path")).expanduser()
     if not keyword_path.exists():
         default = (Path(__file__).parent / 'keywords.txt').read_text()
-        keyword_path.write_text(default);
+        keyword_path.write_text(default)
     keywords = load_keywords_file(keyword_path)
 
     # load the data
     file = file_factory(Path(filename).expanduser())
 
     # Generate an analysis
     outpath = Path(config.get("curriculumAnalysis", "outpath")).expanduser()
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/txt_parser.py` & `curriculum_analysis-0.2.6/curriculum_analysis/txt_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     def __str__(self):
         return f"Programme({self.code})"
 
     def corpora(self):
         return {
             "description": self.description,
-            "learning_teaching_and_assessment_strategies": self.learning_teaching_and_assessment_strategies,
+            "learning, teaching and assessment strategies": self.learning_teaching_and_assessment_strategies,
             "learning outcomes": self.learning_outcomes
         }
 
 
 class Module:
     def __init__(self, data):
         assert data[3] == "Module Specification"
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/html/index.html` & `curriculum_analysis-0.2.6/curriculum_analysis/html/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Document</title>
-    <link rel="stylesheet" href="style.css">
+    <link rel="stylesheet" href="../style.css">
 </head>
 <body>
     <header>
         <h1>Curriculum Analysis</h1>
+        <a href="../index.html">Home</a>
     </header>
     <main>
         <table id="target">
             <tr>
                 <th id="code_header">Code</th>
                 <th id="title_header">Title</th>
                 <th id="details_header">Keywords found</th>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 
 
 ****** Curriculum Analysis ******
-
+Home
 Code Title Keywords found
```

### Comparing `curriculum_analysis-0.2.5/curriculum_analysis/html/module.html` & `curriculum_analysis-0.2.6/curriculum_analysis/html/module.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 <!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Module</title>
-    <link rel="stylesheet" href="style.css">
+    <link rel="stylesheet" href="../style.css">
 </head>
 <body>
     <header>
-        <div>
-            <h1 id="itemCode">Module</h1>
-            <p id="itemName"></p>
-        </div>
+        <h1 id="itemCode">Module</h1>
+        <p id="itemName"></p>
         <a href="index.html">Back</a>
     </header>
     <main id="target"></main>
     <script src="data.js"></script>
     <script src="module.js"></script>
 </body>
 </html>
```

### Comparing `curriculum_analysis-0.2.5/LICENCE` & `curriculum_analysis-0.2.6/LICENCE`

 * *Files identical despite different names*

### Comparing `curriculum_analysis-0.2.5/README.md` & `curriculum_analysis-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 
 The default configuration file (`config.cfg`) is placed in the users home directory under a hidden folder `~/.curriculumAnalysis`.
 
 ```
 [curriculummAnalysis]
 keywords_path = ~/.curriculumAnalysis/keywords.txt
 outpath = ~/.curriculumAnalysis/output
-format = json
+format = js
 ```
 
 Changing these values will influence the default settings.
 
 ## Example usage
 
 ```
 curriculum-analysis modules.txt
 ```
-
```

### Comparing `curriculum_analysis-0.2.5/pyproject.toml` & `curriculum_analysis-0.2.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -8,18 +8,18 @@
   "curriculum_analysis/keywords.txt",
   "curriculum_analysis/html/*",
   "**/*.py",  
 ]
 
 [project]
 name = "curriculum_analysis"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
-  { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
   { name="Tom Harrison" },
+  { name="Graeme Stuart", email="gstuart@dmu.ac.uk" },
 ]
 description = "A simple tool for analysing DMU module and programme specifications with respect to provided keywords."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `curriculum_analysis-0.2.5/PKG-INFO` & `curriculum_analysis-0.2.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curriculum_analysis
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple tool for analysing DMU module and programme specifications with respect to provided keywords.
 Project-URL: Homepage, https://github.com/IESD/curriculumAnalysis
 Project-URL: Bug Tracker, https://github.com/IESD/curriculumAnalysis/issues
 Author: Tom Harrison
 Author-email: Graeme Stuart <gstuart@dmu.ac.uk>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
@@ -39,18 +39,17 @@
 
 The default configuration file (`config.cfg`) is placed in the users home directory under a hidden folder `~/.curriculumAnalysis`.
 
 ```
 [curriculummAnalysis]
 keywords_path = ~/.curriculumAnalysis/keywords.txt
 outpath = ~/.curriculumAnalysis/output
-format = json
+format = js
 ```
 
 Changing these values will influence the default settings.
 
 ## Example usage
 
 ```
 curriculum-analysis modules.txt
 ```
-
```

