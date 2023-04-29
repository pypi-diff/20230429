# Comparing `tmp/nadir-0.0.3.tar.gz` & `tmp/nadir-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadir-0.0.3.tar", last modified: Wed Mar  8 18:08:52 2023, max compression
+gzip compressed data, was "nadir-0.1.0.tar", last modified: Sat Apr 29 19:59:51 2023, max compression
```

## Comparing `nadir-0.0.3.tar` & `nadir-0.1.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-03-08 18:08:52.737256 nadir-0.0.3/
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)    11344 2023-03-04 17:09:02.000000 nadir-0.0.3/LICENCE
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4392 2023-03-08 18:08:52.737256 nadir-0.0.3/PKG-INFO
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     3593 2023-03-08 18:01:41.000000 nadir-0.0.3/README.md
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1006 2023-03-08 18:08:43.000000 nadir-0.0.3/pyproject.toml
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      791 2023-03-08 18:08:52.737256 nadir-0.0.3/setup.cfg
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       37 2023-03-04 17:09:02.000000 nadir-0.0.3/setup.py
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-03-08 18:08:52.733255 nadir-0.0.3/src/
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-03-08 18:08:52.737256 nadir-0.0.3/src/nadir/
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1592 2023-03-08 18:01:57.000000 nadir-0.0.3/src/nadir/__init__.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1812 2023-03-04 17:20:56.000000 nadir-0.0.3/src/nadir/adadelta.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1410 2023-03-04 17:17:09.000000 nadir-0.0.3/src/nadir/adagrad.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1424 2023-03-04 17:18:12.000000 nadir-0.0.3/src/nadir/adam.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1648 2023-03-04 17:19:24.000000 nadir-0.0.3/src/nadir/adamax.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1655 2023-03-08 16:15:57.000000 nadir-0.0.3/src/nadir/adamw.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1694 2023-03-08 16:14:28.000000 nadir-0.0.3/src/nadir/amsgrad.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4415 2023-03-08 15:59:09.000000 nadir-0.0.3/src/nadir/base.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1888 2023-03-08 17:01:50.000000 nadir-0.0.3/src/nadir/lion.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1211 2023-03-04 17:14:51.000000 nadir-0.0.3/src/nadir/momentum.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1863 2023-03-08 16:18:03.000000 nadir-0.0.3/src/nadir/radam.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1232 2023-03-04 17:16:03.000000 nadir-0.0.3/src/nadir/rmsprop.py
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      949 2023-03-04 17:13:53.000000 nadir-0.0.3/src/nadir/sgd.py
-drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-03-08 18:08:52.737256 nadir-0.0.3/src/nadir.egg-info/
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4392 2023-03-08 18:08:52.000000 nadir-0.0.3/src/nadir.egg-info/PKG-INFO
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      473 2023-03-08 18:08:52.000000 nadir-0.0.3/src/nadir.egg-info/SOURCES.txt
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        1 2023-03-08 18:08:52.000000 nadir-0.0.3/src/nadir.egg-info/dependency_links.txt
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       45 2023-03-08 18:08:52.000000 nadir-0.0.3/src/nadir.egg-info/requires.txt
--rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        6 2023-03-08 18:08:52.000000 nadir-0.0.3/src/nadir.egg-info/top_level.txt
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.316702 nadir-0.1.0/
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)    11344 2023-03-04 17:09:02.000000 nadir-0.1.0/LICENCE
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4464 2023-04-29 19:59:51.316702 nadir-0.1.0/PKG-INFO
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     3665 2023-04-29 19:54:16.000000 nadir-0.1.0/README.md
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1006 2023-04-29 19:59:04.000000 nadir-0.1.0/pyproject.toml
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      791 2023-04-29 19:59:51.320702 nadir-0.1.0/setup.cfg
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       37 2023-03-04 17:09:02.000000 nadir-0.1.0/setup.py
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.300703 nadir-0.1.0/src/
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.312703 nadir-0.1.0/src/nadir/
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1065 2023-04-29 19:51:57.000000 nadir-0.1.0/src/nadir/NAG.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1592 2023-04-29 19:59:18.000000 nadir-0.1.0/src/nadir/__init__.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1803 2023-04-29 18:32:39.000000 nadir-0.1.0/src/nadir/adadelta.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1410 2023-03-04 17:17:09.000000 nadir-0.1.0/src/nadir/adagrad.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     3825 2023-04-25 15:23:45.000000 nadir-0.1.0/src/nadir/adam.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1617 2023-04-29 16:39:23.000000 nadir-0.1.0/src/nadir/adamax.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1193 2023-04-29 18:34:17.000000 nadir-0.1.0/src/nadir/adamw.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1201 2023-04-29 18:37:27.000000 nadir-0.1.0/src/nadir/amsgrad.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2569 2023-04-25 15:16:08.000000 nadir-0.1.0/src/nadir/base.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2327 2023-04-29 18:47:36.000000 nadir-0.1.0/src/nadir/lion.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1364 2023-04-29 18:56:03.000000 nadir-0.1.0/src/nadir/momentum.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1802 2023-04-29 18:50:06.000000 nadir-0.1.0/src/nadir/radam.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     1232 2023-03-04 17:16:03.000000 nadir-0.1.0/src/nadir/rmsprop.py
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     2454 2023-04-29 19:50:57.000000 nadir-0.1.0/src/nadir/sgd.py
+drwxrwxr-x   0 ec3dev    (1001) ec3dev    (1001)        0 2023-04-29 19:59:51.316702 nadir-0.1.0/src/nadir.egg-info/
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)     4464 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/PKG-INFO
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)      490 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        1 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)       45 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/requires.txt
+-rw-rw-r--   0 ec3dev    (1001) ec3dev    (1001)        6 2023-04-29 19:59:51.000000 nadir-0.1.0/src/nadir.egg-info/top_level.txt
```

### Comparing `nadir-0.0.3/LICENCE` & `nadir-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `nadir-0.0.3/PKG-INFO` & `nadir-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadir
-Version: 0.0.3
+Version: 0.1.0
 Summary: Nadir is a library of bleeding-edge DL optimisers built for speed and functionality in PyTorch for researchers
 Author-email: Bhavnick Minhas <bhavnicksm@gmail.com>
 Maintainer-email: Bhavnick Minhas <bhavnicksm@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Dawn-Of-Eve/nadir
 Project-URL: Bug Tracker, https://github.com/Dawn-Of-Eve/nadir/issues
 Keywords: machine learning,optimization,adam-optimizer
@@ -73,21 +73,22 @@
 
 # Supported Optimisers
 
 | Optimiser 	| Paper 	                                            |
 |:---------:	|:-----:	                                            |
 |  **SGD**  	| https://paperswithcode.com/method/sgd                 |
 |  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum   |
+|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html       |
 |  **Adagrad** 	| https://www.jmlr.org/papers/volume12/duchi11a/duchi11a.pdf |
 |  **RMSProp** 	| https://paperswithcode.com/method/rmsprop             |
 |  **Adam**     | https://arxiv.org/abs/1412.6980v9                     |
 |  **Adamax**   | https://arxiv.org/abs/1412.6980v9                     |
 |  **AdamW**    | https://arxiv.org/abs/1711.05101v3                    |
 |  **Adadelta** | https://arxiv.org/abs/1212.5701v1                     |
-|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                    |
+|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                  |
 |  **RAdam**    | https://arxiv.org/abs/1908.03265v4                    |
 |  **Lion**     | https://arxiv.org/abs/2302.06675                      |
 
 # Acknowledgements
 
 We would like to thank all the amazing contributors of this project who spent so much effort making this repositary awesome! :heart:
```

