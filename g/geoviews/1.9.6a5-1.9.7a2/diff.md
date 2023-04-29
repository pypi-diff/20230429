# Comparing `tmp/geoviews-1.9.6a5.tar.gz` & `tmp/geoviews-1.9.7a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoviews-1.9.6a5.tar", last modified: Tue Jan 17 08:21:34 2023, max compression
+gzip compressed data, was "geoviews-1.9.7a2.tar", last modified: Sat Apr  8 12:50:27 2023, max compression
```

## Comparing `geoviews-1.9.6a5.tar` & `geoviews-1.9.7a2.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.818322 geoviews-1.9.6a5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/Homepage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.822322 geoviews-1.9.6a5/examples/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.822322 geoviews-1.9.6a5/examples/assets/boundaries/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/assets/boundaries/boundaries.dbf
--rwxr-xr-x   0 runner    (1001) docker     (123)   341072 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/assets/boundaries/boundaries.shp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3292 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/assets/boundaries/boundaries.shx
--rw-r--r--   0 runner    (1001) docker     (123)   496370 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/assets/cities.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/assets/referendum.csv
--rw-r--r--   0 runner    (1001) docker     (123)   100504 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/assets/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/datasets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.818322 geoviews-1.9.6a5/examples/gallery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.822322 geoviews-1.9.6a5/examples/gallery/bokeh/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/airport_graph.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/brexit_choropleth.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/city_populations_2050.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/filled_contours.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/great_circle.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/katrina_track.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/new_york_boroughs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/orthographic_vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/tile_sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/trimesh_uk.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/vectorfield_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/world_population.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/xarray_image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/bokeh/xarray_quadmesh.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.826322 geoviews-1.9.6a5/examples/gallery/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/airport_graph.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/brexit_choropleth.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/city_population.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/filled_contours.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/great_circle.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/katrina_track.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/new_york_boroughs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/orthographic_vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/tile_sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/trimesh_uk.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/vectorfield_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/world_population.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/xarray_image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/gallery/matplotlib/xarray_quadmesh.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.826322 geoviews-1.9.6a5/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Annotators.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Geometries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Gridded_Datasets_I.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Gridded_Datasets_II.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Projections.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Resampling_Grids.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/examples/user_guide/Working_with_Bokeh.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.826322 geoviews-1.9.6a5/geoviews/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-01-17 08:21:31.000000 geoviews-1.9.6a5/geoviews/.version
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/annotators.py
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/bokeh.ext.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.826322 geoviews-1.9.6a5/geoviews/data/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/data/geom_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/data/geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/data/iris.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.830322 geoviews-1.9.6a5/geoviews/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/geoviews.js
--rw-r--r--   0 runner    (1001) docker     (123)    27225 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/geoviews.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77416 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/geoviews.json
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/geoviews.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.830322 geoviews-1.9.6a5/geoviews/dist/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/index.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.830322 geoviews-1.9.6a5/geoviews/dist/lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/checkpoint_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/checkpoint_tool.js
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/checkpoint_tool.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/clear_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/clear_tool.js
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/clear_tool.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/index.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/index.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/poly_draw.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/poly_draw.js
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/poly_draw.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/poly_edit.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/poly_edit.js
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/poly_edit.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/restore_tool.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/restore_tool.js
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews/dist/lib/models/restore_tool.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.830322 geoviews-1.9.6a5/geoviews/element/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/element/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)    33180 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/element/geo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.830322 geoviews-1.9.6a5/geoviews/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/Homepage.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.830322 geoviews-1.9.6a5/geoviews/examples/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.834322 geoviews-1.9.6a5/geoviews/examples/assets/boundaries/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/assets/boundaries/boundaries.dbf
--rwxr-xr-x   0 runner    (1001) docker     (123)   341072 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/assets/boundaries/boundaries.shp
--rwxr-xr-x   0 runner    (1001) docker     (123)     3292 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/assets/boundaries/boundaries.shx
--rw-r--r--   0 runner    (1001) docker     (123)   496370 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/assets/cities.csv
--rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/assets/referendum.csv
--rw-r--r--   0 runner    (1001) docker     (123)   100504 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/assets/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/datasets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.818322 geoviews-1.9.6a5/geoviews/examples/gallery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.834322 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/airport_graph.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/brexit_choropleth.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/city_populations_2050.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/filled_contours.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/great_circle.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/katrina_track.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/new_york_boroughs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/orthographic_vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/tile_sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/trimesh_uk.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/vectorfield_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/world_population.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/xarray_image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/xarray_quadmesh.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.834322 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/airport_graph.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/brexit_choropleth.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/city_population.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/filled_contours.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/great_circle.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/katrina_track.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/new_york_boroughs.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/orthographic_vectorfield.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/tile_sources.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/trimesh_uk.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/vectorfield_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/world_population.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/xarray_image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/xarray_quadmesh.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Annotators.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Geometries.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Gridded_Datasets_I.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Gridded_Datasets_II.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Projections.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Resampling_Grids.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/examples/user_guide/Working_with_Bokeh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/icons/DenoteBackground.png
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/icons/DenoteForeground.png
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/icons/PolyBreak.png
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/links.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/models/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/checkpoint_tool.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/clear_tool.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/custom_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/poly_draw.ts
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/poly_edit.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/models/restore_tool.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/operation/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/operation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/operation/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/operation/regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/operation/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)    31961 2023-01-17 08:20:47.000000 geoviews-1.9.6a5/geoviews/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/plotting/bokeh/
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/plotting/bokeh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/plotting/bokeh/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/plotting/bokeh/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/plotting/mpl/
--rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/plotting/mpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/geoviews/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/data/test_geopandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/data/test_iris.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/data/test_multigeometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/test_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tile_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/geoviews/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 08:21:34.826322 geoviews-1.9.6a5/geoviews.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-17 08:21:34.000000 geoviews-1.9.6a5/geoviews.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-01-17 08:21:34.838322 geoviews-1.9.6a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-01-17 08:15:29.000000 geoviews-1.9.6a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.731918 geoviews-1.9.7a2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/Homepage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.731918 geoviews-1.9.7a2/examples/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.731918 geoviews-1.9.7a2/examples/assets/boundaries/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/assets/boundaries/boundaries.dbf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   341072 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/assets/boundaries/boundaries.shp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3292 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/assets/boundaries/boundaries.shx
+-rw-r--r--   0 runner    (1001) docker     (123)   496370 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/assets/cities.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/assets/referendum.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   100504 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/assets/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/datasets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.727918 geoviews-1.9.7a2/examples/gallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.735919 geoviews-1.9.7a2/examples/gallery/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/airport_graph.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/brexit_choropleth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/city_populations_2050.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/filled_contours.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/great_circle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/katrina_track.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/new_york_boroughs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/orthographic_vectorfield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/tile_sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/trimesh_uk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/vectorfield_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/world_population.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/xarray_image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/bokeh/xarray_quadmesh.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.735919 geoviews-1.9.7a2/examples/gallery/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/airport_graph.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/brexit_choropleth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/city_population.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/filled_contours.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/great_circle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/katrina_track.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/new_york_boroughs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/orthographic_vectorfield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/tile_sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/trimesh_uk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/vectorfield_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/world_population.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/xarray_image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/gallery/matplotlib/xarray_quadmesh.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.739919 geoviews-1.9.7a2/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Annotators.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Geometries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Gridded_Datasets_I.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Gridded_Datasets_II.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Projections.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Resampling_Grids.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/examples/user_guide/Working_with_Bokeh.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.739919 geoviews-1.9.7a2/geoviews/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-08 12:50:24.000000 geoviews-1.9.7a2/geoviews/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/annotators.py
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/bokeh.ext.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.739919 geoviews-1.9.7a2/geoviews/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/data/geom_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23979 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/data/geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14993 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/data/iris.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.743919 geoviews-1.9.7a2/geoviews/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    25756 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/geoviews.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27225 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/geoviews.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77416 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/geoviews.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/geoviews.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.743919 geoviews-1.9.7a2/geoviews/dist/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/index.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.743919 geoviews-1.9.7a2/geoviews/dist/lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/checkpoint_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/checkpoint_tool.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/checkpoint_tool.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/clear_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/clear_tool.js
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/clear_tool.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/index.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/index.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/poly_draw.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/poly_draw.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/poly_draw.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/poly_edit.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/poly_edit.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/poly_edit.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/restore_tool.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/restore_tool.js
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews/dist/lib/models/restore_tool.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.743919 geoviews-1.9.7a2/geoviews/element/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/element/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/element/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33180 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/element/geo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.743919 geoviews-1.9.7a2/geoviews/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/Homepage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.747920 geoviews-1.9.7a2/geoviews/examples/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.747920 geoviews-1.9.7a2/geoviews/examples/assets/boundaries/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/assets/boundaries/boundaries.dbf
+-rwxr-xr-x   0 runner    (1001) docker     (123)   341072 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/assets/boundaries/boundaries.shp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3292 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/assets/boundaries/boundaries.shx
+-rw-r--r--   0 runner    (1001) docker     (123)   496370 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/assets/cities.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23034 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/assets/referendum.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   100504 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/assets/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/datasets.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.727918 geoviews-1.9.7a2/geoviews/examples/gallery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.751920 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/airport_graph.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/brexit_choropleth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/city_populations_2050.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/filled_contours.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/great_circle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/katrina_track.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/new_york_boroughs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/orthographic_vectorfield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/tile_sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/trimesh_uk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/vectorfield_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/world_population.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/xarray_image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/xarray_quadmesh.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.751920 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/airport_graph.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/brexit_choropleth.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/city_population.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/filled_contours.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/great_circle.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/katrina_track.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/new_york_boroughs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/orthographic_vectorfield.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/tile_sources.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/trimesh_uk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/vectorfield_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/world_population.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/xarray_image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/xarray_quadmesh.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.751920 geoviews-1.9.7a2/geoviews/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Annotators.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11979 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Geometries.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Gridded_Datasets_I.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12831 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Gridded_Datasets_II.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Projections.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Resampling_Grids.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/examples/user_guide/Working_with_Bokeh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.751920 geoviews-1.9.7a2/geoviews/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/icons/DenoteBackground.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/icons/DenoteForeground.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/icons/PolyBreak.png
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/links.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/checkpoint_tool.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/clear_tool.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/custom_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/poly_draw.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/poly_edit.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/models/restore_tool.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/operation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/operation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18041 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/operation/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/operation/regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/operation/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31953 2023-04-08 12:49:51.000000 geoviews-1.9.7a2/geoviews/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/plotting/bokeh/
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/plotting/bokeh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/plotting/bokeh/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/plotting/bokeh/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/plotting/mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/plotting/mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.755921 geoviews-1.9.7a2/geoviews/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/data/test_geopandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/data/test_iris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/data/test_multigeometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/test_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tile_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25666 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/geoviews/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:50:27.739919 geoviews-1.9.7a2/geoviews.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 12:50:27.000000 geoviews-1.9.7a2/geoviews.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-08 12:50:27.759921 geoviews-1.9.7a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-04-08 12:43:16.000000 geoviews-1.9.7a2/setup.py
```

### Comparing `geoviews-1.9.6a5/LICENSE` & `geoviews-1.9.7a2/LICENSE`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/PKG-INFO` & `geoviews-1.9.7a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoviews
-Version: 1.9.6a5
+Version: 1.9.7a2
 Summary: GeoViews is a Python library that makes it easy to explore and visualize geographical, meteorological, and oceanographic datasets, such as those used in weather, climate, and remote sensing research.
 Home-page: https://geoviews.org
 License: BSD 3-Clause
 Platform: Windows
 Platform: Mac OS X
 Platform: Linux
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `geoviews-1.9.6a5/README.md` & `geoviews-1.9.7a2/README.md`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/Homepage.ipynb` & `geoviews-1.9.7a2/examples/Homepage.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/assets/boundaries/boundaries.dbf` & `geoviews-1.9.7a2/examples/assets/boundaries/boundaries.dbf`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/assets/boundaries/boundaries.shp` & `geoviews-1.9.7a2/examples/assets/boundaries/boundaries.shp`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/assets/boundaries/boundaries.shx` & `geoviews-1.9.7a2/examples/assets/boundaries/boundaries.shx`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/assets/cities.csv` & `geoviews-1.9.7a2/examples/assets/cities.csv`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/assets/referendum.csv` & `geoviews-1.9.7a2/examples/assets/referendum.csv`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/assets/results.json` & `geoviews-1.9.7a2/examples/assets/results.json`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/airport_graph.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/airport_graph.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/brexit_choropleth.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/brexit_choropleth.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/city_populations_2050.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/city_populations_2050.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/filled_contours.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/filled_contours.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/great_circle.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/great_circle.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/katrina_track.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/katrina_track.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/new_york_boroughs.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/new_york_boroughs.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/orthographic_vectorfield.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/orthographic_vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/tile_sources.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/tile_sources.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/trimesh_uk.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/trimesh_uk.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/vectorfield_example.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/vectorfield_example.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/world_population.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/world_population.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/xarray_image.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/xarray_image.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/bokeh/xarray_quadmesh.ipynb` & `geoviews-1.9.7a2/examples/gallery/bokeh/xarray_quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/airport_graph.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/airport_graph.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/brexit_choropleth.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/brexit_choropleth.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/city_population.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/city_population.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/filled_contours.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/filled_contours.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/great_circle.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/great_circle.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/katrina_track.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/katrina_track.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/new_york_boroughs.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/new_york_boroughs.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/orthographic_vectorfield.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/orthographic_vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/tile_sources.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/tile_sources.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/trimesh_uk.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/trimesh_uk.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/vectorfield_example.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/vectorfield_example.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/world_population.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/world_population.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/xarray_image.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/xarray_image.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/gallery/matplotlib/xarray_quadmesh.ipynb` & `geoviews-1.9.7a2/examples/gallery/matplotlib/xarray_quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Annotators.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Annotators.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Geometries.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Geometries.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Gridded_Datasets_I.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Gridded_Datasets_I.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Gridded_Datasets_II.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Gridded_Datasets_II.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Projections.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Projections.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Resampling_Grids.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Resampling_Grids.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/examples/user_guide/Working_with_Bokeh.ipynb` & `geoviews-1.9.7a2/examples/user_guide/Working_with_Bokeh.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/__init__.py` & `geoviews-1.9.7a2/geoviews/__init__.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/annotators.py` & `geoviews-1.9.7a2/geoviews/annotators.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/data/geom_dict.py` & `geoviews-1.9.7a2/geoviews/data/geom_dict.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/data/geopandas.py` & `geoviews-1.9.7a2/geoviews/data/geopandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,30 @@
 from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 
 from holoviews.core.util import isscalar, unique_iterator, unique_array
 from holoviews.core.data import Dataset, Interface, MultiInterface
-from holoviews.core.data.interface  import DataError
+from holoviews.core.data.interface import DataError
 from holoviews.core.data import PandasInterface
 from holoviews.core.data.spatialpandas import get_value_array
 from holoviews.core.dimension import dimension_name
 from holoviews.element import Path
 
 from ..util import asarray, geom_to_array, geom_types, geom_length
 from .geom_dict import geom_from_dict
 
+try:
+    from holoviews.core.data import PandasAPI
+except ImportError:
+    class PandasAPI: pass
 
-class GeoPandasInterface(MultiInterface):
+
+class GeoPandasInterface(PandasAPI, MultiInterface):
 
     types = ()
 
     datatype = 'geodataframe'
 
     multi = True
```

