# Comparing `tmp/pyobsplot-0.3.3.tar.gz` & `tmp/pyobsplot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobsplot-0.3.3.tar", max compression
+gzip compressed data, was "pyobsplot-0.3.4.tar", max compression
```

## Comparing `pyobsplot-0.3.3.tar` & `pyobsplot-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.3/LICENSE
--rw-r--r--   0        0        0     4287 2023-04-16 14:13:49.662823 pyobsplot-0.3.3/README.md
--rw-r--r--   0        0        0     1303 2023-04-23 17:32:40.447995 pyobsplot-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      535 2023-04-23 14:58:02.739444 pyobsplot-0.3.3/src/pyobsplot/__init__.py
--rw-r--r--   0        0        0     3428 2023-04-11 14:13:06.230946 pyobsplot-0.3.3/src/pyobsplot/data.py
--rw-r--r--   0        0        0     1894 2023-04-23 17:25:31.529014 pyobsplot-0.3.3/src/pyobsplot/jsdom.py
--rw-r--r--   0        0        0     2363 2023-04-14 11:09:43.659346 pyobsplot-0.3.3/src/pyobsplot/jsmodules.py
--rw-r--r--   0        0        0     5896 2023-04-23 17:28:15.464378 pyobsplot-0.3.3/src/pyobsplot/obsplot.py
--rw-r--r--   0        0        0     6158 2023-04-11 14:11:53.254582 pyobsplot-0.3.3/src/pyobsplot/parsing.py
--rw-r--r--   0        0        0       89 2023-04-23 17:34:03.547991 pyobsplot-0.3.3/src/pyobsplot/static/styles.css
--rw-r--r--   0        0        0  2268563 2023-04-23 17:34:03.547991 pyobsplot-0.3.3/src/pyobsplot/static/widget.js
--rw-r--r--   0        0        0     2552 2023-04-23 17:25:05.613152 pyobsplot-0.3.3/src/pyobsplot/utils.py
--rw-r--r--   0        0        0     1437 2023-04-23 17:12:16.978286 pyobsplot-0.3.3/src/pyobsplot/widget.py
--rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 pyobsplot-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-03-29 08:42:01.834769 pyobsplot-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4287 2023-04-16 14:13:49.662823 pyobsplot-0.3.4/README.md
+-rw-r--r--   0        0        0     1303 2023-04-29 17:24:25.836005 pyobsplot-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      535 2023-04-23 14:58:02.739444 pyobsplot-0.3.4/src/pyobsplot/__init__.py
+-rw-r--r--   0        0        0     3428 2023-04-11 14:13:06.230946 pyobsplot-0.3.4/src/pyobsplot/data.py
+-rw-r--r--   0        0        0     1894 2023-04-23 17:25:31.529014 pyobsplot-0.3.4/src/pyobsplot/jsdom.py
+-rw-r--r--   0        0        0     2363 2023-04-14 11:09:43.659346 pyobsplot-0.3.4/src/pyobsplot/jsmodules.py
+-rw-r--r--   0        0        0     5896 2023-04-23 17:28:15.464378 pyobsplot-0.3.4/src/pyobsplot/obsplot.py
+-rw-r--r--   0        0        0     6158 2023-04-11 14:11:53.254582 pyobsplot-0.3.4/src/pyobsplot/parsing.py
+-rw-r--r--   0        0        0       89 2023-04-29 17:17:08.752054 pyobsplot-0.3.4/src/pyobsplot/static/styles.css
+-rw-r--r--   0        0        0  2272243 2023-04-29 17:17:08.752054 pyobsplot-0.3.4/src/pyobsplot/static/widget.js
+-rw-r--r--   0        0        0     2567 2023-04-29 17:16:20.416829 pyobsplot-0.3.4/src/pyobsplot/utils.py
+-rw-r--r--   0        0        0     1437 2023-04-23 17:12:16.978286 pyobsplot-0.3.4/src/pyobsplot/widget.py
+-rw-r--r--   0        0        0     5645 1970-01-01 00:00:00.000000 pyobsplot-0.3.4/PKG-INFO
```

### Comparing `pyobsplot-0.3.3/LICENSE` & `pyobsplot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/README.md` & `pyobsplot-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/pyproject.toml` & `pyobsplot-0.3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyobsplot"
-version = "0.3.3"
+version = "0.3.4"
 description = "Observable Plot in Jupyter notebooks and Quarto documents"
 authors = ["Julien Barnier <julien@nozav.org>"]
 license = "MIT"
 readme = "README.md"
 include = ["src/pyobsplot/static/*"]
 homepage = "https://github.com/juba/pyobsplot"
 documentation = "https://juba.github.io/pyobsplot"
@@ -19,15 +19,15 @@
 ]
 
 [tool.poetry.urls]
 changelog = "https://github.com/juba/pyobsplot/blob/main/NEWS.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-anywidget = {extras = ["dev"], version = "^0.2.2"}
+anywidget = {extras = ["dev"], version = "^0.2.3"}
 pandas = ">=1.2.0"
 polars = ">=0.16.0"
 pyarrow = "^11.0.0"
 ipywidgets = ">=8.0.0"
 jupyterlab_widgets = ">=3.0.0"
 jupyterlab = ">=3.6.0"
 requests = "^2.28.2"
```

### Comparing `pyobsplot-0.3.3/src/pyobsplot/__init__.py` & `pyobsplot-0.3.4/src/pyobsplot/__init__.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/src/pyobsplot/data.py` & `pyobsplot-0.3.4/src/pyobsplot/data.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/src/pyobsplot/jsdom.py` & `pyobsplot-0.3.4/src/pyobsplot/jsdom.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/src/pyobsplot/jsmodules.py` & `pyobsplot-0.3.4/src/pyobsplot/jsmodules.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/src/pyobsplot/obsplot.py` & `pyobsplot-0.3.4/src/pyobsplot/obsplot.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/src/pyobsplot/parsing.py` & `pyobsplot-0.3.4/src/pyobsplot/parsing.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/src/pyobsplot/static/widget.js` & `pyobsplot-0.3.4/src/pyobsplot/static/widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1078,14 +1078,15 @@
     groupZ: () => groupZ,
     hexagon: () => hexagon,
     hexbin: () => hexbin,
     hexgrid: () => hexgrid,
     hull: () => hull,
     identity: () => identity6,
     image: () => image,
+    indexOf: () => indexOf,
     initializer: () => initializer,
     interpolateNearest: () => interpolateNearest,
     interpolateNone: () => interpolateNone,
     interpolatorBarycentric: () => interpolatorBarycentric,
     interpolatorRandomWalk: () => interpolatorRandomWalk,
     legend: () => legend,
     line: () => line,
