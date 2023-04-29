# Comparing `tmp/shareddata-1.4.0.tar.gz` & `tmp/shareddata-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-1.4.0.tar", last modified: Thu Feb 23 20:23:31 2023, max compression
+gzip compressed data, was "shareddata-2.0.0.tar", last modified: Sat Apr 29 13:15:40 2023, max compression
```

## Comparing `shareddata-1.4.0.tar` & `shareddata-2.0.0.tar`

### file list

```diff
@@ -1,49 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 20:23:31.893168 shareddata-1.4.0/
--rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     1218 2023-02-23 20:23:31.894167 shareddata-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      648 2023-02-15 20:29:49.000000 shareddata-1.4.0/README.md
--rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-1.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      906 2023-02-23 20:23:31.895167 shareddata-1.4.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-23 20:23:31.855381 shareddata-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-23 20:23:31.869168 shareddata-1.4.0/src/SharedData/
--rw-rw-rw-   0        0        0     1314 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/Defaults.py
--rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-1.4.0/src/SharedData/Logger.py
--rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-1.4.0/src/SharedData/LoggerConsumerProcess.py
--rw-rw-rw-   0        0        0     9470 2023-02-15 10:43:33.000000 shareddata-1.4.0/src/SharedData/Metadata.py
--rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/MultiProc.py
--rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/SeriesLib.py
--rw-rw-rw-   0        0        0     3093 2023-02-16 12:52:42.000000 shareddata-1.4.0/src/SharedData/SharedData.py
--rw-rw-rw-   0        0        0    14581 2023-02-19 13:42:22.000000 shareddata-1.4.0/src/SharedData/SharedDataAWSKinesis.py
--rw-rw-rw-   0        0        0    11175 2023-02-15 18:03:06.000000 shareddata-1.4.0/src/SharedData/SharedDataAWSS3.py
--rw-rw-rw-   0        0        0     5514 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/SharedDataFeeder.py
--rw-rw-rw-   0        0        0    18414 2023-02-15 10:43:33.000000 shareddata-1.4.0/src/SharedData/SharedDataFrame.py
--rw-rw-rw-   0        0        0     5675 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/SharedDataPeriod.py
--rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/SharedDataRealTime.py
--rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/SharedDataRealTimeProcess.py
--rw-rw-rw-   0        0        0    11673 2023-02-18 11:23:56.000000 shareddata-1.4.0/src/SharedData/SharedDataSparse.py
--rw-rw-rw-   0        0        0    26773 2023-02-15 10:43:33.000000 shareddata-1.4.0/src/SharedData/SharedDataTimeSeries.py
--rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-1.4.0/src/SharedData/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 20:23:31.883167 shareddata-1.4.0/src/shareddata.egg-info/
--rw-rw-rw-   0        0        0     1218 2023-02-23 20:23:31.000000 shareddata-1.4.0/src/shareddata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1293 2023-02-23 20:23:31.000000 shareddata-1.4.0/src/shareddata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 20:23:31.000000 shareddata-1.4.0/src/shareddata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-02-23 20:23:31.000000 shareddata-1.4.0/src/shareddata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-02-23 20:23:31.000000 shareddata-1.4.0/src/shareddata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-23 20:23:31.893168 shareddata-1.4.0/tests/
--rw-rw-rw-   0        0        0      466 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test01_logging.py
--rw-rw-rw-   0        0        0      546 2023-02-15 21:44:47.000000 shareddata-1.4.0/tests/test01_logging_cons.py
--rw-rw-rw-   0        0        0     1640 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test02_checkdata.py
--rw-rw-rw-   0        0        0     1020 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test02_dataset_reading.py
--rw-rw-rw-   0        0        0      526 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test02_history_reading.py
--rw-rw-rw-   0        0        0     1181 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test03_dataset_read_write.py
--rw-rw-rw-   0        0        0     1028 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test03_history_writing.py
--rw-rw-rw-   0        0        0     2529 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test04_a_realtime_consumer.py
--rw-rw-rw-   0        0        0      469 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test04_b_realtime_consumer.py
--rw-rw-rw-   0        0        0      627 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test09_realtime_producer.py
--rw-rw-rw-   0        0        0      959 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test10_shareddataframe_writing.py
--rw-rw-rw-   0        0        0     4419 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test_boto3.py
--rw-rw-rw-   0        0        0     1290 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test_combinedfile copy.py
--rw-rw-rw-   0        0        0     4905 2023-01-14 18:28:34.000000 shareddata-1.4.0/tests/test_combinedfile.py
--rw-rw-rw-   0        0        0     1928 2023-02-20 03:15:25.000000 shareddata-1.4.0/tests/test_sparse.py
--rw-rw-rw-   0        0        0      450 2023-01-12 20:44:38.000000 shareddata-1.4.0/tests/test_watchdog1.py
--rw-rw-rw-   0        0        0     1283 2023-02-19 13:43:11.000000 shareddata-1.4.0/tests/testlinux.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.565590 shareddata-2.0.0/
+-rw-rw-rw-   0        0        0    35823 2023-01-12 20:44:38.000000 shareddata-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1218 2023-04-29 13:15:40.565590 shareddata-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      648 2023-02-15 20:29:49.000000 shareddata-2.0.0/README.md
+-rw-rw-rw-   0        0        0      108 2023-01-12 20:44:38.000000 shareddata-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      906 2023-04-29 13:15:40.566592 shareddata-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.542592 shareddata-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.554592 shareddata-2.0.0/src/SharedData/
+-rw-rw-rw-   0        0        0     1562 2023-04-11 20:53:38.000000 shareddata-2.0.0/src/SharedData/Defaults.py
+-rw-rw-rw-   0        0        0     4735 2023-01-16 18:59:43.000000 shareddata-2.0.0/src/SharedData/Logger.py
+-rw-rw-rw-   0        0        0     1275 2023-02-17 15:06:53.000000 shareddata-2.0.0/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-rw-   0        0        0    11426 2023-04-14 14:51:54.000000 shareddata-2.0.0/src/SharedData/Metadata.py
+-rw-rw-rw-   0        0        0     3862 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/MultiProc.py
+-rw-rw-rw-   0        0        0     5182 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/SeriesLib.py
+-rw-rw-rw-   0        0        0     3085 2023-03-02 10:46:06.000000 shareddata-2.0.0/src/SharedData/SharedData.py
+-rw-rw-rw-   0        0        0    14573 2023-02-27 22:09:20.000000 shareddata-2.0.0/src/SharedData/SharedDataAWSKinesis.py
+-rw-rw-rw-   0        0        0    11230 2023-03-26 19:43:51.000000 shareddata-2.0.0/src/SharedData/SharedDataAWSS3.py
+-rw-rw-rw-   0        0        0     6283 2023-04-25 18:26:16.000000 shareddata-2.0.0/src/SharedData/SharedDataFeeder.py
+-rw-rw-rw-   0        0        0    11229 2023-03-09 15:11:52.000000 shareddata-2.0.0/src/SharedData/SharedDataFrame.py
+-rw-rw-rw-   0        0        0     5818 2023-03-17 12:56:52.000000 shareddata-2.0.0/src/SharedData/SharedDataPeriod.py
+-rw-rw-rw-   0        0        0     3672 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/SharedDataRealTime.py
+-rw-rw-rw-   0        0        0     2545 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/SharedDataRealTimeProcess.py
+-rw-rw-rw-   0        0        0    46626 2023-04-28 21:14:34.000000 shareddata-2.0.0/src/SharedData/SharedDataTable.py
+-rw-rw-rw-   0        0        0    18042 2023-03-20 11:50:36.000000 shareddata-2.0.0/src/SharedData/SharedDataTimeSeries.py
+-rw-rw-rw-   0        0        0        0 2023-01-12 20:44:38.000000 shareddata-2.0.0/src/SharedData/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-29 13:15:40.564590 shareddata-2.0.0/src/shareddata.egg-info/
+-rw-rw-rw-   0        0        0     1218 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      793 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      158 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-29 13:15:40.000000 shareddata-2.0.0/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-1.4.0/LICENSE` & `shareddata-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/PKG-INFO` & `shareddata-2.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 1.4.0
+Version: 2.0.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-1.4.0/README.md` & `shareddata-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/Defaults.py` & `shareddata-2.0.0/src/SharedData/Defaults.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 #print('loading environment variables...')
 
 load_dotenv()  # take environment variables from .env.
 
 if not 'AWS_PROFILE' in os.environ:
     raise Exception('Missing AWS_PROFILE environment variable!')
 
