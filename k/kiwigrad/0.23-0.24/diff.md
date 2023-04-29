# Comparing `tmp/kiwigrad-0.23.tar.gz` & `tmp/kiwigrad-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.23.tar", last modified: Fri Apr 28 11:52:17 2023, max compression
+gzip compressed data, was "kiwigrad-0.24.tar", last modified: Sat Apr 29 14:38:56 2023, max compression
```

## Comparing `kiwigrad-0.23.tar` & `kiwigrad-0.24.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-28 11:52:17.816152 kiwigrad-0.23/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.23/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.23/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2069 2023-04-28 11:52:17.815678 kiwigrad-0.23/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1593 2023-04-27 21:38:59.000000 kiwigrad-0.23/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-28 11:52:17.812422 kiwigrad-0.23/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      253 2023-04-28 10:50:39.000000 kiwigrad-0.23/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9929 2023-04-28 11:51:54.000000 kiwigrad-0.23/kiwigrad/engine.c
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.23/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.23/kiwigrad/layers.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.23/kiwigrad/neurons.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.23/kiwigrad/nn.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.23/kiwigrad/skeleton.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-28 11:52:17.814322 kiwigrad-0.23/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2069 2023-04-28 11:52:17.000000 kiwigrad-0.23/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      312 2023-04-28 11:52:17.000000 kiwigrad-0.23/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-28 11:52:17.000000 kiwigrad-0.23/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-28 11:52:17.000000 kiwigrad-0.23/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-28 11:52:17.816328 kiwigrad-0.23/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-04-28 10:50:35.000000 kiwigrad-0.23/setup.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-28 11:52:17.814874 kiwigrad-0.23/test/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      618 2023-04-27 14:12:42.000000 kiwigrad-0.23/test/test.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.063179 kiwigrad-0.24/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.24/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.24/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2148 2023-04-29 14:38:56.062742 kiwigrad-0.24/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1672 2023-04-28 23:23:14.000000 kiwigrad-0.24/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.060564 kiwigrad-0.24/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      253 2023-04-29 00:16:46.000000 kiwigrad-0.24/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9999 2023-04-29 14:37:23.000000 kiwigrad-0.24/kiwigrad/engine.c
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.24/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1235 2023-04-27 13:43:11.000000 kiwigrad-0.24/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3246 2023-04-27 13:42:56.000000 kiwigrad-0.24/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1566 2023-04-27 13:42:45.000000 kiwigrad-0.24/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.24/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.061845 kiwigrad-0.24/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     2148 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      312 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-29 14:38:55.000000 kiwigrad-0.24/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-29 14:38:56.063274 kiwigrad-0.24/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      942 2023-04-29 00:16:42.000000 kiwigrad-0.24/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-29 14:38:56.062155 kiwigrad-0.24/test/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      618 2023-04-27 14:12:42.000000 kiwigrad-0.24/test/test.py
```

### Comparing `kiwigrad-0.23/LICENSE` & `kiwigrad-0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.23/PKG-INFO` & `kiwigrad-0.24/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.23
+Version: 0.24
 Summary: Mini deep learning framework
 Home-page: https://github.com/marcosalvalaggio/kiwigrad
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,20 @@
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
+- [Kiwigrad](#kiwigrad)
+  - [Install](#install)
+  - [Kiwigrad Library](#kiwigrad-library)
+    - [Examples](#examples)
+  - [TODOS](#todos)
+
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
 ```console
@@ -59,9 +65,9 @@
 
 model = PotNet()
 ```
 
 ## TODOS
 
 * Include the activation functions tanh in the Value object.
-* Add a notebook example for training a neural network on a regression problem.
+* Fix pow function.
```

### Comparing `kiwigrad-0.23/README.md` & `kiwigrad-0.24/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
+- [Kiwigrad](#kiwigrad)
+  - [Install](#install)
+  - [Kiwigrad Library](#kiwigrad-library)
+    - [Examples](#examples)
+  - [TODOS](#todos)
+
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
 ```console
@@ -43,8 +49,8 @@
 
 model = PotNet()
 ```
 
 ## TODOS
 
 * Include the activation functions tanh in the Value object.
-* Add a notebook example for training a neural network on a regression problem.
+* Fix pow function.
```

### Comparing `kiwigrad-0.23/kiwigrad/engine.c` & `kiwigrad-0.24/kiwigrad/engine.c`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 typedef struct List List;
 
 typedef struct {
   PyObject_HEAD
   double data;
   double grad;
+  double oa;
   PyObject *prev;
   int func_idx;
   PyObject *tmp;
   List *topology;
   int visited;
 } Value;
 
@@ -37,14 +38,15 @@
   if (!PyArg_ParseTuple(args, "d", &data))
     return NULL;
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   if (value) {
     value->grad = 0.0;
     value->visited = 0;
     value->data = data;
+    value->oa = 0.0;
     value->prev = PyTuple_New(0);
     value->topology = NULL;
     value->tmp = Py_None;
     value->func_idx = -1;
   }
   return (PyObject *)value;
 }
@@ -151,21 +153,21 @@
   child_2->grad += child_1->data * ((Value *)self)->grad;
   Py_RETURN_NONE;
 }
 
 static PyObject *
 pow_backward(PyObject *self) {
   Value *child = ((Value*)PyTuple_GetItem(((Value *)self)->prev, 0));
-
-  child->grad += PyFloat_AsDouble(((Value *)self)->tmp) *
-    pow(child->data, PyFloat_AsDouble(((Value *)self)->tmp) - 1.0) *
-    ((Value *)self)->grad;
+  double exponent = ((Value *)self)->oa; 
+  double base = child->data;
+  child->grad += exponent * pow(base, exponent - 1.0) * ((Value *)self)->grad;
   Py_RETURN_NONE;
 }
 
+
 typedef PyObject * (*BackwardFunction)(PyObject *);
 static BackwardFunction backward_methods[] = {
    &add_backward,
    &mul_backward,
    &pow_backward,
    &relu_backward,
    &sigmoid_backward,
@@ -297,15 +299,16 @@
 }
 
 PyObject * pyvalue_pow(PyObject *self, PyObject *other, PyObject *arg) {
   Value *value = (Value *)Value_Type.tp_alloc(&Value_Type, 0);
   value->data = pow(((Value *)self)->data, PyFloat_AsDouble(other));
   value->grad = 0.0;
   value->prev = PyTuple_Pack(1, self);
-  value->tmp = other;
+  value->oa = PyFloat_AsDouble(other);
+  //value->tmp = other;
   value->func_idx = 2;
   return (PyObject *)value;
 }
 
 PyObject * pyvalue_negative(PyObject *self) {
   PyObject *other = (PyObject *)Value_Type.tp_alloc(&Value_Type, 0);
   Py_INCREF(other);
@@ -427,8 +430,8 @@
 
   if (PyType_Ready(&Value_Type) < 0) {
     return NULL;
   }
   Py_INCREF(&Value_Type);
   PyModule_AddObject(m, "Value", (PyObject *)&Value_Type);
   return m;
-}
+}
```

### Comparing `kiwigrad-0.23/kiwigrad/engine.py` & `kiwigrad-0.24/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.23/kiwigrad/layers.py` & `kiwigrad-0.24/kiwigrad/layers.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.23/kiwigrad/neurons.py` & `kiwigrad-0.24/kiwigrad/neurons.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.23/kiwigrad/nn.py` & `kiwigrad-0.24/kiwigrad/nn.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.23/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.24/kiwigrad.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.23
+Version: 0.24
 Summary: Mini deep learning framework
 Home-page: https://github.com/marcosalvalaggio/kiwigrad
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,20 @@
 
 <h1 align="center">
 <img src="logo.png" width="200">
 </h1><br>
 
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity) 
 
+- [Kiwigrad](#kiwigrad)
+  - [Install](#install)
+  - [Kiwigrad Library](#kiwigrad-library)
+    - [Examples](#examples)
+  - [TODOS](#todos)
+
 Kiwigrad? yes, it is another version of [micrograd](https://github.com/karpathy/micrograd) that was created just for fun and experimentation.
 
 ## Install 
 
 To install the current release,
 
 ```console
@@ -59,9 +65,9 @@
 
 model = PotNet()
 ```
 
 ## TODOS
 
 * Include the activation functions tanh in the Value object.
-* Add a notebook example for training a neural network on a regression problem.
+* Fix pow function.
```

### Comparing `kiwigrad-0.23/setup.py` & `kiwigrad-0.24/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from setuptools.extension import Extension
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='kiwigrad',
-      version='0.23',
+      version='0.24',
       description='Mini deep learning framework',
       author='Marco Salvalaggio',
       author_email='mar.salvalaggio@gmail.com',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/marcosalvalaggio/kiwigrad',
```

### Comparing `kiwigrad-0.23/test/test.py` & `kiwigrad-0.24/test/test.py`

 * *Files identical despite different names*