### Comparing `nadir-0.0.3/README.md` & `nadir-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,21 +55,22 @@
 
 # Supported Optimisers
 
 | Optimiser 	| Paper 	                                            |
 |:---------:	|:-----:	                                            |
 |  **SGD**  	| https://paperswithcode.com/method/sgd                 |
 |  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum   |
+|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html       |
 |  **Adagrad** 	| https://www.jmlr.org/papers/volume12/duchi11a/duchi11a.pdf |
 |  **RMSProp** 	| https://paperswithcode.com/method/rmsprop             |
 |  **Adam**     | https://arxiv.org/abs/1412.6980v9                     |
 |  **Adamax**   | https://arxiv.org/abs/1412.6980v9                     |
 |  **AdamW**    | https://arxiv.org/abs/1711.05101v3                    |
 |  **Adadelta** | https://arxiv.org/abs/1212.5701v1                     |
-|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                    |
+|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                  |
 |  **RAdam**    | https://arxiv.org/abs/1908.03265v4                    |
 |  **Lion**     | https://arxiv.org/abs/2302.06675                      |
 
 # Acknowledgements
 
 We would like to thank all the amazing contributors of this project who spent so much effort making this repositary awesome! :heart:
```

### Comparing `nadir-0.0.3/pyproject.toml` & `nadir-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nadir"
-version = "0.0.3"
+version = "0.1.0"
 authors = [
   { name="Bhavnick Minhas", email="bhavnicksm@gmail.com" },
 ]
 maintainers = [
   { name = "Bhavnick Minhas", email="bhavnicksm@gmail.com"},
 ]
 description = "Nadir is a library of bleeding-edge DL optimisers built for speed and functionality in PyTorch for researchers"
