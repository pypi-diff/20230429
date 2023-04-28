# Comparing `tmp/gpt-review-0.0.1rc93.post1.tar.gz` & `tmp/gpt-review-0.0.1rc95.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.0.1rc93.post1.tar", last modified: Thu Apr 27 03:38:06 2023, max compression
+gzip compressed data, was "gpt-review-0.0.1rc95.post1.tar", last modified: Thu Apr 27 03:51:20 2023, max compression
```

## Comparing `gpt-review-0.0.1rc93.post1.tar` & `gpt-review-0.0.1rc95.post1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      333 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1333 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      697 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0      747 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      866 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.pypirc
--rw-r--r--   0        0        0      816 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/LICENSE
--rw-r--r--   0        0        0      733 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/README.md
--rw-r--r--   0        0        0     5116 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/action.yml
--rw-r--r--   0        0        0     6847 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/review.py
--rw-r--r--   0        0        0      363 2023-04-27 03:38:05.855001 gpt-review-0.0.1rc93.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0     5796 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      413 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      792 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/tests/conftest.py
--rw-r--r--   0        0        0     1193 2023-04-27 03:37:58.070914 gpt-review-0.0.1rc93.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 gpt-review-0.0.1rc93.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1333 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      697 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0      747 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      866 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.pypirc
+-rw-r--r--   0        0        0      816 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/LICENSE
+-rw-r--r--   0        0        0      733 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/README.md
+-rw-r--r--   0        0        0     5116 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/action.yml
+-rw-r--r--   0        0        0     6847 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/pyproject.toml
+-rw-r--r--   0        0        0    18646 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/review.py
+-rw-r--r--   0        0        0      363 2023-04-27 03:51:19.712891 gpt-review-0.0.1rc95.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0     5796 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1312 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      413 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0      792 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/tests/conftest.py
+-rw-r--r--   0        0        0     1193 2023-04-27 03:51:11.852858 gpt-review-0.0.1rc95.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0     2731 1970-01-01 00:00:00.000000 gpt-review-0.0.1rc95.post1/PKG-INFO
```

### Comparing `gpt-review-0.0.1rc93.post1/.devcontainer/devcontainer.json` & `gpt-review-0.0.1rc95.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.0.1rc95.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/.github/pull_request_template.md` & `gpt-review-0.0.1rc95.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/.github/workflows/python.yml` & `gpt-review-0.0.1rc95.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/.github/workflows/test-action.yml` & `gpt-review-0.0.1rc95.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/.gitignore` & `gpt-review-0.0.1rc95.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/.vscode/settings.json` & `gpt-review-0.0.1rc95.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/LICENSE` & `gpt-review-0.0.1rc95.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/README.md` & `gpt-review-0.0.1rc95.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/action.yml` & `gpt-review-0.0.1rc95.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/pyproject.toml` & `gpt-review-0.0.1rc95.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/review.py` & `gpt-review-0.0.1rc95.post1/review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/src/gpt_review/_ask.py` & `gpt-review-0.0.1rc95.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.0.1rc95.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/tests/conftest.py` & `gpt-review-0.0.1rc95.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/tests/test_gpt_cli.py` & `gpt-review-0.0.1rc95.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.0.1rc93.post1/PKG-INFO` & `gpt-review-0.0.1rc95.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.0.1rc93.post1
+Version: 0.0.1rc95.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