+if not 'PYTHONHASHSEED' in os.environ:
+    raise Exception('PYTHONHASHSEED must be set to 0 in the environment!')
+else:
+    if os.environ['PYTHONHASHSEED']!='0':
+        raise Exception('PYTHONHASHSEED must be set to 0 in the environment!')
+
 if not 'DATABASE_FOLDER' in os.environ:    
     os.environ['DATABASE_FOLDER'] = os.path.expanduser("~")+'\DB' 
 
 if not 'S3_BUCKET' in os.environ:    
     os.environ['S3_BUCKET'] = 's3://deepportfolio'
 
 if not 'S3_AWS_PROFILE' in os.environ:
```

### Comparing `shareddata-1.4.0/src/SharedData/Logger.py` & `shareddata-2.0.0/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.0.0/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/MultiProc.py` & `shareddata-2.0.0/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/SeriesLib.py` & `shareddata-2.0.0/src/SharedData/SeriesLib.py`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/SharedData.py` & `shareddata-2.0.0/src/SharedData/SharedData.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 user=self.user)
             self.mergeUpdate(self.metadata[collection].static)            
         return self.metadata[collection]
 
     def getSymbols(self, collection):        
         return self.getMetadata(collection).static.index.values
 
-    def mergeUpdate(self,newdf):        
+    def mergeUpdate(self,newdf):
         newidx = ~newdf.index.isin(self.static.index)
         if newidx.any():
             self.static = self.static.reindex(index=self.static.index.union(newdf.index))
 
         newcolsidx = ~newdf.columns.isin(self.static.columns)
         if newcolsidx.any():
             newcols = newdf.columns[newcolsidx]
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataAWSKinesis.py` & `shareddata-2.0.0/src/SharedData/SharedDataAWSKinesis.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 )
             time.sleep(10)
         except ClientError as e:
             if e.response['Error']['Code'] == 'ResourceInUseException':                                
                 print("Stream already exists")                
             else:
                 print("Trying to create stream unexpected error: %s" % e)
-                return False        
+                pass        
 
         try:            
             self.stream = self.client.describe_stream(StreamName=os.environ['LOG_STREAMNAME'])            
         except:
             print('Could not describe stream!')
             return False
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataAWSS3.py` & `shareddata-2.0.0/src/SharedData/SharedDataAWSS3.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,15 @@
     return [None, local_mtime, remote_mtime]
 
 def UpdateModTime(local_path, remote_mtime):    
     # update modification time
     remote_mtime_dt = datetime.fromtimestamp(remote_mtime)
     offset =  remote_mtime_dt - datetime.utcfromtimestamp(remote_mtime)        
     remote_mtime_local_tz = remote_mtime_dt+offset
-    remote_mtime_local_tz_ts = remote_mtime_local_tz.timestamp()                
+    remote_mtime_local_tz_ts = remote_mtime_local_tz.timestamp()
     os.utime(local_path, (remote_mtime_local_tz_ts, remote_mtime_local_tz_ts))
 
 def S3SaveLocal(local_path, io_obj, remote_mtime):
     path = Path(local_path)
     if not path.parent.exists():
         path.parent.mkdir(parents=True, exist_ok=True)
     with open(local_path,'wb') as f:
@@ -243,15 +243,16 @@
 
 def S3Upload(file_io, path, mtime):
     remotefilepath = str(path).replace(\
             os.environ['DATABASE_FOLDER'],os.environ['S3_BUCKET'])
     remotefilepath = remotefilepath.replace('\\','/')        
           
     trials = 3
-    success=False
+    success=False    
+    file_io.close = lambda: None # prevents boto3 from closing io
     while trials>0:        
         try:                
             s3,bucket = S3GetSession(isupload=True)            
             mtime_utc = datetime.utcfromtimestamp(mtime).timestamp()
             mtime_str = str(mtime_utc)
             file_io.seek(0)
             bucket.upload_fileobj(file_io,remotefilepath.replace(os.environ['S3_BUCKET'],'')[1:],\
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataFeeder.py` & `shareddata-2.0.0/src/SharedData/SharedDataFeeder.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import numpy as np
 from concurrent.futures import ThreadPoolExecutor
 import time
 
 from SharedData.Metadata import Metadata
 from SharedData.Logger import Logger
 from SharedData.SharedDataPeriod import SharedDataPeriod
+from SharedData.SharedDataTable import SharedDataTable
 
 class SharedDataFeeder():
+
+    dense_datasets = {'W1':'weekly','D1':'daily','M15':'15 min','M1':'1 min'}
     
     def __init__(self, sharedData, feeder):
         self.feeder = feeder
         self.sharedData = sharedData    
         self.database = sharedData.database        
         self.default_collections = None
         
@@ -36,26 +39,36 @@
             uperiod = self.dataset['period'].unique()
             for period in uperiod:
                 self.data[period] = SharedDataPeriod(self, period)
                 ustartdate = self.dataset.set_index('period')['startDate'].unique()
                 for startdate in ustartdate:
                     self.data[period].getContinousTimeIndex(startdate)    
     
-    def __setitem__(self, period, value):
-        self.data[period] = value
+    def __setitem__(self, dataset, value):
+        if not dataset in self.data.keys():
+            if (dataset in SharedDataFeeder.dense_datasets.keys()):
+                period = dataset
+                self.data[period] = value
+            else:
+                self.data[dataset] = SharedDataTable(self, dataset, value)            
+        return self.data[dataset]
                 
-    def __getitem__(self, period):
-        if not period in self.data.keys():
-            if (period=='D1') | (period=='M15') | (period=='M1'):
-                self.data[period] = SharedDataPeriod(self, period)
+    def __getitem__(self, dataset):
+        if not dataset in self.data.keys():
+            if (dataset in SharedDataFeeder.dense_datasets.keys()):
+                period = dataset
+                self.data[period] = SharedDataPeriod(self, period)        
             else:
-                Logger.log.error('Period '+period+ ' not supported!')
-                raise ValueError('Period '+period+ ' not supported!')
-        return self.data[period]
+                self.data[dataset] = SharedDataTable(self, dataset)
 
+        if (dataset in SharedDataFeeder.dense_datasets.keys()):
+            return self.data[dataset]    
+        else:
+            return self.data[dataset].records        
+        
     def load(self, period='D1', tags=None):
             
         if not self.default_collections is None:
             for c in self.default_collections.replace('\n','').split(','):
                 self.sharedData.getMetadata(c)    
 
         for c in self.collections:
@@ -120,7 +133,12 @@
             ds.loc[tag,'memory_size'] = d1[tag].memory_usage(deep=True).sum()/1000000
             ds.loc[tag,'download_time'] = d1.tags[tag].download_time
             ds.loc[tag,'download_speed'] = np.nan
             if not pd.isnull(ds.loc[tag,'download_time']):
                 ds.loc[tag,'download_speed'] = ds.loc[tag,'data_size']*1000000/d1.tags[tag].download_time
         self.dataset_metadata.static = ds.reset_index()
         return ds.reset_index()
+
+    def create(self,dataset,names,formats,size):
+        self.data[dataset] = SharedDataTable(\
+            self,dataset,names=names,formats=formats,size=size)
+        return self.data[dataset].records
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataFrame.py` & `shareddata-2.0.0/src/SharedData/SharedDataFrame.py`

 * *Files 24% similar despite different names*

