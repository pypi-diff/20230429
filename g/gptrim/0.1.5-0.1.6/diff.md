# Comparing `tmp/gptrim-0.1.5-py3-none-any.whl.zip` & `tmp/gptrim-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4097 bytes, number of entries: 7
+Zip file size: 4197 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx       25 b- defN 23-Apr-16 12:45 gptrim/__init__.py
--rw-rw-r--  2.0 unx     3918 b- defN 23-Apr-25 18:13 gptrim/gptrim.py
--rw-rw-r--  2.0 unx     1070 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1113 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      526 b- defN 23-Apr-25 18:16 gptrim-0.1.5.dist-info/RECORD
-7 files, 6751 bytes uncompressed, 3167 bytes compressed:  53.1%
+-rw-rw-r--  2.0 unx     4161 b- defN 23-Apr-29 09:43 gptrim/gptrim.py
+-rw-rw-r--  2.0 unx     1070 b- defN 23-Apr-29 09:48 gptrim-0.1.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1113 b- defN 23-Apr-29 09:48 gptrim-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-29 09:48 gptrim-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-29 09:48 gptrim-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      526 b- defN 23-Apr-29 09:48 gptrim-0.1.6.dist-info/RECORD
+7 files, 6994 bytes uncompressed, 3267 bytes compressed:  53.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: gptrim/__init__.py
 Comment: 
 
 Filename: gptrim/gptrim.py
 Comment: 
 
-Filename: gptrim-0.1.5.dist-info/LICENSE
+Filename: gptrim-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: gptrim-0.1.5.dist-info/METADATA
+Filename: gptrim-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: gptrim-0.1.5.dist-info/WHEEL
+Filename: gptrim-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: gptrim-0.1.5.dist-info/top_level.txt
+Filename: gptrim-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: gptrim-0.1.5.dist-info/RECORD
+Filename: gptrim-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gptrim/gptrim.py

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Optional
+from typing import Optional, List
 
 import nltk
 from nltk.corpus import stopwords
 from nltk.stem import PorterStemmer, SnowballStemmer, LancasterStemmer
 
 nltk.download('punkt')
 nltk.download('stopwords')
@@ -69,35 +69,36 @@
         'won',
         "wont",
         'wouldn',
         "wouldnt",
     ],
 }
 
+PUNCTUATION = [".", ",", "'", '"', "!", "?", ";", ":", "-"]
+
 
 def trim(
     text: str, stemmer: Optional[str] = None, language: str = "english", remove_spaces: bool = True,
         remove_stopwords: bool = True, remove_punctuation: bool = False) -> str:
 
     if language not in stopwords.fileids():
         raise ValueError("Unsupported language")
 
     accepted_stemmers = ("snowball", "porter", "lancaster")
     if stemmer and stemmer not in accepted_stemmers:
         raise ValueError("Stemmer must be one of", accepted_stemmers)
 
     # merge contractions
-    text = text.replace("'", "").replace("’", "")
-
-    # remove punctuation
-    if remove_punctuation:
-        text = re.sub(r'[.,\'\"?!;:-]', '', text)
+    text: str = text.replace("'", "").replace("’", "")
 
     # tokenize words, keep uppercase
-    tokenized = nltk.word_tokenize(text)
+    tokenized: List = nltk.word_tokenize(text)
+
+    if remove_punctuation:
+        tokenized = [word for word in tokenized if word not in PUNCTUATION]
 
     if remove_stopwords:
         nltk_stopwords = stopwords.words(language)
         words_to_exclude = set(
             nltk_stopwords + ARTICLES_PREPOSITIONS.get(language, [])
         ) - set(NEGATION_WORDS.get(language, []))
 
@@ -123,9 +124,13 @@
                 word = word.upper()
             case_restored.append(word)
 
         words = case_restored
 
     # remove spaces
     join_str = "" if remove_spaces else " "
-    trimmed = join_str.join(words)
+    trimmed: str = join_str.join(words).strip()
+    if not remove_punctuation:
+        # this is a hack to remove spaces before punctuation
+        trimmed = re.sub(r"\s([?.!,:;])", r"\1", trimmed)
+
     return trimmed
```

## Comparing `gptrim-0.1.5.dist-info/LICENSE` & `gptrim-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gptrim-0.1.5.dist-info/METADATA` & `gptrim-0.1.6.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptrim
-Version: 0.1.5
+Version: 0.1.6
 Summary: Reduce the size of GPT inputs by 40-60% without losing most of the information.
 Home-page: https://github.com/vlad-ds/gptrim
 Author: Vlad Gheorghe
 Author-email: vlad.datapro@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `gptrim-0.1.5.dist-info/RECORD` & `gptrim-0.1.6.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 gptrim/__init__.py,sha256=8d8ZbeGpOo7V90wSPxM_wifMOXP3fGDPhieQ0J6149k,25
-gptrim/gptrim.py,sha256=7AiKQUaCWP-83SktAPMkuMuE_wK9OCj1viK5NjBiffo,3918
-gptrim-0.1.5.dist-info/LICENSE,sha256=MO2vXFJOxLzaMfZTvHSikrZymSJQxaXCbRirzgC-fj4,1070
-gptrim-0.1.5.dist-info/METADATA,sha256=9CkB0y48Hr21vGO7TFZcDleHO1BOGXFSBZjFeQmgTHU,1113
-gptrim-0.1.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gptrim-0.1.5.dist-info/top_level.txt,sha256=WZGiLK6dSmNLdd8pOVjA0FowMoXuHJ_KmLfGTBk9aFU,7
-gptrim-0.1.5.dist-info/RECORD,,
+gptrim/gptrim.py,sha256=xxDwVdlPYZ8N_-ef3IBtDqWiHGLvAqu3u7kKOP6jBxk,4161
+gptrim-0.1.6.dist-info/LICENSE,sha256=MO2vXFJOxLzaMfZTvHSikrZymSJQxaXCbRirzgC-fj4,1070
+gptrim-0.1.6.dist-info/METADATA,sha256=7VWvqsnbIYCb7fz1w29fm5CtK5_TK6dvvINsDNRBydE,1113
+gptrim-0.1.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gptrim-0.1.6.dist-info/top_level.txt,sha256=WZGiLK6dSmNLdd8pOVjA0FowMoXuHJ_KmLfGTBk9aFU,7
+gptrim-0.1.6.dist-info/RECORD,,
```

