# Comparing `tmp/cramjam-2.7.0rc1.tar.gz` & `tmp/cramjam-2.7.0rc2.tar.gz`

## Comparing `cramjam-2.7.0rc1.tar` & `cramjam-2.7.0rc2.tar`

### file list

```diff
@@ -1,50 +1,49 @@
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 cramjam-2.7.0rc1/Cargo.toml
--rw-r--r--   0      501       20      112 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/.cargo/config
--rw-r--r--   0      501       20     7989 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/.github/workflows/CI.yml
--rw-r--r--   0      501       20     1854 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/.gitignore
--rw-r--r--   0      501       20     1070 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/LICENSE
--rw-r--r--   0      501       20      971 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/Makefile
--rw-r--r--   0      501       20     3075 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/README.md
--rw-r--r--   0      501       20      121 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmark-requirements.txt
--rw-r--r--   0      501       20    75826 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/README.md
--rw-r--r--   0      501       20     1167 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/COPYING
--rw-r--r--   0      501       20    14168 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/Mark.Twain-Tom.Sawyer.txt
--rw-r--r--   0      501       20   152089 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/alice29.txt
--rw-r--r--   0      501       20   125179 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/asyoulik.txt
--rw-r--r--   0      501       20   123093 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/fireworks.jpeg
--rw-r--r--   0      501       20   118588 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/geo.protodata
--rw-r--r--   0      501       20   102400 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/html
--rw-r--r--   0      501       20   409600 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/html_x_4
--rw-r--r--   0      501       20   184320 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/kppkn.gtb
--rw-r--r--   0      501       20   426754 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/lcet10.txt
--rw-r--r--   0      501       20   102400 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/paper-100k.pdf
--rw-r--r--   0      501       20   481861 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/plrabn12.txt
--rw-r--r--   0      501       20   702087 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/data/urls.10K
--rw-r--r--   0      501       20     7670 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/benchmarks/test_bench.py
--rw-r--r--   0      501       20       66 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/dev-requirements.txt
--rw-r--r--   0      501       20      422 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/pyproject.toml
--rw-r--r--   0      501       20       15 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/rustfmt.toml
--rw-r--r--   0      501       20     4381 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/brotli.rs
--rw-r--r--   0      501       20     4239 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/bzip2.rs
--rw-r--r--   0      501       20     4323 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/deflate.rs
--rw-r--r--   0      501       20      577 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/exceptions.rs
--rw-r--r--   0      501       20     4875 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/gzip.rs
--rw-r--r--   0      501       20    20839 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/io.rs
--rw-r--r--   0      501       20    18999 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/lib.rs
--rw-r--r--   0      501       20    10417 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/lz4.rs
--rw-r--r--   0      501       20     6754 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/snappy.rs
--rw-r--r--   0      501       20     4179 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/src/zstd.rs
--rw-r--r--   0      501       20        0 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/__init__.py
--rw-r--r--   0      501       20      857 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt
--rw-r--r--   0      501       20      375 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.br
--rw-r--r--   0      501       20      495 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.bz2
--rw-r--r--   0      501       20      472 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.gz
--rw-r--r--   0      501       20      665 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.lz4
--rw-r--r--   0      501       20      660 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.snappy
--rw-r--r--   0      501       20      465 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.zst
--rw-r--r--   0      501       20     1140 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/test_integration.py
--rw-r--r--   0      501       20      692 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/test_no_numpy.py
--rw-r--r--   0      501       20     1481 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/test_rust_io.py
--rw-r--r--   0      501       20    10737 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/tests/test_variants.py
--rw-r--r--   0      501       20    13963 2023-04-26 04:17:25.000000 cramjam-2.7.0rc1/Cargo.lock
--rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 cramjam-2.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 cramjam-2.7.0rc2/Cargo.toml
+-rw-r--r--   0      501       20      112 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/.cargo/config
+-rw-r--r--   0      501       20     7819 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/.github/workflows/CI.yml
+-rw-r--r--   0      501       20     1854 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/.gitignore
+-rw-r--r--   0      501       20     1070 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/LICENSE
+-rw-r--r--   0      501       20      971 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/Makefile
+-rw-r--r--   0      501       20     3075 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/README.md
+-rw-r--r--   0      501       20      121 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/benchmark-requirements.txt
+-rw-r--r--   0      501       20    75826 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/benchmarks/README.md
+-rw-r--r--   0      501       20     1167 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/benchmarks/data/COPYING
+-rw-r--r--   0      501       20    14168 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/Mark.Twain-Tom.Sawyer.txt
+-rw-r--r--   0      501       20   152089 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/alice29.txt
+-rw-r--r--   0      501       20   125179 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/asyoulik.txt
+-rw-r--r--   0      501       20   123093 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/fireworks.jpeg
+-rw-r--r--   0      501       20   118588 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/geo.protodata
+-rw-r--r--   0      501       20   102400 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/html
+-rw-r--r--   0      501       20   409600 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/html_x_4
+-rw-r--r--   0      501       20   184320 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/kppkn.gtb
+-rw-r--r--   0      501       20   426754 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/lcet10.txt
+-rw-r--r--   0      501       20   102400 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/paper-100k.pdf
+-rw-r--r--   0      501       20   481861 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/plrabn12.txt
+-rw-r--r--   0      501       20   702087 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/data/urls.10K
+-rw-r--r--   0      501       20     7670 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/benchmarks/test_bench.py
+-rw-r--r--   0      501       20       66 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/dev-requirements.txt
+-rw-r--r--   0      501       20      422 2023-04-29 05:00:13.000000 cramjam-2.7.0rc2/pyproject.toml
+-rw-r--r--   0      501       20       15 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/rustfmt.toml
+-rw-r--r--   0      501       20     4381 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/brotli.rs
+-rw-r--r--   0      501       20     4239 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/bzip2.rs
+-rw-r--r--   0      501       20     4323 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/deflate.rs
+-rw-r--r--   0      501       20      577 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/exceptions.rs
+-rw-r--r--   0      501       20     4875 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/gzip.rs
+-rw-r--r--   0      501       20    18803 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/io.rs
+-rw-r--r--   0      501       20    17757 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/lib.rs
+-rw-r--r--   0      501       20    10417 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/lz4.rs
+-rw-r--r--   0      501       20     6754 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/snappy.rs
+-rw-r--r--   0      501       20     4179 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/src/zstd.rs
+-rw-r--r--   0      501       20        0 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/__init__.py
+-rw-r--r--   0      501       20      857 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt
+-rw-r--r--   0      501       20      375 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.br
+-rw-r--r--   0      501       20      495 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.bz2
+-rw-r--r--   0      501       20      472 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.gz
+-rw-r--r--   0      501       20      665 2023-04-29 05:00:14.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.lz4
+-rw-r--r--   0      501       20      660 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.snappy
+-rw-r--r--   0      501       20      465 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.zst
+-rw-r--r--   0      501       20     1140 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/test_integration.py
+-rw-r--r--   0      501       20     1481 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/test_rust_io.py
+-rw-r--r--   0      501       20    10785 2023-04-29 05:00:15.000000 cramjam-2.7.0rc2/tests/test_variants.py
+-rw-r--r--   0      501       20    12043 2023-04-29 05:00:12.000000 cramjam-2.7.0rc2/Cargo.lock
+-rw-r--r--   0        0        0     3703 1970-01-01 00:00:00.000000 cramjam-2.7.0rc2/PKG-INFO
```