```diff
@@ -62,26 +62,16 @@
     def getDataPath(self,iswrite=False):        
         shm_name = self.sharedData.user
         shm_name = shm_name + '/' + self.sharedData.database
         shm_name = shm_name + '/' + self.sharedDataFeeder.feeder
         shm_name = shm_name + '/' + self.period + '/' + self.tagstr
         if os.name=='posix':
             shm_name = shm_name.replace('/','\\')
-
-        if not iswrite:
-            if 'LEGACY_READ' in os.environ:
-                path = Path(os.environ['LEGACY_DATABASE_FOLDER'])
-            else:
-                path = Path(os.environ['DATABASE_FOLDER'])
-        else:
-            if 'LEGACY_WRITE' in os.environ:
-                path = Path(os.environ['LEGACY_DATABASE_FOLDER'])
-            else:
-                path = Path(os.environ['DATABASE_FOLDER'])
-
+        
+        path = Path(os.environ['DATABASE_FOLDER'])
         path = path / self.sharedData.user
         path = path / self.sharedData.database
         path = path / self.sharedDataFeeder.feeder
         path = path / self.period
         path = Path(str(path).replace('\\','/'))
         if self.sharedData.save_local:
             if not os.path.isdir(path):
@@ -181,97 +171,18 @@
 
                 self.create_map = 'map'
                 return True
             except:
                 pass
     
         return False
-
-    def MallocLegacy(self, df=None):
-        tini=time.time()
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            Logger.log.debug('Malloc %s/%s/%s/%s ...%.2f%% ' % \
-                (self.database,self.feeder,self.period,self.tagstr,0.0))      
-
-        #Create write ndarray
-        path, shm_name = self.getDataPath()
-        jsonpath = path / (self.tagstr+'.json')
-        npypath = path / (self.tagstr+'.npy')
-
-        trymap = False
-        if not df is None:
-            rows = len(df.index)
-            cols = len(df.columns)
-            nbytes = int(rows*cols*8)
-
-            try:
-                self.shm = shared_memory.SharedMemory(\
-                    name = shm_name,create=True, size=nbytes)
-                self.shmarr = np.ndarray((rows,cols),\
-                    dtype=np.float64, buffer=self.shm.buf)            
-                self.shmarr[:] = df.values.copy()
-                self.data = pd.DataFrame(self.shmarr,\
-                    index=df.index,\
-                    columns=df.columns,\
-                    copy=False)                                
-
-                with open(str(jsonpath), 'w+') as outfile:
-                    shm_info = {
-                        'shm_name':shm_name,
-                        'index': self.data.index.values.tolist(),
-                        'columns': self.data.columns.values.tolist()                                 
-                        }
-                    json.dump(shm_info, outfile, indent=3)
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    Logger.log.debug('Malloc create %s/%s/%s/%s ...%.2f%% %.2f sec! ' % \
-                        (self.database,self.feeder,self.period,self.tagstr,100,time.time()-tini))
-                self.create_map = 'create'
-                return True
-            except:
-                trymap=True
-
-        if (jsonpath.is_file()) & ((df is None) | (trymap)):
-            with open(str(jsonpath), 'r') as infile:
-                try:
-                    shm_info = json.load(infile)
-                    _index = pd.Index(shm_info['index'])
-                    _columns = pd.Index(shm_info['columns'])
-                    _shm_name = shm_info['shm_name']
-                    rows = len(_index)
-                    cols = len(_columns)
-                    # map memory file
-                    self.shm = shared_memory.SharedMemory(\
-                        name=_shm_name, create=False)
-                    self.shmarr = np.ndarray((rows,cols),\
-                        dtype=np.float64, buffer=self.shm.buf)
-                    self.data = pd.DataFrame(self.shmarr,\
-                                index=_index,\
-                                columns=_columns,\
-                                copy=False)
-
-                    if not df is None:
-                        iidx = df.index.intersection(self.data.index)
-                        icol = df.columns.intersection(self.data.columns)
-                        self.data.loc[iidx, icol] = df.loc[iidx, icol].copy()
-                    if os.environ['LOG_LEVEL']=='DEBUG':
-                        Logger.log.debug('Malloc map %s/%s/%s/%s ...%.2f%% %.2f sec! ' % \
-                            (self.database,self.feeder,self.period,self.tagstr,100,time.time()-tini))       
-                    self.create_map = 'map'
-                    return True
-                except:
-                    return False
-        else:
-            return False
-      
+   
     # READ
     def Read(self):
-        if 'LEGACY_READ' in os.environ:
-            return self.LegacyRead()
-        else:
-            return self.ReadDataFrame()
+        return self.ReadDataFrame()
 
     def ReadDataFrame(self):
         tini = time.time()
         path, shm_name = self.getDataPath()
         local_path = str(path/(self.tagstr+'.bin'))
         remote_path = local_path+'.gzip'
         df_io = None
@@ -317,59 +228,16 @@
         __md5hash_b = df_io.read(16)
         if not _md5hash_b==__md5hash_b:
             raise Exception('DataFrame file corrupted!\n%s' % (local_path))
         df = pd.DataFrame(_data,index=_idx,columns=_cols)
         df_io.close()
         return df
 
-    def LegacyRead(self):
-        tini = time.time()
-        path, shm_name = self.getDataPath()
-        if self.sharedData.s3read:
-            #Synchronize S3
-            LegacyS3SyncDownloadDataFrame(path, shm_name)
-                            
-        jsonpath = path / (self.tagstr+'.json')
-        npypath = path / (self.tagstr+'.npy')
-            
-        if (jsonpath.is_file()) & (npypath.is_file()):
-            if os.environ['LOG_LEVEL']=='DEBUG':
-                Logger.log.debug('Reading %s/%s/%s ...%.2f%% ' % \
-                    (self.feeder,self.period,self.tagstr,0.0))  
-            with open(str(jsonpath), 'r') as infile:
-                try:
-                    shm_info = json.load(infile)
-                    _index = pd.Index(shm_info['index'])
-                    _columns = pd.Index(shm_info['columns'])
-                    _shm_name = shm_info['shm_name']
-                    rows = len(_index)
-                    cols = len(_columns)
-                    values = np.load(str(npypath),mmap_mode='r')
-
-                    df = pd.DataFrame(values,\
-                        index=_index,\
-                        columns=_columns)
-                    if os.environ['LOG_LEVEL']=='DEBUG':
-                        Logger.log.debug('Reading %s/%s/%s/%s ...%.2f%% %.2f sec! ' % \
-                            (self.database,self.feeder,self.period,self.tagstr,100,time.time()-tini))
-                    return df
-                except:
-                    pass
-                    Logger.log.error('File corrupted %s/%s/%s/%s ...%.2f%% %.2f sec! ' % \
-                        (self.database,self.feeder,self.period,self.tagstr,100,time.time()-tini))                
-        return pd.DataFrame([])
-
     # WRITE
-    def Write(self,startDate=None):
-        if 'LEGACY_WRITE' in os.environ:
-            self.LegacyWrite()
-        else:
-            self.write_dataframe()
-
-    def write_dataframe(self):        
+    def Write(self):     
         path, shm_name = self.getDataPath(iswrite=True)
         local_path = str(path/(self.tagstr+'.bin'))
         remote_path = local_path+'.gzip'
         df_io = SharedDataFrame.create_dataframe_io(self.data)
         mtime = datetime.now().timestamp()
         threads=[]
         if self.sharedData.s3write:
@@ -415,45 +283,15 @@
         return io_obj
 
     def write_file(io_obj,path,mtime):
         with open(path, 'wb') as f:
             f.write(io_obj.getbuffer())
             f.flush()
         os.utime(path, (mtime, mtime))
-
-    def LegacyWrite(self):
-        tini = time.time()
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            Logger.log.debug('Writing %s/%s/%s/%s  ...%.2f%% ' % \
-                (self.database,self.feeder,self.period,self.tagstr,0.0))        
-
-        path, shm_name = self.getDataPath(iswrite=True)
-        jsonpath = path / (self.tagstr+'.json')
-        npypath = path / (self.tagstr+'.npy')
-        with open(str(jsonpath), 'w+') as outfile:
-            shm_info = {
-                'shm_name':shm_name,
-                'index': self.data.index.values.tolist(),
-                'columns': self.data.columns.values.tolist()                                 
-                }
-            json.dump(shm_info, outfile, indent=3)
-            outfile.flush()
-
-        with open(str(npypath), 'wb') as f:
-            np.save(f,self.data.values.astype(np.float64))
-            f.flush()
-
-        if self.sharedData.s3write:            
-            Legacy_S3Upload(npypath)
-            Legacy_S3Upload(jsonpath)
-            
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            Logger.log.debug('Writing %s/%s/%s/%s ...%.2f%% %.2f sec!' % \
-                (self.database,self.feeder,self.period,self.tagstr,100,time.time()-tini))
-        
+     
     # MESSAGES
     def Broadcast(self,idx,col):
         SharedDataRealTime.Broadcast(
             self.sharedData,
             self.feeder,
             self.period,
             self.tag,
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataPeriod.py` & `shareddata-2.0.0/src/SharedData/SharedDataPeriod.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         # DATA DICTIONARY
         # tags[tag]
         self.tags = {}
 
         # TIME INDEX
         self.timeidx = {}
         self.ctimeidx = {}        
-        if self.period=='D1':
+        if self.period=='W1':
+            self.periodSeconds = 7*60*60*24
+            self.default_startDate = pd.Timestamp('1990-01-01')
+        elif self.period=='D1':
             self.periodSeconds = 60*60*24       
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M15':
             self.periodSeconds = 60*15
             self.default_startDate = pd.Timestamp('1990-01-01')
         elif self.period=='M1':
             self.periodSeconds = 60
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataRealTime.py` & `shareddata-2.0.0/src/SharedData/SharedDataRealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataRealTimeProcess.py` & `shareddata-2.0.0/src/SharedData/SharedDataRealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataSparse.py` & `shareddata-2.0.0/src/SharedData/Metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,312 +1,307 @@
-# THIRD PARTY LIBS
-import os,sys
+import os
+from dotenv import load_dotenv
+from pathlib import Path
 import pandas as pd
 import numpy as np
-import json
 import time
-import io,gzip, hashlib, shutil
-from threading import Thread
-
-from pandas.tseries.offsets import BDay
-from pathlib import Path
-from multiprocessing import shared_memory
+import subprocess
 from datetime import datetime, timedelta
+import gzip,io,shutil,hashlib
 
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSS3 import S3Download,S3Upload,UpdateModTime
-from SharedData.SharedDataRealTime import SharedDataRealTime
-
-class SharedDataSparse:
-
-    def __init__(self, sharedDataFeeder, tag, df=None):
-        self.sharedDataFeeder = sharedDataFeeder
-        self.tag = tag
-        self.tagstr = self.tag.strftime('%Y%m%d%H%M')
-                
-        self.feeder = sharedDataFeeder.feeder
-        self.sharedData = sharedDataFeeder.sharedData
-        self.database = self.sharedData.database
-
-        self.period = sharedDataFeeder.period
-        self.periodSeconds = sharedDataFeeder.periodSeconds  
-        
-        self.init_time = time.time()
-        
-        # Time series dataframe
-        self.data = pd.DataFrame()
-
-        self.create_map = 'na'
-        if df is None: #Read dataset tag
-            #allocate memory
-            ismapped = self.Malloc()
-            if not ismapped:
-                # Read
-                df = self.Read()
-                if not df.empty:
-                    self.Malloc(df)
-            
-        else: # map existing dataframe   
-            #drop non number fields   
-            df = df._get_numeric_data().astype(np.float64)
-            #allocate memory
-            self.Malloc(df)
-        
-        self.init_time = time.time() - self.init_time
-
-    #GETTERS AND SETTERS
-    def getDataPath(self,iswrite=False):        
-        shm_name = self.sharedData.user
-        shm_name = shm_name + '/' + self.sharedData.database
-        shm_name = shm_name + '/' + self.sharedDataFeeder.feeder
-        shm_name = shm_name + '/' + self.period + '/' + self.tagstr
-        if os.name=='posix':
-            shm_name = shm_name.replace('/','\\')
-
-        if not iswrite:
-            if 'LEGACY_READ' in os.environ:
-                path = Path(os.environ['LEGACY_DATABASE_FOLDER'])
-            else:
-                path = Path(os.environ['DATABASE_FOLDER'])
-        else:
-            if 'LEGACY_WRITE' in os.environ:
-                path = Path(os.environ['LEGACY_DATABASE_FOLDER'])
-            else:
-                path = Path(os.environ['DATABASE_FOLDER'])
-
-        path = path / self.sharedData.user
-        path = path / self.sharedData.database
-        path = path / self.sharedDataFeeder.feeder
-        path = path / self.period
-        path = Path(str(path).replace('\\','/'))
-        if self.sharedData.save_local:
-            if not os.path.isdir(path):
-                os.makedirs(path)
-
-        return path, shm_name
-
-    # C R U D
-    def Malloc(self, df=None):
-        tini=time.time()
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            Logger.log.debug('Malloc %s/%s/%s/%s ...%.2f%% ' % \
-                (self.database,self.feeder,self.period,self.tagstr,0.0))      
-
-        #Create write ndarray
-        path, shm_name = self.getDataPath()
-        if not df is None:
-            # try create memory file
-            try: 
-                r = len(df.index)
-                c = len(df.columns)
-                            
-                idx_b = str.encode(','.join(df.index.values),\
-                    encoding='UTF-8',errors='ignore')
-                colscsv_b = str.encode(','.join(df.columns.values),\
-                    encoding='UTF-8',errors='ignore')
-                nb_idx = len(idx_b)
-                nb_cols = len(colscsv_b)
-                nb_data = int(r*c*8)
-                header_b = np.array([r,c,nb_idx,nb_cols,nb_data]).astype(np.int64).tobytes()
-                nb_header = len(header_b)
-                
-                nb_buf = nb_header+nb_idx+nb_cols+nb_data
-                nb_offset = nb_header+nb_idx+nb_cols
+from SharedData.SharedDataAWSS3 import S3Upload, S3ListFolder, S3Download, UpdateModTime
 
-                self.shm = shared_memory.SharedMemory(\
-                    name = shm_name,create=True, size=nb_buf)
+class Metadata():
+    
+    def __init__(self, name, mode='rw', user='master'):
+        
+        if Logger.log is None:
+            Logger('Metadata')
+        
+        self.user = user
+        
+        self.s3read = False
+        self.s3write = False
+        if mode == 'r':
+            self.s3read = True
+            self.s3write = False
+        elif mode == 'w':
+            self.s3read = False
+            self.s3write = True
+        elif mode == 'rw':
+            self.s3read = True
+            self.s3write = True    
+
+        self.mode = mode
+        self.save_local = True
+        if os.environ['SAVE_LOCAL']!='True':
+            self.save_local = False
+
+        self.name = name
+
+        self._records = np.array([])
+        self.records_chg = False
+
+        self._index_columns = np.array([])
+        self._static = pd.DataFrame([])
+        self.static_chg = False
+
+        self.load()
+
+    @property
+    def static(self):
+        if self.records_chg:
+            self.records_chg = False
+            self._static = self.records2df(self._records)
+        return self._static
+    
+    @static.setter
+    def static(self, df):
+        self.static_chg = True
+        self.records_chg = False
+        self._index_columns = np.array(df.index.names)
+        self._static = df
+        
+        
+    @property
+    def records(self):
+        if self.static_chg:
+            self.static_chg = False
+            self._records = self.df2records(self._static)
+        return self._records
+    
+    @records.setter
+    def records(self, value):
+        self.records_chg = True
+        self._records = value
+
+    def hasindex(self):
+        if self._index_columns.size > 0:
+            if not self._index_columns[0] is None:
+                if self._index_columns[0]!='':
+                    return True
+        return False
 
-                i=0
-                self.shm.buf[i:nb_header] = header_b
-                i = i + nb_header
-                self.shm.buf[i:i+nb_idx] = idx_b
-                i = i + nb_idx
-                self.shm.buf[i:i+nb_cols] = colscsv_b
-
-                self.shmarr = np.ndarray((r,c),\
-                    dtype=np.float64, buffer=self.shm.buf, offset=nb_offset)
-
-                self.shmarr[:] = df.values.copy()
-
-                self.data = pd.DataFrame(self.shmarr,\
-                            index=df.index,\
-                            columns=df.columns,\
-                            copy=False)                
-
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    Logger.log.debug('Malloc create %s ...%.2f%% %.2f sec! ' % \
-                        (shm_name,100,time.time()-tini))            
-                self.create_map = 'create'
-                return True
-            except Exception as e:
-                return False
-        else: # df is None
-            # try map dataframe
+    def records2df(self,records):
+        df = pd.DataFrame(records, copy=False)
+        dtypes = df.dtypes.reset_index()
+        dtypes.columns = ['tag','dtype']
+        # convert object to string
+        string_idx = ['|S' in str(dt) for dt in dtypes['dtype']]
+        string_idx = (string_idx) | (dtypes['dtype']=='object')
+        tags_obj =  dtypes['tag'][string_idx].values
+        for tag in tags_obj:
             try:
-                self.shm = shared_memory.SharedMemory(\
-                    name = shm_name,create=False)
-                i=0
-                nb_header=40
-                header = np.frombuffer(self.shm.buf[i:nb_header],dtype=np.int64)
-                i = i + nb_header
-                nb_idx = header[2]
-                idx_b = bytes(self.shm.buf[i:i+nb_idx])
-                index = idx_b.decode(encoding='UTF-8',errors='ignore').split(',')
-                i = i + nb_idx
-                nb_cols = header[3]
-                cols_b = bytes(self.shm.buf[i:i+nb_cols])
-                columns = cols_b.decode(encoding='UTF-8',errors='ignore').split(',')
-
-                r = header[0]
-                c = header[1]        
-                nb_data = header[4]
-                nb_offset = nb_header+nb_idx+nb_cols                
-                
-                self.shmarr = np.ndarray((r,c), dtype=np.float64,\
-                    buffer=self.shm.buf, offset=nb_offset)
-
-                self.data = pd.DataFrame(self.shmarr,\
-                            index=index,\
-                            columns=columns,\
-                            copy=False)
-
-                if not df is None:
-                    iidx = df.index.intersection(self.data.index)
-                    icol = df.columns.intersection(self.data.columns)
-                    self.data.loc[iidx, icol] = df.loc[iidx, icol]
+                df[tag] = df[tag].str.decode(encoding='utf-8',errors='ignore')
+            except:
+                pass
+        if self.hasindex():
+            df = df.set_index(self._index_columns.tolist())
+        return df
 
-                self.create_map = 'map'
-                return True
+    def df2records(self,df):
+        self._index_columns = np.array(df.index.names)
+        if self.hasindex():
+            df = df.reset_index().copy()
+        else:
+            df = df.copy()
+        dtypes = df.dtypes.reset_index()
+        dtypes.columns = ['tag','dtype']
+        # convert object to string
+        tags_obj =  dtypes['tag'][dtypes['dtype']=='object'].values
+        for tag in tags_obj:
+            try:
+                df[tag] = df[tag].str.encode(encoding='utf-8',errors='ignore')
             except:
                 pass
+            df[tag] = df[tag].astype('|S')        
+        return np.ascontiguousarray(df.to_records(index=False))
     
-        return False
+    def __setitem__(self, tag, value):
+        self.static_chg = True
+        self.static[tag] = value
+                
+    def __getitem__(self, tag):
+        return self.static[tag]
+    
+    @staticmethod
+    def list(keyword, user='master'):
+        mdprefix = user+'/Metadata/'
+        keys = S3ListFolder(mdprefix+keyword)
+        keys = keys[['.bin' in k for k in keys]]
+        keys = [k.replace(mdprefix,'').split('.')[0] for k in keys]
+        return keys
 
     # READ
-    def Read(self):
-        if 'LEGACY_READ' in os.environ:
-            return self.LegacyRead()
-        else:
-            return self.ReadDataFrame()
-
-    def ReadDataFrame(self):
-        tini = time.time()
-        path, shm_name = self.getDataPath()
-        local_path = str(path/(self.tagstr+'.bin'))
-        remote_path = local_path+'.gzip'
-        df_io = None
-        if self.sharedData.s3read:
-            #Synchronize S3
-            force_download= (not self.sharedData.save_local)
-            [df_io_gzip, df_local_mtime, df_remote_mtime] = \
-                S3Download(local_path,remote_path,force_download)
-            if not df_io_gzip is None:
-                df_io = io.BytesIO()
-                df_io_gzip.seek(0)
-                with gzip.GzipFile(fileobj=df_io_gzip, mode='rb') as gz:
-                    shutil.copyfileobj(gz,df_io)                
-                if self.sharedData.save_local:
-                    SharedDataFrame.write_file(df_io,local_path,df_remote_mtime)
-                    UpdateModTime(local_path,df_remote_mtime)
-
-        if (df_io is None) & (self.sharedData.save_local):
-            # read local
-            if os.path.isfile(str(local_path)):
-                df_io = open(str(local_path),'rb')
-
-        if not df_io is None:
-            return SharedDataFrame.read_data(df_io,local_path)
-                
-        return pd.DataFrame([])
+    def load(self):
+        t = time.time()
+        self.fpath = Path(os.environ['DATABASE_FOLDER']) / self.user
+        self.pathxls = self.fpath /  ('Metadata/'+self.name+'.xlsx')
+        self.path = self.fpath /  ('Metadata/'+self.name+'.bin')
+        
+        if not self.path.parent.exists():
+            if self.save_local:
+                self.path.parent.mkdir(parents=True, exist_ok=True)
+        
+        readbin=True
+        readxlsx=False
+        if self.save_local:
+            # prefer read pkl
+            # but read excel if newer        
+            readbin = self.path.is_file()
+            readxlsx = self.pathxls.is_file()
+            if (readbin) & (readxlsx):
+                readxlsx = os.path.getmtime(self.pathxls)>os.path.getmtime(self.path)
+                readbin = not readxlsx
+                        
+        if (not readxlsx) | (not self.save_local):
+            md_io = None
+            if (self.s3read):
+                force_download = (not self.save_local)
+                [md_io_gzip, local_mtime, remote_mtime] = \
+                    S3Download(str(self.path),str(self.path)+'.gzip',force_download)
+                if (not md_io_gzip is None):
+                    md_io = io.BytesIO()
+                    md_io_gzip.seek(0)
+                    with gzip.GzipFile(fileobj=md_io_gzip, mode='rb') as gz:
+                        shutil.copyfileobj(gz,md_io)
+                    self.read_metadata_io(md_io)
+                    if (self.save_local):
+                        #save local
+                        Metadata.write_file(md_io,self.path,remote_mtime)
+                        UpdateModTime(self.path,remote_mtime)
+                        
+            if (md_io is None) & (self.path.is_file()):
+                with open(str(self.path),'rb') as md_io:
+                    self.read_metadata_io(md_io)
 
-    def read_data(df_io,local_path):
-        df_io.seek(0)
-        _header = np.frombuffer(df_io.read(40),dtype=np.int64) 
-        _idx_b = df_io.read(int(_header[2]))
-        _idxcsv = _idx_b.decode(encoding='UTF-8',errors='ignore')   
-        _idx = _idxcsv.split(',')
-        _colscsv_b = df_io.read(int(_header[3]))
-        _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
-        _cols = _colscsv.split(',')
-        _data = np.frombuffer(df_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))        
-        #calculate hash
-        _m = hashlib.md5(_idx_b)
-        _m.update(_colscsv_b)
-        _m.update(_data)
-        _md5hash_b = _m.digest()
-        __md5hash_b = df_io.read(16)
-        if not _md5hash_b==__md5hash_b:
-            raise Exception('DataFrame file corrupted!\n%s' % (local_path))
-        df = pd.DataFrame(_data,index=_idx,columns=_cols)
-        df_io.close()
-        return df
+        elif readxlsx:
+            tini = time.time()
+            
+            xls = pd.read_excel(self.pathxls,sheet_name=None)
+            if 'static' in xls:
+                self.static = xls['static']
+
+            if not self.static.empty:
+                self.static = self.static.set_index(self.static.columns[0])
+                        
+            if os.environ['LOG_LEVEL']=='DEBUG':
+                Logger.log.debug('Loading metadata xlsx %s %.2f done!' % (self.name,time.time()-tini))
+        
+        if os.environ['LOG_LEVEL']=='DEBUG':
+            Logger.log.debug('Initializing Metadata %s,%s DONE!' % (self.name,self.mode))
 
+    def read_metadata_io(self,bin_io):
+        bin_io.seek(0)
+        header = np.frombuffer(bin_io.read(32),dtype=np.int64)
+        descr_str_b = bin_io.read(int(header[0]))
+        data = bin_io.read(int(header[3]))
+        md5hash_b = bin_io.read(16)
+        
+        m = hashlib.md5(descr_str_b)
+        m.update(data)
+        _md5hash_b = m.digest()
+        if not md5hash_b==_md5hash_b:
+            raise Exception('Metadata file corrupted!\n%s' % (self.path))
+
+        descr_str = descr_str_b.decode(encoding='UTF-8',errors='ignore')
+        descr = descr_str.split(';')
+        names = descr[0].split(',')
+        formats = descr[1].split(',')        
+        self._index_columns = np.array(descr[2].split(','))
+        dtype = np.dtype({'names':names,'formats':formats})
+        self.records = np.ndarray((header[2],),dtype=dtype, buffer=data)
+        
     # WRITE
-    def Write(self,startDate=None):
-        if 'LEGACY_WRITE' in os.environ:
-            self.LegacyWrite()
-        else:
-            self.write_dataframe()
+    def save(self,save_excel=False):
+        fpath = Path(os.environ['DATABASE_FOLDER']) / self.user
+        self.pathxls = fpath /  ('Metadata/'+self.name+'.xlsx')
+        self.path = fpath /  ('Metadata/'+self.name+'.bin')
 
-    def write_dataframe(self):        
-        path, shm_name = self.getDataPath(iswrite=True)
-        local_path = str(path/(self.tagstr+'.bin'))
-        remote_path = local_path+'.gzip'
-        df_io = SharedDataFrame.create_dataframe_io(self.data)
+        tini = time.time()
         mtime = datetime.now().timestamp()
-        threads=[]
-        if self.sharedData.s3write:
-            df_io.seek(0)
+        if not os.path.isdir(self.path.parents[0]):
+            os.makedirs(self.path.parents[0])
+        # save excel first so that last modified
+        # timestamp is older
+        if save_excel:
+            with open(self.pathxls, 'wb') as f:
+                writer = pd.ExcelWriter(f, engine='xlsxwriter')
+                if self.hasindex():
+                    self.static.to_excel(writer,sheet_name='static',index=True)
+                else:
+                    self.static.to_excel(writer,sheet_name='static',index=False)
+                writer.close()
+                f.flush()
+            os.utime(self.pathxls, (mtime, mtime))
+                
+        io_obj = None
+        if self.save_local:
+            io_obj = self.create_metadata_io()
+            Metadata.write_file(io_obj,self.path,mtime)
+
+        if self.s3write:
+            if io_obj is None:
+                io_obj = self.create_metadata_io()
+            io_obj.seek(0)
             gzip_io = io.BytesIO()
             with gzip.GzipFile(fileobj=gzip_io, mode='wb', compresslevel=1) as gz:
-                shutil.copyfileobj(df_io, gz)
-            threads = [*threads , \
-                Thread(target=S3Upload,args=(gzip_io, remote_path, mtime) )]
-
-        if self.sharedData.save_local:
-            threads = [*threads , \
-                Thread(target=SharedDataFrame.write_file, args=(df_io, local_path, mtime) )]
-                            
-        for i in range(len(threads)):
-            threads[i].start()
-
-        for i in range(len(threads)):
-            threads[i].join()
-
-    def create_dataframe_io(df):        
-        r, c = df.shape
-        idx_b = str.encode(','.join(df.index.values),\
-            encoding='UTF-8',errors='ignore')
-        colscsv_b = str.encode(','.join(df.columns.values),\
-            encoding='UTF-8',errors='ignore')
-        nbidx = len(idx_b)
-        nbcols = len(colscsv_b)
-        data = np.ascontiguousarray(df.values.astype(np.float64))
-        header = np.array([r,c,nbidx,nbcols,r*c*8]).astype(np.int64)
-        #calculate hash
-        m = hashlib.md5(idx_b)
-        m.update(colscsv_b)
+                shutil.copyfileobj(io_obj, gz)
+            S3Upload(gzip_io, str(self.path)+'.gzip', mtime)
+
+        if os.environ['LOG_LEVEL']=='DEBUG':
+            Logger.log.debug('Saving metadata ' + self.name + ' %.2f done!' % (time.time()-tini))
+
+    def create_metadata_io(self):        
+        data = self.records
+        descr = data.__array_interface__['descr']
+        names = ','.join([item[0] for item in descr])
+        dt = ','.join([item[1] for item in descr])        
+        if self.hasindex():
+            index = ','.join([col for col in self._index_columns])
+            descr_str = names+';'+dt+';'+index
+        else:
+            descr_str = names+';'+dt+';'
+        descr_str_b = str.encode(descr_str,encoding='UTF-8',errors='ignore')
+        header = [len(descr_str_b),data.itemsize,data.size,data.itemsize*data.size]
+        header = np.array(header).astype(np.int64)
+        m = hashlib.md5(descr_str_b)
         m.update(data)
         md5hash_b = m.digest()
-        # allocate memory
-        io_obj = io.BytesIO()
+        io_obj = io.BytesIO()        
         io_obj.write(header)
-        io_obj.write(idx_b)
-        io_obj.write(colscsv_b)
+        io_obj.write(descr_str_b)
         io_obj.write(data)
-        io_obj.write(md5hash_b)        
+        io_obj.write(md5hash_b)
         return io_obj
-
+    
+    @staticmethod
     def write_file(io_obj,path,mtime):
         with open(path, 'wb') as f:
             f.write(io_obj.getbuffer())
             f.flush()
         os.utime(path, (mtime, mtime))
-
-    # MESSAGES
-    def Broadcast(self,idx,col):
-        SharedDataRealTime.Broadcast(
-            self.sharedData,
-            self.feeder,
-            self.period,
-            self.tag,
-            idx,col)
+        
+    # UTILS
+    def mergeUpdate(self,newdf):
+        for i in range(len(newdf.index.names)):
+            idxname = newdf.index.names[i]
+            if idxname==None:
+                Logger.log.error('%s metadata mergeUpdate newdf index is None!' % self.name)
+                raise Exception('%s metadata mergeUpdate newdf index is None!' % self.name)
+            elif idxname!=self.static.index.names[i]:
+                Logger.log.error('%s metadata mergeUpdate newdf index does not match!' % self.name)
+                raise Exception('%s metadata mergeUpdate newdf index does not match!' % self.name)
+
+
+        newidx = ~newdf.index.isin(self.static.index)
+        if newidx.any():
+            self.static = self.static.reindex(index=self.static.index.union(newdf.index))
+
+        newcolsidx = ~newdf.columns.isin(self.static.columns)
+        if newcolsidx.any():
+            newcols = newdf.columns[newcolsidx]            
+            self.static = pd.concat([self.static,newdf[newcols]],axis=1)
+            
+        self.static.update(newdf)
+        self.static_chg = True
```

