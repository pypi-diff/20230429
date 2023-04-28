# Comparing `tmp/nbdefense_jupyter-1.0.3.tar.gz` & `tmp/nbdefense_jupyter-1.0.4.tar.gz`

## Comparing `nbdefense_jupyter-1.0.3.tar` & `nbdefense_jupyter-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/_version.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/handlers.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/package.json
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig
--rw-r--r--   0        0        0    16110 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json
--rw-r--r--   0        0        0    51556 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/117.e6844c28c0311e09d7d5.js
--rw-r--r--   0        0        0    13996 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/355.e71f4acc9570680d68e9.js
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js.LICENSE.txt
--rw-r--r--   0        0        0   157457 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js.LICENSE.txt
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/654.0b96d4d60115144c75b2.js
--rw-r--r--   0        0        0    18496 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js
--rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/remoteEntry.a4d194721ddf3be27f37.js
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/style.js
--rw-r--r--   0        0        0    12463 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/.gitignore
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/LICENSE
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/README.md
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/pyproject.toml
--rw-r--r--   0        0        0    15877 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/_version.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/handlers.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/package.json
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig
+-rw-r--r--   0        0        0    16110 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json
+-rw-r--r--   0        0        0    13996 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/355.e71f4acc9570680d68e9.js
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js.LICENSE.txt
+-rw-r--r--   0        0        0   157457 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js.LICENSE.txt
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/654.0b96d4d60115144c75b2.js
+-rw-r--r--   0        0        0    52121 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/661.42dcb7cf7c20838bfd42.js
+-rw-r--r--   0        0        0    18496 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/remoteEntry.52422cb5d5bada194ec0.js
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/style.js
+-rw-r--r--   0        0        0    12463 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/.gitignore
+-rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/LICENSE
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/README.md
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0    15877 2020-02-02 00:00:00.000000 nbdefense_jupyter-1.0.4/PKG-INFO
```

### Comparing `nbdefense_jupyter-1.0.3/package.json` & `nbdefense_jupyter-1.0.4/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.4'"}*

```diff
@@ -139,9 +139,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/__init__.py` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/handlers.py` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/handlers.py`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/package.json` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9758597883597885%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.52422cb5d5bada194ec0.js'}}",*

 * * "'version'": "'1.0.4'"}*

```diff
@@ -68,15 +68,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a4d194721ddf3be27f37.js",
+            "load": "static/remoteEntry.52422cb5d5bada194ec0.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "nbdefense_jupyter"
                 },
@@ -144,9 +144,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'1.0.4'"}*

