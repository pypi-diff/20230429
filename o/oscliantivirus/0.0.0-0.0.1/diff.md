# Comparing `tmp/oscliantivirus-0.0.0.tar.gz` & `tmp/oscliantivirus-0.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\oscliantivirus-0.0.0.tar", last modified: Sat Apr 29 13:17:26 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

