# Comparing `tmp/issue_db_api-0.6.0.tar.gz` & `tmp/issue_db_api-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.6.0.tar", last modified: Sat Apr 22 10:25:28 2023, max compression
+gzip compressed data, was "issue_db_api-0.6.1.tar", last modified: Sat Apr 29 11:50:42 2023, max compression
```

## Comparing `issue_db_api-0.6.0.tar` & `issue_db_api-0.6.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.0/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.603392 issue_db_api-0.6.0/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-22 10:24:52.000000 issue_db_api-0.6.0/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.0/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.0/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41564 2023-04-21 11:09:36.000000 issue_db_api-0.6.0/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.0/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    36247 2023-04-22 10:20:48.000000 issue_db_api-0.6.0/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-22 09:10:35.000000 issue_db_api-0.6.0/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3710 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6312 2023-04-22 09:15:44.000000 issue_db_api-0.6.0/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.0/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-22 10:25:28.603392 issue_db_api-0.6.0/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.0/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-22 10:25:28.000000 issue_db_api-0.6.0/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-22 10:24:52.000000 issue_db_api-0.6.0/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-22 10:25:28.607392 issue_db_api-0.6.0/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.0/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.6.1/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.994310 issue_db_api-0.6.1/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      469 2023-04-29 11:49:28.000000 issue_db_api-0.6.1/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-04-20 10:30:30.000000 issue_db_api-0.6.1/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8096 2023-04-22 09:15:44.000000 issue_db_api-0.6.1/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    42186 2023-04-29 11:42:32.000000 issue_db_api-0.6.1/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1041 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5280 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3780 2023-04-22 08:55:43.000000 issue_db_api-0.6.1/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1551 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     8676 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    36247 2023-04-22 10:20:48.000000 issue_db_api-0.6.1/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10977 2023-04-24 16:50:02.000000 issue_db_api-0.6.1/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3425 2023-04-29 11:39:02.000000 issue_db_api-0.6.1/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6312 2023-04-22 09:15:44.000000 issue_db_api-0.6.1/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1618 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2460 2023-04-22 09:10:31.000000 issue_db_api-0.6.1/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-04-29 11:50:41.994310 issue_db_api-0.6.1/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      748 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.6.1/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-04-29 11:50:41.000000 issue_db_api-0.6.1/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-04-29 11:49:28.000000 issue_db_api-0.6.1/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-04-29 11:50:41.998310 issue_db_api-0.6.1/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.6.1/setup.py
```

### Comparing `issue_db_api-0.6.0/LICENSE` & `issue_db_api-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/PKG-INFO` & `issue_db_api-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.6.0
+Version: 0.6.1
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.0/issue_db_api/issue_api.pyi` & `issue_db_api-0.6.1/issue_db_api/issue_api.pyi`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/api_core.rs` & `issue_db_api-0.6.1/issue_db_api/src/api_core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 /// This struct provides basics means of session management,
 /// and exposes all available endpoints through Rust functions.
 #[allow(unused)]
 #[derive(Debug, Clone)]
 pub struct IssueAPI {
     url: String,
     token: Option<String>,
-    client: Client
+    client: Client,
+    debug: bool
 }
 
 #[allow(unused)]
 #[derive(Debug, Clone)]
 pub struct IssueData {
     ident: String,
     key: Lazy<String>,
@@ -62,14 +63,15 @@
 }
 
 //////////////////////////////////////////////////////////////////////////////////////////////////
 //////////////////////////////////////////////////////////////////////////////////////////////////
 // Auxiliary structs and enums
 //////////////////////////////////////////////////////////////////////////////////////////////////
 
+#[derive(Debug)]
 #[allow(unused)]
 enum Verb {
     Get,
     Post,
     Patch,
     Put,
     Delete
@@ -269,15 +271,26 @@
         Ok(read_only_api)
     }
 
     pub(crate) fn new_read_only(url: String, allow_self_signed: bool) -> APIResult<Self> {
         let client = ClientBuilder::new()
             .danger_accept_invalid_certs(allow_self_signed)
             .build()?;
-        Ok(IssueAPI{url, token: None, client})
+        println!("Debug state: {}", Self::get_debug_state()?);
+        Ok(IssueAPI{url, token: None, client, debug: Self::get_debug_state()?})
+    }
+
+    fn get_debug_state() -> APIResult<bool> {
+        match std::env::var("ISSUE_API_CLIENT_DEBUG") {
+            Ok(value) => {
+                let converted = value.to_lowercase();
+                Ok(converted == "true" || converted == "1")
+            }
+            Err(_) => Ok(false)
+        }
     }
 
     fn login(&mut self, username: String, password: String) -> APIResult<()> {
         #[derive(serde::Deserialize)]
         struct TokenResponse {
             access_token: String,
             #[allow(dead_code)] token_type: String
@@ -341,17 +354,21 @@
     }
 
     fn call_endpoint_json<I, O>(&self,
                                 suffix: &str,
                                 verb: Verb,
                                 payload: I) -> APIResult<O>
     where
-        I: serde::Serialize,
+        I: serde::Serialize + std::fmt::Debug,
         O: for <'de> serde::Deserialize<'de>,
     {
+        if self.debug {
+            println!("Performing {:?} request to endpoint {}", verb, suffix);
+            println!("Request payload: {:?}", payload);
+        }
         let response = self.build_request_base(suffix, verb)?.json(&payload).send()?;
         let result = self.unpack_response(response)?;
         Ok(result)
     }
 
     fn call_endpoint_form<I, O>(&self,
                                 suffix: &str,
```

