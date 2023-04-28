# Comparing `tmp/omniplot-0.4.4.tar.gz` & `tmp/omniplot-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplot-0.4.4.tar", last modified: Wed Apr 26 10:03:04 2023, max compression
+gzip compressed data, was "omniplot-0.4.5.tar", last modified: Fri Apr 28 23:49:20 2023, max compression
```

## Comparing `omniplot-0.4.4.tar` & `omniplot-0.4.5.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/
--rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.4/LICENSE
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-26 10:03:04.461285 omniplot-0.4.4/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-04-22 04:16:47.000000 omniplot-0.4.4/README.md
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot/
--rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/_adjustText.py
--rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-26 10:02:49.000000 omniplot-0.4.4/omniplot/_version.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/chipseq_utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot/cython_utils/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/cython_utils/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/data.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   100746 2023-04-26 09:57:01.000000 omniplot-0.4.4/omniplot/heatmap.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/igraph_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/networkplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10853 2023-04-22 05:11:17.000000 omniplot-0.4.4/omniplot/plot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/plot_classes.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    73070 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/proportion.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/regressionplot.py
--rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/scatter.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot/scripts/
--rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/scripts/__init__.py
--rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/scripts/gff2tss.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.4/omniplot/statistics.py
--rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.4/omniplot/utils.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/omniplot.egg-info/
--rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/PKG-INFO
--rw-rw-r--   0 koh       (1000) koh       (1000)      674 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/SOURCES.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/dependency_links.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/requires.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-26 10:03:04.000000 omniplot-0.4.4/omniplot.egg-info/top_level.txt
--rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-26 10:03:04.461285 omniplot-0.4.4/setup.cfg
--rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.4/setup.py
-drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-26 10:03:04.461285 omniplot-0.4.4/tests/
--rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-04-22 04:16:47.000000 omniplot-0.4.4/tests/test_chipseq.py
--rw-rw-r--   0 koh       (1000) koh       (1000)     5232 2023-04-26 07:43:20.000000 omniplot-0.4.4/tests/tests heatmap.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/
+-rw-rw-r--   0 koh       (1000) koh       (1000)    35149 2023-04-22 04:16:47.000000 omniplot-0.4.5/LICENSE
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-28 23:49:20.878973 omniplot-0.4.5/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3276 2023-04-22 04:16:47.000000 omniplot-0.4.5/README.md
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      580 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21778 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/_adjustText.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)       21 2023-04-28 23:42:17.000000 omniplot-0.4.5/omniplot/_version.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    57911 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    21857 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/chipseq_utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot/cython_utils/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/cython_utils/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      288 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/data.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   102103 2023-04-28 23:42:02.000000 omniplot-0.4.5/omniplot/heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    12843 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/igraph_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    32121 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/networkplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    20850 2023-04-28 23:24:22.000000 omniplot-0.4.5/omniplot/plot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3511 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/plot_classes.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    73070 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/proportion.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    10740 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/regressionplot.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)   134250 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/scatter.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot/scripts/
+-rw-rw-r--   0 koh       (1000) koh       (1000)        0 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/scripts/__init__.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)      694 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/scripts/gff2tss.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     1584 2023-04-22 04:16:47.000000 omniplot-0.4.5/omniplot/statistics.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    44811 2023-04-23 08:15:37.000000 omniplot-0.4.5/omniplot/utils.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/omniplot.egg-info/
+-rw-rw-r--   0 koh       (1000) koh       (1000)      976 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/PKG-INFO
+-rw-rw-r--   0 koh       (1000) koh       (1000)      711 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/SOURCES.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        1 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/dependency_links.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)      220 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/requires.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)        9 2023-04-28 23:49:20.000000 omniplot-0.4.5/omniplot.egg-info/top_level.txt
+-rw-rw-r--   0 koh       (1000) koh       (1000)       38 2023-04-28 23:49:20.882972 omniplot-0.4.5/setup.cfg
+-rw-rw-r--   0 koh       (1000) koh       (1000)     2770 2023-04-22 04:16:47.000000 omniplot-0.4.5/setup.py
+drwxrwxr-x   0 koh       (1000) koh       (1000)        0 2023-04-28 23:49:20.878973 omniplot-0.4.5/tests/
+-rw-rw-r--   0 koh       (1000) koh       (1000)     4359 2023-03-31 09:25:44.000000 omniplot-0.4.5/tests/test_chipseq.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     3033 2023-04-12 09:33:24.000000 omniplot-0.4.5/tests/test_network.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)     5410 2023-04-28 23:42:02.000000 omniplot-0.4.5/tests/tests heatmap.py
+-rw-rw-r--   0 koh       (1000) koh       (1000)    13863 2023-04-28 23:22:23.000000 omniplot-0.4.5/tests/tests.py
```

### Comparing `omniplot-0.4.4/LICENSE` & `omniplot-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/PKG-INFO` & `omniplot-0.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.4
+Version: 0.4.5
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.4/README.md` & `omniplot-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/__init__.py` & `omniplot-0.4.5/omniplot/__init__.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/_adjustText.py` & `omniplot-0.4.5/omniplot/_adjustText.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/chipseq.py` & `omniplot-0.4.5/omniplot/chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/chipseq_utils.py` & `omniplot-0.4.5/omniplot/chipseq_utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/heatmap.py` & `omniplot-0.4.5/omniplot/heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from omniplot.chipseq_utils import _calc_pearson
 import itertools as it
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Rectangle, Circle,Ellipse, RegularPolygon, Polygon
 import copy
 import textwrap
 from matplotlib.artist import Artist
