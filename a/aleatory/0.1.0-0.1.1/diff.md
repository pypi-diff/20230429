# Comparing `tmp/aleatory-0.1.0.tar.gz` & `tmp/aleatory-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/dialidsantiago/Git/aleatory/dist/.tmp-l8yxxjb2/aleatory-0.1.0.tar", last modified: Mon Dec 26 11:18:43 2022, max compression
+gzip compressed data, was "/Users/dialidsantiago/Git/aleatory/dist/.tmp-h19m8qhs/aleatory-0.1.1.tar", last modified: Sat Apr 29 15:48:20 2023, max compression
```

## Comparing `aleatory-0.1.0.tar` & `aleatory-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.076625 aleatory-0.1.0/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1067 2022-12-23 20:21:22.000000 aleatory-0.1.0/LICENSE
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3169 2022-12-26 11:18:43.076299 aleatory-0.1.0/PKG-INFO
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     2438 2022-12-26 11:12:35.000000 aleatory-0.1.0/README.md
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.065219 aleatory-0.1.0/aleatory/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.0/aleatory/__init__.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.069540 aleatory-0.1.0/aleatory/processes/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      412 2022-12-23 20:21:22.000000 aleatory-0.1.0/aleatory/processes/__init__.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.072110 aleatory-0.1.0/aleatory/processes/analytical/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.0/aleatory/processes/analytical/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5632 2022-12-25 12:21:22.000000 aleatory-0.1.0/aleatory/processes/analytical/brownian_motion.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     2064 2022-12-23 20:21:22.000000 aleatory-0.1.0/aleatory/processes/analytical/gaussian.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5062 2022-12-25 17:41:15.000000 aleatory-0.1.0/aleatory/processes/analytical/geometric_brownian.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     6045 2022-12-24 11:17:49.000000 aleatory-0.1.0/aleatory/processes/base.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.074722 aleatory-0.1.0/aleatory/processes/euler_maruyama/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.0/aleatory/processes/euler_maruyama/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     5189 2022-12-24 23:32:25.000000 aleatory-0.1.0/aleatory/processes/euler_maruyama/cev_process.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4412 2022-12-25 18:17:39.000000 aleatory-0.1.0/aleatory/processes/euler_maruyama/cir_process.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1638 2022-12-25 18:20:27.000000 aleatory-0.1.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3320 2022-12-25 17:42:46.000000 aleatory-0.1.0/aleatory/processes/euler_maruyama/vasicek.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.075607 aleatory-0.1.0/aleatory/utils/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.0/aleatory/utils/__init__.py
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     4456 2022-12-24 11:24:19.000000 aleatory-0.1.0/aleatory/utils/utils.py
-drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2022-12-26 11:18:43.068229 aleatory-0.1.0/aleatory.egg-info/
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     3169 2022-12-26 11:18:43.000000 aleatory-0.1.0/aleatory.egg-info/PKG-INFO
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      751 2022-12-26 11:18:43.000000 aleatory-0.1.0/aleatory.egg-info/SOURCES.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        1 2022-12-26 11:18:43.000000 aleatory-0.1.0/aleatory.egg-info/dependency_links.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)      100 2022-12-26 11:18:43.000000 aleatory-0.1.0/aleatory.egg-info/requires.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)        9 2022-12-26 11:18:43.000000 aleatory-0.1.0/aleatory.egg-info/top_level.txt
--rw-r--r--   0 dialidsantiago   (501) staff       (20)     1014 2022-12-26 11:14:38.000000 aleatory-0.1.0/pyproject.toml
--rw-r--r--   0 dialidsantiago   (501) staff       (20)       38 2022-12-26 11:18:43.076726 aleatory-0.1.0/setup.cfg
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.598162 aleatory-0.1.1/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1067 2022-12-23 20:21:22.000000 aleatory-0.1.1/LICENSE
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3717 2023-04-29 15:48:20.597830 aleatory-0.1.1/PKG-INFO
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2992 2023-04-29 09:39:58.000000 aleatory-0.1.1/README.md
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.584616 aleatory-0.1.1/aleatory/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.1/aleatory/__init__.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.587462 aleatory-0.1.1/aleatory/processes/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      412 2022-12-23 20:21:22.000000 aleatory-0.1.1/aleatory/processes/__init__.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.589796 aleatory-0.1.1/aleatory/processes/analytical/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.1/aleatory/processes/analytical/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5723 2023-04-29 10:34:18.000000 aleatory-0.1.1/aleatory/processes/analytical/brownian_motion.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     2064 2022-12-23 20:21:22.000000 aleatory-0.1.1/aleatory/processes/analytical/gaussian.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5062 2022-12-25 17:41:15.000000 aleatory-0.1.1/aleatory/processes/analytical/geometric_brownian.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     6373 2023-04-29 10:50:35.000000 aleatory-0.1.1/aleatory/processes/base.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.593418 aleatory-0.1.1/aleatory/processes/euler_maruyama/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.1/aleatory/processes/euler_maruyama/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     5260 2023-04-29 10:54:19.000000 aleatory-0.1.1/aleatory/processes/euler_maruyama/cev_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4412 2022-12-25 18:17:39.000000 aleatory-0.1.1/aleatory/processes/euler_maruyama/cir_process.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1638 2022-12-25 18:20:27.000000 aleatory-0.1.1/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3316 2023-04-29 09:43:08.000000 aleatory-0.1.1/aleatory/processes/euler_maruyama/vasicek.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.594474 aleatory-0.1.1/aleatory/utils/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        0 2022-12-23 20:21:22.000000 aleatory-0.1.1/aleatory/utils/__init__.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     4470 2023-04-29 10:48:23.000000 aleatory-0.1.1/aleatory/utils/utils.py
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.586329 aleatory-0.1.1/aleatory.egg-info/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3717 2023-04-29 15:48:20.000000 aleatory-0.1.1/aleatory.egg-info/PKG-INFO
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      836 2023-04-29 15:48:20.000000 aleatory-0.1.1/aleatory.egg-info/SOURCES.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        1 2023-04-29 15:48:20.000000 aleatory-0.1.1/aleatory.egg-info/dependency_links.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      100 2023-04-29 15:48:20.000000 aleatory-0.1.1/aleatory.egg-info/requires.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)        9 2023-04-29 15:48:20.000000 aleatory-0.1.1/aleatory.egg-info/top_level.txt
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     1008 2023-04-29 15:41:27.000000 aleatory-0.1.1/pyproject.toml
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)       38 2023-04-29 15:48:20.598272 aleatory-0.1.1/setup.cfg
+drwxr-xr-x   0 dialidsantiago   (501) staff       (20)        0 2023-04-29 15:48:20.596987 aleatory-0.1.1/tests/
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)     3976 2023-04-29 10:57:17.000000 aleatory-0.1.1/tests/test_charts.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      709 2022-12-25 12:22:36.000000 aleatory-0.1.1/tests/test_marginal_functions.py
+-rw-r--r--   0 dialidsantiago   (501) staff       (20)      258 2022-12-25 12:07:25.000000 aleatory-0.1.1/tests/test_transormation_em.py
```

### Comparing `aleatory-0.1.0/LICENSE` & `aleatory-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aleatory-0.1.0/PKG-INFO` & `aleatory-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: aleatory
-Version: 0.1.0
-Summary: Stochastic Processes Simulation and Visualisation
-Author-email: Dialid Santiago <d.santiago@outlook.com>
-Project-URL: Homepage, https://github.com/quantgirluk/aleatory
-Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
-Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: <3.11,>=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # *aleatory*
 
