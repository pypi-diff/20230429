# Comparing `tmp/pyscemu-0.1.1.tar.gz` & `tmp/pyscemu-0.1.2.tar.gz`

## Comparing `pyscemu-0.1.1.tar` & `pyscemu-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.1/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.1/.gitignore
--rw-r--r--   0     1000     1000     9611 2023-04-29 18:27:14.000000 pyscemu-0.1.1/README.md
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.1/examples/xloader_dexor.py
--rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.1/examples/xloader_keygen.py
--rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.1/pyproject.toml
--rw-r--r--   0     1000     1000    24020 2023-04-29 18:27:36.000000 pyscemu-0.1.1/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-04-29 18:27:36.000000 pyscemu-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     9937 1970-01-01 00:00:00.000000 pyscemu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.2/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.2/.gitignore
+-rw-r--r--   0     1000     1000     9727 2023-04-29 19:27:52.000000 pyscemu-0.1.2/README.md
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.2/examples/xloader_dexor.py
+-rw-r--r--   0     1000     1000      409 2023-04-29 18:27:50.000000 pyscemu-0.1.2/examples/xloader_keygen.py
+-rw-r--r--   0     1000     1000      369 2023-04-28 16:18:25.000000 pyscemu-0.1.2/pyproject.toml
+-rw-r--r--   0     1000     1000    24020 2023-04-29 18:40:24.000000 pyscemu-0.1.2/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-04-29 21:19:59.000000 pyscemu-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0    10053 1970-01-01 00:00:00.000000 pyscemu-0.1.2/PKG-INFO
```

### Comparing `pyscemu-0.1.1/.github/workflows/CI.yml` & `pyscemu-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.1/.gitignore` & `pyscemu-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.1/README.md` & `pyscemu-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # PYSCEMU
 
 ## Install
+pip install --upgrade pip
+pip3 install --upgrade pip
+curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 pip install pyscemu
 
 
 ## Download maps
 download maps32 from releases or maps64 better from git:
 https://github.com/sha0coder/scemu
```

### Comparing `pyscemu-0.1.1/examples/xloader_dexor.py` & `pyscemu-0.1.2/examples/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.1/src/lib.rs` & `pyscemu-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.1/Cargo.lock` & `pyscemu-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.11.4"
+version = "0.11.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9eb71f9e09266eb4eff5c50550b809b94a77bb7a4a403e4367c393c05e2bd950"
+checksum = "ea355172c86c50676adbf3c9753a409ff4ad0149b60ee5bef3eafcfc9727ce48"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.1.1/PKG-INFO` & `pyscemu-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
 
 ## Install
+pip install --upgrade pip
+pip3 install --upgrade pip
+curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
 pip install pyscemu
 
 
 ## Download maps
 download maps32 from releases or maps64 better from git:
 https://github.com/sha0coder/scemu
```

