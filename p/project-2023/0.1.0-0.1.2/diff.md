# Comparing `tmp/project_2023-0.1.0.tar.gz` & `tmp/project_2023-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_2023-0.1.0.tar", last modified: Thu Apr 20 20:06:07 2023, max compression
+gzip compressed data, was "project_2023-0.1.2.tar", last modified: Sat Apr 29 04:13:46 2023, max compression
```

## Comparing `project_2023-0.1.0.tar` & `project_2023-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.849229 project_2023-0.1.0/
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.833449 project_2023-0.1.0/.github/
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.834132 project_2023-0.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 keunwoo    (501) staff       (20)      834 2023-02-20 23:13:02.000000 project_2023-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 keunwoo    (501) staff       (20)      595 2023-02-20 23:13:02.000000 project_2023-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 keunwoo    (501) staff       (20)      118 2023-03-28 04:18:52.000000 project_2023-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.834447 project_2023-0.1.0/.github/workflows/
--rw-r--r--   0 keunwoo    (501) staff       (20)      676 2023-04-18 22:42:16.000000 project_2023-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0 keunwoo    (501) staff       (20)     1799 2023-02-20 23:13:02.000000 project_2023-0.1.0/.gitignore
--rw-r--r--   0 keunwoo    (501) staff       (20)     1887 2023-04-18 22:42:16.000000 project_2023-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 keunwoo    (501) staff       (20)    11357 2023-02-20 23:13:02.000000 project_2023-0.1.0/LICENSE
--rw-r--r--   0 keunwoo    (501) staff       (20)     2239 2023-04-18 22:42:16.000000 project_2023-0.1.0/Makefile
--rw-r--r--   0 keunwoo    (501) staff       (20)    15652 2023-04-20 20:06:07.848734 project_2023-0.1.0/PKG-INFO
--rw-r--r--   0 keunwoo    (501) staff       (20)     1876 2023-04-20 20:05:44.000000 project_2023-0.1.0/README.md
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.835491 project_2023-0.1.0/project_2023.egg-info/
--rw-r--r--   0 keunwoo    (501) staff       (20)    15652 2023-04-20 20:06:07.000000 project_2023-0.1.0/project_2023.egg-info/PKG-INFO
--rw-r--r--   0 keunwoo    (501) staff       (20)      684 2023-04-20 20:06:07.000000 project_2023-0.1.0/project_2023.egg-info/SOURCES.txt
--rw-r--r--   0 keunwoo    (501) staff       (20)        1 2023-04-20 20:06:07.000000 project_2023-0.1.0/project_2023.egg-info/dependency_links.txt
--rw-r--r--   0 keunwoo    (501) staff       (20)      156 2023-04-20 20:06:07.000000 project_2023-0.1.0/project_2023.egg-info/requires.txt
--rw-r--r--   0 keunwoo    (501) staff       (20)       17 2023-04-20 20:06:07.000000 project_2023-0.1.0/project_2023.egg-info/top_level.txt
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.847679 project_2023-0.1.0/project_progress/
--rw-r--r--   0 keunwoo    (501) staff       (20)      213 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/__init__.py
--rw-r--r--   0 keunwoo    (501) staff       (20)      509 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/email_sending.py
--rw-r--r--   0 keunwoo    (501) staff       (20)      809 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/file_attachment.py
--rw-r--r--   0 keunwoo    (501) staff       (20)     1324 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/reading_email_content.py
--rw-r--r--   0 keunwoo    (501) staff       (20)      846 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/reading_email_title.py
--rw-r--r--   0 keunwoo    (501) staff       (20)     1220 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/send_notification.py
--rw-r--r--   0 keunwoo    (501) staff       (20)      300 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/slack_bot.py
-drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-20 20:06:07.848281 project_2023-0.1.0/project_progress/tests/
--rw-r--r--   0 keunwoo    (501) staff       (20)     2979 2023-04-18 22:42:16.000000 project_2023-0.1.0/project_progress/tests/test_all.py
--rw-r--r--   0 keunwoo    (501) staff       (20)     1495 2023-04-18 22:42:16.000000 project_2023-0.1.0/pyproject.toml
--rw-r--r--   0 keunwoo    (501) staff       (20)      132 2023-04-18 22:42:16.000000 project_2023-0.1.0/requirements.txt
--rw-r--r--   0 keunwoo    (501) staff       (20)       38 2023-04-20 20:06:07.849305 project_2023-0.1.0/setup.cfg
--rw-r--r--   0 keunwoo    (501) staff       (20)       38 2023-04-18 22:42:16.000000 project_2023-0.1.0/setup.py
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.876094 project_2023-0.1.2/
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.871580 project_2023-0.1.2/.github/
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.872218 project_2023-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 keunwoo    (501) staff       (20)      834 2023-02-20 23:13:02.000000 project_2023-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 keunwoo    (501) staff       (20)      595 2023-02-20 23:13:02.000000 project_2023-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 keunwoo    (501) staff       (20)      118 2023-03-28 04:18:52.000000 project_2023-0.1.2/.github/dependabot.yml
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.872497 project_2023-0.1.2/.github/workflows/
+-rw-r--r--   0 keunwoo    (501) staff       (20)      686 2023-04-26 00:46:41.000000 project_2023-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1799 2023-02-20 23:13:02.000000 project_2023-0.1.2/.gitignore
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1887 2023-04-18 22:42:16.000000 project_2023-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 keunwoo    (501) staff       (20)    11357 2023-02-20 23:13:02.000000 project_2023-0.1.2/LICENSE
+-rw-r--r--   0 keunwoo    (501) staff       (20)     2239 2023-04-18 22:42:16.000000 project_2023-0.1.2/Makefile
+-rw-r--r--   0 keunwoo    (501) staff       (20)    16554 2023-04-29 04:13:46.875771 project_2023-0.1.2/PKG-INFO
+-rw-r--r--   0 keunwoo    (501) staff       (20)     2778 2023-04-29 04:07:30.000000 project_2023-0.1.2/README.md
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.873497 project_2023-0.1.2/project_2023.egg-info/
+-rw-r--r--   0 keunwoo    (501) staff       (20)    16554 2023-04-29 04:13:46.000000 project_2023-0.1.2/project_2023.egg-info/PKG-INFO
+-rw-r--r--   0 keunwoo    (501) staff       (20)      684 2023-04-29 04:13:46.000000 project_2023-0.1.2/project_2023.egg-info/SOURCES.txt
+-rw-r--r--   0 keunwoo    (501) staff       (20)        1 2023-04-29 04:13:46.000000 project_2023-0.1.2/project_2023.egg-info/dependency_links.txt
+-rw-r--r--   0 keunwoo    (501) staff       (20)      156 2023-04-29 04:13:46.000000 project_2023-0.1.2/project_2023.egg-info/requires.txt
+-rw-r--r--   0 keunwoo    (501) staff       (20)       17 2023-04-29 04:13:46.000000 project_2023-0.1.2/project_2023.egg-info/top_level.txt
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.875205 project_2023-0.1.2/project_progress/
+-rw-r--r--   0 keunwoo    (501) staff       (20)      500 2023-04-29 04:07:30.000000 project_2023-0.1.2/project_progress/__init__.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1160 2023-04-26 00:46:42.000000 project_2023-0.1.2/project_progress/email_sending.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1360 2023-04-26 00:46:42.000000 project_2023-0.1.2/project_progress/file_attachment.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1804 2023-04-26 00:46:42.000000 project_2023-0.1.2/project_progress/reading_email_content.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1320 2023-04-26 00:46:42.000000 project_2023-0.1.2/project_progress/reading_email_title.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1426 2023-04-26 00:46:42.000000 project_2023-0.1.2/project_progress/send_notification.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)      513 2023-04-26 00:46:42.000000 project_2023-0.1.2/project_progress/slack_bot.py
+drwxr-xr-x   0 keunwoo    (501) staff       (20)        0 2023-04-29 04:13:46.875416 project_2023-0.1.2/project_progress/tests/
+-rw-r--r--   0 keunwoo    (501) staff       (20)     2979 2023-04-18 22:42:16.000000 project_2023-0.1.2/project_progress/tests/test_all.py
+-rw-r--r--   0 keunwoo    (501) staff       (20)     1495 2023-04-29 04:12:52.000000 project_2023-0.1.2/pyproject.toml
+-rw-r--r--   0 keunwoo    (501) staff       (20)      132 2023-04-26 00:46:42.000000 project_2023-0.1.2/requirements.txt
+-rw-r--r--   0 keunwoo    (501) staff       (20)       38 2023-04-29 04:13:46.876145 project_2023-0.1.2/setup.cfg
+-rw-r--r--   0 keunwoo    (501) staff       (20)       38 2023-04-18 22:42:16.000000 project_2023-0.1.2/setup.py
```

### Comparing `project_2023-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `project_2023-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `project_2023-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/.github/workflows/CI.yml` & `project_2023-0.1.2/.github/workflows/CI.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: CI
+name: Build Status
 
 on:
   push:
     branches: [main]
   pull_request:
     branches: [main]
