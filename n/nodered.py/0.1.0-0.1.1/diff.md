# Comparing `tmp/nodered.py-0.1.0.tar.gz` & `tmp/nodered.py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodered.py-0.1.0.tar", last modified: Fri Apr 28 05:53:59 2023, max compression
+gzip compressed data, was "nodered.py-0.1.1.tar", last modified: Sat Apr 29 04:47:27 2023, max compression
```

## Comparing `nodered.py-0.1.0.tar` & `nodered.py-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-28 05:53:59.500000 nodered.py-0.1.0/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.0/LICENSE
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1901 2023-04-28 05:53:59.590000 nodered.py-0.1.0/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1585 2023-04-28 05:41:03.000000 nodered.py-0.1.0/README.md
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-28 05:53:59.500000 nodered.py-0.1.0/nodered.py.egg-info/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1901 2023-04-28 05:53:59.000000 nodered.py-0.1.0/nodered.py.egg-info/PKG-INFO
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      412 2023-04-28 05:53:59.000000 nodered.py-0.1.0/nodered.py.egg-info/SOURCES.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 05:53:59.000000 nodered.py-0.1.0/nodered.py.egg-info/dependency_links.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-04-28 05:53:59.000000 nodered.py-0.1.0/nodered.py.egg-info/requires.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       37 2023-04-28 05:53:59.000000 nodered.py-0.1.0/nodered.py.egg-info/top_level.txt
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.0/nodered.py.egg-info/zip-safe
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-28 05:53:59.500000 nodered.py-0.1.0/noderedpy/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      288 2023-04-28 05:52:51.000000 nodered.py-0.1.0/noderedpy/__init__.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6385 2023-04-28 05:14:06.000000 nodered.py-0.1.0/noderedpy/_nodered.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6469 2023-04-28 05:24:44.000000 nodered.py-0.1.0/noderedpy/_server.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     4998 2023-04-28 04:17:23.000000 nodered.py-0.1.0/noderedpy/_templates.py
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      794 2023-04-28 05:18:07.000000 nodered.py-0.1.0/noderedpy/decorator.py
-drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-28 05:53:59.500000 nodered.py-0.1.0/noderedpy/node-red-starter/
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1727 2023-04-28 01:34:09.000000 nodered.py-0.1.0/noderedpy/node-red-starter/index.js
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.0/noderedpy/node-red-starter/package.json
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-04-28 05:53:59.590000 nodered.py-0.1.0/setup.cfg
--rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1044 2023-04-28 05:53:24.000000 nodered.py-0.1.0/setup.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1065 2023-04-28 05:27:55.000000 nodered.py-0.1.1/LICENSE
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1900 2023-04-29 04:47:27.380000 nodered.py-0.1.1/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1584 2023-04-29 03:19:05.000000 nodered.py-0.1.1/README.md
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/nodered.py.egg-info/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1900 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/PKG-INFO
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      412 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      163 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/requires.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       37 2023-04-29 04:47:27.000000 nodered.py-0.1.1/nodered.py.egg-info/top_level.txt
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        1 2023-04-28 03:54:24.000000 nodered.py-0.1.1/nodered.py.egg-info/zip-safe
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/noderedpy/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      288 2023-04-29 04:45:51.000000 nodered.py-0.1.1/noderedpy/__init__.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     7510 2023-04-29 04:31:59.000000 nodered.py-0.1.1/noderedpy/_nodered.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     6406 2023-04-28 10:06:27.000000 nodered.py-0.1.1/noderedpy/_server.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     8536 2023-04-29 04:32:28.000000 nodered.py-0.1.1/noderedpy/_templates.py
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      794 2023-04-28 05:18:07.000000 nodered.py-0.1.1/noderedpy/decorator.py
+drwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)        0 2023-04-29 04:47:27.320000 nodered.py-0.1.1/noderedpy/node-red-starter/
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     2398 2023-04-29 01:58:51.000000 nodered.py-0.1.1/noderedpy/node-red-starter/index.js
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)      296 2023-04-27 11:00:04.000000 nodered.py-0.1.1/noderedpy/node-red-starter/package.json
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)       38 2023-04-29 04:47:27.380000 nodered.py-0.1.1/setup.cfg
+-rwxrwxrwx   0 shlee-d-1-nb   (501) staff       (20)     1044 2023-04-28 05:53:24.000000 nodered.py-0.1.1/setup.py
```

### Comparing `nodered.py-0.1.0/LICENSE` & `nodered.py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.0/PKG-INFO` & `nodered.py-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -86,8 +86,8 @@
 - standalone(with webview)
 ```python
 server.start("{title}")
 ```
 <br/><br/>
 
 ## Todos