### Comparing `cramjam-2.7.0rc1/Cargo.toml` & `cramjam-2.7.0rc2/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "cramjam"
-version = "2.7.0-rc1"
+version = "2.7.0-rc2"
 authors = ["Miles Granger <miles59923@gmail.com>"]
 edition = "2018"
 license = "MIT"
 description = "Thin Python bindings to de/compression algorithms in Rust"
 readme = "README.md"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
@@ -24,8 +24,7 @@
 pyo3 = { version = "^0.18", default-features = false, features = ["macros"] }
 snap = "^1"
 brotli = { version = "^3", default-features = false, features = ["std"] }
 bzip2 = "^0.4"
 lz4 = "^1"
 flate2 = "1.0.25"
 zstd = "0.11.1+zstd.1.5.2"
-numpy = "^0.18"
```

### Comparing `cramjam-2.7.0rc1/.github/workflows/CI.yml` & `cramjam-2.7.0rc2/.github/workflows/CI.yml`

 * *Files 6% similar despite different names*

```diff
@@ -118,19 +118,14 @@
         args: -i ${{ matrix.python-version }} --release --out dist
     - name: Python UnitTest
       if: matrix.target == 'x86_64'
       run: |
         pip install cramjam --no-index --find-links dist --force-reinstall
         pip install -r dev-requirements.txt
         make test
