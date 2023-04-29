# Comparing `tmp/arabica-1.4.7.tar.gz` & `tmp/arabica-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.4.7.tar", last modified: Fri Apr 21 14:07:25 2023, max compression
+gzip compressed data, was "arabica-1.4.8.tar", last modified: Sat Apr 29 01:38:00 2023, max compression
```

## Comparing `arabica-1.4.7.tar` & `arabica-1.4.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 14:07:25.477142 arabica-1.4.7/
--rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.7/LICENSE
--rw-rw-rw-   0        0        0     7537 2023-04-21 14:07:25.477142 arabica-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 14:07:25.421147 arabica-1.4.7/arabica/
--rw-rw-rw-   0        0        0      105 2023-04-21 14:06:32.000000 arabica-1.4.7/arabica/__init__.py
--rw-rw-rw-   0        0        0    11740 2023-04-17 21:41:36.000000 arabica-1.4.7/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    29525 2023-04-20 22:52:23.000000 arabica-1.4.7/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.7/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.7/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.7/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.7/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.7/arabica/preprocess.py
--rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.7/arabica/sentiment.py
--rw-rw-rw-   0        0        0      449 2023-04-20 22:52:23.000000 arabica-1.4.7/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-04-21 14:07:25.469143 arabica-1.4.7/arabica.egg-info/
--rw-rw-rw-   0        0        0     7537 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-21 14:07:25.000000 arabica-1.4.7/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-04-21 14:06:32.000000 arabica-1.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 14:07:25.477142 arabica-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1058 2023-04-21 14:06:32.000000 arabica-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 01:38:00.702672 arabica-1.4.8/
+-rw-rw-rw-   0        0        0       12 2022-11-12 04:06:27.000000 arabica-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0     7537 2023-04-29 01:38:00.702672 arabica-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6766 2023-04-17 21:14:46.000000 arabica-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 01:38:00.687149 arabica-1.4.8/arabica/
+-rw-rw-rw-   0        0        0      105 2023-04-21 14:06:32.000000 arabica-1.4.8/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11414 2023-04-29 01:02:05.000000 arabica-1.4.8/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    29525 2023-04-20 22:52:23.000000 arabica-1.4.8/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.4.8/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.4.8/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     7419 2023-04-16 21:41:53.000000 arabica-1.4.8/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.4.8/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.4.8/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      270 2023-03-01 22:21:19.000000 arabica-1.4.8/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      768 2023-04-29 01:02:05.000000 arabica-1.4.8/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-04-29 01:38:00.702672 arabica-1.4.8/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7537 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 01:38:00.000000 arabica-1.4.8/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-04-29 01:36:53.000000 arabica-1.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 01:38:00.702672 arabica-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1058 2023-04-29 01:36:53.000000 arabica-1.4.8/setup.py
```

### Comparing `arabica-1.4.7/PKG-INFO` & `arabica-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.7/README.md` & `arabica-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `arabica-1.4.7/arabica/arabica_freq.py` & `arabica-1.4.8/arabica/arabica_freq.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import numpy as np
 import nltk
 from nltk.util import ngrams
 from nltk.util import bigrams as bi
 from nltk.util import trigrams as tri
 
 from .preprocess import *
-from .clean_numbers import remove_numbers
-from .stopwords import remove_stopwords
+from .clean_numbers import *
+from .stopwords import *
 from .group import grouper
 from .clean_ngram import *
 
 
 def arabica_freq(text: str,                 # Text
                  time: str,                 # Time
                  date_format: str,          # Date format: 'eur' - European, 'us' - American
@@ -100,102 +100,103 @@
         unigram_ungr['freq'] = unigram_ungr.iloc[:,[0]]
         unigram_ungr = unigram_ungr.sort_values(by='freq', ascending=False)
         unigram_ungr['unigram'] = unigram_ungr['word'].astype(str) + ": " + unigram_ungr['freq'].astype(str)
         unigram_ungr['unigram'] = unigram_ungr['unigram'].str.replace(',', '', regex = True)
         unigram_ungr = unigram_ungr['unigram']
         unigram_ungr = unigram_ungr.iloc[:max_words]
         unigram_ungr= unigram_ungr.astype(str)
-        unigram_ungr = unigram_ungr.str.replace('(', '', regex = True)
-        unigram_ungr = unigram_ungr.str.replace(')', '', regex = True)
-        unigram_ungr = unigram_ungr.str.replace("""'""", '', regex = True)
+        unigram_ungr = unigram_ungr.str.replace('''(''', '')
+        unigram_ungr = unigram_ungr.str.replace(''')''', '')
+        unigram_ungr = unigram_ungr.str.replace("""'""", '')
         unigram_ungr = unigram_ungr.str.split(n = 2, pat=':',expand=True)
         unigram_ungr['unigram_freq'] = unigram_ungr.iloc[:,[1]]
         unigram_ungr['unigram'] = unigram_ungr.iloc[:,[0]]
+        unigram_ungr['unigram'] = unigram_ungr['unigram'].astype("str")
         unigram_ungr = unigram_ungr[['unigram','unigram_freq']]
         unigram_ungr.reset_index(inplace = True)
 
         df['bigrams'] = df['bigrams'].astype(str)
-        df['bigrams']= df['bigrams'].str.replace(")"," ", regex = True)
-        df['bigrams']= df['bigrams'].str.replace("(",' ', regex = True)
-        df['bigrams']= df['bigrams'].str.replace("""', '""","+", regex = True)
-        df['bigrams']= df['bigrams'].str.replace("["," ", regex = True)
-        df['bigrams']= df['bigrams'].str.replace("]"," ", regex = True)
-        df['bigrams']= df['bigrams'].str.replace("'",'', regex = True)
-        df['bigrams']= df['bigrams'].str.replace(" ,  ",' ', regex = True)
-        df['bigrams']= df['bigrams'].str.replace("  ",'', regex = True)
+        df['bigrams']= df['bigrams'].str.replace(")"," ")
+        df['bigrams']= df['bigrams'].str.replace("(",' ')
+        df['bigrams']= df['bigrams'].str.replace("""', '""","+")
+        df['bigrams']= df['bigrams'].str.replace("["," ")
+        df['bigrams']= df['bigrams'].str.replace("]"," ")
+        df['bigrams']= df['bigrams'].str.replace("'",'')
+        df['bigrams']= df['bigrams'].str.replace(" ,  ",' ')
+        df['bigrams']= df['bigrams'].str.replace("  ",'')
         bigrams_str = ' '.join(df['bigrams'])
         tokens_ungr_bi= str(bigrams_str).split()
         bigram_frequency_ungr = nltk.ngrams(tokens_ungr_bi,1)
         bigram_ungr = nltk.FreqDist(bigram_frequency_ungr)
         bigram_ungr=pd.DataFrame.from_dict(bigram_ungr,orient='index')
         bigram_ungr['bigram'] = bigram_ungr.index
         bigram_ungr['bigram_freq'] = bigram_ungr.iloc[:,[0]]
         bigram_ungr = bigram_ungr.sort_values(by='bigram_freq', ascending=False)
         bigram_ungr['bigram'] = bigram_ungr['bigram'].astype(str) + ": " + bigram_ungr['bigram_freq'].astype(str)
         bigram_ungr['bigram'] = bigram_ungr['bigram'].str.replace(',', '', regex = True)
         bigram_ungr = bigram_ungr['bigram']
         bigram_ungr = bigram_ungr.iloc[:max_words]
         bigram_ungr= bigram_ungr.astype(str)
-        bigram_ungr = bigram_ungr.str.replace('(', '', regex = True)
-        bigram_ungr = bigram_ungr.str.replace(')', '', regex = True)
-        bigram_ungr = bigram_ungr.str.replace("""'""", '', regex = True)
+        bigram_ungr = bigram_ungr.str.replace('(', '')
+        bigram_ungr = bigram_ungr.str.replace(')', '')
+        bigram_ungr = bigram_ungr.str.replace("""'""", '')
         bigram_ungr = bigram_ungr.str.split(n = 2, pat=':',expand=True)
         bigram_ungr['bigram_freq'] = bigram_ungr.iloc[:,[1]]
         bigram_ungr['bigram'] = bigram_ungr.iloc[:,[0]]
-        bigram_ungr['bigram'] = bigram_ungr['bigram'].str.replace(' ', ', ', regex = True)
+        bigram_ungr['bigram'] = bigram_ungr['bigram'].str.replace(' ', ', ')
         bigram_ungr['bigram'] = bigram_ungr['bigram'].astype(str)
         bigram_ungr = bigram_ungr[['bigram','bigram_freq']]
         bigram_ungr.reset_index(inplace = True)
 
         bigram_ungr = pd.DataFrame(bigram_ungr)
-        bigram_col = bigram_ungr['bigram'].str.replace("+",",", regex = True)
+        bigram_col = bigram_ungr['bigram'].str.replace("+",",")
         bigram_freq = bigram_ungr['bigram_freq']
         bigram_ungr = pd.merge(bigram_col, bigram_freq, left_index=True, right_index=True)
 
         df['trigrams'] = df['trigrams'].astype(str)
-        df['trigrams']= df['trigrams'].str.replace(")"," ", regex = True)
-        df['trigrams']= df['trigrams'].str.replace("(",' ', regex = True)
-        df['trigrams']= df['trigrams'].str.replace("""', '""","+", regex = True)
-        df['trigrams']= df['trigrams'].str.replace("["," ", regex = True)
-        df['trigrams']= df['trigrams'].str.replace("]"," ", regex = True)
-        df['trigrams']= df['trigrams'].str.replace("'",'', regex = True)
-        df['trigrams']= df['trigrams'].str.replace(" ,  ",' ', regex = True)
-        df['trigrams']= df['trigrams'].str.replace("  ",'', regex = True)
+        df['trigrams']= df['trigrams'].str.replace(")"," ")
+        df['trigrams']= df['trigrams'].str.replace("(",' ')
+        df['trigrams']= df['trigrams'].str.replace("""', '""","+")
+        df['trigrams']= df['trigrams'].str.replace("["," ")
+        df['trigrams']= df['trigrams'].str.replace("]"," ")
+        df['trigrams']= df['trigrams'].str.replace("'",'')
+        df['trigrams']= df['trigrams'].str.replace(" ,  ",' ')
+        df['trigrams']= df['trigrams'].str.replace("  ",'')
         trigrams_str = ' '.join(df['trigrams'])
         tokens_ungr_tri= str(trigrams_str).split()
         trigrams_frequency_ungr = nltk.ngrams(tokens_ungr_tri,1)
         trigram_ungr = nltk.FreqDist(trigrams_frequency_ungr)
         trigram_ungr=pd.DataFrame.from_dict(trigram_ungr,orient='index')
         trigram_ungr['trigrams'] = trigram_ungr.index
         trigram_ungr['trigrams_freq'] = trigram_ungr.iloc[:,[0]]
         trigram_ungr = trigram_ungr.sort_values(by='trigrams_freq', ascending=False)
         trigram_ungr['trigrams'] = trigram_ungr['trigrams'].astype(str) + ": " + trigram_ungr['trigrams_freq'].astype(str)
         trigram_ungr['trigrams'] = trigram_ungr['trigrams'].str.replace(',', '')
         trigram_ungr = trigram_ungr['trigrams']
         trigram_ungr = trigram_ungr.iloc[:max_words]
         trigram_ungr= trigram_ungr.astype(str)
-        trigram_ungr = trigram_ungr.str.replace('(', '', regex = True)
-        trigram_ungr = trigram_ungr.str.replace(')', '', regex = True)
-        trigram_ungr = trigram_ungr.str.replace("""'""", '', regex = True)
+        trigram_ungr = trigram_ungr.str.replace('(', '')
+        trigram_ungr = trigram_ungr.str.replace(')', '')
+        trigram_ungr = trigram_ungr.str.replace("""'""", '')
         trigram_ungr = trigram_ungr.str.split(n = 2, pat=':',expand=True)
         trigram_ungr['trigram_freq'] = trigram_ungr.iloc[:,[1]]
         trigram_ungr['trigram'] = trigram_ungr.iloc[:,[0]]
-        trigram_ungr['trigram'] = trigram_ungr['trigram'].str.replace(' ', ', ', regex = True)
+        trigram_ungr['trigram'] = trigram_ungr['trigram'].str.replace(' ', ', ')
         trigram_ungr['trigram_freq'] = trigram_ungr['trigram_freq'].astype(str)
         trigram_ungr = trigram_ungr[['trigram','trigram_freq']]
         trigram_ungr.reset_index(inplace = True)
 
-        trigram_col = trigram_ungr['trigram'].str.replace("+",",", regex = True)
+        trigram_col = trigram_ungr['trigram'].str.replace("+",",")
         trigram_freq = trigram_ungr['trigram_freq']
         trigram_ungr = pd.merge(trigram_col, trigram_freq, left_index=True, right_index=True)
 
         freq_final = unigram_ungr.merge(bigram_ungr, how='left',left_index=True, right_index=True)
         freq_final = freq_final.merge(trigram_ungr, how='left',left_index=True, right_index=True)
         freq_final = freq_final[['unigram','unigram_freq','bigram','bigram_freq','trigram','trigram_freq']]
-        freq_final = pd.DataFrame(freq_final)
+        freq_final = pd.DataFrame(freq_final, index= None)
 
     else:
 
         df['unigrams'] = np.vectorize(token_cleaning)(df['unigrams'])
         df['bigrams'] = np.vectorize(token_cleaning)(df['bigrams'])
         df['trigrams'] = np.vectorize(token_cleaning)(df['trigrams'])
         unigrams_df = df['unigrams']
@@ -211,15 +212,15 @@
 
         freq_final = freq_final[['period_x','ngram_x','ngram_y','ngram']]
         freq_final.columns=['period','unigram','bigram','trigram']
 
         freq_final['unigram'] = np.vectorize(final_cleaning)(freq_final['unigram'])
         freq_final['bigram'] = np.vectorize(final_cleaning)(freq_final['bigram'])
         freq_final['trigram'] = np.vectorize(final_cleaning)(freq_final['trigram'])
-        freq_final = freq_final[freq_final['unigram']!=': 1']
+        freq_final = freq_final[freq_final['unigram']!=': 1'].astype('str')
         freq_final = freq_final[freq_final['bigram']!=': 1']
         freq_final = freq_final[freq_final['trigram']!=': 1']
 
         if time_freq == 'Y':
             freq_final['period'] = pd.to_datetime(freq_final['period'].astype('str'))
             freq_final['period'] = freq_final['period'].dt.strftime('%Y')
```

### Comparing `arabica-1.4.7/arabica/cappuccino.py` & `arabica-1.4.8/arabica/cappuccino.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.7/arabica/clean_ngram.py` & `arabica-1.4.8/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.7/arabica/coffee_break.py` & `arabica-1.4.8/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.7/arabica/group.py` & `arabica-1.4.8/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.7/arabica/preprocess.py` & `arabica-1.4.8/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.4.7/arabica.egg-info/PKG-INFO` & `arabica-1.4.8/arabica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.4.7
+Version: 1.4.8
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
         
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
```

### Comparing `arabica-1.4.7/pyproject.toml` & `arabica-1.4.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.4.7"
+version = "1.4.8"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.4.7/setup.py` & `arabica-1.4.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.4.7",
+        version="1.4.8",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
```