```

### Comparing `project_2023-0.1.0/.gitignore` & `project_2023-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/CONTRIBUTING.md` & `project_2023-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/LICENSE` & `project_2023-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/Makefile` & `project_2023-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/PKG-INFO` & `project_2023-0.1.2/project_2023.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: project_2023
-Version: 0.1.0
+Name: project-2023
+Version: 0.1.2
 Summary: An example python project
 Author-email: Your Name <Your_Email@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,41 +220,85 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # Sending Notifications to Your Smartphone for Specific Keywords in Emails
 The project involves creating a program that reads gmail and sends notifications to your smartphone using slack when a specific keyword appears.
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Issue](https://img.shields.io/github/issues/kw9212/project_2023)](https://github.com/kw9212/project_2023.git)
+![](https://img.shields.io/github/issues/kw9212/project_2023)
+[![Build Status](https://github.com/kw9212/project_2023/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/kw9212/project_2023/actions?query=workflow%3A%22Build+Status%22)
 ![](https://github.com/kw9212/project_2023/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/github/kw9212/project_2023/branch/main/graph/badge.svg?token=05c337ef-226f-41c3-b136-0fe9842b5192)](https://app.codecov.io/gh/kw9212/project_2023)
+[![PyPI](https://img.shields.io/pypi/v/project-2023)](https://pypi.org/project/project-2023/)
+[![Documentation Status](https://readthedocs.org/projects/project-2023/badge/?version=latest)](https://project-2023.readthedocs.io/en/latest/?badge=latest)
+
+
+Overview
+--------
 
-# Overview
 This idea came from the challenge of having to sort through many emails every day to find the important ones. Gmail already has a labeling function that classifies emails based on specific email addresses as filters. This project aims to create a function that sends notifications based on keywords using slack and smartphones. There is also potential to expand this project to find information in other ways besides just keywords.
 
-## Installation
 
-Install the library using pip:
+Dependencies
+------------
+
+- slack_sdk
+
+Usage
+-----
+
+### Quick Start
+
+1. Install the package:
+
+```python
 
-```bash
 pip install project_progress
+
+```
+
+2. Set up your Slack webhook URL. Follow these [instructions](./documentation.md) to create a Slack webhook URL.
+
+3. Create a Python script and import the required functions:
+
+```python
+
+from project_progress import read_email_titles, sendSlackWebhook
+
+```
+
+4. Use the functions to read email titles and send Slack notifications based on specific keywords:
+
+```python
+email_titles = read_email_titles()
+keyword = "important"
+
+for title in email_titles:
+    if keyword in title:
+        sendSlackWebhook("Keyword found in email title: " + title, webhook_url)
 ```
 
-## Usage
+### Lint/Test
+To run linting and tests, you need to have the following tools installed:
 
-To use the Project Progress Tracking System:
+Flake8 for linting
+pytest for testing
+Install them using pip:
 
-1. Configure your email and Slack settings in the `emails.json` file.
-2. Import the library into your Python script:
+```python
+pip install flake8 pytest
+```
 
-    ```python
-    from project_progress import send_email, send_slack_notification
-    ```
+### Linting
+To lint your code, run the following command in your project directory:
 
-3. Use the `send_email` and `send_slack_notification` functions to send notifications:
+```python
+flake8
+```
 
-    ```python
-    send_email(subject="Task Update", message="The task is now complete.")
-    send_slack_notification(text="The task is now complete.")
-    ```
+### Testing
+To run tests, execute the following command in your project directory:
 
+```python
+pytest
+```
 For more detailed usage instructions and available options, please refer to the [documentation](./documentation.md).
```

### Comparing `project_2023-0.1.0/project_2023.egg-info/PKG-INFO` & `project_2023-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: project-2023
-Version: 0.1.0
+Name: project_2023
+Version: 0.1.2
 Summary: An example python project
 Author-email: Your Name <Your_Email@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -220,41 +220,85 @@
 Provides-Extra: develop
 License-File: LICENSE
 
 # Sending Notifications to Your Smartphone for Specific Keywords in Emails
 The project involves creating a program that reads gmail and sends notifications to your smartphone using slack when a specific keyword appears.
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
-[![Issue](https://img.shields.io/github/issues/kw9212/project_2023)](https://github.com/kw9212/project_2023.git)
+![](https://img.shields.io/github/issues/kw9212/project_2023)
+[![Build Status](https://github.com/kw9212/project_2023/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/kw9212/project_2023/actions?query=workflow%3A%22Build+Status%22)
 ![](https://github.com/kw9212/project_2023/actions/workflows/build.yml/badge.svg)
 [![codecov](https://codecov.io/github/kw9212/project_2023/branch/main/graph/badge.svg?token=05c337ef-226f-41c3-b136-0fe9842b5192)](https://app.codecov.io/gh/kw9212/project_2023)
+[![PyPI](https://img.shields.io/pypi/v/project-2023)](https://pypi.org/project/project-2023/)
+[![Documentation Status](https://readthedocs.org/projects/project-2023/badge/?version=latest)](https://project-2023.readthedocs.io/en/latest/?badge=latest)
+
+
+Overview
+--------
 
-# Overview
 This idea came from the challenge of having to sort through many emails every day to find the important ones. Gmail already has a labeling function that classifies emails based on specific email addresses as filters. This project aims to create a function that sends notifications based on keywords using slack and smartphones. There is also potential to expand this project to find information in other ways besides just keywords.
 
-## Installation
 
-Install the library using pip:
+Dependencies
+------------
+
+- slack_sdk
+
+Usage
+-----
+
+### Quick Start
+
+1. Install the package:
+
+```python
 
-```bash
 pip install project_progress
+
+```
+
+2. Set up your Slack webhook URL. Follow these [instructions](./documentation.md) to create a Slack webhook URL.
+
+3. Create a Python script and import the required functions:
+
+```python
+
+from project_progress import read_email_titles, sendSlackWebhook
+
+```
+
+4. Use the functions to read email titles and send Slack notifications based on specific keywords:
+
+```python
+email_titles = read_email_titles()
+keyword = "important"
+
+for title in email_titles:
+    if keyword in title:
+        sendSlackWebhook("Keyword found in email title: " + title, webhook_url)
 ```
 
-## Usage
+### Lint/Test
+To run linting and tests, you need to have the following tools installed:
 
-To use the Project Progress Tracking System:
+Flake8 for linting
+pytest for testing
+Install them using pip:
 
-1. Configure your email and Slack settings in the `emails.json` file.
-2. Import the library into your Python script:
+```python
+pip install flake8 pytest
+```
 
-    ```python
-    from project_progress import send_email, send_slack_notification
-    ```
+### Linting
+To lint your code, run the following command in your project directory:
 
-3. Use the `send_email` and `send_slack_notification` functions to send notifications:
+```python
+flake8
+```
 
-    ```python
-    send_email(subject="Task Update", message="The task is now complete.")
-    send_slack_notification(text="The task is now complete.")
-    ```
+### Testing
+To run tests, execute the following command in your project directory:
 
+```python
+pytest
+```
 For more detailed usage instructions and available options, please refer to the [documentation](./documentation.md).
```

### Comparing `project_2023-0.1.0/project_2023.egg-info/SOURCES.txt` & `project_2023-0.1.2/project_2023.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/project_progress/reading_email_content.py` & `project_2023-0.1.2/project_progress/reading_email_content.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import email
 from email import policy
 
 
 def find_encoding_info(txt):
+    """
+    Find encoding information for a given text.
+
+    :param txt: The text to find encoding information for (str)
+    :return: A tuple containing the decoded subject and the encoding (tuple)
+    """
     info = email.header.decode_header(txt)
     subject, encode = info[0]
     return subject, encode
 
 
 def read_email_contents(imap, num_emails=5):
+    """
+    Read the email contents from an IMAP mailbox.
+
+    :param imap: An IMAP object connected to the mailbox (IMAP object)
+    :param num_emails: The number of email contents to read (int), default is 5
+    :return: A list of email content information (list)
+    """
     email_contents = []
 
     imap.select("INBOX")
     resp, data = imap.uid("search", None, "All")
     all_email = data[0].split()
     last_email = all_email[-num_emails:]
```

### Comparing `project_2023-0.1.0/project_progress/reading_email_title.py` & `project_2023-0.1.2/project_progress/reading_email_title.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import email
 from email import policy
 
 
 def find_encoding_info(txt):
+    """
+    Find encoding information for a given text.
+
+    :param txt: The text to find encoding information for (str)
+    :return: A tuple containing the decoded subject and the encoding (tuple)
+    """
     info = email.header.decode_header(txt)
     subject, encode = info[0]
     return subject, encode
 
 
 def read_email_titles(imap, num_emails=5):
+    """
+    Read the email titles from an IMAP mailbox.
+
+    :param imap: An IMAP object connected to the mailbox (IMAP object)
+    :param num_emails: The number of email titles to read (int), default is 5
+    :return: A list of email title information (list)
+    """
     email_titles = []
 
     imap.select("INBOX")
     resp, data = imap.uid("search", None, "All")
     all_email = data[0].split()
     last_email = all_email[-num_emails:]
```

### Comparing `project_2023-0.1.0/project_progress/send_notification.py` & `project_2023-0.1.2/project_progress/send_notification.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from .slack_bot import sendSlackWebhook
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
 emails_path = os.path.join(current_dir, "emails.json")
 
 
 def find_encoding_info(txt):
+    """
+    Find encoding information for a given text.
+
+    :param txt: The text to find encoding information for (str)
+    :return: A tuple containing the decoded subject and the encoding (tuple)
+    """
     info = email.header.decode_header(txt)
     subject, encode = info[0]
     return subject, encode
 
 
 # Read email data from the local JSON file
 with open(emails_path, "r") as file:
```

### Comparing `project_2023-0.1.0/project_progress/tests/test_all.py` & `project_2023-0.1.2/project_progress/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `project_2023-0.1.0/pyproject.toml` & `project_2023-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "project_2023"
 authors = [{name = "Your Name", email = "Your_Email@gmail.com"}]
 description="An example python project"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.2"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

