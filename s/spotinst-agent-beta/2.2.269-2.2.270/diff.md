# Comparing `tmp/spotinst-agent-beta-2.2.269.tar.gz` & `tmp/spotinst-agent-beta-2.2.270.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotinst-agent-beta-2.2.269.tar", last modified: Thu Apr 27 15:06:14 2023, max compression
+gzip compressed data, was "spotinst-agent-beta-2.2.270.tar", last modified: Sat Apr 29 19:45:22 2023, max compression
```

## Comparing `spotinst-agent-beta-2.2.269.tar` & `spotinst-agent-beta-2.2.270.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 15:06:14.076537 spotinst-agent-beta-2.2.269/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.269/LICENSE
--rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.269/MANIFEST.in
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 15:06:14.076336 spotinst-agent-beta-2.2.269/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.269/README.rst
--rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-27 15:06:14.076598 spotinst-agent-beta-2.2.269/setup.cfg
--rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-27 15:06:11.000000 spotinst-agent-beta-2.2.269/setup.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 15:06:14.072955 spotinst-agent-beta-2.2.269/spotinst_agent/
--rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.269/spotinst_agent/__init__.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.269/spotinst_agent/agent.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.269/spotinst_agent/agentinit.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.269/spotinst_agent/basemodule.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 15:06:14.068993 spotinst-agent-beta-2.2.269/spotinst_agent/data/
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 15:06:14.073624 spotinst-agent-beta-2.2.269/spotinst_agent/data/configuration/
--rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.269/spotinst_agent/data/configuration/basemodule.yml
--rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.269/spotinst_agent/data/configuration/spotinst-agent.yml
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 15:06:14.073918 spotinst-agent-beta-2.2.269/spotinst_agent/data/installation/
--rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.269/spotinst_agent/data/installation/agent-init.sh
--rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.269/spotinst_agent/scheduler.py
--rw-r--r--   0 ayeletc    (502) staff       (20)    10946 2023-04-27 15:06:05.000000 spotinst-agent-beta-2.2.269/spotinst_agent/taskmanager.py
--rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.269/spotinst_agent/utils.py
-drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-27 15:06:14.075987 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/
--rw-r--r--   0 ayeletc    (502) staff       (20)     1960 2023-04-27 15:06:14.000000 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/PKG-INFO
--rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-27 15:06:14.000000 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/SOURCES.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-27 15:06:14.000000 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/dependency_links.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       56 2023-04-27 15:06:14.000000 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/entry_points.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-27 15:06:14.000000 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/requires.txt
--rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-27 15:06:14.000000 spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/top_level.txt
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.481032 spotinst-agent-beta-2.2.270/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1065 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/LICENSE
+-rw-r--r--   0 ayeletc    (502) staff       (20)      181 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/MANIFEST.in
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-29 19:45:22.480856 spotinst-agent-beta-2.2.270/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1287 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/README.rst
+-rw-r--r--   0 ayeletc    (502) staff       (20)       38 2023-04-29 19:45:22.481085 spotinst-agent-beta-2.2.270/setup.cfg
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1392 2023-04-29 19:43:03.000000 spotinst-agent-beta-2.2.270/setup.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.478479 spotinst-agent-beta-2.2.270/spotinst_agent/
+-rw-r--r--   0 ayeletc    (502) staff       (20)    13080 2023-04-27 12:18:46.000000 spotinst-agent-beta-2.2.270/spotinst_agent/__init__.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     3116 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/agent.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9604 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/agentinit.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1129 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/basemodule.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.474868 spotinst-agent-beta-2.2.270/spotinst_agent/data/
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.478965 spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/
+-rw-r--r--   0 ayeletc    (502) staff       (20)      180 2023-03-12 08:32:58.000000 spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/basemodule.yml
+-rw-r--r--   0 ayeletc    (502) staff       (20)      727 2023-04-27 08:56:57.000000 spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/spotinst-agent.yml
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.479206 spotinst-agent-beta-2.2.270/spotinst_agent/data/installation/
+-rwxr-xr-x   0 ayeletc    (502) staff       (20)     6691 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/data/installation/agent-init.sh
+-rw-r--r--   0 ayeletc    (502) staff       (20)    21605 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/scheduler.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)    11053 2023-04-29 19:41:17.000000 spotinst-agent-beta-2.2.270/spotinst_agent/taskmanager.py
+-rw-r--r--   0 ayeletc    (502) staff       (20)     9420 2023-04-27 09:24:24.000000 spotinst-agent-beta-2.2.270/spotinst_agent/utils.py
+drwxr-xr-x   0 ayeletc    (502) staff       (20)        0 2023-04-29 19:45:22.480561 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/
+-rw-r--r--   0 ayeletc    (502) staff       (20)     1940 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/PKG-INFO
+-rw-r--r--   0 ayeletc    (502) staff       (20)      638 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/SOURCES.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)        1 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/dependency_links.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       55 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/entry_points.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       16 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/requires.txt
+-rw-r--r--   0 ayeletc    (502) staff       (20)       15 2023-04-29 19:45:22.000000 spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/top_level.txt
```

### Comparing `spotinst-agent-beta-2.2.269/LICENSE` & `spotinst-agent-beta-2.2.270/LICENSE`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/PKG-INFO` & `spotinst-agent-beta-2.2.270/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.269
+Version: 2.2.270
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 License-File: LICENSE
 
@@ -52,9 +51,7 @@
 MAKEFILE
 ~~~~~~~~~~~~~
 run 'make release'
 output file is located in the /dist folder
 
 Documentation
 =============
-
-
```