-    - name: Test no numpy installed works
-      if: matrix.target == 'x86_64'
-      run: |
-        pip uninstall numpy -y
-        python -m pytest tests/test_no_numpy.py
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   linux-cross:
```

### Comparing `cramjam-2.7.0rc1/.gitignore` & `cramjam-2.7.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/LICENSE` & `cramjam-2.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/Makefile` & `cramjam-2.7.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/README.md` & `cramjam-2.7.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/README.md` & `cramjam-2.7.0rc2/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/COPYING` & `cramjam-2.7.0rc2/benchmarks/data/COPYING`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/Mark.Twain-Tom.Sawyer.txt` & `cramjam-2.7.0rc2/benchmarks/data/Mark.Twain-Tom.Sawyer.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/alice29.txt` & `cramjam-2.7.0rc2/benchmarks/data/alice29.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/asyoulik.txt` & `cramjam-2.7.0rc2/benchmarks/data/asyoulik.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/fireworks.jpeg` & `cramjam-2.7.0rc2/benchmarks/data/fireworks.jpeg`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/geo.protodata` & `cramjam-2.7.0rc2/benchmarks/data/geo.protodata`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/html` & `cramjam-2.7.0rc2/benchmarks/data/html`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/html_x_4` & `cramjam-2.7.0rc2/benchmarks/data/html_x_4`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/kppkn.gtb` & `cramjam-2.7.0rc2/benchmarks/data/kppkn.gtb`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/lcet10.txt` & `cramjam-2.7.0rc2/benchmarks/data/lcet10.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/paper-100k.pdf` & `cramjam-2.7.0rc2/benchmarks/data/paper-100k.pdf`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/plrabn12.txt` & `cramjam-2.7.0rc2/benchmarks/data/plrabn12.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/data/urls.10K` & `cramjam-2.7.0rc2/benchmarks/data/urls.10K`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/benchmarks/test_bench.py` & `cramjam-2.7.0rc2/benchmarks/test_bench.py`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/brotli.rs` & `cramjam-2.7.0rc2/src/brotli.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/bzip2.rs` & `cramjam-2.7.0rc2/src/bzip2.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/deflate.rs` & `cramjam-2.7.0rc2/src/deflate.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/exceptions.rs` & `cramjam-2.7.0rc2/src/exceptions.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/gzip.rs` & `cramjam-2.7.0rc2/src/gzip.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/io.rs` & `cramjam-2.7.0rc2/src/io.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,201 +1,30 @@
 //! Module holds native Rust objects exposed to Python, or objects
 //! which wrap native Python objects to provide additional functionality
 //! or tighter integration with de/compression algorithms.
 //!
+use std::convert::TryFrom;
 use std::fs::{File, OpenOptions};
 use std::io::{copy, Cursor, Read, Seek, SeekFrom, Write};
 use std::os::raw::c_int;
 
 use crate::exceptions::CompressionError;
 use crate::BytesType;
-use numpy::PyArray1;
+use pyo3::buffer::{Element, PyBuffer};
+use pyo3::exceptions::PyBufferError;
 use pyo3::prelude::*;
-use pyo3::types::{PyByteArray, PyBytes};
+use pyo3::types::PyBytes;
 use pyo3::{ffi, AsPyPointer};
 use std::path::PathBuf;
 
 pub(crate) trait AsBytes {
     fn as_bytes(&self) -> &[u8];
     fn as_bytes_mut(&mut self) -> &mut [u8];
 }
 
-/// Internal wrapper for `numpy.array`/`PyArray1`, to provide Read + Write and other traits
-pub struct RustyNumpyArray<'a> {
-    pub(crate) inner: &'a PyArray1<u8>,
-    pub(crate) cursor: Cursor<&'a mut [u8]>,
-}
-impl<'a> AsBytes for RustyNumpyArray<'a> {
-    fn as_bytes(&self) -> &[u8] {
-        self.cursor.get_ref().as_ref()
-    }
-    fn as_bytes_mut(&mut self) -> &mut [u8] {
-        self.cursor.get_mut()
-    }
-}
-impl<'a> RustyNumpyArray<'a> {
-    pub(crate) fn as_bytes(&self) -> &[u8] {
-        unsafe { self.inner.as_slice().unwrap() }
-    }
-}
-impl<'a> From<&'a PyArray1<u8>> for RustyNumpyArray<'a> {
-    fn from(inner: &'a PyArray1<u8>) -> Self {
-        Self {
-            inner,
-            cursor: Cursor::new(unsafe { inner.as_slice_mut().unwrap() }),
-        }
-    }
-}
-impl<'a> FromPyObject<'a> for RustyNumpyArray<'a> {
-    fn extract(ob: &'a PyAny) -> PyResult<Self> {
-        let pybytes: &PyArray1<u8> = ob.extract()?;
-        Ok(Self::from(pybytes))
-    }
-}
-impl<'a> ToPyObject for RustyNumpyArray<'a> {
-    fn to_object(&self, py: Python<'_>) -> PyObject {
-        self.inner.to_object(py)
-    }
-}
-impl<'a> Write for RustyNumpyArray<'a> {
-    fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
-        self.cursor.write(buf)
-    }
-    fn flush(&mut self) -> std::io::Result<()> {
-        self.cursor.flush()
-    }
-}
-impl<'a> Read for RustyNumpyArray<'a> {
-    fn read(&mut self, buf: &mut [u8]) -> std::io::Result<usize> {
-        self.cursor.read(buf)
-    }
-}
-
-impl<'a> Seek for RustyNumpyArray<'a> {
-    fn seek(&mut self, pos: SeekFrom) -> std::io::Result<u64> {
-        self.cursor.seek(pos)
-    }
-}
-
-/// Internal wrapper for `bytes`/`PyBytes`, to provide Read + Write and other traits
-pub struct RustyPyBytes<'a> {
-    pub(crate) inner: &'a PyBytes,
-    pub(crate) cursor: Cursor<&'a mut [u8]>,
-}
-impl<'a> AsBytes for RustyPyBytes<'a> {
-    fn as_bytes(&self) -> &[u8] {
-        self.inner.as_bytes()
-    }
-    fn as_bytes_mut(&mut self) -> &mut [u8] {
-        self.cursor.get_mut()
-    }
-}
-impl<'a> From<&'a PyBytes> for RustyPyBytes<'a> {
-    fn from(inner: &'a PyBytes) -> Self {
-        let ptr = inner.as_bytes().as_ptr();
-        Self {
-            inner,
-            cursor: Cursor::new(unsafe { std::slice::from_raw_parts_mut(ptr as *mut _, inner.as_bytes().len()) }),
-        }
-    }
-}
-impl<'a> FromPyObject<'a> for RustyPyBytes<'a> {
-    fn extract(ob: &'a PyAny) -> PyResult<Self> {
-        let pybytes: &PyBytes = ob.extract()?;
-        Ok(Self::from(pybytes))
-    }
-}
-impl<'a> ToPyObject for RustyPyBytes<'a> {
-    fn to_object(&self, py: Python<'_>) -> PyObject {
-        self.inner.to_object(py)
-    }
-}
-impl<'a> Read for RustyPyBytes<'a> {
-    fn read(&mut self, buf: &mut [u8]) -> std::io::Result<usize> {
-        self.cursor.read(buf)
-    }
-}
-impl<'a> Write for RustyPyBytes<'a> {
-    fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
-        self.cursor.write(buf)
-    }
-    fn flush(&mut self) -> std::io::Result<()> {
-        self.cursor.flush()
-    }
-}
-impl<'a> Seek for RustyPyBytes<'a> {
-    fn seek(&mut self, style: SeekFrom) -> std::io::Result<u64> {
-        self.cursor.seek(style)
-    }
-}
-
-/// Internal wrapper for `bytearray`/`PyByteArray`, to provide Read + Write and other traits
-pub struct RustyPyByteArray<'a> {
-    pub(crate) inner: &'a PyByteArray,
-    pub(crate) cursor: Cursor<&'a mut [u8]>,
-}
-impl<'a> AsBytes for RustyPyByteArray<'a> {
-    fn as_bytes(&self) -> &[u8] {
-        self.cursor.get_ref()
-    }
-    fn as_bytes_mut(&mut self) -> &mut [u8] {
-        self.cursor.get_mut()
-    }
-}
-impl<'a> From<&'a PyByteArray> for RustyPyByteArray<'a> {
-    fn from(inner: &'a PyByteArray) -> Self {
-        Self {
-            inner,
-            cursor: Cursor::new(unsafe { inner.as_bytes_mut() }),
-        }
-    }
-}
-impl<'a> FromPyObject<'a> for RustyPyByteArray<'a> {
-    fn extract(ob: &'a PyAny) -> PyResult<Self> {
-        let pybytes: &PyByteArray = ob.extract()?;
-        Ok(Self::from(pybytes))
-    }
-}
-impl<'a> ToPyObject for RustyPyByteArray<'a> {
-    fn to_object(&self, py: Python<'_>) -> PyObject {
-        self.inner.to_object(py)
-    }
-}
-impl<'a> Write for RustyPyByteArray<'a> {
-    fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
-        if (self.cursor.position() as usize + buf.len()) > self.inner.len() {
-            let previous_pos = self.cursor.position();
-            self.inner.resize(self.cursor.position() as usize + buf.len()).unwrap();
-            self.cursor = Cursor::new(unsafe { self.inner.as_bytes_mut() });
-            self.cursor.set_position(previous_pos);
-        }
-        self.cursor.write(buf)
-    }
-    fn flush(&mut self) -> std::io::Result<()> {
-        if self.inner.len() != self.cursor.position() as usize {
-            let prev_pos = self.cursor.position();
-            self.inner.resize(self.cursor.position() as usize).unwrap();
-            self.cursor = Cursor::new(unsafe { self.inner.as_bytes_mut() });
-            self.cursor.set_position(prev_pos);
-        }
-        Ok(())
-    }
-}
-impl<'a> Read for RustyPyByteArray<'a> {
-    fn read(&mut self, buf: &mut [u8]) -> std::io::Result<usize> {
-        self.cursor.read(buf)
-    }
-}
-
-impl<'a> Seek for RustyPyByteArray<'a> {
-    fn seek(&mut self, pos: SeekFrom) -> std::io::Result<u64> {
-        self.cursor.seek(pos)
-    }
-}
-
 /// A native Rust file-like object. Reading and writing takes place
 /// through the Rust implementation, allowing access to the underlying
 /// bytes in Python.
 ///
 /// ### Python Example
 /// ```python
 /// from cramjam import File