### Comparing `shareddata-1.4.0/src/SharedData/SharedDataTimeSeries.py` & `shareddata-2.0.0/src/SharedData/SharedDataTimeSeries.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 # THIRD PARTY LIBS
 import os,sys
 import pandas as pd
 import numpy as np
 import json
 import time
 from numba import jit
-from pandas.tseries.offsets import BDay
 from pathlib import Path
 from multiprocessing import shared_memory
-from concurrent.futures import ThreadPoolExecutor
 import io, gzip, hashlib, shutil
 from threading import Thread
 
 from subprocess import run, PIPE
 from datetime import datetime, timedelta
 
 from SharedData.Logger import Logger
-from SharedData.SharedDataAWSS3 import Legacy_S3SyncDownloadTimeSeries,\
-    Legacy_S3Upload,S3Upload,S3Download,UpdateModTime
+from SharedData.SharedDataAWSS3 import S3Upload,S3Download,UpdateModTime
 from SharedData.SharedDataRealTime import SharedDataRealTime
 
 class SharedDataTimeSeries:
 
     def __init__(self, sharedDataPeriod, tag, value=None):    
         self.sharedDataPeriod = sharedDataPeriod
         self.tag = tag
@@ -200,97 +197,15 @@
                 j = 0
                 for s in sidx:
                     if not np.isnan(s):
                         values[np.int64(t),np.int64(s)] = arr[i,j]
                     j=j+1
             i=i+1
 
