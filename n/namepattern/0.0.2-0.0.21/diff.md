# Comparing `tmp/namepattern-0.0.2.tar.gz` & `tmp/namepattern-0.0.21-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "namepattern-0.0.2.tar", last modified: Sat Apr 29 19:05:55 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