+from matplotlib.transforms import Affine2D
+import mpl_toolkits.axisartist.floating_axes as floating_axes
 
 __all__=["correlation", "triangle_heatmap", "complex_clustermap","dotplot", "heatmap"]
 def correlation(df: pd.DataFrame, 
                 category: Union[str, list]=[],
                 variables: List=[],
                 method="pearson",
                 palette: str="coolwarm",
@@ -763,20 +765,20 @@
                
         den=sch.dendrogram(g.dendrogram_row.linkage,
                             labels = g.data.index,
                             color_threshold=t,
                             ax=g.ax_row_dendrogram,
                             orientation="left")
         
-        print(np.amax(den["dcoord"]))
+        # print(np.amax(den["dcoord"]))
         g.ax_row_dendrogram.invert_yaxis()
         clusters = _get_cluster_classes(den)
         
         keys=list(clusters.keys())
-        print(keys)
+        # print(keys)
         ckeys={}
         i=1
         for k in keys:
             if k.startswith("C0_"):
                 ckeys[k]=k
             else:
                 ckeys[k]="C"+str(i)
@@ -1115,19 +1117,21 @@
                 col_colors: Union[dict, list]={},
                 row_plot: Union[dict, list]={},
                 col_plot: Union[dict, list]={},
                 plotkw: dict={},
                 row_scatter: Union[dict, list]={},
                 col_scatter: Union[dict, list]={},
                 scatterkw: dict={},
-
                 row_bar: Union[dict, list]={},
                 col_bar: Union[dict, list]={},
                 barkw: dict={},
-            
+                row_axis: int=0,
+                col_axis: int=0,
+
+
                 approx_clusternum: Union[int, str]=3,
                 approx_clusternum_col: int=3,
 
                 cunit: str="",
                 show: bool=False,
                 ztranform: bool=True,
 
@@ -1346,17 +1350,19 @@
                 scX=np.array(list(shape_colors.values())[0])
             else:
                 scX=np.array(shape_colors)
         if row_cluster==True or col_cluster==True:
             clustering_method="kmodes"
             print("Categorical variables are provided. 'kmodes' will be used for the clustering method.")
     
-    rowplot_num=len(category)+len(row_colors)+len(row_plot)+len(row_scatter)+len(row_bar)+\
+    rowplot_num=len(category)+len(row_colors)+\
+        len(row_plot)+len(row_scatter)+len(row_bar)+row_axis+\
         int(clustering_method=="kmeans" and row_cluster==True)+int(clustering_method=="kmodes" and row_cluster==True)
-    colplot_num=len(col_colors)+len(col_plot)+len(col_scatter)+len(col_bar)+\
+    colplot_num=len(col_colors)+len(col_plot)+\
+        len(col_scatter)+len(col_bar)+col_axis+\
         int(clustering_method=="kmeans" and col_cluster==True)+int(clustering_method=="kmodes" and col_cluster==True)
     Xshape=X.shape
     if np.sum(Xshape)>200:
         edgecolor=None
     show_legend=int(rowplot_num>0 or type(Xsize)!=type(None))
     
 
@@ -1414,15 +1420,15 @@
     tcaty=yori+ltreeh
     tcath=0.025
 
     hmapx=xori+ltreew+lcatw*rowplot_num
     ttreey=yori+ltreeh+tcath*colplot_num
     legendh=(3/Xshape[0])*hmaph
     
-    print([xori,ltreew,hmapw,legendw])
+    # print([xori,ltreew,hmapw,legendw])
     
 
     size_legend_num=3
     size_legend_elements=[]
     if type(Xsize)!=type(None):
         smin=np.amin(Xsize)
         smax=np.amax(Xsize)
@@ -1447,15 +1453,15 @@
         prev_top=0
         for _i in range(size_legend_num):
             s=vmin+_i*vinterval
             if s <0.1:
                 s=0.1
             sx=s*(hmapw/legendw)/Xshape[1]
             sy=s*(hmaph/legendh)*size_legend_num/Xshape[0]
-            print(sx, sy)
+            # print(sx, sy)
             
             if prev_top==0:
                 _yh=0
             else:
                 _yh=prev_top+sy
             if shape=="by_category":
                 size_legend_elements.append(_create_polygon("circle", 0, _i, sx,ry=sy))
@@ -1598,21 +1604,21 @@
                                            row_scatter, 
                                            row_bar, 
                                            rowplot_format, 
                                            legend_elements_dict, 
                                            Xshape, 
                                            lcatx,lcatw,
                                            yori,hmaph, margin, 
-                                           plotkw, scatterkw, barkw, catnum, ax_dict)
+                                           plotkw, scatterkw, barkw, catnum, ax_dict,row_axis=row_axis)
     legend_elements_dict, catnum, axis_dict=_col_plot(sortindexc, fig, col_colors, col_plot, 
                                             col_scatter, col_bar, 
                                             colplot_format,
                                             legend_elements_dict, 
                                             Xshape, tcaty,tcath,hmapx,
-                                            hmapw, margin, plotkw, scatterkw, barkw, catnum, axis_dict)
+                                            hmapw, margin, plotkw, scatterkw, barkw, catnum, axis_dict, col_axis=col_axis)
     
     # Creating the heatmap
 
     # Calculating the maximum and minum values of the data if the data is numerical.
     if dtype=="numerical":
         cmap=plt.get_cmap(palette)
         Xmin=np.amin(X)
