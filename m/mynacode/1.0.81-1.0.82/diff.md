# Comparing `tmp/mynacode-1.0.81-py3-none-any.whl.zip` & `tmp/mynacode-1.0.82-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8768 bytes, number of entries: 9
+Zip file size: 8787 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5678 b- defN 23-Apr-28 05:01 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-28 05:02 mynacode-1.0.81.dist-info/RECORD
-9 files, 28738 bytes uncompressed, 7588 bytes compressed:  73.6%
+-rw-rw-rw-  2.0 fat     5860 b- defN 23-Apr-29 03:47 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 04:27 mynacode-1.0.82.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 04:27 mynacode-1.0.82.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 04:27 mynacode-1.0.82.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 04:27 mynacode-1.0.82.dist-info/RECORD
+9 files, 28920 bytes uncompressed, 7607 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.81.dist-info/METADATA
+Filename: mynacode-1.0.82.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.81.dist-info/WHEEL
+Filename: mynacode-1.0.82.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.81.dist-info/top_level.txt
+Filename: mynacode-1.0.82.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.81.dist-info/RECORD
+Filename: mynacode-1.0.82.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -73,42 +73,42 @@
     print("Authentication failed")
   else:
     print("Metadata saved")
    
 
 
 
-def datasets(train, test, val):
+def datasets(train, test, val, run_id = -999):
 
   train = np.array(train)
   test = np.array(test)
   val = np.array(val)
 
   train_shape = train.shape
   test_shape = test.shape
   val_shape = val.shape
 
 
-  data = {'train_shape' : train_shape, 'test_shape': test_shape, 'val_shape': val_shape,
+  data = {'run_id': run_id, train_shape' : train_shape, 'test_shape': test_shape, 'val_shape': val_shape,
           'username': username, 'key': key}
   
   response = requests.post(protocol+'://'+IP+'/api/add_datasets', data=data)
   
   if response.text == '0':
     print("Authentication failed")
   else:
     print("Datasets Information saved.")
 
-def csv_data(dataframe):
+def csv_data(dataframe, run_id = -999):
     columns_list = dataframe.columns.values.tolist()
     isnull_list = dataframe.isnull().sum().values.tolist()
     isunique_list = dataframe.nunique().values.tolist()
     dtypes_list = dataframe.dtypes.tolist()
 
-    data = {'columns_list': columns_list, 'isnull_list': isnull_list, 'isunique_list': isunique_list, 'dtypes_list': dtypes_list}
+    data = {'run_id': run_id, columns_list': columns_list, 'isnull_list': isnull_list, 'isunique_list': isunique_list, 'dtypes_list': dtypes_list}
 
     response = requests.post(protocol+'://'+IP+'/api/add_csv', data=data)
 
     if response.text == '0':
       print("Authentication failed")
     else:
       print("CSV Information saved.")
@@ -150,23 +150,24 @@
    
     c_matrix = confusion_matrix(y_true, y_pred_binary, labels=[0,1])
    
     return prec, rec, spec, f1, acc, npv_val, c_matrix
 
 
 
-def results(predicted_values, test_labels, problem_type = 'binary classification', threshold = 0.5):
-    prec, rec, spec, f1, acc, npv_val, c_matrix = get_metrics(y_true, y_pred, threshold)
+def results(y_predicted, y_true, problem_type = 'binary classification', threshold = 0.5, run_id = -999):
+    prec, rec, spec, f1, acc, npv_val, c_matrix = get_metrics(y_true, y_predicted, threshold)
+    fpr, tpr, roc_auc, gmeans, best_threshold, index = get_roc_auc(y_true, y_predicted)
     #t_cmatrix = PrettyTable(['', 'No Disease', 'Disease'])
     #t_cmatrix.add_row(["No Disease", c_matrix[0][0], c_matrix[0][1]])
     #t_cmatrix.add_row(["Disease", c_matrix[1][0], c_matrix[1][1]])                
     #print(t_cmatrix)
 
-    data = {'node_id' : node_id, 'precision': prec, 'recall': recall, 'specificity': spec, 'f1': f1, 'accuracy': acc, 'npv': npv, 'c_matrix': c_matrix,
-            'username': username, 'key': key}
+    data = {'run_id' : run_id, 'precision': prec, 'recall': recall, 'specificity': spec, 'f1': f1, 'accuracy': acc, 'npv': npv, 'c_matrix': c_matrix,
+            'username': username, 'key': key, 'test_auc': roc_auc}
 
     response = requests.post(protocol+'://'+IP+'/api/add_results', data=data)
   
     if response.text == '0':
       print("Authentication failed")
     else:
       print("Results saved")
```

## Comparing `mynacode-1.0.81.dist-info/RECORD` & `mynacode-1.0.82.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=HK5tPt4zsGjRVWLEZZA57m5WAD1HqDWNT2tIiG4yueA,5678
-mynacode-1.0.81.dist-info/METADATA,sha256=mUhJtej5ifdTDTJSD6I-erzOONvkFySBzrJS9whhS-Y,352
-mynacode-1.0.81.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.81.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.81.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=SYfO-buU9_HCklmrBTX2JNL_1_aAqU9IqcN_uEdsL9U,5860
+mynacode-1.0.82.dist-info/METADATA,sha256=JB60prYPenMa0GyQennyBtVIqphy_03MpgufD0VgSD8,352
+mynacode-1.0.82.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.82.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.82.dist-info/RECORD,,
```