-[ ] type support for "list" and "dict".
+[x] type support for "list" and "dict"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.0 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.1 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
@@ -20,8 +20,8 @@
 (__dirname, ".node-red"), "/node-red", 1880 ) ) ```
 ### register Node ```python @register("test") def test(props:dict, msg:dict) -
 > dict: # user codes here return msg ``` - See noredpy.decorator.register
 function for details
 ### start server - default server ```python server.start("{port}") ``` -
 standalone(with webview) ```python server.start("{title}") ```
 
-## Todos [ ] type support for "list" and "dict".
+## Todos [x] type support for "list" and "dict"
```

### Comparing `nodered.py-0.1.0/README.md` & `nodered.py-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,8 +74,8 @@
 - standalone(with webview)
 ```python
 server.start("{title}")
 ```
 <br/><br/>
 
 ## Todos
-[ ] type support for "list" and "dict".
+[x] type support for "list" and "dict"
```

#### html2text {}

```diff
@@ -15,8 +15,8 @@
 (__dirname, ".node-red"), "/node-red", 1880 ) ) ```
 ### register Node ```python @register("test") def test(props:dict, msg:dict) -
 > dict: # user codes here return msg ``` - See noredpy.decorator.register
 function for details
 ### start server - default server ```python server.start("{port}") ``` -
 standalone(with webview) ```python server.start("{title}") ```
 
-## Todos [ ] type support for "list" and "dict".
+## Todos [x] type support for "list" and "dict"
```

### Comparing `nodered.py-0.1.0/nodered.py.egg-info/PKG-INFO` & `nodered.py-0.1.1/nodered.py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodered.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: make python function to Node-RED node
 Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev
 Author-email: this.dev.somehit@gmail.com
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -86,8 +86,8 @@
 - standalone(with webview)
 ```python
 server.start("{title}")
 ```
 <br/><br/>
 
 ## Todos
-[ ] type support for "list" and "dict".
+[x] type support for "list" and "dict"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nodered.py Version: 0.1.0 Summary: make python
+Metadata-Version: 2.1 Name: nodered.py Version: 0.1.1 Summary: make python
 function to Node-RED node Home-page: https://github.com/oyajiDev/NodeRED.py
 Author: oyajiDev Author-email: this.dev.somehit@gmail.com License: MIT license
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE
                            ****** NodeRED.py ******
                      make python function to Node-RED node
 
@@ -20,8 +20,8 @@
 (__dirname, ".node-red"), "/node-red", 1880 ) ) ```
 ### register Node ```python @register("test") def test(props:dict, msg:dict) -
 > dict: # user codes here return msg ``` - See noredpy.decorator.register
 function for details
 ### start server - default server ```python server.start("{port}") ``` -
 standalone(with webview) ```python server.start("{title}") ```
 
-## Todos [ ] type support for "list" and "dict".
+## Todos [x] type support for "list" and "dict"
```

### Comparing `nodered.py-0.1.0/noderedpy/_nodered.py` & `nodered.py-0.1.1/noderedpy/_nodered.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 from . import __path__
 
 
 class RED:
     """
     Node-RED manager class
     """
-    def __init__(self, node_red_user_dir:str, node_red_admin_root:str, node_red_port:int = 1880):
+    def __init__(self, user_dir:str, admin_root:str, port:int = 1880, show_default_category:bool = True):
         """
         Set configs of Node-RED and setup
 
         Parameters
         ----------
-        node_red_user_dir: str, required
+        user_dir: str, required
             userDir of Node-RED settings
-        node_red_admin_root: str, required
+        admin_root: str, required
             httpAdminRoot of Node-RED settings
-        node_red_port: int, default 1880
+        port: int, default 1880
             port of Node-RED server
+        show_default_category: bool, default True
+            show default categories of Node-RED or not
         """
-        self.node_red_user_dir, self.node_red_admin_root, self.node_red_port =\
-            node_red_user_dir, node_red_admin_root, node_red_port
+        self.user_dir, self.admin_root, self.port, self.show_default_category =\
+            user_dir, admin_root, port, show_default_category
 
         # setup Node-RED starter
         subprocess.call(
             [ "npm", "install" ],
             stdout = subprocess.DEVNULL,
             cwd = os.path.join(__path__[0], "node-red-starter")
         )
