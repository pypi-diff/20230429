# Comparing `tmp/jurebes-0.1.1a8-py3-none-any.whl.zip` & `tmp/jurebes-0.1.1a9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5887 bytes, number of entries: 7
--rw-r--r--  2.0 unx    17940 b- defN 23-Apr-29 00:11 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-29 00:11 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-29 00:11 jurebes-0.1.1a8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 00:11 jurebes-0.1.1a8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 00:11 jurebes-0.1.1a8.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-29 00:11 jurebes-0.1.1a8.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-29 00:11 jurebes-0.1.1a8.dist-info/RECORD
-7 files, 19514 bytes uncompressed, 4919 bytes compressed:  74.8%
+Zip file size: 5885 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    17948 b- defN 23-Apr-29 01:54 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-29 01:54 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-29 01:54 jurebes-0.1.1a9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 01:54 jurebes-0.1.1a9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 01:54 jurebes-0.1.1a9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-29 01:54 jurebes-0.1.1a9.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-29 01:54 jurebes-0.1.1a9.dist-info/RECORD
+7 files, 19522 bytes uncompressed, 4917 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.1a8.dist-info/METADATA
+Filename: jurebes-0.1.1a9.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.1a8.dist-info/WHEEL
+Filename: jurebes-0.1.1a9.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.1a8.dist-info/top_level.txt
+Filename: jurebes-0.1.1a9.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.1a8.dist-info/zip-safe
+Filename: jurebes-0.1.1a9.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.1a8.dist-info/RECORD
+Filename: jurebes-0.1.1a9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -196,15 +196,15 @@
                 # inject regex extracted entities
                 if self.padacioso.fuzz or exact_intent["conf"] >= 0.8:
                     ents.update(exact_intent["entities"])
                 exact_intents.append(IntentMatch(confidence=exact_intent["conf"],
                                                  intent_name=exact_intent["name"],
                                                  entities=exact_intent["entities"]))
 
-        for intent_name, samples in self.intent_samples:
+        for intent_name, samples in self.intent_samples.items():
             if any(s == query for s in samples if "{" not in s):
                 # update confidence of previous match
                 for idx, i in enumerate(exact_intents):
                     if i.intent_name == intent_name:
                         exact_intents[idx].confidence = 1
                         break
                 # add new exact match
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 1
-VERSION_ALPHA = 8
+VERSION_ALPHA = 9
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.1a8.dist-info/METADATA` & `jurebes-0.1.1a9.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.1a8
+Version: 0.1.1a9
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

