# Comparing `tmp/d3graph-2.4.3.tar.gz` & `tmp/d3graph-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3graph-2.4.3.tar", last modified: Mon Mar 20 18:16:00 2023, max compression
+gzip compressed data, was "d3graph-2.4.4.tar", last modified: Sat Apr 29 17:13:55 2023, max compression
```

## Comparing `d3graph-2.4.3.tar` & `d3graph-2.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-20 18:16:00.412933 d3graph-2.4.3/
--rw-rw-rw-   0        0        0     1700 2022-05-20 19:47:24.000000 d3graph-2.4.3/LICENSE
--rw-rw-rw-   0        0        0       82 2022-05-20 19:47:24.000000 d3graph-2.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6289 2023-03-20 18:16:00.413927 d3graph-2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     5708 2023-03-10 17:10:19.000000 d3graph-2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-20 18:16:00.291546 d3graph-2.4.3/d3graph/
--rw-rw-rw-   0        0        0     1652 2023-03-20 18:15:30.000000 d3graph-2.4.3/d3graph/__init__.py
--rw-rw-rw-   0        0        0     3510 2022-09-03 19:39:37.000000 d3graph-2.4.3/d3graph/adjmat_vec.py
--rw-rw-rw-   0        0        0    51317 2023-03-16 19:27:24.000000 d3graph-2.4.3/d3graph/d3graph.py
-drwxrwxrwx   0        0        0        0 2023-03-20 18:16:00.372400 d3graph-2.4.3/d3graph/d3js/
--rw-rw-rw-   0        0        0        0 2022-05-20 19:47:24.000000 d3graph-2.4.3/d3graph/d3js/__init__.py
--rw-rw-rw-   0        0        0   347498 2022-05-20 19:47:24.000000 d3graph-2.4.3/d3graph/d3js/d3.v3.js
--rw-rw-rw-   0        0        0    10397 2023-03-19 19:24:36.000000 d3graph-2.4.3/d3graph/d3js/d3graphscript.js
--rw-rw-rw-   0        0        0     1253 2023-03-19 19:25:32.000000 d3graph-2.4.3/d3graph/d3js/index.html.j2
--rw-rw-rw-   0        0        0      275 2022-05-20 19:47:24.000000 d3graph-2.4.3/d3graph/d3js/style.css
--rw-rw-rw-   0        0        0    15191 2023-03-19 20:56:46.000000 d3graph-2.4.3/d3graph/examples.py
-drwxrwxrwx   0        0        0        0 2023-03-20 18:16:00.330261 d3graph-2.4.3/d3graph.egg-info/
--rw-rw-rw-   0        0        0     6289 2023-03-20 18:15:58.000000 d3graph-2.4.3/d3graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-03-20 18:15:59.000000 d3graph-2.4.3/d3graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-20 18:15:59.000000 d3graph-2.4.3/d3graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-03-20 18:15:59.000000 d3graph-2.4.3/d3graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-20 18:15:59.000000 d3graph-2.4.3/d3graph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2023-03-20 18:16:00.432507 d3graph-2.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1687 2023-02-17 16:15:40.000000 d3graph-2.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-20 18:16:00.410065 d3graph-2.4.3/tests/
--rw-rw-rw-   0        0        0        0 2022-09-03 19:39:37.000000 d3graph-2.4.3/tests/__init__.py
--rw-rw-rw-   0        0        0      707 2022-09-03 19:39:37.000000 d3graph-2.4.3/tests/conftest.py
--rw-rw-rw-   0        0        0     1072 2022-11-17 10:04:29.000000 d3graph-2.4.3/tests/test_d3graph.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.088237 d3graph-2.4.4/
+-rw-rw-rw-   0        0        0     1700 2022-05-20 19:47:24.000000 d3graph-2.4.4/LICENSE
+-rw-rw-rw-   0        0        0       82 2022-05-20 19:47:24.000000 d3graph-2.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6248 2023-04-29 17:13:55.089234 d3graph-2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5708 2023-03-10 17:10:19.000000 d3graph-2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 17:13:54.950057 d3graph-2.4.4/d3graph/
+-rw-rw-rw-   0        0        0     1652 2023-04-29 17:13:42.000000 d3graph-2.4.4/d3graph/__init__.py
+-rw-rw-rw-   0        0        0     3510 2022-09-03 19:39:37.000000 d3graph-2.4.4/d3graph/adjmat_vec.py
+-rw-rw-rw-   0        0        0    53952 2023-04-29 14:59:55.000000 d3graph-2.4.4/d3graph/d3graph.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.061949 d3graph-2.4.4/d3graph/d3js/
+-rw-rw-rw-   0        0        0        0 2022-05-20 19:47:24.000000 d3graph-2.4.4/d3graph/d3js/__init__.py
+-rw-rw-rw-   0        0        0   347498 2022-05-20 19:47:24.000000 d3graph-2.4.4/d3graph/d3js/d3.v3.js
+-rw-rw-rw-   0        0        0    11062 2023-04-29 14:47:58.000000 d3graph-2.4.4/d3graph/d3js/d3graphscript.js
+-rw-rw-rw-   0        0        0     1253 2023-03-19 19:25:32.000000 d3graph-2.4.4/d3graph/d3js/index.html.j2
+-rw-rw-rw-   0        0        0      275 2022-05-20 19:47:24.000000 d3graph-2.4.4/d3graph/d3js/style.css
+-rw-rw-rw-   0        0        0    16539 2023-04-29 16:20:31.000000 d3graph-2.4.4/d3graph/examples.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.014275 d3graph-2.4.4/d3graph.egg-info/
+-rw-rw-rw-   0        0        0     6248 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-29 17:13:54.000000 d3graph-2.4.4/d3graph.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-04-29 17:13:55.108375 d3graph-2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1687 2023-02-17 16:15:40.000000 d3graph-2.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 17:13:55.087241 d3graph-2.4.4/tests/
+-rw-rw-rw-   0        0        0        0 2022-09-03 19:39:37.000000 d3graph-2.4.4/tests/__init__.py
+-rw-rw-rw-   0        0        0      707 2022-09-03 19:39:37.000000 d3graph-2.4.4/tests/conftest.py
+-rw-rw-rw-   0        0        0     1072 2022-11-17 10:04:29.000000 d3graph-2.4.4/tests/test_d3graph.py
```

### Comparing `d3graph-2.4.3/LICENSE` & `d3graph-2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/PKG-INFO` & `d3graph-2.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: d3graph
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python package to create interactive network based on d3js.
 Home-page: https://erdogant.github.io/d3graph