```diff
@@ -139,9 +139,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/schemas/nbdefense-jupyter/plugin.json`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/117.e6844c28c0311e09d7d5.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/661.42dcb7cf7c20838bfd42.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 "use strict";
 (self.webpackChunknbdefense_jupyter = self.webpackChunknbdefense_jupyter || []).push([
-    [117], {
-        117: (e, t, n) => {
+    [661], {
+        661: (e, t, n) => {
             n.r(t), n.d(t, {
-                PLUGIN_ID: () => Re,
-                default: () => Ae
+                PLUGIN_ID: () => je,
+                default: () => We
             });
             var s = n(687),
                 o = n(123),
                 a = n(38),
                 r = n(923),
                 i = n(33);
             class l {
@@ -30,15 +30,15 @@
                 }
             }
             var c = n(502);
             const d = "isContextualHelpVisible",
                 p = "isNBDefenseDropdownVisible",
                 h = "https://github.com/protectai/nbdefense-jupyter/issues/new",
                 u = "nbdefense-jupyter issues";
-            class C {
+            class g {
                 constructor(e, t, n) {
                     this.nbdefenseWidget = e, this.shell = t, this.settings = n
                 }
                 createNew(e, t) {
                     this.settings.changed.connect((() => {
                         n.value = this.settings.get(d).composite || !1, s.value = this.settings.get(p).composite || !1
                     }));
@@ -50,15 +50,15 @@
                     return s.label = "NB Defense Dropdowns", s.value = this.settings.get(p).composite || !1, s.addClass("nbdefense-toolbar-switch"), s.handleEvent = e => {
                         "click" === e.type && (s.value = !s.value, this.settings.set(p, s.value), this.nbdefenseWidget.setNBDefenseDropdownVisible(s.value))
                     }, e.toolbar.insertItem(11, "ShowContextualHelp", n), e.toolbar.insertItem(12, "showNBDefenseDropdows", s), new r.DisposableDelegate((() => {
                         n.dispose(), s.dispose()
                     }))
                 }
             }
-            const g = new c.LabIcon({
+            const C = new c.LabIcon({
                     name: "nbdefense",
                     svgstr: '<svg width="28" height="28" viewBox="0 0 28 28" fill="none" xmlns="http://www.w3.org/2000/svg">\n  <path fill-rule="evenodd" clip-rule="evenodd"\n    d="M24.5 0H0V24.5C0 26.433 1.567 28 3.5 28H20.125L28 20.125V3.5C28 1.567 26.433 0 24.5 0Z"\n    fill="#705FEB" />\n  <path\n    d="M13.346 8.214H11.456V14.654L6.15 8.214H3.56V8.452C4.246 8.69 4.344 9.376 4.344 10.468V18H6.234V11.42L11.638 18H13.346V8.214ZM24.6028 13.114C24.6028 10.748 22.8808 8.214 19.3388 8.214H14.9848V8.452C15.6708 8.69 15.7688 9.376 15.7688 10.468V18H19.3388C22.8808 18 24.6028 15.466 24.6028 13.114ZM22.4328 13.114C22.4328 14.682 21.5368 16.488 18.8768 16.488H17.7428V9.698H18.8768C21.5368 9.698 22.4328 11.546 22.4328 13.114Z"\n    fill="white" />\n</svg>'
                 }),
                 m = new c.LabIcon({
                     name: "loading",
                     svgstr: '<svg width="16" height="16" viewBox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_205_6521)">\n<path d="M16 7.99998C16 12.4183 12.4183 16 8 16C3.58173 16 0 12.4183 0 7.99998C0 3.58172 3.58173 0 8 0C12.4183 0 16 3.58172 16 7.99998ZM1.45303 7.99998C1.45303 11.6158 4.38421 14.5469 8 14.5469C11.6158 14.5469 14.547 11.6158 14.547 7.99998C14.547 4.3842 11.6158 1.45303 8 1.45303C4.38421 1.45303 1.45303 4.3842 1.45303 7.99998Z" fill="#081E2E"/>\n<path d="M14.9706 6.0911C15.3614 5.99018 15.5982 5.59537 15.4605 5.22187C15.1842 4.47238 14.7939 3.76687 14.3017 3.12985C13.6617 2.30153 12.862 1.60522 11.9483 1.08072C11.0345 0.556217 10.0247 0.213771 8.97632 0.0729379C8.17007 -0.0353709 7.35322 -0.0228082 6.55344 0.108976C6.15489 0.174647 5.92151 0.5714 6.02417 0.955634C6.12685 1.33987 6.52683 1.56529 6.92665 1.50753C7.53911 1.41905 8.16242 1.41562 8.77817 1.49834C9.63612 1.61359 10.4626 1.89384 11.2103 2.32307C11.9581 2.75231 12.6126 3.32215 13.1363 4.00003C13.5122 4.48654 13.8155 5.02186 14.0381 5.5897C14.1835 5.96039 14.5797 6.19204 14.9706 6.0911Z" fill="white"/>\n<animateTransform\n         attributeName="transform" \n         attributeType="XML" \n         type="rotate"\n         dur="1s"\n         from="0 8 8"\n         to="360 8 8"\n         repeatCount="indefinite" />\n</g>\n<defs>\n<clipPath id="clip0_205_6521">\n<rect width="16" height="16" fill="white"/>\n</clipPath>\n</defs>\n</svg>\n'
                 }),
@@ -85,86 +85,89 @@
                 L = new c.LabIcon({
                     name: "header background",
                     svgstr: '<svg width="250" height="62" viewBox="0 0 250 62" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_218_7497)">\n<mask id="mask0_218_7497" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="136" y="-66" width="153" height="153">\n<rect x="136.211" y="-5.71155" width="85.1108" height="129.901" transform="rotate(-45 136.211 -5.71155)" fill="url(#paint0_radial_218_7497)"/>\n</mask>\n<g mask="url(#mask0_218_7497)">\n<g opacity="0.4">\n<path opacity="0.3" d="M250.247 -7.13594L202.864 -54.5198M240.251 2.86066L192.867 -44.5232M230.254 12.8573L182.87 -34.5266M220.058 22.8539L172.674 -24.53M209.961 32.7505L162.577 -14.6334M199.865 42.6471L152.481 -4.73676" stroke="#334155" stroke-width="4"/>\n<path d="M145.271 -11.9468L145.929 -11.2883C146.753 -10.4638 147.769 -9.85558 148.885 -9.51767C150.001 -9.17976 151.183 -9.1226 152.326 -9.35126L161.587 -11.2033C162.73 -11.432 163.912 -11.3748 165.028 -11.0369C166.144 -10.699 167.159 -10.0908 167.984 -9.26629L168.642 -8.60781M194.727 37.5101L195.386 38.1687C196.21 38.9932 197.226 39.6013 198.342 39.9392C199.458 40.2771 200.64 40.3343 201.783 40.1056L211.044 38.2535C212.187 38.0249 213.369 38.0821 214.485 38.42C215.601 38.7579 216.616 39.3661 217.441 40.1906L218.099 40.8491M191.597 14.3468L192.256 15.0052C193.08 15.8298 194.096 16.438 195.212 16.7758C196.328 17.1137 197.51 17.1709 198.653 16.9422L207.913 15.0901C209.057 14.8614 210.239 14.9186 211.355 15.2564C212.471 15.5943 213.486 16.2025 214.311 17.0271L214.969 17.6856M180.955 -36.3624L181.613 -35.7038C182.438 -34.8793 183.453 -34.2711 184.569 -33.9332C185.685 -33.5953 186.867 -33.5382 188.01 -33.7668L197.271 -35.6189C198.414 -35.8476 199.596 -35.7905 200.712 -35.4526C201.828 -35.1147 202.844 -34.5065 203.668 -33.682L204.327 -33.0235M230.203 12.8861L230.861 13.5445C231.686 14.369 232.294 15.3843 232.632 16.5003C232.97 17.6163 233.027 18.7985 232.798 19.9419L230.946 29.2022C230.718 30.3456 230.775 31.5277 231.113 32.6437C231.451 33.7597 232.059 34.775 232.883 35.5995L233.542 36.2581" stroke="#334155" stroke-width="4"/>\n<path d="M230.203 12.886L230.861 13.5445C231.686 14.369 232.294 15.3843 232.632 16.5003C232.97 17.6163 233.027 18.7985 232.799 19.9418L230.946 29.2022C230.718 30.3456 230.775 31.5277 231.113 32.6437C231.451 33.7597 232.059 34.775 232.883 35.5995L233.542 36.2581M222.69 -14.6597L223.349 -14.0012C224.173 -13.1767 224.782 -12.1614 225.12 -11.0454C225.457 -9.92935 225.515 -8.74717 225.286 -7.60378L223.434 1.65656C223.205 2.79995 223.262 3.98211 223.6 5.0981C223.938 6.21409 224.546 7.22939 225.371 8.05389L226.029 8.71236M250.445 13.0947L251.103 13.7531C251.928 14.5777 252.536 15.593 252.874 16.709C253.212 17.825 253.269 19.0072 253.04 20.1506L251.188 29.4109C250.959 30.5543 251.017 31.7365 251.355 32.8525C251.692 33.9685 252.301 34.9838 253.125 35.8082L253.783 36.4662M239.593 -17.79L243.591 -13.7926C244.415 -12.9681 245.024 -11.9528 245.361 -10.8368C245.699 -9.72077 245.756 -8.53862 245.528 -7.39525L243.676 1.8651C243.447 3.00849 243.504 4.19063 243.842 5.30662C244.18 6.42261 244.788 7.43791 245.613 8.26242L246.271 8.92089M237.715 40.4317L238.374 41.0902C239.198 41.9147 239.806 42.93 240.144 44.046C240.482 45.162 240.539 46.3441 240.311 47.4875L238.458 56.7474C238.23 57.8909 238.287 59.0731 238.625 60.1891C238.963 61.3052 239.571 62.3206 240.396 63.1452L241.054 63.804M180.955 -36.3623C182.949 -34.3684 185.995 -33.8739 188.517 -35.1351L206.781 -44.2672C209.303 -45.5283 212.349 -45.0339 214.343 -43.04M179.494 2.24337L182.562 5.31132C184.718 7.46699 188.011 8.0014 190.738 6.63807L208.659 -2.32268C211.181 -3.58375 214.228 -3.08942 216.221 -1.0955M133.376 -23.8415C135.327 -21.8906 138.371 -21.5564 140.698 -23.0376L169.459 -41.3396C171.786 -42.8207 174.83 -42.4867 176.781 -40.5358M169.477 12.26L163.634 6.41695M187.424 10.1733L172.816 -4.43426M250.027 52.7437L237.715 40.4316M159.461 2.24337L145.271 -11.9468M141.097 -16.1205L133.376 -23.8416M129.202 -28.0151L123.151 -34.0668M216.221 -1.0955L180.955 -36.3623M246.271 8.92089L222.691 -14.6598M280.077 22.6939L239.593 -17.7898M218.726 -18.6246L208.5 -28.8498M235.42 -21.9634L218.517 -38.8663M226.029 8.71236L220.395 3.07808M260.044 42.7271L257.957 40.6398M253.783 36.4662L230.203 12.8859M233.542 36.2581L219.143 21.8592M239.802 62.5514L222.273 45.0226M229.994 72.7769L194.727 37.5101M190.554 33.3366L173.651 16.4335" stroke="#334155" stroke-width="4"/>\n<path d="M160.504 3.28676C159.928 3.86303 159.928 4.79737 160.504 5.37364C161.08 5.94992 162.015 5.94992 162.591 5.37365C163.167 4.79737 163.167 3.86303 162.591 3.28675C162.015 2.71047 161.08 2.71048 160.504 3.28676Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M188.467 11.2166C187.891 11.7929 187.891 12.7272 188.467 13.3035C189.043 13.8798 189.978 13.8798 190.554 13.3035C191.13 12.7272 191.13 11.7929 190.554 11.2166C189.978 10.6403 189.043 10.6404 188.467 11.2166Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M217.265 -0.0521685C216.688 0.52411 216.688 1.45844 217.265 2.03472C217.841 2.611 218.775 2.611 219.352 2.03472C219.928 1.45844 219.928 0.524107 219.352 -0.0521716C218.775 -0.62845 217.841 -0.628447 217.265 -0.0521685Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M227.073 9.75575C226.496 10.332 226.496 11.2664 227.073 11.8426C227.649 12.4189 228.583 12.4189 229.159 11.8426C229.736 11.2664 229.736 10.332 229.159 9.75575C228.583 9.17947 227.649 9.17948 227.073 9.75575Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M234.585 37.3015C234.009 37.8777 234.009 38.8121 234.585 39.3884C235.162 39.9646 236.096 39.9646 236.672 39.3884C237.248 38.8121 237.248 37.8777 236.672 37.3015C236.096 36.7252 235.162 36.7252 234.585 37.3015Z" stroke="#334155" stroke-width="4"/>\n<path d="M219.143 41.8924C218.567 42.4687 218.567 43.403 219.143 43.9793C219.719 44.5556 220.653 44.5556 221.23 43.9793C221.806 43.403 221.806 42.4687 221.23 41.8924C220.653 41.3161 219.719 41.3161 219.143 41.8924Z" stroke="#334155" stroke-width="4"/>\n<path d="M216.013 18.729C215.436 19.3052 215.436 20.2396 216.013 20.8158C216.589 21.3921 217.523 21.3921 218.1 20.8158C218.676 20.2396 218.676 19.3052 218.1 18.729C217.523 18.1527 216.589 18.1527 216.013 18.729Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M191.597 34.38C191.021 34.9562 191.021 35.8906 191.597 36.4668C192.173 37.0431 193.108 37.0431 193.684 36.4668C194.26 35.8906 194.26 34.9562 193.684 34.38C193.108 33.8037 192.173 33.8037 191.597 34.38Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M170.521 13.3033C169.945 13.8796 169.945 14.8139 170.521 15.3902C171.097 15.9665 172.031 15.9665 172.608 15.3902C173.184 14.8139 173.184 13.8796 172.608 13.3033C172.031 12.727 171.097 12.727 170.521 13.3033Z" fill="#0EA5E9" fill-opacity="0.42" stroke="#0EA5E9" stroke-width="4"/>\n<path d="M247.314 9.96424C246.738 10.5405 246.738 11.4749 247.314 12.0511C247.891 12.6274 248.825 12.6274 249.401 12.0511C249.978 11.4749 249.978 10.5405 249.401 9.96425C248.825 9.38797 247.891 9.38796 247.314 9.96424Z" stroke="#334155" stroke-width="4"/>\n</g>\n</g>\n</g>\n<g clip-path="url(#clip1_218_7497)">\n<mask id="mask1_218_7497" style="mask-type:alpha" maskUnits="userSpaceOnUse" x="-22" y="-7" width="153" height="153">\n<rect x="-21.7888" y="53.2885" width="85.1108" height="129.901" transform="rotate(-45 -21.7888 53.2885)" fill="url(#paint1_radial_218_7497)"/>\n</mask>\n<g mask="url(#mask1_218_7497)">\n<g opacity="0.4">\n<path opacity="0.3" d="M92.2474 51.8641L44.8636 4.48019M82.2508 61.8607L34.867 14.4768M72.2542 71.8573L24.8704 24.4734M62.0577 81.8539L14.6738 34.47M51.9611 91.7505L4.57728 44.3666M41.8646 101.647L-5.51929 54.2632" stroke="#334155" stroke-width="4"/>\n<path d="M-12.7295 47.0532L-12.071 47.7117C-11.2465 48.5362 -10.2312 49.1444 -9.11523 49.4823C-7.99923 49.8202 -6.81708 49.8774 -5.67369 49.6487L3.58665 47.7967C4.73004 47.568 5.91219 47.6252 7.02818 47.9631C8.14416 48.301 9.15947 48.9092 9.98398 49.7337L10.6425 50.3922M36.7274 96.5101L37.3859 97.1687C38.2104 97.9932 39.2257 98.6013 40.3417 98.9392C41.4577 99.2771 42.6398 99.3343 43.7832 99.1056L53.0435 97.2535C54.1869 97.0249 55.3691 97.0821 56.485 97.42C57.601 97.7579 58.6163 98.3661 59.4408 99.1906L60.0993 99.8491M33.5972 73.3468L34.2557 74.0052C35.0802 74.8298 36.0956 75.438 37.2116 75.7758C38.3276 76.1137 39.5097 76.1709 40.6531 75.9422L49.9135 74.0901C51.0568 73.8614 52.239 73.9186 53.355 74.2564C54.4709 74.5943 55.4862 75.2025 56.3107 76.0271L56.9693 76.6856M22.9547 22.6376L23.6132 23.2962C24.4377 24.1207 25.453 24.7289 26.569 25.0668C27.685 25.4047 28.8671 25.4618 30.0105 25.2332L39.2708 23.3811C40.4142 23.1524 41.5964 23.2095 42.7124 23.5474C43.8284 23.8853 44.8437 24.4935 45.6682 25.318L46.3267 25.9765M72.2029 71.8861L72.8614 72.5445C73.6859 73.369 74.2941 74.3843 74.632 75.5003C74.9699 76.6163 75.0271 77.7985 74.7984 78.9419L72.9463 88.2022C72.7176 89.3456 72.7748 90.5277 73.1126 91.6437C73.4505 92.7597 74.0587 93.775 74.8832 94.5995L75.5418 95.2581" stroke="#334155" stroke-width="4"/>\n<path d="M72.203 71.886L72.8615 72.5445C73.686 73.369 74.2942 74.3843 74.6321 75.5003C74.97 76.6163 75.0272 77.7985 74.7985 78.9418L72.9464 88.2022C72.7177 89.3456 72.7749 90.5277 73.1127 91.6437C73.4506 92.7597 74.0588 93.775 74.8833 94.5995L75.5419 95.2581M64.6904 44.3403L65.3489 44.9988C66.1734 45.8233 66.7816 46.8386 67.1195 47.9546C67.4574 49.0707 67.5146 50.2528 67.2859 51.3962L65.4338 60.6566C65.2051 61.8 65.2623 62.9821 65.6002 64.0981C65.9381 65.2141 66.5463 66.2294 67.3708 67.0539L68.0293 67.7124M92.4448 72.0947L93.1033 72.7531C93.9278 73.5777 94.536 74.593 94.8739 75.709C95.2118 76.825 95.2689 78.0072 95.0402 79.1506L93.1881 88.4109C92.9595 89.5543 93.0166 90.7365 93.3545 91.8525C93.6924 92.9685 94.3007 93.9838 95.1252 94.8082L95.7832 95.4662M81.5935 41.21L85.5909 45.2074C86.4154 46.0319 87.0236 47.0472 87.3615 48.1632C87.6994 49.2792 87.7565 50.4614 87.5278 51.6048L85.6757 60.8651C85.4471 62.0085 85.5042 63.1906 85.8422 64.3066C86.1801 65.4226 86.7883 66.4379 87.6127 67.2624L88.2712 67.9209M79.7152 99.4317L80.3738 100.09C81.1983 100.915 81.8065 101.93 82.1444 103.046C82.4823 104.162 82.5394 105.344 82.3107 106.487L80.4583 115.747C80.2298 116.891 80.2871 118.073 80.6251 119.189C80.963 120.305 81.5712 121.321 82.3956 122.145L83.0544 122.804M22.9547 22.6377C24.9486 24.6316 27.9947 25.1261 30.5169 23.8649L48.7811 14.7328C51.3033 13.4717 54.3494 13.9661 56.3433 15.96M21.494 61.2434L24.5619 64.3113C26.7176 66.467 30.0109 67.0014 32.7377 65.6381L50.6592 56.6773C53.1813 55.4163 56.2275 55.9106 58.2215 57.9045M-24.624 35.1585C-22.6732 37.1094 -19.6291 37.4436 -17.3016 35.9624L11.4586 17.6604C13.7862 16.1793 16.8302 16.5133 18.7812 18.4642M11.4774 71.26L5.63435 65.4169M29.4237 69.1733L14.8161 54.5657M92.0274 111.744L79.7153 99.4316M1.46077 61.2434L-12.7294 47.0532M-16.9031 42.8795L-24.6241 35.1584M-28.7977 30.9849L-34.8494 24.9332M58.2215 57.9045L22.9547 22.6377M88.2712 67.9209L64.6905 44.3402M122.077 81.6939L81.5935 41.2102M60.7257 40.3754L50.5005 30.1502M77.4199 37.0366L60.517 20.1337M68.0293 67.7124L62.395 62.0781M102.044 101.727L99.9567 99.6398M95.7832 95.4662L72.2029 71.8859M75.5419 95.2581L61.143 80.8592M81.8018 121.551L64.273 104.023M71.9943 131.777L36.7275 96.5101M32.554 92.3366L15.6509 75.4335" stroke="#334155" stroke-width="4"/>\n<path d="M2.50419 62.2868C1.92791 62.863 1.92791 63.7974 2.50418 64.3736C3.08046 64.9499 4.0148 64.9499 4.59108 64.3736C5.16735 63.7974 5.16735 62.863 4.59107 62.2868C4.0148 61.7105 3.08046 61.7105 2.50419 62.2868Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M11.6858 51.4355C11.1096 52.0118 11.1096 52.9461 11.6858 53.5224C12.2621 54.0987 13.1964 54.0987 13.7727 53.5224C14.349 52.9461 14.349 52.0118 13.7727 51.4355C13.1964 50.8592 12.2621 50.8592 11.6858 51.4355Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M59.2647 58.9478C58.6884 59.5241 58.6884 60.4584 59.2647 61.0347C59.841 61.611 60.7753 61.611 61.3516 61.0347C61.9279 60.4584 61.9279 59.5241 61.3516 58.9478C60.7753 58.3715 59.841 58.3716 59.2647 58.9478Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M61.5603 41.21C60.9841 41.7863 60.9841 42.7206 61.5603 43.2969C62.1366 43.8731 63.071 43.8731 63.6472 43.2969C64.2235 42.7206 64.2235 41.7863 63.6472 41.21C63.071 40.6337 62.1366 40.6337 61.5603 41.21Z" fill="#0EA5E9" fill-opacity="0.42" stroke="#0EA5E9" stroke-width="4"/>\n<path d="M47.3702 27.0198C46.7939 27.5961 46.7939 28.5305 47.3702 29.1067C47.9464 29.683 48.8808 29.683 49.457 29.1067C50.0333 28.5305 50.0333 27.5961 49.457 27.0198C48.8808 26.4436 47.9464 26.4436 47.3702 27.0198Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M57.3865 17.0034C56.8102 17.5796 56.8102 18.514 57.3865 19.0903C57.9628 19.6665 58.8971 19.6665 59.4734 19.0903C60.0497 18.514 60.0497 17.5796 59.4734 17.0034C58.8971 16.4271 57.9628 16.4271 57.3865 17.0034Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M78.4632 38.08C77.8869 38.6562 77.8869 39.5906 78.4632 40.1669C79.0395 40.7431 79.9738 40.7431 80.5501 40.1669C81.1263 39.5906 81.1263 38.6562 80.5501 38.08C79.9738 37.5037 79.0395 37.5037 78.4632 38.08Z" fill="#1E293B" stroke="#334155" stroke-width="4"/>\n<path d="M19.8245 19.5076C19.2482 20.0839 19.2482 21.0182 19.8245 21.5945C20.4008 22.1707 21.3351 22.1708 21.9114 21.5945C22.4877 21.0182 22.4877 20.0839 21.9114 19.5076C21.3351 18.9313 20.4008 18.9313 19.8245 19.5076Z" stroke="#334155" stroke-width="4"/>\n</g>\n</g>\n</g>\n<g clip-path="url(#clip2_218_7497)">\n<rect width="545" height="530" transform="translate(2 -204)" fill="url(#paint2_radial_218_7497)" fill-opacity="0.2"/>\n</g>\n<rect width="501" height="486" transform="translate(-236 -272)" fill="url(#paint3_radial_218_7497)" fill-opacity="0.2"/>\n<defs>\n<radialGradient id="paint0_radial_218_7497" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(178.767 59.2389) rotate(90) scale(64.9505 42.5554)">\n<stop/>\n<stop offset="1" stop-opacity="0"/>\n</radialGradient>\n<radialGradient id="paint1_radial_218_7497" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(20.7666 118.239) rotate(90) scale(64.9505 42.5554)">\n<stop/>\n<stop offset="1" stop-opacity="0"/>\n</radialGradient>\n<radialGradient id="paint2_radial_218_7497" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(272.5 265) rotate(90) scale(265 272.5)">\n<stop stop-color="#06BCD4"/>\n<stop offset="1" stop-color="#1E293B" stop-opacity="0"/>\n</radialGradient>\n<radialGradient id="paint3_radial_218_7497" cx="0" cy="0" r="1" gradientUnits="userSpaceOnUse" gradientTransform="translate(250.5 243) rotate(90) scale(243 250.5)">\n<stop stop-color="#6F5FEB"/>\n<stop offset="1" stop-color="#1E293B" stop-opacity="0"/>\n</radialGradient>\n<clipPath id="clip0_218_7497">\n<rect width="93.4477" height="145.756" fill="white" transform="translate(125 -16.9226) rotate(-45)"/>\n</clipPath>\n<clipPath id="clip1_218_7497">\n<rect width="93.4477" height="145.756" fill="white" transform="translate(-33 42.0774) rotate(-45)"/>\n</clipPath>\n<clipPath id="clip2_218_7497">\n<rect width="545" height="530" fill="white" transform="translate(2 -204)"/>\n</clipPath>\n</defs>\n</svg>\n'
                 }),
                 v = new c.LabIcon({
                     name: "jupyter notebook",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" viewBox="0 0 22 22" data-icon="ui-components:notebook" data-icon-id="56417dfc-94bc-41cb-a349-cd8623a68424"><g class="jp-icon-warn0 jp-icon-selectable" fill="#EF6C00"><path d="M18.7 3.3v15.4H3.3V3.3h15.4m1.5-1.5H1.8v18.3h18.3l.1-18.3z"></path><path d="M16.5 16.5l-5.4-4.3-5.6 4.3v-11h11z"></path></g></svg>'
+                }),
+                x = new c.LabIcon({
+                    name: "exclamation red",
+                    svgstr: '<svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_263_4733)">\n<path d="M10 1.66675C5.40002 1.66675 1.66669 5.40008 1.66669 10.0001C1.66669 14.6001 5.40002 18.3334 10 18.3334C14.6 18.3334 18.3334 14.6001 18.3334 10.0001C18.3334 5.40008 14.6 1.66675 10 1.66675ZM10.8334 14.1667H9.16669V12.5001H10.8334V14.1667ZM10.8334 10.8334H9.16669V5.83341H10.8334V10.8334Z" fill="#D92D20"/>\n</g>\n<defs>\n<clipPath id="clip0_263_4733">\n<rect width="20" height="20" fill="white"/>\n</clipPath>\n</defs>\n</svg>\n'
                 });
-            new c.LabIcon({
-                name: "exclamation red",
-                svgstr: '<svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">\n<g clip-path="url(#clip0_263_4733)">\n<path d="M10 1.66675C5.40002 1.66675 1.66669 5.40008 1.66669 10.0001C1.66669 14.6001 5.40002 18.3334 10 18.3334C14.6 18.3334 18.3334 14.6001 18.3334 10.0001C18.3334 5.40008 14.6 1.66675 10 1.66675ZM10.8334 14.1667H9.16669V12.5001H10.8334V14.1667ZM10.8334 10.8334H9.16669V5.83341H10.8334V10.8334Z" fill="#D92D20"/>\n</g>\n<defs>\n<clipPath id="clip0_263_4733">\n<rect width="20" height="20" fill="white"/>\n</clipPath>\n</defs>\n</svg>\n'
-            });
-            var x = n(271),
-                M = n.n(x),
-                _ = n(840),
-                y = n(161),
-                N = n.n(y),
-                P = n(554),
-                I = n.n(P),
-                S = n(470),
-                D = n.n(S),
-                O = n(142),
-                T = n(820),
+            var M = n(271),
+                _ = n.n(M),
+                y = n(840),
+                N = n(161),
+                P = n.n(N),
+                I = n(554),
+                S = n.n(I),
+                O = n(470),
+                D = n.n(O),
+                T = n(142),
+                R = n(820),
                 H = n(946);
-            const R = (0, H.zE)({
+            const A = (0, H.zE)({
                     header: {
                         marginBottom: 0
                     },
                     list: {
                         marginBlockStart: 0,
                         marginBlockEnd: 0,
                         paddingInlineStart: 0
                     }
                 }),
-                V = e => "character_start_index" in e && "character_end_index" in e && "line_index" in e;
-            var A, B, j, U, W;
+                B = e => "character_start_index" in e && "character_end_index" in e && "line_index" in e;
+            var V, j, U, W, Z, F;
             ! function(e) {
                 e.SECRETS = "SECRETS", e.PII_FOUND = "PII_FOUND", e.UNAPPROVED_LICENSE = "UNAPPROVED_LICENSE_IMPORT", e.VULNERABLE_DEPENDENCY = "VULNERABLE_DEPENDENCY_IMPORT"
-            }(A || (A = {})),
+            }(V || (V = {})),
             function(e) {
                 e.LOW = "LOW", e.MEDIUM = "MEDIUM", e.HIGH = "HIGH", e.CRITICAL = "CRITICAL", e.ANY = "ANY"
-            }(B || (B = {})),
+            }(j || (j = {})),
             function(e) {
                 e.INPUT = "INPUT", e.OUTPUT = "OUTPUT"
-            }(j || (j = {})),
+            }(U || (U = {})),
             function(e) {
                 e.SOURCE = "SOURCE", e.MARKDOWN = "MARKDOWN", e.STREAM = "STREAM", e.PLAINTEXT = "PLAINTEXT", e.DATAFRAME = "DATAFRAME"
-            }(U || (U = {})),
+            }(W || (W = {})),
             function(e) {
                 e.UNKNOWN_ISSUE = "UNKNOWN_ISSUE", e.HTTP_ERROR = "HTTPError", e.PYTHON_EXCEPTION = "Exception"
-            }(W || (W = {}));
-            const Z = (0, H.zE)({
+            }(Z || (Z = {})),
+            function(e) {
+                e.WARN = "warn", e.ERROR = "error"
+            }(F || (F = {}));
+            const $ = (0, H.zE)({
                     wrapper: {
                         display: "flex",
                         flexDirection: "column",
                         alignItems: "center",
                         justifyContent: "center",
                         marginTop: "78px"
                     },
                     message: {
                         marginTop: "8px",
                         fontWeight: 700,
                         fontSize: "16px"
                     }
                 }),
-                F = () => M().createElement("div", {
-                    className: Z.wrapper
-                }, M().createElement(k.react, null), M().createElement("h2", {
-                    className: Z.message
+                z = () => _().createElement("div", {
+                    className: $.wrapper
+                }, _().createElement(k.react, null), _().createElement("h2", {
+                    className: $.message
                 }, "No issues found"));
-            var $ = n(706),
-                z = n.n($);
-            const G = {
-                    [B.LOW]: "#07B7CE",
-                    [B.MEDIUM]: "#F4BD4F",
-                    [B.HIGH]: "#ED6A5E",
-                    [B.CRITICAL]: "#D01100"
+            var G = n(706),
+                Y = n.n(G);
+            const K = {
+                    [j.LOW]: "#07B7CE",
+                    [j.MEDIUM]: "#F4BD4F",
+                    [j.HIGH]: "#ED6A5E",
+                    [j.CRITICAL]: "#D01100"
                 },
-                Y = (0, H.zE)({
+                X = (0, H.zE)({
                     listItem: {
                         listStyle: "none",
                         margin: "5px 0",
                         paddingInlineStart: 0
                     },
                     link: {
                         display: "inline-flex",
@@ -194,25 +197,25 @@
                         borderRadius: "4px",
                         color: "white",
                         height: "16px",
                         width: "16px",
                         textAlign: "center",
                         margin: "0 4px 0 auto"
                     },
-                    [`issueCount${B.LOW}`]: {
-                        backgroundColor: G[B.LOW]
+                    [`issueCount${j.LOW}`]: {
+                        backgroundColor: K[j.LOW]
                     },
-                    [`issueCount${B.MEDIUM}`]: {
-                        backgroundColor: G[B.MEDIUM]
+                    [`issueCount${j.MEDIUM}`]: {
+                        backgroundColor: K[j.MEDIUM]
                     },
-                    [`issueCount${B.HIGH}`]: {
-                        backgroundColor: G[B.HIGH]
+                    [`issueCount${j.HIGH}`]: {
+                        backgroundColor: K[j.HIGH]
                     },
-                    [`issueCount${B.CRITICAL}`]: {
-                        backgroundColor: G[B.CRITICAL]
+                    [`issueCount${j.CRITICAL}`]: {
+                        backgroundColor: K[j.CRITICAL]
                     },
                     innerList: {
                         listStyle: "none",
                         padding: "12px",
                         backgroundColor: "var(--jp-layout-color2)"
                     },
                     issueListItem: {
@@ -232,125 +235,125 @@
                     },
                     issueListItemWrapper: {
                         display: "block",
                         paddingLeft: "8px",
                         borderLeft: "4px solid",
                         fontSize: "12px"
                     },
-                    [`issueListItemWrapper${B.LOW}`]: {
-                        borderLeftColor: G[B.LOW]
+                    [`issueListItemWrapper${j.LOW}`]: {
+                        borderLeftColor: K[j.LOW]
                     },
-                    [`issueListItemWrapper${B.MEDIUM}`]: {
-                        borderLeftColor: G[B.MEDIUM]
+                    [`issueListItemWrapper${j.MEDIUM}`]: {
+                        borderLeftColor: K[j.MEDIUM]
                     },
-                    [`issueListItemWrapper${B.HIGH}`]: {
-                        borderLeftColor: G[B.HIGH]
+                    [`issueListItemWrapper${j.HIGH}`]: {
+                        borderLeftColor: K[j.HIGH]
                     },
-                    [`issueListItemWrapper${B.CRITICAL}`]: {
-                        borderLeftColor: G[B.CRITICAL]
+                    [`issueListItemWrapper${j.CRITICAL}`]: {
+                        borderLeftColor: K[j.CRITICAL]
                     },
                     issueType: {
                         fontWeight: "bold",
                         fontSize: "14px"
                     }
                 }),
-                K = e => {
+                q = e => {
                     switch (e) {
-                        case A.PII_FOUND:
+                        case V.PII_FOUND:
                             return "PII";
-                        case A.SECRETS:
+                        case V.SECRETS:
                             return "Secret";
-                        case A.UNAPPROVED_LICENSE:
+                        case V.UNAPPROVED_LICENSE:
                             return "License";
-                        case A.VULNERABLE_DEPENDENCY:
+                        case V.VULNERABLE_DEPENDENCY:
                             return "CVE";
                         default:
                             return "Unknown"
                     }
                 },
-                X = e => {
+                J = e => {
                     if (e) {
                         const t = {};
                         for (const n of e) n.cell.cell_index in t ? t[n.cell.cell_index].push(n) : t[n.cell.cell_index] = [n];
                         return t
                     }
                     return {}
                 },
-                q = ({
+                Q = ({
                     scannedNotebook: e,
                     severity: t,
                     issues: n
                 }) => {
-                    const [s, o] = M().useState(!1);
-                    return M().createElement("li", {
-                        className: Y.listItem
-                    }, M().createElement("a", {
+                    const [s, o] = _().useState(!1);
+                    return _().createElement("li", {
+                        className: X.listItem
+                    }, _().createElement("a", {
                         onClick: e => {
                             e.preventDefault(), o(!s)
                         },
-                        className: Y.link
-                    }, M().createElement("b", {
-                        className: Y.title
-                    }, t.toLowerCase()), M().createElement("span", {
-                        className: (0, H.Sh)(Y.issueCount, Y[`issueCount${t}`])
-                    }, (null == n ? void 0 : n.length) || 0), M().createElement(b.react, {
-                        className: (0, H.Sh)(Y.caret, s && Y.expandedCaret)
-                    })), M().createElement(z(), {
+                        className: X.link
+                    }, _().createElement("b", {
+                        className: X.title
+                    }, t.toLowerCase()), _().createElement("span", {
+                        className: (0, H.Sh)(X.issueCount, X[`issueCount${t}`])
+                    }, (null == n ? void 0 : n.length) || 0), _().createElement(b.react, {
+                        className: (0, H.Sh)(X.caret, s && X.expandedCaret)
+                    })), _().createElement(Y(), {
                         duration: 500,
                         height: s ? "auto" : 0
-                    }, M().createElement("ul", {
-                        className: Y.innerList
+                    }, _().createElement("ul", {
+                        className: X.innerList
                     }, null == n ? void 0 : n.map((n => {
                         var s;
-                        return M().createElement("li", {
+                        return _().createElement("li", {
                             key: n.cell.cell_index + n.code + n.location,
-                            className: Y.issueListItem
-                        }, M().createElement("a", {
-                            className: (0, H.Sh)(Y.issueListItemWrapper, Y[`issueListItemWrapper${t}`]),
+                            className: X.issueListItem
+                        }, _().createElement("a", {
+                            className: (0, H.Sh)(X.issueListItemWrapper, X[`issueListItemWrapper${t}`]),
                             onClick: t => {
                                 var s, o;
                                 t.preventDefault();
                                 const a = null === (s = e.notebook) || void 0 === s ? void 0 : s.widgets[n.cell.cell_index];
                                 a && (null === (o = e.notebook) || void 0 === o || o.scrollToCell(a))
                             }
-                        }, M().createElement("p", {
-                            className: Y.issueType
-                        }, "Issue type: ", K(n.code)), M().createElement("p", null, null === (s = n.details) || void 0 === s ? void 0 : s.description), M().createElement("p", null, "Cell index: ", n.cell.cell_index)))
-                    })), 0 === (null == n ? void 0 : n.length) && M().createElement(M().Fragment, null, "No issues were found at this severity level"))))
+                        }, _().createElement("p", {
+                            className: X.issueType
+                        }, "Issue type: ", q(n.code)), _().createElement("p", null, null === (s = n.details) || void 0 === s ? void 0 : s.description), _().createElement("p", null, "Cell index: ", n.cell.cell_index)))
+                    })), 0 === (null == n ? void 0 : n.length) && _().createElement(_().Fragment, null, "No issues were found at this severity level"))))
                 },
-                J = ({
+                ee = ({
                     scannedNotebook: e,
                     results: t,
                     scanHasErrors: n
-                }) => M().createElement(M().Fragment, null, (e => void 0 !== e && e.notebook_issues && 0 === e.notebook_issues[0].issues.length)(t) ? n ? null : M().createElement(F, null) : M().createElement(M().Fragment, null, M().createElement("h2", {
-                    className: R.header
-                }, "Found issues:"), M().createElement("ul", {
-                    className: R.list
+                }) => _().createElement(_().Fragment, null, (e => void 0 !== e && e.notebook_issues && 0 === e.notebook_issues[0].issues.length)(t) ? n ? null : _().createElement(z, null) : _().createElement(_().Fragment, null, _().createElement("h2", {
+                    className: A.header
+                }, "Found issues:"), _().createElement("ul", {
+                    className: A.list
                 }, Object.entries((e => {
                     if (e && "object" == typeof e && "notebook_issues" in e) {
                         const t = {
-                            [B.CRITICAL]: [],
-                            [B.HIGH]: [],
-                            [B.MEDIUM]: [],
-                            [B.LOW]: []
+                            [j.CRITICAL]: [],
+                            [j.HIGH]: [],
+                            [j.MEDIUM]: [],
+                            [j.LOW]: []
                         };
                         return e.notebook_issues[0].issues.forEach((e => {
                             var n;
                             null === (n = t[e.severity]) || void 0 === n || n.push(e)
                         })), t
                     }
                     return {}
-                })(t)).map((([t, n]) => M().createElement(q, {
+                })(t)).map((([t, n]) => _().createElement(Q, {
                     scannedNotebook: e,
                     issues: n,
                     severity: t,
                     key: `${t}-${e.notebookPath}`
                 }))))));
-            var Q = n(456);
-            const ee = (0, H.zE)({
+            var te = n(456);
+            const ne = (0, H.zE)({
                     innerWrapper: {
                         padding: "16px",
                         display: "flex",
                         flexDirection: "column"
                     },
                     issueWrapper: {
                         display: "flex",
@@ -368,18 +371,18 @@
                     header: {
                         fontWeight: 600,
                         fontSize: "14px",
                         lineHeight: "20px",
                         margin: 0
                     }
                 }),
-                te = ({
+                se = ({
                     notebookIssues: e
                 }) => {
-                    return M().createElement("div", {
+                    return _().createElement("div", {
                         className: (0, H.Sh)((t = e[0].cell.cell_index, (0, H.oB)({
                             backgroundColor: "var(--jp-layout-color1)",
                             color: "var(--jp-ui-font-color0)",
                             zIndex: 999 - t,
                             overflowY: "hidden",
                             overflowX: "auto",
                             position: "absolute",
@@ -387,127 +390,127 @@
                             left: "calc(var(--jp-cell-collapser-width) + var(--jp-cell-prompt-width))",
                             width: "460px",
                             maxWidth: "calc(100% - (var(--jp-cell-collapser-width) + var(--jp-cell-prompt-width)))",
                             maxHeight: 0,
                             transition: "max-height .5s ease",
                             boxShadow: "0px 4px 10px rgba(0, 0, 0, 0.1)"
                         })), "nbdefense-cell-error-dropdown")
-                    }, M().createElement("div", {
-                        className: ee.innerWrapper
+                    }, _().createElement("div", {
+                        className: ne.innerWrapper
                     }, e.map((e => {
                         var t, n, s;
-                        return M().createElement("div", {
+                        return _().createElement("div", {
                             key: null === (t = e.details) || void 0 === t ? void 0 : t.description,
-                            className: ee.issueWrapper
-                        }, M().createElement(E.react, {
-                            className: ee.alertIcon
-                        }), M().createElement("div", null, M().createElement("h3", {
-                            className: ee.header
-                        }, K(e.code)), M().createElement("p", null, "Vulnerability: ", (e => {
+                            className: ne.issueWrapper
+                        }, _().createElement(E.react, {
+                            className: ne.alertIcon
+                        }), _().createElement("div", null, _().createElement("h3", {
+                            className: ne.header
+                        }, q(e.code)), _().createElement("p", null, "Vulnerability: ", (e => {
                             switch (e) {
-                                case A.PII_FOUND:
+                                case V.PII_FOUND:
                                     return "Exposed personally identifiable information";
-                                case A.SECRETS:
+                                case V.SECRETS:
                                     return "Exposed secret";
-                                case A.UNAPPROVED_LICENSE:
+                                case V.UNAPPROVED_LICENSE:
                                     return "Unapproved license associated with import";
-                                case A.VULNERABLE_DEPENDENCY:
+                                case V.VULNERABLE_DEPENDENCY:
                                     return "CVE associated with import";
                                 default:
                                     return "Unknown"
                             }
-                        })(e.code)), M().createElement("p", null, "Description: ", null === (n = e.details) || void 0 === n ? void 0 : n.description, (null === (s = e.details) || void 0 === s ? void 0 : s.summary_field) ? M().createElement(M().Fragment, null, " ", "in cell ", e.location, " with tags:", M().createElement("pre", null, JSON.stringify(e.details.summary_field, void 0, "  "))) : null)))
+                        })(e.code)), _().createElement("p", null, "Description: ", null === (n = e.details) || void 0 === n ? void 0 : n.description, (null === (s = e.details) || void 0 === s ? void 0 : s.summary_field) ? _().createElement(_().Fragment, null, " ", "in cell ", e.location, " with tags:", _().createElement("pre", null, JSON.stringify(e.details.summary_field, void 0, "  "))) : null)))
                     }))));
                     var t
                 },
-                ne = "jp-Cell-inputWrapper",
-                se = "nbdefense-cell-input-error",
-                oe = "jp-OutputArea-output",
-                ae = "jp-Collapser",
-                re = "nbdefense-cell-input-collapser-error",
-                ie = "nbdefense-syntax-error",
-                le = (e, t, n, s) => {
-                    const o = null == t ? void 0 : t.node.getElementsByClassName(ne);
+                oe = "jp-Cell-inputWrapper",
+                ae = "nbdefense-cell-input-error",
+                re = "jp-OutputArea-output",
+                ie = "jp-Collapser",
+                le = "nbdefense-cell-input-collapser-error",
+                ce = "nbdefense-syntax-error",
+                de = (e, t, n, s) => {
+                    const o = null == t ? void 0 : t.node.getElementsByClassName(oe);
                     if (o && o.length > 0) {
                         if (!1 !== n) {
-                            o[0].classList.add(se);
-                            const e = o[0].getElementsByClassName(ae);
-                            e && e.length > 0 && e[0].classList.add(re)
+                            o[0].classList.add(ae);
+                            const e = o[0].getElementsByClassName(ie);
+                            e && e.length > 0 && e[0].classList.add(le)
                         }
-                        const a = ue(e),
-                            r = null == t ? void 0 : t.node.getElementsByClassName(oe),
+                        const a = Ce(e),
+                            r = null == t ? void 0 : t.node.getElementsByClassName(re),
                             i = !1 !== n ? Object.entries(a).map((([e, n]) => {
                                 const s = n.flatMap((e => (e => "issues" in e)(e) ? e.issues : e));
-                                return e === U.SOURCE || e === U.MARKDOWN ? s.map((e => de(t, e))) : e === U.STREAM || e === U.PLAINTEXT ? pe(r, e, s) : e === U.DATAFRAME ? he(t, s) : void 0
+                                return e === W.SOURCE || e === W.MARKDOWN ? s.map((e => he(t, e))) : e === W.STREAM || e === W.PLAINTEXT ? ue(r, e, s) : e === W.DATAFRAME ? ge(t, s) : void 0
                             })).flat() : void 0;
-                        return [!1 !== s ? Q.createPortal(M().createElement(te, {
+                        return [!1 !== s ? te.createPortal(_().createElement(se, {
                             notebookIssues: e
                         }), o[0]) : void 0, i]
                     }
                     return [void 0, void 0]
                 },
-                ce = (e, t) => {
+                pe = (e, t) => {
                     e.forEach((e => {
-                        const t = e.node.getElementsByClassName(ne);
+                        const t = e.node.getElementsByClassName(oe);
                         if (t && t.length > 0) {
-                            t[0].classList.remove(se);
-                            const e = t[0].getElementsByClassName(ae);
-                            e && e.length > 0 && e[0].classList.remove(re)
+                            t[0].classList.remove(ae);
+                            const e = t[0].getElementsByClassName(ie);
+                            e && e.length > 0 && e[0].classList.remove(le)
                         }
                     })), t.forEach((e => {
                         e && ("function" != typeof e ? e.clear() : e())
                     }))
                 },
-                de = (e, t) => {
+                he = (e, t) => {
                     const n = null == e ? void 0 : e.editor;
-                    if (n && V(t)) return n.doc.markText({
+                    if (n && B(t)) return n.doc.markText({
                         line: t.line_index,
                         ch: t.character_start_index
                     }, {
                         line: t.line_index,
                         ch: t.character_end_index
                     }, {
-                        className: ie,
+                        className: ce,
                         title: "NB Defense scan issue detected",
                         clearOnEnter: !0
                     })
                 },
-                pe = (e, t, n) => {
+                ue = (e, t, n) => {
                     const s = {};
                     return n.forEach((e => {
                         const t = "output_index" in e.cell ? e.cell.output_index : 0;
                         s[t] ? s[t].push(e) : s[t] = [e]
                     })), Object.entries(s).map((([n, s]) => {
-                        const o = Ce(e, t, Number(n));
+                        const o = me(e, t, Number(n));
                         if (o) {
                             const e = null == o ? void 0 : o.innerHTML,
                                 t = null == o ? void 0 : o.querySelectorAll("pre")[0];
                             if (t) {
                                 const e = {};
                                 let n = t.textContent || "";
                                 const o = n.split("\n") || [];
                                 s.forEach((t => {
-                                    if (V(t)) {
+                                    if (B(t)) {
                                         let s = 0;
                                         t.line_index in e && (s = e[t.line_index]);
                                         const a = o[t.line_index].substring(t.character_start_index + s, t.character_end_index + s),
                                             r = n.length;
-                                        o[t.line_index] = `${o[t.line_index].substring(0,t.character_start_index+s)}<span class='${ie}'>${a}</span>${o[t.line_index].substring(t.character_end_index+s)}`, n = o.join("\n"), s += n.length - r, e[t.line_index] = s
+                                        o[t.line_index] = `${o[t.line_index].substring(0,t.character_start_index+s)}<span class='${ce}'>${a}</span>${o[t.line_index].substring(t.character_end_index+s)}`, n = o.join("\n"), s += n.length - r, e[t.line_index] = s
                                     }
                                 })), t.innerHTML = n
                             }
                             return () => {
                                 o.innerHTML = e
                             }
                         }
                     }))
                 },
-                he = (e, t) => {
-                    const n = null == e ? void 0 : e.node.getElementsByClassName(oe),
-                        s = Ce(n, U.DATAFRAME);
+                ge = (e, t) => {
+                    const n = null == e ? void 0 : e.node.getElementsByClassName(re),
+                        s = me(n, W.DATAFRAME);
                     if (s) {
                         const e = s.innerHTML;
                         return t.forEach((e => {
                             if ((e => "row_index" in e && "column_index" in e)(e)) {
                                 const t = s.querySelectorAll("table.dataframe"),
                                     {
                                         row_index: n,
@@ -519,38 +522,38 @@
                                 i = n < r.length ? r[n].children.item(o + 1) : a[n - r.length].children.item(o + 1), null == i || i.classList.add("nbdefense-table-error")
                             }
                         })), () => {
                             s.innerHTML = e
                         }
                     }
                 },
-                ue = e => {
+                Ce = e => {
                     const t = {
-                        [U.SOURCE]: [],
-                        [U.MARKDOWN]: [],
-                        [U.STREAM]: [],
-                        [U.PLAINTEXT]: [],
-                        [U.DATAFRAME]: []
+                        [W.SOURCE]: [],
+                        [W.MARKDOWN]: [],
+                        [W.STREAM]: [],
+                        [W.PLAINTEXT]: [],
+                        [W.DATAFRAME]: []
                     };
                     return e.forEach((e => {
                         t[e.cell.cell_type].push(e)
                     })), t
                 },
-                Ce = (e, t, n = 0) => {
+                me = (e, t, n = 0) => {
                     var s;
                     if (e)
                         for (const o of Array.from(e)) {
                             const e = null === (s = o.getAttributeNode("data-mime-type")) || void 0 === s ? void 0 : s.value;
-                            if (t === U.PLAINTEXT && "text/plain" === e) return o;
-                            if (t === U.STREAM && "application/vnd.jupyter.stdout" === e && !n) return o;
-                            if (t === U.DATAFRAME && "text/html" === e && o.querySelectorAll("table.dataframe").length > 0) return o;
+                            if (t === W.PLAINTEXT && "text/plain" === e) return o;
+                            if (t === W.STREAM && "application/vnd.jupyter.stdout" === e && !n) return o;
+                            if (t === W.DATAFRAME && "text/html" === e && o.querySelectorAll("table.dataframe").length > 0) return o;
                             n--
                         }
                 },
-                ge = (e, t) => {
+                be = (e, t) => {
                     var n, s, o, a;
                     return "loading" === t.type ? Object.assign(Object.assign({}, e), {
                         [t.notebookPath]: {
                             isLoading: !0,
                             notebook: t.notebook || e[t.notebookPath].notebook,
                             report: void 0,
                             portals: (null === (n = e[t.notebookPath]) || void 0 === n ? void 0 : n.portals) || [],
@@ -597,18 +600,18 @@
                     }) : "clearPortalsAndMarks" === t.type ? Object.assign(Object.assign({}, e), {
                         [t.notebookPath]: Object.assign(Object.assign({}, e[t.notebookPath]), {
                             portals: [],
                             marks: []
                         })
                     }) : "clearAllReports" === t.type ? (Object.values(e).forEach((e => {
                         const t = e.notebook.widgets;
-                        ce(t, e.marks)
+                        pe(t, e.marks)
                     })), {}) : Object.assign({}, e)
                 },
-                me = (0, H.zE)({
+                fe = (0, H.zE)({
                     wrapper: {
                         display: "flex",
                         flexDirection: "column",
                         height: "100%",
                         overflowY: "auto",
                         padding: "1rem",
                         backgroundColor: "var(--jp-layout-color0)"
@@ -622,76 +625,83 @@
                         whiteSpace: "pre-wrap",
                         marginBottom: "8px",
                         fontWeight: "700",
                         fontSize: "16px",
                         lineHeight: "100%"
                     }
                 });
-            var be = n(830);
-            const fe = (e, t) => {
+            var ke = n(830);
+            const Ee = (e, t) => {
                     if (t && t in e) {
                         const n = e[t].lastUpdated;
-                        if (n) return (0, be.format)(n, "MM/dd/yy hh:mm:ss aa")
+                        if (n) return (0, ke.format)(n, "MM/dd/yy hh:mm:ss aa")
                     }
                     return ""
                 },
-                ke = ({
+                we = ({
                     results: e,
                     notebookPath: t
                 }) => {
-                    const [n, s] = M().useState(new Date);
-                    return M().useEffect((() => {
+                    const [n, s] = _().useState(new Date);
+                    return _().useEffect((() => {
                         const e = setInterval((() => s(new Date)), 1e3);
                         return () => clearInterval(e)
-                    }), []), M().createElement("p", {
-                        title: fe(e, t)
-                    }, M().createElement("b", null, "Last scan"), M().createElement("br", null), ((e, t, n) => {
+                    }), []), _().createElement("p", {
+                        title: Ee(e, t)
+                    }, _().createElement("b", null, "Last scan"), _().createElement("br", null), ((e, t, n) => {
                         if (n && n in t) {
                             const s = t[n].lastUpdated;
-                            if (s) return (0, be.differenceInMinutes)(e, s) < 1 ? "Just now" : fe(t, n)
+                            if (s) return (0, ke.differenceInMinutes)(e, s) < 1 ? "Just now" : Ee(t, n)
                         }
                         return "Never scanned"
                     })(n, e, t))
                 },
-                Ee = (0, H.oB)({
+                Le = {
                     display: "flex",
                     justifyContent: "center",
                     marginTop: "16px",
                     border: "none",
                     borderRadius: "6px",
                     padding: "10px",
                     backgroundColor: "#0060A8",
                     color: "white",
                     cursor: "pointer",
                     lineHeight: "16px",
-                    fontSize: "14px",
+                    fontSize: "14px"
+                },
+                ve = (0, H.oB)(Object.assign(Object.assign({}, Le), {
                     $nest: {
                         "&:disabled": {
                             opacity: .5,
                             cursor: "wait"
                         }
                     }
-                }),
-                we = (0, H.oB)({
+                })),
+                xe = (0, H.oB)(Object.assign(Object.assign({}, Le), {
+                    opacity: .5,
+                    cursor: "default"
+                })),
+                Me = (0, H.oB)({
                     height: "16px",
                     width: "16px",
                     marginRight: "8px"
                 }),
-                Le = ({
+                _e = ({
                     isLoading: e,
                     scanExists: t,
-                    onClick: n
-                }) => M().createElement("button", {
-                    disabled: e,
                     onClick: n,
-                    className: Ee
-                }, e ? M().createElement(M().Fragment, null, M().createElement(m.react, {
-                    className: we
+                    disabled: s
+                }) => _().createElement("button", {
+                    disabled: e || s,
+                    onClick: n,
+                    className: s ? xe : ve
+                }, e ? _().createElement(_().Fragment, null, _().createElement(m.react, {
+                    className: Me
                 }), " Scanning...") : t ? "Rescan" : "Scan"),
-                ve = (0, H.zE)({
+                ye = (0, H.zE)({
                     wrapper: {
                         position: "sticky",
                         top: 0
                     },
                     backgroundImage: {
                         height: "65px",
                         background: "#091228",
@@ -709,84 +719,87 @@
                     grow: {
                         flexGrow: "1"
                     },
                     iconWrapper: {
                         height: "27px"
                     }
                 }),
-                xe = () => M().createElement("div", {
-                    className: ve.wrapper
-                }, M().createElement(L.react, {
-                    className: ve.backgroundImage,
+                Ne = () => _().createElement("div", {
+                    className: ye.wrapper
+                }, _().createElement(L.react, {
+                    className: ye.backgroundImage,
                     width: "100%",
                     height: "65px"
-                }), M().createElement("div", {
-                    className: ve.contentWrapper
-                }, M().createElement("div", {
-                    className: ve.iconWrapper
-                }, M().createElement(w.react, {
+                }), _().createElement("div", {
+                    className: ye.contentWrapper
+                }, _().createElement("div", {
+                    className: ye.iconWrapper
+                }, _().createElement(w.react, {
                     height: "27px"
-                })), M().createElement("div", {
-                    className: ve.grow
+                })), _().createElement("div", {
+                    className: ye.grow
                 }))),
-                Me = (0, H.zE)({
+                Pe = (0, H.zE)({
                     spacing: {
                         paddingBottom: "8px"
                     }
                 }),
-                _e = ({
+                Ie = ({
                     notebookPath: e
-                }) => M().createElement("p", {
-                    className: Me.spacing
-                }, M().createElement("b", null, "Full Path"), M().createElement("br", null), e ? `${D().join(O.PageConfig.getOption("serverRoot"),D().dirname(e))}/` : "Please select a notebook"),
-                ye = (0, H.zE)({
+                }) => _().createElement("p", {
+                    className: Pe.spacing
+                }, _().createElement("b", null, "Full Path"), _().createElement("br", null), e ? `${D().join(T.PageConfig.getOption("serverRoot"),D().dirname(e))}/` : "Please select a notebook"),
+                Se = e => (0, H.zE)({
                     wrapper: {
                         display: "flex",
                         marginTop: "16px",
                         padding: "10px",
-                        border: "1px #F4BD4F",
                         borderStyle: "solid",
                         borderRadius: "6px",
-                        backgroundColor: "#FFEFCF"
+                        border: e === F.WARN ? "1px #F4BD4F" : "1px #D01100",
+                        backgroundColor: e === F.WARN ? "#FFEFCF" : "#FFCCCB"
                     },
-                    warning: {
+                    message: {
                         alignItems: "center",
                         padding: "0px",
                         paddingLeft: "10px"
                     }
                 }),
-                Ne = () => M().createElement("div", {
-                    className: ye.wrapper
-                }, M().createElement(f.react, null), M().createElement("p", {
-                    className: ye.warning
-                }, "The notebook contents have changed since the last run. The results may be outdated.")),
-                Pe = (0, H.zE)({
+                Oe = ({
+                    message: e,
+                    level: t = F.WARN
+                }) => _().createElement("div", {
+                    className: Se(t).wrapper
+                }, t === F.WARN && _().createElement(f.react, null), t === F.ERROR && _().createElement(x.react, null), _().createElement("p", {
+                    className: Se(t).message
+                }, e)),
+                De = (0, H.zE)({
                     wrapper: {
                         display: "flex",
                         marginTop: "16px",
                         padding: "10px",
                         border: "1px #d01100",
                         borderStyle: "solid",
                         borderRadius: "6px",
                         backgroundColor: "rgb(208 17 0 / 10%)"
                     }
                 }),
-                Ie = ({
+                Te = ({
                     errors: e
-                }) => M().createElement(M().Fragment, null, e && e.map(((e, t) => {
+                }) => _().createElement(_().Fragment, null, e && e.map(((e, t) => {
                     const n = "plugin_name" in e ? `An error occurred in the ${e.plugin_name} when scanning: ${e.message}` : e.message;
-                    return M().createElement("div", {
+                    return _().createElement("div", {
                         key: `${t}-${n}`,
-                        className: Pe.wrapper,
+                        className: De.wrapper,
                         dangerouslySetInnerHTML: {
                             __html: `${n}`
                         }
                     })
                 }))),
-                Se = (0, H.zE)({
+                Re = (0, H.zE)({
                     warningWrapper: {
                         display: "flex",
                         padding: "10px",
                         border: "1px #F4BD4F",
                         borderStyle: "solid",
                         borderRadius: "6px",
                         backgroundColor: "#FFEFCF"
@@ -796,38 +809,38 @@
                     },
                     warning: {
                         alignItems: "center",
                         padding: "0px",
                         paddingLeft: "10px"
                     }
                 }),
-                De = ({
+                He = ({
                     kernelName: e,
                     sitePackagesPath: t,
                     loading: n
-                }) => M().createElement("div", {
-                    className: Se.spacing
-                }, M().createElement("b", null, "Kernel"), M().createElement("br", null), n || t ? M().createElement(M().Fragment, null, n ? M().createElement(m.react, null) : e) : M().createElement("div", {
-                    className: Se.warningWrapper
-                }, M().createElement(f.react, null), M().createElement("p", {
-                    className: Se.warning
+                }) => _().createElement("div", {
+                    className: Re.spacing
+                }, _().createElement("b", null, "Kernel"), _().createElement("br", null), n || t ? _().createElement(_().Fragment, null, n ? _().createElement(m.react, null) : e) : _().createElement("div", {
+                    className: Re.warningWrapper
+                }, _().createElement(f.react, null), _().createElement("p", {
+                    className: Re.warning
                 }, "No Kernel Selected. Scans that rely on the kernel will be skipped."))),
-                Oe = ({
+                Ae = ({
                     notebookTracker: e,
                     runScanSignal: t,
                     isContextualHelpVisible: n,
                     isNBDefenseDropdownVisible: s,
                     settings: o
                 }) => {
                     var a;
                     const r = (({
                             notebookTracker: e
                         }) => {
-                            const [t, n] = M().useState(void 0), [s, o] = M().useState(void 0), [a, r] = M().useState(void 0), [i, l] = M().useState(void 0);
-                            return M().useEffect((() => (e.currentChanged.connect(((e, s) => {
+                            const [t, n] = _().useState(void 0), [s, o] = _().useState(void 0), [a, r] = _().useState(void 0), [i, l] = _().useState(void 0);
+                            return _().useEffect((() => (e.currentChanged.connect(((e, s) => {
                                 null !== s && t === (null == s ? void 0 : s.context.path) || (r(null == s ? void 0 : s.content), o(null == s ? void 0 : s.model), (null == s ? void 0 : s.context) && (null == i || i.pathChanged.disconnect((() => null)), l(s.context), n(s.context.path), s.context.pathChanged.connect((e => {
                                     n(e.path)
                                 }))))
                             })), () => {
                                 e.currentChanged.disconnect((() => {
                                     n(void 0), o(void 0)
                                 })), null == i || i.pathChanged.disconnect((() => {
@@ -842,47 +855,47 @@
                             notebookTracker: e
                         }),
                         [l, c] = (({
                             notebookTracker: e,
                             isContextualHelpVisible: t,
                             isNBDefenseDropdownVisible: n
                         }) => {
-                            const [s, o] = M().useReducer(ge, {}), a = I()((async (e, t) => {
+                            const [s, o] = _().useReducer(be, {}), a = S()((async (e, t) => {
                                 const n = t.context.path;
                                 n in s && (await t.revealed, o({
                                     notebookPath: n,
                                     type: "isOpen",
                                     isOpen: !0,
                                     notebook: t.content
                                 }))
                             }));
-                            return M().useEffect((() => {
+                            return _().useEffect((() => {
                                 e.widgetAdded.disconnect(a), e.widgetAdded.connect(a)
-                            }), [e, s]), M().useEffect((() => {
+                            }), [e, s]), _().useEffect((() => {
                                 Object.entries(s).map((([e, a]) => {
                                     try {
                                         if (a.notebook.disposed.connect((() => {
                                                 o({
                                                     notebookPath: e,
                                                     type: "isOpen",
                                                     isOpen: !1
                                                 })
                                             })), a.isOpen) {
                                             const r = a.report;
                                             if (!a.hasRenderedResults && r) {
                                                 const s = a.notebook.widgets;
-                                                ce(s, a.marks), o({
+                                                pe(s, a.marks), o({
                                                     notebookPath: e,
                                                     type: "clearPortalsAndMarks"
                                                 });
                                                 const {
                                                     new_portals: i,
                                                     new_marks: l
-                                                } = Object.entries(X(r.notebook_issues[0].issues)).map((([e, o]) => {
-                                                    const [a, r] = le(o, s[parseInt(e)], t, n);
+                                                } = Object.entries(J(r.notebook_issues[0].issues)).map((([e, o]) => {
+                                                    const [a, r] = de(o, s[parseInt(e)], t, n);
                                                     return {
                                                         portal: a,
                                                         cell_marks: r
                                                     }
                                                 })).reduce((({
                                                     new_portals: e,
                                                     new_marks: t
@@ -900,55 +913,55 @@
                                                     notebookPath: e,
                                                     type: "hasRenderedReport",
                                                     portals: i,
                                                     marks: l
                                                 })
                                             } else if (a.isLoading && s[e] && (0 !== s[e].marks.length || 0 !== s[e].portals.length)) {
                                                 const t = a.notebook.widgets;
-                                                ce(t, a.marks), o({
+                                                pe(t, a.marks), o({
                                                     notebookPath: e,
                                                     type: "clearPortalsAndMarks"
                                                 })
                                             }
                                         }
                                     } catch (t) {
                                         o({
                                             notebookPath: e,
                                             type: "error",
                                             error: [{
                                                 message: `<span>There was an issue scanning this notebook. Please create an issue here: <a class="nbdefense-error-link" href=${h} target="_blank">${u}</a></span>`,
                                                 statusCode: 400,
-                                                errorType: W.UNKNOWN_ISSUE,
+                                                errorType: Z.UNKNOWN_ISSUE,
                                                 notebookPath: e
                                             }]
                                         })
                                     }
                                 }))
-                            }), [s]), M().useEffect((() => {
+                            }), [s]), _().useEffect((() => {
                                 Object.entries(s).map((([e, s]) => {
                                     try {
                                         if (s.notebook.disposed.connect((() => {
                                                 o({
                                                     notebookPath: e,
                                                     type: "isOpen",
                                                     isOpen: !1
                                                 })
                                             })), s.isOpen) {
                                             const a = s.report;
                                             if (a) {
                                                 const r = s.notebook.widgets;
-                                                ce(r, s.marks), o({
+                                                pe(r, s.marks), o({
                                                     notebookPath: e,
                                                     type: "clearPortalsAndMarks"
                                                 });
                                                 const {
                                                     new_portals: i,
                                                     new_marks: l
-                                                } = Object.entries(X(a.notebook_issues[0].issues)).map((([e, s]) => {
-                                                    const [o, a] = le(s, r[parseInt(e)], t, n);
+                                                } = Object.entries(J(a.notebook_issues[0].issues)).map((([e, s]) => {
+                                                    const [o, a] = de(s, r[parseInt(e)], t, n);
                                                     return {
                                                         portal: o,
                                                         cell_marks: a
                                                     }
                                                 })).reduce((({
                                                     new_portals: e,
                                                     new_marks: t
@@ -973,15 +986,15 @@
                                     } catch (t) {
                                         o({
                                             notebookPath: e,
                                             type: "error",
                                             error: [{
                                                 message: `<span>There was an issue scanning this notebook. Please create an issue here: <a class="nbdefense-error-link" href=${h} target="_blank">${u}</a></span>`,
                                                 statusCode: 400,
-                                                errorType: W.UNKNOWN_ISSUE,
+                                                errorType: Z.UNKNOWN_ISSUE,
                                                 notebookPath: e
                                             }]
                                         })
                                     }
                                 }))
                             }), [t, n]), [s, o]
                         })({
@@ -989,47 +1002,47 @@
                             isContextualHelpVisible: n,
                             isNBDefenseDropdownVisible: s
                         }),
                         {
                             notebookModel: d,
                             notebookPath: p
                         } = r,
-                        C = (({
+                        g = (({
                             currentNotebookPath: e,
                             notebookTracker: t
                         }) => {
-                            const [n, s] = M().useState(void 0), [o, a] = M().useState(!1), [r, i] = M().useState(void 0), [l, c] = M().useState(void 0), [d, p] = M().useState(!0), h = e => {
+                            const [n, s] = _().useState(void 0), [o, a] = _().useState(!1), [r, i] = _().useState(void 0), [l, c] = _().useState(void 0), [d, p] = _().useState(!0), h = e => {
                                 if (e) {
                                     const t = "import site;print(site.getsitepackages()[0])",
                                         s = null == e ? void 0 : e.requestExecute({
                                             code: t
                                         });
                                     s && (s.onIOPub = e => {
                                         if ("stream" === e.header.msg_type) {
                                             const t = e.content;
                                             "\n" !== t.text && (i(t.text.replace(/(\n|)/gm, "")), c(null == n ? void 0 : n.kernelDisplayName))
                                         }
                                     })
                                 } else i(void 0), c(void 0);
                                 p(!1)
                             };
-                            return M().useEffect((() => (t.currentChanged.connect(((e, t) => {
+                            return _().useEffect((() => (t.currentChanged.connect(((e, t) => {
                                 t && s(t.sessionContext)
                             })), () => {
                                 t.currentChanged.disconnect((() => {
                                     i(void 0), c(void 0), p(!0)
                                 }))
-                            })), [t, n, o]), M().useEffect((() => (null == n || n.statusChanged.connect((e => {
+                            })), [t, n, o]), _().useEffect((() => (null == n || n.statusChanged.connect((e => {
                                 e.isReady !== o && a(e.isReady)
                             })), () => {
                                 null == n || n.statusChanged.disconnect((() => null))
-                            })), [n, o]), M().useEffect((() => {
+                            })), [n, o]), _().useEffect((() => {
                                 var t;
                                 o && (null == n ? void 0 : n.path) === e && h(null === (t = null == n ? void 0 : n.session) || void 0 === t ? void 0 : t.kernel)
-                            }), [n, o, e]), M().useEffect((() => (null == n || n.kernelChanged.connect((t => {
+                            }), [n, o, e]), _().useEffect((() => (null == n || n.kernelChanged.connect((t => {
                                 var n;
                                 t.path === e && o && h(null === (n = t.session) || void 0 === n ? void 0 : n.kernel)
                             })), () => {
                                 null == n || n.kernelChanged.disconnect((() => {
                                     i(void 0), c(void 0), p(!1)
                                 }))
                             })), [n, e, o]), {
@@ -1038,66 +1051,71 @@
                                 kernelIsLoading: d
                             }
                         })({
                             notebookTracker: e,
                             currentNotebookPath: p
                         }),
                         {
-                            kernelName: g,
+                            kernelName: C,
                             kernelSitePackagesPath: m,
                             kernelIsLoading: b
-                        } = C,
-                        [f, k] = (0, x.useState)(null),
+                        } = g,
+                        [f, k] = (0, M.useState)(null),
+                        [E, w] = (0, M.useState)(!1),
                         {
-                            sendJsonMessage: E,
-                            lastJsonMessage: w
-                        } = N()(f);
-                    (0, x.useEffect)((() => {
-                        const e = T.ServerConnection.makeSettings();
-                        k(O.URLExt.join(e.wsUrl, "nbdefense-jupyter", "scan"))
-                    }), []), (0, x.useEffect)((() => {
-                        const e = null == w ? void 0 : w.report;
+                            sendJsonMessage: L,
+                            lastJsonMessage: x
+                        } = P()(f, {
+                            onError: () => {
+                                w(!0)
+                            }
+                        });
+                    (0, M.useEffect)((() => {
+                        const e = R.ServerConnection.makeSettings();
+                        k(T.URLExt.join(e.wsUrl, "nbdefense-jupyter", "scan"))
+                    }), []), (0, M.useEffect)((() => {
+                        const e = null == x ? void 0 : x.report;
                         (e => {
                             const t = e;
                             return t && void 0 !== t.root && "string" == typeof t.root && void 0 !== t.notebook_issues && Array.isArray(t.notebook_issues)
                         })(e) && c({
-                            notebookPath: w.notebookPath,
+                            notebookPath: x.notebookPath,
                             type: "report",
                             report: e
                         }), (e => {
                             const t = e;
-                            return t && (t.errorType === W.HTTP_ERROR || t.errorType === W.PYTHON_EXCEPTION)
-                        })(w) && c({
-                            notebookPath: w.notebookPath,
+                            return t && (t.errorType === Z.HTTP_ERROR || t.errorType === Z.PYTHON_EXCEPTION)
+                        })(x) && c({
+                            notebookPath: x.notebookPath,
                             type: "error",
                             error: [{
                                 message: "An error occurred when scanning. Check that the NB Defense server extension is installed and enabled.",
-                                statusCode: w.statusCode,
-                                errorType: w.errorType,
-                                notebookPath: w.notebookPath
+                                statusCode: x.statusCode,
+                                errorType: x.errorType,
+                                notebookPath: x.notebookPath
                             }]
                         })
-                    }), [w]);
-                    const L = I()((() => {
+                    }), [x]);
+                    const y = S()((() => {
                         p && p in l && l[p].isOpen && c({
                             notebookPath: p,
                             type: "isDirty",
                             isDirty: !0
                         })
                     }));
-                    M().useEffect((() => {
-                        d && (d.contentChanged.disconnect(L), d.contentChanged.connect(L))
+                    _().useEffect((() => {
+                        d && (d.contentChanged.disconnect(y), d.contentChanged.connect(y))
                     }), [d]);
-                    const _ = I()((() => {
-                        p && l[p] && l[p].isLoading || p && y()
+                    const N = S()((() => {
+                        p && l[p] && l[p].isLoading || p && I()
                     }));
-                    M().useEffect((() => {
-                        t.disconnect(_), t.connect(_)
+                    _().useEffect((() => {
+                        t.disconnect(N), t.connect(N)
                     }), [p]);
-                    const y = async () => {
+                    const I = async () => {
                         if (d) {
                             if (null == d ? void 0 : d.dirty) await new i.Dialog({
                                 title: "Notebook has unsaved changes",
                                 body: "Cannot run scan because there are unsaved changes for the selected notebook. Please save your changes and run the scan again.",
                                 focusNodeSelector: "input",
                                 buttons: [i.Dialog.cancelButton({
                                     label: "Close"
@@ -1119,72 +1137,79 @@
                                             o && ("number" == typeof t[e] ? o[s[1]] = Number(t[e]) : "string" == typeof t[e] && (o[s[1]] = String(t[e])))
                                         })), e.plugins["nbdefense.plugins.SecretsPlugin"].secrets_plugins = n, e
                                     })(e) : {};
                                 c({
                                     notebookPath: p,
                                     type: "loading",
                                     notebook: r.notebook
-                                }), E({
+                                }), L({
                                     notebookPath: p,
-                                    fullNotebookPath: `${O.PageConfig.getOption("serverRoot")}/${p}`,
+                                    fullNotebookPath: `${T.PageConfig.getOption("serverRoot")}/${p}`,
                                     sitePackagesPath: m,
                                     scanSettings: t
                                 })
                             }
                         } else await new i.Dialog({
                             title: "No Notebook selected",
                             body: "Cannot run scan because there is no notebook selected.",
                             focusNodeSelector: "input",
                             buttons: [i.Dialog.cancelButton({
                                 label: "Close"
                             })]
                         }).launch()
                     };
-                    return M().createElement(M().Fragment, null, M().createElement(xe, null), M().createElement("div", {
-                        className: me.wrapper
-                    }, p ? M().createElement("p", {
-                        className: me.filepath
-                    }, M().createElement(v.react, {
-                        className: me.notebookIcon
-                    }), D().basename(p)) : null, M().createElement(_e, {
+                    return _().createElement(_().Fragment, null, _().createElement(Ne, null), _().createElement("div", {
+                        className: fe.wrapper
+                    }, p ? _().createElement("p", {
+                        className: fe.filepath
+                    }, _().createElement(v.react, {
+                        className: fe.notebookIcon
+                    }), D().basename(p)) : null, _().createElement(Ie, {
                         notebookPath: p
-                    }), p && M().createElement(De, {
-                        kernelName: g,
+                    }), p && _().createElement(He, {
+                        kernelName: C,
                         sitePackagesPath: m,
                         loading: b
-                    }), M().createElement(ke, {
+                    }), _().createElement(we, {
                         results: l,
                         notebookPath: p
-                    }), p && l[p] && l[p].isDirty && M().createElement(Ne, null), M().createElement(Le, {
+                    }), p && l[p] && l[p].isDirty && _().createElement(Oe, {
+                        message: "The notebook contents have changed since the last run. The results may be outdated.",
+                        level: F.WARN
+                    }), E && _().createElement(Oe, {
+                        message: "Could not connect to the NB Defense server. Make sure to enable the NB Defense server extension.",
+                        level: F.ERROR
+                    }), _().createElement(_e, {
                         isLoading: void 0 !== p && p in l && l[p].isLoading,
-                        onClick: y,
-                        scanExists: !(!p || !l[p])
-                    }), p && l[p] && M().createElement(M().Fragment, null, !l[p].isLoading && l[p].report && M().createElement(J, {
+                        onClick: I,
+                        scanExists: !(!p || !l[p]),
+                        disabled: E
+                    }), p && l[p] && _().createElement(_().Fragment, null, !l[p].isLoading && l[p].report && _().createElement(ee, {
                         scannedNotebook: r,
                         results: l[p].report,
                         scanHasErrors: ((null === (a = l[p].error) || void 0 === a ? void 0 : a.length) || 0) > 0
-                    }), M().createElement(Ie, {
+                    }), _().createElement(Te, {
                         errors: l[p].error
                     })), p && l[p] && Object.values(l[p].portals).flat(1)))
                 },
-                Te = (0, H.oB)({
+                Be = (0, H.oB)({
                     display: "flex",
                     flexDirection: "column",
                     minWidth: "300px",
                     color: "var(--jp-ui-font-color1)",
                     background: "var(--jp-layout-color1)",
                     fontSize: "var(--jp-ui-font-size1)",
                     overflowY: "auto"
                 });
-            class He extends i.ReactWidget {
+            class Ve extends i.ReactWidget {
                 constructor(e, t, n) {
-                    super(n), this.node.id = "NBDefenseSession-root", this.addClass(Te), this._notebookTracker = e, this._settings = t, this._runScanSignal = new _.Signal(this), this._isContextualHelpVisible = t.get(d).composite || !1, this._isNBDefenseDropdownVisible = t.get(p).composite || !1
+                    super(n), this.node.id = "NBDefenseSession-root", this.addClass(Be), this._notebookTracker = e, this._settings = t, this._runScanSignal = new y.Signal(this), this._isContextualHelpVisible = t.get(d).composite || !1, this._isNBDefenseDropdownVisible = t.get(p).composite || !1
                 }
                 render() {
-                    return console.log("@settings", this._settings), M().createElement(M().Fragment, null, M().createElement(Oe, {
+                    return console.log("@settings", this._settings), _().createElement(_().Fragment, null, _().createElement(Ae, {
                         notebookTracker: this._notebookTracker,
                         runScanSignal: this.runScanSignal,
                         isContextualHelpVisible: this._isContextualHelpVisible,
                         isNBDefenseDropdownVisible: this._isNBDefenseDropdownVisible,
                         settings: this._settings
                     }))
                 }
@@ -1197,31 +1222,31 @@
                 setContextualHelpVisible(e) {
                     this._isContextualHelpVisible = e, this.update()
                 }
                 setNBDefenseDropdownVisible(e) {
                     this._isNBDefenseDropdownVisible = e, this.update()
                 }
             }
-            const Re = "nbdefense-jupyter:plugin",
-                Ve = {
-                    id: Re,
+            const je = "nbdefense-jupyter:plugin",
+                Ue = {
+                    id: je,
                     autoStart: !0,
                     requires: [s.ILayoutRestorer, o.INotebookTracker, a.ISettingRegistry],
                     activate: async (e, t, n, s) => {
                         let o;
                         try {
-                            o = await s.load(Ve.id)
+                            o = await s.load(Ue.id)
                         } catch (e) {
                             console.error("Failed to load settings for nbdefense-jupyter.", e)
                         }
                         if (o) {
-                            const s = new He(n, o);
-                            s.id = "jp-nbdefense-sessions", s.title.icon = g, s.title.caption = "NBDefense", t.add(s, "nbdefense-sessions"), e.shell.add(s, "left", {
+                            const s = new Ve(n, o);
+                            s.id = "jp-nbdefense-sessions", s.title.icon = C, s.title.caption = "NBDefense", t.add(s, "nbdefense-sessions"), e.shell.add(s, "left", {
                                 rank: 200
-                            }), e.docRegistry.addWidgetExtension("Notebook", new l(s, e.shell)), e.docRegistry.addWidgetExtension("Notebook", new C(s, e.shell, o))
+                            }), e.docRegistry.addWidgetExtension("Notebook", new l(s, e.shell)), e.docRegistry.addWidgetExtension("Notebook", new g(s, e.shell, o))
                         }
                     }
                 },
-                Ae = Ve
+                We = Ue
         }
     }
 ]);
```

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/239.1c003b0dfd58bc7823a8.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/452.26450d70ddf6735bc3a7.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/500.97d1a5336e530d36f1c4.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/502.ab49aeea7a0fb1ad88e8.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/676.6137834929c84786225d.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/747.5ffca1b512bb6d3e1574.js`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/remoteEntry.a4d194721ddf3be27f37.js` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/remoteEntry.52422cb5d5bada194ec0.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, u, l, f, s, d, c, p, b, h, v, m, g = {
+    var e, r, t, a, n, o, i, u, l, f, s, d, c, p, h, b, v, m, g = {
             774: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(239), t.e(271), t.e(117)]).then((() => () => t(117))),
-                        "./extension": () => Promise.all([t.e(239), t.e(271), t.e(117)]).then((() => () => t(117))),
+                        "./index": () => Promise.all([t.e(239), t.e(271), t.e(661)]).then((() => () => t(661))),
+                        "./extension": () => Promise.all([t.e(239), t.e(271), t.e(661)]).then((() => () => t(661))),
                         "./style": () => t.e(747).then((() => () => t(747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
@@ -43,33 +43,33 @@
         }), r
     }, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        117: "e6844c28c0311e09d7d5",
         239: "1c003b0dfd58bc7823a8",
         271: "a39eca00e565943710ab",
         355: "e71f4acc9570680d68e9",
         452: "26450d70ddf6735bc3a7",
         500: "97d1a5336e530d36f1c4",
         502: "ab49aeea7a0fb1ad88e8",
         654: "0b96d4d60115144c75b2",
+        661: "42dcb7cf7c20838bfd42",
         676: "6137834929c84786225d",
         747: "5ffca1b512bb6d3e1574"
     } [e] + ".js?v=" + {
-        117: "e6844c28c0311e09d7d5",
         239: "1c003b0dfd58bc7823a8",
         271: "a39eca00e565943710ab",
         355: "e71f4acc9570680d68e9",
         452: "26450d70ddf6735bc3a7",
         500: "97d1a5336e530d36f1c4",
         502: "ab49aeea7a0fb1ad88e8",
         654: "0b96d4d60115144c75b2",
+        661: "42dcb7cf7c20838bfd42",
         676: "6137834929c84786225d",
         747: "5ffca1b512bb6d3e1574"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -123,15 +123,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("date-fns", "2.29.3", (() => w.e(500).then((() => () => w(500))))), u("nbdefense-jupyter", "1.0.3", (() => Promise.all([w.e(239), w.e(271), w.e(117)]).then((() => () => w(117))))), u("react-animate-height", "0", (() => Promise.all([w.e(271), w.e(452)]).then((() => () => w(452))))), u("react-use-websocket", "3.0.0", (() => Promise.all([w.e(676), w.e(271)]).then((() => () => w(676))))), u("use-event-callback", "0.1.0", (() => Promise.all([w.e(271), w.e(355)]).then((() => () => w(355)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("date-fns", "2.29.3", (() => w.e(500).then((() => () => w(500))))), u("nbdefense-jupyter", "1.0.4", (() => Promise.all([w.e(239), w.e(271), w.e(661)]).then((() => () => w(661))))), u("react-animate-height", "0", (() => Promise.all([w.e(271), w.e(452)]).then((() => () => w(452))))), u("react-use-websocket", "3.0.0", (() => Promise.all([w.e(676), w.e(271)]).then((() => () => w(676))))), u("use-event-callback", "0.1.0", (() => Promise.all([w.e(271), w.e(355)]).then((() => () => w(355)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -204,16 +204,16 @@
                     l = !1
                 } else "s" != d && "n" != d && (l = !1, u--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
-            var b = e[i];
-            c.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? o(b, r) : !p())
+            var h = e[i];
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = w.S[e];
         if (!t || !w.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
@@ -224,52 +224,52 @@
         return o(a, n) || "undefined" != typeof console && console.warn && console.warn(l(e, t, n, a)), d(e[t][n])
     }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, d = e => (e.loaded = 1, e.get()), p = (c = e => function(r, t, a, n) {
         var o = w.I(r);
         return o && o.then ? o.then(e.bind(e, r, w.S[r], t, a, n)) : e(r, w.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), b = c(((e, r, t, a, n) => {
+    })(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), h = c(((e, r, t, a, n) => {
         var o = r && w.o(r, t) && s(r, t, a);
         return o ? d(o) : n()
-    })), h = {}, v = {
+    })), b = {}, v = {
         271: () => p("default", "react", [1, 17, 0, 1]),
         33: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 3]),
         38: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 3]),
         123: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 3]),
         142: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 3]),
-        161: () => b("default", "react-use-websocket", [4, 3, 0, 0], (() => w.e(676).then((() => () => w(676))))),
+        161: () => h("default", "react-use-websocket", [4, 3, 0, 0], (() => w.e(676).then((() => () => w(676))))),
         456: () => p("default", "react-dom", [1, 17, 0, 1]),
         502: () => p("default", "@jupyterlab/ui-components", [1, 3, 6, 3]),
-        554: () => b("default", "use-event-callback", [2, 0, 1, 0], (() => w.e(654).then((() => () => w(355))))),
+        554: () => h("default", "use-event-callback", [2, 0, 1, 0], (() => w.e(654).then((() => () => w(355))))),
         687: () => p("default", "@jupyterlab/application", [1, 3, 6, 3]),
-        706: () => b("default", "react-animate-height", [1, 3, 0, 4], (() => w.e(502).then((() => () => w(452))))),
+        706: () => h("default", "react-animate-height", [1, 3, 0, 4], (() => w.e(502).then((() => () => w(452))))),
         820: () => p("default", "@jupyterlab/services", [1, 6, 6, 3]),
-        830: () => b("default", "date-fns", [1, 2, 29, 3], (() => w.e(500).then((() => () => w(500))))),
+        830: () => h("default", "date-fns", [1, 2, 29, 3], (() => w.e(500).then((() => () => w(500))))),
         840: () => p("default", "@lumino/signaling", [1, 1, 10, 0]),
         923: () => p("default", "@lumino/disposable", [1, 1, 10, 0])
     }, m = {
-        117: [33, 38, 123, 142, 161, 456, 502, 554, 687, 706, 820, 830, 840, 923],
-        271: [271]
+        271: [271],
+        661: [33, 38, 123, 142, 161, 456, 502, 554, 687, 706, 820, 830, 840, 923]
     }, w.f.consumes = (e, r) => {
         w.o(m, e) && m[e].forEach((e => {
-            if (w.o(h, e)) return r.push(h[e]);
+            if (w.o(b, e)) return r.push(b[e]);
             var t = r => {
-                    h[e] = 0, w.m[e] = t => {
+                    b[e] = 0, w.m[e] = t => {
                         delete w.c[e], t.exports = r()
                     }
                 },
                 a = r => {
-                    delete h[e], w.m[e] = t => {
+                    delete b[e], w.m[e] = t => {
                         throw delete w.c[e], r
                     }
                 };
             try {
                 var n = v[e]();
-                n.then ? r.push(h[e] = n.then(t).catch(a)) : t(n)
+                n.then ? r.push(b[e] = n.then(t).catch(a)) : t(n)
             } catch (e) {
                 a(e)
             }
         }))
     }, (() => {
         var e = {
             815: 0
```

### Comparing `nbdefense_jupyter-1.0.3/nbdefense_jupyter/labextension/static/third-party-licenses.json` & `nbdefense_jupyter-1.0.4/nbdefense_jupyter/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/.gitignore` & `nbdefense_jupyter-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/LICENSE` & `nbdefense_jupyter-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/README.md` & `nbdefense_jupyter-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/pyproject.toml` & `nbdefense_jupyter-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nbdefense_jupyter-1.0.3/PKG-INFO` & `nbdefense_jupyter-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdefense_jupyter
-Version: 1.0.3
+Version: 1.0.4
 Summary: NB Defense Jupyter Lab Extension
 Project-URL: Homepage, https://protectai.com
 Project-URL: Bug Tracker, https://protectai.com/contact-us
 Project-URL: Repository, https://github.com/protectai/nbdefense-jupyter.git
 Author-email: ProtectAI <support@protectai.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
```

