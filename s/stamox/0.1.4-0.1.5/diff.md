# Comparing `tmp/stamox-0.1.4.tar.gz` & `tmp/stamox-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stamox-0.1.4.tar", last modified: Tue Apr 25 06:23:38 2023, max compression
+gzip compressed data, was "stamox-0.1.5.tar", last modified: Sat Apr 29 07:01:07 2023, max compression
```

## Comparing `stamox-0.1.4.tar` & `stamox-0.1.5.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.370901 stamox-0.1.4/
--rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.4/LICENCE
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4837 2023-04-25 06:23:38.370709 stamox-0.1.4/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4513 2023-04-25 03:32:49.000000 stamox-0.1.4/README.md
--rw-r--r--   0 jiayaobo   (501) staff       (20)      328 2023-04-20 16:25:17.000000 stamox-0.1.4/pyproject.toml
--rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-25 06:23:38.370946 stamox-0.1.4/setup.cfg
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1132 2023-04-23 12:15:32.000000 stamox-0.1.4/setup.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.361268 stamox-0.1.4/stamox/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1224 2023-04-24 15:12:30.000000 stamox-0.1.4/stamox/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.362090 stamox-0.1.4/stamox/anova/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       58 2023-04-20 08:53:58.000000 stamox-0.1.4/stamox/anova/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.362359 stamox-0.1.4/stamox/anova/one_way/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.4/stamox/anova/one_way/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4549 2023-04-25 06:17:29.000000 stamox-0.1.4/stamox/anova/one_way/_aov.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      933 2023-04-25 06:11:55.000000 stamox-0.1.4/stamox/basic.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.362632 stamox-0.1.4/stamox/cluster/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/cluster/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5146 2023-04-25 06:15:24.000000 stamox-0.1.4/stamox/cluster/_kmeans.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.363578 stamox-0.1.4/stamox/core/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      640 2023-04-20 08:51:36.000000 stamox-0.1.4/stamox/core/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      154 2023-04-24 15:15:40.000000 stamox-0.1.4/stamox/core/_func_state.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2958 2023-04-24 03:39:07.000000 stamox-0.1.4/stamox/core/base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1670 2023-04-23 12:16:09.000000 stamox-0.1.4/stamox/core/better_partial.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2805 2023-04-24 15:14:50.000000 stamox-0.1.4/stamox/core/jit.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7183 2023-04-25 03:29:46.000000 stamox-0.1.4/stamox/core/maps.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6442 2023-04-25 03:29:11.000000 stamox-0.1.4/stamox/core/pipe.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.364151 stamox-0.1.4/stamox/correlation/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      131 2023-04-17 09:53:48.000000 stamox-0.1.4/stamox/correlation/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1234 2023-04-24 15:32:33.000000 stamox-0.1.4/stamox/correlation/_cor.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1947 2023-04-24 15:32:24.000000 stamox-0.1.4/stamox/correlation/_pearson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2175 2023-04-24 15:32:18.000000 stamox-0.1.4/stamox/correlation/_spearman.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.366520 stamox-0.1.4/stamox/distribution/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1824 2023-04-16 10:53:49.000000 stamox-0.1.4/stamox/distribution/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6296 2023-04-24 15:24:08.000000 stamox-0.1.4/stamox/distribution/_beta.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6218 2023-04-24 15:23:53.000000 stamox-0.1.4/stamox/distribution/_binomial.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6675 2023-04-24 15:24:23.000000 stamox-0.1.4/stamox/distribution/_cauchy.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5069 2023-04-24 15:24:56.000000 stamox-0.1.4/stamox/distribution/_chisq.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2176 2023-04-21 13:54:17.000000 stamox-0.1.4/stamox/distribution/_ecdf.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5827 2023-04-21 13:57:31.000000 stamox-0.1.4/stamox/distribution/_exp.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6211 2023-04-21 14:02:56.000000 stamox-0.1.4/stamox/distribution/_f.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6522 2023-04-24 15:25:41.000000 stamox-0.1.4/stamox/distribution/_gamma.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7011 2023-04-24 15:25:50.000000 stamox-0.1.4/stamox/distribution/_laplace.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7373 2023-04-24 15:26:12.000000 stamox-0.1.4/stamox/distribution/_normal.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6365 2023-04-22 03:02:59.000000 stamox-0.1.4/stamox/distribution/_pareto.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     5787 2023-04-24 15:28:25.000000 stamox-0.1.4/stamox/distribution/_poisson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7219 2023-04-22 03:11:38.000000 stamox-0.1.4/stamox/distribution/_t.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6272 2023-04-22 03:15:15.000000 stamox-0.1.4/stamox/distribution/_uniform.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1511 2023-04-22 03:21:20.000000 stamox-0.1.4/stamox/distribution/_utils.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6922 2023-04-24 15:29:30.000000 stamox-0.1.4/stamox/distribution/_weibull.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.366677 stamox-0.1.4/stamox/experimental/
--rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-20 08:52:04.000000 stamox-0.1.4/stamox/experimental/__init__.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.366989 stamox-0.1.4/stamox/experimental/decomposition/
--rw-r--r--   0 jiayaobo   (501) staff       (20)       74 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/decomposition/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1617 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/decomposition/_pca.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.367425 stamox-0.1.4/stamox/experimental/maps/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/maps/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/maps/auto_map.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/experimental/maps/cube_map.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.367726 stamox-0.1.4/stamox/formula/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/formula/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1556 2023-04-21 12:35:01.000000 stamox-0.1.4/stamox/formula/_formula.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2490 2023-04-25 06:12:34.000000 stamox-0.1.4/stamox/functions.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.368458 stamox-0.1.4/stamox/hypothesis/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      427 2023-04-21 10:11:31.000000 stamox-0.1.4/stamox/hypothesis/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2535 2023-04-24 15:30:51.000000 stamox-0.1.4/stamox/hypothesis/_bartlett.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      923 2023-04-19 05:36:05.000000 stamox-0.1.4/stamox/hypothesis/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2282 2023-04-24 15:31:15.000000 stamox-0.1.4/stamox/hypothesis/_durbin_watson.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2736 2023-04-24 15:31:44.000000 stamox-0.1.4/stamox/hypothesis/_friedman.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.368874 stamox-0.1.4/stamox/math/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/math/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1243 2023-04-21 12:41:38.000000 stamox-0.1.4/stamox/math/combination.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1497 2023-04-21 06:19:17.000000 stamox-0.1.4/stamox/math/special.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     6771 2023-04-25 03:43:41.000000 stamox-0.1.4/stamox/pipe_functions.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.369457 stamox-0.1.4/stamox/regression/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/regression/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2150 2023-04-14 07:26:13.000000 stamox-0.1.4/stamox/regression/_base.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     7260 2023-04-24 15:30:13.000000 stamox-0.1.4/stamox/regression/_lm.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.369933 stamox-0.1.4/stamox/sample/
--rw-r--r--   0 jiayaobo   (501) staff       (20)      228 2023-04-19 05:08:41.000000 stamox-0.1.4/stamox/sample/__init__.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     2719 2023-04-25 06:18:28.000000 stamox-0.1.4/stamox/sample/_bootstrap.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1741 2023-04-25 06:18:12.000000 stamox-0.1.4/stamox/sample/_jackknife.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1803 2023-04-25 06:18:39.000000 stamox-0.1.4/stamox/transformation.py
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.361944 stamox-0.1.4/stamox.egg-info/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     4837 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/PKG-INFO
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1957 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/SOURCES.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/dependency_links.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)      399 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/requires.txt
--rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-25 06:23:38.000000 stamox-0.1.4/stamox.egg-info/top_level.txt
-drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-25 06:23:38.370462 stamox-0.1.4/tests/
--rw-r--r--   0 jiayaobo   (501) staff       (20)     1463 2023-04-25 06:13:09.000000 stamox-0.1.4/tests/test_basic.py
--rw-r--r--   0 jiayaobo   (501) staff       (20)      871 2023-04-24 15:10:59.000000 stamox-0.1.4/tests/test_transformation.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.608994 stamox-0.1.5/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)    11356 2023-03-21 16:33:35.000000 stamox-0.1.5/LICENCE
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4827 2023-04-29 07:01:07.608846 stamox-0.1.5/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4503 2023-04-26 02:48:10.000000 stamox-0.1.5/README.md
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      344 2023-04-29 06:54:47.000000 stamox-0.1.5/pyproject.toml
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       38 2023-04-29 07:01:07.609029 stamox-0.1.5/setup.cfg
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1132 2023-04-29 06:53:58.000000 stamox-0.1.5/setup.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.592231 stamox-0.1.5/stamox/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1224 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.593198 stamox-0.1.5/stamox/anova/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       58 2023-04-20 08:53:58.000000 stamox-0.1.5/stamox/anova/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.593813 stamox-0.1.5/stamox/anova/one_way/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       56 2023-03-28 10:30:27.000000 stamox-0.1.5/stamox/anova/one_way/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     3371 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/anova/one_way/_aov.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      933 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/basic.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.594355 stamox-0.1.5/stamox/cluster/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       90 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/cluster/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5146 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/cluster/_kmeans.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.599407 stamox-0.1.5/stamox/core/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      640 2023-04-20 08:51:36.000000 stamox-0.1.5/stamox/core/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      154 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/core/_func_state.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2958 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/core/base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1670 2023-04-23 12:16:09.000000 stamox-0.1.5/stamox/core/better_partial.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2805 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/core/jit.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7183 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/core/maps.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6442 2023-04-29 06:59:04.000000 stamox-0.1.5/stamox/core/pipe.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.600144 stamox-0.1.5/stamox/correlation/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      131 2023-04-17 09:53:48.000000 stamox-0.1.5/stamox/correlation/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1234 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/correlation/_cor.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1947 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/correlation/_pearson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2175 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/correlation/_spearman.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.600524 stamox-0.1.5/stamox/decomposition/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)       84 2023-04-27 11:40:39.000000 stamox-0.1.5/stamox/decomposition/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2583 2023-04-27 11:40:39.000000 stamox-0.1.5/stamox/decomposition/_pca.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.603265 stamox-0.1.5/stamox/distribution/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1824 2023-04-16 10:53:49.000000 stamox-0.1.5/stamox/distribution/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6198 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_beta.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6116 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_binomial.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6579 2023-04-29 06:52:53.000000 stamox-0.1.5/stamox/distribution/_cauchy.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4969 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_chisq.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2176 2023-04-21 13:54:17.000000 stamox-0.1.5/stamox/distribution/_ecdf.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5693 2023-04-29 06:52:18.000000 stamox-0.1.5/stamox/distribution/_exp.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6113 2023-04-29 06:52:14.000000 stamox-0.1.5/stamox/distribution/_f.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6386 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_gamma.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6873 2023-04-29 06:52:43.000000 stamox-0.1.5/stamox/distribution/_laplace.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7237 2023-04-29 06:52:26.000000 stamox-0.1.5/stamox/distribution/_normal.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6264 2023-04-29 06:52:29.000000 stamox-0.1.5/stamox/distribution/_pareto.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     5693 2023-04-29 06:52:33.000000 stamox-0.1.5/stamox/distribution/_poisson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     7132 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_t.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6138 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_uniform.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1820 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_utils.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6828 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/distribution/_weibull.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.603616 stamox-0.1.5/stamox/experimental/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-20 08:52:04.000000 stamox-0.1.5/stamox/experimental/__init__.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.604475 stamox-0.1.5/stamox/experimental/maps/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      108 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/experimental/maps/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1254 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/experimental/maps/auto_map.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      622 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/experimental/maps/cube_map.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.604891 stamox-0.1.5/stamox/formula/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      100 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/formula/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1556 2023-04-21 12:35:01.000000 stamox-0.1.5/stamox/formula/_formula.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2542 2023-04-27 11:40:39.000000 stamox-0.1.5/stamox/functions.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.605857 stamox-0.1.5/stamox/hypothesis/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      427 2023-04-21 10:11:31.000000 stamox-0.1.5/stamox/hypothesis/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2591 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/hypothesis/_bartlett.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      923 2023-04-19 05:36:05.000000 stamox-0.1.5/stamox/hypothesis/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2304 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/hypothesis/_durbin_watson.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2800 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/hypothesis/_friedman.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.606492 stamox-0.1.5/stamox/math/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      172 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/math/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1243 2023-04-21 12:41:38.000000 stamox-0.1.5/stamox/math/combination.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1497 2023-04-21 06:19:17.000000 stamox-0.1.5/stamox/math/special.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     6888 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/pipe_functions.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.607351 stamox-0.1.5/stamox/regression/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      110 2023-04-14 07:26:13.000000 stamox-0.1.5/stamox/regression/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2158 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/regression/_base.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     9433 2023-04-29 06:52:04.000000 stamox-0.1.5/stamox/regression/_lm.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.608078 stamox-0.1.5/stamox/sample/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      228 2023-04-19 05:08:41.000000 stamox-0.1.5/stamox/sample/__init__.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     2722 2023-04-28 13:24:42.000000 stamox-0.1.5/stamox/sample/_bootstrap.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1744 2023-04-28 13:24:30.000000 stamox-0.1.5/stamox/sample/_jackknife.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1803 2023-04-26 02:48:10.000000 stamox-0.1.5/stamox/transformation.py
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.592962 stamox-0.1.5/stamox.egg-info/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     4827 2023-04-29 07:01:07.000000 stamox-0.1.5/stamox.egg-info/PKG-INFO
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1931 2023-04-29 07:01:07.000000 stamox-0.1.5/stamox.egg-info/SOURCES.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        1 2023-04-29 07:01:07.000000 stamox-0.1.5/stamox.egg-info/dependency_links.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      399 2023-04-29 07:01:07.000000 stamox-0.1.5/stamox.egg-info/requires.txt
+-rw-r--r--   0 jiayaobo   (501) staff       (20)        7 2023-04-29 07:01:07.000000 stamox-0.1.5/stamox.egg-info/top_level.txt
+drwxr-xr-x   0 jiayaobo   (501) staff       (20)        0 2023-04-29 07:01:07.608488 stamox-0.1.5/tests/
+-rw-r--r--   0 jiayaobo   (501) staff       (20)     1463 2023-04-26 02:48:10.000000 stamox-0.1.5/tests/test_basic.py
+-rw-r--r--   0 jiayaobo   (501) staff       (20)      871 2023-04-26 02:48:10.000000 stamox-0.1.5/tests/test_transformation.py
```

### Comparing `stamox-0.1.4/LICENCE` & `stamox-0.1.5/LICENCE`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/PKG-INFO` & `stamox-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.4
+Version: 0.1.5
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -44,15 +44,15 @@
 ![benchmark](./benchmark/benchmark2.png)
 
 ## Installation
 
 ```bash
 pip install -U stamox
 # or