```

### Comparing `nadir-0.0.3/setup.cfg` & `nadir-0.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nadir-0.0.3/src/nadir/__init__.py` & `nadir-0.1.0/src/nadir/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .lion import Lion, LionConfig
 from .momentum import Momentum, MomentumConfig
 from .rmsprop import RMSProp, RMSPropConfig
 from .radam import Radam, RadamConfig
 from .sgd import SGD, SGDConfig
 
 
-__version__ = "0.0.3"
+__version__ = "0.1.0"
 
 __all__ = ('Adadelta',
            'AdadeltaConfig',
            'Adagrad',
            'AdagradConfig',
            'Adam',
            'AdamConfig',
```

### Comparing `nadir-0.0.3/src/nadir/adadelta.py` & `nadir-0.1.0/src/nadir/adadelta.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,39 +12,40 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
 import torch
 
-from .base import BaseOptimizer
-from .base import BaseConfig
+from .adam import Adam, AdamConfig
 
 
 __all__ = ['AdadeltaConfig', 'Adadelta']
 
 @dataclass
-class AdadeltaConfig(BaseConfig):
+class AdadeltaConfig(AdamConfig):
   lr : float = 1
-  adaptive : bool = True
   rho : float = 0.90
+  beta_1 : float = 0.0
   beta_2 : float = 0.90
   eps : float = 1E-6
+  bias_correction : bool = False
 
 
-class Adadelta(BaseOptimizer):
+class Adadelta(Adam):
   def __init__ (self, params, config : AdadeltaConfig = AdadeltaConfig()):
     super().__init__(params, config)
 
     self.config = config
+
     if self.config.rho != self.config.beta_2:
       self.config.beta_2 = self.config.rho
   
   def init_state(self, state, group, param):
-    state['adaptive_step'] = 0
+    state['step'] = 0
     state['adaptivity'] = torch.zeros_like(param, memory_format=torch.preserve_format)
     state['acc_delta'] = torch.zeros_like(param, memory_format=torch.preserve_format)
 
   def update(self, state, group, grad, param):
     eps = self.config.eps
     rho = self.config.rho
     lr = group['lr']
@@ -53,8 +54,8 @@
     denom = self.adaptivity(state, grad)
 
     delta = m.add(eps).sqrt_().div_(denom).mul_(grad)
     
     param.data.add_(delta, alpha = -1 * lr)
 
     m.mul_(rho).addcmul_(delta, delta, value=(1 - rho))
-    state['acc_delta'] = m 
+    state['acc_delta'] = m
```

### Comparing `nadir-0.0.3/src/nadir/adagrad.py` & `nadir-0.1.0/src/nadir/adagrad.py`

 * *Files identical despite different names*

### Comparing `nadir-0.0.3/src/nadir/adam.py` & `nadir-0.1.0/src/nadir/adamax.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,37 +13,40 @@
 # limitations under the License.
 
 from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
 import torch
 
-from .base import BaseOptimizer
-from .base import BaseConfig
+from .adam import Adam, AdamConfig
 
-
-__all__ = ['AdamConfig', 'Adam']
+__all__ = ['AdamaxConfig', 'Adamax']
 
 @dataclass
-class AdamConfig(BaseConfig):
-  lr : float = 3E-4
+class AdamaxConfig(AdamConfig):
+  lr : float = 2E-3
   momentum : bool = True
   adaptive : bool = True
   beta_1 : float = 0.9
   beta_2 : float = 0.999
   eps : float = 1E-8
 
-
-
-class Adam(BaseOptimizer):
-
-  def __init__(self, params, config : AdamConfig = AdamConfig()):
+class Adamax(Adam):
+  def __init__ (self, params, config : AdamaxConfig = AdamaxConfig()):
     if not config.momentum:
       raise ValueError(f"Invalid value for momentum in config: {config.momentum} ", 
                        "Value must be True")
     if not config.adaptive:
       raise ValueError(f"Invalid value for adaptive in config: {config.adaptive} ", 
                        "Value must be True")
-      
+    
     super().__init__(params, config)
-
-    self.config = config
+    self.config = config
+  
+  def adaptivity(self, state, grad):
+    u = state['adaptivity']
+    beta_2 = self.config.beta_2
+
+    u = torch.max(torch.mul(u, beta_2), torch.abs(grad) + self.config.eps)
+    
+    state['adaptivity'] = u
+    return u
```

### Comparing `nadir-0.0.3/src/nadir/adamax.py` & `nadir-0.1.0/src/nadir/momentum.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,47 +7,34 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
-import torch
-
-from .base import BaseOptimizer
-from .base import BaseConfig
-
+from .sgd import SGDConfig, SGD
 
-__all__ = ['AdamaxConfig', 'Adamax']
+__all__ = ['MomentumConfig', 'Momentum']
 
 @dataclass
-class AdamaxConfig(BaseConfig):
-  lr : float = 2E-3
-  momentum : bool = True
-  adaptive : bool = True
-  beta_1 : float = 0.9
-  beta_2 : float = 0.999
-  eps : float = 1E-8
+class MomentumConfig(SGDConfig):
+  lr : float = 1E-3
+  momentum : float = 0.9
+  dampening : float = 0.05
 
 
-class Adamax(BaseOptimizer):
-  def __init__ (self, params, config : AdamaxConfig = AdamaxConfig()):
-    if not config.momentum:
+class Momentum(SGD):
+  
+  def __init__(self, params, config : MomentumConfig = MomentumConfig()):
+    if not 1 >= config.momentum > 0:
       raise ValueError(f"Invalid value for momentum in config: {config.momentum} ", 
-                       "Value must be True")
-    if not config.adaptive:
-      raise ValueError(f"Invalid value for adaptive in config: {config.adaptive} ", 
-                       "Value must be True")
+                       "Value must not be 0")
+      
+    if not 1 >= config.dampening >= 0:
+      raise ValueError(f"Invalid value for dampening in config: {config.dampening} ", 
+                       "Value must not be less than 0")
     
     super().__init__(params, config)
