# Comparing `tmp/carter-py-0.1.3.tar.gz` & `tmp/carter_py-0.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carter-py-0.1.3.tar", last modified: Wed Apr 19 23:07:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