@@ -323,25 +152,116 @@
     }
 
     fn __repr__(&self) -> PyResult<String> {
         let path = match self.path.as_path().to_str() {
             Some(path) => path.to_string(),
             None => self.path.to_string_lossy().to_string(),
         };
-        let repr = format!("cramjam.File(path={}, len={:?})", path, self.len()?);
+        let repr = format!("cramjam.File<path={}, len={:?}>", path, self.len()?);
         Ok(repr)
     }
     fn __bool__(&self) -> PyResult<bool> {
         Ok(self.len()? > 0)
     }
     fn __len__(&self) -> PyResult<usize> {
         self.len()
     }
 }
 
+/// Internal wrapper to PyBuffer, not exposed thru API
+/// used only for impl of Read/Write
+pub struct PythonBuffer<T: Element> {
+    pub(crate) inner: PyBuffer<T>,
+    pub(crate) pos: usize,
+}
+impl<T: Element> PythonBuffer<T> {
+    /// Reset the read/write position of cursor
+    pub fn reset_position(&mut self) {
+        self.pos = 0;
+    }
+    /// Explicitly set the position of the cursor
+    pub fn set_position(&mut self, pos: usize) {
+        self.pos = pos;
+    }
+    /// Get the current position of the cursor
+    pub fn position(&self) -> usize {
+        self.pos
+    }
+    /// Is the Python buffer readonly
+    pub fn readonly(&self) -> bool {
+        self.inner.readonly()
+    }
+    /// Get the underlying buffer as a slice of bytes
+    pub fn as_slice(&self) -> &[u8] {
+        unsafe { std::slice::from_raw_parts(self.inner.buf_ptr() as *const u8, self.inner.len_bytes()) }
+    }
+    /// Get the underlying buffer as a mutable slice of bytes
+    pub fn as_slice_mut(&mut self) -> PyResult<&mut [u8]> {
+        // TODO: For v3 release, add self.readonly check; bytes is readonly but
+        // v1 and v2 releases have not treated it as such.
+        Ok(unsafe { std::slice::from_raw_parts_mut(self.inner.buf_ptr() as *mut u8, self.inner.len_bytes()) })
+    }
+}
+
+impl<'py, T: Element> FromPyObject<'py> for PythonBuffer<T> {
+    fn extract(obj: &'py PyAny) -> PyResult<Self> {
+        let buf = PyBuffer::get(obj)?;
+        PythonBuffer::try_from(buf)
+    }
+}
+
+impl<T: Element> TryFrom<PyBuffer<T>> for PythonBuffer<T> {
+    type Error = PyErr;
+    fn try_from(buf: PyBuffer<T>) -> Result<Self, Self::Error> {
+        if !buf.is_c_contiguous() {
+            Err(PyBufferError::new_err("Buffer is not C contiguous"))
+        } else if buf.dimensions() != 1 {
+            Err(PyBufferError::new_err("Buffer is not 1 dimensional"))
+        } else {
+            Ok(Self { inner: buf, pos: 0 })
+        }
+    }
+}
+
+impl<T: Element> Read for PythonBuffer<T> {
+    fn read(&mut self, buf: &mut [u8]) -> std::io::Result<usize> {
+        let slice = self.as_slice();
+        if self.pos < slice.len() {
+            let nbytes = (&slice[self.pos..]).read(buf)?;
+            self.pos += nbytes;
+            Ok(nbytes)
+        } else {
+            Ok(0)
+        }
+    }
+}
+
+impl<T: Element> Write for PythonBuffer<T> {
+    fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
+        let pos = self.position();
+        let slice = self
+            .as_slice_mut()
+            .map_err(|e| std::io::Error::new(std::io::ErrorKind::Other, e.to_string()))?;
+        let len = slice.len();
+
+        if pos < slice.len() {
+            let nbytes = std::cmp::min(len - pos, buf.len());
+            slice[pos..pos + nbytes].copy_from_slice(&buf[..nbytes]);
+            self.pos += nbytes;
+            Ok(nbytes)
+        } else {
+            Ok(0)
+        }
+    }
+
+    fn flush(&mut self) -> std::io::Result<()> {
+        Ok(())
+    }
+}
+
 /// A native Rust file-like object. Reading and writing takes place
 /// through the Rust implementation, allowing access to the underlying
 /// bytes in Python.
 ///
 /// ### Python Example
 /// ```python
 /// >>> from cramjam import Buffer
