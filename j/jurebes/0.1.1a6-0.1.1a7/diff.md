# Comparing `tmp/jurebes-0.1.1a6-py3-none-any.whl.zip` & `tmp/jurebes-0.1.1a7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5738 bytes, number of entries: 7
--rw-r--r--  2.0 unx    17310 b- defN 23-Apr-25 16:35 jurebes/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-25 16:35 jurebes/version.py
--rw-r--r--  2.0 unx      753 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/zip-safe
--rw-rw-r--  2.0 unx      543 b- defN 23-Apr-25 16:35 jurebes-0.1.1a6.dist-info/RECORD
-7 files, 18884 bytes uncompressed, 4770 bytes compressed:  74.7%
+Zip file size: 5884 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    17979 b- defN 23-Apr-28 23:52 jurebes/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Apr-28 23:52 jurebes/version.py
+-rw-r--r--  2.0 unx      753 b- defN 23-Apr-28 23:52 jurebes-0.1.1a7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 23:52 jurebes-0.1.1a7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-28 23:52 jurebes-0.1.1a7.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-28 23:52 jurebes-0.1.1a7.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      543 b- defN 23-Apr-28 23:52 jurebes-0.1.1a7.dist-info/RECORD
+7 files, 19553 bytes uncompressed, 4916 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jurebes/__init__.py
 Comment: 
 
 Filename: jurebes/version.py
 Comment: 
 
-Filename: jurebes-0.1.1a6.dist-info/METADATA
+Filename: jurebes-0.1.1a7.dist-info/METADATA
 Comment: 
 
-Filename: jurebes-0.1.1a6.dist-info/WHEEL
+Filename: jurebes-0.1.1a7.dist-info/WHEEL
 Comment: 
 
-Filename: jurebes-0.1.1a6.dist-info/top_level.txt
+Filename: jurebes-0.1.1a7.dist-info/top_level.txt
 Comment: 
 
-Filename: jurebes-0.1.1a6.dist-info/zip-safe
+Filename: jurebes-0.1.1a7.dist-info/zip-safe
 Comment: 
 
-Filename: jurebes-0.1.1a6.dist-info/RECORD
+Filename: jurebes-0.1.1a7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jurebes/__init__.py

```diff
@@ -52,14 +52,15 @@
 
     def disable_fuzzy(self):
         self.padacioso.fuzz = False
 
     def add_intent(self, intent_name, samples):
         expanded = []
         for l in samples:
+            l = l.replace("{{", "{").replace("}}", "}")
             expanded += expand_parentheses(l.lower())
         samples = list(set(expanded))
 
         self.padacioso.add_intent(intent_name, samples)
         self.intent_samples[intent_name] = samples
 
     def detach_intent(self, intent_name):
@@ -193,16 +194,29 @@
             if exact_intent["name"]:
                 if exact_intent["name"] in excluded_intents:
                     continue
                 # inject regex extracted entities
                 if self.padacioso.fuzz or exact_intent["conf"] >= 0.8:
                     ents.update(exact_intent["entities"])
                 exact_intents.append(IntentMatch(confidence=exact_intent["conf"],
-                                                                  intent_name=exact_intent["name"],
-                                                                  entities=exact_intent["entities"]))
+                                                 intent_name=exact_intent["name"],
+                                                 entities=exact_intent["entities"]))
+
+        for intent_name, samples in self.intent_samples:
+            if any(s == query for s in samples if "{" not in s):
+                # update confidence of previous match
+                for idx, i in enumerate(exact_intents):
+                    if i.intent_name == intent_name:
+                        exact_intents[idx].confidence = 1
+                        break
+                # add new exact match
+                else:
+                    exact_intents.append(IntentMatch(confidence=1.0,
+                                                     intent_name=intent_name,
+                                                     entities={}))
 
         ents = {k: v for k, v in ents.items() if k not in self.detached_entities}
 
         classified_intents = []
         leftover_prob = 0  # redistribute prob of excluded intents so predictions still sum up to 1
 
         classes = self.classifier.clf.classes_
@@ -418,8 +432,7 @@
     engine.exclude_keywords("name", ["laugh"])
     print(engine.calc_intent("make me laugh"))
     # IntentMatch(intent_name='joke', confidence=0.5125373111690074, entities={})
 
     engine.exclude_keywords("hello", ["laugh"])
     print(engine.calc_intent("make me laugh"))
     # IntentMatch(intent_name='joke', confidence=1.0, entities={})
-
```

## jurebes/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 1
 VERSION_BUILD = 1
-VERSION_ALPHA = 6
+VERSION_ALPHA = 7
 # END_VERSION_BLOCK
```

## Comparing `jurebes-0.1.1a6.dist-info/METADATA` & `jurebes-0.1.1a7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jurebes
-Version: 0.1.1a6
+Version: 0.1.1a7
 Summary: A intent parser from OpenVoiceOS
 Home-page: https://github.com/OpenVoiceOS/jurebes
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

