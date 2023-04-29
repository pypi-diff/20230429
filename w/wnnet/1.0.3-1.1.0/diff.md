# Comparing `tmp/wnnet-1.0.3.tar.gz` & `tmp/wnnet-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wnnet-1.0.3.tar", last modified: Mon Apr  3 15:13:40 2023, max compression
+gzip compressed data, was "wnnet-1.1.0.tar", last modified: Sat Apr 29 20:39:34 2023, max compression
```

## Comparing `wnnet-1.0.3.tar` & `wnnet-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-03 15:13:40.937894 wnnet-1.0.3/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-19 23:05:37.000000 wnnet-1.0.3/LICENSE.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      188 2023-02-20 16:56:48.000000 wnnet-1.0.3/MANIFEST.in
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-04-03 15:13:40.938246 wnnet-1.0.3/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      837 2023-03-18 14:20:36.000000 wnnet-1.0.3/README.rst
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2023-04-03 15:13:40.940185 wnnet-1.0.3/setup.cfg
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6056 2023-03-18 14:18:12.000000 wnnet-1.0.3/setup.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-03 15:13:40.929406 wnnet-1.0.3/wnnet/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      279 2023-04-03 15:13:03.000000 wnnet-1.0.3/wnnet/__about__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      197 2023-03-18 14:18:12.000000 wnnet-1.0.3/wnnet/__init__.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      993 2023-02-20 16:43:35.000000 wnnet-1.0.3/wnnet/consts.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    12680 2023-04-03 15:00:42.000000 wnnet-1.0.3/wnnet/flows.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)    46445 2023-04-03 15:07:47.000000 wnnet-1.0.3/wnnet/graph.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     6795 2023-02-20 16:43:35.000000 wnnet-1.0.3/wnnet/net.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     4155 2023-02-20 16:43:35.000000 wnnet-1.0.3/wnnet/nuc.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     3531 2023-02-20 16:43:35.000000 wnnet-1.0.3/wnnet/reac.py
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      864 2023-01-19 23:05:37.000000 wnnet-1.0.3/wnnet/zones.py
-drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-03 15:13:40.936695 wnnet-1.0.3/wnnet.egg-info/
--rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-04-03 15:13:40.000000 wnnet-1.0.3/wnnet.egg-info/PKG-INFO
--rw-r--r--   0 bradleymeyer   (501) staff       (20)      335 2023-04-03 15:13:40.000000 wnnet-1.0.3/wnnet.egg-info/SOURCES.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-04-03 15:13:40.000000 wnnet-1.0.3/wnnet.egg-info/dependency_links.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)       66 2023-04-03 15:13:40.000000 wnnet-1.0.3/wnnet.egg-info/requires.txt
--rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2023-04-03 15:13:40.000000 wnnet-1.0.3/wnnet.egg-info/top_level.txt
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-29 20:39:34.469135 wnnet-1.1.0/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    35147 2023-01-19 23:05:37.000000 wnnet-1.1.0/LICENSE.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      188 2023-02-20 16:56:48.000000 wnnet-1.1.0/MANIFEST.in
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-04-29 20:39:34.469490 wnnet-1.1.0/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      837 2023-03-18 14:20:36.000000 wnnet-1.1.0/README.rst
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      107 2023-04-29 20:39:34.471778 wnnet-1.1.0/setup.cfg
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     6056 2023-03-18 14:18:12.000000 wnnet-1.1.0/setup.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-29 20:39:34.455627 wnnet-1.1.0/wnnet/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      279 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/__about__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      197 2023-03-18 14:18:12.000000 wnnet-1.1.0/wnnet/__init__.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      993 2023-02-20 16:43:35.000000 wnnet-1.1.0/wnnet/consts.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    15337 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/flows.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)    47384 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/graph.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     7120 2023-04-29 20:37:57.000000 wnnet-1.1.0/wnnet/net.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     4155 2023-02-20 16:43:35.000000 wnnet-1.1.0/wnnet/nuc.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     3531 2023-02-20 16:43:35.000000 wnnet-1.1.0/wnnet/reac.py
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      864 2023-01-19 23:05:37.000000 wnnet-1.1.0/wnnet/zones.py
+drwxr-xr-x   0 bradleymeyer   (501) staff       (20)        0 2023-04-29 20:39:34.465451 wnnet-1.1.0/wnnet.egg-info/
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)     1623 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/PKG-INFO
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)      335 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/SOURCES.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        1 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/dependency_links.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)       66 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/requires.txt
+-rw-r--r--   0 bradleymeyer   (501) staff       (20)        6 2023-04-29 20:39:34.000000 wnnet-1.1.0/wnnet.egg-info/top_level.txt
```

### Comparing `wnnet-1.0.3/LICENSE.txt` & `wnnet-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/PKG-INFO` & `wnnet-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnnet
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python project to handle webnucleo reaction networks
 Home-page: https://github.com/mbradle/wnnet
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnnet/issues
 Project-URL: Source, https://github.com/mbradle/wnnet/