-    self.config = config
-  
-  def adaptivity(self, state, grad):
-    u = state['adaptivity']
-    beta_2 = self.config.beta_2
-    u = torch.max(torch.mul(u, beta_2), torch.abs(grad) + self.config.eps)
-    state['adaptivity'] = u
-    return u
+    self.config = config
```

### Comparing `nadir-0.0.3/src/nadir/adamw.py` & `nadir-0.1.0/src/nadir/adamw.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,37 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
 import torch
 
-from .base import BaseOptimizer
-from .base import BaseConfig
+from .adam import Adam, AdamConfig
 
 
 __all__ = ['AdamWConfig', 'AdamW']
 
 @dataclass
-class AdamWConfig(BaseConfig):
+class AdamWConfig(AdamConfig):
   lr : float = 3E-4
-  momentum : bool = True
-  adaptive : bool = True
-  beta_1 : float = 0.9
-  beta_2 : float = 0.999
-  eps : float = 1E-8
   weight_decay : float = 0.01
 
-class AdamW(BaseOptimizer):
+class AdamW(Adam):
   def __init__ (self, params, config : AdamWConfig = AdamWConfig()):
-    if not config.momentum:
-      raise ValueError(f"Invalid value for momentum in config: {config.momentum} ", 
-                       "Value must be True")
-    if not config.adaptive:
-      raise ValueError(f"Invalid value for adaptive in config: {config.adaptive} ", 
-                       "Value must be True")
+
     if not 1.0 > config.weight_decay > 0.0:
       raise ValueError(f"Invalid value for weight_decay in config: {config.weight_decay} ", 
                        "Value must be float between 0 and 1")  
