# Comparing `tmp/toolcli-0.6.8.tar.gz` & `tmp/toolcli-0.6.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolcli-0.6.8.tar", last modified: Wed Sep 21 02:33:39 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

