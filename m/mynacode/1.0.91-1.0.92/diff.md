# Comparing `tmp/mynacode-1.0.91-py3-none-any.whl.zip` & `tmp/mynacode-1.0.92-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8794 bytes, number of entries: 9
+Zip file size: 8814 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      102 b- defN 22-Sep-11 20:53 mlauto/__init__.py
 -rw-rw-rw-  2.0 fat    13388 b- defN 23-Feb-02 06:52 mlauto/mlauto.py
 -rw-rw-rw-  2.0 fat      111 b- defN 23-Feb-24 03:08 mynacode/__init__.py
 -rw-rw-rw-  2.0 fat     8317 b- defN 23-Mar-20 01:11 mynacode/mynacode - Copy.py
--rw-rw-rw-  2.0 fat     5928 b- defN 23-Apr-29 20:20 mynacode/mynacode.py
--rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 20:21 mynacode-1.0.91.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 20:21 mynacode-1.0.91.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 20:21 mynacode-1.0.91.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 20:21 mynacode-1.0.91.dist-info/RECORD
-9 files, 28988 bytes uncompressed, 7614 bytes compressed:  73.7%
+-rw-rw-rw-  2.0 fat     5979 b- defN 23-Apr-29 21:34 mynacode/mynacode.py
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Apr-29 21:35 mynacode-1.0.92.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-29 21:35 mynacode-1.0.92.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-29 21:35 mynacode-1.0.92.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      689 b- defN 23-Apr-29 21:35 mynacode-1.0.92.dist-info/RECORD
+9 files, 29039 bytes uncompressed, 7634 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mynacode/mynacode - Copy.py
 Comment: 
 
 Filename: mynacode/mynacode.py
 Comment: 
 
-Filename: mynacode-1.0.91.dist-info/METADATA
+Filename: mynacode-1.0.92.dist-info/METADATA
 Comment: 
 
-Filename: mynacode-1.0.91.dist-info/WHEEL
+Filename: mynacode-1.0.92.dist-info/WHEEL
 Comment: 
 
-Filename: mynacode-1.0.91.dist-info/top_level.txt
+Filename: mynacode-1.0.92.dist-info/top_level.txt
 Comment: 
 
-Filename: mynacode-1.0.91.dist-info/RECORD
+Filename: mynacode-1.0.92.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mynacode/mynacode.py

```diff
@@ -98,15 +98,18 @@
   else:
     print("Datasets Information saved.")
 
 def csv(dataframe, run_id):
     columns_list = dataframe.columns.values.tolist()
     isnull_list = dataframe.isnull().sum().values.tolist()
     isunique_list = dataframe.nunique().values.tolist()
-    dtypes_list = dataframe.dtypes.tolist()
+    dtypes_list = []
+
+    for d in dataframe.dtypes.tolist():
+        dtypes_list.append(d)
 
     data = {'run_id': run_id, 'columns_list': str(columns_list), 'isnull_list': str(isnull_list), 'isunique_list': str(isunique_list), 'dtypes_list': str(dtypes_list),
             'username': username, 'key': key}
 
     response = requests.post(protocol+'://'+IP+'/api/add_csv', data=data)
 
     if response.text == '0':
```

## Comparing `mynacode-1.0.91.dist-info/RECORD` & `mynacode-1.0.92.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlauto/__init__.py,sha256=oF_0vCehmivw-qD8z2tkyGk12n7CIJK2WPKqtcGtK_Y,102
 mlauto/mlauto.py,sha256=Qx7vf9SoDjsM_xBhSwg6TSf8F3xjS63wxMYvsxlCFb0,13388
 mynacode/__init__.py,sha256=qzUS3oZUS9IMp1DFKSYsXkwCY9whoh9pSUicECIkFks,111
 mynacode/mynacode - Copy.py,sha256=6wRDTZ27gkfKlqucw2bTfbaHdQBEEsqsVacPd3Qnn2o,8317
-mynacode/mynacode.py,sha256=dejnxMDkdM9EoL4FgWN2aKLy2z44NepZgDLyhoIM4lw,5928
-mynacode-1.0.91.dist-info/METADATA,sha256=ucNuEQtH3PduT3Up-TIH2PHPk_aAkzbFjT1HG55TT5k,352
-mynacode-1.0.91.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mynacode-1.0.91.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
-mynacode-1.0.91.dist-info/RECORD,,
+mynacode/mynacode.py,sha256=ojIa6p1ol2OurMf948g6EBH7i7N0J1H2OhaV4K-1i6s,5979
+mynacode-1.0.92.dist-info/METADATA,sha256=oALjgNv_MxvuyzNKQf6kkWZXdG27lLO8gOkq9cttzX4,352
+mynacode-1.0.92.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mynacode-1.0.92.dist-info/top_level.txt,sha256=tXscqhNo1yaYgnPdY61gZmmSsmDNJ96O2ebga4CPYvo,9
+mynacode-1.0.92.dist-info/RECORD,,
```