-pip install git+[stamox](https://github.com/JiaYaobo/stamox.git)
+pip install git+https://github.com/JiaYaobo/stamox.git
 ```
 
 ## Documentation
 
 More comprehensive introduction and examples can be found in the [documentation](https://jiayaobo.github.io/stamox/).
 
 ## Quick Start
```

### Comparing `stamox-0.1.4/README.md` & `stamox-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ![benchmark](./benchmark/benchmark2.png)
 
 ## Installation
 
 ```bash
 pip install -U stamox
 # or
-pip install git+[stamox](https://github.com/JiaYaobo/stamox.git)
+pip install git+https://github.com/JiaYaobo/stamox.git
 ```
 
 ## Documentation
 
 More comprehensive introduction and examples can be found in the [documentation](https://jiayaobo.github.io/stamox/).
 
 ## Quick Start
```

### Comparing `stamox-0.1.4/setup.py` & `stamox-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 
 from setuptools import find_packages, setup
 
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 PACKAGE_NAME = "stamox"
 AUTHOR = "Jia Yaobo"
 URL = "https://github.com/jiayaobo/stamox"
 
 LICENSE = "Apache 2.0"
 DESCRIPTION = "Accelerate Your Statistical Analysis with JAX."
 LONG_DESCRIPTION = (HERE / "README.md").read_text()
```

### Comparing `stamox-0.1.4/stamox/__init__.py` & `stamox-0.1.5/stamox/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/basic.py` & `stamox-0.1.5/stamox/basic.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/cluster/_kmeans.py` & `stamox-0.1.5/stamox/cluster/_kmeans.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/core/__init__.py` & `stamox-0.1.5/stamox/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/core/base.py` & `stamox-0.1.5/stamox/core/base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/core/better_partial.py` & `stamox-0.1.5/stamox/core/better_partial.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/core/jit.py` & `stamox-0.1.5/stamox/core/jit.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/core/maps.py` & `stamox-0.1.5/stamox/core/maps.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/core/pipe.py` & `stamox-0.1.5/stamox/core/pipe.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/correlation/_cor.py` & `stamox-0.1.5/stamox/correlation/_cor.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/correlation/_pearson.py` & `stamox-0.1.5/stamox/correlation/_pearson.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/correlation/_spearman.py` & `stamox-0.1.5/stamox/correlation/_spearman.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/distribution/__init__.py` & `stamox-0.1.5/stamox/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/distribution/_beta.py` & `stamox-0.1.5/stamox/distribution/_beta.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Float
 from tensorflow_probability.substrates.jax.math import special as tfp_special
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pbeta(
     x: Union[Float, ArrayLike], a: Union[Float, ArrayLike], b: Union[Float, ArrayLike]
 ):
@@ -51,17 +52,16 @@
         >>> q = jnp.array([0.1, 0.5, 0.9])
         >>> a = 2.0
         >>> b = 3.0
         >>> pbeta(q, a, b)
         Array([0.05230004, 0.68749976, 0.9963    ], dtype=float32)
     """
     q, dtype = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, 0.0, 1.0)
-    p = filter_vmap(_pbeta)(q, a, b)
+    p = svmap_(_pbeta, q, a, b)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dbeta = filter_jit(filter_grad(_pbeta))
 
 
@@ -84,20 +84,19 @@
       dtype: The dtype of the output. Defaults to None.
 
     Returns:
       ArrayLike: The probability density function of the beta distribution evaluated at x.
 
     Example:
         >>> dbeta(0.5, 2, 3, lower_tail=True, log_prob=False)
-        Array([1.4999996], dtype=float32, weak_type=True)
+        Array(1.4999996, dtype=float32, weak_type=True)
     """
     x, dtype = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, 0.0, 1.0)
-    d = filter_vmap(_dbeta)(x, a, b)
+    d = svmap_(_dbeta, x, a, b)
     d = _post_process(d, lower_tail, log_prob)
     return d
 
 
 @filter_jit
 def _qbeta(
     p: Union[Float, ArrayLike], a: Union[Float, ArrayLike], b: Union[Float, ArrayLike]
@@ -126,20 +125,19 @@
         dtype: The dtype of the output. Defaults to None.
 
     Returns:
         ArrayLike: The value of the beta distribution at the given quantile.
 
     Example:
         >>> qbeta(0.5, 2, 3)
-        Array([0.38572744], dtype=float32)
+        Array(0.38572744, dtype=float32)
     """
     p, dtype = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail=lower_tail, log_prob=log_prob)
-    x = filter_vmap(_qbeta)(p, a, b)
+    x = svmap_(_qbeta, p, a, b)
     return x
 
 
 def rbeta(
     key: KeyArray,
     sample_shape: Optional[Shape] = None,
     a: Union[Float, ArrayLike] = None,
```

### Comparing `stamox-0.1.4/stamox/distribution/_binomial.py` & `stamox-0.1.5/stamox/distribution/_binomial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Optional
 
 import jax.numpy as jnp
-from equinox import filter_jit, filter_vmap
+from equinox import filter_jit
 from jax import pure_callback, ShapeDtypeStruct
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Bool
 from scipy.stats import binom
 from tensorflow_probability.substrates.jax.distributions import Binomial as tfp_Binomial
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pbinom(q, size, prob) -> ArrayLike:
     size = jnp.asarray(size, dtype=q.dtype)
     prob = jnp.asarray(prob, dtype=q.dtype)
@@ -48,17 +49,16 @@
     Example:
         >>> q = jnp.array([0.1, 0.5, 0.9])
         >>> size = 10
         >>> prob = 0.5
         >>> pbinom(q, size, prob)
     """
     q, dtype = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, 0, size)
-    p = filter_vmap(_pbinom)(q, size, prob)
+    p = svmap_(_pbinom, q, size, prob)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 @filter_jit
 def _dbinom(q, size, prob) -> ArrayLike:
     size = jnp.asarray(size, dtype=q.dtype)
@@ -91,16 +91,15 @@
     Example:
         >>> q = jnp.array([0.1, 0.5, 0.9])
         >>> size = 10
         >>> prob = 0.5
         >>> dbinom(q, size, prob)
     """
     q, dtype = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
-    d = filter_vmap(_dbinom)(q, size, prob)
+    d = svmap_(_dbinom, q, size, prob)
     d = _post_process(d, lower_tail, log_prob)
     return d
 
 
 @filter_jit
 def _qbinom(p, size, prob, dtype) -> ArrayLike:
     result_shape_type = ShapeDtypeStruct(jnp.shape(p), dtype)
@@ -135,17 +134,16 @@
         >>> size = 10
         >>> prob = 0.5
         >>> qbinom(p, size, prob)
     """
     if dtype is None:
         dtype = jnp.int_
     p = jnp.asarray(p, dtype=jnp.float_)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    q = filter_vmap(_qbinom)(p, size, prob, dtype)
+    q = _qbinom(p, size, prob, dtype)
     return q
 
 
 @filter_jit
 def _rbinom(key, size, prob, sample_shape, dtype) -> ArrayLike:
     bino = tfp_Binomial(total_count=size, probs=prob)
     return bino.sample(sample_shape=sample_shape, seed=key).astype(dtype)
```

### Comparing `stamox-0.1.4/stamox/distribution/_cauchy.py` & `stamox-0.1.5/stamox/distribution/_cauchy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jaxtyping import ArrayLike, Bool, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pcauchy(
     x: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
@@ -48,20 +49,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cumulative density function of the Cauchy distribution.
 
     Example:
         >>> pcauchy(1.0, loc=0.0, scale=1.0, lower_tail=True, log_prob=False)
-        Array([0.75], dtype=float32, weak_type=True)
+        Array(0.75, dtype=float32, weak_type=True)
     """
     q, dtype = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q)
-    p = filter_vmap(_pcauchy)(q, loc, scale)
+    p = svmap_(_pcauchy, q, loc, scale)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dcauchy = filter_grad(filter_jit(_pcauchy))
 
 
@@ -87,17 +87,16 @@
         ArrayLike: The pdf of the Cauchy distribution.
 
     Example:
         >>> dcauchy(1.0, loc=0.0, scale=1.0)
         Array([0.15915494], dtype=float32, weak_type=True)
     """
     x, dtype = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x)
-    grads = filter_vmap(_dcauchy)(x, loc, scale)
+    grads = svmap_(_dcauchy, x, loc, scale)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qcauchy(
     q: Union[Float, ArrayLike],
@@ -132,17 +131,16 @@
         ArrayLike: The quantiles of the Cauchy distribution.
 
     Example:
         >>> qcauchy(0.5, loc=1.0, scale=2.0)
         Array([1.], dtype=float32, weak_type=True)
     """
     q, dtype = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_probability(q, lower_tail, log_prob)
-    return filter_vmap(_qcauchy)(q, loc, scale)
+    return svmap_(_qcauchy, q, loc, scale)
 
 
 @filter_jit
 def _rcauchy(
     key: KeyArray,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
```

### Comparing `stamox-0.1.4/stamox/distribution/_chisq.py` & `stamox-0.1.5/stamox/distribution/_chisq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_jit, filter_vmap
+from equinox import filter_jit
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Float, Int
 
 from ._gamma import _dgamma, _pgamma, _qgamma
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 def dchisq(
     x: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
     lower_tail=True,
@@ -32,20 +33,19 @@
         dtype: The dtype of the output (defaults to float32).
 
     Returns:
         ArrayLike: The chi-squared distribution evaluated at `x`.
 
     Example:
         >>> dchisq(2.0, 3)
-        Array([0.20755368], dtype=float32, weak_type=True)
+        Array(0.20755368, dtype=float32, weak_type=True)
     """
     x, dtype = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, 0.0, jnp.inf)
-    grads = filter_vmap(_dgamma)(x, df / 2, 1 / 2)
+    grads = svmap_(_dgamma, x, df / 2, 1 / 2)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 def pchisq(
     q: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
@@ -63,20 +63,19 @@
         dtype (dtype): The dtype of the output (default jnp.float_).
 
     Returns:
         ArrayLike: The chi-squared probability density function.
 
     Example:
         >>> pchisq(2.0, 3)
-        Array([0.42759317], dtype=float32, weak_type=True)
+        Array(0.42759317, dtype=float32, weak_type=True)
     """
     q = jnp.asarray(q, dtype=dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, 0.0, jnp.inf)
-    p = filter_vmap(_pgamma)(q, df / 2, 1 / 2)
+    p = svmap_(_pgamma, q, df / 2, 1 / 2)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 def qchisq(
     p: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
@@ -94,20 +93,19 @@
         dtype (dtype, optional): The dtype of the output (default jnp.float_).
 
     Returns:
         ArrayLike: The quantiles corresponding to the given probabilities.
 
     Example:
         >>> qchisq(0.95, 10)
-        Array([18.307034], dtype=float32)
+        Array(18.307034, dtype=float32)
     """
     p = jnp.asarray(p, dtype=dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    q = filter_vmap(_qgamma)(p, df / 2, 1 / 2)
+    q = svmap_(_qgamma, p, df / 2, 1 / 2)
     return q
 
 
 @filter_jit
 def _rchisq(
     key: KeyArray,
     df: Union[Int, Float, ArrayLike],
```

### Comparing `stamox-0.1.4/stamox/distribution/_ecdf.py` & `stamox-0.1.5/stamox/distribution/_ecdf.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/distribution/_exp.py` & `stamox-0.1.5/stamox/distribution/_exp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pexp(x: Union[float, ArrayLike], rate: float) -> Float:
     return -jnp.expm1(-rate * x)
 
@@ -37,20 +38,19 @@
         dtype: jnp.dtype, optional. The dtype of the output (default is float_).
 
     Returns:
         ArrayLike: The probability of the given value or array of values.
 
     Example:
         >>> pexp(1.0, 0.5)
-        Array([0.39346933], dtype=float32, weak_type=True)
+        Array(0.39346933, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, 0)
-    p = filter_vmap(_pexp)(q, rate)
+    p = svmap_(_pexp, q, rate)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 @filter_jit
 def _qexp(q: Union[float, ArrayLike], rate: float) -> Float:
     dtype = lax.dtype(q)
@@ -78,17 +78,16 @@
         ArrayLike: The quantile of the exponential distribution.
 
     Example:
         >>> qexp(0.5, 1.0)
         Array([0.6931472], dtype=float32, weak_type=True)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    x = filter_vmap(_qexp)(p, rate)
+    x = svmap_(_qexp, p, rate)
     return x
 
 
 _dexp = filter_jit(filter_grad(_pexp))
 
 
 def dexp(
@@ -111,17 +110,16 @@
         ArrayLike: The derivative of the exponential distribution evaluated at x.
 
     Example:
         >>> dexp(1.0, 0.5, lower_tail=True, log_prob=False)
         Array([0.30326533], dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, 0)
-    grads = filter_vmap(_dexp)(x, rate)
+    grads = svmap_(_dexp, x, rate)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _rexp(
     key: KeyArray,
@@ -159,12 +157,9 @@
     Example:
         >>> key = jax.random.PRNGKey(0)
         >>> rexp(key, sample_shape=(2, 3), rate=1.0, lower_tail=False, log_prob=True)
         Array([[-0.69314718, -0.69314718, -0.69314718],
                [-0.69314718, -0.69314718, -0.69314718]], dtype=float32)
     """
     rvs = _rexp(key, rate, sample_shape, dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.4/stamox/distribution/_f.py` & `stamox-0.1.5/stamox/distribution/_f.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Float
 
 from ..math.special import fdtr, fdtri
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pf(
     x: Union[Float, ArrayLike],
     dfn: Union[Float, ArrayLike],
@@ -45,20 +46,19 @@
         dtype (jnp.dtype, optional): The dtype of the output (default is jnp.float_).
 
     Returns:
         ArrayLike: The cumulative distribution function evaluated at `q`.
 
     Example:
         >>> pF(1.0, 1.0, 1.0)
-        Array([0.5000001], dtype=float32, weak_type=True)
+        Array(0.5000001, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, 0)
-    p = filter_vmap(_pf)(q, dfn, dfd)
+    p = svmap_(_pf, q, dfn, dfd)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _df = filter_jit(filter_grad(_pf))
 
 
@@ -81,20 +81,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The gradient of the cumulative distribution function.
 
     Example:
         >>> dF(1.0, 1.0, 1.0)
-        Array([0.1591549], dtype=float32, weak_type=True)
+        Array(0.1591549, dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, 0)
-    grads = filter_vmap(_df)(x, dfn, dfd)
+    grads = svmap_(_df, x, dfn, dfd)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qf(
     q: Union[Float, ArrayLike],
@@ -128,17 +127,16 @@
         ArrayLike: The calculated quantile.
 
     Example:
         >>> qF(0.5, 1.0, 1.0)
         Array([0.99999714], dtype=float32)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    return filter_vmap(_qf)(p, dfn, dfd)
+    return svmap_(_qf, p, dfn, dfd)
 
 
 @filter_jit
 def _rf(
     key: KeyArray,
     dfn: Union[Float, ArrayLike],
     dfd: Union[Float, ArrayLike],
```

### Comparing `stamox-0.1.4/stamox/distribution/_gamma.py` & `stamox-0.1.5/stamox/distribution/_gamma.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
 import tensorflow_probability.substrates.jax.math as tfp_math
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import KeyArray, Shape
 from jax.scipy.special import gammainc
 from jaxtyping import ArrayLike, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pgamma(
     q, shape: Union[Float, ArrayLike] = 1.0, rate: Union[Float, ArrayLike] = 1.0
 ):
@@ -43,20 +44,19 @@
         dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The CDF value of the given value or array of values.
 
     Example:
         >>> pgamma(1.0, 0.5, 0.5)
-        Array([0.6826893], dtype=float32, weak_type=True)
+        Array(0.6826893, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, 0.0, jnp.inf)
-    p = filter_vmap(_pgamma)(q, shape, rate)
+    p = svmap_(_pgamma, q, shape, rate)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dgamma = filter_jit(filter_grad(_pgamma))
 
 
@@ -85,20 +85,19 @@
 
     Returns:
         ArrayLike: The density of the gamma distribution evaluated
             at `x`. If `log_prob` is True, returns the log probability.
 
     Example:
         >>> dgamma(1.0, 0.5, 0.5)
-        Array([0.24197064], dtype=float32, weak_type=True)
+        Array(0.24197064, dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, 0.0, jnp.inf)
-    grads = filter_vmap(_dgamma)(x, shape, rate)
+    grads = svmap_(_dgamma, x, shape, rate)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qgamma(
     q: Union[Float, ArrayLike],
@@ -133,17 +132,16 @@
         ArrayLike: The quantile of the gamma distribution.
 
     Example:
         >>> qgamma(0.5, 0.5, 0.5)
         Array([0.45493677], dtype=float32)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    x = filter_vmap(_qgamma)(p, shape, rate)
+    x = svmap_(_qgamma, p, shape, rate)
     return x
 
 
 def rgamma(
     key,
     sample_shape: Optional[Shape] = None,
     shape: Union[Float, ArrayLike] = 1.0,
@@ -167,18 +165,15 @@
         ArrayLike: A random gamma value or an array of random gamma values.
 
     Example:
         >>> rgamma(key, shape=0.5, rate=0.5)
         Array(0.3384059, dtype=float32)
     """
     rvs = _rgamma(key, shape, rate, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
 
 
 @filter_jit
 def _rgamma(
     key: KeyArray,
     shape: Union[Float, ArrayLike] = 1.0,
```

### Comparing `stamox-0.1.4/stamox/distribution/_laplace.py` & `stamox-0.1.5/stamox/distribution/_laplace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jaxtyping import ArrayLike, Bool, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _plaplace(
     x: Union[Float, ArrayLike],
     loc: Union[Float, ArrayLike] = 0.0,
@@ -50,20 +51,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The Laplace CDF evaluated at `q`.
 
     Example:
         >>> plaplace(1.0, 1.0, 1.0)
-        Array([0.5], dtype=float32, weak_type=True)
+        Array(0.5, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q)
-    p = filter_vmap(_plaplace)(q, loc, scale)
+    p = svmap_(_plaplace, q, loc, scale)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dlaplace = filter_grad(filter_jit(_plaplace))
 
 
@@ -86,20 +86,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The probability density at the given x.
 
     Example:
         >>> dlaplace(1.0, 1.0, 1.0)
-        Array([0.], dtype=float32, weak_type=True)
+        Array(0., dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x)
-    grads = filter_vmap(_dlaplace)(x, loc, scale)
+    grads = svmap_(_dlaplace, x, loc, scale)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qlaplace(
     q: Union[Float, ArrayLike],
@@ -133,20 +132,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The quantiles of the Laplace distribution.
 
     Example:
         >>> qlaplace(0.5, 1.0, 1.0)
-        Array([1.], dtype=float32, weak_type=True)
+        Array(1., dtype=float32, weak_type=True)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    return filter_vmap(_qlaplace)(p, loc, scale)
+    return svmap_(_qlaplace, p, loc, scale)
 
 
 @filter_jit
 def _rlaplace(
     key: KeyArray,
     loc: Union[Float, ArrayLike] = 0.0,
     scale: Union[Float, ArrayLike] = 1.0,
@@ -186,12 +184,9 @@
     Example:
         >>> rlaplace(key, (2, 3))
         Array([[-0.16134426,  1.6125823 , -0.6615164 ],
                 [-1.5528525 , -0.21459664,  0.09816013]], dtype=float32)
 
     """
     rvs = _rlaplace(key, loc, scale, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-    if log_prob:
-        rvs = jnp.log(rvs)
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.4/stamox/distribution/_normal.py` & `stamox-0.1.5/stamox/distribution/_normal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jax.scipy.special import ndtr, ndtri
 from jaxtyping import ArrayLike, Bool, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pnorm(
     x: Union[Float, ArrayLike],
     mean: Union[Float, ArrayLike] = 0.0,
@@ -53,23 +54,22 @@
 
     Returns:
         ArrayLike: The CDF of the normal distribution evaluated at x.
 
 
     Examples:
         >>> pnorm(2.0)
-        Array([0.97724986], dtype=float32)
+        Array(0.97724986, dtype=float32)
 
         >>> pnorm([1.5, 2.0, 2.5], mean=2.0, sd=0.5, lower_tail=False)
         Array([0.8413447 , 0.5       , 0.15865529], dtype=float32)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q)
-    p = filter_vmap(_pnorm)(q, mean, sd)
+    p = svmap_(_pnorm, q, mean, sd)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dnorm = filter_jit(filter_grad(_pnorm))
 
 
@@ -98,17 +98,16 @@
     Example:
         >>> import jax.numpy as jnp
         >>> x = jnp.array([0.5, 1.0, -1.5])
         >>> dnorm(x)
         Array([0.35206532, 0.24197075, 0.12951761], dtype=float32)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x)
-    grads = filter_vmap(_dnorm)(x, mean, sd)
+    grads = svmap_(_dnorm, x, mean, sd)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qnorm(
     p: Union[Float, ArrayLike],
@@ -147,17 +146,16 @@
     Examples:
         >>> qnorm(0.5)
         Array([0.], dtype=float32)
         >>> qnorm([0.25, 0.75], mean=3, sd=2)
         Array([1.6510204, 4.3489795], dtype=float32)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    x = filter_vmap(_qnorm)(p, mean, sd)
+    x = svmap_(_qnorm, p, mean, sd)
     return x
 
 
 @filter_jit
 def _rnorm(key, mean, sd, sample_shape, dtype):
     if sample_shape is None:
         sample_shape = jnp.broadcast_shapes(jnp.shape(mean), jnp.shape(sd))
@@ -195,14 +193,9 @@
         >>> rnorm(key, sample_shape=(3, 2))
         Array([[ 0.18784384, -1.2833426 ],
                 [ 0.6494181 ,  1.2490594 ],
                 [ 0.24447003, -0.11744965]], dtype=float32)
 
     """
     rvs = _rnorm(key, mean, sd, sample_shape, dtype=dtype)
-    if not lower_tail:
-        rvs = 1 - rvs
-
-    if log_prob:
-        rvs = jnp.log(rvs)
-
+    rvs = _post_process(rvs, lower_tail, log_prob)
     return rvs
```

### Comparing `stamox-0.1.4/stamox/distribution/_pareto.py` & `stamox-0.1.5/stamox/distribution/_pareto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jaxtyping import ArrayLike, Bool, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _ppareto(
     x: Union[Float, ArrayLike],
     scale: Union[Float, ArrayLike],
@@ -43,20 +44,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cumulative distribution function of the Pareto distribution evaluated at `q`.
 
     Example:
         >>> ppareto(0.2, 0.1, 2.0)
-        Array([0.75], dtype=float32, weak_type=True)
+        Array(0.75, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
-    q = filter_vmap(_check_clip_distribution_domain)(q, scale)
-    p = filter_vmap(_ppareto)(q, scale, alpha)
+    q = svmap_(_check_clip_distribution_domain, q, scale)
+    p = svmap_(_ppareto, q, scale, alpha)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dpareto = filter_grad(filter_jit(_ppareto))
 
 
@@ -82,16 +82,15 @@
         ArrayLike: The density of the Pareto distribution evaluated at `x`.
 
     Example:
         >>> dpareto(0.2, 0.1, 2.0)
         Array([2.4999998], dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
-    grads = filter_vmap(_dpareto)(x, scale, alpha)
+    grads = svmap_(_dpareto, x, scale, alpha)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qpareto(
     q: Union[Float, ArrayLike],
@@ -123,17 +122,16 @@
         ArrayLike: The quantiles of the Pareto distribution.
 
     Example:
         >>> qpareto(0.2, 0.1, 2.0)
         Array([0.1118034], dtype=float32, weak_type=True)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    return filter_vmap(_qpareto)(p, scale, alpha)
+    return svmap_(_qpareto, p, scale, alpha)
 
 
 @filter_jit
 def _rpareto(
     key: KeyArray,
     scale: Union[Float, ArrayLike],
     alpha: Union[Float, ArrayLike],
```

### Comparing `stamox-0.1.4/stamox/distribution/_poisson.py` & `stamox-0.1.5/stamox/distribution/_poisson.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_jit, filter_vmap
+from equinox import filter_jit
 from jax import pure_callback, ShapeDtypeStruct
 from jax._src.random import Shape
 from jax.random import KeyArray
 from jax.scipy.special import gammainc, gammaln
 from jaxtyping import Array, ArrayLike, Bool, Float
 from scipy.stats import poisson
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _ppoisson(x: Union[Float, ArrayLike], rate: Union[Float, ArrayLike]) -> Array:
     k = jnp.floor(x) + 1.0
     return 1 - gammainc(k, rate)
@@ -43,17 +44,16 @@
     Returns:
         ArrayLike: The cumulative distribution function of the Poisson distribution evaluated at `q`.
 
     Example:
         >>> ppoisson(1.0, rate=1.0)
     """
     q, dtype = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, lower=0.0)
-    p = filter_vmap(_ppoisson)(q, rate)
+    p = svmap_(_ppoisson, q, rate)
     p = _post_process(p, lower_tail=lower_tail, log_prob=log_prob)
     return p
 
 
 @filter_jit
 def _dpoisson(x, rate):
     e = jnp.exp(-rate)
@@ -81,17 +81,16 @@
     Returns:
         ArrayLike: The probability density function of the Poisson distribution evaluated at `x`.
 
     Examples:
         >>> dpoisson(1.0, rate=1.0)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, lower=0.0)
-    grads = filter_vmap(_dpoisson)(x, rate)
+    grads = svmap_(_dpoisson, x, rate)
     grads = _post_process(grads, lower_tail=lower_tail, log_prob=log_prob)
     return grads
 
 
 @filter_jit
 def _rpoisson(
     key: KeyArray,
@@ -159,11 +158,10 @@
     Returns:
         ArrayLike: The quantile function of the Poisson distribution evaluated at `p`.
 
     Example:
         >>> qpoisson(0.5, rate=1.0)
     """
     p, _ = _promote_dtype_to_floating(p, None)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    q = filter_vmap(_qpoisson)(p, rate, dtype)
+    q = svmap_(_qpoisson, p, rate, dtype)
     return q
```

### Comparing `stamox-0.1.4/stamox/distribution/_t.py` & `stamox-0.1.5/stamox/distribution/_t.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from jaxtyping import ArrayLike, Float, Int
 from tensorflow_probability.substrates.jax.math import special as tfp_special
 
 from ._utils import (
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pt(
     x: Union[Float, ArrayLike],
     df: Union[Int, Float, ArrayLike],
@@ -57,19 +58,18 @@
         dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cdf value of the given value for Student T distribution.
 
     Example:
         >>> pt(1.0, 1.0)
-        Array([0.74999994], dtype=float32, weak_type=True)
+        Array(0.74999994, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
-    p = filter_vmap(_pt)(q, df, loc, scale)
+    p = svmap_(_pt, q, df, loc, scale)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dt = filter_jit(filter_grad(_pt))
 
 
@@ -95,19 +95,18 @@
         dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The probability density function evaluated at `x`.
 
     Example:
         >>> dt(1.0, 1.0)
-        Array([0.1591549], dtype=float32, weak_type=True)
+        Array(0.1591549, dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
-    grads = filter_vmap(_dt)(x, df, loc, scale)
+    grads = svmap_(_dt, x, df, loc, scale)
     grads = _post_process(grads, lower_tail, log_prob)
     return grads
 
 
 @filter_jit
 def _qt(
     q: Union[Float, ArrayLike],
@@ -146,20 +145,19 @@
         dtype: The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The quantile of the Student T distribution.
 
     Example:
         >>> qt(0.5, 1.0)
-        Array([0.], dtype=float32, weak_type=True)
+        Array(0., dtype=float32, weak_type=True)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail=lower_tail, log_prob=log_prob)
-    q = filter_vmap(_qt)(p, df, loc, scale)
+    q = svmap_(_qt, p, df, loc, scale)
     return q
 
 
 @filter_jit
 def _rt(
     key: KeyArray,
     df: Union[Int, Float, ArrayLike],
```

### Comparing `stamox-0.1.4/stamox/distribution/_uniform.py` & `stamox-0.1.5/stamox/distribution/_uniform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Bool, Float
 
 from ._utils import (
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _punif(
     x: Union[Float, ArrayLike],
     mini: Union[Float, ArrayLike] = 0.0,
@@ -46,19 +47,18 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The cumulative distribution function of the uniform distribution evaluated at `q`.
 
     Example:
         >>> punif(0.5)
-        Array([0.5], dtype=float32, weak_type=True)
+        Array(0.5, dtype=float32, weak_type=True)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
-    p = filter_vmap(_punif)(q, mini, maxi)
+    p = svmap_(_punif, q, mini, maxi)
     p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 _dunif = filter_grad(filter_jit(_punif))
 
 
@@ -81,23 +81,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
         ArrayLike: The probability density of the given value(s).
 
     Example:
         >>> dunif(0.5)
-        Array([1.], dtype=float32, weak_type=True)
+        Array(1., dtype=float32, weak_type=True)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
-    p = filter_vmap(_dunif)(x, mini, maxi)
-    if not lower_tail:
-        p = 1 - p
-    if log_prob:
-        p = jnp.log(p)
+    p = svmap_(_dunif, x, mini, maxi)
+    p = _post_process(p, lower_tail, log_prob)
     return p
 
 
 @filter_jit
 def _qunif(
     q: Union[Float, ArrayLike],
     mini: Union[Float, ArrayLike] = 0.0,
@@ -128,20 +124,19 @@
         dtype (jnp.dtype, optional): The dtype of the output. Defaults to jnp.float_.
 
     Returns:
        ArrayLike: The quantiles of the uniform distribution.
 
     Example:
         >>> qunif(0.5)
-        Array([0.5], dtype=float32, weak_type=True)
+        Array(0.5, dtype=float32, weak_type=True)
     """
     p = jnp.asarray(p, dtype=dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    q = filter_vmap(_qunif)(p, mini, maxi)
+    q = svmap_(_qunif, p, mini, maxi)
     return q
 
 
 @filter_jit
 def _runif(
     key: KeyArray,
     mini: Union[Float, ArrayLike] = 0.0,
```

### Comparing `stamox-0.1.4/stamox/distribution/_utils.py` & `stamox-0.1.5/stamox/distribution/_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import functools
 
 import jax.numpy as jnp
+from equinox import filter_vmap
 from jax import jit, lax
 
 
 inf = jnp.inf
 nan = jnp.nan
 
 
 @functools.partial(jit, static_argnums=(1, 2))
-def _check_clip_probability(
-    p: jnp.ndarray, lower_tail=True, log_prob=False
-) -> jnp.ndarray:
+def _check_clip_probability(p, lower_tail=True, log_prob=False):
     if not lower_tail:
         p = 1 - p
     if log_prob:
         p = jnp.exp(p)
     return jnp.clip(p, 0.0, 1.0)
 
 
 @functools.partial(jit, static_argnums=(1, 2))
-def _check_clip_distribution_domain(
-    x: jnp.ndarray, lower=-inf, upper=inf
-) -> jnp.ndarray:
+def _check_clip_distribution_domain(x, lower=-inf, upper=inf):
     return jnp.clip(x, lower, upper)
 
 
 def _promote_dtype_to_floating(q, dtype):
     if dtype is None:
         if jnp.issubdtype(lax.dtype(q), jnp.integer):
             return jnp.asarray(q, dtype=jnp.float_), jnp.float_
@@ -42,24 +39,41 @@
             return jnp.asarray(x, dtype=jnp.int_), jnp.int_
         else:
             return jnp.asarray(x), lax.dtype(x)
     else:
         return jnp.asarray(x, dtype=dtype), dtype
 
 
+@functools.partial(jit, static_argnums=(1, 2))
 def _post_process(p, lower_tail=True, log_prob=False):
     if not lower_tail:
         p = 1 - p
     if log_prob:
         p = jnp.log(p)
     return p
 
 
+def _check_all_scalar(*args):
+    for arg in args:
+        if not jnp.shape(arg) == ():
+            return False
+    return True
+
+
+def svmap_(f, *args):
+    if _check_all_scalar(*args):
+        return f(*args)
+    else:
+        return filter_vmap(f)(*args)
+
+
 __all__ = [  # noqa: F405
     "inf",
     "nan",
     "_check_clip_probability",
     "_check_clip_distribution_domain",
     "_promote_dtype_to_floating",
     "_promote_dtype_to_integer",
     "_post_process",
+    "_check_all_scalar",
+    "svmap_",
 ]
```

### Comparing `stamox-0.1.4/stamox/distribution/_weibull.py` & `stamox-0.1.5/stamox/distribution/_weibull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Optional, Union
 
 import jax.numpy as jnp
 import jax.random as jrand
-from equinox import filter_grad, filter_jit, filter_vmap
+from equinox import filter_grad, filter_jit
 from jax import lax
 from jax._src.random import KeyArray, Shape
 from jaxtyping import ArrayLike, Float
 
 from ._utils import (
     _check_clip_distribution_domain,
     _check_clip_probability,
     _post_process,
     _promote_dtype_to_floating,
+    svmap_,
 )
 
 
 @filter_jit
 def _pweibull(
     x: Union[Float, ArrayLike],
     concentration: Union[Float, ArrayLike] = 0.0,
@@ -49,17 +50,16 @@
     Returns:
         Array: The cumulative distribution function of the Weibull distribution evaluated at `q`.
 
     Example:
         >>> pweibull(1.0, concentration=1.0, scale=1.0)
     """
     q, _ = _promote_dtype_to_floating(q, dtype)
-    q = jnp.atleast_1d(q)
     q = _check_clip_distribution_domain(q, lower=0.0)
-    p = filter_vmap(_pweibull)(q, concentration, scale)
+    p = svmap_(_pweibull, q, concentration, scale)
     p = _post_process(p, lower_tail=lower_tail, log_prob=log_prob)
     return p
 
 
 _dweibull = filter_grad(filter_jit(_pweibull))
 
 
@@ -80,17 +80,16 @@
     Returns:
         Array: The probability density function of the Weibull distribution evaluated at `x`.
 
     Example:
         >>> dweibull(0.5, 1.0, 1.0)
     """
     x, _ = _promote_dtype_to_floating(x, dtype)
-    x = jnp.atleast_1d(x)
     x = _check_clip_distribution_domain(x, lower=0.0)
-    grads = filter_vmap(_dweibull)(x, concentration, scale)
+    grads = svmap_(_dweibull, x, concentration, scale)
     grads = _post_process(grads, lower_tail=lower_tail, log_prob=log_prob)
     return grads
 
 
 @filter_jit
 def _qweibull(
     q: Union[Float, ArrayLike],
@@ -129,17 +128,16 @@
     Returns:
         Array: The computed quantiles.
 
     Example:
         >>> qweibull(0.5, 1.0, 1.0)
     """
     p, _ = _promote_dtype_to_floating(p, dtype)
-    p = jnp.atleast_1d(p)
     p = _check_clip_probability(p, lower_tail, log_prob)
-    q = filter_vmap(_qweibull)(p, concentration, scale)
+    q = svmap_(_qweibull, p, concentration, scale)
     return q
 
 
 @filter_jit
 def _rweibull(
     key: KeyArray,
     concentration: Union[Float, ArrayLike] = 0.0,
```

### Comparing `stamox-0.1.4/stamox/experimental/maps/auto_map.py` & `stamox-0.1.5/stamox/experimental/maps/auto_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/experimental/maps/cube_map.py` & `stamox-0.1.5/stamox/experimental/maps/cube_map.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/formula/_formula.py` & `stamox-0.1.5/stamox/formula/_formula.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/functions.py` & `stamox-0.1.5/stamox/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from .cluster import kmeans
 from .core import (
     predict,
     summary,
 )
 from .correlation import cor, pearsonr, spearmanr
+from .decomposition import princomp
 from .distribution import (
     dbeta,
     dbinom,
     dcauchy,
     dchisq,
     dexp,
     dF,
@@ -173,8 +174,9 @@
     "max",
     "sum",
     "prod",
     "cumsum",
     "cumprod",
     "diff",
     "scale",
+    "princomp",
 ]
```

### Comparing `stamox-0.1.4/stamox/hypothesis/_bartlett.py` & `stamox-0.1.5/stamox/hypothesis/_bartlett.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
     @property
     def df(self):
         return self.parameters
 
 
-def bartlett_test(*samples: Sequence[ArrayLike]) -> BartlettTest:
+def bartlett_test(*samples: Sequence[ArrayLike], axis=0) -> BartlettTest:
     """Calculates the Bartlett test statistic for multiple samples.
 
     Args:
         *samples Sequence[ArrayLike]): A sequence of 1-D arrays, each containing
             a sample of scores. All samples must have the same length.
 
     Returns:
@@ -60,27 +60,28 @@
 
     Example:
         >>> from stamox.functions import bartlett_test
         >>> bartlett_test([1, 2, 3], [1, 2, 3])
         BartlettTest(statistic=0.0, parameters=1, p_value=1.0)
     """
     samples = jnp.vstack(samples)
-    return _bartlett(samples)
+    return _bartlett(samples, axis)
 
 
 @filter_jit
-def _bartlett(samples):
+def _bartlett(samples, axis):
     k = samples.shape[0]
-    Ni = jnp.asarray(vmap(jnp.size, in_axes=(0,))(samples), dtype=samples.dtype)
-    ssq = vmap(partial(jnp.var, ddof=1), in_axes=(0,))(samples)
-    Ntot = jnp.sum(Ni, axis=0)
-    spsq = jnp.sum((Ni - 1) * ssq, axis=0) / (1.0 * (Ntot - k))
+    Ni = jnp.asarray(vmap(jnp.size, in_axes=(axis,))(samples), dtype=samples.dtype)
+    ssq = vmap(partial(jnp.var, ddof=1), in_axes=(axis,))(samples)
+    Ntot = jnp.sum(Ni, axis=axis)
+    spsq = jnp.sum((Ni - 1) * ssq, axis=axis) / (1.0 * (Ntot - k))
     numer = (Ntot * 1.0 - k) * jnp.log(spsq) - jnp.sum(
-        (Ni - 1.0) * jnp.log(ssq), axis=0
+        (Ni - 1.0) * jnp.log(ssq), axis=axis
     )
     denom = 1.0 + 1.0 / (3 * (k - 1)) * (
-        (jnp.sum(1.0 / (Ni - 1.0), axis=0)) - 1.0 / (Ntot - k)
+        (jnp.sum(1.0 / (Ni - 1.0), axis=axis)) - 1.0 / (Ntot - k)
     )
     stats = numer / denom
     param = k - 1
-    pval = pchisq(stats, param, lower_tail=False).squeeze()
+    stats = stats.squeeze()
+    pval = pchisq(stats, param, lower_tail=False)
     return BartlettTest(statistic=stats, parameters=param, p_value=pval)
```

### Comparing `stamox-0.1.4/stamox/hypothesis/_base.py` & `stamox-0.1.5/stamox/hypothesis/_base.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/hypothesis/_durbin_watson.py` & `stamox-0.1.5/stamox/hypothesis/_durbin_watson.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,8 +69,9 @@
     Returns:
         float: The Durbin-Watson statistic.
     """
     diff_resids = jnp.diff(resids, 1, axis=axis)
     dw = jnp.sum(diff_resids**2, axis=axis, keepdims=True) / jnp.sum(
         resids**2, axis=axis, keepdims=True
     )
+    dw = dw.squeeze()
     return DurbinWatsonTest(statistic=dw)
```

### Comparing `stamox-0.1.4/stamox/hypothesis/_friedman.py` & `stamox-0.1.5/stamox/hypothesis/_friedman.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,42 +41,43 @@
             statistic, parameters, p_value, estimate, null_value, alternative, name
         )
     
     def __repr__(self):
         return f"{self.name}(statistic={self.statistic}, parameters={self.parameters}, p_value={self.p_value})"
 
 
-def friedman_test(*samples: Sequence[ArrayLike]) -> FriedmanTest:
+def friedman_test(*samples: Sequence[ArrayLike], axis=0) -> FriedmanTest:
     """Computes the Friedman statistic for a set of samples.
 
     Args:
         *samples: A sequence of samples, each sample being a sequence of
             observations.
 
     Returns:
         FriedmanTest: The Friedman Test object.
     """
     ImportWarning("This function is not yet functioned with ties. Use with caution.")
     samples = jnp.vstack(samples).T
-    return _friedman(samples)
+    return _friedman(samples, axis)
 
 
 @filter_jit
-def _friedman(samples):
+def _friedman(samples, axis):
     """Computes the Friedman statistic for a set of samples.
 
     Args:
         samples: A 2D array of samples, with the first dimension representing
             the treatments and the second dimension representing the blocks.
 
     Returns:
         The computed Friedman statistic.
     """
     n_blocks, k_treatments = samples.shape
-    ranks = vmap(lambda x: rankdata(x))(samples)
-    avg_ranks = jnp.mean(ranks, axis=0)
+    ranks = vmap(lambda x: rankdata(x), in_axes=(axis, ))(samples)
+    avg_ranks = jnp.mean(ranks, axis=axis)
     Q = 12.0 * n_blocks / (k_treatments * (k_treatments + 1)) * jnp.sum(
-        avg_ranks**2, axis=0, keepdims=True
+        avg_ranks**2, axis=axis, keepdims=True
     ) - 3 * n_blocks * (k_treatments + 1)
+    Q = Q.squeeze()
     param = k_treatments - 1
     pval = pchisq(Q, param, lower_tail=False)
     return FriedmanTest(statistic=Q, parameters=param, p_value=pval)
```

### Comparing `stamox-0.1.4/stamox/math/combination.py` & `stamox-0.1.5/stamox/math/combination.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/math/special.py` & `stamox-0.1.5/stamox/math/special.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox/pipe_functions.py` & `stamox-0.1.5/stamox/pipe_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .core import (
     make_partial_pipe,
     make_pipe,
     predict,
     summary,
 )
 from .correlation import cor, pearsonr, spearmanr
+from .decomposition import princomp
 from .distribution import (
     dbeta,
     dbinom,
     dcauchy,
     dchisq,
     dexp,
     dF,
@@ -80,17 +81,17 @@
 
 
 one_way = make_partial_pipe(one_way, name="one_way")
 kmeans = make_partial_pipe(kmeans, name="kmeans")
 spearmanr = make_partial_pipe(spearmanr, name="spearmanr")
 pearsonr = make_partial_pipe(pearsonr, name="pearsonr")
 cor = make_partial_pipe(cor, name="cor")
-bartlett_test = make_pipe(bartlett_test, name="bartlett_test")
+bartlett_test = make_partial_pipe(bartlett_test, name="bartlett_test")
 durbin_watson_test = make_partial_pipe(durbin_watson_test, name="durbin_watson_test")
-friedman_test = make_pipe(friedman_test, name="friedman_test")
+friedman_test = make_partial_pipe(friedman_test, name="friedman_test")
 bootstrap = make_partial_pipe(bootstrap, name="bootstrap")
 bootstrap_sample = make_partial_pipe(bootstrap_sample, name="bootstrap_sample")
 jackknife = make_partial_pipe(jackknife, name="jackknife")
 jackknife_sample = make_pipe(jackknife_sample, name="jackknife_sample")
 boxcox = make_partial_pipe(boxcox, name="boxcox")
 z_fisher = make_partial_pipe(z_fisher, name="z_fisher")
 lm = make_partial_pipe(lm, name="lm")
@@ -162,16 +163,15 @@
 max = make_partial_pipe(jnp.max, "max")
 sum = make_partial_pipe(jnp.sum, "sum")
 prod = make_partial_pipe(jnp.prod, "prod")
 cumsum = make_partial_pipe(jnp.cumsum, "cumsum")
 cumprod = make_partial_pipe(jnp.cumprod, "cumprod")
 diff = make_partial_pipe(jnp.diff, "diff")
 scale = make_partial_pipe(scale, "scale")
-
-
+princomp = make_partial_pipe(princomp, "princomp")
 
 __all__ = [
     "one_way",
     "kmeans",
     "spearmanr",
     "pearsonr",
     "cor",
@@ -253,8 +253,9 @@
     "max",
     "sum",
     "prod",
     "cumsum",
     "cumprod",
     "diff",
     "scale",
+    "princomp",
 ]
```

### Comparing `stamox-0.1.4/stamox/regression/_base.py` & `stamox-0.1.5/stamox/regression/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
     @property
     def params(self):
         return self._coefs
 
     @property
     def coefs(self):
-        return self._coefs
+        return self._coefs.ravel()
 
     @property
     def coefs_X(self):
         return self.params[1:, :]
 
     @property
     def intercept(self):
```

### Comparing `stamox-0.1.4/stamox/sample/_bootstrap.py` & `stamox-0.1.5/stamox/sample/_bootstrap.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
     Returns:
         PyTree: The return value of `call` on each bootstrap sample.
 
     Example:
         >>> import jax.numpy as jnp
         >>> import jax.random as jrandom
-        >>> from stamox.sample import bootstrap
+        >>> from stamox.functions import bootstrap
         >>> data = jnp.arange(10)
         >>> bootstrap(data, jnp.mean, 3, key=key)
         Array([5.7000003, 3.9      , 4.6      ], dtype=float32)
 
     """
     samples = bootstrap_sample(data, num_samples=num_samples, key=key)
     return filter_jit(filter_vmap(lambda x: call(x)))(samples)
```

### Comparing `stamox-0.1.4/stamox/sample/_jackknife.py` & `stamox-0.1.5/stamox/sample/_jackknife.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,14 @@
         call (Callable[..., ReturnValue]): A function to be applied to each sample.
 
     Returns:
         PyTree: The jackknife estimate of the data set.
 
     Example:
         >>> import jax.numpy as jnp
-        >>> from stamox.sample import jackknife
+        >>> from stamox.functions import jackknife
         >>> data = jnp.arange(3)
         >>> jackknife(data, lambda x: jnp.mean(x))
         Array([1.5, 1. , 0.5], dtype=float32)
     """
     samples = jackknife_sample(data)
     return filter_jit(filter_vmap(lambda x: call(x)))(samples)
```

### Comparing `stamox-0.1.4/stamox/transformation.py` & `stamox-0.1.5/stamox/transformation.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/stamox.egg-info/PKG-INFO` & `stamox-0.1.5/stamox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stamox
-Version: 0.1.4
+Version: 0.1.5
 Summary: Accelerate Your Statistical Analysis with JAX.
 Home-page: https://github.com/jiayaobo/stamox
 Author: Jia Yaobo
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -44,15 +44,15 @@
 ![benchmark](./benchmark/benchmark2.png)
 
 ## Installation
 
 ```bash
 pip install -U stamox
 # or
-pip install git+[stamox](https://github.com/JiaYaobo/stamox.git)
+pip install git+https://github.com/JiaYaobo/stamox.git
 ```
 
 ## Documentation
 
 More comprehensive introduction and examples can be found in the [documentation](https://jiayaobo.github.io/stamox/).
 
 ## Quick Start
```

### Comparing `stamox-0.1.4/stamox.egg-info/SOURCES.txt` & `stamox-0.1.5/stamox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 stamox/core/jit.py
 stamox/core/maps.py
 stamox/core/pipe.py
 stamox/correlation/__init__.py
 stamox/correlation/_cor.py
 stamox/correlation/_pearson.py
 stamox/correlation/_spearman.py
+stamox/decomposition/__init__.py
+stamox/decomposition/_pca.py
 stamox/distribution/__init__.py
 stamox/distribution/_beta.py
 stamox/distribution/_binomial.py
 stamox/distribution/_cauchy.py
 stamox/distribution/_chisq.py
 stamox/distribution/_ecdf.py
 stamox/distribution/_exp.py
@@ -42,16 +44,14 @@
 stamox/distribution/_pareto.py
 stamox/distribution/_poisson.py
 stamox/distribution/_t.py
 stamox/distribution/_uniform.py
 stamox/distribution/_utils.py
 stamox/distribution/_weibull.py
 stamox/experimental/__init__.py
-stamox/experimental/decomposition/__init__.py
-stamox/experimental/decomposition/_pca.py
 stamox/experimental/maps/__init__.py
 stamox/experimental/maps/auto_map.py
 stamox/experimental/maps/cube_map.py
 stamox/formula/__init__.py
 stamox/formula/_formula.py
 stamox/hypothesis/__init__.py
 stamox/hypothesis/_bartlett.py
```

### Comparing `stamox-0.1.4/tests/test_basic.py` & `stamox-0.1.5/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `stamox-0.1.4/tests/test_transformation.py` & `stamox-0.1.5/tests/test_transformation.py`

 * *Files identical despite different names*

