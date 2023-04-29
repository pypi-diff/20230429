# Comparing `tmp/denmune-0.1.11.tar.gz` & `tmp/denmune-1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denmune-0.1.11.tar", last modified: Sat Dec 31 19:10:10 2022, max compression
+gzip compressed data, was "denmune-1.12.tar", last modified: Sat Apr 29 21:47:58 2023, max compression
```

## Comparing `denmune-0.1.11.tar` & `denmune-1.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-12-31 19:10:10.983901 denmune-0.1.11/
--rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-0.1.11/LICENSE
--rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-0.1.11/MANIFEST.in
--rw-rw-rw-   0        0        0    32267 2022-12-31 19:10:10.983901 denmune-0.1.11/PKG-INFO
--rw-rw-rw-   0        0        0    31594 2022-12-31 19:05:39.000000 denmune-0.1.11/README.md
--rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-0.1.11/pyproject.toml
--rw-rw-rw-   0        0        0      810 2022-12-31 19:10:10.991908 denmune-0.1.11/setup.cfg
--rw-rw-rw-   0        0        0      259 2022-11-11 20:43:51.000000 denmune-0.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-31 19:10:10.842208 denmune-0.1.11/src/
-drwxrwxrwx   0        0        0        0 2022-12-31 19:10:10.935269 denmune-0.1.11/src/denmune/
--rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-0.1.11/src/denmune/__init__.py
--rw-rw-rw-   0        0        0    39275 2022-05-12 03:42:03.000000 denmune-0.1.11/src/denmune/denmune.py
-drwxrwxrwx   0        0        0        0 2022-12-31 19:10:10.983901 denmune-0.1.11/src/denmune.egg-info/
--rw-rw-rw-   0        0        0    32267 2022-12-31 19:10:10.000000 denmune-0.1.11/src/denmune.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2022-12-31 19:10:10.000000 denmune-0.1.11/src/denmune.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-31 19:10:10.000000 denmune-0.1.11/src/denmune.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2022-12-31 19:10:10.000000 denmune-0.1.11/src/denmune.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-12-31 19:10:10.000000 denmune-0.1.11/src/denmune.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.755907 denmune-1.12/
+-rw-rw-rw-   0        0        0     1498 2021-12-31 23:30:13.000000 denmune-1.12/LICENSE
+-rw-rw-rw-   0        0        0       47 2021-12-27 21:52:58.000000 denmune-1.12/MANIFEST.in
+-rw-rw-rw-   0        0        0    31198 2023-04-29 21:47:58.756901 denmune-1.12/PKG-INFO
+-rw-rw-rw-   0        0        0    30529 2023-04-29 21:17:35.000000 denmune-1.12/README.md
+-rw-rw-rw-   0        0        0      108 2021-12-23 20:19:35.000000 denmune-1.12/pyproject.toml
+-rw-rw-rw-   0        0        0      808 2023-04-29 21:47:58.763965 denmune-1.12/setup.cfg
+-rw-rw-rw-   0        0        0      259 2023-04-29 21:18:51.000000 denmune-1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.698902 denmune-1.12/src/
+drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.734903 denmune-1.12/src/denmune/
+-rw-rw-rw-   0        0        0       28 2022-05-12 02:48:25.000000 denmune-1.12/src/denmune/__init__.py
+-rw-rw-rw-   0        0        0    39275 2022-05-12 03:42:03.000000 denmune-1.12/src/denmune/denmune.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:47:58.752905 denmune-1.12/src/denmune.egg-info/
+-rw-rw-rw-   0        0        0    31198 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      125 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-29 21:47:58.000000 denmune-1.12/src/denmune.egg-info/top_level.txt
```

### Comparing `denmune-0.1.11/LICENSE` & `denmune-1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `denmune-0.1.11/PKG-INFO` & `denmune-1.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,109 @@
 Metadata-Version: 2.1
 Name: denmune
-Version: 0.1.11
+Version: 1.12
 Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
 Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
 Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
 Author-email: mohamed.alyabbas@outlook.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # DenMune: A density-peak clustering algorithm
+DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
-  DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
 
-  Scientific Work
-  ---------------------
+Collaborative Test Drive (New)
+------------------------------
+
+Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using my capsule on CodeOcean, your collaborative test drive.
+
+https://codeocean.com/capsule/3560333/tree/v1
+
 
-| Paper                                                        | Journal                                                      | Data                                                         |
-| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) |
 
-  Coding, Security & Maintenance
-  -----------------------
 
-| Git Repo                                                     | Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning |
-| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |-------------------|
-| [![GitHub commit activity](https://img.shields.io/github/commit-activity/y/egy1st/denmune-clustering-algorithm)](https://github.com/egy1st/denmune-clustering-algorithm) | ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml)|
+Scientific Work
+---------------------
 
-  Docs & Tutorials
-  ----------------------------
+| Paper                                                        | Journal                                                      | Data                                                         | ResearchGate stats                                           |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
 
-| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       | ReviewNB                                                     |
+Coding, Security & Maintenance
+-----------------------
+
+| Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning                                                |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) | [![Review NB](https://img.shields.io/badge/review-on%20reviewNB-blueviolet)](https://app.reviewnb.com/egy1st/denmune-clustering-algorithm/) |
+| ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml) |
 
-  Downloads Stats
-  --------------------
+Docs & Tutorials
+----------------------------
 
-| download/day                                               | download/week                                               | download/month     | Total downloads                                         |
-| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |------------------------------|
-| ![PyPI - Downloads](https://img.shields.io/pypi/dd/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune)
+| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
 
-  Suggestions & Reporting Issues
-  -------------------------------
+Downloads Stats
+--------------------
 
-| Github                                                       | Gitter                                                       | Slack                                                        |
+| download/week                                                | download/month                                               | Total downloads                                              |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![GitHub Discussions](https://img.shields.io/github/discussions/egy1st/denmune-clustering-algorithm)](https://github.com/egy1st/denmune-clustering-algorithm/discussions) | [![Gitter](https://badges.gitter.im/EG1ST/community.svg)](https://gitter.im/EG1ST/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) | [![Slack](https://img.shields.io/badge/chat-on%20slack-orange)](https://app.slack.com/client/T032DJEC8AW/C0326UK1VFY) |
+| [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) |
 
-  Based on the paper
-  -------------------
+Based on the paper
+-------------------
 
-  |Paper|
-  |-------------------------------------------------------------------------------------------
-  |Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
-  |*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
-  |In: Journal of Pattern Recognition, Elsevier,                                                                 
-  |volume 109, number 107589, January 2021                                                                      
-  |DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
+|Paper|
+|-------------------------------------------------------------------------------------------
+|Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
+|*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
+|In: Journal of Pattern Recognition, Elsevier,                                                                 
+|volume 109, number 107589, January 2021                                                                      
+|DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
 
-  Documentation:
-  ---------------
+Documentation:
+---------------
 
- Documentation, including tutorials, are available on:
-   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
+Documentation, including tutorials, are available on:
    -  [![read the docs](https://img.shields.io/badge/read_the-docs-orange)](https://denmune.readthedocs.io/en/latest/?badge=latest)
+   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
 
 
-  Watch it in action
-  -------------------
+Watch it in action
+-------------------
 
-  This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
+This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-  
 
-  When less means more
-  --------------------
 
-  Most calssic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
+When less means more
+--------------------
+
+Most classic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
   Recently, a density-based algorithm named DenMune showed great ability in detecting complex shapes even in noisy data. it can detect number of clusters automatically, detect both pre-identified-noise and post-identified-noise automatically and removing them.
 
   It can achieve accuracy reach 100% in some classic pattern problems, achieve 97% in MNIST dataset. A great advantage of this algorithm is being single-parameter algorithm. All you need is to set number of k-nearest neighbor and the algorithm will care about the rest. Being Non-sensitive to changes in k, make it robust and stable.
 
   Keep in mind, the algorithm reduce any N-D dataset to only 2-D dataset initially, so it is a good benefit of this algorithm is being always to plot your data and explore it which make this algorithm a good candidate for data exploration. Finally, the algorithm comes with neat package for visualizing data, validating it and analyze the whole clustering process.
 
-  How to install DenMune
-  ------------------------
+How to install DenMune
+------------------------
 
-  Simply install DenMune clustering algorithm using pip command from the official Python repository
+Simply install DenMune clustering algorithm using pip command from the official Python repository
 
   [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/)
 
   From the shell run the command
 
   ```shell
 pip install denmune
