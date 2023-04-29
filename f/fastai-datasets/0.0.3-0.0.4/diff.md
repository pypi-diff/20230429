# Comparing `tmp/fastai-datasets-0.0.3.tar.gz` & `tmp/fastai-datasets-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastai-datasets-0.0.3.tar", last modified: Tue Apr 25 14:48:13 2023, max compression
+gzip compressed data, was "fastai-datasets-0.0.4.tar", last modified: Sat Apr 29 20:46:54 2023, max compression
```

## Comparing `fastai-datasets-0.0.3.tar` & `fastai-datasets-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-25 14:48:13.279806 fastai-datasets-0.0.3/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.3/LICENSE
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.3/MANIFEST.in
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-25 14:48:13.275805 fastai-datasets-0.0.3/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3894 2023-04-25 14:46:07.000000 fastai-datasets-0.0.3/README.md
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-25 14:48:13.275805 fastai-datasets-0.0.3/fastai_datasets/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/__init__.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/_modidx.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.3/fastai_datasets/all.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/cifar10.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/imagenette.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/lfw.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/mnist.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3802 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/pairs.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5841 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/patches.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/pfr.py
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1894 2023-04-25 14:47:34.000000 fastai-datasets-0.0.3/fastai_datasets/utils.py
-drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-25 14:48:13.275805 fastai-datasets-0.0.3/fastai_datasets.egg-info/
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/PKG-INFO
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/SOURCES.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/dependency_links.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/entry_points.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/not-zip-safe
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/requires.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-04-25 14:48:13.000000 fastai-datasets-0.0.3/fastai_datasets.egg-info/top_level.txt
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-04-25 14:48:02.000000 fastai-datasets-0.0.3/settings.ini
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-04-25 14:48:13.279806 fastai-datasets-0.0.3/setup.cfg
--rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.3/setup.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    35149 2023-04-13 22:08:00.000000 fastai-datasets-0.0.4/LICENSE
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      111 2023-04-13 22:08:00.000000 fastai-datasets-0.0.4/MANIFEST.in
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3894 2023-04-25 14:46:07.000000 fastai-datasets-0.0.4/README.md
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-29 20:46:54.345998 fastai-datasets-0.0.4/fastai_datasets/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      313 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/__init__.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)    12255 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/_modidx.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      172 2023-04-14 23:03:52.000000 fastai-datasets-0.0.4/fastai_datasets/all.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      461 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/cifar10.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      615 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/imagenette.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     4575 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/lfw.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      858 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/mnist.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     3675 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/pairs.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5767 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/patches.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      796 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/pfr.py
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     1877 2023-04-29 20:46:46.000000 fastai-datasets-0.0.4/fastai_datasets/utils.py
+drwxrwxr-x   0 paperspace  (1000) paperspace  (1000)        0 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/fastai_datasets.egg-info/
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     5492 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/PKG-INFO
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      608 2023-04-29 20:46:54.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/SOURCES.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/dependency_links.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       73 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/entry_points.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)        1 2023-04-13 22:13:24.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/not-zip-safe
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       30 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/requires.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       16 2023-04-29 20:46:53.000000 fastai-datasets-0.0.4/fastai_datasets.egg-info/top_level.txt
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)      991 2023-04-29 20:44:50.000000 fastai-datasets-0.0.4/settings.ini
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)       38 2023-04-29 20:46:54.349998 fastai-datasets-0.0.4/setup.cfg
+-rw-rw-r--   0 paperspace  (1000) paperspace  (1000)     2560 2023-04-13 22:08:00.000000 fastai-datasets-0.0.4/setup.py
```

### Comparing `fastai-datasets-0.0.3/LICENSE` & `fastai-datasets-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/PKG-INFO` & `fastai-datasets-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.3
+Version: 0.0.4
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
```

### Comparing `fastai-datasets-0.0.3/README.md` & `fastai-datasets-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/fastai_datasets/_modidx.py` & `fastai-datasets-0.0.4/fastai_datasets/_modidx.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/fastai_datasets/imagenette.py` & `fastai-datasets-0.0.4/fastai_datasets/imagenette.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/fastai_datasets/lfw.py` & `fastai-datasets-0.0.4/fastai_datasets/lfw.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/fastai_datasets/mnist.py` & `fastai-datasets-0.0.4/fastai_datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/fastai_datasets/pairs.py` & `fastai-datasets-0.0.4/fastai_datasets/pairs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/pairs.ipynb.
 
 # %% auto 0
 __all__ = ['ImagePair', 'Sameness', 'Pairs']
 
 # %% ../nbs/pairs.ipynb 2
 import random