```

### Comparing `wnnet-1.0.3/README.rst` & `wnnet-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/setup.py` & `wnnet-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/wnnet/consts.py` & `wnnet-1.1.0/wnnet/consts.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/wnnet/flows.py` & `wnnet-1.1.0/wnnet/flows.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 """This module computes various reaction flows in a network."""
 
 import wnutils.xml as wx
 import numpy as np
 
 
 def _compute_flows_for_valid_reactions(
-    net, t9, rho, mass_fractions, valid_reactions, dups, nuc_xpath, reac_xpath
+    net,
+    t9,
+    rho,
+    mass_fractions,
+    valid_reactions,
+    dups,
+    nuc_xpath,
+    reac_xpath,
+    user_funcs,
 ):
 
     result = {}
 
     for reaction in valid_reactions:
-        my_reaction = valid_reactions[reaction]
+        _reaction = valid_reactions[reaction]
 
-        forward, reverse = net.compute_rates_for_reaction(reaction, t9)
+        forward, reverse = net.compute_rates_for_reaction(
+            reaction, t9, user_funcs=user_funcs
+        )
 
-        forward *= np.power(rho, len(my_reaction.nuclide_reactants) - 1)
+        forward *= np.power(rho, len(_reaction.nuclide_reactants) - 1)
         forward /= dups[reaction][0]
         forward *= _compute_abundance_product(
-            net, mass_fractions, my_reaction.nuclide_reactants
+            net, mass_fractions, _reaction.nuclide_reactants
         )
 
         if not net.is_weak_reaction(reaction):
-            reverse *= np.power(rho, len(my_reaction.nuclide_products) - 1)
+            reverse *= np.power(rho, len(_reaction.nuclide_products) - 1)
             reverse /= dups[reaction][1]
             reverse *= _compute_abundance_product(
-                net, mass_fractions, my_reaction.nuclide_products
+                net, mass_fractions, _reaction.nuclide_products
             )
         else:
             reverse = 0
 
         result[reaction] = (forward, reverse)
 
     return result
 
 
-def compute_flows(net, t9, rho, mass_fractions, nuc_xpath="", reac_xpath=""):
+def compute_flows(
+    net, t9, rho, mass_fractions, nuc_xpath="", reac_xpath="", user_funcs=""
+):
     """A routine to compute flows for a given set of mass fractions at the input temperature and density.
 
     Args:
         ``net``: A wnnet network.
 
         ``t9`` (:obj:`float`):  The temperature in 10\ :sup:`9` K at which to compute the flows.
 
@@ -51,33 +63,49 @@
         to select nuclides for flow computations.  Defaults to all
         species.
 
         ``reac_xpath`` (:obj:`str`, optional): XPath expression
         to select reactions for flow computations.  Defaults to all
         reactions.
 
+        ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined
+        functions associated with a user_rate key.
+        The prototype for each
+        user rate function should be (*reaction*, *t9*), where
+        *t9* is the temperature in billions of Kelvin and *reaction*
+        is a `wnutils <https://wnutils.readthedocs.io>`_ reaction
+        instance.  Other data can be bound to the function.
+
     Returns:
         A :obj:`dict` of reactions with each
         item in the dictionary a tuple giving the forward and
         reverse flow.
 
     """
 
     valid_reactions = net.get_valid_reactions(
         nuc_xpath=nuc_xpath, reac_xpath=reac_xpath
     )
 
     dups = net.compute_duplicate_factors()
 
     return _compute_flows_for_valid_reactions(
-        net, t9, rho, mass_fractions, valid_reactions, dups, nuc_xpath, reac_xpath
+        net,
+        t9,
+        rho,
+        mass_fractions,
+        valid_reactions,
+        dups,
+        nuc_xpath,
+        reac_xpath,
+        user_funcs,
     )
 
 
