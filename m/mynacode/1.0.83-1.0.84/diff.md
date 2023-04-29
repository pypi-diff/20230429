# Comparing `tmp/mynacode-1.0.83-py3-none-any.whl.zip` & `tmp/mynacode-1.0.84-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 8792 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5853 b- defN 23-Apr-29 05:15 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 05:15 mynacode-1.0.83.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 05:15 mynacode-1.0.83.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 05:15 mynacode-1.0.83.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 05:15 mynacode-1.0.83.dist-info/RECORD
-9 files, 28913 bytes uncompressed, 7612 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     5854 b- defN 23-Apr-29 05:17 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 05:17 mynacode-1.0.84.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 05:17 mynacode-1.0.84.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 05:17 mynacode-1.0.84.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 05:17 mynacode-1.0.84.dist-info/RECORD
+9 files, 28914 bytes uncompressed, 7612 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.83.dist-info/METADATA
+Filename: mynacode-1.0.84.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.83.dist-info/WHEEL
+Filename: mynacode-1.0.84.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.83.dist-info/top_level.txt
+Filename: mynacode-1.0.84.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.83.dist-info/RECORD
+Filename: mynacode-1.0.84.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -84,15 +84,15 @@
   val = np.array(val)
 
   train_shape = train.shape
   test_shape = test.shape
   val_shape = val.shape
 
 
-  data = {'run_id': run_id, train_shape' : train_shape, 'test_shape': test_shape, 'val_shape': val_shape,
+  data = {'run_id': run_id, 'train_shape' : train_shape, 'test_shape': test_shape, 'val_shape': val_shape,
           'username': username, 'key': key}
   
   response = requests.post(protocol+'://'+IP+'/api/add_datasets', data=data)
   
   if response.text == '0':
     print("Authentication failed")
   else:
```

## Comparing `mynacode-1.0.83.dist-info/RECORD` & `mynacode-1.0.84.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=-A0RUCJ_dCvPlCrSklxguIEM--jKaje4iAXasp2Yi74,5853
-mynacode-1.0.83.dist-info/METADATA,sha256=dWZxVO8ezCTwGkCCx5iL6BNJ91cG9T45DzFPVkCC_fU,352
-mynacode-1.0.83.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.83.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.83.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=dqWkyBXbcH3mCRje8aqT8HNYTdXWYJLfw7Vm92n6fMI,5854
+mynacode-1.0.84.dist-info/METADATA,sha256=i9iJx_hFyN_XtRxNUsj_QMUXKwV26qt2mFI50sHtgF0,352
+mynacode-1.0.84.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.84.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.84.dist-info/RECORD,,
```