@@ -1728,37 +1734,37 @@
         _y=0
         boxfont=12
         ax=fig.add_axes([hmapx+hmapw,yori+_y,boxwidth,hmaph])
         ax.axis('off')
         for i, (_c,c) in enumerate(zip(_cnums, cnums)):
             text=", ".join(rowlabels[_r:_r+c])
             word_list = wrapper.wrap(text=text)
-            print(word_list)
+            # print(word_list)
             t=ax.text(0.1,_y+_c-0.01,"\n".join(word_list), fontsize=boxfont,va="top",
                       bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="gray", lw=1, alpha=0.8))
             bb=t.get_window_extent(renderer=render)
-            print("width", rwidth, bb.width)
+            # print("width", rwidth, bb.width)
             if i==0 and bb.width/rwidth> boxwidth:
                 while bb.width/rwidth > boxwidth:
                     Artist.remove(t)
                     boxfont-=0.5
-                    print(boxfont)
+                    # print(boxfont)
                     if boxfont<0:
                         break
                     t=ax.text(0.1,_y+_c-0.01,"\n".join(word_list), fontsize=boxfont, va="top",
                       bbox=dict(boxstyle="round,pad=0.3", fc="white", ec="gray", lw=1, alpha=0.8))
                     bb=t.get_window_extent(renderer=render)
 
 
             _r+=c
             _y+=_c
 
     #Drawing a heatmap
     pcolormesh=False