@@ -108,38 +111,42 @@
 
   From Jupyter notebook cell run the command
 
   ```ipython3
 !pip install denmune
   ```
 
-  How to use  DenMune
-  --------------------
 
-  Once DenMune is installed, you just need to import it 
+
+How to use  DenMune
+--------------------
+
+Once DenMune is installed, you just need to import it 
 
   ```python
 from denmune import DenMune
   ```
 
   ###### Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case.
 
 
-  Read data
-  -----------
 
-  There are four possible cases of data:
+
+Read data
+-----------
+
+There are four possible cases of data:
 
   - only train data without labels
   - only labeled train data
   - labeled train data in addition to test data without labels
   - labeled train data in addition to labeled test data
 
 
-  ```python
+```python
 #=============================================
 # First scenario: train data without labels 
 # ============================================
 
 data_path = 'datasets/denmune/chameleon/'  
 dataset = "t7.10k.csv" 
 data_file = data_path + dataset 
@@ -148,21 +155,21 @@
 X_train = pd.read_csv(data_file, sep=',', header=None)
 
 knn = 39 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=False, show_noise=True)
 
-  ```
+```
 
   This is an intuitive dataset which has no groundtruth provided
 
   ![t710](https://raw.githubusercontent.com/egy1st/images/main/clustering/t710.png)
 
-  ```python
+```python
 #=============================================
 # Second scenario: train data with labels 
 # ============================================
 
 data_path = 'datasets/denmune/shapes/'  
 dataset = "aggregation.csv"
 data_file = data_path + dataset 
@@ -172,26 +179,26 @@
 y_train = X_train.iloc[:, -1]
 X_train = X_train.drop(X_train.columns[-1], axis=1)  
 
 knn = 6 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, train_truth= y_train, k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=False, show_noise=True)
-  ```
+```
 
-  Datset groundtruth
+Datset groundtruth
 
   ![aggregation groundtruth](https://raw.githubusercontent.com/egy1st/images/main/clustering/aggregation_ground.png)
 
-  Dataset as detected by DenMune at k=6
+Dataset as detected by DenMune at k=6
 
   ![aggregation train](https://raw.githubusercontent.com/egy1st/images/main/clustering/aggregation_6.png)
 
 
-  ```python
+```python
 #=================================================================
 # Third scenario: train data with labels in addition to test data
 # ================================================================
 
 data_path = 'datasets/denmune/pendigits/'  
 file_2d = data_path + 'pendigits-2d.csv'
 
@@ -206,32 +213,32 @@
 
 knn = 50 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, train_truth= y_train,
              test_data= X_test, 
              k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=True, show_noise=True)
-  ```
+```
 
-  dataset groundtruth
+dataset groundtruth
 
   ![pendigits groundtruth](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_ground.png)
 
 
-  dataset as detected by DenMune at k=50
+dataset as detected by DenMune at k=50
 
   ![pendigits train](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_50.png)
 
-  test data as predicted by DenMune on training the dataset at k=50
+test data as predicted by DenMune on training the dataset at k=50
 
   ![pendigits test](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_test_50.png)
 
 
-  Algorithm's Parameters
-  -----------------------
+Algorithm's Parameters
+-----------------------
 
     1. Parameters used within the initialization of the DenMune class
 
   ```python
 def __init__ (self,
                   train_data=None, test_data=None,
                   train_truth=None, test_truth=None, 
@@ -305,24 +312,26 @@
   - show_noise:
     - show/hide noise and outlier
     - default: True
 
   - show_analyzer:
     - show/hide the analyzer
     - default: True
+    
+    
 
-  The Analyzer
-  -------------
+The Analyzer
+-------------
 
-  The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
+The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
 
   ![DenMune Analyzer](https://raw.githubusercontent.com/egy1st/images/main/clustering/analyzer.png)
 
-  Noise Detection
-  ----------------
+Noise Detection
+----------------
 
   DenMune detects noise and outlier automatically, no need to any further work from your side.
 
   - It plots pre-identified noise in black
   - It plots post-identified noise in light grey
 
   You can set show_noise parameter to False.
@@ -343,16 +352,16 @@
   ```
 
 | noisy data                                                   | clean data                                                   |
 | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![noisy data](https://raw.githubusercontent.com/egy1st/images/main/clustering/noisy_data.png) | ![clean data](https://raw.githubusercontent.com/egy1st/images/main/clustering/clean_data.png) |
 
 
-  Validatation
-  --------------
+Validation
+--------------
 
   You can get your validation results using 3 methods
 
   - by showing the Analyzer
   - extract values from the validity returned list from fit_predict function
   - extract values from the Analyzer dictionary
     -
@@ -362,24 +371,24 @@
   - F1 score
   - NMI index (Normalized Mutual Information)
   - AMI index (Adjusted Mutual Information)
   - ARI index (Adjusted Rand Index)
 
   ![Validation snapshot](https://raw.githubusercontent.com/egy1st/images/main/clustering/validation.png) 
 
-  K-nearest Evolution
-  -------------------
+K-nearest Evolution
+-------------------
 
-  The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
+The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
 
   ![knn evolution chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/knn_vs_noise.png)
 
 
-  The Scalability
-  ----------------
+The Scalability
+----------------
 
 | data size          | time                   |
 | ------------------ | ---------------------- |
 | data  size: 5000   | time: 2.3139 seconds   |
 | data  size: 10000  | time: 5.8752 seconds   |
 | data  size: 15000  | time: 12.4535 seconds  |
 | data  size: 20000  | time: 18.8466 seconds  |
@@ -396,26 +405,27 @@
 | data  size: 75000  | time: 204.0712 seconds |
 | data  size: 80000  | time: 220.502 seconds  |
 | data  size: 85000  | time: 251.7625 seconds |
 | data  size: 100000 | time: 257.563 seconds  |
 
   | ![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
 
-  The Stability
-  --------------
+
+The Stability
+--------------
 
   The algorithm is only single-parameter, even more it not sensitive to changes in that parameter, k. You may guess that from the following chart yourself. This is of great benefit for you as a data exploration analyst. You can simply explore the dataset using an arbitrary k. Being Non-sensitive to changes in k, make it robust and stable.
 
   ![DenMune Stability chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/stability.png)
 
 
-  Reveal the propagation
-  -----------------------
+Reveal the propagation
+-----------------------
 
-  one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
+one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
 
   ```python
 dataset = "t7.10k" #
 data_path = 'datasets/denmune/chameleon/' 
 
 # train file
 data_file = data_path + dataset +'.csv'
@@ -436,36 +446,37 @@
     clear_output(wait=True)
     dm = DenMune(train_data=X_train, k_nearest=knn, rgn_tsne=False, prop_step=snapshot)
     labels, validity = dm.fit_predict(show_analyzer=False, show_noise=False)  
   ```
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-  Interact with the algorithm
-  ---------------------------
+Interact with the algorithm
+---------------------------
 
   [![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
 
   This notebook allows you interact with the algorithm in many aspects:
 
   - you can choose which dataset to cluster (among 4 chameleon datasets)
   - you can decide which number of k-nearest neighbor to use 
   - show noise on/off; thus you can invesetigate noise detected by the algorithm
   - show analyzer on/off
 
-  How to run and test
-  --------------------
+
+How to run and test
+--------------------
 
   1. Launch Examples in Repo2Docker Binder
 
      Simply use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
 
      [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD)
 
-  <a name="colab"></a>
+
 
   2. Launch each Example in Google Research, CoLab
          
      Need to test examples one by one, then here another option. Use colab offered by google research to test each example individually.
 
      Here is a list of Google CoLab URL to use the algorithm interactively
      ----------------------------------------------------------------------
@@ -484,15 +495,15 @@
 | Validation - colab                               | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/13_EVaQOv_QiNmQiMWJAcFFHPJHGCrQLe) |
 | How it propagates - colab                        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing) |
 | Snapshots of propagation - colab                 | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPXNKa8Rf3TnqDHSD3YSWl3g1iNSqjl2?usp=sharing) |
 | Scalability - colab                              | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1d55wkBndLLapO7Yx1ePHhE8mL61j9-TH?usp=sharing) |
 | Stability vs number of nearest neighbors - colab | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17VgVRMFBWvkSIH1yA3tMl6UQ7Eu68K2l?usp=sharing) |
 | k-nearest-evolution - colab                      | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1DZ-CQPV3WwJSiaV3-rjwPwmXw4RUh8Qj) |
 
