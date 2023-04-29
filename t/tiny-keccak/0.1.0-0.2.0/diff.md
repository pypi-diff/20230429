# Comparing `tmp/tiny_keccak-0.1.0.tar.gz` & `tmp/tiny_keccak-0.2.0.tar.gz`

## Comparing `tiny_keccak-0.1.0.tar` & `tiny_keccak-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 tiny_keccak-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2776 2023-04-29 17:54:23.000000 tiny_keccak-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-29 17:54:23.000000 tiny_keccak-0.1.0/.gitignore
--rw-r--r--   0     1001      123     1071 2023-04-29 17:54:23.000000 tiny_keccak-0.1.0/LICENSE
--rw-r--r--   0     1001      123      373 2023-04-29 17:54:23.000000 tiny_keccak-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123      623 2023-04-29 17:54:23.000000 tiny_keccak-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     8091 2023-04-29 17:54:23.000000 tiny_keccak-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      282 1970-01-01 00:00:00.000000 tiny_keccak-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 tiny_keccak-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2768 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/.gitignore
+-rw-r--r--   0     1001      123     1071 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      146 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/README.md
+-rw-r--r--   0     1001      123      687 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123      652 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     8091 2023-04-29 19:35:37.000000 tiny_keccak-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 tiny_keccak-0.2.0/PKG-INFO
```

### Comparing `tiny_keccak-0.1.0/.github/workflows/CI.yml` & `tiny_keccak-0.2.0/.github/workflows/CI.yml`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 #    maturin generate-ci github
 #
 name: CI
 
 on:
   push:
     branches:
-      - main
       - master
     tags:
       - '*'
   pull_request:
   workflow_dispatch:
 
 permissions:
@@ -103,18 +102,19 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     if: "startsWith(github.ref, 'refs/tags/')"
     needs: [linux, windows, macos, sdist]
+    environment:
+      name: pypi
+      url: https://pypi.org/p/tiny-keccak
+    permissions:
+      id-token: write
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
+          path: dist
       - name: Publish to PyPI
-        uses: PyO3/maturin-action@v1
-        env:
-          MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
-        with:
-          command: upload
-          args: --skip-existing *
+        uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `tiny_keccak-0.1.0/.gitignore` & `tiny_keccak-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tiny_keccak-0.1.0/LICENSE` & `tiny_keccak-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_keccak-0.1.0/src/lib.rs` & `tiny_keccak-0.2.0/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 use pyo3::{prelude::*, types::PyBytes};
 use tiny_keccak::{Hasher, Keccak};
 
-/// The Keccak hash functions defined in Keccak SHA3 submission
+/// The Keccak-256 hash function defined in Keccak SHA3 submission
 #[pyfunction]
 fn keccak256<'a>(py: Python<'a>, input: &[u8]) -> PyResult<&'a PyBytes> {
     let mut hasher = Keccak::v256();
     hasher.update(input);
     PyBytes::new_with(py, 32, |mut output: &mut [u8]| {
         hasher.finalize(&mut output);
         Ok(())
     })
 }
 
-/// A Python module implemented in Rust.
+/// The Keccak-256 hash function defined in Keccak SHA3 submission
 #[pymodule]
 #[pyo3(name = "tiny_keccak")]
 fn tiny_keccak_py(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(keccak256, m)?)?;
     Ok(())
 }
```

### Comparing `tiny_keccak-0.1.0/Cargo.lock` & `tiny_keccak-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
 name = "tiny-keccak-py"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "unicode-ident"
```