-    if Xshape[0]>1000 and Xshape[1]>1000:
+    if Xshape[0]>1000 or Xshape[1]>1000:
         pcolormesh=True
     if row_split==True and row_cluster==True:
         
         # print(cnums, _cnums)
         _y=0
         _r=0
         for i, (_c,c) in enumerate(zip(_cnums, cnums)):
@@ -2039,16 +2045,16 @@
         _row_col=np.array(row_col)
         _shapes = [Rectangle((- 0.5,- 0.5), np.amax(_row_col[:,0])+1, np.amax(_row_col[:,1])+1)]
         _pc = PatchCollection(_shapes, facecolor="w", alpha=1,
                     edgecolor="w")
         ax.add_collection(_pc)
 
     if type(shape)==dict:
-        print(shape)
-        print(Xflatten)
+        # print(shape)
+        # print(Xflatten)
         if type(Xsize)!=type(None):
             # shapes = [_create_polygon(shape[val], x,y, wh)
             #             for (x, y), wh, val in zip(row_col, _Xsize,Xflatten)]
             shapes=Parallel(n_jobs=n_jobs)(delayed(_create_polygon)(
                 shape[val], x,y, wh) for (x, y), wh, val in zip(row_col, _Xsize,Xflatten))
 
 
@@ -2127,33 +2133,49 @@
                     rs.append([x+0.5*r*np.cos(np.pi/2+(_l+_m/m)*2*np.pi/l),y+0.5*ry*np.sin(np.pi/2+(_l+_m/m)*2*np.pi/l)])
         else:
             for i in range(n):
                 rs.append([x+0.5*r*np.cos(np.pi/2+(m*i)*2*np.pi/n),y+0.5*ry*np.sin(np.pi/2+(m*i)*2*np.pi/n)])
         return Polygon(rs, **kwargs)
     else:
         raise Exception["Unknown shape! you gave {}, but it only accepts 'rectangle', 'circle', 'star', 'polygon:n', 'star:n:m'".format(shape)]
-def _row_plot(df, leaves, fig, 
-              category, lut, row_colors, row_plot, 
-              row_scatter, row_bar, 
+def _row_plot(df, 
+              leaves, 
+              fig, 
+              category, 
+              lut, 
+              row_colors, 
+              row_plot, 
+              row_scatter, 
+              row_bar, 
               rowplot_format,
                 legend_elements_dict, 
-                Xshape, lcatx,lcatw,yori,
-                hmaph, margin, plotkw, scatterkw, barkw ,catnum,axis_dict):
+                Xshape, 
+                lcatx,
+                lcatw,
+                yori,
+                hmaph, 
+                margin, 
+                plotkw, 
+                scatterkw, 
+                barkw ,
+                catnum,
+                axis_dict, row_axis=0):
     
     def set_axis(_ax, _val, _cat, _margin, _rowplot_format):
         _ax.tick_params(pad=-5)
         _ax.margins(x=_margin,y=_margin)
         _ax.set_xlabel(_cat, rotation=90)
         vmin, vmax=np.amin(_val), np.amax(_val)
         shift=(vmax-vmin)/5
         ax.set_xticks([vmin+shift, vmax-shift],
                         labels=[_rowplot_format.format(x=vmin), 
                         _rowplot_format.format(x=vmax)], 
                         rotation=90)
         ax.set_yticks([])