-  <a name="kaggle"></a>  
+
 
   3. Launch each Example in Kaggle workspace
 
      If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
 
      | Dataset                                  | Kaggle URL                                                   |
@@ -509,18 +520,19 @@
      | The beauty of propagation part2 - kaggle | [![The beauty of propagation part 2 - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-propagation-part2) |
      | Snapshots of propagation -kaggle         | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/beauty-of-propagation-part3) |
      | Scalability kaggle                       | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/scalability-vs-speed) |
      | Stability - kaggle                       | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/stability-vs-number-of-nearest-neighbor) |
      | k-nearest-evolution - kaggle             | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/k-nearest-evolution) |
 
 
-  How to cite
-  =====
 
-  If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
+How to cite
+------------
+
+If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
       In: Journal of Pattern Recognition, Elsevier, volume 109, number 107589.
       January 2021
 
 
   ```bib
@@ -535,30 +547,34 @@
 url = {https://www.sciencedirect.com/science/article/pii/S0031320320303927},
 author = {Mohamed Abbas and Adel El-Zoghabi and Amin Shoukry},
 keywords = {Clustering, Mutual neighbors, Dimensionality reduction, Arbitrary shapes, Pattern recognition, Nearest neighbors, Density peak},
 abstract = {Many clustering algorithms fail when clusters are of arbitrary shapes, of varying densities, or the data classes are unbalanced and close to each other, even in two dimensions. A novel clustering algorithm “DenMune” is presented to meet this challenge. It is based on identifying dense regions using mutual nearest neighborhoods of size K, where K is the only parameter required from the user, besides obeying the mutual nearest neighbor consistency principle. The algorithm is stable for a wide range of values of K. Moreover, it is able to automatically detect and remove noise from the clustering process as well as detecting the target clusters. It produces robust results on various low and high dimensional datasets relative to several known state of the art clustering algorithms.}
 }
   ```
 
-  Licensing
-  ------------
 
-   The DenMune algorithm is 3-clause BSD licensed. Enjoy.
 