+      
     super().__init__(params, config)
     
     self.config = config
```

### Comparing `nadir-0.0.3/src/nadir/amsgrad.py` & `nadir-0.1.0/src/nadir/amsgrad.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,37 +14,25 @@
 
 from typing import Dict, Tuple, Any, Optional
 from dataclasses import dataclass
 
 import torch
 from torch.optim.optimizer import Optimizer
 
-from .base import BaseOptimizer
-from .base import BaseConfig
+from .adam import Adam, AdamConfig
 
 __all__ = ['AMSGradConfig', 'AMSGrad']
 
 @dataclass
-class AMSGradConfig(BaseConfig):
+class AMSGradConfig(AdamConfig):
   lr : float = 3E-4
-  momentum : bool = True
-  adaptive : bool = True
-  beta_1 : float = 0.9
-  beta_2 : float = 0.999
-  eps : float = 1E-8
-  weight_decay : float = 0.
   amsgrad : bool = True
 
-class AMSGrad(BaseOptimizer):
+class AMSGrad(Adam):
   def __init__ (self, params, config : AMSGradConfig = AMSGradConfig()):
-    if not config.momentum:
-      raise ValueError(f"Invalid value for momentum in config: {config.momentum} ", 
-                       "Value must be True")
-    if not config.adaptive:
-      raise ValueError(f"Invalid value for adaptive in config: {config.adaptive} ", 
-                       "Value must be True")
+    
     if not config.amsgrad:
       raise ValueError(f"Invalid value for amsgrad in config: {config.amsgrad} ", 
                        "Value must be True")
     super().__init__(params, config)
     
     self.config = config
```

### Comparing `nadir-0.0.3/src/nadir/base.py` & `nadir-0.1.0/src/nadir/adam.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,77 +8,77 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Dict, Tuple, Any, Optional
+from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
 import torch
-from torch.optim.optimizer import Optimizer
 
-__all__ = ['BaseConfig', 'BaseOptimizer']
+from .base import BaseOptimizer
+from .base import BaseConfig
+
+
+__all__ = ['AdamConfig', 'Adam']
 
 @dataclass
-class BaseConfig:
-  lr : float = 1E-3
-  momentum : bool = False
-  adaptive : bool = False
-  beta_1 : float = 0.0
-  beta_2 : float = 0.0
+class AdamConfig(BaseConfig):
+  lr : float = 3E-4
+  beta_1 : float = 0.9
+  beta_2 : float = 0.999
   eps : float = 1E-8
   weight_decay : float = 0.0
   amsgrad : bool = False