-Download-URL: https://github.com/erdogant/d3graph/archive/2.4.3.tar.gz
+Download-URL: https://github.com/erdogant/d3graph/archive/2.4.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -117,9 +115,7 @@
 ### Citation
 Please cite d3graph in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

### Comparing `d3graph-2.4.3/README.md` & `d3graph-2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/d3graph/__init__.py` & `d3graph-2.4.4/d3graph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     json_create,
     adjmat2dict,
     data_checks,
     )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.4.3'
+__version__ = '2.4.4'
 
 
 # module level doc-string
 __doc__ = """
 d3graph
 =======================================================================================
```

### Comparing `d3graph-2.4.3/d3graph/adjmat_vec.py` & `d3graph-2.4.4/d3graph/adjmat_vec.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/d3graph/d3graph.py` & `d3graph-2.4.4/d3graph/d3graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,25 @@
             time.sleep(sleep)
             file_location = os.path.abspath(self.config['filepath'])
             if platform == "darwin":  # check if on OSX
                 file_location = "file:///" + file_location
             if os.path.isfile(file_location):
                 webbrowser.open(file_location, new=2)
 
-    def set_edge_properties(self, edge_distance: int = None, scaler: str = 'zscore', minmax: List[float] = None, directed: bool = False, marker_start=None, marker_end='arrow', marker_color='#808080', label='') -> dict:
+    def set_edge_properties(self,
+                            edge_distance: int = None,
+                            scaler: str = 'zscore',
+                            minmax: List[float] = None,
+                            directed: bool = False,
+                            marker_start=None,
+                            marker_end='arrow',
+                            marker_color='#808080',
+                            label: str = None,
+                            label_color = '#808080',
+                            label_fontsize : int = 8) -> dict:
         """Edge properties.
 
         Parameters
         ----------
         edge_distance : Int (default: 30)
             Distance of nodes on the edges.
             * 0: Weighted approach using edge weights in the adjacency matrix. Weights are normalized between the minmax
