# Comparing `tmp/sneaksmc-0.0.6.tar.gz` & `tmp/sneaksmc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sneaksmc-0.0.6.tar", last modified: Tue Apr 11 20:25:21 2023, max compression
+gzip compressed data, was "sneaksmc-0.0.7.tar", last modified: Sat Apr 29 14:48:22 2023, max compression
```

## Comparing `sneaksmc-0.0.6.tar` & `sneaksmc-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.6/README.rst
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/setup.cfg
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-11 20:25:02.000000 sneaksmc-0.0.6/setup.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/sneaksmc/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.6/sneaksmc/__init__.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     3461 2023-04-11 13:50:50.000000 sneaksmc-0.0.6/sneaksmc/client.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.6/sneaksmc/crypt.py
--rw-rw-r--   0 tsy       (1000) tsy       (1000)    23642 2023-04-11 20:23:45.000000 sneaksmc-0.0.6/sneaksmc/server.py
-drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-11 20:25:21.782092 sneaksmc-0.0.6/sneaksmc.egg-info/
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/PKG-INFO
--rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/SOURCES.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/dependency_links.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/requires.txt
--rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-11 20:25:21.000000 sneaksmc-0.0.6/sneaksmc.egg-info/top_level.txt
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       79 2023-04-11 13:58:02.000000 sneaksmc-0.0.7/README.rst
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      107 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/setup.cfg
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      407 2023-04-29 14:46:26.000000 sneaksmc-0.0.7/setup.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/sneaksmc/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       73 2023-04-11 13:54:48.000000 sneaksmc-0.0.7/sneaksmc/__init__.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     3665 2023-04-29 12:46:43.000000 sneaksmc-0.0.7/sneaksmc/client.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)     6390 2023-04-11 13:50:17.000000 sneaksmc-0.0.7/sneaksmc/crypt.py
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)    25039 2023-04-29 14:15:29.000000 sneaksmc-0.0.7/sneaksmc/server.py
+drwxrwxr-x   0 tsy       (1000) tsy       (1000)        0 2023-04-29 14:48:22.439231 sneaksmc-0.0.7/sneaksmc.egg-info/
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      268 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/PKG-INFO
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)      265 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        1 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)       13 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/requires.txt
+-rw-rw-r--   0 tsy       (1000) tsy       (1000)        9 2023-04-29 14:48:22.000000 sneaksmc-0.0.7/sneaksmc.egg-info/top_level.txt
```

### Comparing `sneaksmc-0.0.6/sneaksmc/client.py` & `sneaksmc-0.0.7/sneaksmc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,38 +45,42 @@
         # If the node is not coordinator then the request is dropped.
         # Sends its public key as the result will be encrypted
         r = send_client_request(type="GET", url="/start_analysis", body=pub_key, 
                                     receiver=self.coordinator_node, timeout=3.0)
         return r
         
     
-    def get_result(self, tries=100, ms=50):
-        """ Sends http request to coordinator node for the result of a requestes analysis operation.
+    def get_result(self, id, tries=100, ms=50):
+        """ Sends http request to coordinator node for the result of a requested analysis operation.
             Returns the result (if received) (response-code, response-msg) tuple, otherwise if not received, 
             returns from last message sent. Raises exception on error.