-    # C R U D
-
-    # MALLOC LEGACY
-    def MallocLegacy(self, value=None):
-        tini=time.time()
-        
-        #Create write ndarray
-        path, shm_name = self.getDataPath()
-        fpath = path / ('shm_info.json')
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            Logger.log.debug('Malloc %s ...%.2f%% ' % (shm_name,0.0))
-
-        file_exists = False
-        try: # try create memory file
-            rows = len(self.index)
-            cols = len(self.columns)
-            nbytes = int(rows*cols*8)
-
-            self.shm = shared_memory.SharedMemory(\
-                name = shm_name,create=True, size=nbytes)
-
-            self.shmarr = np.ndarray((rows,cols),\
-                dtype=np.float64, buffer=self.shm.buf)
-            
-            if not value is None:
-                self.shmarr[:] = value.values.copy()
-            else:
-                self.shmarr[:] = np.nan
-            
-            self.data = pd.DataFrame(self.shmarr,\
-                        index=self.index,\
-                        columns=self.columns,\
-                        copy=False)
-            
-            if not value is None:
-                value = self.data
-
-            with open(str(fpath), 'w+') as outfile:
-                shm_info = {
-                    'shm_name':shm_name,
-                    'index': self.data.index.values.tolist(),
-                    'columns': self.data.columns.values.tolist()                                 
-                    }
-                json.dump(shm_info, outfile, indent=3)
-            
-            if os.environ['LOG_LEVEL']=='DEBUG':
-                Logger.log.debug('Malloc create %s ...%.2f%% %.2f sec! ' % \
-                    (shm_name,100,time.time()-tini))            
-            self.create_map = 'create'
-            return True
-        except:
-            pass
-        
-        if fpath.is_file():
-            with open(str(fpath), 'r') as infile:                
-                shm_info = json.load(infile)                
-                self.index = pd.Index(shm_info['index']).astype('datetime64[ns]')
-                self.columns = pd.Index(shm_info['columns'])
-                shm_name = shm_info['shm_name']
-                rows = len(self.index)
-                cols = len(self.columns)
-
-                # map memory file
-                self.shm = shared_memory.SharedMemory(\
-                    name=shm_name, create=False)
-                self.shmarr = np.ndarray((rows,cols),\
-                    dtype=np.float64, buffer=self.shm.buf)
-                self.data = pd.DataFrame(self.shmarr,\
-                            index=self.index,\
-                            columns=self.columns,\
-                            copy=False)
-                
-                if not value is None:
-                    iidx = value.index.intersection(self.data.index)
-                    icol = value.columns.intersection(self.data.columns)
-                    self.data.loc[iidx, icol] = value.loc[iidx, icol]
-
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    Logger.log.debug('Malloc map %s/%s/%s ...%.2f%% %.2f sec! ' % \
-                        (self.feeder,self.period,self.tag,100,time.time()-tini)) 
-                self.create_map = 'map'
-        return False
-      
+    # C R U D     
     def Malloc(self, value=None):
         tini=time.time()
         
         #Create write ndarray
         path, shm_name = self.getDataPath(iswrite=True)
         
         if os.environ['LOG_LEVEL']=='DEBUG':
