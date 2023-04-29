# Comparing `tmp/opencv_stubs-0.0.4.tar.gz` & `tmp/opencv_stubs-0.0.5.tar.gz`

## Comparing `opencv_stubs-0.0.4.tar` & `opencv_stubs-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,101 @@
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/requirements/requirements.txt
--rw-r--r--   0        0        0    49905 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/src/cv2-stubs/__init__.pyi
--rw-r--r--   0        0        0    18359 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/src/cv2-stubs/constants.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/src/cv2-stubs/py.typed
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/LICENSE
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/README.md
--rw-r--r--   0        0        0     3188 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 opencv_stubs-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/requirements/requirements.txt
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/__init__.pyi
+-rw-r--r--   0        0        0   165718 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/classes.pyi
+-rw-r--r--   0        0        0    51441 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/constants.pyi
+-rw-r--r--   0        0        0   529741 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/functions.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/py.typed
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/__init__.py
+-rw-r--r--   0        0        0    34278 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/aruco.pyi
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/barcode.pyi
+-rw-r--r--   0        0        0    11087 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/bgsegm.pyi
+-rw-r--r--   0        0        0    19723 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/bioinspired.pyi
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ccm.pyi
+-rw-r--r--   0        0        0     4579 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/colored_kinfu.pyi
+-rw-r--r--   0        0        0    23465 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/cuda.pyi
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/data.pyi
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/datasets.pyi
+-rw-r--r--   0        0        0    16562 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/detail.pyi
+-rw-r--r--   0        0        0    44941 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dnn.pyi
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dnn_superres.pyi
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dpm.pyi
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/dynafu.pyi
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/error.pyi
+-rw-r--r--   0        0        0    34295 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/face.pyi
+-rw-r--r--   0        0        0    21983 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/fisheye.pyi
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/flann.pyi
+-rw-r--r--   0        0        0     9340 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ft.pyi
+-rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/hfs.pyi
+-rw-r--r--   0        0        0     5701 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/img_hash.pyi
+-rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/intensity_transform.pyi
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ipp.pyi
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/large_kinfu.pyi
+-rw-r--r--   0        0        0     4353 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/legacy.pyi
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/line_descriptor.pyi
+-rw-r--r--   0        0        0     8769 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/linemod.pyi
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/load_config_py3.pyi
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/mat_wrapper.pyi
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/mcc.pyi
+-rw-r--r--   0        0        0    59687 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ml.pyi
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/motempl.pyi
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/multicalib.pyi
+-rw-r--r--   0        0        0     6571 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ocl.pyi
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ogl.pyi
+-rw-r--r--   0        0        0    14145 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/omnidir.pyi
+-rw-r--r--   0        0        0    27907 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/optflow.pyi
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/parallel.pyi
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/phase_unwrapping.pyi
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/plot.pyi
+-rw-r--r--   0        0        0     8089 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ppf_match_3d.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/qt.pyi
+-rw-r--r--   0        0        0    11898 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/quality.pyi
+-rw-r--r--   0        0        0     5249 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/rapid.pyi
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/reg.pyi
+-rw-r--r--   0        0        0    29883 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/rgbd.pyi
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/saliency.pyi
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/samples.pyi
+-rw-r--r--   0        0        0     4834 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/segmentation.pyi
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/stereo.pyi
+-rw-r--r--   0        0        0     7467 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/structured_light.pyi
+-rw-r--r--   0        0        0    26786 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/text.pyi
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/version.pyi
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/videoio_registry.pyi
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/videostab.pyi
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/wechat_qrcode.pyi
+-rw-r--r--   0        0        0    40532 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/xfeatures2d.pyi
+-rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/xphoto.pyi
+-rw-r--r--   0        0        0   105662 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/__init__.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/core.pyi
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/ie.pyi
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/oak.pyi
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/onnx.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/own.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/render.pyi
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/video.pyi
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/streaming/__init__.pyi
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/__init__.pyi
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/draw.pyi
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/gapi/wip/gst.pyi
+-rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/kinfu/__init__.pyi
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/kinfu/detail.pyi
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/misc/__init__.pyi
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/misc/version.pyi
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/__init__.pyi
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/fs.pyi
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/utils/nested.pyi
+-rw-r--r--   0        0        0    80008 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ximgproc/__init__.pyi
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/src/cv2-stubs/modules/ximgproc/segmentation.pyi
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/add_missing_overloads.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/generate_classes.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/generate_constants.py
+-rw-r--r--   0        0        0     3594 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/generate_modules.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/merge_with_microsoft_stubs.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/processing_utils.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/utils/undefined_to_any.py
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/README.md
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 opencv_stubs-0.0.5/PKG-INFO
```

### Comparing `opencv_stubs-0.0.4/.pre-commit-config.yaml` & `opencv_stubs-0.0.5/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     hooks:
       - id: ruff
 
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.300
     hooks:
     - id: pyright
