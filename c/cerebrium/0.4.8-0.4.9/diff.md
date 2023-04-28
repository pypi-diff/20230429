# Comparing `tmp/cerebrium-0.4.8.tar.gz` & `tmp/cerebrium-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-0.4.8.tar", max compression
+gzip compressed data, was "cerebrium-0.4.9.tar", max compression
```

## Comparing `cerebrium-0.4.8.tar` & `cerebrium-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-02-20 16:43:21.319909 cerebrium-0.4.8/LICENSE
--rw-r--r--   0        0        0     3321 2023-02-20 16:43:21.319909 cerebrium-0.4.8/README.md
--rw-r--r--   0        0        0      258 2023-02-20 16:47:20.907431 cerebrium-0.4.8/cerebrium/__init__.py
--rw-r--r--   0        0        0    19261 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/conduit.py
--rw-r--r--   0        0        0     2248 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/core.py
--rw-r--r--   0        0        0     2524 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/errors.py
--rw-r--r--   0        0        0    11252 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/flow.py
--rw-r--r--   0        0        0     2804 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      807 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/models/base.py
--rw-r--r--   0        0        0      202 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/models/hf_transformer.py
--rw-r--r--   0        0        0      417 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/models/torch.py
--rw-r--r--   0        0        0     4568 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-02-20 16:43:21.319909 cerebrium-0.4.8/cerebrium/utils.py
--rw-r--r--   0        0        0     1584 2023-02-20 16:47:20.907431 cerebrium-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 cerebrium-0.4.8/setup.py
--rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 cerebrium-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-02-21 14:55:13.514897 cerebrium-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3321 2023-02-21 14:55:13.514897 cerebrium-0.4.9/README.md
+-rw-r--r--   0        0        0      258 2023-02-21 14:59:12.597668 cerebrium-0.4.9/cerebrium/__init__.py
+-rw-r--r--   0        0        0    19297 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/conduit.py
+-rw-r--r--   0        0        0     2248 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/core.py
+-rw-r--r--   0        0        0     2524 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/errors.py
+-rw-r--r--   0        0        0    11252 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/flow.py
+-rw-r--r--   0        0        0     2804 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      807 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/base.py
+-rw-r--r--   0        0        0      202 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/hf_transformer.py
+-rw-r--r--   0        0        0      417 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-02-21 14:55:13.514897 cerebrium-0.4.9/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     4568 2023-02-21 14:55:13.518897 cerebrium-0.4.9/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-02-21 14:55:13.518897 cerebrium-0.4.9/cerebrium/utils.py
+-rw-r--r--   0        0        0     1584 2023-02-21 14:59:12.597668 cerebrium-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     4503 1970-01-01 00:00:00.000000 cerebrium-0.4.9/setup.py
+-rw-r--r--   0        0        0     4638 1970-01-01 00:00:00.000000 cerebrium-0.4.9/PKG-INFO
```

### Comparing `cerebrium-0.4.8/LICENSE` & `cerebrium-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/README.md` & `cerebrium-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/conduit.py` & `cerebrium-0.4.9/cerebrium/conduit.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,19 +205,21 @@
         from torch import Tensor
 
         if not self.ready:
             return "Conduit not ready. Conduit components have not been loaded."
         else:
             if self.flow[0][0] == ModelType.TORCH:
                 data = Tensor(atleast_2d(data)).to(self.device)
-            elif self.flow[0][0] == ModelType.ONNX or self.flow[0][0] == ModelType.HUGGINGFACE_TRANSFORMER:
+            elif self.flow[0][0] == ModelType.ONNX:
                 if isinstance(data, list):
                     data = data[0]
                 else:
                     pass
+            elif self.flow[0][0] == ModelType.HUGGINGFACE_TRANSFORMER:
+                pass
             elif self.flow[0][0] == ModelType.SPACY:
                 data = data[0]
             else:
                 data = atleast_2d(data)
 
             for (model_type, _, processors), (model) in zip(self.flow, self.graph):
                 # Run the preprocessor