@@ -215,48 +225,60 @@
             False: Edges do not show markers.
         marker_start : (list of) str, (default: 'arrow')
             The start of the edge can be one of the following markers:
             'arrow','square','circle','stub',None or ''
         marker_end : (list of) str, (default: 'arrow')
             The end of the edge can be one of the following markers:
             'arrow','square','circle','stub',None or ''
+        marker_color : str, (default: '#808080')
+            The label color in hex.
+        label : str, (default: '')
+            The edge label.
+        label_color : str, (default: None)
+            The label color in hex.
+            None : Inherits the color from marker_color.
+        label_fontsize : int, (default: 8)
+            The fontsize of the label.
 
         Returns
         -------
         edge_properties: dict
             key: (source, target)
                 'weight': weight of the edge
                 'weight_scaled': scaled weight of the edge
                 'color': color of the edge
 
         """
-        if minmax is None:
-            minmax = [0.5, 15.0]
+        if minmax is None: minmax = [0.5, 15.0]
         self.config['directed'] = directed
         self.config['edge_distance'] = 30 if edge_distance is None else edge_distance
         self.config['minmax'] = minmax
         self.config['edge_scaler'] = scaler
         self.config['marker_start'] = marker_start
         self.config['marker_end'] = marker_end
         self.config['marker_color'] = marker_color
         self.config['label'] = label
+        self.config['label_color'] = label_color
+        self.config['label_fontsize'] = label_fontsize
 
         if (not directed) and (marker_end is not None) or (marker_start is not None):
             logger.info('Set directed=True to see the markers!')
 
         # Set the edge properties
         # Set the edge properties
         self.edge_properties = adjmat2dict(self.adjmat,
                                            min_weight=0,
                                            minmax=self.config['minmax'],
                                            scaler=self.config['edge_scaler'],
                                            marker_start=self.config['marker_start'],
                                            marker_end=self.config['marker_end'],
                                            marker_color=self.config['marker_color'],
                                            label=self.config['label'],
+                                           label_color=self.config['label_color'],
+                                           label_fontsize=self.config['label_fontsize'],
                                            )
 
         logger.debug('Number of edges: %.0d', len(self.edge_properties.keys()))
 
     def set_node_properties(self,
                             label: List[str] = None,
                             tooltip: List[str] = None,
@@ -792,14 +814,16 @@
         links[i]['target'] = int(target[i])
         links[i]['source_label'] = edges[i][0]
         links[i]['target_label'] = edges[i][1]
         links[i]['marker_start'] = links[i]['marker_start']
         links[i]['marker_end'] = links[i]['marker_end']
         links[i]['marker_color'] = links[i]['marker_color']
         links[i]['label'] = links[i]['label']
+        links[i]['label_color'] = links[i]['label_color']
+        links[i]['label_fontsize'] = links[i]['label_fontsize']
         links_new.append(links[i])
     nodes = pd.DataFrame([*G.nodes.values()]).T.to_dict()
     nodes_new = [None] * len(nodes)
     for i, node in enumerate(nodes):
         nodes[i]['node_name'] = nodes[i].pop('label')
         # nodes[i]['node_label'] = nodes[i].pop('label')
         nodes[i]['node_tooltip'] = nodes[i].pop('tooltip')
@@ -812,15 +836,25 @@
         # Combine all information into new list
         nodes_new[i] = nodes[i]
     data = {'links': links_new, 'nodes': nodes_new}
     return dumps(data, separators=(',', ':'))
 
 
 # %%  Convert adjacency matrix to vector
-def adjmat2dict(adjmat: pd.DataFrame, min_weight: float = 0.0, scaler: str = 'zscore', minmax=None, marker_start=None, marker_end='arrow', marker_color='#808080', label='') -> dict:
+def adjmat2dict(adjmat: pd.DataFrame,
+                min_weight: float = 0.0,
+                scaler: str = 'zscore',
+                minmax=None,
+                marker_start=None,
+                marker_end='arrow',
+                marker_color='#808080',
+                label=None,
+                label_color='#808080',
+                label_fontsize: int = 8,
+                ) -> dict:
     """Convert adjacency matrix into vector with source and target.
 
     Parameters
     ----------
     adjmat : pd.DataFrame()
         Adjacency matrix.
     min_weight : float
