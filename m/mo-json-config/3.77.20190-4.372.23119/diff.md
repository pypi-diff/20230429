# Comparing `tmp/mo-json-config-3.77.20190.tar.gz` & `tmp/mo_json_config-4.372.23119-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mo-json-config-3.77.20190.tar", last modified: Wed Jul  8 11:17:06 2020, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