@@ -66,17 +68,18 @@
         if callback:
             threading.Thread(target = self.__on_started, args = (callback,), daemon = True).start()
 
         # set subprocess args
         args = [
             "node",
             "index.js",
-            f"--user-dir={self.node_red_user_dir}",
-            f"--admin-root={self.node_red_admin_root}",
-            f"--port={self.node_red_port}"
+            f"--user-dir={self.user_dir}",
+            f"--admin-root={self.admin_root}",
+            f"--port={self.port}",
+            f"--show-default-category={'true' if self.show_default_category else 'false'}"
         ]
         if server:
             args.append(
                 f"--user-category={','.join(list(set([ node.category for node in server.registered_nodes ])))}"
             )
 
         # run Node-RED server
@@ -100,15 +103,15 @@
     def __stop(self):
         import psutil, signal
 
         killed = False
         for process in psutil.process_iter():
             try:
                 for conns in process.connections(kind = "inet"):
-                    if conns.laddr.port == self.node_red_port:
+                    if conns.laddr.port == self.port:
                         process.send_signal(signal.SIGTERM)
                         killed = True
                         break
             except psutil.AccessDenied:
                 pass
 
             if killed:
@@ -124,37 +127,61 @@
         self.__stop()
 
 
 class NodeProperty:
     """
     Property for Node function
     """
-    def __init__(self, name:str, type:Literal["str", "int", "float"], default_value:Any = None, required:bool = False):
+    def __init__(self, name:str, type:Literal["str", "int", "float", "list", "dict"], default_value:Any = None, required:bool = False, display_icon:str = None):
         """
         Property information for Node function
 
         Parameters
         ----------
         name: str, required
             name of Property
         type: Literal["str", "int", "float"], required
             type of Property
         default_value: Any, default None
             default value of Property
         required: bool, default False
             set Property is required or not
+        display_icon: str, default None
+            icon for Node-RED node display
         """
         if " " in name.strip():
             raise NameError("Property name cannot contain space!")
         
-        if not type in ("str", "int", "float"):
-            raise TypeError("Currently supported types: [ 'str', 'int', 'float' ]")
+        if not type in ("str", "int", "float", "list", "dict"):
+            raise TypeError("Currently supported types: [ 'str', 'int', 'float', 'list', 'dict' ]")
+        
+        if default_value is not None and not isinstance(default_value, ( str, int, float, list, dict )):
+            raise TypeError("Currently supported value types: [ str, int, float, list, dict ]")
 
         self.name, self.type, self.default_value, self.required =\
             name, type, default_value, required
+        
+        if display_icon is None:
+            if type in ( "int", "float" ):
+                self.display_icon = "fa fa-sort-numeric-asc"
+            elif type == "str":
+                self.display_icon = "fa fa-font"
+            elif type == "list":
+                self.display_icon = "fa fa-list"
+            elif type == "dict":
+                self.display_icon = "fa fa-code"
+        else:
+            self.display_icon = display_icon
+        
+    @property
+    def display_name(self) -> str:
+        return " ".join([
+            item.capitalize()
+            for item in self.name.split("_")
+        ])
 
 class Node:
     def __init__(self, name:str, category:str, properties:List[NodeProperty], node_func:MethodType):
         if " " in name.strip():
             raise NameError("Node name cannot contain spaces!")
         
         if "-" in category.strip() or "," in category.strip():
```

### Comparing `nodered.py-0.1.0/noderedpy/_server.py` & `nodered.py-0.1.1/noderedpy/_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             text = json.dumps(node.run(data["props"], data["msg"])),
             content_type = "application/json"
         )
 
     def __on_started(self):
         if self.__show_browser:
             import webbrowser
-            webbrowser.open_new(f"http://127.0.0.1:{self.__red.node_red_port}/node-red")
+            webbrowser.open_new(f"http://127.0.0.1:{self.__red.port}/node-red")
 
         if self.__start_callback:
             self.__start_callback()
 
 
     def register(self, node_func:MethodType, name:str, category:str = "nodered_py", properties:List[NodeProperty] = []):
         """
@@ -77,24 +77,24 @@
         callback: MethodType, default None
             callback when Server started
         """
         self.__port, self.__show_browser, self.__start_callback = port, show_browser, callback
         self.__red.start(callback = self.__on_started, server = Server)
 
         # remove existing nodes
-        for node_dir in glob(os.path.join(self.__red.node_red_user_dir, "node_modules", "nodered-py-*")):
+        for node_dir in glob(os.path.join(self.__red.user_dir, "node_modules", "nodered-py-*")):
             shutil.rmtree(node_dir)
 
         # create nodes
         for node in Server.registered_nodes:
-            node.create(self.__red.node_red_user_dir, port)
+            node.create(self.__red.user_dir, port)
 
         # map nodes to route
         self.add_routes([
-            web.get("", lambda _: web.HTTPFound(f"http://127.0.0.1:{self.__red.node_red_port}/node-red")),
+            web.get("", lambda _: web.HTTPFound(f"http://127.0.0.1:{self.__red.port}/node-red")),
             web.post("/nodes/{node_name}", lambda req: self.__call_node(req, req.match_info["node_name"]))
         ])
 
         # start server
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
         server = loop.create_server(self.make_handler(), host = "127.0.0.1", port = port)
@@ -174,20 +174,20 @@
             default y location of webview window
         debug: bool, default False
             debug(devtools) or not
         port: int, default 1881
             port for Server
         default_root: str, default None
             default url root to show
-            if None, use node_red_admin_root of Node-RED settings
+            if None, use admin_root of Node-RED settings
         """
-        default_root = self.__red.node_red_admin_root if default_root is None else default_root
+        default_root = self.__red.admin_root if default_root is None else default_root
         if not default_root.startswith("/"):
             raise ValueError("default_root must startswith '/'!")
 
         import webview
 
         webview.initialize("cocoa" if sys.platform == "darwin" else "cef" if sys.platform == "win32" else "qt")
         win = webview.create_window(title, width = width, height = height, x = x, y = y)
         win.events.closing += self.__server.stop
 
-        webview.start(lambda: self.__server.start(port, False, lambda: win.load_url(f"http://127.0.0.1:{self.__red.node_red_port}{default_root}")), debug = debug)
+        webview.start(lambda: self.__server.start(port, False, lambda: win.load_url(f"http://127.0.0.1:{self.__red.port}{default_root}")), debug = debug)
```

### Comparing `nodered.py-0.1.0/noderedpy/decorator.py` & `nodered.py-0.1.1/noderedpy/decorator.py`

 * *Files identical despite different names*

### Comparing `nodered.py-0.1.0/noderedpy/node-red-starter/index.js` & `nodered.py-0.1.1/noderedpy/node-red-starter/index.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -18,14 +18,17 @@
 parser.add_argument("--port", {
     type: "int"
 });
 parser.add_argument("--user-category", {
     type: "str",
     default: ""
 });
+parser.add_argument("--show-default-category", {
+    type: "str"
+});
 const args = parser.parse_args();
 
 // parse user-category
 if (args["user_category"] == "") {
     args["user_category"] = [];
 } else {
     const raw_categories = args["user_category"].split(",");
@@ -37,26 +40,47 @@
 
 
 // create express and node-red server
 const exapp = express();
 const RED_server = http.createServer(exapp);
 
 // set configs
-RED.init(RED_server, {
+let opts = {
     editorTheme: {
         projects: {
             enabled: false
         }
     },
     httpAdminRoot: args["admin_root"].startsWith("/") ? args["admin_root"] : `/${args["admin_root"]}`,
     httpNodeRoot: "/",
     flowFile: "noderedpy.json",
     userDir: args["user_dir"],
-    paletteCategories: args["user_category"].concat(["subflows", "flow", "input", "output", "function", "parser", "social", "mobile", "storage", "analysis", "advanced"])
-});
+    paletteCategories: args["show_default_category"] == "true" ? args["user_category"].concat(["subflows", "common", "function", "network", "sequence", "parser", "storage"]) : args["user_category"]
+};
+// if (![ "None", "null", "" ].includes(args["admin_auth"])) {
+//     opts.adminAuth = {
+//         type: "credentials",
+//         users: [
+//             {
+//                 username: "nodered-py",
+//                 password: args["admin_auth"],
+//                 permissions: "*"
+//             }
+//         ]
+//     };
+//     opts.httpNodeAuth = {
+//         user: "nodered-py", pass: args["admin_auth"]
+//     };
+
+//     fs.writeFileSync(path.join(args["user_dir"], "settings.js"), `
+// module.exports = ${JSON.stringify(opts, space = 4)};
+// `);
+// }
+
+RED.init(RED_server, opts);
 
 // node-red default routes
 exapp.use("/", express.static("web"));
 exapp.use(RED.settings.httpAdminRoot, RED.httpAdmin);
 exapp.use(RED.settings.httpNodeRoot, RED.httpNode);
 
 // start node-red
```

### Comparing `nodered.py-0.1.0/setup.py` & `nodered.py-0.1.1/setup.py`

 * *Files identical despite different names*