@@ -384,21 +299,14 @@
             Logger.log.debug('Malloc map %s/%s/%s ...%.2f%% %.2f sec! ' % \
                 (self.feeder,self.period,self.tag,100,time.time()-tini)) 
         self.create_map = 'map'
         return False
     
     # READ
     def Read(self):           
-        if 'LEGACY_READ' in os.environ:
-            return self.legacy_read_multithread()
-        else:
-            return self.read_partitions()
-
-    # READ CURRENT
-    def read_partitions(self):
         tini = time.time()
         path, shm_name = self.getDataPath()
         headpath = path / (self.tag+'_head.bin')
         tailpath = path / (self.tag+'_tail.bin')   
         head_io = None
         tail_io = None
         if self.sharedData.s3read:
@@ -407,27 +315,27 @@
             [head_io_gzip, head_local_mtime, head_remote_mtime] = \
                 S3Download(str(headpath),str(headpath)+'.gzip',force_download)
             if not head_io_gzip is None:
                 head_io = io.BytesIO()
                 head_io_gzip.seek(0)
                 with gzip.GzipFile(fileobj=head_io_gzip, mode='rb') as gz:
                     shutil.copyfileobj(gz,head_io)
-                if self.sharedData.save_local:                    
+                if self.sharedData.save_local:
                     SharedDataTimeSeries.write_file(head_io,headpath,mtime=head_remote_mtime)
                     UpdateModTime(headpath,head_remote_mtime)
                     
             
             [tail_io_gzip, tail_local_mtime, tail_remote_mtime] = \
                 S3Download(str(tailpath),str(tailpath)+'.gzip',force_download)
             if not tail_io_gzip is None:
                 tail_io = io.BytesIO()
                 tail_io_gzip.seek(0)
                 with gzip.GzipFile(fileobj=tail_io_gzip, mode='rb') as gz:
                     shutil.copyfileobj(gz,tail_io)