-def compute_flows_for_zones(net, zones, nuc_xpath="", reac_xpath=""):
+def compute_flows_for_zones(net, zones, nuc_xpath="", reac_xpath="", user_funcs=""):
     """A routine to compute flows for a set of zones.
 
     Args:
         ``net``: A wnnet network.
 
         ``zones`` (:obj:`dict`): A dictionary of `wnutils <https://wnutils.readthedocs.io>`_ *zone data*.
 
@@ -85,14 +113,23 @@
         to select nuclides for flow computations.  Defaults to all
         species.
 
         ``reac_xpath`` (:obj:`str`, optional): XPath expression
         to select reactions for flow computations.  Defaults to all
         reactions.
 
+        ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined
+        functions associated with a user_rate key.
+        The prototype for each
+        user rate function should be (*reaction*, *t9*, *zone*), where
+        *t9* is the temperature in billions of Kelvin and *reaction* and
+        *zone* are `wnutils <https://wnutils.readthedocs.io>`_ reaction and
+        zone instances.  Other data can be bound to the function.
+
+
     Returns:
         A :obj:`dict` of flows for each zone.  The data for
         each zone are themselves a :obj:`dict` of reactions with each
         item in the dictionary a tuple giving the forward and
         reverse flow.
 
     """
@@ -104,25 +141,35 @@
     )
 
     dups = net.compute_duplicate_factors()
 
     for zone in zones:
         s_t9 = "t9"
         s_rho = "rho"
-        props = zones[zone]["properties"]
+        _zone = zones[zone]
+        props = _zone["properties"]
         if s_t9 in props and s_rho in props:
+            t9 = float(props[s_t9])
+            rho = float(props[s_rho])
+            _user_funcs = {}
+            if user_funcs:
+                for func in user_funcs:
+                    _user_funcs[func] = lambda reaction, t9, func=func: user_funcs[
+                        func
+                    ](reaction, t9, _zone)
             zone_flows[zone] = _compute_flows_for_valid_reactions(
                 net,
-                float(props[s_t9]),
-                float(props[s_rho]),
-                zones[zone]["mass fractions"],
+                t9,
+                rho,
+                _zone["mass fractions"],
                 valid_reactions,
                 dups,
                 nuc_xpath,
                 reac_xpath,
+                _user_funcs,
             )
 
     return zone_flows
 
 
 def _compute_link_flows_for_valid_reactions(
     net,
@@ -130,32 +177,35 @@
     rho,
     mass_fractions,
     valid_reactions,
     dups,
     scale,
     nuc_xpath,
     reac_xpath,
+    user_funcs,
     direction,
     order,
 ):
     nuclides = net.get_nuclides()
 
     link_flows = {}
 
     for reaction in valid_reactions:
         tup_array = []
-        my_reaction = valid_reactions[reaction]
+        _reaction = valid_reactions[reaction]
 
-        reactants = my_reaction.nuclide_reactants
-        products = my_reaction.nuclide_products
+        reactants = _reaction.nuclide_reactants
+        products = _reaction.nuclide_products
 
-        forward, reverse = net.compute_rates_for_reaction(reaction, t9)
+        forward, reverse = net.compute_rates_for_reaction(
+            reaction, t9, user_funcs=user_funcs
+        )
 
         if direction == "forward" or direction == "both" or direction == "all":
-            forward *= np.power(rho, len(my_reaction.nuclide_reactants) - 1)
+            forward *= np.power(rho, len(_reaction.nuclide_reactants) - 1)
             forward /= dups[reaction][0]
 
             for i in range(len(reactants)):
                 source = reactants[i]
                 p_source = _compute_abundance_product(
                     net, mass_fractions, reactants, exclude_index=i
                 )
@@ -172,15 +222,15 @@
                             tup = (source, target, -forward * p_source * scale)
                         else:
                             tup = (target, source, -forward * p_source * scale)
                         tup_array.append(tup)
 
         if not net.is_weak_reaction(reaction):
             if direction == "reverse" or direction == "both" or direction == "all":
-                reverse *= np.power(rho, len(my_reaction.nuclide_products) - 1)
+                reverse *= np.power(rho, len(_reaction.nuclide_products) - 1)
                 reverse /= dups[reaction][1]
 
                 for i in range(len(products)):
                     source = products[i]
                     p_source = _compute_abundance_product(
                         net, mass_fractions, products, exclude_index=i
                     )