+  bias_correction: bool = True
 
-  def dict(self):
-    return self.__dict__
-
-
-class BaseOptimizer (Optimizer):
+class Adam(BaseOptimizer):
 
-  def __init__  (self, params, config: BaseConfig = BaseConfig()):
-    if not config.lr > 0.0:
-      raise ValueError(f"Invalid value for lr in config: {config.lr} ", 
-                       "Value must be > 0")
-    if not 1.0 > config.beta_1 >= 0.0:
+  def __init__(self, params, config : AdamConfig = AdamConfig()):
+    if not 1 >= config.beta_1 >= 0:
       raise ValueError(f"Invalid value for beta_1 in config: {config.beta_1} ", 
-                       "Value must be 1 > x >= 0")
-    if not 1.0 > config.beta_2 >= 0.0:
+                       "Value must be between 0 and 1")
+    if not 1 >= config.beta_2 >= 0:
       raise ValueError(f"Invalid value for beta_2 in config: {config.beta_2} ", 
-                       "Value must be 1 > x >= 0")
-    super().__init__(params, config.dict())
+                       "Value must be between 0 and 1")
+    super().__init__(params, config)
 
     self.config = config
 
   def init_state(self,
                  state,
                  group,
                  param):
     state['step'] = 0
 
-    if self.config.momentum:
+    if 1 >= self.config.beta_1 > 0:
       state['momentum'] = torch.zeros_like(param, memory_format=torch.preserve_format)
     
-    if self.config.adaptive:
+    if 1 >= self.config.beta_2 > 0:
       state['adaptivity'] = torch.zeros_like(param, memory_format=torch.preserve_format)
       
       if self.config.amsgrad:
         state['amsgrad'] = torch.zeros_like(param, memory_format=torch.preserve_format)
 
   def momentum(self,
                state, 
                grad):
     step = state['step']
     m = state['momentum']
     beta_1 = self.config.beta_1
+    bias_correction = self.config.bias_correction
 
     m.mul_(beta_1).add_(grad, alpha= (1 - beta_1))
-    m_hat = m.div(1 - beta_1**(step + 1))
+    
+    if bias_correction:
+      m_hat = m.div(1 - beta_1**(step + 1))
+    else:
+      m_hat = m
 
     state['momentum'] = m
     return m_hat
 
   def amsgrad(adaptivity):
 
     def __adaptivity__(self, state, grad):
@@ -98,62 +98,46 @@
   def adaptivity(self, 
                  state, 
                  grad):
     
     step = state['step']
     v = state['adaptivity']
     beta_2 = self.config.beta_2
+    bias_correction = self.config.bias_correction
 
     v.mul_(beta_2).addcmul_(grad, grad, value = (1 - beta_2))
-    v_hat = v.div(1 - beta_2**(step + 1))
 
+    if bias_correction:
+      v_hat = v.div(1 - beta_2**(step + 1))
+    else:
+      v_hat = v
+    
     state['adaptivity'] = v
     return torch.sqrt(v_hat + self.config.eps)
 
   def update(self,
              state: Dict[str, any],
              group: Dict[str, any],
              grad:  torch.Tensor,
              param: torch.Tensor):
     
     lr = group['lr']
+    beta_1 = self.config.beta_1
+    beta_2 = self.config.beta_2
 
-    if self.config.momentum:
+    if 1 >= beta_1 > 0:
       m = self.momentum(state, grad)
       upd = m
     else:
       upd = grad
     
-    if self.config.adaptive:
+    if 1>= beta_2 > 0:
       v = self.adaptivity(state, grad)
       param.data.addcdiv_(upd, v, value = -1 * lr)
     else:
       param.data.add_(upd, alpha = -1 * lr)
 
     if self.config.weight_decay > 0:
       param.data.add_(param.data,
                       alpha = -1 * lr * self.config.weight_decay)
       
