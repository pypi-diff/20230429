# Comparing `tmp/uedge-8.0.0.1.tar.gz` & `tmp/uedge-8.0.0.dev0-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uedge-8.0.0.1.tar", last modified: Sat Apr  1 05:49:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