+        
         ax.invert_xaxis()
 
     row_plot_index=0
     _df=df.iloc[leaves]
     if len(category)!=0:
         for cat in category:
             ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
@@ -2173,15 +2195,15 @@
             for _cat, _color in lut[cat]["colorlut"].items():
                 legend_elements.append(Line2D([0], [0], marker="s", linewidth=0, markeredgecolor="darkgray",
                                     label=_cat,
                                     markerfacecolor=_color))
             legend_elements_dict[cat]=legend_elements
             row_plot_index+=1
             catnum+=1
-            axis_dict[cat]=ax
+            axis_dict["row_"+cat]=ax
 
     if len(row_colors)!=0:
         for i, (cat, val) in enumerate(row_colors.items()):
             # print(leaves)
             val=np.array(val)[leaves]
             ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
             uniq_labels=np.unique(val)
@@ -2204,81 +2226,94 @@
             for _cat, _color in color_lut.items():
                 legend_elements.append(Line2D([0], [0], marker="s", linewidth=0, markeredgecolor="darkgray",
                                     label=_cat,
                                     markerfacecolor=_color))
             legend_elements_dict[cat]=legend_elements
             row_plot_index+=1
             catnum+=1
-            axis_dict[cat]=ax
+            axis_dict["row_"+cat]=ax
     if len(row_plot)!=0:
         if type(row_plot)==list:
             for cat in row_plot:
                 val=_df[cat]
                 ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
                 ax.plot(val,np.arange(len(val)),**plotkw)
                 set_axis(ax, val, cat, margin, rowplot_format)
-
+                ax.set_ylim(-0.5, val.shape[0]-0.5)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["row_"+cat]=ax
         elif type(row_plot)==dict:
             
             for cat, val in row_plot.items():
                 val=np.array(val)[leaves]
                 ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
                 ax.plot(val,np.arange(len(val)),**plotkw)