-    state['step'] += 1
-
-  @torch.no_grad()
-  def step(self, closure = None):
-    loss = None
-    if closure is not None:
-      with torch.enable_grad():
-        loss = closure()
-
-    for group in self.param_groups:
-      for param in group['params']:
-        if param.grad is None:
-         continue
-        grad = param.grad.data
-        if grad.is_sparse:
-          raise RuntimeError('This Optimizer does not support sparse gradients,'
-                                  ' please consider SparseAdam instead')
-        state = self.state[param]
-        if len(state) == 0:
-          self.init_state(state, group, param)
-
-        self.update(state, group, grad, param)
-    
-    return loss
+    state['step'] += 1
```

### Comparing `nadir-0.0.3/src/nadir/lion.py` & `nadir-0.1.0/src/nadir/lion.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,43 +20,61 @@
 from .base import BaseConfig
 
 
 __all__ = ['LionConfig', 'Lion']
 
 @dataclass
 class LionConfig(BaseConfig):
-  lr : float = 1E-4
-  momentum : bool = True
+  lr : float = 3E-4
   beta_1 : float = 0.9
   beta_2 : float = 0.99
-  eps : float = 1E-8
-  weight_decay : float = 0.
-
-
+  weight_decay : float = 0.0
 
 class Lion(BaseOptimizer):
-  
-  def __init__(self, params, config: LionConfig = LionConfig()):
-    if not config.momentum:
-      raise ValueError(f"Invalid value for momentum in config: {config.momentum} ", 
-                       "Value must be True")
+  def __init__ (self, params, config : LionConfig = LionConfig()):
     if not 1 > config.beta_1 > 0.:
       raise ValueError(f"Invalid value for beta_1 in config: {config.beta_1} ", 
                        "Value must be between 1 and 0")
     if not 1 > config.beta_2 > 0.:
       raise ValueError(f"Invalid value for beta_2 in config: {config.beta_2} ", 
                        "Value must be between 1 and 0")
     super().__init__(params, config)
     self.config = config
 
+  def init_state(self,
+                 state,
+                 group,
+                 param):
+    
+    state['step'] = 0
+    
+    state['momentum'] = torch.zeros_like(param, memory_format=torch.preserve_format)
+
   def momentum(self, state, grad):
     m = state['momentum']
     beta_1 = self.config.beta_1
     beta_2 = self.config.beta_2
 
     u = m.mul(beta_1).add_(grad, alpha=(1-beta_1))
     
     m.mul_(beta_2).add_(grad, alpha=(1-beta_2))
 
     state['momentum'] = m
 
-    return torch.sign(u)
+    return torch.sign(u)
+  
+  def update(self,
+             state: Dict[str, any],
+             group: Dict[str, any],
+             grad:  torch.Tensor,
+             param: torch.Tensor):
+    
+    lr = group['lr']
+    
+    m = self.momentum(state, grad)
+
+    param.data.add_(m, alpha = -1 * lr)
+
+    if self.config.weight_decay > 0:
+      param.data.add_(param.data,
+                      alpha = -1 * lr * self.config.weight_decay)
+    state['step'] += 1
```

### Comparing `nadir-0.0.3/src/nadir/momentum.py` & `nadir-0.1.0/src/nadir/NAG.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,27 +12,24 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Dict, Any, Optional
 from dataclasses import dataclass
 
 import torch
 
-from .base import BaseOptimizer
-from .base import BaseConfig
+from .momentum import Momentum, MomentumConfig
 
-
-__all__ = ['MomentumConfig', 'Momentum']
+__all__ = ['NAGConfig', 'NAG']
 
 @dataclass