-![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest) [![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/)
+[![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/) [![Downloads](https://static.pepy.tech/personalized-badge/aleatory?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aleatory)
+
+![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest) 
+
+
 
 
 - [Git Homepage](https://github.com/quantgirluk/aleatory)
 - [Pip Repository](https://pypi.org/project/aleatory/)
 - [Documentation](https://aleatory.readthedocs.io/en/latest/)
 
 
@@ -95,7 +82,19 @@
 <figure>
   <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"
     width="900" height="450">
 </figure>
 
 
 For more example visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
+
+## Thanks for Visiting! ✨
+
+Connect with me via:
+
+- 🦜 [Twitter](https://twitter.com/Quant_Girl)
+- 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
+- 📸 [Instagram](https://www.instagram.com/quant_girl/)
+- 👾 [Personal Website](https://quantgirl.blog)
+
+
+⭐️ **If you like this projet, please give it a star!** ⭐️
```

### Comparing `aleatory-0.1.0/README.md` & `aleatory-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,31 @@
+Metadata-Version: 2.1
+Name: aleatory
+Version: 0.1.1
+Summary: Stochastic Processes Simulation and Visualisation
+Author-email: Dialid Santiago <d.santiago@outlook.com>
+Project-URL: Homepage, https://github.com/quantgirluk/aleatory
+Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
+Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # *aleatory*
 
-![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest) [![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/)
+[![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/) [![Downloads](https://static.pepy.tech/personalized-badge/aleatory?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aleatory)
+
+![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest) 
+
+
 
 
 - [Git Homepage](https://github.com/quantgirluk/aleatory)
 - [Pip Repository](https://pypi.org/project/aleatory/)
 - [Documentation](https://aleatory.readthedocs.io/en/latest/)
 
 
@@ -78,7 +99,19 @@
 <figure>
   <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"
     width="900" height="450">
 </figure>
 
 
 For more example visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
+
+## Thanks for Visiting! ✨
+
+Connect with me via:
+
+- 🦜 [Twitter](https://twitter.com/Quant_Girl)
+- 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
+- 📸 [Instagram](https://www.instagram.com/quant_girl/)
+- 👾 [Personal Website](https://quantgirl.blog)
+
+
+⭐️ **If you like this projet, please give it a star!** ⭐️
```

### Comparing `aleatory-0.1.0/aleatory/processes/analytical/brownian_motion.py` & `aleatory-0.1.1/aleatory/processes/analytical/brownian_motion.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,34 +143,35 @@
         stds = self._process_stds()
         return stds
 
     def get_marginal(self, t):
         marginal = norm(loc=self.drift * t, scale=self.scale * np.sqrt(t))
         return marginal
 
-    def draw(self, n, N, marginal=True, envelope=False, type='3sigma', **fig_kw):
+    def draw(self, n, N, marginal=True, envelope=False, type='3sigma', title=None, **fig_kw):
         """
         Simulates and plots paths/trajectories from the instanced stochastic process.
 
         Produces different kind of visualisation illustrating the following elements:
 
         - times versus process values as lines
         - the expectation of the process across time
         - histogram showing the empirical marginal distribution :math:`X_T` (optional when ``marginal = True``)
         - probability density function of the marginal distribution :math:`X_T` (optional when ``marginal = True``)
-        - envelope of confidence intervals acroos time (optional when ``envelope = True``)
+        - envelope of confidence intervals across time (optional when ``envelope = True``)
 
 
         :param n: number of steps in each path
         :param N: number of paths to simulate
         :param marginal: bool, default: True
         :param envelope: bool, default: False
         :param type: string, default: '3sigma'
+        :param title: string to customise plot title
         :return:
         """
 
         if type == '3sigma':
-            return self._draw_3sigmastyle(n=n, N=N, marginal=marginal, envelope=envelope, **fig_kw)
+            return self._draw_3sigmastyle(n=n, N=N, marginal=marginal, envelope=envelope, title=title, **fig_kw)
         elif type == 'qq':
-            return self._draw_qqstyle(n, N, marginal=marginal, envelope=envelope, **fig_kw)
+            return self._draw_qqstyle(n, N, marginal=marginal, envelope=envelope, title=title, **fig_kw)
         else:
             raise ValueError
```

### Comparing `aleatory-0.1.0/aleatory/processes/analytical/gaussian.py` & `aleatory-0.1.1/aleatory/processes/analytical/gaussian.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.1.0/aleatory/processes/analytical/geometric_brownian.py` & `aleatory-0.1.1/aleatory/processes/analytical/geometric_brownian.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.1.0/aleatory/processes/base.py` & `aleatory-0.1.1/aleatory/processes/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,28 +88,32 @@
     def _process_variance(self):
         pass
 
     @abstractmethod
     def _process_stds(self):
         pass
 
-    def plot(self, n, N, **fig_kw):
+    def plot(self, n, N, title=None, **fig_kw):
         """
         Simulates and plots paths/trajectories from the instanced stochastic process.
         Simple plot of times versus process values as lines and/or markers.
 
         :param n: number of steps in each path
         :param N: number of paths to simulate
+        :param title: string to customise plot title
         :return:
         """
         self.simulate(n, N)
-        figure = plot_paths(self.times, self.paths, self.name, **fig_kw)
+        if title:
+            figure = plot_paths(self.times, self.paths, title=title, **fig_kw)
+        else:
+            figure = plot_paths(self.times, self.paths, title=self.name, **fig_kw)
         return figure
 
-    def _draw_paths(self, n, N, marginal=False, envelope=False, type=None, **fig_kw):
+    def _draw_paths(self, n, N, marginal=False, envelope=False, type=None, title=None, **fig_kw):
         self.simulate(n, N)
         expectations = self._process_expectation()
 
         if envelope:
             if type == '3sigma':
                 stds = self._process_stds()
                 upper = expectations + 3.0 * stds
@@ -123,31 +127,32 @@
             lower = None
 
         if marginal:
             marginalT = self.get_marginal(self.T)
         else:
             marginalT = None
 
-        fig = draw_paths(times=self.times, paths=self.paths, N=N, expectations=expectations, name=self.name,
+        chart_title = title if title else self.name
+        fig = draw_paths(times=self.times, paths=self.paths, N=N, title=chart_title, expectations=expectations,
                          marginal=marginal, marginalT=marginalT, envelope=envelope, lower=lower, upper=upper,
                          **fig_kw)
         return fig
 
-    def _draw_qqstyle(self, n, N, marginal=False, envelope=False,
+    def _draw_qqstyle(self, n, N, marginal=False, envelope=False, title=None,
                       **fig_kw):
 
-        fig = self._draw_paths(n=n, N=N, marginal=marginal, envelope=envelope, type='qq', **fig_kw)
+        fig = self._draw_paths(n=n, N=N, marginal=marginal, envelope=envelope, type='qq', title=title, **fig_kw)
         return fig
 
-    def _draw_3sigmastyle(self, n, N, marginal=False, envelope=False, **fig_kw):
+    def _draw_3sigmastyle(self, n, N, marginal=False, envelope=False, title=None, **fig_kw):
 
-        fig = self._draw_paths(n=n, N=N, marginal=marginal, envelope=envelope, type='3sigma', **fig_kw)
+        fig = self._draw_paths(n=n, N=N, marginal=marginal, envelope=envelope, type='3sigma', title=title, **fig_kw)
         return fig
 
-    def draw(self, n, N, marginal=True, envelope=False, **fig_kw):
+    def draw(self, n, N, marginal=True, envelope=False, title=None, **fig_kw):
         """
         Simulates and plots paths/trajectories from the instanced stochastic process.
         Visualisation shows
         - times versus process values as lines
         - the expectation of the process across time
         - histogram showing the empirical marginal distribution :math:`X_T`
         - probability density function of the marginal distribution :math:`X_T`
@@ -155,15 +160,15 @@
 
         :param n: number of steps in each path
         :param N: number of paths to simulate
         :param marginal: bool, default: True
         :param envelope: bool, default: False
         :return:
         """
-        return self._draw_qqstyle(n, N, marginal=marginal, envelope=envelope, **fig_kw)
+        return self._draw_qqstyle(n, N, marginal=marginal, envelope=envelope, title=title, **fig_kw)
 
 
 class SPEulerMaruyama(SPExplicit):
     def __int__(self, f=None, g=None, initial=0.0, T=1.0, rng=None):
         super().__init__(T=T, rng=rng, initial=initial)
         self.f = f
         self.g = g
```

### Comparing `aleatory-0.1.0/aleatory/processes/euler_maruyama/cev_process.py` & `aleatory-0.1.1/aleatory/processes/euler_maruyama/cev_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,30 +135,32 @@
         stds = np.sqrt(self.process_variance())
         return stds
 
     def process_stds(self):
         stds = self._process_stds()
         return stds
 
-    def draw(self, n, N, marginal=True, envelope=False, **fig_kw):
+    def draw(self, n, N, marginal=True, envelope=False, title=None, **fig_kw):
         self.simulate(n, N)
         expectations = self.estimate_expectations()
 
         if envelope:
             lower = self.estimate_quantiles(0.005)
             upper = self.estimate_quantiles(0.995)
         else:
             lower = None
             upper = None
 
+        chart_title = title if title else self.name
+
         if marginal:
-            fig = draw_paths(times=self.times, paths=self.paths, N=N, KDE=True, name=self.name, marginal=marginal,
+            fig = draw_paths(times=self.times, paths=self.paths, N=N, title=chart_title, KDE=True, marginal=marginal,
                              expectations=expectations, envelope=envelope, lower=lower, upper=upper,
                              **fig_kw)
         else:
-            fig = draw_paths(times=self.times, paths=self.paths, N=N, name=self.name,
+            fig = draw_paths(times=self.times, paths=self.paths, N=N, title=chart_title,
                              expectations=expectations, marginal=marginal, **fig_kw)
 
         return fig
 
     def sample(self, n):
         return self._sample_em_process(n, log=True)
```

### Comparing `aleatory-0.1.0/aleatory/processes/euler_maruyama/cir_process.py` & `aleatory-0.1.1/aleatory/processes/euler_maruyama/cir_process.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.1.0/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py` & `aleatory-0.1.1/aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py`

 * *Files identical despite different names*

### Comparing `aleatory-0.1.0/aleatory/processes/euler_maruyama/vasicek.py` & `aleatory-0.1.1/aleatory/processes/euler_maruyama/vasicek.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,17 +64,17 @@
         return "Vasicek process with parameters {speed}, {mean}, and {volatility} on [0, {T}].".format(
             T=str(self.T), speed=str(self.theta), mean=str(self.mu), volatility=str(self.sigma))
 
     def _process_expectation(self, times=None):
         if times is None:
             times = self.times
         return self.initial * np.exp((-1.0) * self.theta * times) + self.mu * (
-                np.ones(len(times)) - np.exp((-1.0) * self.theta * self.times))
+                np.ones(len(times)) - np.exp((-1.0) * self.theta * times))
 
-    def process_expectation(self, times=None):
+    def marginal_expectation(self, times=None):
         expectations = self._process_expectation(times=times)
         return expectations
 
     def _process_variance(self,times=None):
         if times is None:
             times = self.times
         variances = (self.sigma ** 2) * (1.0 / (2.0 * self.theta)) * (
```

### Comparing `aleatory-0.1.0/aleatory/utils/utils.py` & `aleatory-0.1.1/aleatory/utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,27 +42,27 @@
 
 
 def times_to_increments(times):
     """Ensure a positive, monotonically increasing sequence."""
     return check_increments(times)
 
 
-def plot_paths(times, paths, name, style="seaborn-v0_8-whitegrid", **fig_kw):
+def plot_paths(times, paths, style="seaborn-v0_8-whitegrid", title=None, **fig_kw):
     with plt.style.context(style):
         fig, ax = plt.subplots(**fig_kw)
         for p in paths:
             ax.plot(times, p)
-        ax.set_title(name)
+        ax.set_title(title)
         ax.set_xlabel('$t$')
         ax.set_ylabel('$X(t)$')
         plt.show()
     return fig
 
 
-def draw_paths(times, paths, N, expectations, name, KDE=False, marginal=False, marginalT=None, envelope=False,
+def draw_paths(times, paths, N, expectations, title=None, KDE=False, marginal=False, marginalT=None, envelope=False,
                lower=None, upper=None, style="seaborn-v0_8-whitegrid", colormap="RdYlBu_r", **fig_kw):
     with plt.style.context(style):
         if marginal:
             fig = plt.figure(**fig_kw)
             gs = GridSpec(1, 5)
             ax1 = fig.add_subplot(gs[:4])
             ax2 = fig.add_subplot(gs[4:], sharey=ax1)
@@ -105,15 +105,15 @@
             fig, ax1 = plt.subplots(**fig_kw)
             for i in range(N):
                 ax1.plot(times, paths[i], '-', lw=1.0)
             ax1.plot(times, expectations, '--', lw=1.75, label='$E[X_t]$')
             if envelope:
                 ax1.fill_between(times, upper, lower, color='grey', alpha=0.25)
 
-        fig.suptitle(name)
+        fig.suptitle(title)
         ax1.set_title('Simulated Paths $X_t, t \in [t_0, T]$')  # Title
         ax1.set_xlabel('t')
         ax1.set_ylabel('X(t)')
         ax1.legend()
         plt.show()
 
     return fig
```

### Comparing `aleatory-0.1.0/aleatory.egg-info/PKG-INFO` & `aleatory-0.1.1/aleatory.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: aleatory
-Version: 0.1.0
+Version: 0.1.1
 Summary: Stochastic Processes Simulation and Visualisation
 Author-email: Dialid Santiago <d.santiago@outlook.com>
 Project-URL: Homepage, https://github.com/quantgirluk/aleatory
 Project-URL: Bug Tracker, https://github.com/quantgirluk/aleatory/issues
 Project-URL: Documentation, https://aleatory.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # *aleatory*
 
-![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest) [![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/)
+[![PyPI version fury.io](https://badge.fury.io/py/aleatory.svg)](https://pypi.org/project/aleatory/) [![Downloads](https://static.pepy.tech/personalized-badge/aleatory?period=total&units=international_system&left_color=black&right_color=blue&left_text=Downloads)](https://pepy.tech/project/aleatory)
+
+![example workflow](https://github.com/quantgirluk/aleatory/actions/workflows/python-package.yml/badge.svg) [![Documentation Status](https://readthedocs.org/projects/aleatory/badge/?version=latest)](https://aleatory.readthedocs.io/en/latest/?badge=latest) 
+
+
 
 
 - [Git Homepage](https://github.com/quantgirluk/aleatory)
 - [Pip Repository](https://pypi.org/project/aleatory/)
 - [Documentation](https://aleatory.readthedocs.io/en/latest/)
 
 
@@ -95,7 +99,19 @@
 <figure>
   <p><img src="https://raw.githubusercontent.com/quantgirluk/aleatory/main/docs/source/_static/brownian_motion_quickstart_08.png"
     width="900" height="450">
 </figure>
 
 
 For more example visit the [Quick-Start Guide](https://aleatory.readthedocs.io/en/latest/general.html).
+
+## Thanks for Visiting! ✨
+
+Connect with me via:
+
+- 🦜 [Twitter](https://twitter.com/Quant_Girl)
+- 👩🏽‍💼 [Linkedin](https://www.linkedin.com/in/dialidsantiago/)
+- 📸 [Instagram](https://www.instagram.com/quant_girl/)
+- 👾 [Personal Website](https://quantgirl.blog)
+
+
+⭐️ **If you like this projet, please give it a star!** ⭐️
```

### Comparing `aleatory-0.1.0/aleatory.egg-info/SOURCES.txt` & `aleatory-0.1.1/aleatory.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 aleatory/processes/analytical/geometric_brownian.py
 aleatory/processes/euler_maruyama/__init__.py
 aleatory/processes/euler_maruyama/cev_process.py
 aleatory/processes/euler_maruyama/cir_process.py
 aleatory/processes/euler_maruyama/ornstein_uhlenbeck.py
 aleatory/processes/euler_maruyama/vasicek.py
 aleatory/utils/__init__.py
-aleatory/utils/utils.py
+aleatory/utils/utils.py
+tests/test_charts.py
+tests/test_marginal_functions.py
+tests/test_transormation_em.py
```

### Comparing `aleatory-0.1.0/pyproject.toml` & `aleatory-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aleatory"
-version = "0.1.0"
+version = "0.1.1"
 authors = [{ name = "Dialid Santiago", email = "d.santiago@outlook.com" }, ]
 description = "Stochastic Processes Simulation and Visualisation"
 readme = "README.md"
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.8"
 dependencies = ["pandas>=1.5.2",
                 "numpy>=1.23.5",
                 "scipy>=1.9.3",
                 "matplotlib>=3.6.2",
                 "statsmodels>=0.13.5",
                 "parameterized>=0.8.1"
                 ]
```