@@ -458,15 +378,15 @@
         self.len()
     }
     fn __contains__(&self, py: Python, x: BytesType) -> bool {
         let bytes = x.as_bytes();
         py.allow_threads(|| self.inner.get_ref().windows(bytes.len()).any(|w| w == bytes))
     }
     fn __repr__(&self) -> String {
-        format!("cramjam.Buffer(len={:?})", self.len())
+        format!("cramjam.Buffer<len={:?}>", self.len())
     }
     fn __bool__(&self) -> bool {
         self.len() > 0
     }
     unsafe fn __getbuffer__(slf: PyRefMut<Self>, view: *mut ffi::Py_buffer, flags: c_int) -> PyResult<()> {
         if view.is_null() {
             return Err(pyo3::exceptions::PyBufferError::new_err("View is null"));
@@ -479,15 +399,15 @@
         (*view).obj = slf.as_ptr();
         ffi::Py_INCREF((*view).obj);
 
         let bytes = slf.inner.get_ref().as_slice();
 
         (*view).buf = bytes.as_ptr() as *mut std::os::raw::c_void;
         (*view).len = bytes.len() as isize;
-        (*view).readonly = 1;
+        (*view).readonly = 0;
         (*view).itemsize = 1;
 
         (*view).format = std::ptr::null_mut();
         if (flags & ffi::PyBUF_FORMAT) == ffi::PyBUF_FORMAT {
             let msg = std::ffi::CStr::from_bytes_with_nul(b"B\0").unwrap();
             (*view).format = msg.as_ptr() as *mut _;
         }
@@ -508,22 +428,17 @@
         Ok(())
     }
     unsafe fn __releasebuffer__(&self, _view: *mut ffi::Py_buffer) {}
 }
 
 fn write<W: Write>(input: &mut BytesType, output: &mut W) -> std::io::Result<u64> {
     let result = match input {
+        BytesType::RustyBuffer(buf) => copy(&mut buf.borrow_mut().inner, output)?,
         BytesType::RustyFile(data) => copy(&mut data.borrow_mut().inner, output)?,
-        BytesType::RustyBuffer(data) => copy(&mut data.borrow_mut().inner, output)?,
-        BytesType::ByteArray(data) => copy(data, output)?,
-        BytesType::NumpyArray(array) => copy(array, output)?,
-        BytesType::Bytes(data) => {
-            let buffer = data.as_bytes();
-            copy(&mut Cursor::new(buffer), output)?
-        }
+        BytesType::PyBuffer(buf) => copy(buf, output)?,
     };
     Ok(result)
 }
 
 fn read<'a, R: Read>(reader: &mut R, py: Python<'a>, n_bytes: Option<usize>) -> PyResult<&'a PyBytes> {
     match n_bytes {
         Some(n) => PyBytes::new_with(py, n, |buf| {
@@ -544,14 +459,26 @@
     }
 }
 impl Seek for RustyFile {
     fn seek(&mut self, pos: SeekFrom) -> std::io::Result<u64> {
         self.inner.seek(pos)
     }
 }
+impl<T: Element> Seek for PythonBuffer<T> {
+    fn seek(&mut self, pos: SeekFrom) -> std::io::Result<u64> {
+        let len = self.inner.len_bytes();
+        let current = self.position();
+        match pos {
+            SeekFrom::Start(n) => self.set_position(n as usize),
+            SeekFrom::End(n) => self.set_position((len as i64 - n) as usize),
+            SeekFrom::Current(n) => self.set_position((current as i64 + n) as usize),
+        }
+        Ok(self.position() as _)
+    }
+}
 impl Write for RustyBuffer {
     fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
         self.inner.write(buf)
     }
     fn flush(&mut self) -> std::io::Result<()> {
         self.inner.flush()
     }
```

### Comparing `cramjam-2.7.0rc1/src/lib.rs` & `cramjam-2.7.0rc2/src/lib.rs`

 * *Files 10% similar despite different names*

```diff
@@ -57,139 +57,112 @@
 pub mod exceptions;
 pub mod gzip;
 pub mod io;
 pub mod lz4;
 pub mod snappy;
 pub mod zstd;
 
+use io::{PythonBuffer, RustyBuffer};
 use pyo3::prelude::*;
 
-use crate::io::{AsBytes, RustyBuffer, RustyFile, RustyNumpyArray, RustyPyByteArray, RustyPyBytes};
+use crate::io::{AsBytes, RustyFile};
 use exceptions::{CompressionError, DecompressionError};
 use std::io::{Read, Seek, SeekFrom, Write};
 
 /// Any possible input/output to de/compression algorithms.
 /// Typically, as a Python user, you never have to worry about this object. It's exposed here in
 /// the documentation to see what types are acceptable for de/compression functions.
 #[derive(FromPyObject)]
 pub enum BytesType<'a> {
-    /// `bytes`
-    #[pyo3(transparent, annotation = "bytes")]
-    Bytes(RustyPyBytes<'a>),
-    /// `bytearray`
-    #[pyo3(transparent, annotation = "bytearray")]
-    ByteArray(RustyPyByteArray<'a>),
-    /// [`cramjam.File`](io/struct.RustyFile.html)
-    #[pyo3(transparent, annotation = "File")]
-    RustyFile(&'a PyCell<RustyFile>),
     /// [`cramjam.Buffer`](io/struct.RustyBuffer.html)
     #[pyo3(transparent, annotation = "Buffer")]
     RustyBuffer(&'a PyCell<RustyBuffer>),
-    /// `numpy.array` with `dtype=np.uint8`
-    #[pyo3(transparent, annotation = "numpy")]
-    NumpyArray(RustyNumpyArray<'a>),
+    /// [`cramjam.File`](io/struct.RustyFile.html)
+    #[pyo3(transparent, annotation = "File")]
+    RustyFile(&'a PyCell<RustyFile>),
+    /// `object` implementing the Buffer Protocol
+    #[pyo3(transparent, annotation = "pybuffer")]
+    PyBuffer(PythonBuffer<u8>),
 }
 
 impl<'a> AsBytes for BytesType<'a> {
     fn as_bytes(&self) -> &[u8] {
         match self {
-            BytesType::Bytes(b) => b.as_bytes(),
-            BytesType::ByteArray(b) => b.as_bytes(),
-            BytesType::NumpyArray(b) => b.as_bytes(),
             BytesType::RustyBuffer(b) => {
                 let py_ref = b.borrow();
                 let bytes = py_ref.as_bytes();
                 unsafe { std::slice::from_raw_parts(bytes.as_ptr(), bytes.len()) }
             }
+            BytesType::PyBuffer(b) => b.as_slice(),
             BytesType::RustyFile(b) => {
                 let py_ref = b.borrow();
                 let bytes = py_ref.as_bytes();
                 unsafe { std::slice::from_raw_parts(bytes.as_ptr(), bytes.len()) }
             }
         }
     }
     fn as_bytes_mut(&mut self) -> &mut [u8] {
         match self {
-            BytesType::Bytes(b) => b.as_bytes_mut(),
-            BytesType::ByteArray(b) => b.as_bytes_mut(),
-            BytesType::NumpyArray(b) => b.as_bytes_mut(),
             BytesType::RustyBuffer(b) => {
                 let mut py_ref = b.borrow_mut();
                 let bytes = py_ref.as_bytes_mut();
                 unsafe { std::slice::from_raw_parts_mut(bytes.as_mut_ptr(), bytes.len()) }
             }
+            BytesType::PyBuffer(b) => b.as_slice_mut().unwrap(),
             BytesType::RustyFile(b) => {
                 let mut py_ref = b.borrow_mut();
                 let bytes = py_ref.as_bytes_mut();
                 unsafe { std::slice::from_raw_parts_mut(bytes.as_mut_ptr(), bytes.len()) }
             }
         }
     }
 }
 
 impl<'a> Write for BytesType<'a> {
     fn write(&mut self, buf: &[u8]) -> std::io::Result<usize> {
         let result = match self {
-            BytesType::RustyFile(out) => out.borrow_mut().inner.write(buf)?,
             BytesType::RustyBuffer(out) => out.borrow_mut().inner.write(buf)?,
-            BytesType::ByteArray(out) => out.write(buf)?,
-            BytesType::NumpyArray(out) => out.write(buf)?,
-            BytesType::Bytes(out) => out.write(buf)?,
+            BytesType::RustyFile(out) => out.borrow_mut().inner.write(buf)?,
+            BytesType::PyBuffer(out) => out.write(buf)?,
         };
         Ok(result)
     }
     fn flush(&mut self) -> std::io::Result<()> {
         match self {
-            BytesType::RustyFile(f) => f.borrow_mut().flush(),
             BytesType::RustyBuffer(b) => b.borrow_mut().flush(),
-            BytesType::ByteArray(_) | BytesType::Bytes(_) | BytesType::NumpyArray(_) => Ok(()),
+            BytesType::RustyFile(f) => f.borrow_mut().flush(),
+            BytesType::PyBuffer(_) => Ok(()),
         }
     }
 }
 impl<'a> Read for BytesType<'a> {
     fn read(&mut self, buf: &mut [u8]) -> std::io::Result<usize> {
         match self {
-            BytesType::RustyFile(data) => data.borrow_mut().inner.read(buf),
             BytesType::RustyBuffer(data) => data.borrow_mut().inner.read(buf),
-            BytesType::ByteArray(data) => data.read(buf),
-            BytesType::NumpyArray(array) => array.read(buf),
-            BytesType::Bytes(data) => data.read(buf),
+            BytesType::RustyFile(data) => data.borrow_mut().inner.read(buf),
+            BytesType::PyBuffer(data) => data.read(buf),
         }
     }
 }
 impl<'a> Seek for BytesType<'a> {
     fn seek(&mut self, style: SeekFrom) -> std::io::Result<u64> {
         match self {
-            BytesType::RustyFile(f) => f.borrow_mut().inner.seek(style),
             BytesType::RustyBuffer(b) => b.borrow_mut().inner.seek(style),
-            BytesType::ByteArray(a) => a.seek(style),
-            BytesType::NumpyArray(a) => a.seek(style),
-            BytesType::Bytes(b) => b.seek(style),
+            BytesType::RustyFile(f) => f.borrow_mut().inner.seek(style),
+            BytesType::PyBuffer(buf) => buf.seek(style),
         }
     }
 }
 
 impl<'a> BytesType<'a> {
     fn len(&self) -> usize {
         self.as_bytes().len()
     }
 }
 
-impl<'a> IntoPy<PyObject> for BytesType<'a> {
-    fn into_py(self, py: Python) -> PyObject {
-        match self {
-            Self::Bytes(bytes) => bytes.inner.into(),
-            Self::ByteArray(byte_array) => byte_array.inner.into(),
-            Self::RustyFile(file) => file.to_object(py),
-            Self::RustyBuffer(buffer) => buffer.into_py(py),
-            Self::NumpyArray(array) => array.to_object(py),
-        }
-    }
-}
-
 /// Macro for generating the implementation of de/compression against a variant interface
 #[macro_export]
 macro_rules! generic {
     // de/compress
     ($py:ident, $op:path[$input:expr], output_len=$output_len:ident $(, level=$level:ident)?) => {
         {
             use crate::io::RustyBuffer;
@@ -232,15 +205,15 @@
                         },
                         BytesType::RustyBuffer(buffer) => {
                             let mut borrowed = buffer.borrow_mut();
                             let mut buf_out = &mut borrowed.inner;
                             $py.allow_threads(|| {
                                 $op(f_in, &mut buf_out $(, $level)? )
                             })
-                        }
+                        },
                         _ => {
                             let bytes_out = $output.as_bytes_mut();
                             $py.allow_threads(|| {
                                 $op(f_in, &mut Cursor::new(bytes_out) $(, $level)? )
                             })
                         }
                     }
```

### Comparing `cramjam-2.7.0rc1/src/lz4.rs` & `cramjam-2.7.0rc2/src/lz4.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/snappy.rs` & `cramjam-2.7.0rc2/src/snappy.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/src/zstd.rs` & `cramjam-2.7.0rc2/src/zstd.rs`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/tests/data/integration/plaintext.txt` & `cramjam-2.7.0rc2/tests/data/integration/plaintext.txt`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.lz4` & `cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.lz4`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/tests/data/integration/plaintext.txt.snappy` & `cramjam-2.7.0rc2/tests/data/integration/plaintext.txt.snappy`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/tests/test_integration.py` & `cramjam-2.7.0rc2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/tests/test_rust_io.py` & `cramjam-2.7.0rc2/tests/test_rust_io.py`

 * *Files identical despite different names*

### Comparing `cramjam-2.7.0rc1/tests/test_variants.py` & `cramjam-2.7.0rc2/tests/test_variants.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,18 @@
 def test_variants_raise_exception(variant_str):
     variant = getattr(cramjam, variant_str)
     with pytest.raises(cramjam.DecompressionError):
         variant.decompress(b"sknow")
 
 
 @pytest.mark.parametrize(
-    "input_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File)
+    "input_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File, memoryview)
 )
 @pytest.mark.parametrize(
-    "output_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File)
+    "output_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File, memoryview)
 )
 @pytest.mark.parametrize("variant_str", VARIANTS)
 @given(raw_data=st.binary())
 def test_variants_compress_into(
     variant_str, input_type, output_type, raw_data, tmp_path_factory
 ):
     variant = getattr(cramjam, variant_str)
@@ -109,18 +109,18 @@
         output = output.tobytes()
     else:
         output = bytes(output)
     assert same_same(output, compressed)
 
 
 @pytest.mark.parametrize(
-    "input_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File)
+    "input_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File, memoryview)
 )
 @pytest.mark.parametrize(
-    "output_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File)
+    "output_type", (bytes, bytearray, "numpy", cramjam.Buffer, cramjam.File, memoryview)
 )
 @pytest.mark.parametrize("variant_str", VARIANTS)
 @given(raw_data=st.binary())
 def test_variants_decompress_into(
     variant_str, input_type, output_type, tmp_path_factory, raw_data
 ):
     variant = getattr(cramjam, variant_str)
```

### Comparing `cramjam-2.7.0rc1/Cargo.lock` & `cramjam-2.7.0rc2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -90,21 +90,20 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "cramjam"
-version = "2.7.0-rc1"
+version = "2.7.0-rc2"
 dependencies = [
  "brotli",
  "bzip2",
  "flate2",
  "lz4",
- "numpy",
  "pyo3",
  "snap",
  "zstd",
 ]
 
 [[package]]
 name = "crc32fast"
@@ -173,23 +172,14 @@
 checksum = "57d27b317e207b10f69f5e75494119e391a96f48861ae870d1da6edac98ca900"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
-name = "matrixmultiply"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
-dependencies = [
- "rawpointer",
-]
-
-[[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
@@ -200,70 +190,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
 
 [[package]]
-name = "ndarray"
-version = "0.15.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
-dependencies = [
- "matrixmultiply",
- "num-complex",
- "num-integer",
- "num-traits",
- "rawpointer",
-]
-
-[[package]]
-name = "num-complex"
-version = "0.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
-name = "num-traits"
-version = "0.2.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
-dependencies = [
- "autocfg",
-]
-
-[[package]]
-name = "numpy"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96b0fee4571867d318651c24f4a570c3f18408cf95f16ccb576b3ce85496a46e"
-dependencies = [
- "libc",
- "ndarray",
- "num-complex",
- "num-integer",
- "num-traits",
- "pyo3",
- "rustc-hash",
-]
-
-[[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
@@ -369,35 +303,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
-name = "rawpointer"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
-
-[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
-name = "rustc-hash"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
-
-[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "smallvec"
```

### Comparing `cramjam-2.7.0rc1/PKG-INFO` & `cramjam-2.7.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: cramjam
-Version: 2.7.0rc1
+Version: 2.7.0rc2
 License-File: LICENSE
 Summary: Thin Python bindings to de/compression algorithms in Rust
 Keywords: compression,decompression,snappy,zstd,bz2,gzip,lz4,brotli,deflate
 Author: Miles Granger <miles59923@gmail.com>
 Author-email: Miles Granger <miles59923@gmail.com>
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/milesgranger/pyrus-cramjam
 Project-URL: documentation, https://docs.rs/cramjam/latest/cramjam
 Project-URL: repository, https://github.com/milesgranger/pyrus-cramjam
-Project-URL: homepage, https://github.com/milesgranger/pyrus-cramjam
 
 # pyrus-cramjam
 
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
 [![CI](https://github.com/milesgranger/pyrus-cramjam/workflows/CI/badge.svg?branch=master)](https://github.com/milesgranger/pyrus-cramjam/actions?query=branch=master)
 [![PyPI](https://img.shields.io/pypi/v/cramjam.svg)](https://pypi.org/project/cramjam)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/cramjam/badges/version.svg)](https://anaconda.org/conda-forge/cramjam)
```