### Comparing `geoviews-1.9.6a5/geoviews/data/iris.py` & `geoviews-1.9.7a2/geoviews/data/iris.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/geoviews.js` & `geoviews-1.9.7a2/geoviews/dist/geoviews.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/geoviews.js.map` & `geoviews-1.9.7a2/geoviews/dist/geoviews.js.map`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/geoviews.json` & `geoviews-1.9.7a2/geoviews/dist/geoviews.json`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/geoviews.min.js` & `geoviews-1.9.7a2/geoviews/dist/geoviews.min.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/checkpoint_tool.d.ts` & `geoviews-1.9.7a2/geoviews/dist/lib/models/checkpoint_tool.d.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/checkpoint_tool.js` & `geoviews-1.9.7a2/geoviews/dist/lib/models/checkpoint_tool.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/checkpoint_tool.js.map` & `geoviews-1.9.7a2/geoviews/dist/lib/models/checkpoint_tool.js.map`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/clear_tool.d.ts` & `geoviews-1.9.7a2/geoviews/dist/lib/models/clear_tool.d.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/clear_tool.js` & `geoviews-1.9.7a2/geoviews/dist/lib/models/clear_tool.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/clear_tool.js.map` & `geoviews-1.9.7a2/geoviews/dist/lib/models/clear_tool.js.map`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/poly_draw.d.ts` & `geoviews-1.9.7a2/geoviews/dist/lib/models/poly_draw.d.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/poly_draw.js` & `geoviews-1.9.7a2/geoviews/dist/lib/models/poly_draw.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/poly_draw.js.map` & `geoviews-1.9.7a2/geoviews/dist/lib/models/poly_draw.js.map`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/poly_edit.d.ts` & `geoviews-1.9.7a2/geoviews/dist/lib/models/poly_edit.d.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/poly_edit.js` & `geoviews-1.9.7a2/geoviews/dist/lib/models/poly_edit.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/poly_edit.js.map` & `geoviews-1.9.7a2/geoviews/dist/lib/models/poly_edit.js.map`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/restore_tool.d.ts` & `geoviews-1.9.7a2/geoviews/dist/lib/models/restore_tool.d.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/restore_tool.js` & `geoviews-1.9.7a2/geoviews/dist/lib/models/restore_tool.js`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/dist/lib/models/restore_tool.js.map` & `geoviews-1.9.7a2/geoviews/dist/lib/models/restore_tool.js.map`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/element/__init__.py` & `geoviews-1.9.7a2/geoviews/element/__init__.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/element/comparison.py` & `geoviews-1.9.7a2/geoviews/element/comparison.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/element/geo.py` & `geoviews-1.9.7a2/geoviews/element/geo.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/Homepage.ipynb` & `geoviews-1.9.7a2/geoviews/examples/Homepage.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/assets/boundaries/boundaries.dbf` & `geoviews-1.9.7a2/geoviews/examples/assets/boundaries/boundaries.dbf`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/assets/boundaries/boundaries.shp` & `geoviews-1.9.7a2/geoviews/examples/assets/boundaries/boundaries.shp`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/assets/boundaries/boundaries.shx` & `geoviews-1.9.7a2/geoviews/examples/assets/boundaries/boundaries.shx`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/assets/cities.csv` & `geoviews-1.9.7a2/geoviews/examples/assets/cities.csv`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/assets/referendum.csv` & `geoviews-1.9.7a2/geoviews/examples/assets/referendum.csv`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/assets/results.json` & `geoviews-1.9.7a2/geoviews/examples/assets/results.json`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/airport_graph.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/airport_graph.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/brexit_choropleth.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/brexit_choropleth.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/city_populations_2050.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/city_populations_2050.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/filled_contours.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/filled_contours.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/great_circle.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/great_circle.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/katrina_track.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/katrina_track.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/new_york_boroughs.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/new_york_boroughs.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/orthographic_vectorfield.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/orthographic_vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/tile_sources.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/tile_sources.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/trimesh_uk.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/trimesh_uk.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/vectorfield_example.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/vectorfield_example.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/world_population.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/world_population.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/xarray_image.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/xarray_image.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/bokeh/xarray_quadmesh.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/bokeh/xarray_quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/airport_graph.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/airport_graph.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/brexit_choropleth.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/brexit_choropleth.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/city_population.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/city_population.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/filled_contours.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/filled_contours.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/great_circle.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/great_circle.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/katrina_track.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/katrina_track.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/new_york_boroughs.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/new_york_boroughs.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/orthographic_vectorfield.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/orthographic_vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/tile_sources.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/tile_sources.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/trimesh_uk.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/trimesh_uk.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/vectorfield_example.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/vectorfield_example.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/world_population.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/world_population.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/xarray_image.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/xarray_image.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/gallery/matplotlib/xarray_quadmesh.ipynb` & `geoviews-1.9.7a2/geoviews/examples/gallery/matplotlib/xarray_quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Annotators.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Annotators.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Geometries.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Geometries.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Gridded_Datasets_I.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Gridded_Datasets_I.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Gridded_Datasets_II.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Gridded_Datasets_II.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Projections.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Projections.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Resampling_Grids.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Resampling_Grids.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/examples/user_guide/Working_with_Bokeh.ipynb` & `geoviews-1.9.7a2/geoviews/examples/user_guide/Working_with_Bokeh.ipynb`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/feature.py` & `geoviews-1.9.7a2/geoviews/feature.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/icons/DenoteBackground.png` & `geoviews-1.9.7a2/geoviews/icons/DenoteBackground.png`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/icons/DenoteForeground.png` & `geoviews-1.9.7a2/geoviews/icons/DenoteForeground.png`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/icons/PolyBreak.png` & `geoviews-1.9.7a2/geoviews/icons/PolyBreak.png`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/links.py` & `geoviews-1.9.7a2/geoviews/links.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/models/checkpoint_tool.ts` & `geoviews-1.9.7a2/geoviews/models/checkpoint_tool.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/models/clear_tool.ts` & `geoviews-1.9.7a2/geoviews/models/clear_tool.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/models/custom_tools.py` & `geoviews-1.9.7a2/geoviews/models/custom_tools.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/models/poly_draw.ts` & `geoviews-1.9.7a2/geoviews/models/poly_draw.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/models/poly_edit.ts` & `geoviews-1.9.7a2/geoviews/models/poly_edit.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/models/restore_tool.ts` & `geoviews-1.9.7a2/geoviews/models/restore_tool.ts`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/operation/__init__.py` & `geoviews-1.9.7a2/geoviews/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/operation/projection.py` & `geoviews-1.9.7a2/geoviews/operation/projection.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/operation/regrid.py` & `geoviews-1.9.7a2/geoviews/operation/regrid.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/operation/resample.py` & `geoviews-1.9.7a2/geoviews/operation/resample.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/package-lock.json` & `geoviews-1.9.7a2/geoviews/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9165865384615385%*

 * *Differences: {"'packages'": "{'': {'version': '1.9.6'}}", "'version'": "'1.9.6'"}*

