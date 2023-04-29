# Comparing `tmp/custom_plotly_templates-2.0.0.tar.gz` & `tmp/custom_plotly_templates-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custom_plotly_templates-2.0.0.tar", max compression
+gzip compressed data, was "custom_plotly_templates-2.0.1.tar", max compression
```

## Comparing `custom_plotly_templates-2.0.0.tar` & `custom_plotly_templates-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1076 2023-03-06 20:56:23.612630 custom_plotly_templates-2.0.0/LICENSE
--rw-r--r--   0        0        0      734 2023-03-07 08:20:19.124834 custom_plotly_templates-2.0.0/README.md
--rw-r--r--   0        0        0      365 2023-03-07 08:01:19.502306 custom_plotly_templates-2.0.0/custom_plotly_templates/__init__.py
--rw-r--r--   0        0        0      111 2023-03-07 08:01:07.565161 custom_plotly_templates-2.0.0/custom_plotly_templates/_version.py
--rw-r--r--   0        0        0      331 2023-03-06 23:30:09.582412 custom_plotly_templates-2.0.0/custom_plotly_templates/render_config.py
--rw-r--r--   0        0        0      778 2023-03-07 08:01:57.415503 custom_plotly_templates-2.0.0/custom_plotly_templates/templates/__init__.py
--rw-r--r--   0        0        0     1011 2023-03-06 23:30:09.571531 custom_plotly_templates-2.0.0/custom_plotly_templates/templates/white.py
--rw-r--r--   0        0        0      872 2023-03-07 08:07:00.551140 custom_plotly_templates-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 custom_plotly_templates-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-29 09:29:14.140639 custom_plotly_templates-2.0.1/LICENSE
+-rw-r--r--   0        0        0      734 2023-04-29 12:01:47.797827 custom_plotly_templates-2.0.1/README.md
+-rw-r--r--   0        0        0      331 2023-04-29 13:12:37.671115 custom_plotly_templates-2.0.1/custom_plotly_templates/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-29 09:29:14.141013 custom_plotly_templates-2.0.1/custom_plotly_templates/_version.py
+-rw-r--r--   0        0        0      331 2023-04-29 09:29:14.141100 custom_plotly_templates-2.0.1/custom_plotly_templates/render_config.py
+-rw-r--r--   0        0        0      377 2023-04-29 13:12:37.671666 custom_plotly_templates-2.0.1/custom_plotly_templates/templates/__init__.py
+-rw-r--r--   0        0        0     1084 2023-04-29 13:12:37.672084 custom_plotly_templates-2.0.1/custom_plotly_templates/templates/white.py
+-rw-r--r--   0        0        0     1201 2023-04-29 13:12:37.698894 custom_plotly_templates-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 custom_plotly_templates-2.0.1/PKG-INFO
```

### Comparing `custom_plotly_templates-2.0.0/LICENSE` & `custom_plotly_templates-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `custom_plotly_templates-2.0.0/README.md` & `custom_plotly_templates-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `custom_plotly_templates-2.0.0/custom_plotly_templates/templates/white.py` & `custom_plotly_templates-2.0.1/custom_plotly_templates/templates/white.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import plotly.graph_objects as go
 import plotly.io as pio
 
-WHITE_TEMPLATE = pio.templates["plotly_white"]
-WHITE_TEMPLATE.update(
+CUSTOM_WHITE = pio.templates["plotly_white"]
+CUSTOM_WHITE.update(
     dict(
         data=dict(
             histogram=[go.Histogram(histnorm="probability")],
             pie=[go.Pie(textinfo="label+percent", insidetextfont_color="white")],
         ),
         layout=dict(
             font=dict(
                 color="black",
-                size=14,
+                size=14,  # noqa: WPS432
             ),
             xaxis=dict(
                 tickcolor="white",
                 ticklen=5,
                 ticks="outside",
             ),
             yaxis=dict(
@@ -23,14 +23,15 @@
                 ticklen=5,
                 ticks="outside",
             ),
             legend=dict(
                 itemclick="toggleothers",
                 itemdoubleclick="toggle",
             ),
-            margin=dict(t=100, b=40),
+            margin=dict(t=100, b=40),  # noqa: WPS432
             dragmode="pan",
             modebar_remove=["autoScale", "lasso2d", "select"],
             modebar_activecolor="#F39C12",
         ),
     )
 )
+pio.templates["custom_white"] = CUSTOM_WHITE
```

### Comparing `custom_plotly_templates-2.0.0/PKG-INFO` & `custom_plotly_templates-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: custom-plotly-templates
-Version: 2.0.0
+Version: 2.0.1
 Summary: Custom templates and configurations for Plotly
 Home-page: https://github.com/rusmux/custom-plotly-templates
 License: MIT
 Keywords: plotly,template,config
 Author: Ruslan Mukhametshin
 Author-email: rusmux21@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: plotly (>=5.8.0)
+Requires-Dist: plotly (>=5.14.1)
 Description-Content-Type: text/markdown
 
 # Custom plotly templates
 
 [![PyPI](https://img.shields.io/pypi/v/custom-plotly-templates?color=brightgreen)](https://pypi.org/project/custom-plotly-templates/)
 
 [![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://wemake-python-styleguide.readthedocs.io/en/latest/)
```