+                ax.set_ylim(-0.5,val.shape[0]-0.5)
                 set_axis(ax, val, cat, margin, rowplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["row_"+cat]=ax
     if len(row_scatter)!=0:
         if type(row_scatter)==list:
             for cat in row_scatter:
                 val=_df[cat]
                 ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
                 ax.scatter(val,np.arange(len(val)),**scatterkw)
+                ax.set_ylim(-0.5, val.shape[0]-0.5)
                 set_axis(ax, val, cat, margin, rowplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["row_"+cat]=ax
         elif type(row_scatter)==dict:
             
             for cat, val in row_scatter.items():
                 val=np.array(val)[leaves]
                 ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
                 ax.scatter(val,np.arange(len(val)),**scatterkw)
+                ax.set_ylim(-0.5, val.shape[0]-0.5)
                 set_axis(ax, val, cat, margin, rowplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["row_"+cat]=ax
     if len(row_bar)!=0:
         if type(row_bar)==list:
             for cat in row_bar:
                 val=_df[cat]
                 ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
                 ax.barh(np.arange(len(val)), width=val,**barkw)
                 set_axis(ax, val, cat, margin, rowplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["row_"+cat]=ax
         elif type(row_bar)==dict:
             
             for cat, val in row_bar.items():
                 val=np.array(val)[leaves]
                 ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
                 ax.barh(np.arange(len(val)), width=val,**barkw)
                 set_axis(ax, val, cat, margin, rowplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["row_"+cat]=ax
+
+    if row_axis!=0:
+        for i in range(row_axis):
+            ax=fig.add_axes([lcatx+row_plot_index*lcatw,yori,lcatw,hmaph])
+            
+            set_axis(ax, val, cat, margin, rowplot_format)
+            row_plot_index+=1
+            axis_dict["row_"+str(i)]=ax
+
+
     return legend_elements_dict, catnum, axis_dict
 
 
 
 def _col_plot(leaves, fig, col_colors, col_plot, 
               
               col_scatter, col_bar, 
               colplot_format,
                 legend_elements_dict, 
                 Xshape, tcaty,tcatw,hmapx,
-                hmapw, margin, plotkw, scatterkw, barkw ,catnum, axis_dict):
+                hmapw, margin, plotkw, scatterkw, barkw ,catnum, axis_dict,col_axis=0):
     
     def set_axis(_ax, _val, _cat, _margin, _lowplot_format, pad=-5):
         _ax.tick_params(pad=pad)
         _ax.margins(x=_margin,y=_margin)
         _ax.set_ylabel(_cat, rotation=0,labelpad=5, ha="right")
         vmin, vmax=np.amin(_val), np.amax(_val)
         shift=(vmax-vmin)/5
@@ -2317,53 +2352,63 @@
             for _cat, _color in color_lut.items():
                 legend_elements.append(Line2D([0], [0], marker="s", linewidth=0, markeredgecolor="darkgray",
                                     label=_cat,
                                     markerfacecolor=_color))
             legend_elements_dict[cat]=legend_elements
             row_plot_index+=1
             catnum+=1
-            axis_dict[cat]=ax
+            axis_dict["col_"+cat]=ax
     if len(col_plot)!=0:
         if type(col_plot)==list:
             raise Exception("Currently, 'col_plot' option accepts only dictionary")
         elif type(col_plot)==dict:
             
             for cat, val in col_plot.items():
                 val=np.array(val)[leaves]
                 ax=fig.add_axes([hmapx,tcaty+row_plot_index*tcatw,hmapw,tcatw])
                 ax.plot(val,np.arange(len(val)),**plotkw)
                 set_axis(ax, val, cat, margin, colplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["col_"+cat]=ax
     if len(col_scatter)!=0:
         if type(col_scatter)==list:
             raise Exception("Currently, 'col_scatter' option accepts only dictionary")
 
         elif type(col_scatter)==dict:
             
             for cat, val in col_scatter.items():
                 val=np.array(val)[leaves]
                 ax=fig.add_axes([hmapx,tcaty+row_plot_index*tcatw,hmapw,tcatw])
                 ax.scatter(val,np.arange(len(val)),**scatterkw)
                 set_axis(ax, val, cat, margin, colplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["col_"+cat]=ax
     if len(col_bar)!=0:
         if type(col_bar)==list:
             raise Exception("Currently, 'col_scatter' option accepts only dictionary")
 
         elif type(col_bar)==dict:
             
             for cat, val in col_bar.items():
                 val=np.array(val)[leaves]
                 ax=fig.add_axes([hmapx,tcaty+row_plot_index*tcatw,hmapw,tcatw])
                 ax.bar(np.arange(len(val)), height=val,**barkw)
                 set_axis(ax, val, cat, margin, colplot_format)
                 row_plot_index+=1
-                axis_dict[cat]=ax
+                axis_dict["col_"+cat]=ax
+
+    if col_axis!=0:
+        for i in range(col_axis):
+            ax=fig.add_axes([hmapx,tcaty+row_plot_index*tcatw,hmapw,tcatw])
+            set_axis(ax, val, cat, margin, colplot_format)
+            row_plot_index+=1
+            axis_dict["col_"+str(i)]=ax
+
+
+
     return legend_elements_dict, catnum, axis_dict
 
 
 def _process_vdata(df, variables,category ,row,  col,rowlabels, sizes, size_title, colors, lut,fillna, ztranform,cunit):
     Xsize=None
     if len(variables)==0 and len(category)==0 and len(row)==0 and len(col)==0:
         print("Assuming data is a wide form")
@@ -2537,17 +2582,17 @@
 
 class _AnyObjectHandler:
     def __init__(self, facecolor, shape):
         self.facecolor=facecolor
         self.shape=shape
     def legend_artist(self, legend, orig_handle, fontsize, handlebox):
         x0, y0 = handlebox.xdescent, handlebox.ydescent
-        print(x0, y0)
+        # print(x0, y0)
         width, height = handlebox.width, handlebox.height
-        print(width, height)
+        # print(width, height)
         patch=_create_polygon(self.shape, 10, 3, 10, facecolor=self.facecolor,
                                    edgecolor='black', lw=1,
                                    transform=handlebox.get_transform())
         # patch = Ellipse([10, 3], 10, 10, facecolor=self.facecolor,
         #                            edgecolor='black', lw=1,
         #                            transform=handlebox.get_transform())
         handlebox.add_artist(patch)
```

### Comparing `omniplot-0.4.4/omniplot/igraph_classes.py` & `omniplot-0.4.5/omniplot/igraph_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/networkplot.py` & `omniplot-0.4.5/omniplot/networkplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/plot_classes.py` & `omniplot-0.4.5/omniplot/plot_classes.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/proportion.py` & `omniplot-0.4.5/omniplot/proportion.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/regressionplot.py` & `omniplot-0.4.5/omniplot/regressionplot.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/scatter.py` & `omniplot-0.4.5/omniplot/scatter.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/scripts/gff2tss.py` & `omniplot-0.4.5/omniplot/scripts/gff2tss.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/statistics.py` & `omniplot-0.4.5/omniplot/statistics.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot/utils.py` & `omniplot-0.4.5/omniplot/utils.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/omniplot.egg-info/PKG-INFO` & `omniplot-0.4.5/omniplot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplot
-Version: 0.4.4
+Version: 0.4.5
 Summary: To draw scientific plots easily
 Home-page: https://github.com/koonimaru/omniplot
 Author: Koh Onimaru
 Author-email: koh.onimaru@gmail.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `omniplot-0.4.4/omniplot.egg-info/SOURCES.txt` & `omniplot-0.4.5/omniplot.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 omniplot.egg-info/dependency_links.txt
 omniplot.egg-info/requires.txt
 omniplot.egg-info/top_level.txt
 omniplot/cython_utils/__init__.py
 omniplot/scripts/__init__.py
 omniplot/scripts/gff2tss.py
 tests/test_chipseq.py
-tests/tests heatmap.py
+tests/test_network.py
+tests/tests heatmap.py
+tests/tests.py
```

### Comparing `omniplot-0.4.4/setup.py` & `omniplot-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/tests/test_chipseq.py` & `omniplot-0.4.5/tests/test_chipseq.py`

 * *Files identical despite different names*

### Comparing `omniplot-0.4.4/tests/tests heatmap.py` & `omniplot-0.4.5/tests/tests heatmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,56 +62,59 @@
                         col_colors=["features"],
                         approx_clusternum=3,
                         marginalsum=True, title="Penguins")
     plt.show()
 elif test=="heatmap":
     from PIL import Image
     im=Image.open("/home/koh/Pictures/wave128.jpg").convert("LA")
-    op.heatmap(pd.DataFrame(np.array(im)[:,:,0][::-1]), shape="triangle",row_cluster=True, col_cluster=False,
-    ztranform=False, row_ticklabels=False, col_ticklabels=False)
-    plt.show()
+    df=pd.DataFrame(np.array(im)[:,:,0][::-1])
+    op.heatmap(df, shape="triangle",row_cluster=False, col_cluster=False,
+    ztranform=False, row_plot={"mean": df.mean(axis=1)}, row_ticklabels=False, col_ticklabels=False)
+    
     
-    # df=sns.load_dataset("penguins")
+    df=sns.load_dataset("penguins")
     
-    # df=df.dropna(axis=0)
-    # df=df.reset_index(drop=True)
-    # op.heatmap(df=df,boxlabels=True, 
-    # variables=["bill_length_mm","bill_depth_mm","flipper_length_mm"],
-    # row_split=True, clustering_method="kmeans",
-    #            category=["species", "island"],
-    #            col_colors={"colors": ["bill","bill","flipper"]}, 
-    #            row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3)
-    # op.heatmap(df=df, dtype="categorical", variables=["species", "island", "sex"],
-    #            row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3,column_wise_color=True) 
+    df=df.dropna(axis=0)
+    df=df.reset_index(drop=True)
+    res=op.heatmap(df=df,boxlabels=True, 
+    variables=["bill_length_mm","bill_depth_mm","flipper_length_mm"],
+    row_split=True, clustering_method="kmeans",
+               category=["species", "island"],
+               col_colors={"colors": ["bill","bill","flipper"]}, 
+               row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3)
+    op.heatmap(df=df, dtype="categorical", variables=["species", "island", "sex"],
+               row_plot=["body_mass_g"], row_ticklabels=False, approx_clusternum=3,column_wise_color=True) 
     # _df=df.sample(n=25, replace=False, random_state=1)
     # _df=_df.reset_index(drop=True)
     # op.heatmap(df=_df, 
-
-
-
-
     # dtype="categorical", 
     # variables=["species", "island", "sex"],
     #            row_plot=["body_mass_g"], 
     #            shape="by_category", shape_colors=np.arange(25*3).reshape([25,3]),
     #            row_ticklabels=False, 
     #            approx_clusternum=3,
     #            column_wise_color=True, sizes=np.arange(25*3).reshape([25,3])) 
 
-    # mat=np.concatenate([0.25*np.random.uniform(0,1,size=[10, 25]),0.5*np.random.uniform(0,1,size=[15, 25]),
-    #                     np.random.uniform(0,1,size=[15, 25])])
-    # mat=np.concatenate([mat, np.random.uniform(0,1,size=[40, 15])], axis=1)
-    # print(mat.shape)
-    # df=pd.DataFrame(mat)
-    # op.heatmap(df, sizes=mat, size_title="random",cbar_title="random colors",
-    #            col_split=True,
-    #            row_plot={"normal": np.random.normal(size=mat.shape[0])}, 
-    #            row_scatter={"uniform": np.random.uniform(size=mat.shape[0])}, 
-    #            row_bar={"range": np.arange(mat.shape[0])},
-    #            col_bar={"range": np.arange(mat.shape[1])},
+    mat=np.concatenate([0.25*np.random.uniform(0,1,size=[10, 25]),0.5*np.random.uniform(0,1,size=[15, 25]),
+                        np.random.uniform(0,1,size=[15, 25])])
+    mat=np.concatenate([mat, np.random.uniform(0,1,size=[40, 15])], axis=1)
+    print(mat.shape)
+    df=pd.DataFrame(mat)
+    res=op.heatmap(df, sizes=mat, size_title="random",cbar_title="random colors",
+               col_split=True,
+               row_plot={"mean": mat.mean(axis=1)}, 
+               row_scatter={"uniform": np.random.uniform(size=mat.shape[0])}, 
+               row_axis=2,
+               col_bar={"range": np.arange(mat.shape[1])},
                
-    #            edgecolor=None, approx_clusternum=3, ztranform=False)
+               edgecolor=None, approx_clusternum=3, ztranform=False)
+    print(res.keys())
+    ax=res["axes"]["row_0"]
+    op.violinplot2(mat[res["rowsort"]], ax=ax,orientation="horizontal")
+    ax.set_xlabel("violin")
+    res["axes"]["row_0"].set_ylim(-0.5, mat.shape[0]-0.5)
     # # op.heatmap(df, shape="circle", sizes=mat, edgecolor=None, approx_clusternum=3, row_split=True, ztranform=False)
     # mat=np.arange(50).reshape([5,10]).astype(np.float)
     # df=pd.DataFrame(mat)
     # op.heatmap(df, shape="circle", sizes=mat, row_cluster=False,col_cluster=False, edgecolor=None, approx_clusternum=3, ztranform=False, row_split=True)
-    # plt.show()
+    print(res["axes"].keys())
+    plt.show()
```

