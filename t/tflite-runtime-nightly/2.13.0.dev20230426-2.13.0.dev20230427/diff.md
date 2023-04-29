# Comparing `tmp/tflite_runtime_nightly-2.13.0.dev20230426-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/tflite_runtime_nightly-2.13.0.dev20230427-cp39-cp39-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 2385859 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       80 b- defN 23-Apr-27 04:51 tflite_runtime/__init__.py
--rwxrwxr-x  2.0 unx  6781128 b- defN 23-Apr-27 04:53 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
--rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-27 04:51 tflite_runtime/interpreter.py
--rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-27 04:51 tflite_runtime/metrics_interface.py
--rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-27 04:51 tflite_runtime/metrics_portable.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-27 04:53 tflite_runtime_nightly-2.13.0.dev20230426.dist-info/METADATA
--rw-rw-r--  2.0 unx      111 b- defN 23-Apr-27 04:53 tflite_runtime_nightly-2.13.0.dev20230426.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Apr-27 04:53 tflite_runtime_nightly-2.13.0.dev20230426.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      878 b- defN 23-Apr-27 04:53 tflite_runtime_nightly-2.13.0.dev20230426.dist-info/RECORD
-9 files, 6826017 bytes uncompressed, 2384313 bytes compressed:  65.1%
+Zip file size: 2385864 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       80 b- defN 23-Apr-28 04:56 tflite_runtime/__init__.py
+-rwxrwxr-x  2.0 unx  6781128 b- defN 23-Apr-28 04:58 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so
+-rw-rw-r--  2.0 unx    38775 b- defN 23-Apr-28 04:55 tflite_runtime/interpreter.py
+-rw-rw-r--  2.0 unx     1542 b- defN 23-Apr-28 04:55 tflite_runtime/metrics_interface.py
+-rw-rw-r--  2.0 unx     2048 b- defN 23-Apr-28 04:55 tflite_runtime/metrics_portable.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA
+-rw-rw-r--  2.0 unx      111 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      878 b- defN 23-Apr-28 04:58 tflite_runtime_nightly-2.13.0.dev20230427.dist-info/RECORD
+9 files, 6826017 bytes uncompressed, 2384318 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: tflite_runtime/metrics_interface.py
 Comment: 
 
 Filename: tflite_runtime/metrics_portable.py
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230426.dist-info/METADATA
+Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230426.dist-info/WHEEL
+Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/WHEEL
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230426.dist-info/top_level.txt
+Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/top_level.txt
 Comment: 
 
-Filename: tflite_runtime_nightly-2.13.0.dev20230426.dist-info/RECORD
+Filename: tflite_runtime_nightly-2.13.0.dev20230427.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tflite_runtime/__init__.py

```diff
@@ -1,2 +1,2 @@
-__version__ = '2.13.0dev20230426'
-__git_version__ = '0.6.0-147064-g05e524c7c27'
+__version__ = '2.13.0dev20230427'
+__git_version__ = '0.6.0-147137-g24558c4400c'
```

## Comparing `tflite_runtime_nightly-2.13.0.dev20230426.dist-info/METADATA` & `tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tflite-runtime-nightly
-Version: 2.13.0.dev20230426
+Version: 2.13.0.dev20230427
 Summary: TensorFlow Lite is for mobile and embedded devices.
 Home-page: https://www.tensorflow.org/lite/
 Author: Google, LLC
 Author-email: packages@tensorflow.org
 License: Apache 2.0
 Keywords: tflite tensorflow tensor machine learning
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `tflite_runtime_nightly-2.13.0.dev20230426.dist-info/RECORD` & `tflite_runtime_nightly-2.13.0.dev20230427.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tflite_runtime/__init__.py,sha256=yBRTAl6_Fu_awJDp3DdXyN21QAcREbU3Qmduwc8SqzQ,80
+tflite_runtime/__init__.py,sha256=F9_s-fTWE75UG3NhnmjkdTdTWZ1PhwvbW1xDisbO4UQ,80
 tflite_runtime/_pywrap_tensorflow_interpreter_wrapper.so,sha256=cnFV2pm9WN70jW5eZs_ESl3VsxWEMEHA3I_gK-Hkzak,6781128
 tflite_runtime/interpreter.py,sha256=WdMKqxuFdoGPyOKoCsZsHbvsVQXs_81OrG7VUE8p5JU,38775
 tflite_runtime/metrics_interface.py,sha256=dVu6SmbnQUntPgE5o6BxHVMyemwli-7F6tDfVMGrlYI,1542
 tflite_runtime/metrics_portable.py,sha256=YBiMNokP9JtoQaUcCRRY1T_iFSZGeWCjr6L0iUR6eY8,2048
-tflite_runtime_nightly-2.13.0.dev20230426.dist-info/METADATA,sha256=IA29aa0A8o9pLoSrdRrtkA6llrhVo9MaL0azqIeyoO4,1440
-tflite_runtime_nightly-2.13.0.dev20230426.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
-tflite_runtime_nightly-2.13.0.dev20230426.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
-tflite_runtime_nightly-2.13.0.dev20230426.dist-info/RECORD,,
+tflite_runtime_nightly-2.13.0.dev20230427.dist-info/METADATA,sha256=ItXPA-ntqzHTQixLw84DYBgIEVqfErXSDlplacgnPb8,1440
+tflite_runtime_nightly-2.13.0.dev20230427.dist-info/WHEEL,sha256=IoSdNuZzCHbwOfmM81cEV5tUXku8iYpWuW3ThlGJK8I,111
+tflite_runtime_nightly-2.13.0.dev20230427.dist-info/top_level.txt,sha256=uNbSt_JkE5qb43UeqR4Wx6_Y6A5613g6gtS49welF08,15
+tflite_runtime_nightly-2.13.0.dev20230427.dist-info/RECORD,,
```

