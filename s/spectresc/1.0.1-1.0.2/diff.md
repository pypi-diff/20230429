# Comparing `tmp/spectresc-1.0.1.tar.gz` & `tmp/spectresc-1.0.2-cp36-cp36m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectresc-1.0.1.tar", last modified: Wed Apr 26 00:48:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