-                if self.sharedData.save_local:                    
+                if self.sharedData.save_local:
                     SharedDataTimeSeries.write_file(tail_io,tailpath,mtime=tail_remote_mtime)
                     UpdateModTime(tailpath,tail_remote_mtime)
         
         if (head_io is None) & (self.sharedData.save_local):
             # read local
             if os.path.isfile(str(headpath)):
                 head_io = open(str(headpath),'rb')
@@ -449,103 +357,36 @@
     def read_data(self,data_io,path):
         _header = np.frombuffer(data_io.read(40),dtype=np.int64)
         _idx_b = data_io.read(int(_header[2]))
         _idx = pd.to_datetime(np.frombuffer(_idx_b,dtype=np.int64))
         _colscsv_b = data_io.read(int(_header[3]))
         _colscsv = _colscsv_b.decode(encoding='UTF-8',errors='ignore')
         _cols = _colscsv.split(',')
-        _data = np.frombuffer(data_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))        
+        _data = np.frombuffer(data_io.read(int(_header[4])),dtype=np.float64).reshape((_header[0],_header[1]))
         #calculate hash
         _m = hashlib.md5(_idx_b)
         _m.update(_colscsv_b)
         _m.update(_data)
         _md5hash_b = _m.digest()
         __md5hash_b = data_io.read(16)
         if not _md5hash_b==__md5hash_b:
             raise Exception('Timeseries file corrupted!\n%s' % (path))
         sidx = np.array([self.get_loc_symbol(s) for s in _cols])
         ts = _idx.values.astype(np.int64)/10**9 #seconds
         tidx = self.get_loc_timestamp(ts)
         self.setValuesJit(self.data.values,tidx,sidx,_data)
         data_io.close()
