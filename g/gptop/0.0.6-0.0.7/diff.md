# Comparing `tmp/gptop-0.0.6.tar.gz` & `tmp/gptop-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptop-0.0.6.tar", last modified: Mon Apr 24 03:49:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

