# Comparing `tmp/issue_db_api-0.6.1.tar.gz` & `tmp/issue_db_api-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.6.1.tar", last modified: Sat Apr 29 11:50:42 2023, max compression
+gzip compressed data, was "issue_db_api-0.6.2.tar", last modified: Sat Apr 29 11:57:38 2023, max compression
```

## Comparing `issue_db_api-0.6.1.tar` & `issue_db_api-0.6.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.1/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.994310 issue_db_api-0.6.1/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-29 11:49:28.000000 issue_db_api-0.6.1/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.1/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.1/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    42186 2023-04-29 11:42:32.000000 issue_db_api-0.6.1/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.1/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    36247 2023-04-22 10:20:48.000000 issue_db_api-0.6.1/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.1/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3425 2023-04-29 11:39:02.000000 issue_db_api-0.6.1/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6312 2023-04-22 09:15:44.000000 issue_db_api-0.6.1/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.1/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.994310 issue_db_api-0.6.1/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.1/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-29 11:49:28.000000 issue_db_api-0.6.1/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.939976 issue_db_api-0.6.2/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.2/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-29 11:56:56.000000 issue_db_api-0.6.2/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.2/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.2/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    42186 2023-04-29 11:42:32.000000 issue_db_api-0.6.2/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.2/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    36247 2023-04-22 10:20:48.000000 issue_db_api-0.6.2/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.2/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3425 2023-04-29 11:39:02.000000 issue_db_api-0.6.2/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6385 2023-04-29 11:56:43.000000 issue_db_api-0.6.2/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.2/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:57:38.935976 issue_db_api-0.6.2/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.2/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-29 11:57:38.000000 issue_db_api-0.6.2/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-29 11:56:56.000000 issue_db_api-0.6.2/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-29 11:57:38.939976 issue_db_api-0.6.2/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.2/setup.py
```

### Comparing `issue_db_api-0.6.1/LICENSE` & `issue_db_api-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/PKG-INFO` & `issue_db_api-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.6.1
+Version: 0.6.2
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.1/issue_db_api/issue_api.pyi` & `issue_db_api-0.6.2/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/api_core.rs` & `issue_db_api-0.6.2/issue_db_api/src/api_core.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/comments.rs` & `issue_db_api-0.6.2/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/config.rs` & `issue_db_api-0.6.2/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/embedding.rs` & `issue_db_api-0.6.2/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/errors.rs` & `issue_db_api-0.6.2/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/issues.rs` & `issue_db_api-0.6.2/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/labels.rs` & `issue_db_api-0.6.2/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/lib.rs` & `issue_db_api-0.6.2/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/models.rs` & `issue_db_api-0.6.2/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/query.rs` & `issue_db_api-0.6.2/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/repository.rs` & `issue_db_api-0.6.2/issue_db_api/src/repository.rs`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,17 @@
         )
     }
 
     pub fn search(&self,
                   query: Query,
                   issue_loading_settings: IssueLoadingSettings) -> APIResult<Vec<Issue>> {
         let ids = self.api.search(query)?;
+        if ids.is_empty() {
+            return Ok(Vec::new());
+        }
         issue_loading_settings.load_issues(self.api.clone(),
                                            ids,
                                            self.label_caching)
     }
 
     pub fn find_issue_by_key(&self,
                              project: String,
```

### Comparing `issue_db_api-0.6.1/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.6.2/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/tags.rs` & `issue_db_api-0.6.2/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api/src/util.rs` & `issue_db_api-0.6.2/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.6.2/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.6.1
+Version: 0.6.2
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.1/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.6.2/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.1/pyproject.toml` & `issue_db_api-0.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