@@ -207,14 +257,15 @@
 def compute_link_flows(
     net,
     t9,
     rho,
     mass_fractions,
     nuc_xpath="",
     reac_xpath="",
+    user_funcs="",
     direction="both",
     order="normal",
 ):
     """A routine to compute link flows for a given set of mass fractions at the input temperature and density.
 
     Args:
         ``net``: A wnnet network.
@@ -229,14 +280,22 @@
         to select nuclides for flow computations.  Defaults to all
         species.
 
         ``reac_xpath`` (:obj:`str`, optional): XPath expression
         to select reactions for flow computations.  Defaults to all
         reactions.
 
+        ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined
+        functions associated with a user_rate key.
+        The prototype for each
+        user rate function should be (*reaction*, *t9*), where
+        *t9* is the temperature in billions of Kelvin and *reaction*
+        is a `wnutils <https://wnutils.readthedocs.io>`_ reaction
+        instance.  Other data can be bound to the function.
+
         ``direction`` (:obj:`str`, optional):  A string indicating the direction of the links ("forward", from reactants to products; "reverse", from products to reactants; "both", both "forward" and "reverse").  Default is "both".
 
         ``order`` (:obj:`str`, optional):  A string indicating the order of the links.  Default is *normal*, in which the *source* and *target* of the link are in the time-forward direction of the reaction.  For *reversed*, the *source* and *target* are in the opposite of the time-forward direction of the reaction such that the *target* is the *contribution* to the *source* over some interval.
 
     Returns:
         A :obj:`dict` of reactions with each
         item in the dictionary an array of three-element :obj:`tuple` objects.
@@ -268,24 +327,26 @@
         rho,
         mass_fractions,
         valid_reactions,
         dups,
         scale,
         nuc_xpath,
         reac_xpath,
+        user_funcs,
         direction,
         order,
     )
 
 
 def compute_link_flows_for_zones(
     net,
     zones,
     nuc_xpath="",
     reac_xpath="",
+    user_funcs="",
     direction="both",
     include_dt=False,
     order="normal",
 ):
     """A routine to compute link flows for a set of zones.
 
     Args:
@@ -297,14 +358,22 @@
         to select nuclides for flow computations.  Defaults to all
         species.
 
         ``reac_xpath`` (:obj:`str`, optional): XPath expression
         to select reactions for flow computations.  Defaults to all
         reactions.
 
+        ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined
+        functions associated with a user_rate key.
+        The prototype for each
+        user rate function should be (*reaction*, *t9*, *zone*), where
+        *t9* is the temperature in billions of Kelvin and *reaction* and
+        *zone* are `wnutils <https://wnutils.readthedocs.io>`_ reaction and
+        zone instances.  Other data can be bound to the function.
+
         ``direction`` (:obj:`str`, optional):  A string indicating the direction of the links ("forward", from reactants to products; "reverse", from products to reactants; "both", both "forward" and "reverse").  Default is "both".
 
         ``include_dt`` (:obj:`bool`, optional):  Boolean determining whether to include the *dt* (time interval) in the flow (True) or not (False).  Default is False.
 
         ``order`` (:obj:`str`, optional):  A string indicating the order of the links.  Default is *normal*, in which the *source* and *target* of the link are in the time-forward direction of the reaction.  For *reversed*, the *source* and *target* are in the opposite of the time-forward direction of the reaction such that the *target* is the *contribution* to the *source* over some interval.
 
     Returns:
@@ -339,24 +408,31 @@
         props = zones[zone]["properties"]
         f = {}
         if s_t9 in props and s_rho in props:
             if include_dt:
                 scale = float(props[s_dt])
             else:
                 scale = 1
+            _user_funcs = {}
+            if user_funcs:
+                for func in user_funcs:
+                    _user_funcs[func] = lambda reaction, t9, func=func: user_funcs[
+                        func
+                    ](reaction, t9, zones[zone])
             f = _compute_link_flows_for_valid_reactions(
                 net,
                 float(props[s_t9]),
                 float(props[s_rho]),
                 zones[zone]["mass fractions"],
                 valid_reactions,
                 dups,
                 scale,
                 nuc_xpath,
                 reac_xpath,
+                _user_funcs,
                 direction,
                 order,
             )
 
             zone_link_flows[zone] = f
 
     return zone_link_flows
```

### Comparing `wnnet-1.0.3/wnnet/graph.py` & `wnnet-1.1.0/wnnet/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,23 +573,23 @@
 ):
 
     nuclides = net.get_nuclides()
     reactions = net.get_reactions()
 
     # Solar species
 
-    my_solar_species = solar_species
+    _solar_species = solar_species
     if not solar_species:
-        my_solar_species = get_solar_species()
+        _solar_species = get_solar_species()
 
     # Solar species
 
-    my_solar_species = solar_species
+    _solar_species = solar_species
     if not solar_species:
-        my_solar_species = get_solar_species()
+        _solar_species = get_solar_species()
 
     DG = nx.MultiDiGraph()
 
     for nuc in nuclides:
         DG.add_node(nuc, shape="box", fontsize=16)
 
     for r in f:
@@ -639,15 +639,15 @@
 
     _apply_graph_attributes(DG, graph_attributes)
 
     _apply_node_attributes(DG, node_attributes)
 
     _apply_edge_attributes(DG, edge_attributes)
 
