# Comparing `tmp/pybet-0.5.0.tar.gz` & `tmp/pybet-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybet-0.5.0.tar", max compression
+gzip compressed data, was "pybet-0.6.0.tar", max compression
```

## Comparing `pybet-0.5.0.tar` & `pybet-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.5.0/LICENSE
--rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.5.0/pybet/__init__.py
--rw-r--r--   0        0        0     6745 2023-02-18 00:28:56.232325 pybet-0.5.0/pybet/market.py
--rw-r--r--   0        0        0    11292 2023-02-18 00:28:56.233330 pybet-0.5.0/pybet/odds.py
--rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.5.0/pybet/staking/__init__.py
--rw-r--r--   0        0        0     1496 2023-04-27 22:41:50.387749 pybet-0.5.0/pybet/staking/kelly.py
--rw-r--r--   0        0        0      936 2023-04-27 22:47:41.639108 pybet-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.5.0/README.md
--rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-12-14 21:43:12.915289 pybet-0.6.0/LICENSE
+-rw-r--r--   0        0        0       84 2023-02-18 00:28:56.230892 pybet-0.6.0/pybet/__init__.py
+-rw-r--r--   0        0        0     8032 2023-04-28 22:23:52.695338 pybet-0.6.0/pybet/market.py
+-rw-r--r--   0        0        0    11292 2023-02-18 00:28:56.233330 pybet-0.6.0/pybet/odds.py
+-rw-r--r--   0        0        0       49 2023-02-18 00:28:56.233330 pybet-0.6.0/pybet/staking/__init__.py
+-rw-r--r--   0        0        0     1496 2023-04-27 22:41:50.387749 pybet-0.6.0/pybet/staking/kelly.py
+-rw-r--r--   0        0        0      936 2023-04-29 12:06:24.755196 pybet-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      539 2023-02-18 00:28:56.218112 pybet-0.6.0/README.md
+-rw-r--r--   0        0        0     1389 1970-01-01 00:00:00.000000 pybet-0.6.0/PKG-INFO
```

### Comparing `pybet-0.5.0/LICENSE` & `pybet-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybet-0.5.0/pybet/market.py` & `pybet-0.6.0/pybet/market.py`

 * *Files 10% similar despite different names*

```diff
@@ -157,14 +157,42 @@
 
         odds_to_apply = Odds.percentage(missing_percentage / len(unpriced_runners))
         for runner in unpriced_runners:
             self[runner] = odds_to_apply
 
         return self
 
+    def meld(self, other: Market, other_percentage: float = 50) -> Market:
+        """Melds two markets together so that the odds for each runner are a weighted average of the two markets
+
+        :param other: The market to meld with
+        :type other: Market
+        :param other_percentage: The percentage of the melded market that should be made up of the other market, defaults to 50
+        :type other_percentage: float, optional
+        :raises ValueError: if the two markets do not have the same runners
+        :return: A market with the weighted average odds of the two markets
+        """
+
+        if self.keys() != other.keys():
+            raise ValueError("Markets must have the same runners")
+
+        if 0 <= other_percentage <= 100:
+            raise ValueError("Percentage must be between 0 and 100")
+
+        new_market = Market(zip(self.keys(), [None] * len(self)))
+        market_1 = self.apply_margin(0)
+        market_2 = other.apply_margin(0)
+        for runner in self.keys():
+            new_market[runner] = Odds.percentage(
+                (market_1[runner].to_percentage() * (100 - other_percentage) / 100)
+                + (market_2[runner].to_percentage() * other_percentage / 100)
+            )
+
+        return new_market
+
     def wipe(self) -> Market:
         """Wipe market so that none of the runners have any odds
 
         :return: An empty market
         :rtype: Market
 
         :Example:
```

### Comparing `pybet-0.5.0/pybet/odds.py` & `pybet-0.6.0/pybet/odds.py`

 * *Files identical despite different names*

### Comparing `pybet-0.5.0/pybet/staking/kelly.py` & `pybet-0.6.0/pybet/staking/kelly.py`

 * *Files identical despite different names*

### Comparing `pybet-0.5.0/pyproject.toml` & `pybet-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybet"
-version = "0.5.0"
+version = "0.6.0"
 description = "A library of betting utilities to assist with calculation of bets, stakes and markets"
 license = "GPL-3.0-only"
 authors = ["Robert Peacock <robertjamespeacock@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/peaky76/pybet"
 documentation = "https://pybet.readthedocs.io/"
 keywords = ["betting", "gambling"]
```

### Comparing `pybet-0.5.0/README.md` & `pybet-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pybet-0.5.0/PKG-INFO` & `pybet-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybet
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library of betting utilities to assist with calculation of bets, stakes and markets
 Home-page: https://github.com/peaky76/pybet
 License: GPL-3.0-only
 Keywords: betting,gambling
 Author: Robert Peacock
 Author-email: robertjamespeacock@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
```