@@ -829,31 +863,47 @@
         Scale the edge-width using the following scaler:
         'zscore' : Scale values to Z-scores.
         'minmax' : The sklearn scaler will shrink the distribution between minmax.
         None : No scaler is used.
     minmax : tuple(int,int), (default: [0.5, 15])
         Weights are normalized between minimum and maximum
         * [0.5, 15]
+    marker_start : (list of) str, (default: 'arrow')
+        The start of the edge can be one of the following markers:
+        'arrow','square','circle','stub',None or ''
+    marker_end : (list of) str, (default: 'arrow')
+        The end of the edge can be one of the following markers:
+        'arrow','square','circle','stub',None or ''
+    marker_color : str, (default: '#808080')
+        The label color in hex.
+    label : str, (default: None)
+        The edge label.
+    label_color : str, (default: None)
+        The label color in hex.
+        None : Inherits the color from marker_color.
+    label_fontsize : int, (default: 8)
+        The fontsize of the label.
 
     Returns
     -------
     edge_properties: dict
         key: (source, target)
             'weight': weight of the edge.
             'weight_scaled': scaled weight of the edge.
             'color': color of the edge.
             'marker_start': '', 'circle', 'square', 'arrow', 'stub'
             'marker_end': '', 'circle', 'square', 'arrow', 'stub'
             'marker_color': hex color of the marker.
             'label': Text label for the edge.
+            'label_color': color of the label.
+            'label_fontsize': fontsize of the label.
 
     """
     # Convert adjacency matrix into vector
-    if minmax is None:
-        minmax = [0.5, 15]
+    if minmax is None: minmax = [0.5, 15]
     df = adjmat.stack().reset_index()
     # Set columns
     df.columns = ['source', 'target', 'weight']
     # Remove self loops and no-connected edges
     Iloc = df['source'] != df['target']
     # Keep only edges with a minimum edge strength
     if min_weight is not None:
@@ -869,28 +919,35 @@
     else:
         df['weight_scaled'] = np.ones(df.shape[0]) * 1
 
     # Set marker start-end
     if marker_start is None: marker_start=''
     if marker_end is None: marker_end=''
     if label is None: label=''
+
+    # Store in dataframe
     df['marker_start']=marker_start
     df['marker_end']=marker_end
     df['marker_color']=marker_color
     df['label']=label
+    df['label_color']=label_color
+    df['label_fontsize']=label_fontsize
 
     # Creation dictionary
     source_target = list(zip(df['source'], df['target']))
     # Return
     return {edge: {'weight': df['weight'].iloc[i],
                    'weight_scaled': df['weight_scaled'].iloc[i],
                    'color': '#808080', 'marker_start': df['marker_start'].iloc[i],
                    'marker_end': df['marker_end'].iloc[i],
                    'marker_color': df['marker_color'].iloc[i],
-                   'label': df['label'].iloc[i]} for
+                   'label': df['label'].iloc[i],
+                   'label_color': df['label_color'].iloc[i],
+                   'label_fontsize': df['label_fontsize'].iloc[i],
+                   } for
             i, edge in enumerate(source_target)}
 
 
 # %% Convert dict with edges to graph (G) (also works with lower versions of networkx)
 def edges2G(edge_properties: dict, G: nx.Graph = None) -> nx.Graph:
     """Convert edges to Graph.
 
@@ -916,14 +973,16 @@
                    marker_color=edge_properties[edge]['marker_color'],
                    marker_start=edge_properties[edge]['marker_start'],
                    marker_end=edge_properties[edge]['marker_end'],
                    weight_scaled=np.abs(edge_properties[edge]['weight_scaled']),
                    weight=np.abs(edge_properties[edge]['weight']),
                    color=edge_properties[edge]['color'],
                    label=edge_properties[edge]['label'],