-class MomentumConfig(BaseConfig):
-  lr : float = 1E-3
-  momentum : bool = True
-  beta_1 : float = 0.95
+class NAGConfig(MomentumConfig):
+  lr : float = 3E-4
+  momentum : float = 0.99
+  dampening : float = 0.05
+  weight_decay : float = 0.
+  nesterov : bool = True
 
-class Momentum(BaseOptimizer):
-  
-  def __init__(self, params, config : MomentumConfig = MomentumConfig()):
-    if not config.momentum:
-      raise ValueError(f"Invalid value for momentum in config: {config.momentum} ", 
-                       "Value must be True")
+class NAG(Momentum):
+  def __init__ (self, params, config : NAGConfig = NAGConfig()):
     super().__init__(params, config)
-    self.config = config
+    self.config = config
+
```

### Comparing `nadir-0.0.3/src/nadir/radam.py` & `nadir-0.1.0/src/nadir/radam.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,25 +20,23 @@
 from .base import BaseOptimizer
 from .base import BaseConfig
 
 
 __all__ = ['RadamConfig', 'Radam']
 
 @dataclass
-class RadamConfig(BaseConfig):
+class RadamConfig(AdamConfig):
   lr : float = 3E-4
-  momentum : bool = True
-  adaptive : bool = True
   beta_1 : float = 0.9
   beta_2 : float = 0.99
   eps : float = 1E-8
   weight_decay : float = 0.
 
-class Radam(BaseOptimizer):
-  def __init__ (self, params, config : RadamConfig = RadamConfig()):
+class Radam(Adam):
+  def __init__ (self, params, config : LionConfig = LionConfig()):
     super().__init__(params, config)
     self.config = config
 
   def update(self, state, group, grad, param):
     lr = group['lr']
     beta_2 = self.config.beta_2
     step = state['step']
```

### Comparing `nadir-0.0.3/src/nadir/rmsprop.py` & `nadir-0.1.0/src/nadir/rmsprop.py`

 * *Files identical despite different names*

### Comparing `nadir-0.0.3/src/nadir.egg-info/PKG-INFO` & `nadir-0.1.0/src/nadir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadir
-Version: 0.0.3
+Version: 0.1.0
 Summary: Nadir is a library of bleeding-edge DL optimisers built for speed and functionality in PyTorch for researchers
 Author-email: Bhavnick Minhas <bhavnicksm@gmail.com>
 Maintainer-email: Bhavnick Minhas <bhavnicksm@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/Dawn-Of-Eve/nadir
 Project-URL: Bug Tracker, https://github.com/Dawn-Of-Eve/nadir/issues
 Keywords: machine learning,optimization,adam-optimizer
@@ -73,21 +73,22 @@
 
 # Supported Optimisers
 
 | Optimiser 	| Paper 	                                            |
 |:---------:	|:-----:	                                            |
 |  **SGD**  	| https://paperswithcode.com/method/sgd                 |
 |  **Momentum** | https://paperswithcode.com/method/sgd-with-momentum   |
+|  **NAG**      | https://jlmelville.github.io/mize/nesterov.html       |
 |  **Adagrad** 	| https://www.jmlr.org/papers/volume12/duchi11a/duchi11a.pdf |
 |  **RMSProp** 	| https://paperswithcode.com/method/rmsprop             |
 |  **Adam**     | https://arxiv.org/abs/1412.6980v9                     |
 |  **Adamax**   | https://arxiv.org/abs/1412.6980v9                     |
 |  **AdamW**    | https://arxiv.org/abs/1711.05101v3                    |
 |  **Adadelta** | https://arxiv.org/abs/1212.5701v1                     |
-|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                    |
+|  **AMSGrad**    | https://arxiv.org/abs/1904.09237v1                  |
 |  **RAdam**    | https://arxiv.org/abs/1908.03265v4                    |
 |  **Lion**     | https://arxiv.org/abs/2302.06675                      |
 
 # Acknowledgements
 
 We would like to thank all the amazing contributors of this project who spent so much effort making this repositary awesome! :heart:
```

