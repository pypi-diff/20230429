# Comparing `tmp/spotinst-agent-beta-2.2.270.tar.gz` & `tmp/spotinst-agent-beta-2.2.271.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.270.tar", last modified: Sat Apr 29 19:45:22 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.271.tar", last modified: Sat Apr 29 20:22:33 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.270.tar` & `spotinst-agent-beta-2.2.271.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.481032 spotinst-agent-beta-2.2.270/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-29 19:45:22.480856 spotinst-agent-beta-2.2.270/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-29 19:45:22.481085 spotinst-agent-beta-2.2.270/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-29 19:43:03.000000 spotinst-agent-beta-2.2.270/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.478479 spotinst-agent-beta-2.2.270/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.270/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.474868 spotinst-agent-beta-2.2.270/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.478965 spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.479206 spotinst-agent-beta-2.2.270/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    11053 2023-04-29 19:41:17.000000 spotinst-agent-beta-2.2.270/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.480561 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 20:22:33.037216 spotinst-agent-beta-2.2.271/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.271/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.271/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-29 20:22:33.036966 spotinst-agent-beta-2.2.271/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.271/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-29 20:22:33.037295 spotinst-agent-beta-2.2.271/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-29 20:22:30.000000 spotinst-agent-beta-2.2.271/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 20:22:33.027390 spotinst-agent-beta-2.2.271/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.271/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.271/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.271/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.271/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 20:22:33.018986 spotinst-agent-beta-2.2.271/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 20:22:33.030276 spotinst-agent-beta-2.2.271/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.271/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.271/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 20:22:33.031194 spotinst-agent-beta-2.2.271/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.271/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.271/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    11269 2023-04-29 20:22:20.000000 spotinst-agent-beta-2.2.271/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.271/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 20:22:33.036705 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-29 20:22:32.000000 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-29 20:22:32.000000 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-29 20:22:32.000000 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-29 20:22:32.000000 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-29 20:22:32.000000 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-29 20:22:32.000000 spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.270/LICENSE` & `spotinst-agent-beta-2.2.271/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/PKG-INFO` & `spotinst-agent-beta-2.2.271/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.270
+Version: 2.2.271
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.270/README.rst` & `spotinst-agent-beta-2.2.271/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/setup.py` & `spotinst-agent-beta-2.2.271/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.270",
+    version="2.2.271",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.271/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.271/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/taskmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,17 +129,17 @@
 
                 modname = f[:-3]
                 mod_modification_time = os.path.getmtime(os.path.join(path, f))
                 mod_modification_time_str = str(mod_modification_time)
                 self.log.info("Py file found: %s" % modname)
 
                 modules_list = [x.lower() for x in self.tasks.keys()]
-                # if modname in modules_list:
-                #     if self.tasks[modname]['modification_time'] == mod_modification_time_str:
-                #         self.log.info("Module '{0}' already loaded".format(modname))
+                if modname in modules_list:
+                    if self.tasks[modname]['modification_time'] == mod_modification_time_str:
+                        self.log.info("Module '{0}' already loaded".format(modname))
                 #         continue
 
                 if modname == "utils" or modname == "basemodule":
                     continue
 
                 # import module only if it exists for more than 1 second (had enough time to write the entire content)
                 now = time.time()
@@ -154,16 +154,21 @@
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
                     continue
 
                 # Find all classes defined in the module
                 self.log.info("Finding classes defined in module " + str(modname))
-                self.log.info("Modname is" + mod + "string is " + str(mod) + "and his size is " + len(dir(mod)))
 
+                try :
+                    self.log.info("Modname is" + mod + "string is " + str(mod) + "and his size is " + len(dir(mod)))
+                except Exception as e:
+                    # Log error
+                    self.log.error("Failed to log: %s. %s" % (modname, traceback.format_exc()))
+                    continue
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
                     self.log.info("Checking " + str(modname) + " Attribute " + str(attrname))
 
                     if inspect.isclass(attr) and isModule(attr) and attr != basemodule.Module:
```

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.271/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.270
+Version: 2.2.271
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.271/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