### Comparing `issue_db_api-0.6.0/issue_db_api/src/comments.rs` & `issue_db_api-0.6.1/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/config.rs` & `issue_db_api-0.6.1/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/embedding.rs` & `issue_db_api-0.6.1/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/errors.rs` & `issue_db_api-0.6.1/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/issues.rs` & `issue_db_api-0.6.1/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/labels.rs` & `issue_db_api-0.6.1/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/lib.rs` & `issue_db_api-0.6.1/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/models.rs` & `issue_db_api-0.6.1/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/query.rs` & `issue_db_api-0.6.1/issue_db_api/src/query.rs`

 * *Files 18% similar despite different names*

```diff
@@ -43,67 +43,67 @@
             }
             Query::Key(key) => {
                 let mut map = Map::new();
                 map.insert("key".to_string(), Value::String(key));
                 Value::Object(map)
             }
             Query::And(branches) => {
-                let mut json_branches: Vec<Value> = Vec::with_capacity(branches.len());
-                for branch in branches {
-                    json_branches.push(branch.into_json());
-                }
                 let mut map = Map::new();
-                map.insert("$and".to_string(), Value::Array(json_branches));
+                map.insert("$and".to_string(), serialize_logical_op_branches(branches));
                 Value::Object(map)
             }
             Query::Or(branches) => {
-                let mut json_branches: Vec<Value> = Vec::with_capacity(branches.len());
-                for branch in branches {
-                    json_branches.push(branch.into_json());
-                }
                 let mut map = Map::new();
-                map.insert("$or".to_string(), Value::Array(json_branches));
+                map.insert("$or".to_string(), serialize_logical_op_branches(branches));
                 Value::Object(map)
             }
         }
     }
 }
 
+fn serialize_logical_op_branches(arms: Vec<Query>) -> Value {
+    let mut json_branches: Vec<Value> = Vec::with_capacity(arms.len());
+    for branch in arms {
+        json_branches.push(branch.into_json());
+    }
+    Value::Array(json_branches)
+}
+
+
 impl Display for Query {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         match self {
             Query::Tag(cmp, name) => match cmp {
                 QueryCMP::Eq => write!(f, "{{\"tags\": {{\"$eq\": \"{}\"}}}}", name),
                 QueryCMP::Ne => write!(f, "{{\"tags\": {{\"$ne\": \"{}\"}}}}", name)
             },
             Query::Project(project) => write!(f, "{{\"tags\": {{\"$eq\": \"{}\"}}}}", project),
             Query::Identifier(ident) => write!(f, "{{\"_id\": {{\"$eq\": \"{}\"}}}}", ident),
             Query::Key(key) => write!(f, "{{\"key\": {{\"$eq\": \"{}\"}}}}", key),
-            Query::And(arms) => {
+            Query::And(arms)=> {
                 write!(f, "{{\"$and\": [")?;
-                let mut first = true;
-                for a in arms {
-                    if !first {
-                        write!(f, ", {}", a)?;
-                    } else {
-                        write!(f, "{}", a)?;
-                        first = false;
-                    }
-                }
+                write_logical_op_body(f, arms)?;
+                write!(f, "]")?;
                 Ok(())
             },
             Query::Or(arms) => {
                 write!(f, "{{\"$or\": [")?;
-                let mut first = true;
-                for a in arms {
-                    if !first {
-                        write!(f, ", {}", a)?;
-                    } else {
-                        write!(f, "{}", a)?;
-                        first = false;
-                    }
-                }
+                write_logical_op_body(f, arms)?;
+                write!(f, "]")?;
                 Ok(())
             }
         }
     }
 }
+
+fn write_logical_op_body(f: &mut Formatter<'_>, arms: &Vec<Query>) -> std::fmt::Result {
+    let mut first = true;
+    for a in arms {
+        if !first {
+            write!(f, ", {}", a)?;
+        } else {
+            write!(f, "{}", a)?;
+            first = false;
+        }
+    }
+    Ok(())
+}
```

### Comparing `issue_db_api-0.6.0/issue_db_api/src/repository.rs` & `issue_db_api-0.6.1/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.6.1/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/tags.rs` & `issue_db_api-0.6.1/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api/src/util.rs` & `issue_db_api-0.6.1/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.6.1/issue_db_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.6.0
+Version: 0.6.1
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.6.0/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.6.1/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.6.0/pyproject.toml` & `issue_db_api-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

