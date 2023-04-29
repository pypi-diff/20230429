# Comparing `tmp/mynacode-1.0.88-py3-none-any.whl.zip` & `tmp/mynacode-1.0.89-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8791 bytes, number of entries: 9
+Zip file size: 8789 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5876 b- defN 23-Apr-29 05:22 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 05:22 mynacode-1.0.88.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 05:22 mynacode-1.0.88.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 05:22 mynacode-1.0.88.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 05:22 mynacode-1.0.88.dist-info/RECORD
-9 files, 28936 bytes uncompressed, 7611 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     5880 b- defN 23-Apr-29 05:24 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 05:25 mynacode-1.0.89.dist-info/RECORD
+9 files, 28940 bytes uncompressed, 7609 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.88.dist-info/METADATA
+Filename: mynacode-1.0.89.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.88.dist-info/WHEEL
+Filename: mynacode-1.0.89.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.88.dist-info/top_level.txt
+Filename: mynacode-1.0.89.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.88.dist-info/RECORD
+Filename: mynacode-1.0.89.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -158,15 +158,15 @@
     prec, rec, spec, f1, acc, npv_val, c_matrix = get_metrics(y_true, y_predicted, threshold)
     fpr, tpr, roc_auc, gmeans, best_threshold, index = get_roc_auc(y_true, y_predicted)
     #t_cmatrix = PrettyTable(['', 'No Disease', 'Disease'])
     #t_cmatrix.add_row(["No Disease", c_matrix[0][0], c_matrix[0][1]])
     #t_cmatrix.add_row(["Disease", c_matrix[1][0], c_matrix[1][1]])                
     #print(t_cmatrix)
 
-    data = {'run_id' : run_id, 'precision': prec, 'recall': rec, 'specificity': spec, 'f1': f1, 'accuracy': acc, 'npv': npv, 'c_matrix': c_matrix,
+    data = {'run_id' : run_id, 'precision': prec, 'recall': rec, 'specificity': spec, 'f1': f1, 'accuracy': acc, 'npv': npv_val, 'c_matrix': c_matrix,
             'username': username, 'key': key, 'test_auc': roc_auc}
 
     response = requests.post(protocol+'://'+IP+'/api/add_results', data=data)
   
     if response.text == '0':
       print("Authentication failed")
     else:
```

## Comparing `mynacode-1.0.88.dist-info/RECORD` & `mynacode-1.0.89.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=yDKLN9E6mzyGygKUOX-f72y08UEkO9PuKLOyolbC5J4,5876
-mynacode-1.0.88.dist-info/METADATA,sha256=LBtycY16f7VWiGbWy3_tARhIkzFlLidKP8AETCHzkEA,352
-mynacode-1.0.88.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.88.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.88.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=COW9lnhyBSOG1WUke4hIIuIzpV3KBAaulNRk0EE0BXI,5880
+mynacode-1.0.89.dist-info/METADATA,sha256=CNQKKS30ITGT29r5kOvGve3-Hqs_WJe23tiI5DcP34Q,352
+mynacode-1.0.89.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.89.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.89.dist-info/RECORD,,
```