+            Returns immediately if given operation_id is not valid.
             Params:
                 @tries  : Max number of get-requests sent until giving up
                 @ms     : Sleep in ms between each request try. """
 
         if self.coordinator_node == None:
-            raise Exception("No SMC request has been sent to coordinator")
+            raise Exception("No SMC request has been sent to coordinator.")
         if tries <= 0 or ms < 0:
-            raise Exception("Invalid arguments tries=%d, ms=%d given" % (tries, ms))
+            raise Exception("Invalid arguments tries=%d, ms=%d given." % (tries, ms))
+        if id <= 0:
+            raise Exception("Invalid id (%d) given." % id)
 
-        pub_key = Crypt.key2string(self.ck.get_public_key())
+        #pub_key = Crypt.key2string(self.ck.get_public_key())
         response_code = 408
         response_msg = "Response timeout"
 
         # Request the result from coordinator. Asks every @ms until it receives the result.
         for i in range(0, tries):
-            r = send_client_request(type="GET", url="/get_result", body=pub_key, 
+            r = send_client_request(type="GET", url="/get_result", body=str(id), 
                                     receiver=self.coordinator_node, timeout=3.0)
             response_code = r[0]
             response_msg = r[1]
-            if response_code == 200:
+            if response_code  != 102:
+                # Server done processing request
                 break
             
             time.sleep(0.001*ms)
         
         return (response_code, response_msg)
     
     def shutdown(self):
```

### Comparing `sneaksmc-0.0.6/sneaksmc/crypt.py` & `sneaksmc-0.0.7/sneaksmc/crypt.py`

 * *Files identical despite different names*

### Comparing `sneaksmc-0.0.6/sneaksmc/server.py` & `sneaksmc-0.0.7/sneaksmc/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,20 +24,22 @@
 _server_address = None
 _server_nodefile = None
 _server_iscoordinator = False
 _server_coordinator_addr = None
 ck = Crypt()
 # Latest analysis result stored here
 _result_value = None
-# Offset that the coordinator sets on result to make sure no other nodes can read it.
-scramble_list = []
 
 _analysis_function = None
 _request_timeout_sec = 3
 
+# Offset that the coordinator sets on result to make sure no other nodes can read it.
+_operations = None
+
+
 def get_scramble():
     return random.randint(-1000000, 1000000)
 
 def get_machine_info():
     """ Returns machine host name and public ip. If no public ip is found 
         then returns ip as localhost (127.0.0.1)"""
 
@@ -52,28 +54,66 @@
         ip = '127.0.0.1'
     finally:
         s.close()
     
     return socket.gethostname(), ip
 
 
+class Operation():
+    def __init__(self):
+        self.operations = {}
+        self.id = 0
+    def _get_id(self):
+        # Returns a new valid operation id > 0
+        self.id += 1
+        return self.id
+    def add(self, scramble_list):
+        # Adds new operation
+        new_id = self._get_id()
+        self.operations[new_id] = [scramble_list, None]
+        return new_id
+    def get(self, id, remove=True):
+        # Return None if id doesn't exist
+        # Removes id from dictionary if remove=True
+        return self.operations.pop(int(id), None) if remove == True else self.operations.get(int(id), None)
+    def set_result(self, id, result):
+        # Sets the result for given operation id
+        x = self.get(int(id), False)
+        x[1] = result
+    def get_result(self, id):
+        # Returns result or None if result has not been set yet
+        x = self.get(int(id), False)
+        scramble_list = x[0]
+        result = x[1]
+        if result == None:
+            return None
+        for scramble in scramble_list:
+            result -= scramble
+        
+        # Remove result from dict
+        self.operations.pop(int(id))
+        return result
+
+
+
 def analysis(sum_data):
     """ Function to be overridden by user. Param @sum_data gives previous sum data and this function must return the new sum data after the analysis is complete.
         @sum_data will be None if it has not been previously set (first time).
     """
     return 1 if sum_data is None else sum_data + 10
 
 
 
 def run_server(coordinator=None, analysis_function=None, nodefile=None, ip=None, 
                 port=None, timeout=None, request_timout=None, min_nodes=1):
         """ Main function to run the server """
         global _server_nodefile, _server_ip, _server_port, _server_connected_ips
         global _analysis_function, _server_iscoordinator, _server_address, _request_timeout_sec
         global _server_coordinator_addr, _server_auto_shutdown
+        global _operations
 
         if timeout is not None:
             _server_auto_shutdown = timeout
         if request_timout is not None:
             _request_timeout_sec = request_timout
 
         if analysis_function is None:
@@ -83,14 +123,16 @@
         if ip is None:
             ip = host_ip
         if port is None:
             # Set random port between 49152->65535
             #port = random.randint(49152, 65535)
             # Default port used
             port = 8985
+        
+        _operations = Operation()
 
         _analysis_function = analysis_function
         _server_nodefile = nodefile
         _server_ip = ip
         _server_port = int(port)
         _server_iscoordinator = True if nodefile is not None else False
 
@@ -365,19 +407,18 @@
 
         elif self.path.startswith("/analysis_done"):
             global _result_value, _analysis_offset_value
 
             print("got analysis done")
             data_dict = json.loads(msg)
             result = data_dict['data']
-            # Remove all scrambles from result
-            for scramble in scramble_list:
-                result -= scramble
-            # Save result value
-            _result_value = str(result)
+            operation_id = data_dict['id']
+            # Save result
+            _operations.set_result(operation_id, result)
+            
             self.send_whole_response(200, "ok")
         
         elif self.path.startswith("/analysis"):
             print("Received analysis request")
             self.send_whole_response(200, "ok")
 
             # The decrypted message will be a dictonary in string format.
@@ -441,29 +482,35 @@
             print(_server_connected_ips)
             self.send_encrypted_msg("0")
             self.send_whole_response(200, "ok")
         
 
         # Shutdown
         elif self.path.startswith("/shutdown"):
-            self.send_whole_response(200, "okay shutting down")
+            self.send_whole_response(200, "ok")
             self.server.shutdown()
             exit(0)
         
         elif self.path.startswith("/get_result"):
             """ Client request the result from coordinator. """
             if not _server_iscoordinator:
                 raise Exception("Client sent get-result request to a node whose not coordinator.")
 
             print("Received result request")
-            if _result_value != None:
-                self.send_whole_response(200, _result_value)
-                #self.result_value = None
+
+            # Read the operation id from client
+            content_length = int(self.headers.get('Content-Length'))
+            data = self.rfile.read(content_length)
+            operation_id = int(data)
+            result = _operations.get_result(operation_id)
+
+            if result != None:
+                self.send_whole_response(200, result)
             else:
-                self.send_whole_response(404, "Not ready yet")
+                self.send_whole_response(102, "Not ready yet")
 
         
         elif self.path.startswith("/certificate"):
             # Only non coordinator node should get this request
             # If this node is the coordinator then raise an exception
             if _server_iscoordinator:
                 raise Exception("Coordinator node should not receive a certificate request from other nodes.")
@@ -473,30 +520,30 @@
             #     raise Exception("Connected node %s is not whitelisted within nodefile for coordinator" % str(self.client_address))
 
             self.send_whole_response(200, self.get_certificate())
            
         
         elif self.path.startswith("/start_analysis"):
             """ Start analysis request. Only coordinator will receive this request from a client. """
-            global scramble_list
 
             if not _server_iscoordinator:
                 self.send_whole_response(404, "Only coordinator should get a start_analysis request")
                 return
 
 
             content_length = int(self.headers.get('content-length', 0))
             value = self.rfile.read(content_length).decode()
 
             # Send a dictionary containing encrypted list of receivers (send_list)
             # and some analysis data sum (data) which is initialized with a given offset such that no node can know the current data sum.
             enc = []
-            # List of encrypted scramble values to each participant to hide their result
-            # from other nodes.
-            enc_dict = {'send_list': enc, 'data': 0}
+            scramble_list = []
+            operation_id = _operations.add(scramble_list)
+
+            enc_dict = {'send_list': enc, 'data': 0, 'id': operation_id}
 
             # Create sequence list of nodes to perform analysis of its data
             # This is such that the nodes know which node to forward the data to.
 
             # Add all nodes from certificate-file into a list with address and their public key
             node_list = []
             with open(certificate_file, "r") as f:
@@ -504,14 +551,16 @@
                     print(line)
                     addr, strkey = line.split("@")
                     node_list.append((addr, Crypt.string2key(strkey)))
             
             # Shuffle the node list to make the order random
             random.shuffle(node_list)
 
+            
+
             # Encrypt for each node who they should further their results to. The last node will further it back to the coordinator.
             for i in range(len(node_list)):
                 addr, key = node_list[i]
                 print(addr)
                 # Last node sends back to coordinator again (loops around)
                 if i >= len(node_list)-1:
                     scramble = get_scramble()
@@ -540,17 +589,17 @@
 
             status, content = self.send_encrypted_msg(order, url="/analysis", ip=first_node)
 
             if status != 200:
                 self.send_whole_response(404, "Error occurred: %s" % content)
                 raise Exception("Error starting analysis: %s" % content)
 
-            # Send ok response back to client.
+            # Send ok response (200) back to client with the created operation id.
             # The client have to ask for the result in a separate request.
-            self.send_whole_response(200, "ok")
+            self.send_whole_response(200, str(operation_id))
 
 
 
 def arg_parser():
     parser = argparse.ArgumentParser(prog="server", description="http server")
 
     parser.add_argument("-p", "--port", type=int, required=True,
```