-
-    # READ LEGACY
-    def legacy_read_multithread(self):
-        path, shm_name = self.getDataPath() 
-        if self.sharedData.s3read:            
-            self.download_time = time.time()
-            Legacy_S3SyncDownloadTimeSeries(str(path), shm_name)
-            self.download_time = time.time()-self.download_time
-       
-        years = [int(x.stem) for x in path.glob('*.npy') if x.is_file()]
-        fpaths = [x for x in path.glob('*.npy') if x.is_file()]
-        if len(fpaths)>0:
-            mtime = [datetime.fromtimestamp(os.stat(f).st_mtime) for f in fpaths]
-            if len(mtime)>0:
-                self.last_update = max(mtime)
-                self.first_update = min(mtime)
-            else:
-                self.last_update = pd.NaT
-                self.first_update = pd.NaT
-                
-            files = pd.DataFrame([years,fpaths]).T
-            files.columns = ['year','fpath']
-            files = files.sort_values(by='year')
-            nfiles = len(files.index)
-            if nfiles>0:
-                tini=time.time()
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    Logger.log.debug('Reading %s ...%.2f%% ' % (shm_name,0.0))   
-                n=0
-                file_paths = files['fpath']
-                if file_paths.shape[0]>0:
-                    # create a thread pool
-                    with ThreadPoolExecutor(file_paths.shape[0]) as exe:
-                        futures = [exe.submit(self.legacy_read_thread, fpath) \
-                            for fpath in file_paths]
-                        # collect data
-                        data = [future.result() for future in futures]                
-                if os.environ['LOG_LEVEL']=='DEBUG':
-                    Logger.log.debug('Reading %s ...%.2f%% %.2f sec! ' % \
-                        (shm_name,100*(n/nfiles),time.time()-tini))        
-        
-    def legacy_read_thread(self,fpath):
-        arr = np.load(str(fpath),mmap_mode='r')
-        r ,c = arr.shape
-        if (r>0):                   
-            idxfpath = str(fpath).replace('.npy','.csv')
-            with open(idxfpath,'r') as f:
-                dfidx = f.read()
-            dfidx = dfidx.split(',')
-            sidx = [self.get_loc_symbol(s) for s in dfidx[1:]]
-            sidx = np.array(sidx)                    
-            ts = (arr[:,0]).astype(np.int64) #seconds
-            tidx = self.get_loc_timestamp(ts)
-
-            self.setValuesJit(self.data.values,tidx,sidx,arr[:,1:])
-            return True
-        return False
-                    
+ 
     # WRITE
-    def Write(self, busdays=None, startDate=None):
-
+    def Write(self, startDate=None):
         firstdate = self.data.first_valid_index()
-        if (startDate is None) & (busdays is None):
-            firstdate = self.startDate
-        elif not busdays is None:
-            firstdate =  self.data.last_valid_index() - BDay(busdays)
-        elif not startDate is None:
+        if not startDate is None:
             firstdate = startDate
-        
-        if 'LEGACY_WRITE' in os.environ:
-            self.legacy_write_multithread(firstdate)
-        else:
-            self.write_partitions(firstdate)
+        self.write_partitions(firstdate)
             
-    # WRITE CURRENT
     def write_partitions(self,firstdate):
         tini = time.time()
         path, shm_name = self.getDataPath(iswrite=True)
         
         partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
         threads = []
 
@@ -607,69 +448,23 @@
         md5hash_b = m.digest()
         # allocate memory
         io_obj = io.BytesIO()        
         io_obj.write(header)
         io_obj.write(idx_b)
         io_obj.write(colscsv_b)
         io_obj.write(data)
-        io_obj.write(md5hash_b)        
+        io_obj.write(md5hash_b)
         return io_obj
 
     def write_file(io_obj,path,mtime):
         with open(path, 'wb') as f:
             f.write(io_obj.getbuffer())
             f.flush()
         os.utime(path, (mtime, mtime))
 
-    # WRITE LEGACY
-    def legacy_write_multithread(self, firstdate):
-        tini = time.time()
-        if os.environ['LOG_LEVEL']=='DEBUG':
-            startdatestr = firstdate.strftime('%Y-%m-%d')
-            Logger.log.debug('Writing %s from %s ...%.2f%% ' % \
-                (shm_name,startdatestr,0.0))
-        path, shm_name = self.getDataPath(iswrite=True)
-        if not os.path.isdir(path):
-            os.makedirs(path)                
-        years = self.data.loc[firstdate:,:].index.year.unique()
-        if years.shape[0]>0:
-            # create a thread pool
-            with ThreadPoolExecutor(years.shape[0]) as exe:
-                futures = [exe.submit(self.legacy_write_thread, year, path) \
-                    for year in years]
-                # collect data
-                data = [future.result() for future in futures]
-
-            if os.environ['LOG_LEVEL']=='DEBUG':
-                Logger.log.debug('Writing %s from %s ...%.2f%% %.2f sec!' % \
-                    (shm_name,startdatestr,100,time.time()-tini))        
-        
-    def legacy_write_thread(self,y, path):
-        idx = self.data.index[self.data.index.year==y]
-        dfyear = self.data.loc[idx,:].copy()
-        dfyear = dfyear.dropna(how='all').dropna(axis=1,how='all')
-        if dfyear.shape[0]>0:
-            dfyear.index = (dfyear.index.astype(np.int64)/10**9).astype(np.int64)
-            dfyear = dfyear.reset_index()
-
-            fpath_npy = path / (str(y)+'.npy')
-            with open(fpath_npy, 'wb') as f:
-                np.save(f,dfyear.values.astype(np.float64))
-                f.flush()
-            
-            cols = ','.join(dfyear.columns)            
-            fpath_csv = path / (str(y)+'.csv')    
-            with open(fpath_csv, 'w') as f:
-                f.write(cols)
-                f.flush()
-
-            if self.sharedData.s3write:                
-                Legacy_S3Upload(fpath_npy)
-                Legacy_S3Upload(fpath_csv)
-            
     # MESSAGES
     def Broadcast(self,idx,col):
         SharedDataRealTime.Broadcast(
             self.sharedData,
             self.feeder,
             self.period,
             self.tag,
```

### Comparing `shareddata-1.4.0/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.0.0/src/shareddata.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 1.4.0
+Version: 2.0.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

