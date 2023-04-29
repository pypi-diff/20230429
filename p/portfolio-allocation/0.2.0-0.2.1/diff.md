# Comparing `tmp/portfolio_allocation-0.2.0.tar.gz` & `tmp/portfolio_allocation-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_allocation-0.2.0.tar", last modified: Mon Apr  3 20:42:06 2023, max compression
+gzip compressed data, was "portfolio_allocation-0.2.1.tar", last modified: Sat Apr 29 06:19:29 2023, max compression
```

## Comparing `portfolio_allocation-0.2.0.tar` & `portfolio_allocation-0.2.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/portfolio_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/gnucash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/portfolio_allocation/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/funds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/portfolio_allocation/report/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/portfolio_allocation/report/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/report/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/report/resources/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/report/resources/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/portfolio_allocation/report/resources/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-03 20:42:06.000000 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-03 20:42:06.000000 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 20:42:06.000000 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-03 20:42:06.000000 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-03 20:42:06.000000 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-03 20:42:06.000000 portfolio_allocation-0.2.0/portfolio_allocation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 20:42:06.645005 portfolio_allocation-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-03 20:41:57.000000 portfolio_allocation-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.035043 portfolio_allocation-0.2.1/portfolio_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/gnucash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.039044 portfolio_allocation-0.2.1/portfolio_allocation/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/funds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/portfolio_allocation/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.039044 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/setup.py
```

### Comparing `portfolio_allocation-0.2.0/LICENSE` & `portfolio_allocation-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/PKG-INFO` & `portfolio_allocation-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_allocation
-Version: 0.2.0
+Version: 0.2.1
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.0/README.md` & `portfolio_allocation-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/cli.py` & `portfolio_allocation-0.2.1/portfolio_allocation/cli.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/gnucash.py` & `portfolio_allocation-0.2.1/portfolio_allocation/gnucash.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/instruments/instruments.py` & `portfolio_allocation-0.2.1/portfolio_allocation/instruments/instruments.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/currencies.py` & `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/currencies.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/custom.py` & `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/custom.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/funds.py` & `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/funds.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/instruments/sources/securities.py` & `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/securities.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/report/report.py` & `portfolio_allocation-0.2.1/portfolio_allocation/report/report.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation/report/resources/main.js` & `portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -120,29 +120,33 @@
 
     Object.entries(valuesByParameter).forEach(entry => {
         const parameter = entry[0];
         const values = entry[1];
         const includes = document.createElement("div");
         includes.classList.add('includes');
         includes.id = 'includes-' + parameter;
-        const label = document.createElement("label");
-        label.innerHTML = parameter;
-        includes.appendChild(label);
-        includes.appendChild(document.createElement("br"));
+        const button = document.createElement("button");
+        button.type = "button";
+        button.classList.add('collapsible');
+        button.innerHTML = parameter;
+        includes.appendChild(button);
+        const content = document.createElement("div");
+        content.classList.add('content');
+        includes.appendChild(content);
         values.forEach(value => {
             const checkbox = document.createElement("input");
             checkbox.setAttribute('type', 'checkbox');
             checkbox.setAttribute('checked', 'true');
             checkbox.setAttribute('parameter', parameter);
             checkbox.setAttribute('value', value);
-            includes.appendChild(checkbox);
+            content.appendChild(checkbox);
             const label = document.createElement("label");
             label.innerHTML = value;
-            includes.appendChild(label);
-            includes.appendChild(document.createElement("br"));
+            content.appendChild(label);
+            content.appendChild(document.createElement("br"));
         })
         settings.appendChild(includes);
     });
     const chart = new Chart(document.getElementById("chart"),
         getConfig(allocationBySelect.value, getAllocs(allocationBySelect.value, parameters)));
 
     function updateChart(filter = {}) {
@@ -165,8 +169,16 @@
             } else {
                 filterOut[parameter] = [value];
             }
         });
         console.log("Filter out: " + JSON.stringify(filterOut, null, 4));
         updateChart(filterOut)
     }));
+
+    [].forEach.call(document.getElementsByClassName("collapsible"),
+        elem => elem.addEventListener("click", function() {
+            this.classList.toggle("active");
+            const content = this.nextElementSibling;
+            content.style.display = content.style.display === "block" ? "none" : "block";
+        })
+    );
 }
```

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation.egg-info/PKG-INFO` & `portfolio_allocation-0.2.1/portfolio_allocation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-allocation
-Version: 0.2.0
+Version: 0.2.1
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation.egg-info/SOURCES.txt` & `portfolio_allocation-0.2.1/portfolio_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/portfolio_allocation.egg-info/requires.txt` & `portfolio_allocation-0.2.1/portfolio_allocation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.0/setup.py` & `portfolio_allocation-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name="portfolio_allocation",
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.0",
+    version="0.2.1",
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds",
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

