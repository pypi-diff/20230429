# Comparing `tmp/opentrain-0.0.3.tar.gz` & `tmp/opentrain-0.0.4.tar.gz`

## Comparing `opentrain-0.0.3.tar` & `opentrain-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 opentrain-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 opentrain-0.0.3/examples/text_classification_imdb.ipynb
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 opentrain-0.0.3/src/opentrain/__init__.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 opentrain-0.0.3/src/opentrain/predict.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 opentrain-0.0.3/src/opentrain/train.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 opentrain-0.0.3/src/opentrain/utils.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 opentrain-0.0.3/.gitignore
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentrain-0.0.3/LICENSE
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 opentrain-0.0.3/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 opentrain-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 opentrain-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 opentrain-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0     9670 2020-02-02 00:00:00.000000 opentrain-0.0.4/examples/text_classification_imdb.ipynb
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/__init__.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/predict.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/schemas.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/train.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 opentrain-0.0.4/src/opentrain/utils.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 opentrain-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 opentrain-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 opentrain-0.0.4/README.md
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 opentrain-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 opentrain-0.0.4/PKG-INFO
```

### Comparing `opentrain-0.0.3/mkdocs.yml` & `opentrain-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.3/examples/text_classification_imdb.ipynb` & `opentrain-0.0.4/examples/text_classification_imdb.ipynb`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.3/src/opentrain/train.py` & `opentrain-0.0.4/src/opentrain/train.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,40 +35,48 @@
             "davinci",
         ], "The model must be one of the following: ada, babbage, curie, davinci."
         self.model = model
 
     def train(
         self,
         path_or_buf: Union[str, Path, list],
+        local_validation: bool = False,
         epochs: int = 10,
         batch_size: int = 32,
     ) -> str:
         """Train (fine-tune) an OpenAI model on a given dataset.
 
         Args:
             path_or_buf: The path to the training data, or a list of dictionaries
                 containing the training data.
+            local_validation: If True, validate the training data locally before
+                uploading it to OpenAI. Defaults to False, which means that the
+                data will be validated, but in OpenAI-side.
             epochs: The number of epochs to train the model for.
             batch_size: The batch size to use for training.
 
         Returns:
             The fine-tune ID.
         """
+        # TODO(alvarobartt): create a `Dataset` class to handle the training data.
         if isinstance(path_or_buf, list):
             file_path = prepare_openai_dataset(path_or_buf)
         elif isinstance(path_or_buf, Path):
             file_path = path_or_buf.as_posix()
         else:
             file_path = path_or_buf
 
-        assert validate_openai_dataset(file_path), (
-            "The dataset is not valid, since it must contain only prompt-completion"
-            " pairs."
-        )
+        if local_validation:
+            assert validate_openai_dataset(file_path), (
+                "The dataset is not valid, since it must contain only prompt-completion"
+                " pairs."
+            )
 
+        # TODO(alvarobartt): one may want to use a previously uploaded file, so we
+        #  should check if the file is already uploaded, and if so, then use it.
         upload_response = openai.File.create(
             file=open(file_path, "rb"),
             purpose="fine-tune",
         )
         file_id = upload_response.id
         fine_tune_response = openai.FineTune.create(
             training_file=file_id,
```

### Comparing `opentrain-0.0.3/src/opentrain/utils.py` & `opentrain-0.0.4/src/opentrain/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import json
 from pathlib import Path
 from typing import List, Union
 from uuid import uuid4
 
 import openai
 
+from opentrain.schemas import PromptCompletion
+
 
 def list_fine_tunes(just_succeeded: bool = True) -> List[str]:
     """List all fine-tuned models in your OpenAI account.
 
     Args:
         just_succeeded: If True, only return models that have succeeded.
 
     Returns:
         A list of fine-tuned model IDs.
     """
     fine_tunes = openai.FineTune.list()["data"]
     if just_succeeded:
+        # TODO(alvarobartt): add an `Enum` to handle possible statuses.
         return [
             fine_tune["fine_tuned_model"]
             for fine_tune in fine_tunes
             if fine_tune["status"] == "succeeded"
         ]
     return [fine_tune["fine_tuned_model"] for fine_tune in fine_tunes]
 
@@ -59,15 +62,23 @@
 
     Returns:
         True if the training data is valid, False otherwise.
     """
     if isinstance(file_path, Path):
         file_path = file_path.as_posix()
     with open(file_path, "r") as f:
-        for line in f:
+        lines = f.readlines()
+        if len(lines) < 1:
+            # TODO(alvarobartt): log error with `structlog`
+            return False
+        for line in lines:
             try:
-                json_line = json.loads(line)
-            except json.JSONDecodeError as e:
-                raise ValueError(f"Line {line} is not a JSON object.") from e
-            if not ["prompt", "completion"] == list(json_line.keys()):
+                PromptCompletion(**json.loads(line))
+            except json.JSONDecodeError:
+                # TODO(alvarobartt): add `structlog`
+                # raise ValueError(f"Line {line} is not a JSON object.") from e
+                return False
+            except Exception:
+                # TODO(alvarobartt): add `structlog`
+                # raise ValueError(f"Line {line} is not a prompt-completion pair.") from e
                 return False
     return True
```

### Comparing `opentrain-0.0.3/.gitignore` & `opentrain-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.3/LICENSE` & `opentrain-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.3/README.md` & `opentrain-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `opentrain-0.0.3/pyproject.toml` & `opentrain-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 authors = [{name = "Alvaro Bartolome", email = "alvarobartt@gmail.com"}]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["openai~=0.27.4"]
 description = "🚂 Fine-tune OpenAI models for text classification, question answering, and more"
 dynamic = ["version"]
 keywords = []
@@ -34,17 +33,18 @@
 [project.optional-dependencies]
 docs = [
   "mkdocs~=1.4.0",
   "mkdocs-material~=8.5.4",
   "mkdocs-git-revision-date-localized-plugin~=1.1.0",
   "mkdocstrings[python]~=0.19.0",
 ]
+pydantic = ["pydantic>=1.10,<2"]
 quality = [
   "black~=22.10.0",
-  "ruff~=0.0.194",
+  "ruff~=0.0.263",
   "pre-commit~=2.20.0",
 ]
 tests = [
   "pytest~=7.1.2",
 ]
 
 [tool.hatch.envs.quality]
```

### Comparing `opentrain-0.0.3/PKG-INFO` & `opentrain-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: opentrain
-Version: 0.0.3
+Version: 0.0.4
 Summary: 🚂 Fine-tune OpenAI models for text classification, question answering, and more
 Project-URL: Documentation, https://alvarobartt.github.io/opentrain
 Project-URL: Issues, https://github.com/alvarobartt/opentrain/issues
 Project-URL: Source, https://github.com/alvarobartt/opentrain
 Author-email: Alvaro Bartolome <alvarobartt@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <3.11,>=3.8
 Requires-Dist: openai~=0.27.4
 Provides-Extra: docs
 Requires-Dist: mkdocs-git-revision-date-localized-plugin~=1.1.0; extra == 'docs'
 Requires-Dist: mkdocs-material~=8.5.4; extra == 'docs'
 Requires-Dist: mkdocstrings[python]~=0.19.0; extra == 'docs'
 Requires-Dist: mkdocs~=1.4.0; extra == 'docs'
+Provides-Extra: pydantic
+Requires-Dist: pydantic<2,>=1.10; extra == 'pydantic'
 Provides-Extra: quality
 Requires-Dist: black~=22.10.0; extra == 'quality'
 Requires-Dist: pre-commit~=2.20.0; extra == 'quality'
-Requires-Dist: ruff~=0.0.194; extra == 'quality'
+Requires-Dist: ruff~=0.0.263; extra == 'quality'
 Provides-Extra: tests
 Requires-Dist: pytest~=7.1.2; extra == 'tests'
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>opentrain</h1>
   <p>
```

