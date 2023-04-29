# Comparing `tmp/IMDbTraktSyncer-1.0.2.tar.gz` & `tmp/IMDbTraktSyncer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.0.2.tar", last modified: Sat Apr 29 05:46:29 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.0.3.tar", last modified: Sat Apr 29 21:55:10 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.0.2.tar` & `IMDbTraktSyncer-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 05:46:29.808764 IMDbTraktSyncer-1.0.2/
-drwxrwxrwx   0        0        0        0 2023-04-29 05:46:29.777805 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     6373 2023-04-29 05:37:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     2280 2023-04-29 02:08:16.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-04-28 23:59:44.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     3697 2023-04-29 02:12:00.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1802 2023-04-29 02:08:38.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     1782 2023-04-29 02:19:56.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-04-29 05:46:29.806269 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     4821 2023-04-29 05:46:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-04-29 05:46:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 05:46:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-04-29 05:46:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-04-29 05:46:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 05:46:29.000000 IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     4821 2023-04-29 05:46:29.807767 IMDbTraktSyncer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4233 2023-04-29 01:25:00.000000 IMDbTraktSyncer-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 05:46:29.808764 IMDbTraktSyncer-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-04-29 05:46:19.000000 IMDbTraktSyncer-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:55:10.241639 IMDbTraktSyncer-1.0.3/
+drwxrwxrwx   0        0        0        0 2023-04-29 21:55:10.221665 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     6673 2023-04-29 21:54:57.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 17:50:08.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     2280 2023-04-29 02:08:16.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-04-28 23:59:44.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     3697 2023-04-29 02:12:00.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1802 2023-04-29 02:08:38.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     1782 2023-04-29 02:19:56.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-04-29 21:55:10.239642 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5850 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-29 21:55:10.000000 IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5850 2023-04-29 21:55:10.241150 IMDbTraktSyncer-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5242 2023-04-29 21:54:18.000000 IMDbTraktSyncer-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-29 21:55:10.241639 IMDbTraktSyncer-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1280 2023-04-29 21:53:14.000000 IMDbTraktSyncer-1.0.3/setup.py
```

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import json
 import subprocess
 import requests
 import time
-from . import checkChromedriver
-from . import verifyCredentials
-from . import traktRatings
-from . import imdbRatings
+from IMDbTraktSyncer import checkChromedriver
+from IMDbTraktSyncer import verifyCredentials
+from IMDbTraktSyncer import traktRatings
+from IMDbTraktSyncer import imdbRatings
 from chromedriver_py import binary_path
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
@@ -72,14 +72,16 @@
     else:
         print("Signed in")
         
     print('Setting IMDB Ratings')
         
     trakt_ratings = traktRatings.trakt_ratings
     imdb_ratings = imdbRatings.imdb_ratings
+    trakt_ratings = [rating for rating in trakt_ratings if rating['ID'] is not None] #filter out items without imdb id
+    imdb_ratings = [rating for rating in imdb_ratings if rating['ID'] is not None] #filter out items without imdb id
     imdb_ratings_to_set = [rating for rating in trakt_ratings if rating['ID'] not in [imdb_rating['ID'] for imdb_rating in imdb_ratings]]
     trakt_ratings_to_set = [rating for rating in imdb_ratings if rating['ID'] not in [trakt_rating['ID'] for trakt_rating in trakt_ratings]]
 
     # loop through each movie and TV show rating and submit rating on IMDb website
     for item in imdb_ratings_to_set:
         print(f'{item["Title"]} ({item["Year"]}): {item["Rating"]}/10 (IMDb ID: {item["ID"]})')
         driver.get(f'https://www.imdb.com/title/{item["ID"]}/')
@@ -123,26 +125,26 @@
                 "shows": [{
                     "ids": {
                         "imdb": item["ID"]
                     },
                     "rating": item["Rating"]
                 }]
             }
-            print(f"Rating TV show {item['Title']} ({item['Year']}) with rating {item['Rating']} on Trakt")
+            print(f"Rating TV show {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
         else:
             # This is a movie
             data = {
                 "movies": [{
                     "ids": {
                         "imdb": item["ID"]
                     },
                     "rating": item["Rating"]
                 }]
             }
-            print(f"Rating movie {item['Title']} ({item['Year']}) with rating {item['Rating']} on Trakt")
+            print(f"Rating movie {item['Title']} ({item['Year']}) with rating {item['Rating']}/10 on Trakt")
 
         # Make the API call to rate the item
         response = requests.post(rate_url, headers=headers, json=data)
         time.sleep(1)
         while response.status_code == 429:
             print("Rate limit exceeded. Waiting for 1 second...")
             time.sleep(1)
```

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.2/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-Metadata-Version: 2.1
-Name: IMDbTraktSyncer
-Version: 1.0.2
-Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
-Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
-Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
-2. Run `python -m pip install IMDbTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Run:
-`IMDbTraktSyncer` in command line.
-
-## Update:
-`python -m pip install IMDbTraktSyncer --upgrade` in command line.
-
-## Uninstall:
-`python -m pip uninstall IMDbTraktSyncer` in command line.
-
-## Alternative manual install method:
-1. Download the latest .zip from the releases page and move it to the file directory of your choice.
-2. Run the IMDbTraktSyncer.py. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Troubleshooting, known issues, workarounds & future outlook:
-* IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
-* If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace VERSION_NUMBER wuth the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
-* Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconvential method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
-* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
+# IMDb-Trakt-Syncer
+This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
+## Install Instructions:
+1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
+2. Run `python -m pip install IMDbTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
+4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+
+## Run:
+`IMDbTraktSyncer` in command line.
+
+## Update:
+`python -m pip install IMDbTraktSyncer --upgrade` in command line.
+
+## Uninstall:
+`python -m pip uninstall IMDbTraktSyncer` in command line.
+
+## Alternative manual install method:
+1. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and move it to the file directory of your choice.
+2. Open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+
+## Troubleshooting, known issues, workarounds & future outlook:
+* IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
+* If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
+* Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
+* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/uydTDcg.png)
+
+
+## Sponsorships, Donations and Custom Projects:
+Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More donation options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also posted on:
+* [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/imdb_trakt_rating_syncer_tool_sync_both_ways/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `IMDbTraktSyncer-1.0.2/LICENSE` & `IMDbTraktSyncer-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.2/PKG-INFO` & `IMDbTraktSyncer-1.0.3/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.2
+Version: 1.0.3
 Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -27,16 +27,36 @@
 ## Update:
 `python -m pip install IMDbTraktSyncer --upgrade` in command line.
 
 ## Uninstall:
 `python -m pip uninstall IMDbTraktSyncer` in command line.
 
 ## Alternative manual install method:
-1. Download the latest .zip from the releases page and move it to the file directory of your choice.
-2. Run the IMDbTraktSyncer.py. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+1. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and move it to the file directory of your choice.
+2. Open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
 
 ## Troubleshooting, known issues, workarounds & future outlook:
 * IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
-* If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace VERSION_NUMBER wuth the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
-* Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconvential method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
+* If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
+* Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
 * If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/uydTDcg.png)
+
+
+## Sponsorships, Donations and Custom Projects:
+Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More donation options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also posted on:
+* [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/imdb_trakt_rating_syncer_tool_sync_both_ways/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `IMDbTraktSyncer-1.0.2/README.md` & `IMDbTraktSyncer-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,62 @@
-# IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
-## Install Instructions:
-1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
-2. Run `python -m pip install IMDbTraktSyncer` in command line.
-3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
-4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Run:
-`IMDbTraktSyncer` in command line.
-
-## Update:
-`python -m pip install IMDbTraktSyncer --upgrade` in command line.
-
-## Uninstall:
-`python -m pip uninstall IMDbTraktSyncer` in command line.
-
-## Alternative manual install method:
-1. Download the latest .zip from the releases page and move it to the file directory of your choice.
-2. Run the IMDbTraktSyncer.py. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
-3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
-
-## Troubleshooting, known issues, workarounds & future outlook:
-* IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
-* If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace VERSION_NUMBER wuth the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
-* Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconvential method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
-* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
+Metadata-Version: 2.1
+Name: IMDbTraktSyncer
+Version: 1.0.3
+Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
+Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
+Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# IMDb-Trakt-Syncer
+This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python is supported.
+## Install Instructions:
+1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
+2. Run `python -m pip install IMDbTraktSyncer` in command line.
+3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
+4. Run the script by calling `IMDbTraktSyncer` in command line. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+5. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+
+## Run:
+`IMDbTraktSyncer` in command line.
+
+## Update:
+`python -m pip install IMDbTraktSyncer --upgrade` in command line.
+
+## Uninstall:
+`python -m pip uninstall IMDbTraktSyncer` in command line.
+
+## Alternative manual install method:
+1. Download the latest .zip from the [releases page](https://github.com/RileyXX/IMDb-Trakt-Syncer/releases) and move it to the file directory of your choice.
+2. Open terminal and navigate to folder where `IMDbTraktSyncer.py` is located. Run `IMDbTraktSyncer.py` in terminal. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
+3. Done. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
+
+## Troubleshooting, known issues, workarounds & future outlook:
+* IMDb may require a captcha on login. If you see "Not signed in" appear in the script then the script will fail and the captcha is likely to be the cause. To fix this, navigate to IMDb website in your browser, preferably Chrome and from the same computer. If logged in, logout, and log back in. It may ask you to fill in a captch, complete it and finish logging in. After logging in succesfully on your browser run the script again and it should work. You may need to repeat this step once or twice if it still gives you issues. I'm looking into adding a captcha solver into the script to solve this problem, but it is currently not implemented. 
+* If you see an error about having the incorrect version of Chrome driver. Uninstall it by running `python -m pip uninstall chromedriver-py` in command line. In your Chrome browser navigate to Settings > About Chrome and check your version (112... or 111 etc). This would indicate you are on Chrome version 112. Navigate to [chromedriver-py releases page](https://pypi.org/project/chromedriver-py/#history) and find the latest version that is the same Chrome version (112) already on your machine. Copy the version number you need. Then in command line run `python -m pip install chromedriver-py==VERSION_NUMBER`. Replace `VERSION_NUMBER` with the version you copied and press enter. This will install the correct chromedriver version. Run the script again and it should work.
+* Due to IMDb's lack of API and lack of rating import ability, this script uses a rather unconventional method that mimics using a web browser to set ratings on IMDB. So there are many points of failure that could arise. I will try my best to keep the script updated as best possible.
+* If any of your details change, passwords, logins, api keys etc, just delete credentials.txt and that will reset the script. It will prompt you to enter your new details on next run.
+
+## Screenshot:
+![Demo](https://i.imgur.com/uydTDcg.png)
+
+
+## Sponsorships, Donations and Custom Projects:
+Like my scripts? Become a [sponsor](https://github.com/sponsors/RileyXX) and support my projects! See below for other donation options. Need help with a project? Open an issue and I will try my best to help! For other inquiries and custom projects contact me on [Twitter](https://twitter.com/RileyxBell).
+
+#### More donation options:
+- Cashapp: `$rileyxx`
+- Venmo: `@rileyxx`
+- Bitcoin: `bc1qrjevwqv49z8y77len3azqfghxrjmrjvhy5zqau`
+- Amazon Wishlist: [Link ↗](https://www.amazon.com/hz/wishlist/ls/WURF5NWZ843U)
+
+## Also posted on:
+* [Reddit](https://www.reddit.com/r/trakt/comments/132heo0/imdb_trakt_rating_syncer_tool_sync_both_ways/)
+
+<br>
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `IMDbTraktSyncer-1.0.2/setup.py` & `IMDbTraktSyncer-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