-      additional_dependencies: ["numpy>=1.21"]
+      additional_dependencies: ["numpy>=1.21", "opencv-python"]
```

### Comparing `opencv_stubs-0.0.4/requirements/requirements-build.txt` & `opencv_stubs-0.0.5/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.4/requirements/requirements-dev.txt` & `opencv_stubs-0.0.5/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.4/LICENSE` & `opencv_stubs-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opencv_stubs-0.0.4/pyproject.toml` & `opencv_stubs-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 [project.urls]
 "Homepage" = "https://github.com/hoel-bagard/opencv-stubs"
 "Bug Tracker" = "https://github.com/hoel-bagard/opencv-stubs/issues"
 
 [project.optional-dependencies]
 dev = ["pre-commit", "pip-tools", "ruff", "pyright"]
 build = ["hatch"]
+flake8 = ["flake8", "flake8-bugbear", "flake8-comprehensions", "flake8-docstrings", "flake8-builtins", "flake8-quotes", "pep8-naming", "flake8-import-order", "flake8-noqa", "flake8-broken-line", "flake8-commas", "Flake8-pyproject"]
 # I couldn't figure out how to have "opencv or opencv-headless" as dependency, so they are both optional.
 opencv = ["opencv-python>=4.7.0"]
+opencv-contrib = ["opencv-contrib-python>=4.7.0"]
 opencv-headless = ["opencv-python-headless>=4.7.0"]
 
 [tool.hatch.version]
 path = "src/cv2-stubs/__init__.pyi"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
@@ -55,17 +57,17 @@
 
 [tool.hatch.envs.pypi.scripts]
 # hatch run pypi:publish_test
 publish_test = "hatch build --clean && hatch publish -r test"
 publish = "hatch build --clean && hatch publish"
 
 [tool.ruff]