### Comparing `spotinst-agent-beta-2.2.269/README.rst` & `spotinst-agent-beta-2.2.270/README.rst`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/setup.py` & `spotinst-agent-beta-2.2.270/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='spotinst-agent-beta',
 
-    version="2.2.269",
+    version="2.2.270",
 
     description='Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.',
 
     long_description=description,
 
     # The project's main homepage.
     url='https://github.com/spotinst/spotinst-spectrum-agent',
```

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/__init__.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/agent.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/agent.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/agentinit.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/agentinit.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/basemodule.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/basemodule.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/data/configuration/spotinst-agent.yml` & `spotinst-agent-beta-2.2.270/spotinst_agent/data/configuration/spotinst-agent.yml`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/data/installation/agent-init.sh` & `spotinst-agent-beta-2.2.270/spotinst_agent/data/installation/agent-init.sh`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/scheduler.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/scheduler.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/taskmanager.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/taskmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,30 +138,31 @@
                 #         self.log.info("Module '{0}' already loaded".format(modname))
                 #         continue
 
                 if modname == "utils" or modname == "basemodule":
                     continue
 
                 # import module only if it exists for more than 1 second (had enough time to write the entire content)
-                # now = time.time()
-                # if now - mod_modification_time < 1:
-                #     self.log.info("Not loading file since it was created too recently: modified at %s, now is %s" % (mod_modification_time, now))
+                now = time.time()
+                if now - mod_modification_time < 1:
+                    self.log.info("Not loading file since it was created too recently: modified at %s, now is %s" % (mod_modification_time, now))
                 #     continue
-                time.sleep(30)
+                time.sleep(45)
                 try:
                     # Import the module
                     self.log.info("Importing %s" % modname)
                     mod = __import__(modname, globals(), locals(), ['*'])
                 except Exception as e:
                     # Log error
                     self.log.error("Failed to import module: %s. %s" % (modname, traceback.format_exc()))
                     continue
 
                 # Find all classes defined in the module
                 self.log.info("Finding classes defined in module " + str(modname))
+                self.log.info("Modname is" + mod + "string is " + str(mod) + "and his size is " + len(dir(mod)))
 
                 for attrname in dir(mod):
                     attr = getattr(mod, attrname)
                     # Only attempt to load classes that are infact classes but not the base Module class
                     self.log.debug("Checking " + str(modname) + " Attribute " + str(attrname))
                     self.log.info("Checking " + str(modname) + " Attribute " + str(attrname))
```

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent/utils.py` & `spotinst-agent-beta-2.2.270/spotinst_agent/utils.py`

 * *Files identical despite different names*

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/PKG-INFO` & `spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: spotinst-agent-beta
-Version: 2.2.269
+Version: 2.2.270
 Summary: Spectrum instance spotinst-agent that is able to run remote scripts, collect data, deploy applications and more.
 Home-page: https://github.com/spotinst/spotinst-spectrum-agent
 Author: Spotinst
 Author-email: service@spotinst.com
 License: MIT
 Keywords: spotinst agent infrastructure monitoring execution deployment
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 License-File: LICENSE
 
@@ -52,9 +51,7 @@
 MAKEFILE
 ~~~~~~~~~~~~~
 run 'make release'
 output file is located in the /dist folder
 
 Documentation
 =============
-
-
```

### Comparing `spotinst-agent-beta-2.2.269/spotinst_agent_beta.egg-info/SOURCES.txt` & `spotinst-agent-beta-2.2.270/spotinst_agent_beta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

