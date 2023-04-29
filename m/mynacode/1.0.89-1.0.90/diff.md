# Comparing `tmp/mynacode-1.0.89-py3-none-any.whl.zip` & `tmp/mynacode-1.0.90-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8789 bytes, number of entries: 9
+Zip file size: 8812 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5880 b- defN 23-Apr-29 05:24 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/RECORD
-9 files, 28940 bytes uncompressed, 7609 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     5985 b- defN 23-Apr-29 20:09 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 20:17 mynacode-1.0.90.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 20:17 mynacode-1.0.90.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 20:17 mynacode-1.0.90.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 20:17 mynacode-1.0.90.dist-info/RECORD
+9 files, 29045 bytes uncompressed, 7632 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.89.dist-info/METADATA
+Filename: mynacode-1.0.90.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.89.dist-info/WHEEL
+Filename: mynacode-1.0.90.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.89.dist-info/top_level.txt
+Filename: mynacode-1.0.90.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.89.dist-info/RECORD
+Filename: mynacode-1.0.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -73,15 +73,15 @@
     print("Authentication failed")
   else:
     print("Metadata saved")
    
 
 
 
-def datasets(train, test, val, run_id = -999):
+def datasets(train, test, val, run_id):
 
   train = np.array(train)
   test = np.array(test)
   val = np.array(val)
 
   train_shape = train.shape
   test_shape = test.shape
@@ -94,21 +94,25 @@
   response = requests.post(protocol+'://'+IP+'/api/add_datasets', data=data)
   
   if response.text == '0':
     print("Authentication failed")
   else:
     print("Datasets Information saved.")
 
-def csv_data(dataframe, run_id = -999):
+def csv_data(dataframe, run_id):
     columns_list = dataframe.columns.values.tolist()
+    print(columns_list)
     isnull_list = dataframe.isnull().sum().values.tolist()
+    print(isnull_list)
     isunique_list = dataframe.nunique().values.tolist()
+    print(isunique_list)
     dtypes_list = dataframe.dtypes.tolist()
+    print(dtypes_list)
 
-    data = {'run_id': run_id, 'columns_list': columns_list, 'isnull_list': isnull_list, 'isunique_list': isunique_list, 'dtypes_list': dtypes_list}
+    data = {'run_id': run_id, 'columns_list': str(columns_list), 'isnull_list': str(isnull_list), 'isunique_list': str(isunique_list), 'dtypes_list': str(dtypes_list)}
 
     response = requests.post(protocol+'://'+IP+'/api/add_csv', data=data)
 
     if response.text == '0':
       print("Authentication failed")
     else:
       print("CSV Information saved.")
```

## Comparing `mynacode-1.0.89.dist-info/RECORD` & `mynacode-1.0.90.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=COW9lnhyBSOG1WUke4hIIuIzpV3KBAaulNRk0EE0BXI,5880
-mynacode-1.0.89.dist-info/METADATA,sha256=CNQKKS30ITGT29r5kOvGve3-Hqs_WJe23tiI5DcP34Q,352
-mynacode-1.0.89.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.89.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.89.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=3C9VLSlHzNcSaB8hd2vSuQJlA0jBeaNwIMSrLOBcuJk,5985
+mynacode-1.0.90.dist-info/METADATA,sha256=7tPWwCH0m3hiQWSqx7yhi3IxW_AhsG8MZxML3bWKYSU,352
+mynacode-1.0.90.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.90.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.90.dist-info/RECORD,,
```