-    _apply_solar_node_attributes(DG, my_solar_species, solar_node_attributes)
+    _apply_solar_node_attributes(DG, _solar_species, solar_node_attributes)
 
     _apply_special_node_attributes(DG, special_node_attributes)
 
     # Subgraph and maximum flow within subgraph
 
     S = nx.subgraph(DG, subset_nuclides)
 
@@ -657,35 +657,35 @@
 
     f_max = 0
 
     if len(w) > 0:
         f_max = max(w.items(), key=operator.itemgetter(1))[1]
 
         if not scale_edge_weight_func:
-            my_scale_edge_weight_func = lambda edge_data: scale_edge_weight(
+            _scale_edge_weight_func = lambda edge_data: scale_edge_weight(
                 edge_data, f_max, scale, threshold
             )
         else:
-            my_scale_edge_weight_func = lambda edge_data: scale_edge_weight_func(
+            _scale_edge_weight_func = lambda edge_data: scale_edge_weight_func(
                 edge_data, f_max, scale, threshold
             )
 
         remove_edges = []
         for edge in DG.edges:
-            if not my_scale_edge_weight_func(DG.get_edge_data(*edge)):
+            if not _scale_edge_weight_func(DG.get_edge_data(*edge)):
                 remove_edges.append(edge)
 
         DG.remove_edges_from(remove_edges)
 
     # Remove isolated nodes if desired
 
     if not allow_isolated_species:
         isolated_nodes = list(nx.isolates(DG))
         for node in isolated_nodes:
-            if node not in my_solar_species:
+            if node not in _solar_species:
                 DG.remove_node(node)
 
     # Restore anchors
 
     for anchor in anchors:
         if anchor not in DG.nodes:
             DG.add_node(anchor, style="invis")
@@ -711,14 +711,15 @@
     net,
     t9,
     rho,
     mass_fractions,
     flow_type="net",
     induced_nuc_xpath="",
     induced_reac_xpath="",
+    user_funcs="",
     reaction_color_tuples=None,
     threshold=0.01,
     scale=10,
     state_scaling=0.325,
     allow_isolated_species=False,
     title_func=None,
     node_label_func=None,
@@ -745,14 +746,22 @@
 
         ``induced_nuc_xpath`` (:obj:`str`, optional): An XPath expression to select the subset of nuclides in the graph.  The default is all species in the network.
 
         ``induced_reac_xpath`` (:obj:`str`, optional): An XPath expression to select the subset of reactions in the graph.  The default is all reactions in the network.
 
         ``reaction_color_tuples`` (:obj:`tuple`, optional): A tuple to select arc colors for reaction types.  The first member of the tuple is an XPath expression to select the reaction type while the second member is a string giving the color for that reaction type.  The default is that all arcs are black.
 
+        ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined
+        functions associated with a user_rate key.
+        The prototype for each
+        user rate function should be (*reaction*, *t9*), where
+        *t9* is the temperature in billions of Kelvin and *reaction*
+        is a `wnutils <https://wnutils.readthedocs.io>`_ reaction
+        instance.  Other data can be bound to the function.
+
         ``threshold`` (:obj:`float`, optional):  The minimum flow (relative to the maximum flow) to be shown on the graph
         
         ``scale`` (:obj:`float`, optional):  Scaling factor for the maximum weight arc.
         
         ``state_scaling`` (:obj:`float`, optional):  Scaling factor for isomeric states.
         
         ``allow_isolated_species`` (:obj:`bool`, optional):  Boolean to choose whether to allow isolated species (ones without incoming or outgoing arcs) in the graph.
@@ -796,48 +805,55 @@
     Returns:
         A `networkx multidigraph <https://networkx.org/documentation/stable/reference/classes/multidigraph.html>`_ showing the flows.
      
 
     """
     assert flow_type == "net" or flow_type == "full"
 
-    f = wf.compute_flows(net, t9, rho, mass_fractions, reac_xpath=induced_reac_xpath)
+    f = wf.compute_flows(
+        net,
+        t9,
+        rho,
+        mass_fractions,
+        reac_xpath=induced_reac_xpath,
+        user_funcs=user_funcs,
+    )
 
     # Get the subset of nuclides to view in the graph.  Get anchors.
 
     subset_nuclides, anchors = _get_subset_and_anchors(net, induced_nuc_xpath)
 
     # Title
 
     if not title_func:
-        my_title_func = lambda f_max: make_t9_rho_flow_string(f_max, t9, rho)
+        _title_func = lambda f_max: make_t9_rho_flow_string(f_max, t9, rho)
     else:
-        my_title_func = title_func
+        _title_func = title_func
 
     # Node label
 
     if not node_label_func:
         g_names = net.xml.get_graphviz_names(subset_nuclides)
-        my_node_label_func = lambda name: make_node_label(name, g_names)
+        _node_label_func = lambda name: make_node_label(name, g_names)
     else:
-        my_node_label_func = node_label_func
+        _node_label_func = node_label_func
 
     return _create_flow_graph(
         net,
         f,
         flow_type,
         subset_nuclides,
         anchors,
         allow_isolated_species,
         reaction_color_tuples,
         threshold,
         scale,
         state_scaling,
-        my_title_func,
-        my_node_label_func,
+        _title_func,
+        _node_label_func,
         scale_edge_weight_func,
         graph_attributes,
         node_attributes,
         edge_attributes,
         solar_species,
         solar_node_attributes,
         special_node_attributes,
@@ -847,14 +863,15 @@
 def create_zone_flow_graphs(
     net,
     zones,
     flow_type="net",
     induced_nuc_xpath="",
     induced_reac_xpath="",
     reaction_color_tuples=None,
+    user_funcs="",
     threshold=0.01,
     scale=10,
     state_scaling=0.325,
     allow_isolated_species=False,
     title_func=None,
     zone_node_label_func=None,
     scale_edge_weight_func=None,
@@ -874,14 +891,22 @@
 
         ``flow_type`` (:obj:`str`, optional): A string giving the flow type to be presented.  The possible values are `net`, which shows the forward minus the reverse flow (or the opposite if the reverse flow is larger), and `full`, which shows both the foward and reverse flows.
 
         ``induced_nuc_xpath`` (:obj:`str`, optional): An XPath expression to select the subset of nuclides in the graph.  The default is all species in the network.
 
         ``induced_reac_xpath`` (:obj:`str`, optional): An XPath expression to select the subset of reactions in the graph.  The default is all reactions in the network.
 
+        ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined
+        functions associated with a user_rate key.
+        The prototype for each
+        user rate function should be (*reaction*, *t9*, *zone*), where
+        *t9* is the temperature in billions of Kelvin and *reaction* and
+        *zone* are `wnutils <https://wnutils.readthedocs.io>`_ reaction and
+        zone instances.  Other data can be bound to the function.
+
         ``reaction_color_tuples`` (:obj:`tuple`, optional): A tuple to select arc colors for reaction types.  The first member of the tuple is an XPath expression to select the reaction type while the second member is a string giving the color for that reaction type.  The default is that all arcs are black.
 
         ``threshold`` (:obj:`float`, optional):  The minimum flow (relative to the maximum flow) to be shown on the graph
         
         ``scale`` (:obj:`float`, optional):  Scaling factor for the maximum weight arc.
         
         ``state_scaling`` (:obj:`float`, optional):  Scaling factor for isomeric states.
@@ -937,40 +962,42 @@
         A :obj:`dict` of `networkx multidigraphs <https://networkx.org/documentation/stable/reference/classes/multidigraph.html>`_ showing the flows.  The keys are the zone labels.
      
 
     """
 
     result = {}
 
-    f = wf.compute_flows_for_zones(net, zones, reac_xpath=induced_reac_xpath)
+    f = wf.compute_flows_for_zones(
+        net, zones, reac_xpath=induced_reac_xpath, user_funcs=user_funcs
+    )
 
     subset_nuclides, anchors = _get_subset_and_anchors(net, induced_nuc_xpath)
 
     # Loop on zones
 
     for zone in f:
 
         # Title
 
         if not title_func:
-            my_title_func = lambda f_max: make_time_t9_rho_flow_string(
+            _title_func = lambda f_max: make_time_t9_rho_flow_string(
                 zones[zone], zone, f_max
             )
         else:
-            my_title_func = lambda f_max: title_func(zones[zone], zone, f_max)
+            _title_func = lambda f_max: title_func(zones[zone], zone, f_max)
 
         # Node label
 
         g_names = net.xml.get_graphviz_names(subset_nuclides)
         if not zone_node_label_func:
-            my_zone_node_label_func = lambda name: make_zone_node_label(
+            _zone_node_label_func = lambda name: make_zone_node_label(
                 zones[zone], zone, name, g_names
             )
         else:
-            my_zone_node_label_func = lambda name: zone_node_label_func(
+            _zone_node_label_func = lambda name: zone_node_label_func(
                 zones[zone], zone, name
             )
 
         # Create graph
 
         result[zone] = _create_flow_graph(
             net,
@@ -979,16 +1006,16 @@
             subset_nuclides,
             anchors,
             allow_isolated_species,
             reaction_color_tuples,
             threshold,
             scale,
             state_scaling,
-            my_title_func,
-            my_zone_node_label_func,
+            _title_func,
+            _zone_node_label_func,
             scale_edge_weight_func,
             graph_attributes,
             node_attributes,
             edge_attributes,
             solar_species,
             solar_node_attributes,
             special_node_attributes,
@@ -1116,22 +1143,22 @@
     # Subgraph
 
     S = nx.subgraph(DG, val)
 
     # Node label
 
     if node_label_func:
-        my_node_label_func = node_label_func
+        _node_label_func = node_label_func
     else:
         g_names = net.xml.get_graphviz_names(list(S.nodes.keys()))
-        my_node_label_func = lambda name: make_node_label(name, g_names)
+        _node_label_func = lambda name: make_node_label(name, g_names)
 
     for node in S.nodes:
         S.nodes[node]["pos"] = _get_pos_string(net, node, state_scaling)
-        S.nodes[node]["label"] = my_node_label_func(node)
+        S.nodes[node]["label"] = _node_label_func(node)
 
     _color_edges(S, net, reaction_color_tuples)
 
     return S
 
 
 def _create_integrated_current_graph(
@@ -1156,23 +1183,23 @@
     special_node_attributes,
 ):
     nuclides = net.get_nuclides()
     reactions = net.get_reactions()
 
     # Solar species
 
-    my_solar_species = solar_species
+    _solar_species = solar_species
     if not solar_species:
-        my_solar_species = get_solar_species()
+        _solar_species = get_solar_species()
 
     # Solar species
 
-    my_solar_species = solar_species
+    _solar_species = solar_species
     if not solar_species:
-        my_solar_species = get_solar_species()
+        _solar_species = get_solar_species()
 
     subset_nuclides, anchors = _get_subset_and_anchors(net, induced_nuc_xpath)
 
     props = zone["properties"]
 
     DG = nx.MultiDiGraph()
 
@@ -1206,15 +1233,15 @@
 
     _apply_graph_attributes(DG, graph_attributes)
 
     _apply_node_attributes(DG, node_attributes)
 
     _apply_edge_attributes(DG, edge_attributes)
 
-    _apply_solar_node_attributes(DG, my_solar_species, solar_node_attributes)
+    _apply_solar_node_attributes(DG, _solar_species, solar_node_attributes)
 
     _apply_special_node_attributes(DG, special_node_attributes)
 
     # Subgraph and maximum flow within subgraph
 
     S = nx.subgraph(DG, subset_nuclides)
 
@@ -1224,35 +1251,35 @@
 
     f_max = 0
 
     if len(w) > 0:
         f_max = max(w.items(), key=operator.itemgetter(1))[1]
 
         if not scale_edge_weight_func:
-            my_scale_edge_weight_func = lambda edge_data: scale_edge_weight(
+            _scale_edge_weight_func = lambda edge_data: scale_edge_weight(
                 edge_data, f_max, scale, threshold
             )
         else:
-            my_scale_edge_weight_func = lambda edge_data: scale_edge_weight_func(
+            _scale_edge_weight_func = lambda edge_data: scale_edge_weight_func(
                 edge_data, f_max, scale, threshold
             )
 
         remove_edges = []
         for edge in DG.edges:
-            if not my_scale_edge_weight_func(DG.get_edge_data(*edge)):
+            if not _scale_edge_weight_func(DG.get_edge_data(*edge)):
                 remove_edges.append(edge)
 
         DG.remove_edges_from(remove_edges)
 
     # Remove isolated nodes if desired
 
     if not allow_isolated_species:
         isolated_nodes = list(nx.isolates(DG))
         for node in isolated_nodes:
-            if node not in my_solar_species:
+            if node not in _solar_species:
                 DG.remove_node(node)
 
     # Restore anchors
 
     for anchor in anchors:
         if anchor not in DG.nodes:
             DG.add_node(anchor, style="invis")
@@ -1372,45 +1399,45 @@
     subset_nuclides, anchors = _get_subset_and_anchors(net, induced_nuc_xpath)
 
     for zone in zones:
 
         # Title
 
         if not title_func:
-            my_title_func = lambda f_max: make_time_t9_rho_current_string(
+            _title_func = lambda f_max: make_time_t9_rho_current_string(
                 zones[zone], zone, f_max
             )
         else:
-            my_title_func = lambda f_max: title_func(zones[zone], zone, f_max)
+            _title_func = lambda f_max: title_func(zones[zone], zone, f_max)
 
         # Node label
 
         g_names = net.xml.get_graphviz_names(subset_nuclides)
         if not zone_node_label_func:
-            my_zone_node_label_func = lambda name: make_zone_node_label(
+            _zone_node_label_func = lambda name: make_zone_node_label(
                 zones[zone], zone, name, g_names
             )
         else:
-            my_zone_node_label_func = lambda name: zone_node_label_func(
+            _zone_node_label_func = lambda name: zone_node_label_func(
                 zones[zone], zone, name
             )
 
         result[zone] = _create_integrated_current_graph(
             net,
             zones[zone],
             subset_nuclides,
             induced_nuc_xpath,
             induced_reac_xpath,
             reaction_color_tuples,
             threshold,
             scale,
             state_scaling,
             allow_isolated_species,
-            my_title_func,
-            my_zone_node_label_func,
+            _title_func,
+            _zone_node_label_func,
             scale_edge_weight_func,
             graph_attributes,
             edge_attributes,
             node_attributes,
             solar_species,
             solar_node_attributes,
             special_node_attributes,
```

### Comparing `wnnet-1.0.3/wnnet/net.py` & `wnnet-1.1.0/wnnet/net.py`

 * *Files 13% similar despite different names*

```diff
@@ -130,32 +130,34 @@
         nuclides = self.get_nuclides(nuc_xpath=nuc_xpath)
         reaction = self.get_reactions()[name]
         for sp in reaction.nuclide_reactants + reaction.nuclide_products:
             if sp not in nuclides:
                 return False
         return True
 
-    def compute_rates_for_reaction(self, name, t9):
+    def compute_rates_for_reaction(self, name, t9, user_funcs=""):
         """Method to compute the forward and reverse rates for a valid reaction.
 
         Args:
             ``name`` (:obj:`str`):  A string giving the reaction.
 
             ``t9`` (:obj:`float`):  The temperature in 10\ :sup:`9` K at which to compute the rates.
 
+            ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined functions associated with a user_rate key.
+
         Returns:
             A two-element :obj:`tuple` with the first element being the forward rate and the second element being the reverse rate.  If the reaction is not valid, returns None.
 
         """
 
         if not self.is_valid_reaction(name):
             return None
 
         reaction = self.get_reactions()[name]
-        forward = reaction.compute_rate(t9)
+        forward = reaction.compute_rate(t9, user_funcs=user_funcs)
 
         if self.is_weak_reaction(name):
             return (forward, 0)
 
         d_exp = 0
 
         for sp in reaction.nuclide_reactants:
@@ -169,33 +171,34 @@
         if d_exp > 300.0:
             return (0, 0)
 
         tup = self.compute_reaction_duplicate_factors(name)
 
         return (forward, np.exp(d_exp) * (tup[1] / tup[0]) * forward)
 
-    def compute_rates(self, t9, nuc_xpath="", reac_xpath=""):
+    def compute_rates(self, t9, nuc_xpath="", reac_xpath="", user_funcs=""):
         """Method to compute the forward and reverse rates for valid reactions in a network.
 
         Args:
             ``t9`` (:obj:`float`):  The temperature in 10\ :sup:`9` K at which to compute the rates.
 
             ``nuc_xpath`` (:obj:`str`, optional):  An XPath expression to select nuclides.  Default is all nuclides.
 
             ``reac_xpath`` (:obj:`str`, optional):  An XPath expression to select reactions.  Default is all reactions.
 
+            ``user_funcs`` (:obj:`dict`, optional): A dictionary of user-defined functions associated with a user_rate key.
 
         Returns:
             A :obj:`dict` containing the rates.  The key is the reaction string while the value is a two-element  :obj:`tuple` with the first element being the forward rate and the second element being the reverse rate.
 
         """
 
         v_reactions = self.get_valid_reactions(
             nuc_xpath=nuc_xpath, reac_xpath=reac_xpath
         )
 
         result = {}
 
         for r in v_reactions:
-            result[r] = self.compute_rates_for_reaction(r, t9)
+            result[r] = self.compute_rates_for_reaction(r, t9, user_funcs=user_funcs)
 
         return result
```

### Comparing `wnnet-1.0.3/wnnet/nuc.py` & `wnnet-1.1.0/wnnet/nuc.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/wnnet/reac.py` & `wnnet-1.1.0/wnnet/reac.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/wnnet/zones.py` & `wnnet-1.1.0/wnnet/zones.py`

 * *Files identical despite different names*

### Comparing `wnnet-1.0.3/wnnet.egg-info/PKG-INFO` & `wnnet-1.1.0/wnnet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wnnet
-Version: 1.0.3
+Version: 1.1.0
 Summary: Python project to handle webnucleo reaction networks
 Home-page: https://github.com/mbradle/wnnet
 Author: Clemson University
 Author-email: mbradle@g.clemson.edu
 License: GPLv3+
 Project-URL: Bug Reports, https://github.com/mbradle/wnnet/issues
 Project-URL: Source, https://github.com/mbradle/wnnet/
```

