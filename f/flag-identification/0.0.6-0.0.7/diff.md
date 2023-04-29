# Comparing `tmp/flag_identification-0.0.6.tar.gz` & `tmp/flag_identification-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flag_identification-0.0.6.tar", last modified: Sat Mar  4 15:50:38 2023, max compression
+gzip compressed data, was "flag_identification-0.0.7.tar", last modified: Sat Apr 29 10:31:30 2023, max compression
```

## Comparing `flag_identification-0.0.6.tar` & `flag_identification-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 15:50:38.177229 flag_identification-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-04 15:49:15.000000 flag_identification-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-04 15:50:38.177229 flag_identification-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-04 15:49:15.000000 flag_identification-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-04 15:50:38.177229 flag_identification-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-04 15:49:15.000000 flag_identification-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 15:50:38.173229 flag_identification-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 15:50:38.173229 flag_identification-0.0.6/src/flag_identification/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 15:50:38.173229 flag_identification-0.0.6/src/flag_identification/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/move_additional_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/predict_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/pull_wikimedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/remove_dups.py
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/bin/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-04 15:49:15.000000 flag_identification-0.0.6/src/flag_identification/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 15:50:38.173229 flag_identification-0.0.6/src/flag_identification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-04 15:50:38.000000 flag_identification-0.0.6/src/flag_identification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-03-04 15:50:38.000000 flag_identification-0.0.6/src/flag_identification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-04 15:50:38.000000 flag_identification-0.0.6/src/flag_identification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-04 15:50:38.000000 flag_identification-0.0.6/src/flag_identification.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-04 15:50:38.000000 flag_identification-0.0.6/src/flag_identification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-04 15:50:38.000000 flag_identification-0.0.6/src/flag_identification.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-04 15:50:38.177229 flag_identification-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-04 15:49:15.000000 flag_identification-0.0.6/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:31:30.204437 flag_identification-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-29 10:30:04.000000 flag_identification-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 10:31:30.204437 flag_identification-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-29 10:30:04.000000 flag_identification-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 10:31:30.204437 flag_identification-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-29 10:30:04.000000 flag_identification-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:31:30.196437 flag_identification-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:31:30.200437 flag_identification-0.0.7/src/flag_identification/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:31:30.204437 flag_identification-0.0.7/src/flag_identification/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/move_additional_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/predict_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/pull_wikimedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/remove_dups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/bin/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-29 10:30:04.000000 flag_identification-0.0.7/src/flag_identification/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:31:30.200437 flag_identification-0.0.7/src/flag_identification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-29 10:31:30.000000 flag_identification-0.0.7/src/flag_identification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-04-29 10:31:30.000000 flag_identification-0.0.7/src/flag_identification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 10:31:30.000000 flag_identification-0.0.7/src/flag_identification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-29 10:31:30.000000 flag_identification-0.0.7/src/flag_identification.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-29 10:31:30.000000 flag_identification-0.0.7/src/flag_identification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-29 10:31:30.000000 flag_identification-0.0.7/src/flag_identification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 10:31:30.204437 flag_identification-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-29 10:30:04.000000 flag_identification-0.0.7/test/test_utils.py
```

### Comparing `flag_identification-0.0.6/LICENSE` & `flag_identification-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/README.md` & `flag_identification-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/setup.py` & `flag_identification-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "scikit-learn",
     "Pillow",
     "opencv-python",
 )
 
 setup(
     name="flag_identification",
-    version="0.0.6",
+    version="0.0.7",
     python_requires=">=3.6",
     description="Identify a flag by an image",
     long_description="Identify a flag by an image",
     author="Robert Lucey",
     url="https://github.com/RobertLucey/flag-identification",
     packages=find_packages("src"),
     package_dir={"": "src"},
```

### Comparing `flag_identification-0.0.6/src/flag_identification/bin/predict.py` & `flag_identification-0.0.7/src/flag_identification/bin/predict.py`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/src/flag_identification/bin/predict_single.py` & `flag_identification-0.0.7/src/flag_identification/bin/predict_single.py`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/src/flag_identification/bin/prep.py` & `flag_identification-0.0.7/src/flag_identification/bin/prep.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,16 @@
 
 
 def populate_prep():
     # TODO: warn of dups
 
     wipe_dir(PREP_DIR)
 
-    copy_tree(ADDITIONAL_IMAGES_DIR, PREP_DIR)
+    if os.path.exists(ADDITIONAL_IMAGES_DIR):
+        copy_tree(ADDITIONAL_IMAGES_DIR, PREP_DIR)
 
     print(f"Moving pngs from {RAW_DIR} to {PREP_DIR}")
     labels = set()
     for f in os.listdir(RAW_DIR):
         label = f.split("_")[-1].replace("–", "-")
         label = unicodedata.normalize("NFKD", label).encode("ASCII", "ignore")
         label = str(label, "utf-8")
@@ -119,15 +120,15 @@
     # Only do this if mogrify installed
     clean_pngs(PREP_DIR)
 
     wipe_dir(AUGMENTED_DIR)
 
     pool = Pool()
     for _ in tqdm.tqdm(
-        pool.imap_unordered(mod_file, [(100, f) for f in os.listdir(PREP_DIR)]),
+        pool.imap_unordered(mod_file, [(50, f) for f in os.listdir(PREP_DIR)]),
         total=len(os.listdir(PREP_DIR)),
     ):
         pass
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flag_identification-0.0.6/src/flag_identification/bin/pull_wikimedia.py` & `flag_identification-0.0.7/src/flag_identification/bin/pull_wikimedia.py`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/src/flag_identification/bin/remove_dups.py` & `flag_identification-0.0.7/src/flag_identification/bin/remove_dups.py`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/src/flag_identification/bin/train.py` & `flag_identification-0.0.7/src/flag_identification/bin/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         yield l[i : i + n]
 
 
 def main():
 
     prep_files = os.listdir(PREP_DIR)
 
-    range_max = int(len(prep_files) / 300)
+    range_max = int(len(prep_files) / 500)
 
     for idx in range(range_max):
         print(f"STARTING ROUND {idx + 1}")
 
         # split into range_max and select idx of os.path.listdir(PREP_DIR)
         flags_to_use = list(chunks(prep_files, int(len(prep_files) / range_max)))[idx]
 
@@ -198,15 +198,15 @@
 
         classes = list(df.keys())
         model = get_model(classes)
 
         model.fit(
             x_train,
             y_train,
-            epochs=4,
+            epochs=6,
             validation_data=(x_test, y_test),
             batch_size=64,
         )
 
         model.save(f"{MODEL_PATH}_{idx}")
```

### Comparing `flag_identification-0.0.6/src/flag_identification/logging.py` & `flag_identification-0.0.7/src/flag_identification/logging.py`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/src/flag_identification/utils.py` & `flag_identification-0.0.7/src/flag_identification/utils.py`

 * *Files identical despite different names*

### Comparing `flag_identification-0.0.6/src/flag_identification.egg-info/SOURCES.txt` & `flag_identification-0.0.7/src/flag_identification.egg-info/SOURCES.txt`

 * *Files identical despite different names*