-from typing import NamedTuple, Union
+from typing import Union
 
 from fastai.vision.all import *
 from fastprogress.fastprogress import *
 
 import fastai_datasets.patches
 from .utils import *
 
@@ -50,27 +50,27 @@
 def _pairs_for_split(singles: DataLoaders, split_idx: int, factor: int):
     assert singles.n_inp == 1
 
     indices = L(range_of(singles))[singles.splits[split_idx]]
     num = int(len(indices) * factor)
 
     class_map = defaultdict(list)
-    for i, c in progress_bar(indices.zipwith(singles.i2t.subset(split_idx)), comment='Class map: scanning targets'):
+    for i, c in progress_bar(indices.zipwith(singles.i2t.subset(split_idx))):
         class_map[singles.vocab[c]].append(i)
 
     @return_list
     def _positive_pairs():
         multi_item_class_map = {k: v for k, v in class_map.items() if len(v)>1}
-        for _ in progress_bar(range(num//2), comment=f'Generating positive pairs'):
+        for _ in progress_bar(range(num//2)):
             c, idxs = random.choice(list(multi_item_class_map.items()))
             yield tuple(random.sample(idxs, 2))
 
     @return_list
     def _negative_pairs():
-        for _ in progress_bar(range(num//2), comment=f'Generating negative pairs'):
+        for _ in progress_bar(range(num//2)):
             (c1, idxs1), (c2, idxs2) = random.sample(list(class_map.items()), 2)
             yield (random.choice(idxs1), random.choice(idxs2))
 
     return _positive_pairs() + _negative_pairs()
 
 
 def Pairs(singles: Datasets,  # Used to construct pairs
```

### Comparing `fastai-datasets-0.0.3/fastai_datasets/patches.py` & `fastai-datasets-0.0.4/fastai_datasets/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,18 +94,18 @@
     assert self.n_inp == len(self.tls) - 1
     return self.tls[-1]
 
 # %% ../nbs/Core/patches.ipynb 35
 @patch(as_prop=True)
 def by_target(self: Datasets) -> Dict[int, Datasets]:
     if not hasattr(self, '_by_target'):
-        targets = [int(t) for t in progress_bar(self.i2t, comment='Class map: scanning targets')]
+        targets = [int(t) for t in progress_bar(self.i2t)]
         class_map = groupby(enumerate(targets), key=1, val=0)
         self._by_target = {self.vocab[c]: self.sub_dsets(indices)
-                           for c, indices in progress_bar(class_map.items(), comment='Class map: partitioning')}
+                           for c, indices in progress_bar(class_map.items())}
     return self._by_target
 
 
 # %% ../nbs/Core/patches.ipynb 37
 import matplotlib.pyplot as plt
 
 @patch()
```

### Comparing `fastai-datasets-0.0.3/fastai_datasets/pfr.py` & `fastai-datasets-0.0.4/fastai_datasets/pfr.py`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/fastai_datasets/utils.py` & `fastai-datasets-0.0.4/fastai_datasets/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,12 +54,12 @@
     loader = torch.utils.data.DataLoader(
         Datasets(get_image_files(path), [PIL.Image.open, noop]),
         num_workers=0 if os.name == 'nt' else 8,
         batch_size=64 if batched else 1,
         collate_fn=training.collate_pil
     )
 
-    for imgs, paths in progress_bar(loader, comment='MTCNN'):
+    for imgs, paths in progress_bar(loader):
         output_paths = [mtcnn_path/p.relative_to(path) for p in paths]
         mtcnn(imgs, save_path=output_paths)
 
     return mtcnn_path
```

### Comparing `fastai-datasets-0.0.3/fastai_datasets.egg-info/PKG-INFO` & `fastai-datasets-0.0.4/fastai_datasets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastai-datasets
-Version: 0.0.3
+Version: 0.0.4
 Summary: Leveraging fastai to easily load and handle datasets
 Home-page: https://github.com/Irad-Zehavi/fastai-datasets
 Author: iradz
 Author-email: irad.zehavi@outlook.com
 License: Apache Software License 2.0
 Description: fastai-datasets
         ================
```

### Comparing `fastai-datasets-0.0.3/fastai_datasets.egg-info/SOURCES.txt` & `fastai-datasets-0.0.4/fastai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastai-datasets-0.0.3/settings.ini` & `fastai-datasets-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastai-datasets
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastai_datasets
```

### Comparing `fastai-datasets-0.0.3/setup.py` & `fastai-datasets-0.0.4/setup.py`

 * *Files identical despite different names*