-   [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
+Licensing
+------------
+
+The DenMune algorithm is 3-clause BSD licensed. Enjoy.
+
+ [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
+
 
 
-  Task List
-  ------------
+Task List
+------------
 
-  - [x] Update Github with the DenMune sourcode
+  - [x] Update Github with the DenMune sourcecode
   - [x] create repo2docker repository
   - [x] Create pip Package
   - [x] create CoLab shared examples
   - [x] create documentation
   - [x] create Kaggle shared examples
   - [x] PEP8 compliant
   - [x] Continuous integration
   - [x] scikit-learn compatible
   - [x] creating unit tests (coverage: 100%)
   - [x] generating API documentation
+  - [x] create reproducible capsule on codeocean
   - [ ] create conda package
```

### Comparing `denmune-0.1.11/README.md` & `denmune-1.12/src/denmune.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,109 @@
+Metadata-Version: 2.1
+Name: denmune
+Version: 1.12
+Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
+Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
+Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
+Author-email: mohamed.alyabbas@outlook.com
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DenMune: A density-peak clustering algorithm
+DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
-  DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
 
-  Scientific Work
-  ---------------------
+Collaborative Test Drive (New)
+------------------------------
+
+Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using my capsule on CodeOcean, your collaborative test drive.
+
+https://codeocean.com/capsule/3560333/tree/v1
 
-| Paper                                                        | Journal                                                      | Data                                                         |
-| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) |
 
-  Coding, Security & Maintenance
-  -----------------------
 
-| Git Repo                                                     | Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning |
-| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |-------------------|
-| [![GitHub commit activity](https://img.shields.io/github/commit-activity/y/egy1st/denmune-clustering-algorithm)](https://github.com/egy1st/denmune-clustering-algorithm) | ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml)|
 
-  Docs & Tutorials
-  ----------------------------
+Scientific Work
+---------------------
 
-| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       | ReviewNB                                                     |
+| Paper                                                        | Journal                                                      | Data                                                         | ResearchGate stats                                           |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
+
+Coding, Security & Maintenance
+-----------------------
+
+| Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning                                                |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) | [![Review NB](https://img.shields.io/badge/review-on%20reviewNB-blueviolet)](https://app.reviewnb.com/egy1st/denmune-clustering-algorithm/) |
+| ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml) |
 
-  Downloads Stats
-  --------------------
+Docs & Tutorials
+----------------------------
 
-| download/day                                               | download/week                                               | download/month     | Total downloads                                         |
-| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |------------------------------|
-| ![PyPI - Downloads](https://img.shields.io/pypi/dd/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune)
+| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
 
-  Suggestions & Reporting Issues
-  -------------------------------
+Downloads Stats
+--------------------
 
-| Github                                                       | Gitter                                                       | Slack                                                        |
+| download/week                                                | download/month                                               | Total downloads                                              |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![GitHub Discussions](https://img.shields.io/github/discussions/egy1st/denmune-clustering-algorithm)](https://github.com/egy1st/denmune-clustering-algorithm/discussions) | [![Gitter](https://badges.gitter.im/EG1ST/community.svg)](https://gitter.im/EG1ST/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) | [![Slack](https://img.shields.io/badge/chat-on%20slack-orange)](https://app.slack.com/client/T032DJEC8AW/C0326UK1VFY) |
+| [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) |
 
-  Based on the paper
-  -------------------
+Based on the paper
+-------------------
 
-  |Paper|
-  |-------------------------------------------------------------------------------------------
-  |Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
-  |*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
-  |In: Journal of Pattern Recognition, Elsevier,                                                                 
-  |volume 109, number 107589, January 2021                                                                      
-  |DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
+|Paper|
+|-------------------------------------------------------------------------------------------
+|Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
+|*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
+|In: Journal of Pattern Recognition, Elsevier,                                                                 
+|volume 109, number 107589, January 2021                                                                      
+|DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
 
-  Documentation:
-  ---------------
+Documentation:
+---------------
 
- Documentation, including tutorials, are available on:
-   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
+Documentation, including tutorials, are available on:
    -  [![read the docs](https://img.shields.io/badge/read_the-docs-orange)](https://denmune.readthedocs.io/en/latest/?badge=latest)
+   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
 
 
-  Watch it in action
-  -------------------
+Watch it in action
+-------------------
 
-  This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
+This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-  
 
-  When less means more
-  --------------------
 
-  Most calssic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
+When less means more
+--------------------
+
+Most classic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
   Recently, a density-based algorithm named DenMune showed great ability in detecting complex shapes even in noisy data. it can detect number of clusters automatically, detect both pre-identified-noise and post-identified-noise automatically and removing them.
 
   It can achieve accuracy reach 100% in some classic pattern problems, achieve 97% in MNIST dataset. A great advantage of this algorithm is being single-parameter algorithm. All you need is to set number of k-nearest neighbor and the algorithm will care about the rest. Being Non-sensitive to changes in k, make it robust and stable.
 
   Keep in mind, the algorithm reduce any N-D dataset to only 2-D dataset initially, so it is a good benefit of this algorithm is being always to plot your data and explore it which make this algorithm a good candidate for data exploration. Finally, the algorithm comes with neat package for visualizing data, validating it and analyze the whole clustering process.
 
-  How to install DenMune
-  ------------------------
+How to install DenMune
+------------------------
 
-  Simply install DenMune clustering algorithm using pip command from the official Python repository
+Simply install DenMune clustering algorithm using pip command from the official Python repository
 
   [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/)
 
   From the shell run the command
 
   ```shell
 pip install denmune
@@ -93,38 +111,42 @@
 
   From Jupyter notebook cell run the command
 
   ```ipython3
 !pip install denmune
   ```
 
-  How to use  DenMune
-  --------------------
 
-  Once DenMune is installed, you just need to import it 
+
+How to use  DenMune
+--------------------
+
+Once DenMune is installed, you just need to import it 
 
   ```python
 from denmune import DenMune
   ```
 
   ###### Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case.
 
 
-  Read data
-  -----------
 
-  There are four possible cases of data:
+
+Read data
+-----------
+
+There are four possible cases of data:
 
   - only train data without labels
   - only labeled train data
   - labeled train data in addition to test data without labels
   - labeled train data in addition to labeled test data
 
 
-  ```python
+```python
 #=============================================
 # First scenario: train data without labels 
 # ============================================
 
 data_path = 'datasets/denmune/chameleon/'  
 dataset = "t7.10k.csv" 
 data_file = data_path + dataset 
@@ -133,21 +155,21 @@
 X_train = pd.read_csv(data_file, sep=',', header=None)
 
 knn = 39 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=False, show_noise=True)
 
-  ```
+```
 
   This is an intuitive dataset which has no groundtruth provided
 
   ![t710](https://raw.githubusercontent.com/egy1st/images/main/clustering/t710.png)
 
-  ```python
+```python
 #=============================================
 # Second scenario: train data with labels 
 # ============================================
 
 data_path = 'datasets/denmune/shapes/'  
 dataset = "aggregation.csv"
 data_file = data_path + dataset 
@@ -157,26 +179,26 @@
 y_train = X_train.iloc[:, -1]
 X_train = X_train.drop(X_train.columns[-1], axis=1)  
 
 knn = 6 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, train_truth= y_train, k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=False, show_noise=True)
-  ```
+```
 
-  Datset groundtruth
+Datset groundtruth
 
   ![aggregation groundtruth](https://raw.githubusercontent.com/egy1st/images/main/clustering/aggregation_ground.png)
 
-  Dataset as detected by DenMune at k=6
+Dataset as detected by DenMune at k=6
 
   ![aggregation train](https://raw.githubusercontent.com/egy1st/images/main/clustering/aggregation_6.png)
 
 
-  ```python
+```python
 #=================================================================
 # Third scenario: train data with labels in addition to test data
 # ================================================================
 
 data_path = 'datasets/denmune/pendigits/'  
 file_2d = data_path + 'pendigits-2d.csv'
 
@@ -191,32 +213,32 @@
 
 knn = 50 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, train_truth= y_train,
              test_data= X_test, 
              k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=True, show_noise=True)
-  ```
+```
 
-  dataset groundtruth
+dataset groundtruth
 
   ![pendigits groundtruth](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_ground.png)
 
 
-  dataset as detected by DenMune at k=50
+dataset as detected by DenMune at k=50
 
   ![pendigits train](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_50.png)
 
-  test data as predicted by DenMune on training the dataset at k=50
+test data as predicted by DenMune on training the dataset at k=50
 
   ![pendigits test](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_test_50.png)
 
 
-  Algorithm's Parameters
-  -----------------------
+Algorithm's Parameters
+-----------------------
 
     1. Parameters used within the initialization of the DenMune class
 
   ```python
 def __init__ (self,
                   train_data=None, test_data=None,
                   train_truth=None, test_truth=None, 
@@ -290,24 +312,26 @@
   - show_noise:
     - show/hide noise and outlier
     - default: True
 
   - show_analyzer:
     - show/hide the analyzer
     - default: True
+    
+    
 
-  The Analyzer
-  -------------
+The Analyzer
+-------------
 
-  The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
+The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
 
   ![DenMune Analyzer](https://raw.githubusercontent.com/egy1st/images/main/clustering/analyzer.png)
 
-  Noise Detection
-  ----------------
+Noise Detection
+----------------
 
   DenMune detects noise and outlier automatically, no need to any further work from your side.
 
   - It plots pre-identified noise in black
   - It plots post-identified noise in light grey
 
   You can set show_noise parameter to False.
@@ -328,16 +352,16 @@
   ```
 
 | noisy data                                                   | clean data                                                   |
 | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![noisy data](https://raw.githubusercontent.com/egy1st/images/main/clustering/noisy_data.png) | ![clean data](https://raw.githubusercontent.com/egy1st/images/main/clustering/clean_data.png) |
 
 
-  Validatation
-  --------------
+Validation
+--------------
 
   You can get your validation results using 3 methods
 
   - by showing the Analyzer
   - extract values from the validity returned list from fit_predict function
   - extract values from the Analyzer dictionary
     -
@@ -347,24 +371,24 @@
   - F1 score
   - NMI index (Normalized Mutual Information)
   - AMI index (Adjusted Mutual Information)
   - ARI index (Adjusted Rand Index)
 
   ![Validation snapshot](https://raw.githubusercontent.com/egy1st/images/main/clustering/validation.png) 
 
-  K-nearest Evolution
-  -------------------
+K-nearest Evolution
+-------------------
 
-  The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
+The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
 
   ![knn evolution chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/knn_vs_noise.png)
 
 
-  The Scalability
-  ----------------
+The Scalability
+----------------
 
 | data size          | time                   |
 | ------------------ | ---------------------- |
 | data  size: 5000   | time: 2.3139 seconds   |
 | data  size: 10000  | time: 5.8752 seconds   |
 | data  size: 15000  | time: 12.4535 seconds  |
 | data  size: 20000  | time: 18.8466 seconds  |
@@ -381,26 +405,27 @@
 | data  size: 75000  | time: 204.0712 seconds |
 | data  size: 80000  | time: 220.502 seconds  |
 | data  size: 85000  | time: 251.7625 seconds |
 | data  size: 100000 | time: 257.563 seconds  |
 
   | ![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
 
-  The Stability
-  --------------
+
+The Stability
+--------------
 
   The algorithm is only single-parameter, even more it not sensitive to changes in that parameter, k. You may guess that from the following chart yourself. This is of great benefit for you as a data exploration analyst. You can simply explore the dataset using an arbitrary k. Being Non-sensitive to changes in k, make it robust and stable.
 
   ![DenMune Stability chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/stability.png)
 
 
-  Reveal the propagation
-  -----------------------
+Reveal the propagation
+-----------------------
 
-  one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
+one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
 
   ```python
 dataset = "t7.10k" #
 data_path = 'datasets/denmune/chameleon/' 
 
 # train file
 data_file = data_path + dataset +'.csv'
@@ -421,36 +446,37 @@
     clear_output(wait=True)
     dm = DenMune(train_data=X_train, k_nearest=knn, rgn_tsne=False, prop_step=snapshot)
     labels, validity = dm.fit_predict(show_analyzer=False, show_noise=False)  
   ```
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-  Interact with the algorithm
-  ---------------------------
+Interact with the algorithm
+---------------------------
 
   [![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
 
   This notebook allows you interact with the algorithm in many aspects:
 
   - you can choose which dataset to cluster (among 4 chameleon datasets)
   - you can decide which number of k-nearest neighbor to use 
   - show noise on/off; thus you can invesetigate noise detected by the algorithm
   - show analyzer on/off
 
-  How to run and test
-  --------------------
+
+How to run and test
+--------------------
 
   1. Launch Examples in Repo2Docker Binder
 
      Simply use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
 
      [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD)
 
-  <a name="colab"></a>
+
 
   2. Launch each Example in Google Research, CoLab
          
      Need to test examples one by one, then here another option. Use colab offered by google research to test each example individually.
 
      Here is a list of Google CoLab URL to use the algorithm interactively
      ----------------------------------------------------------------------
@@ -469,15 +495,15 @@
 | Validation - colab                               | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/13_EVaQOv_QiNmQiMWJAcFFHPJHGCrQLe) |
 | How it propagates - colab                        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing) |
 | Snapshots of propagation - colab                 | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPXNKa8Rf3TnqDHSD3YSWl3g1iNSqjl2?usp=sharing) |
 | Scalability - colab                              | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1d55wkBndLLapO7Yx1ePHhE8mL61j9-TH?usp=sharing) |
 | Stability vs number of nearest neighbors - colab | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17VgVRMFBWvkSIH1yA3tMl6UQ7Eu68K2l?usp=sharing) |
 | k-nearest-evolution - colab                      | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1DZ-CQPV3WwJSiaV3-rjwPwmXw4RUh8Qj) |
 
-  <a name="kaggle"></a>  
+
 
   3. Launch each Example in Kaggle workspace
 
      If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
 
      | Dataset                                  | Kaggle URL                                                   |
@@ -494,18 +520,19 @@
      | The beauty of propagation part2 - kaggle | [![The beauty of propagation part 2 - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-propagation-part2) |
      | Snapshots of propagation -kaggle         | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/beauty-of-propagation-part3) |
      | Scalability kaggle                       | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/scalability-vs-speed) |
      | Stability - kaggle                       | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/stability-vs-number-of-nearest-neighbor) |
      | k-nearest-evolution - kaggle             | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/k-nearest-evolution) |
 
 
-  How to cite
-  =====
 
-  If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
+How to cite
+------------
+
+If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
       In: Journal of Pattern Recognition, Elsevier, volume 109, number 107589.
       January 2021
 
 
   ```bib
@@ -520,30 +547,34 @@
 url = {https://www.sciencedirect.com/science/article/pii/S0031320320303927},
 author = {Mohamed Abbas and Adel El-Zoghabi and Amin Shoukry},
 keywords = {Clustering, Mutual neighbors, Dimensionality reduction, Arbitrary shapes, Pattern recognition, Nearest neighbors, Density peak},
 abstract = {Many clustering algorithms fail when clusters are of arbitrary shapes, of varying densities, or the data classes are unbalanced and close to each other, even in two dimensions. A novel clustering algorithm “DenMune” is presented to meet this challenge. It is based on identifying dense regions using mutual nearest neighborhoods of size K, where K is the only parameter required from the user, besides obeying the mutual nearest neighbor consistency principle. The algorithm is stable for a wide range of values of K. Moreover, it is able to automatically detect and remove noise from the clustering process as well as detecting the target clusters. It produces robust results on various low and high dimensional datasets relative to several known state of the art clustering algorithms.}
 }
   ```
 
-  Licensing
-  ------------
 
-   The DenMune algorithm is 3-clause BSD licensed. Enjoy.
 
-   [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
+Licensing
+------------
+
+The DenMune algorithm is 3-clause BSD licensed. Enjoy.
+
+ [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
+
 
 
-  Task List
-  ------------
+Task List
+------------
 
-  - [x] Update Github with the DenMune sourcode
+  - [x] Update Github with the DenMune sourcecode
   - [x] create repo2docker repository
   - [x] Create pip Package
   - [x] create CoLab shared examples
   - [x] create documentation
   - [x] create Kaggle shared examples
   - [x] PEP8 compliant
   - [x] Continuous integration
   - [x] scikit-learn compatible
   - [x] creating unit tests (coverage: 100%)
   - [x] generating API documentation
-  - [ ] create conda package
+  - [x] create reproducible capsule on codeocean
+  - [ ] create conda package
```

### Comparing `denmune-0.1.11/setup.cfg` & `denmune-1.12/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 656e 6d75 6e65 0d0a 7665 7273   = denmune..vers
-00000020: 696f 6e20 3d20 302e 312e 3131 0d0a 6175  ion = 0.1.11..au
-00000030: 7468 6f72 203d 2044 722e 204d 6f68 616d  thor = Dr. Moham
-00000040: 6564 2041 6c69 2041 6262 6173 2026 2050  ed Ali Abbas & P
-00000050: 726f 662e 2041 6d69 6e20 2053 686f 756b  rof. Amin  Shouk
-00000060: 7279 0d0a 6175 7468 6f72 5f65 6d61 696c  ry..author_email
-00000070: 203d 206d 6f68 616d 6564 2e61 6c79 6162   = mohamed.alyab
-00000080: 6261 7340 6f75 746c 6f6f 6b2e 636f 6d0d  bas@outlook.com.
-00000090: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
-000000a0: 6869 7320 6973 2074 6865 2070 6163 6b61  his is the packa
-000000b0: 6765 2066 6f72 2044 656e 4d75 6e65 2043  ge for DenMune C
-000000c0: 6c75 7374 6572 696e 6720 416c 676f 7269  lustering Algori
-000000d0: 7468 6d20 7075 626c 6973 6865 6420 696e  thm published in
-000000e0: 2070 6170 6572 2068 7474 7073 3a2f 2f64   paper https://d
-000000f0: 6f69 2e6f 7267 2f31 302e 3130 3136 2f6a  oi.org/10.1016/j
-00000100: 2e70 6174 636f 672e 3230 3230 2e31 3037  .patcog.2020.107
-00000110: 3538 390d 0a6c 6f6e 675f 6465 7363 7269  589..long_descri
-00000120: 7074 696f 6e20 3d20 6669 6c65 3a20 5245  ption = file: RE
-00000130: 4144 4d45 2e6d 640d 0a6c 6f6e 675f 6465  ADME.md..long_de
-00000140: 7363 7269 7074 696f 6e5f 636f 6e74 656e  scription_conten
-00000150: 745f 7479 7065 203d 2074 6578 742f 6d61  t_type = text/ma
-00000160: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
-00000170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000180: 2f73 6369 6b69 742d 6c65 6172 6e2d 636f  /scikit-learn-co
-00000190: 6e74 7269 622f 6465 6e6d 756e 652d 636c  ntrib/denmune-cl
-000001a0: 7573 7465 7269 6e67 2d61 6c67 6f72 6974  ustering-algorit
-000001b0: 686d 0d0a 7072 6f6a 6563 745f 7572 6c73  hm..project_urls
-000001c0: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-000001d0: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-000001e0: 7562 2e63 6f6d 2f70 7970 612f 7361 6d70  ub.com/pypa/samp
-000001f0: 6c65 7072 6f6a 6563 742f 6973 7375 6573  leproject/issues
-00000200: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000210: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-00000220: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000230: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
-00000240: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
-00000250: 203a 3a20 4253 4420 4c69 6365 6e73 650d   :: BSD License.
-00000260: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
-00000270: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-00000280: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
-00000290: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-000002a0: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-000002b0: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000002c0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002d0: 3d33 2e36 0d0a 0d0a 5b6f 7074 696f 6e73  =3.6....[options
-000002e0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000002f0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-00000300: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-00000310: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000320: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000020: 696f 6e20 3d20 312e 3132 0d0a 6175 7468  ion = 1.12..auth
+00000030: 6f72 203d 2044 722e 204d 6f68 616d 6564  or = Dr. Mohamed
+00000040: 2041 6c69 2041 6262 6173 2026 2050 726f   Ali Abbas & Pro
+00000050: 662e 2041 6d69 6e20 2053 686f 756b 7279  f. Amin  Shoukry
+00000060: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000070: 206d 6f68 616d 6564 2e61 6c79 6162 6261   mohamed.alyabba
+00000080: 7340 6f75 746c 6f6f 6b2e 636f 6d0d 0a64  s@outlook.com..d
+00000090: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
+000000a0: 7320 6973 2074 6865 2070 6163 6b61 6765  s is the package
+000000b0: 2066 6f72 2044 656e 4d75 6e65 2043 6c75   for DenMune Clu
+000000c0: 7374 6572 696e 6720 416c 676f 7269 7468  stering Algorith
+000000d0: 6d20 7075 626c 6973 6865 6420 696e 2070  m published in p
+000000e0: 6170 6572 2068 7474 7073 3a2f 2f64 6f69  aper https://doi
+000000f0: 2e6f 7267 2f31 302e 3130 3136 2f6a 2e70  .org/10.1016/j.p
+00000100: 6174 636f 672e 3230 3230 2e31 3037 3538  atcog.2020.10758
+00000110: 390d 0a6c 6f6e 675f 6465 7363 7269 7074  9..long_descript
+00000120: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+00000130: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+00000140: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+00000150: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+00000160: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f73  s://github.com/s
+00000180: 6369 6b69 742d 6c65 6172 6e2d 636f 6e74  cikit-learn-cont
+00000190: 7269 622f 6465 6e6d 756e 652d 636c 7573  rib/denmune-clus
+000001a0: 7465 7269 6e67 2d61 6c67 6f72 6974 686d  tering-algorithm
+000001b0: 0d0a 7072 6f6a 6563 745f 7572 6c73 203d  ..project_urls =
+000001c0: 200d 0a09 4275 6720 5472 6163 6b65 7220   ...Bug Tracker 
+000001d0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+000001e0: 2e63 6f6d 2f70 7970 612f 7361 6d70 6c65  .com/pypa/sample
+000001f0: 7072 6f6a 6563 742f 6973 7375 6573 0d0a  project/issues..
+00000200: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+00000210: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000220: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000230: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
+00000240: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
+00000250: 3a20 4253 4420 4c69 6365 6e73 650d 0a09  : BSD License...
+00000260: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
+00000270: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
+00000280: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
+00000290: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+000002a0: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
+000002b0: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+000002c0: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+000002d0: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
+000002e0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000002f0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+00000300: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000310: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000320: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `denmune-0.1.11/src/denmune/denmune.py` & `denmune-1.12/src/denmune/denmune.py`

 * *Files identical despite different names*

### Comparing `denmune-0.1.11/src/denmune.egg-info/PKG-INFO` & `denmune-1.12/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,106 +1,94 @@
-Metadata-Version: 2.1
-Name: denmune
-Version: 0.1.11
-Summary: This is the package for DenMune Clustering Algorithm published in paper https://doi.org/10.1016/j.patcog.2020.107589
-Home-page: https://github.com/scikit-learn-contrib/denmune-clustering-algorithm
-Author: Dr. Mohamed Ali Abbas & Prof. Amin  Shoukry
-Author-email: mohamed.alyabbas@outlook.com
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DenMune: A density-peak clustering algorithm
+DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
-  DenMune is a clustering algorithm that can find clusters of arbitrary size, shapes and densities in two-dimensions. Higher dimensions are first reduced to 2-D using the t-sne. The algorithm relies on a single parameter K (the number of nearest neighbors). The results show the superiority of the algorithm. Enjoy the simplicity but the power of DenMune.
 
 
-  Scientific Work
-  ---------------------
+Collaborative Test Drive (New)
+------------------------------
+
+Now you can reproduce all the research experiments, and even share the results and collaborate to the algorithm using my capsule on CodeOcean, your collaborative test drive.
+
+https://codeocean.com/capsule/3560333/tree/v1
 
-| Paper                                                        | Journal                                                      | Data                                                         |
-| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) |
 
-  Coding, Security & Maintenance
-  -----------------------
 
-| Git Repo                                                     | Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning |
-| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |-------------------|
-| [![GitHub commit activity](https://img.shields.io/github/commit-activity/y/egy1st/denmune-clustering-algorithm)](https://github.com/egy1st/denmune-clustering-algorithm) | ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml)|
 
-  Docs & Tutorials
-  ----------------------------
+Scientific Work
+---------------------
 
-| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       | ReviewNB                                                     |
+| Paper                                                        | Journal                                                      | Data                                                         | ResearchGate stats                                           |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [![Elsevier, journal's article publisher ](https://img.shields.io/badge/elsevier-published-orange)](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927) | [![scimagojr](https://www.scimagojr.com/journal_img.php?id=24823)](https://www.scimagojr.com/journalsearch.php?q=24823&tip=sid&clean=0) | [![Research datasets at  Mendeley ](https://img.shields.io/badge/mendeley-data-bluegreen)](https://data.mendeley.com/datasets/b73cw5n43r/4) | ![Researchgate Stats](https://raw.githubusercontent.com/egy1st/images/main/clustering/researshgate.png) |
+
+Coding, Security & Maintenance
+-----------------------
+
+| Code Style                                                   | Installation                                                 | CI Workflow                                                  | Code Coverage                                                | Code Scanning                                                |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) | [![Review NB](https://img.shields.io/badge/review-on%20reviewNB-blueviolet)](https://app.reviewnb.com/egy1st/denmune-clustering-algorithm/) |
+| ![Code Style: Black](https://img.shields.io/badge/code%20style-black-black) | [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/) | [![CircleCI, continuous integration](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main.svg?style=shield)](https://circleci.com/gh/egy1st/denmune-clustering-algorithm/tree/main) | [![codecov](https://codecov.io/gh/egy1st/denmune-clustering-algorithm/branch/main/graph/badge.svg?token=QCbRdRtzYE)](https://codecov.io/gh/egy1st/denmune-clustering-algorithm) | [![CodeQL](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml/badge.svg)](https://github.com/adrinjalali/denmune-clustering-algorithm/actions/workflows/codeql.yml) |
 
-  Downloads Stats
-  --------------------
+Docs & Tutorials
+----------------------------
 
-| download/day                                               | download/week                                               | download/month     | Total downloads                                         |
-| ----------------------------------------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------- |------------------------------|
-| ![PyPI - Downloads](https://img.shields.io/pypi/dd/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune)
+| Read the Docs                                                | Repo2Docker                                                  | Colab                                                        | kaggle                                                       |
+| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
+| [![Documentation Status](https://readthedocs.org/projects/denmune/badge/?version=latest)](https://denmune.readthedocs.io/en/latest/?badge=latest) | [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD) | [![Launch notebook examples in Colaboratory, Google Research]( https://colab.research.google.com/assets/colab-badge.svg)](#colab) | [![Launch notebook examples in Kaggle, the workspace where data scientist meet](https://kaggle.com/static/images/open-in-kaggle.svg)](#kaggle) |
 
-  Suggestions & Reporting Issues
-  -------------------------------
+Downloads Stats
+--------------------
 
-| Github                                                       | Gitter                                                       | Slack                                                        |
+| download/week                                                | download/month                                               | Total downloads                                              |
 | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
-| [![GitHub Discussions](https://img.shields.io/github/discussions/egy1st/denmune-clustering-algorithm)](https://github.com/egy1st/denmune-clustering-algorithm/discussions) | [![Gitter](https://badges.gitter.im/EG1ST/community.svg)](https://gitter.im/EG1ST/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge) | [![Slack](https://img.shields.io/badge/chat-on%20slack-orange)](https://app.slack.com/client/T032DJEC8AW/C0326UK1VFY) |
+| [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=week&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=month&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) | [![Downloads](https://static.pepy.tech/personalized-badge/denmune?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/denmune) |
 
-  Based on the paper
-  -------------------
+Based on the paper
+-------------------
 
-  |Paper|
-  |-------------------------------------------------------------------------------------------
-  |Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
-  |*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
-  |In: Journal of Pattern Recognition, Elsevier,                                                                 
-  |volume 109, number 107589, January 2021                                                                      
-  |DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
+|Paper|
+|-------------------------------------------------------------------------------------------
+|Mohamed Abbas, Adel El-Zoghabi, Amin Shoukry,                                                                       
+|*DenMune: Density peak based clustering using mutual nearest neighbors*                                           
+|In: Journal of Pattern Recognition, Elsevier,                                                                 
+|volume 109, number 107589, January 2021                                                                      
+|DOI: https://doi.org/10.1016/j.patcog.2020.107589                                                 
 
-  Documentation:
-  ---------------
+Documentation:
+---------------
 
- Documentation, including tutorials, are available on:
-   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
+Documentation, including tutorials, are available on:
    -  [![read the docs](https://img.shields.io/badge/read_the-docs-orange)](https://denmune.readthedocs.io/en/latest/?badge=latest)
+   -  [https://docs.zerobytes.one/](https://docs.zerobytes.one)
 
 
-  Watch it in action
-  -------------------
+Watch it in action
+-------------------
 
-  This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
+This 30 seconds will tell you how a density-based algorithm, DenMune propagates:
 
   [![interact with the propagation](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing)
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-  
 
-  When less means more
-  --------------------
 
-  Most calssic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
+When less means more
+--------------------
+
+Most classic clustering algorithms fail in detecting complex clusters where clusters are of different size, shape, density, and being exist in noisy data.
   Recently, a density-based algorithm named DenMune showed great ability in detecting complex shapes even in noisy data. it can detect number of clusters automatically, detect both pre-identified-noise and post-identified-noise automatically and removing them.
 
   It can achieve accuracy reach 100% in some classic pattern problems, achieve 97% in MNIST dataset. A great advantage of this algorithm is being single-parameter algorithm. All you need is to set number of k-nearest neighbor and the algorithm will care about the rest. Being Non-sensitive to changes in k, make it robust and stable.
 
   Keep in mind, the algorithm reduce any N-D dataset to only 2-D dataset initially, so it is a good benefit of this algorithm is being always to plot your data and explore it which make this algorithm a good candidate for data exploration. Finally, the algorithm comes with neat package for visualizing data, validating it and analyze the whole clustering process.
 
-  How to install DenMune
-  ------------------------
+How to install DenMune
+------------------------
 
-  Simply install DenMune clustering algorithm using pip command from the official Python repository
+Simply install DenMune clustering algorithm using pip command from the official Python repository
 
   [![PyPI Version](https://img.shields.io/pypi/v/denmune.svg)]( https://pypi.org/project/denmune/)
 
   From the shell run the command
 
   ```shell
 pip install denmune
@@ -108,38 +96,42 @@
 
   From Jupyter notebook cell run the command
 
   ```ipython3
 !pip install denmune
   ```
 
-  How to use  DenMune
-  --------------------
 
-  Once DenMune is installed, you just need to import it 
+
+How to use  DenMune
+--------------------
+
+Once DenMune is installed, you just need to import it 
 
   ```python
 from denmune import DenMune
   ```
 
   ###### Please note that first denmune (the package) in small letters, while the other one(the class itself) has D and M in capital case.
 
 
-  Read data
-  -----------
 
-  There are four possible cases of data:
+
+Read data
+-----------
+
+There are four possible cases of data:
 
   - only train data without labels
   - only labeled train data
   - labeled train data in addition to test data without labels
   - labeled train data in addition to labeled test data
 
 
-  ```python
+```python
 #=============================================
 # First scenario: train data without labels 
 # ============================================
 
 data_path = 'datasets/denmune/chameleon/'  
 dataset = "t7.10k.csv" 
 data_file = data_path + dataset 
@@ -148,21 +140,21 @@
 X_train = pd.read_csv(data_file, sep=',', header=None)
 
 knn = 39 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=False, show_noise=True)
 
-  ```
+```
 
   This is an intuitive dataset which has no groundtruth provided
 
   ![t710](https://raw.githubusercontent.com/egy1st/images/main/clustering/t710.png)
 
-  ```python
+```python
 #=============================================
 # Second scenario: train data with labels 
 # ============================================
 
 data_path = 'datasets/denmune/shapes/'  
 dataset = "aggregation.csv"
 data_file = data_path + dataset 
@@ -172,26 +164,26 @@
 y_train = X_train.iloc[:, -1]
 X_train = X_train.drop(X_train.columns[-1], axis=1)  
 
 knn = 6 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, train_truth= y_train, k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=False, show_noise=True)
-  ```
+```
 
-  Datset groundtruth
+Datset groundtruth
 
   ![aggregation groundtruth](https://raw.githubusercontent.com/egy1st/images/main/clustering/aggregation_ground.png)
 
-  Dataset as detected by DenMune at k=6
+Dataset as detected by DenMune at k=6
 
   ![aggregation train](https://raw.githubusercontent.com/egy1st/images/main/clustering/aggregation_6.png)
 
 
-  ```python
+```python
 #=================================================================
 # Third scenario: train data with labels in addition to test data
 # ================================================================
 
 data_path = 'datasets/denmune/pendigits/'  
 file_2d = data_path + 'pendigits-2d.csv'
 
@@ -206,32 +198,32 @@
 
 knn = 50 # k-nearest neighbor, the only parameter required by the algorithm
 
 dm = DenMune(train_data=X_train, train_truth= y_train,
              test_data= X_test, 
              k_nearest=knn)
 labels, validity = dm.fit_predict(show_analyzer=True, show_noise=True)
-  ```
+```
 
-  dataset groundtruth
+dataset groundtruth
 
   ![pendigits groundtruth](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_ground.png)
 
 
-  dataset as detected by DenMune at k=50
+dataset as detected by DenMune at k=50
 
   ![pendigits train](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_50.png)
 
-  test data as predicted by DenMune on training the dataset at k=50
+test data as predicted by DenMune on training the dataset at k=50
 
   ![pendigits test](https://raw.githubusercontent.com/egy1st/images/main/clustering/pendigits_test_50.png)
 
 
-  Algorithm's Parameters
-  -----------------------
+Algorithm's Parameters
+-----------------------
 
     1. Parameters used within the initialization of the DenMune class
 
   ```python
 def __init__ (self,
                   train_data=None, test_data=None,
                   train_truth=None, test_truth=None, 
@@ -305,24 +297,26 @@
   - show_noise:
     - show/hide noise and outlier
     - default: True
 
   - show_analyzer:
     - show/hide the analyzer
     - default: True
+    
+    
 
-  The Analyzer
-  -------------
+The Analyzer
+-------------
 
-  The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
+The algorithm provide an exploratory tool called analyzer, once called it will provide you with in-depth analysis on how your clustering results perform.
 
   ![DenMune Analyzer](https://raw.githubusercontent.com/egy1st/images/main/clustering/analyzer.png)
 
-  Noise Detection
-  ----------------
+Noise Detection
+----------------
 
   DenMune detects noise and outlier automatically, no need to any further work from your side.
 
   - It plots pre-identified noise in black
   - It plots post-identified noise in light grey
 
   You can set show_noise parameter to False.
@@ -343,16 +337,16 @@
   ```
 
 | noisy data                                                   | clean data                                                   |
 | ------------------------------------------------------------ | ------------------------------------------------------------ |
 | ![noisy data](https://raw.githubusercontent.com/egy1st/images/main/clustering/noisy_data.png) | ![clean data](https://raw.githubusercontent.com/egy1st/images/main/clustering/clean_data.png) |
 
 
-  Validatation
-  --------------
+Validation
+--------------
 
   You can get your validation results using 3 methods
 
   - by showing the Analyzer
   - extract values from the validity returned list from fit_predict function
   - extract values from the Analyzer dictionary
     -
@@ -362,24 +356,24 @@
   - F1 score
   - NMI index (Normalized Mutual Information)
   - AMI index (Adjusted Mutual Information)
   - ARI index (Adjusted Rand Index)
 
   ![Validation snapshot](https://raw.githubusercontent.com/egy1st/images/main/clustering/validation.png) 
 
-  K-nearest Evolution
-  -------------------
+K-nearest Evolution
+-------------------
 
-  The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
+The following chart shows the evolution of pre and post identified noise in correspondence to increase of number of knn. Also, detected number of clusters is analyzed in the same chart in relation with both types of identified  noise.
 
   ![knn evolution chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/knn_vs_noise.png)
 
 
-  The Scalability
-  ----------------
+The Scalability
+----------------
 
 | data size          | time                   |
 | ------------------ | ---------------------- |
 | data  size: 5000   | time: 2.3139 seconds   |
 | data  size: 10000  | time: 5.8752 seconds   |
 | data  size: 15000  | time: 12.4535 seconds  |
 | data  size: 20000  | time: 18.8466 seconds  |
@@ -396,26 +390,27 @@
 | data  size: 75000  | time: 204.0712 seconds |
 | data  size: 80000  | time: 220.502 seconds  |
 | data  size: 85000  | time: 251.7625 seconds |
 | data  size: 100000 | time: 257.563 seconds  |
 
   | ![noisy data chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/scalability.png)
 
-  The Stability
-  --------------
+
+The Stability
+--------------
 
   The algorithm is only single-parameter, even more it not sensitive to changes in that parameter, k. You may guess that from the following chart yourself. This is of great benefit for you as a data exploration analyst. You can simply explore the dataset using an arbitrary k. Being Non-sensitive to changes in k, make it robust and stable.
 
   ![DenMune Stability chart](https://raw.githubusercontent.com/egy1st/images/main/clustering/stability.png)
 
 
-  Reveal the propagation
-  -----------------------
+Reveal the propagation
+-----------------------
 
-  one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
+one of the top performing feature in this algorithm is enabling you to watch how your clusters propagate to construct the final output clusters. just use the parameter 'prop_step' as in the following example:
 
   ```python
 dataset = "t7.10k" #
 data_path = 'datasets/denmune/chameleon/' 
 
 # train file
 data_file = data_path + dataset +'.csv'
@@ -436,36 +431,37 @@
     clear_output(wait=True)
     dm = DenMune(train_data=X_train, k_nearest=knn, rgn_tsne=False, prop_step=snapshot)
     labels, validity = dm.fit_predict(show_analyzer=False, show_noise=False)  
   ```
 
   [![Propagation in DenMune](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/propagation.gif)]()
 
-  Interact with the algorithm
-  ---------------------------
+Interact with the algorithm
+---------------------------
 
   [![chameleon datasets](https://raw.githubusercontent.com/egy1st/denmune-clustering-algorithm/main/images/chameleon_detection.png)](https://colab.research.google.com/drive/1EUROd6TRwxW3A_XD3KTxL8miL2ias4Ue?usp=sharing)
 
   This notebook allows you interact with the algorithm in many aspects:
 
   - you can choose which dataset to cluster (among 4 chameleon datasets)
   - you can decide which number of k-nearest neighbor to use 
   - show noise on/off; thus you can invesetigate noise detected by the algorithm
   - show analyzer on/off
 
-  How to run and test
-  --------------------
+
+How to run and test
+--------------------
 
   1. Launch Examples in Repo2Docker Binder
 
      Simply use our repo2docker offered by mybinder.org, which encapsulate the algorithm and all required data in one virtual machine instance. All Jupyter notebooks examples found in this repository will be also available to you in action to practice in this respo2docer. Thanks mybinder.org, you made it possible!
 
      [![Launch notebook examples in Binder](https://static.mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/egy1st/denmune-clustering-algorithm/HEAD)
 
-  <a name="colab"></a>
+
 
   2. Launch each Example in Google Research, CoLab
          
      Need to test examples one by one, then here another option. Use colab offered by google research to test each example individually.
 
      Here is a list of Google CoLab URL to use the algorithm interactively
      ----------------------------------------------------------------------
@@ -484,15 +480,15 @@
 | Validation - colab                               | [![Validation - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/13_EVaQOv_QiNmQiMWJAcFFHPJHGCrQLe) |
 | How it propagates - colab                        | [![How it propagates - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1o-tP3uvDGjxBOGYkir1lnbr74sZ06e0U?usp=sharing) |
 | Snapshots of propagation - colab                 | [![snapshots of the propagation - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1vPXNKa8Rf3TnqDHSD3YSWl3g1iNSqjl2?usp=sharing) |
 | Scalability - colab                              | [![Scalability - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1d55wkBndLLapO7Yx1ePHhE8mL61j9-TH?usp=sharing) |
 | Stability vs number of nearest neighbors - colab | [![Stability vs number of nearest neighbors - colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/17VgVRMFBWvkSIH1yA3tMl6UQ7Eu68K2l?usp=sharing) |
 | k-nearest-evolution - colab                      | [![k-nearest-evolution - colab](https://colab.research.google.com/assets/colab-badge.svg)]( https://colab.research.google.com/drive/1DZ-CQPV3WwJSiaV3-rjwPwmXw4RUh8Qj) |
 
-  <a name="kaggle"></a>  
+
 
   3. Launch each Example in Kaggle workspace
 
      If you are a kaggler like me, then Kaggle, the best workspace where data scientist meet, should fit you to test the algorithm with great experience. 
 
 
      | Dataset                                  | Kaggle URL                                                   |
@@ -509,18 +505,19 @@
      | The beauty of propagation part2 - kaggle | [![The beauty of propagation part 2 - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/the-beauty-of-propagation-part2) |
      | Snapshots of propagation -kaggle         | [![The beauty of propagation - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/beauty-of-propagation-part3) |
      | Scalability kaggle                       | [![Scalability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/scalability-vs-speed) |
      | Stability - kaggle                       | [![Stability - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/stability-vs-number-of-nearest-neighbor) |
      | k-nearest-evolution - kaggle             | [![k-nearest-evolution - kaggle](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/egyfirst/k-nearest-evolution) |
 
 
-  How to cite
-  =====
 
-  If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
+How to cite
+------------
+
+If you have used this codebase in a scientific publication and wish to cite it, please use the [Journal of Pattern Recognition article](https://www.sciencedirect.com/science/article/abs/pii/S0031320320303927)
 
       Mohamed Abbas McInnes, Adel El-Zoghaby, Amin Ahoukry, *DenMune: Density peak based clustering using mutual nearest neighbors*
       In: Journal of Pattern Recognition, Elsevier, volume 109, number 107589.
       January 2021
 
 
   ```bib
@@ -535,30 +532,34 @@
 url = {https://www.sciencedirect.com/science/article/pii/S0031320320303927},
 author = {Mohamed Abbas and Adel El-Zoghabi and Amin Shoukry},
 keywords = {Clustering, Mutual neighbors, Dimensionality reduction, Arbitrary shapes, Pattern recognition, Nearest neighbors, Density peak},
 abstract = {Many clustering algorithms fail when clusters are of arbitrary shapes, of varying densities, or the data classes are unbalanced and close to each other, even in two dimensions. A novel clustering algorithm “DenMune” is presented to meet this challenge. It is based on identifying dense regions using mutual nearest neighborhoods of size K, where K is the only parameter required from the user, besides obeying the mutual nearest neighbor consistency principle. The algorithm is stable for a wide range of values of K. Moreover, it is able to automatically detect and remove noise from the clustering process as well as detecting the target clusters. It produces robust results on various low and high dimensional datasets relative to several known state of the art clustering algorithms.}
 }
   ```
 
-  Licensing
-  ------------
 
-   The DenMune algorithm is 3-clause BSD licensed. Enjoy.
 
-   [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
+Licensing
+------------
+
+The DenMune algorithm is 3-clause BSD licensed. Enjoy.
+
+ [![BSD 3-Clause “New” or “Revised” License" ](https://img.shields.io/badge/license-BSD-green)](https://choosealicense.com/licenses/bsd-3-clause/)
+
 
 
-  Task List
-  ------------
+Task List
+------------
 
-  - [x] Update Github with the DenMune sourcode
+  - [x] Update Github with the DenMune sourcecode
   - [x] create repo2docker repository
   - [x] Create pip Package
   - [x] create CoLab shared examples
   - [x] create documentation
   - [x] create Kaggle shared examples
   - [x] PEP8 compliant
   - [x] Continuous integration
   - [x] scikit-learn compatible
   - [x] creating unit tests (coverage: 100%)
   - [x] generating API documentation
+  - [x] create reproducible capsule on codeocean
   - [ ] create conda package
```