-select = ["A", "B", "C4", "E", "I", "Q", "UP", "ANN", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM","PTH", "TRY", "NPY", "RUF"]
-ignore = ["D1", "D401", "D204", "D203", "D213", "S101", "PLR2004", "A002", "A003"]
-line-length = 10000
+select = ["B", "C4", "E", "I", "Q", "UP", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM","PTH", "TRY", "NPY", "RUF"]  # , "ANN"
+ignore = ["D1", "D401", "D204", "D203", "D213", "S101", "PLR2004"]
+line-length = 20000
 
 [tool.ruff.isort]
 order-by-type = false
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
@@ -75,34 +77,35 @@
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
 
 reportMissingModuleSource = false
 reportMissingImports = true
 reportMissingTypeStubs = false
-reportUnusedImport = true
+reportUnusedImport = false
 reportUnusedClass = "warning"
 reportUnusedFunction = "warning"
 reportUnusedVariable = "warning"
 reportDuplicateImport = "warning"
 reportUntypedNamedTuple = "warning"
 reportUntypedFunctionDecorator = "warning"
 reportUntypedClassDecorator = "warning"
 reportMissingSuperCall = false
 reportUnknownArgumentType = "warning"
 reportUnknownLambdaType = "warning"
 reportUnknownVariableType = "warning"
 reportUnknownMemberType = false
-reportMissingParameterType = "warning"
-reportMissingTypeArgument = "warning"
+# reportMissingParameterType = "warning"
+# reportMissingTypeArgument = "warning"
 reportCallInDefaultInitializer = false
 reportUnnecessaryIsInstance = "warning"
 reportUnnecessaryCast = "warning"
 reportUnnecessaryComparison = "warning"
 reportImplicitStringConcatenation = false
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
+reportInvalidStringEscapeSequence = false
 
 pythonVersion = "3.10"
 pythonPlatform = "Linux"
```

### Comparing `opencv_stubs-0.0.4/PKG-INFO` & `opencv_stubs-0.0.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,44 @@
-Metadata-Version: 2.1
-Name: opencv-stubs
-Version: 0.0.4
-Summary: Unofficial stubs for the opencv-python package.
-Project-URL: Homepage, https://github.com/hoel-bagard/opencv-stubs
-Project-URL: Bug Tracker, https://github.com/hoel-bagard/opencv-stubs/issues
-Author: Bagard Hoel
-License: MIT
-License-File: LICENSE
-Keywords: OpenCV,stubs
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.8
-Requires-Dist: numpy>=1.21
-Provides-Extra: build
-Requires-Dist: hatch; extra == 'build'
-Provides-Extra: dev
-Requires-Dist: pip-tools; extra == 'dev'
-Requires-Dist: pre-commit; extra == 'dev'
-Requires-Dist: pyright; extra == 'dev'
-Requires-Dist: ruff; extra == 'dev'
-Provides-Extra: opencv
-Requires-Dist: opencv-python>=4.7.0; extra == 'opencv'
-Provides-Extra: opencv-headless
-Requires-Dist: opencv-python-headless>=4.7.0; extra == 'opencv-headless'
-Description-Content-Type: text/markdown
-
 # OpenCV stubs
 
 [![PyPI](https://img.shields.io/pypi/v/opencv-stubs?color=green&style=flat)](https://pypi.org/project/opencv-stubs)
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/opencv-stubs?style=flat)](https://pypi.org/project/opencv-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/opencv-stubs?style=flat)](https://pypi.org/project/opencv-stubs)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/opencv-stubs?style=flat-square)](https://pypistats.org/packages/opencv-stubs)
 [![License](https://img.shields.io/pypi/l/opencv-stubs?style=flat)](https://opensource.org/licenses/MIT)
 ![Linting](https://github.com/hoel-bagard/opencv-stubs/actions/workflows/pre-commit.yaml/badge.svg)
 
-
 Unofficial python stubs for the opencv-python package.
 
-A stub file with all the cv2 function can be found on the [Microsoft stubs repo](https://github.com/microsoft/python-type-stubs/tree/main/cv2).\
-The stubs from this package are different in the sense that they include better (although wrong) typing. OpenCV handles more types than defined in this package (and has much more functions than defined in this package). If you would like a function / type to be added, feel free to open a PR.
+This package includes all the functions, classes and constants (please open an issue if you find a missing one).\
+For some functions, OpenCV may handle more types than defined in this package. If you would like a type/function to be added or modified, please open an issue or a PR. There may also be a few errors as some types have been added progrmmatically. Please open an issue if you see one.
+The typing is still a work in progress, if you want a function/method to be added first you can open an issue.
 
 The stubs include the docstrings as they are otherwise not available in the IDE (as far as I know).
 
-These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590#issuecomment-1493255962)).
+These stubs are a temporary help until official ones are made (see [this issue](https://github.com/opencv/opencv/issues/14590)).
 
 
 ## Installation
 
 The package is available on pypi [here](https://pypi.org/project/opencv-stubs/), you can install it with:
 
 ```
 pip install opencv-stubs
 ```
 
-The dependency on opencv is optional, and be accessed with `pip install opencv-stubs[opencv]` or `pip install opencv-stubs[opencv-headless]`.
+The dependency on opencv is optional, and can be accessed with:
+- `pip install opencv-stubs[opencv]`
+- `pip install opencv-stubs[opencv-contrib]`
+- `pip install opencv-stubs[opencv-headless]`
+
+
+## Acknowledgements
+
+A stub file with all the cv2 functions can be found on the [Microsoft stubs repo](https://github.com/microsoft/python-type-stubs/tree/main/cv2). This package reused those functions and added typing.
+
+
+## TODO:
+- [ ] Fix missing "..."   (` """\n\n/"""\n    ...\n\n`)
+- [ ] Do something about `cv2.gapi.cv`, `cv2.utils.cv2` and `cv2.mat_wrapper.cv` (do not duplicate everything if possible).
+- [ ] Handle cases like `cv2.misc.version.cv2.misc.version.cv2.misc.get_ocv_version()`.
+- [ ] Only include the `opencv-contrib` specific stubs when using `opencv-stubs[opencv-contrib]`.
```

