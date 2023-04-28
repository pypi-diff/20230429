# Comparing `tmp/spikesafe-python-1.3.0.tar.gz` & `tmp/spikesafe-python-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spikesafe-python-1.3.0.tar", last modified: Tue Jan 10 22:24:55 2023, max compression
+gzip compressed data, was "spikesafe-python-1.4.5.tar", last modified: Tue Apr 25 21:52:41 2023, max compression
```

## Comparing `spikesafe-python-1.3.0.tar` & `spikesafe-python-1.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-01-10 22:24:55.345224 spikesafe-python-1.3.0/
--rw-rw-rw-   0        0        0     1928 2020-04-27 17:14:40.000000 spikesafe-python-1.3.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-01-10 22:24:55.277236 spikesafe-python-1.3.0/.vscode/
--rw-rw-rw-   0        0        0        4 2020-07-03 00:26:15.000000 spikesafe-python-1.3.0/.vscode/settings.json
--rw-rw-rw-   0        0        0     1085 2022-09-12 18:51:49.000000 spikesafe-python-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     4227 2023-01-10 22:24:55.341223 spikesafe-python-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3843 2022-09-12 18:51:49.000000 spikesafe-python-1.3.0/README.md
--rw-rw-rw-   0        0        0      173 2020-05-05 18:24:01.000000 spikesafe-python-1.3.0/__init__.py
--rw-rw-rw-   0        0        0  2569500 2023-01-09 23:44:52.000000 spikesafe-python-1.3.0/get-pip.py
--rw-rw-rw-   0        0        0      460 2023-01-10 22:24:35.000000 spikesafe-python-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-10 22:24:55.345224 spikesafe-python-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-01-10 20:06:39.000000 spikesafe-python-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-10 22:24:55.325578 spikesafe-python-1.3.0/spikesafe_python/
--rw-rw-rw-   0        0        0     2768 2020-05-26 20:24:12.000000 spikesafe-python-1.3.0/spikesafe_python/ChannelData.py
--rw-rw-rw-   0        0        0      574 2022-09-02 18:40:50.000000 spikesafe-python-1.3.0/spikesafe_python/DigitizerData.py
--rw-rw-rw-   0        0        0     3865 2022-09-13 22:40:55.000000 spikesafe-python-1.3.0/spikesafe_python/DigitizerDataFetch.py
--rw-rw-rw-   0        0        0     6469 2020-05-26 20:24:12.000000 spikesafe-python-1.3.0/spikesafe_python/EventData.py
--rw-rw-rw-   0        0        0     8495 2022-09-13 22:05:52.000000 spikesafe-python-1.3.0/spikesafe_python/MemoryTableReadData.py
--rw-rw-rw-   0        0        0     7490 2022-09-13 22:41:11.000000 spikesafe-python-1.3.0/spikesafe_python/ReadAllEvents.py
--rw-rw-rw-   0        0        0     1069 2020-06-04 21:05:13.000000 spikesafe-python-1.3.0/spikesafe_python/SpikeSafeError.py
--rw-rw-rw-   0        0        0     4325 2022-09-12 19:11:23.000000 spikesafe-python-1.3.0/spikesafe_python/SpikeSafeEvents.py
--rw-rw-rw-   0        0        0     6905 2022-09-13 23:21:46.000000 spikesafe-python-1.3.0/spikesafe_python/TcpSocket.py
--rw-rw-rw-   0        0        0     2542 2022-09-02 18:40:58.000000 spikesafe-python-1.3.0/spikesafe_python/TemperatureData.py
--rw-rw-rw-   0        0        0      320 2022-09-06 18:50:24.000000 spikesafe-python-1.3.0/spikesafe_python/Threading.py
--rw-rw-rw-   0        0        0        0 2020-04-28 21:09:20.000000 spikesafe-python-1.3.0/spikesafe_python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-10 22:24:55.337223 spikesafe-python-1.3.0/spikesafe_python.egg-info/
--rw-rw-rw-   0        0        0     4227 2023-01-10 22:24:55.000000 spikesafe-python-1.3.0/spikesafe_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      662 2023-01-10 22:24:55.000000 spikesafe-python-1.3.0/spikesafe_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-10 22:24:55.000000 spikesafe-python-1.3.0/spikesafe_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-01-10 22:24:55.000000 spikesafe-python-1.3.0/spikesafe_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 21:52:41.588645 spikesafe-python-1.4.5/
+-rw-rw-rw-   0        0        0     1928 2020-04-27 17:14:40.000000 spikesafe-python-1.4.5/.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-25 21:52:41.486699 spikesafe-python-1.4.5/.vscode/
+-rw-rw-rw-   0        0        0        4 2020-07-03 00:26:15.000000 spikesafe-python-1.4.5/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1085 2022-09-12 18:51:49.000000 spikesafe-python-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0     4228 2023-04-25 21:52:41.584616 spikesafe-python-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3844 2023-04-25 16:46:48.000000 spikesafe-python-1.4.5/README.md
+-rw-rw-rw-   0        0        0      173 2023-04-25 21:51:23.000000 spikesafe-python-1.4.5/__init__.py
+-rw-rw-rw-   0        0        0  2569500 2023-01-09 23:44:52.000000 spikesafe-python-1.4.5/get-pip.py
+-rw-rw-rw-   0        0        0      460 2023-04-25 21:51:33.000000 spikesafe-python-1.4.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 21:52:41.589645 spikesafe-python-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-01-10 20:06:39.000000 spikesafe-python-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:52:41.559484 spikesafe-python-1.4.5/spikesafe_python/
+-rw-rw-rw-   0        0        0     2768 2020-05-26 20:24:12.000000 spikesafe-python-1.4.5/spikesafe_python/ChannelData.py
+-rw-rw-rw-   0        0        0      574 2022-09-02 18:40:50.000000 spikesafe-python-1.4.5/spikesafe_python/DigitizerData.py
+-rw-rw-rw-   0        0        0     3867 2023-04-25 16:46:56.000000 spikesafe-python-1.4.5/spikesafe_python/DigitizerDataFetch.py
+-rw-rw-rw-   0        0        0     6469 2020-05-26 20:24:12.000000 spikesafe-python-1.4.5/spikesafe_python/EventData.py
+-rw-rw-rw-   0        0        0     8495 2022-09-13 22:05:52.000000 spikesafe-python-1.4.5/spikesafe_python/MemoryTableReadData.py
+-rw-rw-rw-   0        0        0     7490 2022-09-13 22:41:11.000000 spikesafe-python-1.4.5/spikesafe_python/ReadAllEvents.py
+-rw-rw-rw-   0        0        0     1069 2020-06-04 21:05:13.000000 spikesafe-python-1.4.5/spikesafe_python/SpikeSafeError.py
+-rw-rw-rw-   0        0        0     4325 2022-09-12 19:11:23.000000 spikesafe-python-1.4.5/spikesafe_python/SpikeSafeEvents.py
+-rw-rw-rw-   0        0        0     6905 2022-09-13 23:21:46.000000 spikesafe-python-1.4.5/spikesafe_python/TcpSocket.py
+-rw-rw-rw-   0        0        0     2542 2022-09-02 18:40:58.000000 spikesafe-python-1.4.5/spikesafe_python/TemperatureData.py
+-rw-rw-rw-   0        0        0      510 2023-04-25 17:05:29.000000 spikesafe-python-1.4.5/spikesafe_python/Threading.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 21:51:17.000000 spikesafe-python-1.4.5/spikesafe_python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 21:52:41.580615 spikesafe-python-1.4.5/spikesafe_python.egg-info/
+-rw-rw-rw-   0        0        0     4228 2023-04-25 21:52:41.000000 spikesafe-python-1.4.5/spikesafe_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2023-04-25 21:52:41.000000 spikesafe-python-1.4.5/spikesafe_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 21:52:41.000000 spikesafe-python-1.4.5/spikesafe_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-25 21:52:41.000000 spikesafe-python-1.4.5/spikesafe_python.egg-info/top_level.txt
```

### Comparing `spikesafe-python-1.3.0/.gitignore` & `spikesafe-python-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/LICENSE` & `spikesafe-python-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/PKG-INFO` & `spikesafe-python-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spikesafe-python
-Version: 1.3.0
+Version: 1.4.5
 Summary: SpikeSafe Python Library
 Author-email: Vektrex <support@vektrex.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spikesafe-python
 
 The official Python driver supporting Vektrex SpikeSafe products:
-- [SpikeSafe SMU](https://www.vektrex.com/products/spikesafe-source-measure-unit/)
+- [SpikeSafe PSMU](https://www.vektrex.com/products/spikesafe-source-measure-unit/)
 - [SpikeSafe Performance Series ("PRF")](https://www.vektrex.com/products/spikesafe-performance-series-precision-pulsed-current-sources/)
 
 Vektrex SpikeSafe Python API used for automation of custom instrument control sequences for testing LED, laser, and electronic equipment.
 
 The Vektrex SpikeSafe Python API powers the Python examples published on Github.
 
 GitHub Repository: [SpikeSafe Python Samples](https://github.com/VektrexElectronicSystems/SpikeSafePythonSamples)
```

### Comparing `spikesafe-python-1.3.0/README.md` & `spikesafe-python-1.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # spikesafe-python
 
 The official Python driver supporting Vektrex SpikeSafe products:
-- [SpikeSafe SMU](https://www.vektrex.com/products/spikesafe-source-measure-unit/)
+- [SpikeSafe PSMU](https://www.vektrex.com/products/spikesafe-source-measure-unit/)
 - [SpikeSafe Performance Series ("PRF")](https://www.vektrex.com/products/spikesafe-performance-series-precision-pulsed-current-sources/)
 
 Vektrex SpikeSafe Python API used for automation of custom instrument control sequences for testing LED, laser, and electronic equipment.
 
 The Vektrex SpikeSafe Python API powers the Python examples published on Github.
 
 GitHub Repository: [SpikeSafe Python Samples](https://github.com/VektrexElectronicSystems/SpikeSafePythonSamples)
```

### Comparing `spikesafe-python-1.3.0/get-pip.py` & `spikesafe-python-1.4.5/get-pip.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/ChannelData.py` & `spikesafe-python-1.4.5/spikesafe_python/ChannelData.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/DigitizerData.py` & `spikesafe-python-1.4.5/spikesafe_python/DigitizerData.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/DigitizerDataFetch.py` & `spikesafe-python-1.4.5/spikesafe_python/DigitizerDataFetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Goal: Read all new voltage readings from SpikeSafe SMU Digitizer
+# Goal: Read all new voltage readings from SpikeSafe PSMU Digitizer
 # SCPI Command: VOLT:FETC?
 # Array of voltage readings are parsed into DigitizerData class
 # Example data return: b'9.9712145e-01,1.0005457e+00,3.2105038e+01\n'
 
 import sys
 import logging
 from .DigitizerData import DigitizerData
@@ -54,15 +54,15 @@
 
     except Exception as err:
         # print any error to the log file and raise error to function caller
         log.error("Error fetching digitizer voltage data: {}".format(err))                                     
         raise
 
 def wait_for_new_voltage_data(spike_safe_socket, wait_time = 0.0, enable_logging = None):
-    """Queries the SpikeSafe SMU digitizer until it responds that it has acquired new data
+    """Queries the SpikeSafe PSMU digitizer until it responds that it has acquired new data
 
     This is a useful function to call prior to sending a fetch query, because it determines whether fetched data will be freshly acquired
 
     Parameters
     ----------
     spike_safe_socket : TcpSocket
         Socket object used to communicate with SpikeSafe
```

### Comparing `spikesafe-python-1.3.0/spikesafe_python/EventData.py` & `spikesafe-python-1.4.5/spikesafe_python/EventData.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/MemoryTableReadData.py` & `spikesafe-python-1.4.5/spikesafe_python/MemoryTableReadData.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/ReadAllEvents.py` & `spikesafe-python-1.4.5/spikesafe_python/ReadAllEvents.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/SpikeSafeError.py` & `spikesafe-python-1.4.5/spikesafe_python/SpikeSafeError.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/SpikeSafeEvents.py` & `spikesafe-python-1.4.5/spikesafe_python/SpikeSafeEvents.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/TcpSocket.py` & `spikesafe-python-1.4.5/spikesafe_python/TcpSocket.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python/TemperatureData.py` & `spikesafe-python-1.4.5/spikesafe_python/TemperatureData.py`

 * *Files identical despite different names*

### Comparing `spikesafe-python-1.3.0/spikesafe_python.egg-info/PKG-INFO` & `spikesafe-python-1.4.5/spikesafe_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: spikesafe-python
-Version: 1.3.0
+Version: 1.4.5
 Summary: SpikeSafe Python Library
 Author-email: Vektrex <support@vektrex.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # spikesafe-python
 
 The official Python driver supporting Vektrex SpikeSafe products:
-- [SpikeSafe SMU](https://www.vektrex.com/products/spikesafe-source-measure-unit/)
+- [SpikeSafe PSMU](https://www.vektrex.com/products/spikesafe-source-measure-unit/)
 - [SpikeSafe Performance Series ("PRF")](https://www.vektrex.com/products/spikesafe-performance-series-precision-pulsed-current-sources/)
 
 Vektrex SpikeSafe Python API used for automation of custom instrument control sequences for testing LED, laser, and electronic equipment.
 
 The Vektrex SpikeSafe Python API powers the Python examples published on Github.
 
 GitHub Repository: [SpikeSafe Python Samples](https://github.com/VektrexElectronicSystems/SpikeSafePythonSamples)
```

### Comparing `spikesafe-python-1.3.0/spikesafe_python.egg-info/SOURCES.txt` & `spikesafe-python-1.4.5/spikesafe_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