+                   label_color=edge_properties[edge]['label_color'],
+                   label_fontsize=edge_properties[edge]['label_fontsize'],
                    )
     return G
 
 
 # %% Convert dict with nodes to graph (G)
 def nodes2G(node_properties: dict, G: nx.Graph = None) -> nx.Graph:
     """Convert nodes to Graph.
@@ -981,14 +1040,19 @@
     return G
 
 
 # %% Normalize.
 def _normalize_size(getsizes, minscale: Union[int, float] = 0.5, maxscale: Union[int, float] = 4, scaler: str = 'zscore'):
     # Instead of Min-Max scaling, that shrinks any distribution in the [0, 1] interval, scaling the variables to
     # Z-scores is better. Min-Max Scaling is too sensitive to outlier observations and generates unseen problems,
+
+    # Set sizes to 0 if not available
+    getsizes[np.isinf(getsizes)]=0
+    getsizes[np.isnan(getsizes)]=0
+
     # out-of-scale datapoints.
     if scaler == 'zscore' and len(np.unique(getsizes)) > 3:
         getsizes = (getsizes.flatten() - np.mean(getsizes)) / np.std(getsizes)
         getsizes = getsizes + (minscale - np.min(getsizes))
     elif scaler == 'minmax':
         try:
             from sklearn.preprocessing import MinMaxScaler
```

### Comparing `d3graph-2.4.3/d3graph/d3js/d3.v3.js` & `d3graph-2.4.4/d3graph/d3js/d3.v3.js`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/d3graph/d3js/d3graphscript.js` & `d3graph-2.4.4/d3graph/d3js/d3graphscript.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -83,14 +83,32 @@
         }) // LINK-WIDTH
         .style("stroke", function(d) {
             return d.color;
         }) // EDGE-COLORS
     //  .style("stroke-width", 1); // WIDTH OF THE LINKS
     ;
 
+    // ADD TEXT ON THE EDGES (PART 1/2)
+    var linkText = svg.selectAll(".link-text")
+        .data(graph.links)
+        .enter().append("text")
+        .attr("class", "link-text")
+        .attr("font-size", function(d) {
+            return d.label_fontsize + "px";
+        })
+        .style("fill", function(d) {
+            return d.label_color;
+        })
+        .style("font-family", "Arial")
+        //.attr("transform", "rotate(90)")
+        .text(function(d) {
+            return d.label;
+        });
+
+
     //Do the same with the circles for the nodes
     var node = svg.selectAll(".node")
         .data(graph.nodes)
         .enter().append("g")
         .attr("class", "node")
         .call(drag)
         .on('dblclick', connectedNodes); // HIGHLIGHT ON/OFF
@@ -162,15 +180,22 @@
                 return d.y;
             });
         d3.selectAll("text").attr("x", function(d) {
                 return d.x;
             })
             .attr("y", function(d) {
                 return d.y;
-            });
+            })
+        linkText.attr("x", function(d) {
+                return (d.source.x + d.target.x) / 2;
+            }) // ADD TEXT ON THE EDGES (PART 2/2)
+            .attr("y", function(d) {
+                return (d.source.y + d.target.y) / 2;
+            })
+            .attr("text-anchor", "middle");;
 
         node.each(collide(config.collision)); //COLLISION DETECTION. High means a big fight to get untouchable nodes (default=0.5)
 
     });
 
     // --------- MARKER -----------
```

### Comparing `d3graph-2.4.3/d3graph/d3js/index.html.j2` & `d3graph-2.4.4/d3graph/d3js/index.html.j2`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/d3graph/examples.py` & `d3graph-2.4.4/d3graph/examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,72 @@
 import networkx as nx
 import pandas as pd
 import numpy as np
 from d3graph import d3graph, adjmat2vec
 
 # %% Edge link
 d3 = d3graph()
-adjmat, df = d3.import_example('bigbang')
+adjmat, df = d3.import_example('karate')
+d3.graph(adjmat, color='cluster')
+d3.show(filepath=r'c:\temp\\d3graph\d3graph1.html')
+
+# %% Edge link
+
+# Import
+from d3graph import d3graph
+# intialize to load example dataset
+d3 = d3graph()
+adjmat, _ = d3.import_example('bigbang')
+
+# Initialize with clustering colors
 d3.graph(adjmat, color='cluster')
-d3.set_edge_properties(directed=True, marker_end='square', marker_color='#000000', label='TEST')
 
+# Set all edge labels to "test"
+d3.set_edge_properties(directed=True, label='test')
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_1.html')
+
+# Set edge labels 
 d3.edge_properties
-d3.show(filepath=r'c:\temp\\d3graph\d3graph1.html')
+
+# We will first set all label properties to None and then we will adjust two of them
+d3.set_edge_properties(directed=True, marker_color='#000FFF', label=None)
+d3.edge_properties['Amy', 'Bernadette']['weight_scaled']=10
+d3.edge_properties['Amy', 'Bernadette']['label']='amy-bern'
+d3.edge_properties['Amy', 'Bernadette']['label_color']='#000FFF'
+d3.edge_properties['Amy', 'Bernadette']['label_fontsize']=8
+d3.edge_properties['Bernadette', 'Howard']['label']='bern-how'
+d3.edge_properties['Bernadette', 'Howard']['label_fontsize']=20
+d3.edge_properties['Bernadette', 'Howard']['label_color']='#000000'
+
+d3.show(filepath=r'c:\temp\\d3graph\edge_labels_2.html')
 
 # %% Change color of text
+
+# Import library
 from d3graph import d3graph
 
+# Initialize with defaults
 d3 = d3graph()
-adjmat, df = d3.import_example('bigbang')
-d3.graph(adjmat, color='cluster')
-d3.set_node_properties(color='cluster', scaler='minmax', fontcolor='node_color', fontsize=12)
-d3.show(filepath=r'c:\temp\\d3graph\d3graph.html', click={'fill': 'black'})
-d3.show(filepath=r'c:\temp\\d3graph\d3graph.html')
 
+# Load example
+adjmat, df = d3.import_example('bigbang')
+# Color on clustering
+d3.graph(adjmat)
 fontsize=np.random.randint(low=6, high=40, size=adjmat.shape[0])
+
+# Set some node properties
+d3.set_node_properties(color='cluster', scaler='minmax', fontcolor='node_color')
+
+# Set the click properties: Create green node on click with black border
+d3.show(filepath=r'c:\temp\\d3graph\click_example_1.html', click={'fill': '#00FF00', 'stroke': '#000000'})
+
+# Keep the original color but set the stroke to grey and increase both node size and stroke width
+d3.show(filepath=r'c:\temp\\d3graph\click_example_2.html', click={'fill': None, 'stroke': '#F0F0F0', 'size': 2.5, 'stroke-width': 10})
+
+
 d3.set_node_properties(color='cluster', scaler='minmax', fontcolor='node_color', fontsize=fontsize)
 d3.show(filepath=r'c:\temp\\d3graph\d3graph.html')
 
 # %% 
 from d3graph import d3graph
 adjmat, df = d3.import_example('bigbang')
 d3.graph(adjmat, color='cluster')
```

### Comparing `d3graph-2.4.3/d3graph.egg-info/PKG-INFO` & `d3graph-2.4.4/d3graph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: d3graph
-Version: 2.4.3
+Version: 2.4.4
 Summary: Python package to create interactive network based on d3js.
 Home-page: https://erdogant.github.io/d3graph
-Download-URL: https://github.com/erdogant/d3graph/archive/2.4.3.tar.gz
+Download-URL: https://github.com/erdogant/d3graph/archive/2.4.4.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -117,9 +115,7 @@
 ### Citation
 Please cite d3graph in your publications if this is useful for your research. See column right for citation information.
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
-
-
```

### Comparing `d3graph-2.4.3/setup.py` & `d3graph-2.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/tests/conftest.py` & `d3graph-2.4.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `d3graph-2.4.3/tests/test_d3graph.py` & `d3graph-2.4.4/tests/test_d3graph.py`

 * *Files identical despite different names*