```

### Comparing `cerebrium-0.4.8/cerebrium/core.py` & `cerebrium-0.4.9/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/errors.py` & `cerebrium-0.4.9/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/flow.py` & `cerebrium-0.4.9/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/logging/arize.py` & `cerebrium-0.4.9/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/logging/base.py` & `cerebrium-0.4.9/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/logging/censius.py` & `cerebrium-0.4.9/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/models/base.py` & `cerebrium-0.4.9/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/models/sklearn.py` & `cerebrium-0.4.9/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/cerebrium/requests.py` & `cerebrium-0.4.9/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.4.8/pyproject.toml` & `cerebrium-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "0.4.8"
+version = "0.4.9"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.urls]
 "Homepage" = "https://www.cerebrium.ai"
```

### Comparing `cerebrium-0.4.8/setup.py` & `cerebrium-0.4.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 extras_require = \
 {'onnxruntime': ['onnxruntime>=1.13,<1.15'],
  'onnxruntime-gpu': ['onnxruntime-gpu>=1.14,<1.15']}
 
 setup_kwargs = {
     'name': 'cerebrium',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': '',
     'long_description': '# Cerebrium\n\nCerebrium is the Python package built for use with the [Cerebrium](https://www.cerebrium.ai/) platform, which allows you to deploy your machine learning models as a REST API with a single line of code.\n\nFor usage consult the [documentation](https://docs.cerebrium.ai/). The repo for the documentation can be found [here](https://github.com/CerebriumAI/docs).\n\n# Development environment\nCerebrium uses Poetry for dependency management and packaging. To install Poetry, follow the instructions [here](https://python-poetry.org/docs/#installation). Alternatively, consult our article on [how to manage your python environments](https://blog.cerebrium.ai/setting-up-your-data-science-and-ml-development-environment-949277339939?gi=54b980dd4e1d).\n\nYou can run the following steps to setup your Python development environment with the following commands:\n```bash\npoetry install\npoetry shell\n```\nYou should use this environment to run tests, notebooks and build the package.\n\nFurthermore, you should set up a `.env` file in the project root with the following environment variables:\n```bash\nDEVELOPMENT_ENV=dev\n```\n\nYou can add packages to the project by running the following command:\n```bash\npoetry add <package>\n```\n\nYou **will** need to relock if you have added any packages to the project. You can do this by running the following command:\n```bash\npoetry lock\n```\n\n## Codespaces Setup\nTo set up a Codespaces for development, you should run the following command to setup AWS:\n```bash\ncd ~\ncurl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"\nunzip awscliv2.zip\nsudo ./aws/install\n```\n\n## Running tests\nTo run the tests, run the following command:\n```bash\npoetry run pytest --cov-report html:cov_html\\\n          --cov-report annotate:cov_annotate\\\n          --cov=cerebrium tests/\n```\n\n## Publishing Development Builds\nTo publish a development build on CodeArtifact, run the following command to configure Poetry:\n```bash\npoetry config http-basic.cerebrium aws $(aws codeartifact get-authorization-token --domain-owner 288552132534 --domain cerebrium --query \'authorizationToken\' --output text --region eu-west-1)\n```\n\nThen, run the following command to publish the package:\n```bash\npoetry shell # this is needed to set the version dynamically\npoetry publish --build -r cerebrium\n```\n\nIf the patch version is not up to date, merge the latest version tag into the branch:\n```bash\ngit merge v<tag>\n```\n\n## Install a development build\nTo install a development build, run the following command to configure pip:\n```bash\n\naws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1\n```\nThen, pip install:\n```bash\npip install --pre cerebrium\n```\n\n## Exporting Requirements for Cerebrium Server\nYou should export the requirements for the Cerebrium server by running the following command:\n```bash\npoetry export >> cerebrium-requirements.txt\n```\nOnce this is done, add them to the `cerebrium-conduit-server` repo.\n\n### Resources for Poetry/CodeArtifact\n- https://repost.aws/questions/QURD7aFNj_R9-8odJY5mfgrw/npm-publish-for-a-package-to-aws-code-artifact-repo-fails-with-error-the-provided-package-is-configured-to-block-new-version-publishes\n- https://docs.aws.amazon.com/codeartifact/latest/ug/python-configure-pip.html',
     'author': 'Elijah Roussos',
     'author_email': 'elijah@cerebrium.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cerebrium-0.4.8/PKG-INFO` & `cerebrium-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 0.4.8
+Version: 0.4.9
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