@@ -1151,15 +1152,15 @@
 var src_exports = {};
 __export(src_exports, {
     Adder: () => Adder,
     Delaunay: () => Delaunay,
     FormatSpecifier: () => FormatSpecifier,
     InternMap: () => InternMap,
     InternSet: () => InternSet,
-    Node: () => Node2,
+    Node: () => Node,
     Path: () => Path,
     Voronoi: () => Voronoi,
     ZoomTransform: () => Transform,
     active: () => active_default,
     arc: () => arc_default,
     area: () => area_default5,
     areaRadial: () => areaRadial_default,
@@ -3267,15 +3268,15 @@
     function axis3(context) {
         var values3 = tickValues == null ? scale5.ticks ? scale5.ticks.apply(scale5, tickArguments) : scale5.domain() : tickValues,
             format5 = tickFormat3 == null ? scale5.tickFormat ? scale5.tickFormat.apply(scale5, tickArguments) : identity_default : tickFormat3,
             spacing = Math.max(tickSizeInner, 0) + tickPadding,
             range9 = scale5.range(),
             range0 = +range9[0] + offset3,
             range1 = +range9[range9.length - 1] + offset3,
-            position3 = (scale5.bandwidth ? center : number2)(scale5.copy(), offset3),
+            position5 = (scale5.bandwidth ? center : number2)(scale5.copy(), offset3),
             selection3 = context.selection ? context.selection() : context,
             path3 = selection3.selectAll(".domain").data([null]),
             tick = selection3.selectAll(".tick").data(values3, scale5).order(),
             tickExit = tick.exit(),
             tickEnter = tick.enter().append("g").attr("class", "tick"),
             line3 = tick.select("line"),
             text3 = tick.select("text");
@@ -3285,31 +3286,31 @@
         text3 = text3.merge(tickEnter.append("text").attr("fill", "currentColor").attr(x7, k3 * spacing).attr("dy", orient === top ? "0em" : orient === bottom ? "0.71em" : "0.32em"));
         if (context !== selection3) {
             path3 = path3.transition(context);
             tick = tick.transition(context);
             line3 = line3.transition(context);
             text3 = text3.transition(context);
             tickExit = tickExit.transition(context).attr("opacity", epsilon).attr("transform", function(d) {
-                return isFinite(d = position3(d)) ? transform3(d + offset3) : this.getAttribute("transform");
+                return isFinite(d = position5(d)) ? transform3(d + offset3) : this.getAttribute("transform");
             });
             tickEnter.attr("opacity", epsilon).attr("transform", function(d) {
                 var p = this.parentNode.__axis;
-                return transform3((p && isFinite(p = p(d)) ? p : position3(d)) + offset3);
+                return transform3((p && isFinite(p = p(d)) ? p : position5(d)) + offset3);
             });
         }
         tickExit.remove();
         path3.attr("d", orient === left || orient === right ? tickSizeOuter ? "M" + k3 * tickSizeOuter + "," + range0 + "H" + offset3 + "V" + range1 + "H" + k3 * tickSizeOuter : "M" + offset3 + "," + range0 + "V" + range1 : tickSizeOuter ? "M" + range0 + "," + k3 * tickSizeOuter + "V" + offset3 + "H" + range1 + "V" + k3 * tickSizeOuter : "M" + range0 + "," + offset3 + "H" + range1);
         tick.attr("opacity", 1).attr("transform", function(d) {
-            return transform3(position3(d) + offset3);
+            return transform3(position5(d) + offset3);
         });
         line3.attr(x7 + "2", k3 * tickSizeInner);
         text3.attr(x7, k3 * spacing).text(format5);
         selection3.filter(entering).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", orient === right ? "start" : orient === left ? "end" : "middle");
         selection3.each(function() {
-            this.__axis = position3;
+            this.__axis = position5;
         });
     }
     axis3.scale = function(_) {
         return arguments.length ? (scale5 = _, axis3) : scale5;
     };
     axis3.ticks = function() {
         return tickArguments = Array.from(arguments), axis3;
@@ -15341,22 +15342,22 @@
     if (data instanceof Map) {
         data = [void 0, data];
         if (children3 === void 0)
             children3 = mapChildren;
     } else if (children3 === void 0) {
         children3 = objectChildren;
     }
-    var root5 = new Node2(data),
+    var root5 = new Node(data),
         node, nodes = [root5],
         child, childs, i, n;
     while (node = nodes.pop()) {
         if ((childs = children3(node.data)) && (n = (childs = Array.from(childs)).length)) {
             node.children = childs;
             for (i = n - 1; i >= 0; --i) {
-                nodes.push(child = childs[i] = new Node2(childs[i]));
+                nodes.push(child = childs[i] = new Node(childs[i]));
                 child.parent = node;
                 child.depth = node.depth + 1;
             }
         }
     }
     return root5.eachBefore(computeHeight);
 }
@@ -15382,21 +15383,21 @@
 function computeHeight(node) {
     var height = 0;
     do
         node.height = height;
     while ((node = node.parent) && node.height < ++height);
 }
 
-function Node2(data) {
+function Node(data) {
     this.data = data;
     this.depth = this.height = 0;
     this.parent = null;
 }
-Node2.prototype = hierarchy.prototype = {
-    constructor: Node2,
+Node.prototype = hierarchy.prototype = {
+    constructor: Node,
     count: count_default,
     each: each_default2,
     eachAfter: eachAfter_default,
     eachBefore: eachBefore_default,
     find: find_default2,
     sum: sum_default,
     sort: sort_default2,
@@ -15629,15 +15630,15 @@
         b = node.next._,
         ab7 = a7.r + b.r,
         dx = (a7.x * b.r + b.x * a7.r) / ab7,
         dy = (a7.y * b.r + b.y * a7.r) / ab7;
     return dx * dx + dy * dy;
 }
 
-function Node3(circle3) {
+function Node2(circle3) {
     this._ = circle3;
     this.next = null;
     this.previous = null;
 }
 
 function packSiblingsRandom(circles, random) {
     if (!(n = (circles = array_default2(circles)).length))
@@ -15646,21 +15647,21 @@
     a7 = circles[0], a7.x = 0, a7.y = 0;
     if (!(n > 1))
         return a7.r;
     b = circles[1], a7.x = -b.r, b.x = a7.r, b.y = 0;
     if (!(n > 2))
         return a7.r + b.r;
     place(b, a7, c11 = circles[2]);
-    a7 = new Node3(a7), b = new Node3(b), c11 = new Node3(c11);
+    a7 = new Node2(a7), b = new Node2(b), c11 = new Node2(c11);
     a7.next = c11.previous = b;
     b.next = a7.previous = c11;
     c11.next = b.previous = a7;
     pack:
         for (i = 3; i < n; ++i) {
-            place(a7._, b._, c11 = circles[i]), c11 = new Node3(c11);
+            place(a7._, b._, c11 = circles[i]), c11 = new Node2(c11);
             j = b.next, k3 = a7.previous, sj = b._.r, sk = a7._.r;
             do {
                 if (sj <= sk) {
                     if (intersects(j._, c11._)) {
                         b = j, a7.next = b, b.previous = a7, --i;
                         continue pack;
                     }
@@ -15872,15 +15873,15 @@
                     nodes.push(imputed);
                 }
             }
             currentId = (_, i2) => I[i2];
             currentParentId = (_, i2) => P[i2];
         }
         for (i = 0, n = nodes.length; i < n; ++i) {
-            d = nodes[i], node = nodes[i] = new Node2(d);
+            d = nodes[i], node = nodes[i] = new Node(d);
             if ((nodeId = currentId(d, i, data)) != null && (nodeId += "")) {
                 nodeKey = node.id = nodeId;
                 nodeByKey.set(nodeKey, nodeByKey.has(nodeKey) ? ambiguous : node);
             }
             if ((nodeId = currentParentId(d, i, data)) != null && (nodeId += "")) {
                 node.parent = nodeId;
             }
@@ -16019,15 +16020,15 @@
     this.z = 0;
     this.m = 0;
     this.c = 0;
     this.s = 0;
     this.t = null;
     this.i = i;
 }
-TreeNode.prototype = Object.create(Node2.prototype);
+TreeNode.prototype = Object.create(Node.prototype);
 
 function treeRoot(root5) {
     var tree3 = new TreeNode(root5, 0),
         node, nodes = [tree3],
         child, children3, i, n;
     while (node = nodes.pop()) {
         if (children3 = node._.children) {
@@ -22160,15 +22161,17 @@
     return type3 === void 0 ? arrayify2(data) : data instanceof type3 ? data : type3.prototype instanceof TypedArray && !(data instanceof TypedArray) ? type3.from(data, coerceNumber) : type3.from(data);
 }
 
 function floater(f) {
     return (d, i) => coerceNumber(f(d, i));
 }
 var field = (name) => (d) => d[name];
-var indexOf = (d, i) => i;
+var indexOf = {
+    transform: range4
+};
 var identity6 = {
     transform: (d) => d
 };
 var one2 = () => 1;
 var yes = () => true;
 var string = (x7) => x7 == null ? x7 : `${x7}`;
 var number5 = (x7) => x7 == null ? x7 : +x7;
@@ -22338,20 +22341,27 @@
     };
 }
 
 function maybeInterval(interval3, type3) {
     if (interval3 == null)
         return;
     if (typeof interval3 === "number") {
-        const n = interval3;
-        return {
-            floor: (d) => n * Math.floor(d / n),
+        if (0 < interval3 && interval3 < 1 && Number.isInteger(1 / interval3))
+            interval3 = -1 / interval3;
+        const n = Math.abs(interval3);
+        return interval3 < 0 ? {
+            floor: (d) => Math.floor(d * n) / n,
+            offset: (d) => (d * n + 1) / n,
+            // note: no optional step for simplicity
+            range: (lo, hi) => range(Math.ceil(lo * n), hi * n).map((x7) => x7 / n)
+        } : {
+            floor: (d) => Math.floor(d / n) * n,
             offset: (d) => d + n,
             // note: no optional step for simplicity
-            range: (lo, hi) => range(Math.ceil(lo / n), hi / n).map((x7) => n * x7)
+            range: (lo, hi) => range(Math.ceil(lo / n), hi / n).map((x7) => x7 * n)
         };
     }
     if (typeof interval3 === "string")
         return (type3 === "time" ? maybeTimeInterval : maybeUtcInterval)(interval3);
     if (typeof interval3.floor !== "function")
         throw new Error("invalid interval; missing floor method");
     if (typeof interval3.offset !== "function")
@@ -23712,43 +23722,44 @@
 }
 
 function applyPosition(channels, scales, context) {
     const {
         x: x7,
         y: y7
     } = channels;
-    let position3 = {};
+    let position5 = {};
     if (x7)
-        position3.x = x7;
+        position5.x = x7;
     if (y7)
-        position3.y = y7;
-    position3 = valueObject(position3, scales);
+        position5.y = y7;
+    position5 = valueObject(position5, scales);
     if (context.projection)
-        maybeProject("x", "y", channels, position3, context);
+        maybeProject("x", "y", channels, position5, context);
     if (x7)
-        position3.x = coerceNumbers(position3.x);
+        position5.x = coerceNumbers(position5.x);
     if (y7)
-        position3.y = coerceNumbers(position3.y);
-    return position3;
+        position5.y = coerceNumbers(position5.y);
+    return position5;
 }
 
 function hasGeometry(marks3) {
     for (const mark of marks3)
         if (mark.channels.geometry)
             return true;
     return false;
 }
 
 // node_modules/@observablehq/plot/src/context.js
-function createContext(options = {}, dimensions) {
+function createContext(options = {}, dimensions, className) {
     const {
         document: document2 = typeof window !== "undefined" ? window.document : void 0
     } = options;
     return {
         document: document2,
+        className,
         projection: createProjection(options, dimensions)
     };
 }
 
 function create2(name, {
     document: document2
 }) {
@@ -25272,15 +25283,15 @@
 function formatAuto(locale5 = "en-US") {
     const number14 = formatNumber(locale5);
     return (v3) => (v3 instanceof Date ? formatIsoDate : typeof v3 === "number" ? number14 : string)(v3);
 }
 var formatDefault = formatAuto();
 
 // node_modules/@observablehq/plot/src/style.js
-var offset = typeof window !== "undefined" && window.devicePixelRatio > 1 ? 0 : 0.5;
+var offset = (typeof window !== "undefined" ? window.devicePixelRatio > 1 : typeof it === "undefined") ? 0 : 0.5;
 var nextClipId = 0;
 
 function getClipId() {
     return `plot-clip-${++nextClipId}`;
 }
 
 function styles(mark, {
@@ -25522,22 +25533,22 @@
         warn(
             `Warning: the implicit z channel has high cardinality. This may occur when the fill or stroke channel is associated with quantitative data rather than ordinal or categorical data. You can suppress this warning by setting the z option explicitly; if this data represents a single series, set z to null.`
         );
     }
     return G.values();
 }
 
-function* groupIndex(I, position3, {
+function* groupIndex(I, position5, {
     z
 }, channels) {
     const {
         z: Z
     } = channels;
     const A6 = groupAesthetics(channels);
-    const C4 = [...position3, ...A6];
+    const C4 = [...position5, ...A6];
     for (const G of Z ? groupZ2(I, Z, z) : [I]) {
         let Ag;
         let Gg;
         out:
             for (const i of G) {
                 for (const c11 of C4) {
                     if (!defined(c11[i])) {
@@ -25686,15 +25697,15 @@
     if ((value = number5(value)) !== impliedValue)
         return value;
 }
 var validClassName = /^-?([_a-z]|[\240-\377]|\\[0-9a-f]{1,6}(\r\n|[ \t\r\n\f])?|\\[^\r\n\f0-9a-f])([_a-z0-9-]|[\240-\377]|\\[0-9a-f]{1,6}(\r\n|[ \t\r\n\f])?|\\[^\r\n\f0-9a-f])*$/i;
 
 function maybeClassName(name) {
     if (name === void 0)
-        return `plot-${Math.random().toString(16).slice(2)}`;
+        return "plot-d6a7b5";
     name = `${name}`;
     if (!validClassName.test(name))
         throw new Error(`invalid class name: ${name}`);
     return name;
 }
 
 function applyInlineStyles(selection3, style) {
@@ -25884,21 +25895,25 @@
         i
     })) : fyDomain ? fyDomain.map((y7, i) => ({
         y: y7,
         i
     })) : void 0;
 }
 
-function facetOrder({
+function recreateFacets(facets, {
     x: X4,
     y: Y4
 }) {
-    const xi = X4 && new Map(X4.map((v3, i) => [v3, i]));
-    const yi = Y4 && new Map(Y4.map((v3, i) => [v3, i]));
-    return X4 && Y4 ? (a7, b) => xi.get(a7.x) - xi.get(b.x) || yi.get(a7.y) - yi.get(b.y) : X4 ? (a7, b) => xi.get(a7.x) - xi.get(b.x) : (a7, b) => yi.get(a7.y) - yi.get(b.y);
+    X4 &&= new InternMap(X4.map((x7, i) => [x7, i]));
+    Y4 &&= new InternMap(Y4.map((y7, i) => [y7, i]));
+    return facets.filter(
+        X4 && Y4 ? (f) => X4.has(f.x) && Y4.has(f.y) : X4 ? (f) => X4.has(f.x) : (f) => Y4.has(f.y)
+    ).sort(
+        X4 && Y4 ? (a7, b) => X4.get(a7.x) - X4.get(b.x) || Y4.get(a7.y) - Y4.get(b.y) : X4 ? (a7, b) => X4.get(a7.x) - X4.get(b.x) : (a7, b) => Y4.get(a7.y) - Y4.get(b.y)
+    );
 }
 
 function facetGroups(data, {
     fx,
     fy
 }) {
     const I = range4(data);
@@ -26128,28 +26143,31 @@
             className
     } = options;
     const context = createContext(options);
     className = maybeClassName(className);
     opacity3 = maybeNumberChannel(opacity3)[1];
     if (tickFormat3 === null)
         tickFormat3 = () => null;
-    const svg3 = create2("svg", context).attr("class", className).attr("font-family", "system-ui, sans-serif").attr("font-size", 10).attr("width", width).attr("height", height).attr("viewBox", `0 0 ${width} ${height}`).call(
-        (svg4) => svg4.append("style").text(`
-        .${className} {
-          display: block;
-          background: white;
-          height: auto;
-          height: intrinsic;
-          max-width: 100%;
-          overflow: visible;
-        }
-        .${className} text {
-          white-space: pre;
-        }
-      `)
+    const svg3 = create2("svg", context).attr("class", `${className}-ramp`).attr("font-family", "system-ui, sans-serif").attr("font-size", 10).attr("width", width).attr("height", height).attr("viewBox", `0 0 ${width} ${height}`).call(
+        (svg4) => (
+            // Warning: if you edit this, change defaultClassName.
+            svg4.append("style").text(
+                `.${className}-ramp {
+  display: block;
+  background: white;
+  height: auto;
+  height: intrinsic;
+  max-width: 100%;
+  overflow: visible;
+}
+.${className}-ramp text {
+  white-space: pre;
+}`
+            )
+        )
     ).call(applyInlineStyles, style);
     let tickAdjust = (g) => g.selectAll(".tick line").attr("y1", marginTop + marginBottom - height);
     let x7;
     const applyRange = round3 ? (x8, range10) => x8.rangeRound(range10) : (x8, range10) => x8.range(range10);
     const {
         type: type3,
         domain,
@@ -26213,20 +26231,15 @@
     ...options
 } = {}) {
     if (!isOrdinalScale(color5) && !isThresholdScale(color5))
         throw new Error(`swatches legend requires ordinal or threshold color scale (not ${color5.type})`);
     return legendItems(
         color5,
         options,
-        (selection3, scale5) => selection3.append("svg").attr("fill", scale5.scale).attr("fill-opacity", maybeNumberChannel(opacity3)[1]).append("rect").attr("width", "100%").attr("height", "100%"),
-        (className) => `.${className}-swatch svg {
-        width: var(--swatchWidth);
-        height: var(--swatchHeight);
-        margin-right: 0.5em;
-      }`
+        (selection3, scale5, width, height) => selection3.append("svg").attr("width", width).attr("height", height).attr("fill", scale5.scale).attr("fill-opacity", maybeNumberChannel(opacity3)[1]).append("rect").attr("width", "100%").attr("height", "100%")
     );
 }
 
 function legendSymbols(symbol3, {
     fill = symbol3.hint?.fill !== void 0 ? symbol3.hint.fill : "none",
     fillOpacity = 1,
     stroke = symbol3.hint?.stroke !== void 0 ? symbol3.hint.stroke : isNoneish(fill) ? "currentColor" : "none",
@@ -26242,34 +26255,23 @@
     const size = r * r * Math.PI;
     fillOpacity = maybeNumberChannel(fillOpacity)[1];
     strokeOpacity = maybeNumberChannel(strokeOpacity)[1];
     strokeWidth = maybeNumberChannel(strokeWidth)[1];
     return legendItems(
         symbol3,
         options,
-        (selection3) => selection3.append("svg").attr("viewBox", "-8 -8 16 16").attr("fill", vf === "color" ? (d) => sf.scale(d) : null).attr("stroke", vs === "color" ? (d) => ss.scale(d) : null).append("path").attr("d", (d) => {
+        (selection3, scale6, width, height) => selection3.append("svg").attr("viewBox", "-8 -8 16 16").attr("width", width).attr("height", height).attr("fill", vf === "color" ? (d) => sf.scale(d) : cf).attr("fill-opacity", fillOpacity).attr("stroke", vs === "color" ? (d) => ss.scale(d) : cs).attr("stroke-opacity", strokeOpacity).attr("stroke-width", strokeWidth).append("path").attr("d", (d) => {
             const p = pathRound();
             symbol3.scale(d).draw(p, size);
             return p;
-        }),
-        (className) => `.${className}-swatch > svg {
-        width: var(--swatchWidth);
-        height: var(--swatchHeight);
-        margin-right: 0.5em;
-        overflow: visible;
-        fill: ${cf};
-        fill-opacity: ${fillOpacity};
-        stroke: ${cs};
-        stroke-width: ${strokeWidth}px;
-        stroke-opacity: ${strokeOpacity};
-      }`
+        })
     );
 }
 
-function legendItems(scale5, options = {}, swatch, swatchStyle) {
+function legendItems(scale5, options = {}, swatch) {
     let {
         columns,
         tickFormat: tickFormat3,
         fontVariant = inferFontVariant(scale5),
         // TODO label,
         swatchSize = 15,
         swatchWidth = swatchSize,
@@ -26278,73 +26280,67 @@
         className,
         style,
         width
     } = options;
     const context = createContext(options);
     className = maybeClassName(className);
     tickFormat3 = maybeAutoTickFormat(tickFormat3, scale5.domain);
-    const swatches = create2("div", context).attr("class", className).attr(
-        "style",
-        `
-        --swatchWidth: ${+swatchWidth}px;
-        --swatchHeight: ${+swatchHeight}px;
-      `
+    const swatches = create2("div", context).attr(
+        "class",
+        `${className}-swatches ${className}-swatches-${columns != null ? "columns" : "wrap"}`
     );
     let extraStyle;
     if (columns != null) {
-        extraStyle = `
-      .${className}-swatch {
-        display: flex;
-        align-items: center;
-        break-inside: avoid;
-        padding-bottom: 1px;
-      }
-      .${className}-swatch::before {
-        flex-shrink: 0;
-      }
-      .${className}-label {
-        white-space: nowrap;
-        overflow: hidden;
-        text-overflow: ellipsis;
-      }
-    `;
-        swatches.style("columns", columns).selectAll().data(scale5.domain).enter().append("div").attr("class", `${className}-swatch`).call(swatch, scale5).call(
-            (item) => item.append("div").attr("class", `${className}-label`).attr("title", tickFormat3).text(tickFormat3)
+        extraStyle = `.${className}-swatches-columns .${className}-swatch {
+  display: flex;
+  align-items: center;
+  break-inside: avoid;
+  padding-bottom: 1px;
+}
+.${className}-swatches-columns .${className}-swatch::before {
+  flex-shrink: 0;
+}
+.${className}-swatches-columns .${className}-swatch-label {
+  white-space: nowrap;
+  overflow: hidden;
+  text-overflow: ellipsis;
+}`;
+        swatches.style("columns", columns).selectAll().data(scale5.domain).enter().append("div").attr("class", `${className}-swatch`).call(swatch, scale5, swatchWidth, swatchHeight).call(
+            (item) => item.append("div").attr("class", `${className}-swatch-label`).attr("title", tickFormat3).text(tickFormat3)
         );
     } else {
-        extraStyle = `
-      .${className} {
-        display: flex;
-        align-items: center;
-        min-height: 33px;
-        flex-wrap: wrap;
-      }
-      .${className}-swatch {
-        display: inline-flex;
-        align-items: center;
-        margin-right: 1em;
-      }
-    `;
-        swatches.selectAll().data(scale5.domain).enter().append("span").attr("class", `${className}-swatch`).call(swatch, scale5).append(function() {
+        extraStyle = `.${className}-swatches-wrap {
+  display: flex;
+  align-items: center;
+  min-height: 33px;
+  flex-wrap: wrap;
+}
+.${className}-swatches-wrap .${className}-swatch {
+  display: inline-flex;
+  align-items: center;
+  margin-right: 1em;
+}`;
+        swatches.selectAll().data(scale5.domain).enter().append("span").attr("class", `${className}-swatch`).call(swatch, scale5, swatchWidth, swatchHeight).append(function() {
             return this.ownerDocument.createTextNode(tickFormat3.apply(this, arguments));
         });
     }
     return swatches.call(
-        (div) => div.insert("style", "*").text(`
-        .${className} {
-          font-family: system-ui, sans-serif;
-          font-size: 10px;
-          margin-bottom: 0.5em;${marginLeft === void 0 ? "" : `
-          margin-left: ${+marginLeft}px;`}${width === void 0 ? "" : `
-          width: ${width}px;`}
-        }
-        ${swatchStyle(className)}
-        ${extraStyle}
-      `)
-    ).style("font-variant", impliedString(fontVariant, "normal")).call(applyInlineStyles, style).node();
+        (div) => div.insert("style", "*").text(
+            `.${className}-swatches {
+  font-family: system-ui, sans-serif;
+  font-size: 10px;
+  margin-bottom: 0.5em;
+}
+.${className}-swatch > svg {
+  margin-right: 0.5em;
+  overflow: visible;
+}
+${extraStyle}`
+        )
+    ).style("margin-left", marginLeft ? `${+marginLeft}px` : null).style("width", width === void 0 ? null : `${+width}px`).style("font-variant", impliedString(fontVariant, "normal")).call(applyInlineStyles, style).node();
 }
 
 // node_modules/@observablehq/plot/src/legends.js
 var legendRegistry = /* @__PURE__ */ new Map([
     ["symbol", legendSymbols],
     ["color", legendColor],
     ["opacity", legendOpacity]
@@ -26382,20 +26378,26 @@
             throw new Error(`unknown legend type: ${key}`);
         if (!(key in scales))
             return;
         return legendRegistry.get(key)(scales[key], legendOptions(context, defaults41[key], options), (key2) => scales[key2]);
     };
 }
 
-function legendOptions(context, {
+function legendOptions({
+    className,
+    ...context
+}, {
     label,
     ticks: ticks3,
     tickFormat: tickFormat3
 } = {}, options) {
-    return inherit2(options, context, {
+    return inherit2(options, {
+        className,
+        ...context
+    }, {
         label,
         ticks: ticks3,
         tickFormat: tickFormat3
     });
 }
 
 function legendColor(color5, {
@@ -27724,18 +27726,19 @@
     textStroke,
     textStrokeOpacity,
     textStrokeWidth,
     tickSize = k3 === "y" ? 6 : 0,
     tickPadding,
     tickRotate,
     x: x7,
-    marginTop = 20,
-    marginRight = anchor === "right" ? 40 : 0,
-    marginBottom = 20,
-    marginLeft = anchor === "left" ? 40 : 0,
+    margin,
+    marginTop = margin === void 0 ? 20 : margin,
+    marginRight = margin === void 0 ? anchor === "right" ? 40 : 0 : margin,
+    marginBottom = margin === void 0 ? 20 : margin,
+    marginLeft = margin === void 0 ? anchor === "left" ? 40 : 0 : margin,
     label,
     labelOffset,
     labelAnchor,
     ...options
 }) {
     tickSize = number5(tickSize);
     tickPadding = number5(tickPadding);
@@ -27766,24 +27769,21 @@
             x: x7,
             marginTop,
             marginRight,
             marginBottom,
             marginLeft,
             ...options
         }) : null,
-        !isNoneish(fill) && label !== null ? text([], {
-            fill,
-            fillOpacity,
-            ...options,
-            lineWidth: void 0,
-            textOverflow: void 0,
-            facet: "super",
-            x: null,
-            y: null,
-            initializer: function(data2, facets, channels, scales, dimensions) {
+        !isNoneish(fill) && label !== null ? text(
+            [],
+            labelOptions({
+                fill,
+                fillOpacity,
+                ...options
+            }, function(data2, facets, channels, scales, dimensions) {
                 const scale5 = scales[k3];
                 const {
                     marginTop: marginTop2,
                     marginRight: marginRight2,
                     marginBottom: marginBottom2,
                     marginLeft: marginLeft2
                 } = k3 === "y" && dimensions.inset || dimensions;
@@ -27809,16 +27809,16 @@
                     ],
                     channels: {
                         text: {
                             value: [label === void 0 ? inferAxisLabel(k3, scale5, cla) : label]
                         }
                     }
                 };
-            }
-        }) : null
+            })
+        ) : null
     );
 }
 
 function axisKx(k3, anchor, data, {
     color: color5 = "currentColor",
     opacity: opacity3 = 1,
     stroke = color5,
@@ -27830,18 +27830,19 @@
     textStroke,
     textStrokeOpacity,
     textStrokeWidth,
     tickSize = k3 === "x" ? 6 : 0,
     tickPadding,
     tickRotate,
     y: y7,
-    marginTop = anchor === "top" ? 30 : 0,
-    marginRight = 20,
-    marginBottom = anchor === "bottom" ? 30 : 0,
-    marginLeft = 20,
+    margin,
+    marginTop = margin === void 0 ? anchor === "top" ? 30 : 0 : margin,
+    marginRight = margin === void 0 ? 20 : margin,
+    marginBottom = margin === void 0 ? anchor === "bottom" ? 30 : 0 : margin,
+    marginLeft = margin === void 0 ? 20 : margin,
     label,
     labelAnchor,
     labelOffset,
     ...options
 }) {
     tickSize = number5(tickSize);
     tickPadding = number5(tickPadding);
@@ -27872,24 +27873,21 @@
             y: y7,
             marginTop,
             marginRight,
             marginBottom,
             marginLeft,
             ...options
         }) : null,
-        !isNoneish(fill) && label !== null ? text([], {
-            fill,
-            fillOpacity,
-            ...options,
-            lineWidth: void 0,
-            textOverflow: void 0,
-            facet: "super",
-            x: null,
-            y: null,
-            initializer: function(data2, facets, channels, scales, dimensions) {
+        !isNoneish(fill) && label !== null ? text(
+            [],
+            labelOptions({
+                fill,
+                fillOpacity,
+                ...options
+            }, function(data2, facets, channels, scales, dimensions) {
                 const scale5 = scales[k3];
                 const {
                     marginTop: marginTop2,
                     marginRight: marginRight2,
                     marginBottom: marginBottom2,
                     marginLeft: marginLeft2
                 } = k3 === "x" && dimensions.inset || dimensions;
@@ -27912,16 +27910,16 @@
                     ],
                     channels: {
                         text: {
                             value: [label === void 0 ? inferAxisLabel(k3, scale5, cla) : label]
                         }
                     }
                 };
-            }
-        }) : null
+            })
+        ) : null
     );
 }
 
 function axisTickKy(k3, anchor, data, {
     strokeWidth = 1,
     strokeLinecap = null,
     strokeLinejoin = null,
@@ -28127,14 +28125,44 @@
         stroke,
         strokeOpacity,
         strokeWidth,
         ...options
     };
 }
 
+function labelOptions({
+    fill,
+    fillOpacity,
+    fontFamily,
+    fontSize,
+    fontStyle,
+    fontWeight,
+    monospace,
+    pointerEvents,
+    shapeRendering
+}, initializer3) {
+    [, fill] = maybeColorChannel(fill);
+    [, fillOpacity] = maybeNumberChannel(fillOpacity);
+    return {
+        facet: "super",
+        x: null,
+        y: null,
+        fill,
+        fillOpacity,
+        fontFamily,
+        fontSize,
+        fontStyle,
+        fontWeight,
+        monospace,
+        pointerEvents,
+        shapeRendering,
+        initializer: initializer3
+    };
+}
+
 function axisMark(mark, k3, ariaLabel, data, options, initialize) {
     let channels;
     const m5 = mark(
         data,
         initializer(options, function(data2, facets, _channels, scales) {
             const {
                 [k3]: scale5
@@ -28341,15 +28369,15 @@
     const axes = flatMarks(inferAxes(marks3, channelsByScale, options));
     for (const mark of axes) {
         const facetState = maybeMarkFacet(mark, topFacetState, options);
         if (facetState)
             facetStateByMark.set(mark, facetState);
     }
     marks3.unshift(...axes);
-    const facets = createFacets(channelsByScale, options);
+    let facets = createFacets(channelsByScale, options);
     if (facets !== void 0) {
         const topFacetsIndex = topFacetState ? facetFilter(facets, topFacetState) : void 0;
         for (const mark of marks3) {
             if (mark.facet === null || mark.facet === "super")
                 continue;
             const facetState = facetStateByMark.get(mark);
             if (facetState === void 0)
@@ -28409,15 +28437,15 @@
     autoScaleRange(scaleDescriptors, dimensions);
     const {
         fx,
         fy
     } = scales;
     const subdimensions = fx || fy ? innerDimensions(scaleDescriptors, dimensions) : dimensions;
     const superdimensions = fx || fy ? actualDimensions(scales, dimensions) : dimensions;
-    const context = createContext(options, subdimensions, scaleDescriptors);
+    const context = createContext(options, subdimensions, className);
     const newByScale = /* @__PURE__ */ new Set();
     for (const [mark, state] of stateByMark) {
         if (mark.initializer != null) {
             const dimensions2 = mark.facet === "super" ? superdimensions : subdimensions;
             const update = mark.initializer(state.data, state.facets, state.channels, scales, dimensions2, context);
             if (update.data !== void 0) {
                 state.data = update.data;
@@ -28469,34 +28497,37 @@
         state.values = mark.scale(state.channels, scales, context);
     }
     const {
         width,
         height
     } = dimensions;
     const svg3 = create2("svg", context).attr("class", className).attr("fill", "currentColor").attr("font-family", "system-ui, sans-serif").attr("font-size", 10).attr("text-anchor", "middle").attr("width", width).attr("height", height).attr("viewBox", `0 0 ${width} ${height}`).attr("aria-label", ariaLabel).attr("aria-description", ariaDescription).call(
-        (svg4) => svg4.append("style").text(`
-        .${className} {
-          display: block;
-          background: white;
-          height: auto;
-          height: intrinsic;
-          max-width: 100%;
-        }
-        .${className} text,
-        .${className} tspan {
-          white-space: pre;
-        }
-      `)
+        (svg4) => (
+            // Warning: if you edit this, change defaultClassName.
+            svg4.append("style").text(
+                `.${className} {
+  display: block;
+  background: white;
+  height: auto;
+  height: intrinsic;
+  max-width: 100%;
+}
+.${className} text,
+.${className} tspan {
+  white-space: pre;
+}`
+            )
+        )
     ).call(applyInlineStyles, style).node();
     if (facets !== void 0) {
         const facetDomains = {
             x: fx?.domain(),
             y: fy?.domain()
         };
-        facets.sort(facetOrder(facetDomains));
+        facets = recreateFacets(facets, facetDomains);
         select_default2(svg3).selectAll().data(facets).enter().append("g").attr("aria-label", "facet").attr("transform", facetTranslate(fx, fy, dimensions)).each(function(f) {
             let empty7 = true;
             for (const mark of marks3) {
                 if (mark.facet === "super")
                     continue;
                 const {
                     channels,
@@ -28551,15 +28582,15 @@
         figure = document2.createElement("figure");
         figure.style.maxWidth = "initial";
         for (const legend3 of legends)
             figure.appendChild(legend3);
         figure.appendChild(svg3);
         if (caption != null) {
             const figcaption = document2.createElement("figcaption");
-            figcaption.appendChild(caption instanceof Node ? caption : document2.createTextNode(caption));
+            figcaption.appendChild(caption?.ownerDocument ? caption : document2.createTextNode(caption));
             figure.appendChild(figcaption);
         }
     }
     figure.scale = exposeScales(scaleDescriptors);
     figure.legend = exposeLegends(scaleDescriptors, context, options);
     const w = consumeWarnings();
     if (w > 0) {
@@ -28716,15 +28747,15 @@
         data
     } = topFacetState;
     if (mark.facet !== "auto" || mark.data === data)
         return {
             channels,
             groups: groups3
         };
-    if ((groups3.size > 1 || groups3.size === 1 && channels.fx && channels.fy && [...groups3][0][1].size > 1) && arrayify2(mark.data)?.length === data.length) {
+    if (data.length > 0 && (groups3.size > 1 || groups3.size === 1 && channels.fx && channels.fy && [...groups3][0][1].size > 1) && arrayify2(mark.data)?.length === data.length) {
         warn(
             `Warning: the ${mark.ariaLabel} mark appears to use faceted data, but isn\u2019t faceted. The mark data has the same length as the facet data and the mark facet option is "auto", but the mark data and facet data are distinct. If this mark should be faceted, set the mark facet option to true; otherwise, suppress this warning by setting the mark facet option to false.`
         );
     }
 }
 
 function inferAxes(marks3, channelsByScale, options) {
@@ -32864,15 +32895,15 @@
                 const j = halfedges[i2];
                 if (j > i2)
                     link7(triangles[i2], triangles[j]);
             }
             for (let i2 = 0; i2 < hull3.length; ++i2) {
                 link7(hull3[i2], hull3[(i2 + 1) % hull3.length]);
             }
-            select_default2(this).selectAll().data(newIndex).join("path").call(applyDirectStyles, mark).attr("d", (i2) => {
+            select_default2(this).selectAll().data(newIndex).enter().append("path").call(applyDirectStyles, mark).attr("d", (i2) => {
                 const p = pathRound();
                 const c11 = curve(p);
                 c11.lineStart();
                 c11.point(X15[i2], Y15[i2]);
                 c11.point(X25[i2], Y25[i2]);
                 c11.lineEnd();
                 return p;
@@ -33131,15 +33162,15 @@
         return index5;
     }
     render(index5, scales, channels, dimensions, context) {
         const {
             contours
         } = channels;
         const path3 = path_default();
-        return create_default("svg:g", context).call(applyIndirectStyles, this, dimensions, context).call(applyTransform, this, {}).call(
+        return create2("svg:g", context).call(applyIndirectStyles, this, dimensions, context).call(applyTransform, this, {}).call(
             (g) => g.selectAll().data(index5).enter().append("path").call(applyDirectStyles, this).call(applyChannelStyles, this, channels).attr("d", (i) => path3(contours[i]))
         ).node();
     }
 };
 
 function density(data, options = {}) {
     let {
@@ -33625,62 +33656,82 @@
     return typeof value === "string" && (isPath(value) || isUrl(value)) ? [void 0, value] : [value, void 0];
 }
 var Image2 = class extends Mark {
     constructor(data, options = {}) {
         let {
             x: x7,
             y: y7,
+            r,
             width,
             height,
+            rotate,
             src,
             preserveAspectRatio,
             crossOrigin,
             frameAnchor,
             imageRendering
         } = options;
-        if (width === void 0 && height !== void 0)
+        if (r == null)
+            r = void 0;
+        if (r === void 0 && width === void 0 && height === void 0)
+            width = height = 16;
+        else if (width === void 0 && height !== void 0)
             width = height;
         else if (height === void 0 && width !== void 0)
             height = width;
         const [vs, cs] = maybePathChannel(src);
-        const [vw, cw] = maybeNumberChannel(width, 16);
-        const [vh, ch] = maybeNumberChannel(height, 16);
+        const [vr, cr] = maybeNumberChannel(r);
+        const [vw, cw] = maybeNumberChannel(width, cr !== void 0 ? cr * 2 : void 0);
+        const [vh, ch] = maybeNumberChannel(height, cr !== void 0 ? cr * 2 : void 0);
+        const [va, ca5] = maybeNumberChannel(rotate, 0);
         super(
             data, {
                 x: {
                     value: x7,
                     scale: "x",
                     optional: true
                 },
                 y: {
                     value: y7,
                     scale: "y",
                     optional: true
                 },
+                r: {
+                    value: vr,
+                    scale: "r",
+                    filter: positive,
+                    optional: true
+                },
                 width: {
                     value: vw,
                     filter: positive,
                     optional: true
                 },
                 height: {
                     value: vh,
                     filter: positive,
                     optional: true
                 },
+                rotate: {
+                    value: va,
+                    optional: true
+                },
                 src: {
                     value: vs,
                     optional: true
                 }
             },
-            options,
+            withDefaultSort(options),
             defaults19
         );
         this.src = cs;
         this.width = cw;
+        this.rotate = ca5;
         this.height = ch;
+        this.r = cr;
         this.preserveAspectRatio = impliedString(preserveAspectRatio, "xMidYMid");
         this.crossOrigin = string(crossOrigin);
         this.frameAnchor = maybeFrameAnchor(frameAnchor);
         this.imageRendering = impliedString(imageRendering, "auto");
     }
     render(index5, scales, channels, dimensions, context) {
         const {
@@ -33688,32 +33739,38 @@
             y: y7
         } = scales;
         const {
             x: X4,
             y: Y4,
             width: W,
             height: H,
+            r: R,
+            rotate: A6,
             src: S
         } = channels;
+        const {
+            r,
+            width,
+            height,
+            rotate
+        } = this;
         const [cx, cy] = applyFrameAnchor(this, dimensions);
         return create2("svg:g", context).call(applyIndirectStyles, this, dimensions, context).call(applyTransform, this, {
             x: X4 && x7,
             y: Y4 && y7
         }).call(
-            (g) => g.selectAll().data(index5).enter().append("image").call(applyDirectStyles, this).attr(
-                "x",
-                W && X4 ? (i) => X4[i] - W[i] / 2 : W ? (i) => cx - W[i] / 2 : X4 ? (i) => X4[i] - this.width / 2 : cx - this.width / 2
-            ).attr(
-                "y",
-                H && Y4 ? (i) => Y4[i] - H[i] / 2 : H ? (i) => cy - H[i] / 2 : Y4 ? (i) => Y4[i] - this.height / 2 : cy - this.height / 2
-            ).attr("width", W ? (i) => W[i] : this.width).attr("height", H ? (i) => H[i] : this.height).call(applyAttr, "href", S ? (i) => S[i] : this.src).call(applyAttr, "preserveAspectRatio", this.preserveAspectRatio).call(applyAttr, "crossorigin", this.crossOrigin).call(applyAttr, "image-rendering", this.imageRendering).call(applyChannelStyles, this, channels)
+            (g) => g.selectAll().data(index5).enter().append("image").call(applyDirectStyles, this).attr("x", position2(X4, W, R, cx, width, r)).attr("y", position2(Y4, H, R, cy, height, r)).attr("width", W ? (i) => W[i] : width !== void 0 ? width : R ? (i) => R[i] * 2 : r * 2).attr("height", H ? (i) => H[i] : height !== void 0 ? height : R ? (i) => R[i] * 2 : r * 2).attr("transform", A6 ? (i) => `rotate(${A6[i]})` : rotate ? `rotate(${rotate})` : null).attr("transform-origin", A6 || rotate ? template`${X4 ? (i) => X4[i] : cx}px ${Y4 ? (i) => Y4[i] : cy}px` : null).call(applyAttr, "href", S ? (i) => S[i] : this.src).call(applyAttr, "preserveAspectRatio", this.preserveAspectRatio).call(applyAttr, "crossorigin", this.crossOrigin).call(applyAttr, "image-rendering", this.imageRendering).call(applyAttr, "clip-path", R ? (i) => `circle(${R[i]}px)` : r !== void 0 ? `circle(${r}px)` : null).call(applyChannelStyles, this, channels)
         ).node();
     }
 };
 
+function position2(X4, W, R, x7, w, r) {
+    return W && X4 ? (i) => X4[i] - W[i] / 2 : W ? (i) => x7 - W[i] / 2 : X4 && w !== void 0 ? (i) => X4[i] - w / 2 : w !== void 0 ? x7 - w / 2 : R && X4 ? (i) => X4[i] - R[i] : R ? (i) => x7 - R[i] : X4 ? (i) => X4[i] - r : x7 - r;
+}
+
 function image(data, options = {}) {
     let {
         x: x7,
         y: y7,
         ...remainingOptions
     } = options;
     if (options.frameAnchor === void 0)
@@ -34511,70 +34568,71 @@
     } : anchor;
 }
 
 function dodgeX(dodgeOptions = {}, options = {}) {
     if (arguments.length === 1)
         [dodgeOptions, options] = mergeOptions3(dodgeOptions);
     let {
-        anchor = "left", padding = 1
+        anchor = "left", padding = 1, r = options.r
     } = maybeAnchor2(dodgeOptions);
     switch (`${anchor}`.toLowerCase()) {
         case "left":
             anchor = anchorXLeft;
             break;
         case "right":
             anchor = anchorXRight;
             break;
         case "middle":
             anchor = anchorXMiddle;
             break;
         default:
             throw new Error(`unknown dodge anchor: ${anchor}`);
     }
-    return dodge("x", "y", anchor, number5(padding), options);
+    return dodge("x", "y", anchor, number5(padding), r, options);
 }
 
 function dodgeY(dodgeOptions = {}, options = {}) {
     if (arguments.length === 1)
         [dodgeOptions, options] = mergeOptions3(dodgeOptions);
     let {
-        anchor = "bottom", padding = 1
+        anchor = "bottom", padding = 1, r = options.r
     } = maybeAnchor2(dodgeOptions);
     switch (`${anchor}`.toLowerCase()) {
         case "top":
             anchor = anchorYTop;
             break;
         case "bottom":
             anchor = anchorYBottom;
             break;
         case "middle":
             anchor = anchorYMiddle;
             break;
         default:
             throw new Error(`unknown dodge anchor: ${anchor}`);
     }
-    return dodge("y", "x", anchor, number5(padding), options);
+    return dodge("y", "x", anchor, number5(padding), r, options);
 }
 
 function mergeOptions3(options) {
     const {
         anchor,
         padding,
         ...rest
     } = options;
+    const {
+        r
+    } = rest;
     return [{
         anchor,
-        padding
+        padding,
+        r
     }, rest];
 }
 
-function dodge(y7, x7, anchor, padding, options) {
-    const {
-        r
-    } = options;
+function dodge(y7, x7, anchor, padding, r, options) {
     if (r != null && typeof r !== "number") {
         const {
             channels,
             sort: sort5,
             reverse: reverse5
         } = options;
         options = {
@@ -34598,35 +34656,35 @@
             [x7]: X4, r: R
         } = channels;
         if (!channels[x7])
             throw new Error(`missing channel: ${x7}`);
         ({
             [x7]: X4
         } = applyPosition(channels, scales, context));
-        const r2 = R ? void 0 : this.r !== void 0 ? this.r : options.r !== void 0 ? number5(options.r) : 3;
+        const cr = R ? void 0 : r !== void 0 ? number5(r) : this.r !== void 0 ? this.r : 3;
         if (R)
             R = valueof(R.value, scales[R.scale] || identity6, Float64Array);
         let [ky3, ty] = anchor(dimensions);
         const compare = ky3 ? compareAscending : compareSymmetric;
         const Y4 = new Float64Array(X4.length);
-        const radius3 = R ? (i) => R[i] : () => r2;
+        const radius3 = R ? (i) => R[i] : () => cr;
         for (let I of facets) {
             const tree3 = (0, import_interval_tree_1d.default)();
             I = I.filter(R ? (i) => finite2(X4[i]) && positive(R[i]) : (i) => finite2(X4[i]));
             const intervals = new Float64Array(2 * I.length + 2);
             for (const i of I) {
                 const ri = radius3(i);
                 const y011 = ky3 ? ri + padding : 0;
                 const l = X4[i] - ri;
                 const h = X4[i] + ri;
                 let k3 = 2;
                 tree3.queryInterval(l - padding, h + padding, ([, , j]) => {
                     const yj = Y4[j] - y011;
                     const dx = X4[i] - X4[j];
-                    const dr = padding + (R ? R[i] + R[j] : 2 * r2);
+                    const dr = padding + (R ? R[i] + R[j] : 2 * cr);
                     const dy = Math.sqrt(dr * dr - dx * dx);
                     intervals[k3++] = yj - dy;
                     intervals[k3++] = yj + dy;
                 });
                 let candidates = intervals.slice(0, k3);
                 if (ky3)
                     candidates = candidates.filter((y8) => y8 >= 0);
@@ -35289,14 +35347,15 @@
     groupZ: () => groupZ3,
     hexagon: () => hexagon2,
     hexbin: () => hexbin2,
     hexgrid: () => hexgrid2,
     hull: () => hull2,
     identity: () => identity13,
     image: () => image2,
+    indexOf: () => indexOf2,
     initializer: () => initializer2,
     interpolateNearest: () => interpolateNearest2,
     interpolateNone: () => interpolateNone2,
     interpolatorBarycentric: () => interpolatorBarycentric2,
     interpolatorRandomWalk: () => interpolatorRandomWalk2,
     legend: () => legend2,
     line: () => line2,
@@ -35362,15 +35421,15 @@
 var src_exports3 = {};
 __export(src_exports3, {
     Adder: () => Adder2,
     Delaunay: () => Delaunay2,
     FormatSpecifier: () => FormatSpecifier2,
     InternMap: () => InternMap2,
     InternSet: () => InternSet2,
-    Node: () => Node4,
+    Node: () => Node3,
     Path: () => Path3,
     Voronoi: () => Voronoi3,
     ZoomTransform: () => Transform2,
     active: () => active_default2,
     arc: () => arc_default2,
     area: () => area_default10,
     areaRadial: () => areaRadial_default2,
@@ -37478,15 +37537,15 @@
     function axis3(context) {
         var values3 = tickValues == null ? scale5.ticks ? scale5.ticks.apply(scale5, tickArguments) : scale5.domain() : tickValues,
             format5 = tickFormat3 == null ? scale5.tickFormat ? scale5.tickFormat.apply(scale5, tickArguments) : identity_default6 : tickFormat3,
             spacing = Math.max(tickSizeInner, 0) + tickPadding,
             range9 = scale5.range(),
             range0 = +range9[0] + offset3,
             range1 = +range9[range9.length - 1] + offset3,
-            position3 = (scale5.bandwidth ? center2 : number8)(scale5.copy(), offset3),
+            position5 = (scale5.bandwidth ? center2 : number8)(scale5.copy(), offset3),
             selection3 = context.selection ? context.selection() : context,
             path3 = selection3.selectAll(".domain").data([null]),
             tick = selection3.selectAll(".tick").data(values3, scale5).order(),
             tickExit = tick.exit(),
             tickEnter = tick.enter().append("g").attr("class", "tick"),
             line3 = tick.select("line"),
             text3 = tick.select("text");
@@ -37496,31 +37555,31 @@
         text3 = text3.merge(tickEnter.append("text").attr("fill", "currentColor").attr(x7, k3 * spacing).attr("dy", orient === top2 ? "0em" : orient === bottom2 ? "0.71em" : "0.32em"));
         if (context !== selection3) {
             path3 = path3.transition(context);
             tick = tick.transition(context);
             line3 = line3.transition(context);
             text3 = text3.transition(context);
             tickExit = tickExit.transition(context).attr("opacity", epsilon9).attr("transform", function(d) {
-                return isFinite(d = position3(d)) ? transform3(d + offset3) : this.getAttribute("transform");
+                return isFinite(d = position5(d)) ? transform3(d + offset3) : this.getAttribute("transform");
             });
             tickEnter.attr("opacity", epsilon9).attr("transform", function(d) {
                 var p = this.parentNode.__axis;
-                return transform3((p && isFinite(p = p(d)) ? p : position3(d)) + offset3);
+                return transform3((p && isFinite(p = p(d)) ? p : position5(d)) + offset3);
             });
         }
         tickExit.remove();
         path3.attr("d", orient === left2 || orient === right2 ? tickSizeOuter ? "M" + k3 * tickSizeOuter + "," + range0 + "H" + offset3 + "V" + range1 + "H" + k3 * tickSizeOuter : "M" + offset3 + "," + range0 + "V" + range1 : tickSizeOuter ? "M" + range0 + "," + k3 * tickSizeOuter + "V" + offset3 + "H" + range1 + "V" + k3 * tickSizeOuter : "M" + range0 + "," + offset3 + "H" + range1);
         tick.attr("opacity", 1).attr("transform", function(d) {
-            return transform3(position3(d) + offset3);
+            return transform3(position5(d) + offset3);
         });
         line3.attr(x7 + "2", k3 * tickSizeInner);
         text3.attr(x7, k3 * spacing).text(format5);
         selection3.filter(entering2).attr("fill", "none").attr("font-size", 10).attr("font-family", "sans-serif").attr("text-anchor", orient === right2 ? "start" : orient === left2 ? "end" : "middle");
         selection3.each(function() {
-            this.__axis = position3;
+            this.__axis = position5;
         });
     }
     axis3.scale = function(_) {
         return arguments.length ? (scale5 = _, axis3) : scale5;
     };
     axis3.ticks = function() {
         return tickArguments = Array.from(arguments), axis3;
@@ -49566,22 +49625,22 @@
     if (data instanceof Map) {
         data = [void 0, data];
         if (children3 === void 0)
             children3 = mapChildren2;
     } else if (children3 === void 0) {
         children3 = objectChildren2;
     }
-    var root5 = new Node4(data),
+    var root5 = new Node3(data),
         node, nodes = [root5],
         child, childs, i, n;
     while (node = nodes.pop()) {
         if ((childs = children3(node.data)) && (n = (childs = Array.from(childs)).length)) {
             node.children = childs;
             for (i = n - 1; i >= 0; --i) {
-                nodes.push(child = childs[i] = new Node4(childs[i]));
+                nodes.push(child = childs[i] = new Node3(childs[i]));
                 child.parent = node;
                 child.depth = node.depth + 1;
             }
         }
     }
     return root5.eachBefore(computeHeight2);
 }
@@ -49607,21 +49666,21 @@
 function computeHeight2(node) {
     var height = 0;
     do
         node.height = height;
     while ((node = node.parent) && node.height < ++height);
 }
 
-function Node4(data) {
+function Node3(data) {
     this.data = data;
     this.depth = this.height = 0;
     this.parent = null;
 }
-Node4.prototype = hierarchy2.prototype = {
-    constructor: Node4,
+Node3.prototype = hierarchy2.prototype = {
+    constructor: Node3,
     count: count_default2,
     each: each_default4,
     eachAfter: eachAfter_default2,
     eachBefore: eachBefore_default2,
     find: find_default4,
     sum: sum_default2,
     sort: sort_default4,
@@ -49854,15 +49913,15 @@
         b = node.next._,
         ab7 = a7.r + b.r,
         dx = (a7.x * b.r + b.x * a7.r) / ab7,
         dy = (a7.y * b.r + b.y * a7.r) / ab7;
     return dx * dx + dy * dy;
 }
 
-function Node5(circle3) {
+function Node4(circle3) {
     this._ = circle3;
     this.next = null;
     this.previous = null;
 }
 
 function packSiblingsRandom2(circles, random) {
     if (!(n = (circles = array_default5(circles)).length))
@@ -49871,21 +49930,21 @@
     a7 = circles[0], a7.x = 0, a7.y = 0;
     if (!(n > 1))
         return a7.r;
     b = circles[1], a7.x = -b.r, b.x = a7.r, b.y = 0;
     if (!(n > 2))
         return a7.r + b.r;
     place2(b, a7, c11 = circles[2]);
-    a7 = new Node5(a7), b = new Node5(b), c11 = new Node5(c11);
+    a7 = new Node4(a7), b = new Node4(b), c11 = new Node4(c11);
     a7.next = c11.previous = b;
     b.next = a7.previous = c11;
     c11.next = b.previous = a7;
     pack:
         for (i = 3; i < n; ++i) {
-            place2(a7._, b._, c11 = circles[i]), c11 = new Node5(c11);
+            place2(a7._, b._, c11 = circles[i]), c11 = new Node4(c11);
             j = b.next, k3 = a7.previous, sj = b._.r, sk = a7._.r;
             do {
                 if (sj <= sk) {
                     if (intersects2(j._, c11._)) {
                         b = j, a7.next = b, b.previous = a7, --i;
                         continue pack;
                     }
@@ -50097,15 +50156,15 @@
                     nodes.push(imputed2);
                 }
             }
             currentId = (_, i2) => I[i2];
             currentParentId = (_, i2) => P[i2];
         }
         for (i = 0, n = nodes.length; i < n; ++i) {
-            d = nodes[i], node = nodes[i] = new Node4(d);
+            d = nodes[i], node = nodes[i] = new Node3(d);
             if ((nodeId = currentId(d, i, data)) != null && (nodeId += "")) {
                 nodeKey = node.id = nodeId;
                 nodeByKey.set(nodeKey, nodeByKey.has(nodeKey) ? ambiguous2 : node);
             }
             if ((nodeId = currentParentId(d, i, data)) != null && (nodeId += "")) {
                 node.parent = nodeId;
             }
@@ -50244,15 +50303,15 @@
     this.z = 0;
     this.m = 0;
     this.c = 0;
     this.s = 0;
     this.t = null;
     this.i = i;
 }
-TreeNode2.prototype = Object.create(Node4.prototype);
+TreeNode2.prototype = Object.create(Node3.prototype);
 
 function treeRoot2(root5) {
     var tree3 = new TreeNode2(root5, 0),
         node, nodes = [tree3],
         child, children3, i, n;
     while (node = nodes.pop()) {
         if (children3 = node._.children) {
@@ -56385,15 +56444,17 @@
     return type3 === void 0 ? arrayify4(data) : data instanceof type3 ? data : type3.prototype instanceof TypedArray2 && !(data instanceof TypedArray2) ? type3.from(data, coerceNumber2) : type3.from(data);
 }
 
 function floater2(f) {
     return (d, i) => coerceNumber2(f(d, i));
 }
 var field2 = (name) => (d) => d[name];
-var indexOf2 = (d, i) => i;
+var indexOf2 = {
+    transform: range8
+};
 var identity13 = {
     transform: (d) => d
 };
 var one4 = () => 1;
 var yes2 = () => true;
 var string2 = (x7) => x7 == null ? x7 : `${x7}`;
 var number11 = (x7) => x7 == null ? x7 : +x7;
@@ -56563,20 +56624,27 @@
     };
 }
 
 function maybeInterval2(interval3, type3) {
     if (interval3 == null)
         return;
     if (typeof interval3 === "number") {
-        const n = interval3;
-        return {
-            floor: (d) => n * Math.floor(d / n),
+        if (0 < interval3 && interval3 < 1 && Number.isInteger(1 / interval3))
+            interval3 = -1 / interval3;
+        const n = Math.abs(interval3);
+        return interval3 < 0 ? {
+            floor: (d) => Math.floor(d * n) / n,
+            offset: (d) => (d * n + 1) / n,
+            // note: no optional step for simplicity
+            range: (lo, hi) => range5(Math.ceil(lo * n), hi * n).map((x7) => x7 / n)
+        } : {
+            floor: (d) => Math.floor(d / n) * n,
             offset: (d) => d + n,
             // note: no optional step for simplicity
-            range: (lo, hi) => range5(Math.ceil(lo / n), hi / n).map((x7) => n * x7)
+            range: (lo, hi) => range5(Math.ceil(lo / n), hi / n).map((x7) => x7 * n)
         };
     }
     if (typeof interval3 === "string")
         return (type3 === "time" ? maybeTimeInterval2 : maybeUtcInterval2)(interval3);
     if (typeof interval3.floor !== "function")
         throw new Error("invalid interval; missing floor method");
     if (typeof interval3.offset !== "function")
@@ -56778,25 +56846,25 @@
 }
 
 function maybeNamed2(things) {
     return isIterable2(things) ? named4(things) : things;
 }
 
 // js/pyobsplot-js/node_modules/@observablehq/plot/src/scales/index.js
-var position2 = Symbol("position");
+var position3 = Symbol("position");
 var color4 = Symbol("color");
 var radius2 = Symbol("radius");
 var length6 = Symbol("length");
 var opacity2 = Symbol("opacity");
 var symbol2 = Symbol("symbol");
 var registry2 = /* @__PURE__ */ new Map([
-    ["x", position2],
-    ["y", position2],
-    ["fx", position2],
-    ["fy", position2],
+    ["x", position3],
+    ["y", position3],
+    ["fx", position3],
+    ["fy", position3],
     ["r", radius2],
     ["color", color4],
     ["opacity", opacity2],
     ["symbol", symbol2],
     ["length", length6]
 ]);
 
@@ -57937,43 +58005,44 @@
 }
 
 function applyPosition2(channels, scales, context) {
     const {
         x: x7,
         y: y7
     } = channels;
-    let position3 = {};
+    let position5 = {};
     if (x7)
-        position3.x = x7;
+        position5.x = x7;
     if (y7)
-        position3.y = y7;
-    position3 = valueObject2(position3, scales);
+        position5.y = y7;
+    position5 = valueObject2(position5, scales);
     if (context.projection)
-        maybeProject2("x", "y", channels, position3, context);
+        maybeProject2("x", "y", channels, position5, context);
     if (x7)
-        position3.x = coerceNumbers2(position3.x);
+        position5.x = coerceNumbers2(position5.x);
     if (y7)
-        position3.y = coerceNumbers2(position3.y);
-    return position3;
+        position5.y = coerceNumbers2(position5.y);
+    return position5;
 }
 
 function hasGeometry2(marks3) {
     for (const mark of marks3)
         if (mark.channels.geometry)
             return true;
     return false;
 }
 
 // js/pyobsplot-js/node_modules/@observablehq/plot/src/context.js
-function createContext2(options = {}, dimensions) {
+function createContext2(options = {}, dimensions, className) {
     const {
         document: document2 = typeof window !== "undefined" ? window.document : void 0
     } = options;
     return {
         document: document2,
+        className,
         projection: createProjection2(options, dimensions)
     };
 }
 
 function create4(name, {
     document: document2
 }) {
@@ -58781,15 +58850,15 @@
         for (const v3 of value)
             values3.add(v3);
     }
     if (interval3 !== void 0) {
         const [min7, max9] = extent3(values3).map(interval3.floor, interval3);
         return interval3.range(min7, interval3.offset(max9));
     }
-    if (values3.size > 1e4 && registry2.get(key) === position2) {
+    if (values3.size > 1e4 && registry2.get(key) === position3) {
         throw new Error(`implicit ordinal domain of ${key} scale has more than 10,000 values`);
     }
     return sort3(values3, ascendingDefined4);
 }
 
 function inferHint2(channels, key) {
     let value;
@@ -58839,15 +58908,15 @@
     } = {},
     ...options
 } = {}) {
     const scales = {};
     for (const [key, channels] of channelsByScale) {
         const scaleOptions = options[key];
         const scale5 = createScale2(key, channels, {
-            round: registry2.get(key) === position2 ? round3 : void 0,
+            round: registry2.get(key) === position3 ? round3 : void 0,
             // only for position
             nice: nice5,
             clamp,
             zero: zero5,
             align,
             padding,
             projection: projection3,
@@ -59128,15 +59197,15 @@
         case "pow":
         case "log":
         case "symlog":
             options = coerceType2(channels, options, coerceNumbers2);
             break;
         case "identity":
             switch (registry2.get(key)) {
-                case position2:
+                case position3:
                     options = coerceType2(channels, options, coerceNumbers2);
                     break;
                 case symbol2:
                     options = coerceType2(channels, options, coerceSymbols2);
                     break;
             }
             break;
@@ -59183,15 +59252,15 @@
         case "time":
             return createScaleTime2(key, channels, options);
         case "point":
             return createScalePoint2(key, channels, options);
         case "band":
             return createScaleBand2(key, channels, options);
         case "identity":
-            return registry2.get(key) === position2 ? createScaleIdentity2() : {
+            return registry2.get(key) === position3 ? createScaleIdentity2() : {
                 type: "identity"
             };
         case void 0:
             return;
         default:
             throw new Error(`unknown scale type: ${type3}`);
     }
@@ -59263,15 +59332,15 @@
     if (kind === color4 && (pivot != null || isDivergingScheme2(scheme55)))
         return "diverging";
     return "linear";
 }
 
 function asOrdinalType2(kind) {
     switch (kind) {
-        case position2:
+        case position3:
             return "point";
         case color4:
             return ordinalImplicit2;
         default:
             return "ordinal";
     }
 }
@@ -59497,15 +59566,15 @@
 function formatAuto2(locale5 = "en-US") {
     const number14 = formatNumber2(locale5);
     return (v3) => (v3 instanceof Date ? formatIsoDate2 : typeof v3 === "number" ? number14 : string2)(v3);
 }
 var formatDefault2 = formatAuto2();
 
 // js/pyobsplot-js/node_modules/@observablehq/plot/src/style.js
-var offset2 = typeof window !== "undefined" && window.devicePixelRatio > 1 ? 0 : 0.5;
+var offset2 = (typeof window !== "undefined" ? window.devicePixelRatio > 1 : typeof it === "undefined") ? 0 : 0.5;
 var nextClipId2 = 0;
 
 function getClipId2() {
     return `plot-clip-${++nextClipId2}`;
 }
 
 function styles2(mark, {
@@ -59747,22 +59816,22 @@
         warn2(
             `Warning: the implicit z channel has high cardinality. This may occur when the fill or stroke channel is associated with quantitative data rather than ordinal or categorical data. You can suppress this warning by setting the z option explicitly; if this data represents a single series, set z to null.`
         );
     }
     return G.values();
 }
 
-function* groupIndex2(I, position3, {
+function* groupIndex2(I, position5, {
     z
 }, channels) {
     const {
         z: Z
     } = channels;
     const A6 = groupAesthetics2(channels);
-    const C4 = [...position3, ...A6];
+    const C4 = [...position5, ...A6];
     for (const G of Z ? groupZ4(I, Z, z) : [I]) {
         let Ag;
         let Gg;
         out:
             for (const i of G) {
                 for (const c11 of C4) {
                     if (!defined2(c11[i])) {
@@ -59911,15 +59980,15 @@
     if ((value = number11(value)) !== impliedValue)
         return value;
 }
 var validClassName2 = /^-?([_a-z]|[\240-\377]|\\[0-9a-f]{1,6}(\r\n|[ \t\r\n\f])?|\\[^\r\n\f0-9a-f])([_a-z0-9-]|[\240-\377]|\\[0-9a-f]{1,6}(\r\n|[ \t\r\n\f])?|\\[^\r\n\f0-9a-f])*$/i;
 
 function maybeClassName2(name) {
     if (name === void 0)
-        return `plot-${Math.random().toString(16).slice(2)}`;
+        return "plot-d6a7b5";
     name = `${name}`;
     if (!validClassName2.test(name))
         throw new Error(`invalid class name: ${name}`);
     return name;
 }
 
 function applyInlineStyles2(selection3, style) {
@@ -60109,21 +60178,25 @@
         i
     })) : fyDomain ? fyDomain.map((y7, i) => ({
         y: y7,
         i
     })) : void 0;
 }
 
-function facetOrder2({
+function recreateFacets2(facets, {
     x: X4,
     y: Y4
 }) {
-    const xi = X4 && new Map(X4.map((v3, i) => [v3, i]));
-    const yi = Y4 && new Map(Y4.map((v3, i) => [v3, i]));
-    return X4 && Y4 ? (a7, b) => xi.get(a7.x) - xi.get(b.x) || yi.get(a7.y) - yi.get(b.y) : X4 ? (a7, b) => xi.get(a7.x) - xi.get(b.x) : (a7, b) => yi.get(a7.y) - yi.get(b.y);
+    X4 &&= new InternMap2(X4.map((x7, i) => [x7, i]));
+    Y4 &&= new InternMap2(Y4.map((y7, i) => [y7, i]));
+    return facets.filter(
+        X4 && Y4 ? (f) => X4.has(f.x) && Y4.has(f.y) : X4 ? (f) => X4.has(f.x) : (f) => Y4.has(f.y)
+    ).sort(
+        X4 && Y4 ? (a7, b) => X4.get(a7.x) - X4.get(b.x) || Y4.get(a7.y) - Y4.get(b.y) : X4 ? (a7, b) => X4.get(a7.x) - X4.get(b.x) : (a7, b) => Y4.get(a7.y) - Y4.get(b.y)
+    );
 }
 
 function facetGroups2(data, {
     fx,
     fy
 }) {
     const I = range8(data);
@@ -60353,28 +60426,31 @@
             className
     } = options;
     const context = createContext2(options);
     className = maybeClassName2(className);
     opacity3 = maybeNumberChannel2(opacity3)[1];
     if (tickFormat3 === null)
         tickFormat3 = () => null;
-    const svg3 = create4("svg", context).attr("class", className).attr("font-family", "system-ui, sans-serif").attr("font-size", 10).attr("width", width).attr("height", height).attr("viewBox", `0 0 ${width} ${height}`).call(
-        (svg4) => svg4.append("style").text(`
-        .${className} {
-          display: block;
-          background: white;
-          height: auto;
-          height: intrinsic;
-          max-width: 100%;
-          overflow: visible;
-        }
-        .${className} text {
-          white-space: pre;
-        }
-      `)
+    const svg3 = create4("svg", context).attr("class", `${className}-ramp`).attr("font-family", "system-ui, sans-serif").attr("font-size", 10).attr("width", width).attr("height", height).attr("viewBox", `0 0 ${width} ${height}`).call(
+        (svg4) => (
+            // Warning: if you edit this, change defaultClassName.
+            svg4.append("style").text(
+                `.${className}-ramp {
+  display: block;
+  background: white;
+  height: auto;
+  height: intrinsic;
+  max-width: 100%;
+  overflow: visible;
+}
+.${className}-ramp text {
+  white-space: pre;
+}`
+            )
+        )
     ).call(applyInlineStyles2, style);
     let tickAdjust = (g) => g.selectAll(".tick line").attr("y1", marginTop + marginBottom - height);
     let x7;
     const applyRange = round3 ? (x8, range10) => x8.rangeRound(range10) : (x8, range10) => x8.range(range10);
     const {
         type: type3,
         domain,
@@ -60438,20 +60514,15 @@
     ...options
 } = {}) {
     if (!isOrdinalScale2(color5) && !isThresholdScale2(color5))
         throw new Error(`swatches legend requires ordinal or threshold color scale (not ${color5.type})`);
     return legendItems2(
         color5,
         options,
-        (selection3, scale5) => selection3.append("svg").attr("fill", scale5.scale).attr("fill-opacity", maybeNumberChannel2(opacity3)[1]).append("rect").attr("width", "100%").attr("height", "100%"),
-        (className) => `.${className}-swatch svg {
-        width: var(--swatchWidth);
-        height: var(--swatchHeight);
-        margin-right: 0.5em;
-      }`
+        (selection3, scale5, width, height) => selection3.append("svg").attr("width", width).attr("height", height).attr("fill", scale5.scale).attr("fill-opacity", maybeNumberChannel2(opacity3)[1]).append("rect").attr("width", "100%").attr("height", "100%")
     );
 }
 
 function legendSymbols2(symbol3, {
     fill = symbol3.hint?.fill !== void 0 ? symbol3.hint.fill : "none",
     fillOpacity = 1,
     stroke = symbol3.hint?.stroke !== void 0 ? symbol3.hint.stroke : isNoneish2(fill) ? "currentColor" : "none",
@@ -60467,34 +60538,23 @@
     const size = r * r * Math.PI;
     fillOpacity = maybeNumberChannel2(fillOpacity)[1];
     strokeOpacity = maybeNumberChannel2(strokeOpacity)[1];
     strokeWidth = maybeNumberChannel2(strokeWidth)[1];
     return legendItems2(
         symbol3,
         options,
-        (selection3) => selection3.append("svg").attr("viewBox", "-8 -8 16 16").attr("fill", vf === "color" ? (d) => sf.scale(d) : null).attr("stroke", vs === "color" ? (d) => ss.scale(d) : null).append("path").attr("d", (d) => {
+        (selection3, scale6, width, height) => selection3.append("svg").attr("viewBox", "-8 -8 16 16").attr("width", width).attr("height", height).attr("fill", vf === "color" ? (d) => sf.scale(d) : cf).attr("fill-opacity", fillOpacity).attr("stroke", vs === "color" ? (d) => ss.scale(d) : cs).attr("stroke-opacity", strokeOpacity).attr("stroke-width", strokeWidth).append("path").attr("d", (d) => {
             const p = pathRound2();
             symbol3.scale(d).draw(p, size);
             return p;
-        }),
-        (className) => `.${className}-swatch > svg {
-        width: var(--swatchWidth);
-        height: var(--swatchHeight);
-        margin-right: 0.5em;
-        overflow: visible;
-        fill: ${cf};
-        fill-opacity: ${fillOpacity};
-        stroke: ${cs};
-        stroke-width: ${strokeWidth}px;
-        stroke-opacity: ${strokeOpacity};
-      }`
+        })
     );
 }
 
-function legendItems2(scale5, options = {}, swatch, swatchStyle) {
+function legendItems2(scale5, options = {}, swatch) {
     let {
         columns,
         tickFormat: tickFormat3,
         fontVariant = inferFontVariant4(scale5),
         // TODO label,
         swatchSize = 15,
         swatchWidth = swatchSize,
@@ -60503,73 +60563,67 @@
         className,
         style,
         width
     } = options;
     const context = createContext2(options);
     className = maybeClassName2(className);
     tickFormat3 = maybeAutoTickFormat2(tickFormat3, scale5.domain);
-    const swatches = create4("div", context).attr("class", className).attr(
-        "style",
-        `
-        --swatchWidth: ${+swatchWidth}px;
-        --swatchHeight: ${+swatchHeight}px;
-      `
+    const swatches = create4("div", context).attr(
+        "class",
+        `${className}-swatches ${className}-swatches-${columns != null ? "columns" : "wrap"}`
     );
     let extraStyle;
     if (columns != null) {
-        extraStyle = `
-      .${className}-swatch {
-        display: flex;
-        align-items: center;
-        break-inside: avoid;
-        padding-bottom: 1px;
-      }
-      .${className}-swatch::before {
-        flex-shrink: 0;
-      }
-      .${className}-label {
-        white-space: nowrap;
-        overflow: hidden;
-        text-overflow: ellipsis;
-      }
-    `;
-        swatches.style("columns", columns).selectAll().data(scale5.domain).enter().append("div").attr("class", `${className}-swatch`).call(swatch, scale5).call(
-            (item) => item.append("div").attr("class", `${className}-label`).attr("title", tickFormat3).text(tickFormat3)
+        extraStyle = `.${className}-swatches-columns .${className}-swatch {
+  display: flex;
+  align-items: center;
+  break-inside: avoid;
+  padding-bottom: 1px;
+}
+.${className}-swatches-columns .${className}-swatch::before {
+  flex-shrink: 0;
+}
+.${className}-swatches-columns .${className}-swatch-label {
+  white-space: nowrap;
+  overflow: hidden;
+  text-overflow: ellipsis;
+}`;
+        swatches.style("columns", columns).selectAll().data(scale5.domain).enter().append("div").attr("class", `${className}-swatch`).call(swatch, scale5, swatchWidth, swatchHeight).call(
+            (item) => item.append("div").attr("class", `${className}-swatch-label`).attr("title", tickFormat3).text(tickFormat3)
         );
     } else {
-        extraStyle = `
-      .${className} {
-        display: flex;
-        align-items: center;
-        min-height: 33px;
-        flex-wrap: wrap;
-      }
-      .${className}-swatch {
-        display: inline-flex;
-        align-items: center;
-        margin-right: 1em;
-      }
-    `;
-        swatches.selectAll().data(scale5.domain).enter().append("span").attr("class", `${className}-swatch`).call(swatch, scale5).append(function() {
+        extraStyle = `.${className}-swatches-wrap {
+  display: flex;
+  align-items: center;
+  min-height: 33px;
+  flex-wrap: wrap;
+}
+.${className}-swatches-wrap .${className}-swatch {
+  display: inline-flex;
+  align-items: center;
+  margin-right: 1em;
+}`;
+        swatches.selectAll().data(scale5.domain).enter().append("span").attr("class", `${className}-swatch`).call(swatch, scale5, swatchWidth, swatchHeight).append(function() {
             return this.ownerDocument.createTextNode(tickFormat3.apply(this, arguments));
         });
     }
     return swatches.call(
-        (div) => div.insert("style", "*").text(`
-        .${className} {
-          font-family: system-ui, sans-serif;
-          font-size: 10px;
-          margin-bottom: 0.5em;${marginLeft === void 0 ? "" : `
-          margin-left: ${+marginLeft}px;`}${width === void 0 ? "" : `
-          width: ${width}px;`}
-        }
-        ${swatchStyle(className)}
-        ${extraStyle}
-      `)
-    ).style("font-variant", impliedString2(fontVariant, "normal")).call(applyInlineStyles2, style).node();
+        (div) => div.insert("style", "*").text(
+            `.${className}-swatches {
+  font-family: system-ui, sans-serif;
+  font-size: 10px;
+  margin-bottom: 0.5em;
+}
+.${className}-swatch > svg {
+  margin-right: 0.5em;
+  overflow: visible;
+}
+${extraStyle}`
+        )
+    ).style("margin-left", marginLeft ? `${+marginLeft}px` : null).style("width", width === void 0 ? null : `${+width}px`).style("font-variant", impliedString2(fontVariant, "normal")).call(applyInlineStyles2, style).node();
 }
 
 // js/pyobsplot-js/node_modules/@observablehq/plot/src/legends.js
 var legendRegistry2 = /* @__PURE__ */ new Map([
     ["symbol", legendSymbols2],
     ["color", legendColor2],
     ["opacity", legendOpacity2]
@@ -60607,20 +60661,26 @@
             throw new Error(`unknown legend type: ${key}`);
         if (!(key in scales))
             return;
         return legendRegistry2.get(key)(scales[key], legendOptions2(context, defaults41[key], options), (key2) => scales[key2]);
     };
 }
 
-function legendOptions2(context, {
+function legendOptions2({
+    className,
+    ...context
+}, {
     label,
     ticks: ticks3,
     tickFormat: tickFormat3
 } = {}, options) {
-    return inherit4(options, context, {
+    return inherit4(options, {
+        className,
+        ...context
+    }, {
         label,
         ticks: ticks3,
         tickFormat: tickFormat3
     });
 }
 
 function legendColor2(color5, {
@@ -61949,18 +62009,19 @@
     textStroke,
     textStrokeOpacity,
     textStrokeWidth,
     tickSize = k3 === "y" ? 6 : 0,
     tickPadding,
     tickRotate,
     x: x7,
-    marginTop = 20,
-    marginRight = anchor === "right" ? 40 : 0,
-    marginBottom = 20,
-    marginLeft = anchor === "left" ? 40 : 0,
+    margin,
+    marginTop = margin === void 0 ? 20 : margin,
+    marginRight = margin === void 0 ? anchor === "right" ? 40 : 0 : margin,
+    marginBottom = margin === void 0 ? 20 : margin,
+    marginLeft = margin === void 0 ? anchor === "left" ? 40 : 0 : margin,
     label,
     labelOffset,
     labelAnchor,
     ...options
 }) {
     tickSize = number11(tickSize);
     tickPadding = number11(tickPadding);
@@ -61991,24 +62052,21 @@
             x: x7,
             marginTop,
             marginRight,
             marginBottom,
             marginLeft,
             ...options
         }) : null,
-        !isNoneish2(fill) && label !== null ? text2([], {
-            fill,
-            fillOpacity,
-            ...options,
-            lineWidth: void 0,
-            textOverflow: void 0,
-            facet: "super",
-            x: null,
-            y: null,
-            initializer: function(data2, facets, channels, scales, dimensions) {
+        !isNoneish2(fill) && label !== null ? text2(
+            [],
+            labelOptions2({
+                fill,
+                fillOpacity,
+                ...options
+            }, function(data2, facets, channels, scales, dimensions) {
                 const scale5 = scales[k3];
                 const {
                     marginTop: marginTop2,
                     marginRight: marginRight2,
                     marginBottom: marginBottom2,
                     marginLeft: marginLeft2
                 } = k3 === "y" && dimensions.inset || dimensions;
@@ -62034,16 +62092,16 @@
                     ],
                     channels: {
                         text: {
                             value: [label === void 0 ? inferAxisLabel2(k3, scale5, cla) : label]
                         }
                     }
                 };
-            }
-        }) : null
+            })
+        ) : null
     );
 }
 
 function axisKx2(k3, anchor, data, {
     color: color5 = "currentColor",
     opacity: opacity3 = 1,
     stroke = color5,
@@ -62055,18 +62113,19 @@
     textStroke,
     textStrokeOpacity,
     textStrokeWidth,
     tickSize = k3 === "x" ? 6 : 0,
     tickPadding,
     tickRotate,
     y: y7,
-    marginTop = anchor === "top" ? 30 : 0,
-    marginRight = 20,
-    marginBottom = anchor === "bottom" ? 30 : 0,
-    marginLeft = 20,
+    margin,
+    marginTop = margin === void 0 ? anchor === "top" ? 30 : 0 : margin,
+    marginRight = margin === void 0 ? 20 : margin,
+    marginBottom = margin === void 0 ? anchor === "bottom" ? 30 : 0 : margin,
+    marginLeft = margin === void 0 ? 20 : margin,
     label,
     labelAnchor,
     labelOffset,
     ...options
 }) {
     tickSize = number11(tickSize);
     tickPadding = number11(tickPadding);
@@ -62097,24 +62156,21 @@
             y: y7,
             marginTop,
             marginRight,
             marginBottom,
             marginLeft,
             ...options
         }) : null,
-        !isNoneish2(fill) && label !== null ? text2([], {
-            fill,
-            fillOpacity,
-            ...options,
-            lineWidth: void 0,
-            textOverflow: void 0,
-            facet: "super",
-            x: null,
-            y: null,
-            initializer: function(data2, facets, channels, scales, dimensions) {
+        !isNoneish2(fill) && label !== null ? text2(
+            [],
+            labelOptions2({
+                fill,
+                fillOpacity,
+                ...options
+            }, function(data2, facets, channels, scales, dimensions) {
                 const scale5 = scales[k3];
                 const {
                     marginTop: marginTop2,
                     marginRight: marginRight2,
                     marginBottom: marginBottom2,
                     marginLeft: marginLeft2
                 } = k3 === "x" && dimensions.inset || dimensions;
@@ -62137,16 +62193,16 @@
                     ],
                     channels: {
                         text: {
                             value: [label === void 0 ? inferAxisLabel2(k3, scale5, cla) : label]
                         }
                     }
                 };
-            }
-        }) : null
+            })
+        ) : null
     );
 }
 
 function axisTickKy2(k3, anchor, data, {
     strokeWidth = 1,
     strokeLinecap = null,
     strokeLinejoin = null,
@@ -62352,14 +62408,44 @@
         stroke,
         strokeOpacity,
         strokeWidth,
         ...options
     };
 }
 
+function labelOptions2({
+    fill,
+    fillOpacity,
+    fontFamily,
+    fontSize,
+    fontStyle,
+    fontWeight,
+    monospace,
+    pointerEvents,
+    shapeRendering
+}, initializer3) {
+    [, fill] = maybeColorChannel2(fill);
+    [, fillOpacity] = maybeNumberChannel2(fillOpacity);
+    return {
+        facet: "super",
+        x: null,
+        y: null,
+        fill,
+        fillOpacity,
+        fontFamily,
+        fontSize,
+        fontStyle,
+        fontWeight,
+        monospace,
+        pointerEvents,
+        shapeRendering,
+        initializer: initializer3
+    };
+}
+
 function axisMark2(mark, k3, ariaLabel, data, options, initialize) {
     let channels;
     const m5 = mark(
         data,
         initializer2(options, function(data2, facets, _channels, scales) {
             const {
                 [k3]: scale5
@@ -62566,15 +62652,15 @@
     const axes = flatMarks2(inferAxes2(marks3, channelsByScale, options));
     for (const mark of axes) {
         const facetState = maybeMarkFacet2(mark, topFacetState, options);
         if (facetState)
             facetStateByMark.set(mark, facetState);
     }
     marks3.unshift(...axes);
-    const facets = createFacets2(channelsByScale, options);
+    let facets = createFacets2(channelsByScale, options);
     if (facets !== void 0) {
         const topFacetsIndex = topFacetState ? facetFilter2(facets, topFacetState) : void 0;
         for (const mark of marks3) {
             if (mark.facet === null || mark.facet === "super")
                 continue;
             const facetState = facetStateByMark.get(mark);
             if (facetState === void 0)
@@ -62634,15 +62720,15 @@
     autoScaleRange2(scaleDescriptors, dimensions);
     const {
         fx,
         fy
     } = scales;
     const subdimensions = fx || fy ? innerDimensions2(scaleDescriptors, dimensions) : dimensions;
     const superdimensions = fx || fy ? actualDimensions2(scales, dimensions) : dimensions;
-    const context = createContext2(options, subdimensions, scaleDescriptors);
+    const context = createContext2(options, subdimensions, className);
     const newByScale = /* @__PURE__ */ new Set();
     for (const [mark, state] of stateByMark) {
         if (mark.initializer != null) {
             const dimensions2 = mark.facet === "super" ? superdimensions : subdimensions;
             const update = mark.initializer(state.data, state.facets, state.channels, scales, dimensions2, context);
             if (update.data !== void 0) {
                 state.data = update.data;
@@ -62653,15 +62739,15 @@
             if (update.channels !== void 0) {
                 inferChannelScales2(update.channels);
                 Object.assign(state.channels, update.channels);
                 for (const channel of Object.values(update.channels)) {
                     const {
                         scale: scale5
                     } = channel;
-                    if (scale5 != null && registry2.get(scale5) !== position2) {
+                    if (scale5 != null && registry2.get(scale5) !== position3) {
                         applyScaleTransform2(channel, options);
                         newByScale.add(scale5);
                     }
                 }
                 const {
                     fx: fx2,
                     fy: fy2
@@ -62694,34 +62780,37 @@
         state.values = mark.scale(state.channels, scales, context);
     }
     const {
         width,
         height
     } = dimensions;
     const svg3 = create4("svg", context).attr("class", className).attr("fill", "currentColor").attr("font-family", "system-ui, sans-serif").attr("font-size", 10).attr("text-anchor", "middle").attr("width", width).attr("height", height).attr("viewBox", `0 0 ${width} ${height}`).attr("aria-label", ariaLabel).attr("aria-description", ariaDescription).call(
-        (svg4) => svg4.append("style").text(`
-        .${className} {
-          display: block;
-          background: white;
-          height: auto;
-          height: intrinsic;
-          max-width: 100%;
-        }
-        .${className} text,
-        .${className} tspan {
-          white-space: pre;
-        }
-      `)
+        (svg4) => (
+            // Warning: if you edit this, change defaultClassName.
+            svg4.append("style").text(
+                `.${className} {
+  display: block;
+  background: white;
+  height: auto;
+  height: intrinsic;
+  max-width: 100%;
+}
+.${className} text,
+.${className} tspan {
+  white-space: pre;
+}`
+            )
+        )
     ).call(applyInlineStyles2, style).node();
     if (facets !== void 0) {
         const facetDomains = {
             x: fx?.domain(),
             y: fy?.domain()
         };
-        facets.sort(facetOrder2(facetDomains));
+        facets = recreateFacets2(facets, facetDomains);
         select_default5(svg3).selectAll().data(facets).enter().append("g").attr("aria-label", "facet").attr("transform", facetTranslate2(fx, fy, dimensions)).each(function(f) {
             let empty7 = true;
             for (const mark of marks3) {
                 if (mark.facet === "super")
                     continue;
                 const {
                     channels,
@@ -62776,15 +62865,15 @@
         figure = document2.createElement("figure");
         figure.style.maxWidth = "initial";
         for (const legend3 of legends)
             figure.appendChild(legend3);
         figure.appendChild(svg3);
         if (caption != null) {
             const figcaption = document2.createElement("figcaption");
-            figcaption.appendChild(caption instanceof Node ? caption : document2.createTextNode(caption));
+            figcaption.appendChild(caption?.ownerDocument ? caption : document2.createTextNode(caption));
             figure.appendChild(figcaption);
         }
     }
     figure.scale = exposeScales2(scaleDescriptors);
     figure.legend = exposeLegends2(scaleDescriptors, context, options);
     const w = consumeWarnings2();
     if (w > 0) {
@@ -62941,15 +63030,15 @@
         data
     } = topFacetState;
     if (mark.facet !== "auto" || mark.data === data)
         return {
             channels,
             groups: groups3
         };
-    if ((groups3.size > 1 || groups3.size === 1 && channels.fx && channels.fy && [...groups3][0][1].size > 1) && arrayify4(mark.data)?.length === data.length) {
+    if (data.length > 0 && (groups3.size > 1 || groups3.size === 1 && channels.fx && channels.fy && [...groups3][0][1].size > 1) && arrayify4(mark.data)?.length === data.length) {
         warn2(
             `Warning: the ${mark.ariaLabel} mark appears to use faceted data, but isn\u2019t faceted. The mark data has the same length as the facet data and the mark facet option is "auto", but the mark data and facet data are distinct. If this mark should be faceted, set the mark facet option to true; otherwise, suppress this warning by setting the mark facet option to false.`
         );
     }
 }
 
 function inferAxes2(marks3, channelsByScale, options) {
@@ -67089,15 +67178,15 @@
                 const j = halfedges[i2];
                 if (j > i2)
                     link7(triangles[i2], triangles[j]);
             }
             for (let i2 = 0; i2 < hull3.length; ++i2) {
                 link7(hull3[i2], hull3[(i2 + 1) % hull3.length]);
             }
-            select_default5(this).selectAll().data(newIndex).join("path").call(applyDirectStyles2, mark).attr("d", (i2) => {
+            select_default5(this).selectAll().data(newIndex).enter().append("path").call(applyDirectStyles2, mark).attr("d", (i2) => {
                 const p = pathRound2();
                 const c11 = curve(p);
                 c11.lineStart();
                 c11.point(X15[i2], Y15[i2]);
                 c11.point(X25[i2], Y25[i2]);
                 c11.lineEnd();
                 return p;
@@ -67356,15 +67445,15 @@
         return index5;
     }
     render(index5, scales, channels, dimensions, context) {
         const {
             contours
         } = channels;
         const path3 = path_default3();
-        return create_default2("svg:g", context).call(applyIndirectStyles2, this, dimensions, context).call(applyTransform2, this, {}).call(
+        return create4("svg:g", context).call(applyIndirectStyles2, this, dimensions, context).call(applyTransform2, this, {}).call(
             (g) => g.selectAll().data(index5).enter().append("path").call(applyDirectStyles2, this).call(applyChannelStyles2, this, channels).attr("d", (i) => path3(contours[i]))
         ).node();
     }
 };
 
 function density2(data, options = {}) {
     let {
@@ -67850,62 +67939,82 @@
     return typeof value === "string" && (isPath2(value) || isUrl2(value)) ? [void 0, value] : [value, void 0];
 }
 var Image3 = class extends Mark2 {
     constructor(data, options = {}) {
         let {
             x: x7,
             y: y7,
+            r,
             width,
             height,
+            rotate,
             src,
             preserveAspectRatio,
             crossOrigin,
             frameAnchor,
             imageRendering
         } = options;
-        if (width === void 0 && height !== void 0)
+        if (r == null)
+            r = void 0;
+        if (r === void 0 && width === void 0 && height === void 0)
+            width = height = 16;
+        else if (width === void 0 && height !== void 0)
             width = height;
         else if (height === void 0 && width !== void 0)
             height = width;
         const [vs, cs] = maybePathChannel2(src);
-        const [vw, cw] = maybeNumberChannel2(width, 16);
-        const [vh, ch] = maybeNumberChannel2(height, 16);
+        const [vr, cr] = maybeNumberChannel2(r);
+        const [vw, cw] = maybeNumberChannel2(width, cr !== void 0 ? cr * 2 : void 0);
+        const [vh, ch] = maybeNumberChannel2(height, cr !== void 0 ? cr * 2 : void 0);
+        const [va, ca5] = maybeNumberChannel2(rotate, 0);
         super(
             data, {
                 x: {
                     value: x7,
                     scale: "x",
                     optional: true
                 },
                 y: {
                     value: y7,
                     scale: "y",
                     optional: true
                 },
+                r: {
+                    value: vr,
+                    scale: "r",
+                    filter: positive2,
+                    optional: true
+                },
                 width: {
                     value: vw,
                     filter: positive2,
                     optional: true
                 },
                 height: {
                     value: vh,
                     filter: positive2,
                     optional: true
                 },
+                rotate: {
+                    value: va,
+                    optional: true
+                },
                 src: {
                     value: vs,
                     optional: true
                 }
             },
-            options,
+            withDefaultSort2(options),
             defaults39
         );
         this.src = cs;
         this.width = cw;
+        this.rotate = ca5;
         this.height = ch;
+        this.r = cr;
         this.preserveAspectRatio = impliedString2(preserveAspectRatio, "xMidYMid");
         this.crossOrigin = string2(crossOrigin);
         this.frameAnchor = maybeFrameAnchor2(frameAnchor);
         this.imageRendering = impliedString2(imageRendering, "auto");
     }
     render(index5, scales, channels, dimensions, context) {
         const {
@@ -67913,32 +68022,38 @@
             y: y7
         } = scales;
         const {
             x: X4,
             y: Y4,
             width: W,
             height: H,
+            r: R,
+            rotate: A6,
             src: S
         } = channels;
+        const {
+            r,
+            width,
+            height,
+            rotate
+        } = this;
         const [cx, cy] = applyFrameAnchor2(this, dimensions);
         return create4("svg:g", context).call(applyIndirectStyles2, this, dimensions, context).call(applyTransform2, this, {
             x: X4 && x7,
             y: Y4 && y7
         }).call(
-            (g) => g.selectAll().data(index5).enter().append("image").call(applyDirectStyles2, this).attr(
-                "x",
-                W && X4 ? (i) => X4[i] - W[i] / 2 : W ? (i) => cx - W[i] / 2 : X4 ? (i) => X4[i] - this.width / 2 : cx - this.width / 2
-            ).attr(
-                "y",
-                H && Y4 ? (i) => Y4[i] - H[i] / 2 : H ? (i) => cy - H[i] / 2 : Y4 ? (i) => Y4[i] - this.height / 2 : cy - this.height / 2
-            ).attr("width", W ? (i) => W[i] : this.width).attr("height", H ? (i) => H[i] : this.height).call(applyAttr2, "href", S ? (i) => S[i] : this.src).call(applyAttr2, "preserveAspectRatio", this.preserveAspectRatio).call(applyAttr2, "crossorigin", this.crossOrigin).call(applyAttr2, "image-rendering", this.imageRendering).call(applyChannelStyles2, this, channels)
+            (g) => g.selectAll().data(index5).enter().append("image").call(applyDirectStyles2, this).attr("x", position4(X4, W, R, cx, width, r)).attr("y", position4(Y4, H, R, cy, height, r)).attr("width", W ? (i) => W[i] : width !== void 0 ? width : R ? (i) => R[i] * 2 : r * 2).attr("height", H ? (i) => H[i] : height !== void 0 ? height : R ? (i) => R[i] * 2 : r * 2).attr("transform", A6 ? (i) => `rotate(${A6[i]})` : rotate ? `rotate(${rotate})` : null).attr("transform-origin", A6 || rotate ? template2`${X4 ? (i) => X4[i] : cx}px ${Y4 ? (i) => Y4[i] : cy}px` : null).call(applyAttr2, "href", S ? (i) => S[i] : this.src).call(applyAttr2, "preserveAspectRatio", this.preserveAspectRatio).call(applyAttr2, "crossorigin", this.crossOrigin).call(applyAttr2, "image-rendering", this.imageRendering).call(applyAttr2, "clip-path", R ? (i) => `circle(${R[i]}px)` : r !== void 0 ? `circle(${r}px)` : null).call(applyChannelStyles2, this, channels)
         ).node();
     }
 };
 
+function position4(X4, W, R, x7, w, r) {
+    return W && X4 ? (i) => X4[i] - W[i] / 2 : W ? (i) => x7 - W[i] / 2 : X4 && w !== void 0 ? (i) => X4[i] - w / 2 : w !== void 0 ? x7 - w / 2 : R && X4 ? (i) => X4[i] - R[i] : R ? (i) => x7 - R[i] : X4 ? (i) => X4[i] - r : x7 - r;
+}
+
 function image2(data, options = {}) {
     let {
         x: x7,
         y: y7,
         ...remainingOptions
     } = options;
     if (options.frameAnchor === void 0)
@@ -68736,70 +68851,71 @@
     } : anchor;
 }
 
 function dodgeX2(dodgeOptions = {}, options = {}) {
     if (arguments.length === 1)
         [dodgeOptions, options] = mergeOptions6(dodgeOptions);
     let {
-        anchor = "left", padding = 1
+        anchor = "left", padding = 1, r = options.r
     } = maybeAnchor5(dodgeOptions);
     switch (`${anchor}`.toLowerCase()) {
         case "left":
             anchor = anchorXLeft2;
             break;
         case "right":
             anchor = anchorXRight2;
             break;
         case "middle":
             anchor = anchorXMiddle2;
             break;
         default:
             throw new Error(`unknown dodge anchor: ${anchor}`);
     }
-    return dodge2("x", "y", anchor, number11(padding), options);
+    return dodge2("x", "y", anchor, number11(padding), r, options);
 }
 
 function dodgeY2(dodgeOptions = {}, options = {}) {
     if (arguments.length === 1)
         [dodgeOptions, options] = mergeOptions6(dodgeOptions);
     let {
-        anchor = "bottom", padding = 1
+        anchor = "bottom", padding = 1, r = options.r
     } = maybeAnchor5(dodgeOptions);
     switch (`${anchor}`.toLowerCase()) {
         case "top":
             anchor = anchorYTop2;
             break;
         case "bottom":
             anchor = anchorYBottom2;
             break;
         case "middle":
             anchor = anchorYMiddle2;
             break;
         default:
             throw new Error(`unknown dodge anchor: ${anchor}`);
     }
-    return dodge2("y", "x", anchor, number11(padding), options);
+    return dodge2("y", "x", anchor, number11(padding), r, options);
 }
 
 function mergeOptions6(options) {
     const {
         anchor,
         padding,
         ...rest
     } = options;
+    const {
+        r
+    } = rest;
     return [{
         anchor,
-        padding
+        padding,
+        r
     }, rest];
 }
 
-function dodge2(y7, x7, anchor, padding, options) {
-    const {
-        r
-    } = options;
+function dodge2(y7, x7, anchor, padding, r, options) {
     if (r != null && typeof r !== "number") {
         const {
             channels,
             sort: sort5,
             reverse: reverse5
         } = options;
         options = {
@@ -68823,35 +68939,35 @@
             [x7]: X4, r: R
         } = channels;
         if (!channels[x7])
             throw new Error(`missing channel: ${x7}`);
         ({
             [x7]: X4
         } = applyPosition2(channels, scales, context));
-        const r2 = R ? void 0 : this.r !== void 0 ? this.r : options.r !== void 0 ? number11(options.r) : 3;
+        const cr = R ? void 0 : r !== void 0 ? number11(r) : this.r !== void 0 ? this.r : 3;
         if (R)
             R = valueof2(R.value, scales[R.scale] || identity13, Float64Array);
         let [ky3, ty] = anchor(dimensions);
         const compare = ky3 ? compareAscending2 : compareSymmetric2;
         const Y4 = new Float64Array(X4.length);
-        const radius3 = R ? (i) => R[i] : () => r2;
+        const radius3 = R ? (i) => R[i] : () => cr;
         for (let I of facets) {
             const tree3 = (0, import_interval_tree_1d2.default)();
             I = I.filter(R ? (i) => finite5(X4[i]) && positive2(R[i]) : (i) => finite5(X4[i]));
             const intervals = new Float64Array(2 * I.length + 2);
             for (const i of I) {
                 const ri = radius3(i);
                 const y011 = ky3 ? ri + padding : 0;
                 const l = X4[i] - ri;
                 const h = X4[i] + ri;
                 let k3 = 2;
                 tree3.queryInterval(l - padding, h + padding, ([, , j]) => {
                     const yj = Y4[j] - y011;
                     const dx = X4[i] - X4[j];
-                    const dr = padding + (R ? R[i] + R[j] : 2 * r2);
+                    const dr = padding + (R ? R[i] + R[j] : 2 * cr);
                     const dy = Math.sqrt(dr * dr - dx * dx);
                     intervals[k3++] = yj - dy;
                     intervals[k3++] = yj + dy;
                 });
                 let candidates = intervals.slice(0, k3);
                 if (ky3)
                     candidates = candidates.filter((y8) => y8 >= 0);
@@ -69845,18 +69961,18 @@
 };
 
 function* toArrayBufferViewIterator(ArrayCtor, source) {
     const wrap = function*(x7) {
         yield x7;
     };
     const buffers = typeof source === "string" ? wrap(source) : ArrayBuffer.isView(source) ? wrap(source) : source instanceof ArrayBuffer ? wrap(source) : source instanceof SharedArrayBuf ? wrap(source) : !isIterable3(source) ? wrap(source) : source;
-    yield* pump(function*(it) {
+    yield* pump(function*(it2) {
         let r = null;
         do {
-            r = it.next(yield toArrayBufferView(ArrayCtor, r));
+            r = it2.next(yield toArrayBufferView(ArrayCtor, r));
         } while (!r.done);
     }(buffers[Symbol.iterator]()));
     return new ArrayCtor();
 }
 var toInt8ArrayIterator = (input) => toArrayBufferViewIterator(Int8Array, input);
 var toInt16ArrayIterator = (input) => toArrayBufferViewIterator(Int16Array, input);
 var toInt32ArrayIterator = (input) => toArrayBufferViewIterator(Int32Array, input);
@@ -69875,30 +69991,30 @@
         const wrap = function(x7) {
             return __asyncGenerator(this, arguments, function*() {
                 yield yield __await(yield __await(x7));
             });
         };
         const emit = function(source2) {
             return __asyncGenerator(this, arguments, function*() {
-                yield __await(yield* __asyncDelegator(__asyncValues(pump(function*(it) {
+                yield __await(yield* __asyncDelegator(__asyncValues(pump(function*(it2) {
                     let r = null;
                     do {
-                        r = it.next(yield r === null || r === void 0 ? void 0 : r.value);
+                        r = it2.next(yield r === null || r === void 0 ? void 0 : r.value);
                     } while (!r.done);
                 }(source2[Symbol.iterator]())))));
             });
         };
         const buffers = typeof source === "string" ? wrap(source) : ArrayBuffer.isView(source) ? wrap(source) : source instanceof ArrayBuffer ? wrap(source) : source instanceof SharedArrayBuf ? wrap(source) : isIterable3(source) ? emit(source) : !isAsyncIterable(source) ? wrap(source) : source;
         yield __await(
             // otherwise if AsyncIterable, use it
-            yield* __asyncDelegator(__asyncValues(pump(function(it) {
+            yield* __asyncDelegator(__asyncValues(pump(function(it2) {
                 return __asyncGenerator(this, arguments, function*() {
                     let r = null;
                     do {
-                        r = yield __await(it.next(yield yield __await(toArrayBufferView(ArrayCtor, r))));
+                        r = yield __await(it2.next(yield yield __await(toArrayBufferView(ArrayCtor, r))));
                     } while (!r.done);
                 });
             }(buffers[Symbol.asyncIterator]()))))
         );
         return yield __await(new ArrayCtor());
     });
 }
@@ -69979,38 +70095,38 @@
         [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);
         return buffer;
     }
     ({
         cmd,
         size
     } = yield null);
-    const it = toUint8ArrayIterator(source)[Symbol.iterator]();
+    const it2 = toUint8ArrayIterator(source)[Symbol.iterator]();
     try {
         do {
             ({
                 done,
                 value: buffer
-            } = Number.isNaN(size - bufferLength) ? it.next() : it.next(size - bufferLength));
+            } = Number.isNaN(size - bufferLength) ? it2.next() : it2.next(size - bufferLength));
             if (!done && buffer.byteLength > 0) {
                 buffers.push(buffer);
                 bufferLength += buffer.byteLength;
             }
             if (done || size <= bufferLength) {
                 do {
                     ({
                         cmd,
                         size
                     } = yield byteRange());
                 } while (size < bufferLength);
             }
         } while (!done);
     } catch (e) {
-        (threw = true) && typeof it.throw === "function" && it.throw(e);
+        (threw = true) && typeof it2.throw === "function" && it2.throw(e);
     } finally {
-        threw === false && typeof it.return === "function" && it.return(null);
+        threw === false && typeof it2.return === "function" && it2.return(null);
     }
     return null;
 }
 
 function fromAsyncIterable(source) {
     return __asyncGenerator(this, arguments, function* fromAsyncIterable_1() {
         let done, threw = false;
@@ -70025,38 +70141,38 @@
             [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);
             return buffer;
         }
         ({
             cmd,
             size
         } = yield yield __await(null));
-        const it = toUint8ArrayAsyncIterator(source)[Symbol.asyncIterator]();
+        const it2 = toUint8ArrayAsyncIterator(source)[Symbol.asyncIterator]();
         try {
             do {
                 ({
                     done,
                     value: buffer
-                } = Number.isNaN(size - bufferLength) ? yield __await(it.next()): yield __await(it.next(size - bufferLength)));
+                } = Number.isNaN(size - bufferLength) ? yield __await(it2.next()): yield __await(it2.next(size - bufferLength)));
                 if (!done && buffer.byteLength > 0) {
                     buffers.push(buffer);
                     bufferLength += buffer.byteLength;
                 }
                 if (done || size <= bufferLength) {
                     do {
                         ({
                             cmd,
                             size
                         } = yield yield __await(byteRange()));
                     } while (size < bufferLength);
                 }
             } while (!done);
         } catch (e) {
-            (threw = true) && typeof it.throw === "function" && (yield __await(it.throw(e)));
+            (threw = true) && typeof it2.throw === "function" && (yield __await(it2.throw(e)));
         } finally {
-            threw === false && typeof it.return === "function" && (yield __await(it.return(new Uint8Array(0))));
+            threw === false && typeof it2.return === "function" && (yield __await(it2.return(new Uint8Array(0))));
         }
         return yield __await(null);
     });
 }
 
 function fromDOMStream(source) {
     return __asyncGenerator(this, arguments, function* fromDOMStream_1() {
@@ -70073,38 +70189,38 @@
             [buffer, buffers, bufferLength] = joinUint8Arrays(buffers, size);
             return buffer;
         }
         ({
             cmd,
             size
         } = yield yield __await(null));
-        const it = new AdaptiveByteReader(source);
+        const it2 = new AdaptiveByteReader(source);
         try {
             do {
                 ({
                     done,
                     value: buffer
-                } = Number.isNaN(size - bufferLength) ? yield __await(it["read"]()): yield __await(it["read"](size - bufferLength)));
+                } = Number.isNaN(size - bufferLength) ? yield __await(it2["read"]()): yield __await(it2["read"](size - bufferLength)));
                 if (!done && buffer.byteLength > 0) {
                     buffers.push(toUint8Array(buffer));
                     bufferLength += buffer.byteLength;
                 }
                 if (done || size <= bufferLength) {
                     do {
                         ({
                             cmd,
                             size
                         } = yield yield __await(byteRange()));
                     } while (size < bufferLength);
                 }
             } while (!done);
         } catch (e) {
-            (threw = true) && (yield __await(it["cancel"](e)));
+            (threw = true) && (yield __await(it2["cancel"](e)));
         } finally {
-            threw === false ? yield __await(it["cancel"]()): source["locked"] && it.releaseLock();
+            threw === false ? yield __await(it2["cancel"]()): source["locked"] && it2.releaseLock();
         }
         return yield __await(null);
     });
 }
 var AdaptiveByteReader = class {
     constructor(source) {
         this.source = source;
@@ -74338,16 +74454,16 @@
      */
     position() {
         return this.position_;
     }
     /**
      * Set the buffer's position.
      */
-    setPosition(position3) {
-        this.position_ = position3;
+    setPosition(position5) {
+        this.position_ = position5;
     }
     /**
      * Get the buffer's capacity.
      */
     capacity() {
         return this.bytes_.length;
     }
@@ -76922,44 +77038,44 @@
 var RandomAccessFile = class extends ByteStream {
     constructor(buffer, byteLength) {
         super();
         this.position = 0;
         this.buffer = toUint8Array(buffer);
         this.size = typeof byteLength === "undefined" ? this.buffer.byteLength : byteLength;
     }
-    readInt32(position3) {
+    readInt32(position5) {
         const {
             buffer,
             byteOffset
-        } = this.readAt(position3, 4);
+        } = this.readAt(position5, 4);
         return new DataView(buffer, byteOffset).getInt32(0, true);
     }
-    seek(position3) {
-        this.position = Math.min(position3, this.size);
-        return position3 < this.size;
+    seek(position5) {
+        this.position = Math.min(position5, this.size);
+        return position5 < this.size;
     }
     read(nBytes) {
         const {
             buffer,
             size,
-            position: position3
+            position: position5
         } = this;
-        if (buffer && position3 < size) {
+        if (buffer && position5 < size) {
             if (typeof nBytes !== "number") {
                 nBytes = Number.POSITIVE_INFINITY;
             }
-            this.position = Math.min(size, position3 + Math.min(size - position3, nBytes));
-            return buffer.subarray(position3, this.position);
+            this.position = Math.min(size, position5 + Math.min(size - position5, nBytes));
+            return buffer.subarray(position5, this.position);
         }
         return null;
     }
-    readAt(position3, nBytes) {
+    readAt(position5, nBytes) {
         const buf = this.buffer;
-        const end = Math.min(this.size, position3 + nBytes);
-        return buf ? buf.subarray(position3, end) : new Uint8Array(nBytes);
+        const end = Math.min(this.size, position5 + nBytes);
+        return buf ? buf.subarray(position5, end) : new Uint8Array(nBytes);
     }
     close() {
         this.buffer && (this.buffer = null);
     }
     throw (value) {
         this.close();
         return {
@@ -76985,68 +77101,68 @@
         } else {
             this._pending = (() => __awaiter(this, void 0, void 0, function*() {
                 this.size = (yield file.stat()).size;
                 delete this._pending;
             }))();
         }
     }
-    readInt32(position3) {
+    readInt32(position5) {
         return __awaiter(this, void 0, void 0, function*() {
             const {
                 buffer,
                 byteOffset
-            } = yield this.readAt(position3, 4);
+            } = yield this.readAt(position5, 4);
             return new DataView(buffer, byteOffset).getInt32(0, true);
         });
     }
-    seek(position3) {
+    seek(position5) {
         return __awaiter(this, void 0, void 0, function*() {
             this._pending && (yield this._pending);
-            this.position = Math.min(position3, this.size);
-            return position3 < this.size;
+            this.position = Math.min(position5, this.size);
+            return position5 < this.size;
         });
     }
     read(nBytes) {
         return __awaiter(this, void 0, void 0, function*() {
             this._pending && (yield this._pending);
             const {
                 _handle: file,
                 size,
-                position: position3
+                position: position5
             } = this;
-            if (file && position3 < size) {
+            if (file && position5 < size) {
                 if (typeof nBytes !== "number") {
                     nBytes = Number.POSITIVE_INFINITY;
                 }
-                let pos = position3,
+                let pos = position5,
                     offset3 = 0,
                     bytesRead = 0;
                 const end = Math.min(size, pos + Math.min(size - pos, nBytes));
                 const buffer = new Uint8Array(Math.max(0, (this.position = end) - pos));
                 while ((pos += bytesRead) < end && (offset3 += bytesRead) < buffer.byteLength) {
                     ({
                         bytesRead
                     } = yield file.read(buffer, offset3, buffer.byteLength - offset3, pos));
                 }
                 return buffer;
             }
             return null;
         });
     }
-    readAt(position3, nBytes) {
+    readAt(position5, nBytes) {
         return __awaiter(this, void 0, void 0, function*() {
             this._pending && (yield this._pending);
             const {
                 _handle: file,
                 size
             } = this;
-            if (file && position3 + nBytes < size) {
-                const end = Math.min(size, position3 + nBytes);
-                const buffer = new Uint8Array(end - position3);
-                return (yield file.read(buffer, 0, nBytes, position3)).buffer;
+            if (file && position5 + nBytes < size) {
+                const end = Math.min(size, position5 + nBytes);
+                const buffer = new Uint8Array(end - position5);
+                return (yield file.read(buffer, 0, nBytes, position5)).buffer;
             }
             return new Uint8Array(nBytes);
         });
     }
     close() {
         return __awaiter(this, void 0, void 0, function*() {
             const f = this._handle;
@@ -81655,79 +81771,79 @@
     if (isIterable3(source)) {
         return iterableAsReadableDOMStream(source, options);
     }
     throw new Error(`toDOMStream() must be called with an Iterable or AsyncIterable`);
 }
 
 function iterableAsReadableDOMStream(source, options) {
-    let it = null;
+    let it2 = null;
     const bm = (options === null || options === void 0 ? void 0 : options.type) === "bytes" || false;
     const hwm = (options === null || options === void 0 ? void 0 : options.highWaterMark) || Math.pow(2, 24);
     return new ReadableStream(Object.assign(Object.assign({}, options), {
         start(controller) {
-            next(controller, it || (it = source[Symbol.iterator]()));
+            next(controller, it2 || (it2 = source[Symbol.iterator]()));
         },
         pull(controller) {
-            it ? next(controller, it) : controller.close();
+            it2 ? next(controller, it2) : controller.close();
         },
         cancel() {
-            ((it === null || it === void 0 ? void 0 : it.return) && it.return() || true) && (it = null);
+            ((it2 === null || it2 === void 0 ? void 0 : it2.return) && it2.return() || true) && (it2 = null);
         }
     }), Object.assign({
         highWaterMark: bm ? hwm : void 0
     }, options));
 
-    function next(controller, it2) {
+    function next(controller, it3) {
         let buf;
         let r = null;
         let size = controller.desiredSize || null;
-        while (!(r = it2.next(bm ? size : null)).done) {
+        while (!(r = it3.next(bm ? size : null)).done) {
             if (ArrayBuffer.isView(r.value) && (buf = toUint8Array(r.value))) {
                 size != null && bm && (size = size - buf.byteLength + 1);
                 r.value = buf;
             }
             controller.enqueue(r.value);
             if (size != null && --size <= 0) {
                 return;
             }
         }
         controller.close();
     }
 }
 
 function asyncIterableAsReadableDOMStream(source, options) {
-    let it = null;
+    let it2 = null;
     const bm = (options === null || options === void 0 ? void 0 : options.type) === "bytes" || false;
     const hwm = (options === null || options === void 0 ? void 0 : options.highWaterMark) || Math.pow(2, 24);
     return new ReadableStream(Object.assign(Object.assign({}, options), {
         start(controller) {
             return __awaiter(this, void 0, void 0, function*() {
-                yield next(controller, it || (it = source[Symbol.asyncIterator]()));
+                yield next(controller, it2 || (it2 = source[Symbol.asyncIterator]()));
             });
         },
         pull(controller) {
             return __awaiter(this, void 0, void 0, function*() {
-                it ? yield next(controller, it): controller.close();
+                it2 ? yield next(controller, it2): controller.close();
             });
         },
         cancel() {
             return __awaiter(this, void 0, void 0, function*() {
-                ((it === null || it === void 0 ? void 0 : it.return) && (yield it.return()) || true) && (it = null);
+                ((it2 === null || it2 === void 0 ? void 0 : it2.return) && (yield it2.return()) || true) && (it2 = null);
             });
         }
     }), Object.assign({
         highWaterMark: bm ? hwm : void 0
     }, options));
 
-    function next(controller, it2) {
+    function next(controller, it3) {
         return __awaiter(this, void 0, void 0, function*() {
             let buf;
             let r = null;
             let size = controller.desiredSize || null;
-            while (!(r = yield it2.next(bm ? size : null)).done) {
+            while (!(r = yield it3.next(bm ? size : null)).done) {
                 if (ArrayBuffer.isView(r.value) && (buf = toUint8Array(r.value))) {
                     size != null && bm && (size = size - buf.byteLength + 1);
                     r.value = buf;
                 }
                 controller.enqueue(r.value);
                 if (size != null && --size <= 0) {
                     return;
```

### Comparing `pyobsplot-0.3.3/src/pyobsplot/utils.py` & `pyobsplot-0.3.4/src/pyobsplot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pathlib
 
 # Output directory of esbuild
 bundler_output_dir = pathlib.Path(__file__).parent / "static"
 
 # Minimum npm package version
-min_npm_version = "0.3.3"
+min_npm_version = "0.3.4"
 
 # Allowed default values
 allowed_defaults = [
     "marginTop",
     "marginRight",
     "marginBottom",
     "marginLeft",
@@ -100,14 +100,15 @@
     "groupZ",
     "hexagon",
     "hexbin",
     "hexgrid",
     "hull",
     "identity",
     "image",
+    "indexOf",
     "initializer",
     "interpolateNearest",
     "interpolateNone",
     "interpolatorBarycentric",
     "interpolatorRandomWalk",
     "legend",
     "line",
```

### Comparing `pyobsplot-0.3.3/src/pyobsplot/widget.py` & `pyobsplot-0.3.4/src/pyobsplot/widget.py`

 * *Files identical despite different names*

### Comparing `pyobsplot-0.3.3/PKG-INFO` & `pyobsplot-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobsplot
-Version: 0.3.3
+Version: 0.3.4
 Summary: Observable Plot in Jupyter notebooks and Quarto documents
 Home-page: https://github.com/juba/pyobsplot
 License: MIT
 Author: Julien Barnier
 Author-email: julien@nozav.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Dist: anywidget[dev] (>=0.2.2,<0.3.0)
+Requires-Dist: anywidget[dev] (>=0.2.3,<0.3.0)
 Requires-Dist: ipywidgets (>=8.0.0)
 Requires-Dist: jupyterlab (>=3.6.0)
 Requires-Dist: jupyterlab_widgets (>=3.0.0)
 Requires-Dist: pandas (>=1.2.0)
 Requires-Dist: polars (>=0.16.0)
 Requires-Dist: pyarrow (>=11.0.0,<12.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
```