```diff
@@ -385,15 +385,15 @@
         "": {
             "dependencies": {
                 "@bokeh/bokehjs": "^2.4.2"
             },
             "devDependencies": {},
             "license": "BSD-3-Clause",
             "name": "@holoviz/geoviews",
-            "version": "1.9.6-a.5"
+            "version": "1.9.6"
         },
         "node_modules/@bokeh/bokehjs": {
             "dependencies": {
                 "@bokeh/numbro": "^1.6.2",
                 "@bokeh/slickgrid": "~2.4.2702",
                 "choices.js": "^9.0.1",
                 "es5-ext": "^0.10.53",
@@ -795,9 +795,9 @@
             },
             "integrity": "sha512-f9s+fUkX04BxQf+7mMWAp5zk61pciie+fFLC9hX9UVvCeJQfNHRHXpeo5MPcR0EUf57PYLdt+ZO4f3Ipk2oZUw==",
             "resolved": "https://registry.npmjs.org/xmldom-sre/-/xmldom-sre-0.1.31.tgz",
             "version": "0.1.31"
         }
     },
     "requires": true,
-    "version": "1.9.6-a.5"
+    "version": "1.9.6"
 }
```

### Comparing `geoviews-1.9.6a5/geoviews/plotting/__init__.py` & `geoviews-1.9.7a2/geoviews/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/plotting/bokeh/__init__.py` & `geoviews-1.9.7a2/geoviews/plotting/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/plotting/bokeh/callbacks.py` & `geoviews-1.9.7a2/geoviews/plotting/bokeh/callbacks.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/plotting/bokeh/plot.py` & `geoviews-1.9.7a2/geoviews/plotting/bokeh/plot.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/plotting/mpl/__init__.py` & `geoviews-1.9.7a2/geoviews/plotting/mpl/__init__.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/plotting/plot.py` & `geoviews-1.9.7a2/geoviews/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/streams.py` & `geoviews-1.9.7a2/geoviews/streams.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tests/data/test_geopandas.py` & `geoviews-1.9.7a2/geoviews/tests/data/test_geopandas.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tests/data/test_iris.py` & `geoviews-1.9.7a2/geoviews/tests/data/test_iris.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tests/data/test_multigeometry.py` & `geoviews-1.9.7a2/geoviews/tests/data/test_multigeometry.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tests/test_conversions.py` & `geoviews-1.9.7a2/geoviews/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tests/test_element.py` & `geoviews-1.9.7a2/geoviews/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tests/test_projection.py` & `geoviews-1.9.7a2/geoviews/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tile_sources.py` & `geoviews-1.9.7a2/geoviews/tile_sources.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/tsconfig.json` & `geoviews-1.9.7a2/geoviews/tsconfig.json`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews/util.py` & `geoviews-1.9.7a2/geoviews/util.py`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews.egg-info/PKG-INFO` & `geoviews-1.9.7a2/geoviews.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoviews
-Version: 1.9.6a5
+Version: 1.9.7a2
 Summary: GeoViews is a Python library that makes it easy to explore and visualize geographical, meteorological, and oceanographic datasets, such as those used in weather, climate, and remote sensing research.
 Home-page: https://geoviews.org
 License: BSD 3-Clause
 Platform: Windows
 Platform: Mac OS X
 Platform: Linux
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `geoviews-1.9.6a5/geoviews.egg-info/SOURCES.txt` & `geoviews-1.9.7a2/geoviews.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geoviews-1.9.6a5/geoviews.egg-info/requires.txt` & `geoviews-1.9.7a2/geoviews.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 bokeh<2.5,>=2.4.0
 cartopy>=0.18.0
 holoviews>=1.14.2
 packaging
 numpy
 shapely
 param
-panel
+panel<1.0.0
 
 [all]
 cartopy>=0.20.0
 codecov
 datashader
 fiona
 flake8
```

### Comparing `geoviews-1.9.6a5/setup.py` & `geoviews-1.9.7a2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     'bokeh >=2.4.0,<2.5',
     'cartopy >=0.18.0',
     'holoviews >=1.14.2',
     'packaging',
     'numpy',
     'shapely',
     'param',
-    'panel',
+    'panel <1.0.0',
 ]
 
 _recommended = [
     # geopandas-base installed with conda, see setup.cfg
     'geopandas',
     'netcdf4',
     'jupyter',
```

