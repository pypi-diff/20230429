# Comparing `tmp/anomalearn-0.0.1.tar.gz` & `tmp/anomalearn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anomalearn-0.0.1.tar", max compression
+gzip compressed data, was "anomalearn-0.0.2.tar", max compression
```

## Comparing `anomalearn-0.0.1.tar` & `anomalearn-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,119 @@
--rw-r--r--   0        0        0        0 2023-03-31 12:49:40.133024 anomalearn-0.0.1/anomalearn/__init__.py
--rw-r--r--   0        0        0     1088 2023-03-31 12:55:17.226713 anomalearn-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1046 2023-03-31 13:48:48.206743 anomalearn-0.0.1/README.md
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 anomalearn-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      770 2023-04-19 10:38:37.660681 anomalearn-0.0.2/anomalearn/__init__.py
+-rw-r--r--   0        0        0     3742 2023-04-15 14:33:53.106116 anomalearn-0.0.2/anomalearn/abc.py
+-rw-r--r--   0        0        0      971 2023-04-15 14:33:53.105116 anomalearn-0.0.2/anomalearn/algorithms/__init__.py
+-rw-r--r--   0        0        0     6039 2023-04-15 14:33:53.104115 anomalearn-0.0.2/anomalearn/algorithms/algo_functions.py
+-rw-r--r--   0        0        0     3976 2023-04-15 14:33:53.103114 anomalearn-0.0.2/anomalearn/algorithms/BaseModel.py
+-rw-r--r--   0        0        0     1012 2023-04-15 14:30:39.234325 anomalearn-0.0.2/anomalearn/algorithms/IBoundaryClassifier.py
+-rw-r--r--   0        0        0     1092 2023-04-15 14:33:53.102114 anomalearn-0.0.2/anomalearn/algorithms/IClassifier.py
+-rw-r--r--   0        0        0      973 2023-04-15 14:30:39.264332 anomalearn-0.0.2/anomalearn/algorithms/ICluster.py
+-rw-r--r--   0        0        0      395 2023-04-15 14:33:53.101115 anomalearn-0.0.2/anomalearn/algorithms/ICopyable.py
+-rw-r--r--   0        0        0     1489 2023-04-15 14:30:39.293340 anomalearn-0.0.2/anomalearn/algorithms/IMultipleParametric.py
+-rw-r--r--   0        0        0     1203 2023-04-15 14:30:39.310342 anomalearn-0.0.2/anomalearn/algorithms/IParametric.py
+-rw-r--r--   0        0        0     1082 2023-04-15 14:30:39.324346 anomalearn-0.0.2/anomalearn/algorithms/IPredictor.py
+-rw-r--r--   0        0        0     1192 2023-04-15 14:30:39.341351 anomalearn-0.0.2/anomalearn/algorithms/IProbabilisticClassifier.py
+-rw-r--r--   0        0        0     1010 2023-04-15 14:30:39.357354 anomalearn-0.0.2/anomalearn/algorithms/IRegressor.py
+-rw-r--r--   0        0        0     1748 2023-04-15 14:33:53.100115 anomalearn-0.0.2/anomalearn/algorithms/ISavable.py
+-rw-r--r--   0        0        0     1579 2023-04-15 14:30:39.395362 anomalearn-0.0.2/anomalearn/algorithms/IShapeChanger.py
+-rw-r--r--   0        0        0      916 2023-04-15 14:30:39.409365 anomalearn-0.0.2/anomalearn/algorithms/ITransformer.py
+-rw-r--r--   0        0        0       76 2023-04-15 14:33:53.100115 anomalearn-0.0.2/anomalearn/algorithms/models/__init__.py
+-rw-r--r--   0        0        0     1068 2023-04-15 14:33:53.099113 anomalearn-0.0.2/anomalearn/algorithms/models/IAnomalyScorer.py
+-rw-r--r--   0        0        0       79 2023-04-15 14:33:53.015093 anomalearn-0.0.2/anomalearn/algorithms/models/machine_learning/__init__.py
+-rw-r--r--   0        0        0    15870 2023-04-20 15:06:33.533610 anomalearn-0.0.2/anomalearn/algorithms/models/machine_learning/IsolationForest.py
+-rw-r--r--   0        0        0       16 2023-04-15 14:33:53.011094 anomalearn-0.0.2/anomalearn/algorithms/models/neural/__init__.py
+-rw-r--r--   0        0        0       16 2023-04-15 14:33:53.010093 anomalearn-0.0.2/anomalearn/algorithms/models/statistical/__init__.py
+-rw-r--r--   0        0        0      380 2023-04-15 14:33:53.009093 anomalearn-0.0.2/anomalearn/algorithms/pipelines/__init__.py
+-rw-r--r--   0        0        0      175 2023-04-15 14:30:39.695429 anomalearn-0.0.2/anomalearn/algorithms/pipelines/AbstractPipelineBaseLayer.py
+-rw-r--r--   0        0        0      181 2023-04-15 14:30:39.706431 anomalearn-0.0.2/anomalearn/algorithms/pipelines/AbstractPipelineSavableLayer.py
+-rw-r--r--   0        0        0     8971 2023-04-15 14:33:53.008091 anomalearn-0.0.2/anomalearn/algorithms/pipelines/IPipeline.py
+-rw-r--r--   0        0        0     3407 2023-04-20 15:11:58.781237 anomalearn-0.0.2/anomalearn/algorithms/pipelines/IPipelineLayer.py
+-rw-r--r--   0        0        0    34689 2023-04-15 14:33:53.006092 anomalearn-0.0.2/anomalearn/algorithms/pipelines/Pipeline.py
+-rw-r--r--   0        0        0      670 2023-04-15 14:33:53.005093 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/__init__.py
+-rw-r--r--   0        0        0     2432 2023-04-15 14:33:53.003091 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/BuilderErrorVectorsAbsDifference.py
+-rw-r--r--   0        0        0     2394 2023-04-15 14:33:53.002090 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/BuilderErrorVectorsDifference.py
+-rw-r--r--   0        0        0     2492 2023-04-15 14:33:53.001090 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/BuilderErrorVectorsNorm.py
+-rw-r--r--   0        0        0     7373 2023-04-15 14:33:53.001090 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/BuilderVectorsSlidingWindow.py
+-rw-r--r--   0        0        0     7362 2023-04-15 14:33:53.000090 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/ScorerGaussian.py
+-rw-r--r--   0        0        0     8187 2023-04-15 14:33:52.999091 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/ScorerMahalanobis.py
+-rw-r--r--   0        0        0     4243 2023-04-15 14:33:52.998090 anomalearn-0.0.2/anomalearn/algorithms/postprocessing/ThresholdMaxOnNormal.py
+-rw-r--r--   0        0        0      189 2023-04-15 14:33:52.997090 anomalearn-0.0.2/anomalearn/algorithms/preprocessing/__init__.py
+-rw-r--r--   0        0        0     5781 2023-04-15 14:33:52.997090 anomalearn-0.0.2/anomalearn/algorithms/preprocessing/SlidingWindowForecast.py
+-rw-r--r--   0        0        0     5128 2023-04-15 14:33:52.996090 anomalearn-0.0.2/anomalearn/algorithms/preprocessing/SlidingWindowReconstruct.py
+-rw-r--r--   0        0        0     2615 2023-04-20 15:11:56.274979 anomalearn-0.0.2/anomalearn/algorithms/SavableModel.py
+-rw-r--r--   0        0        0      132 2023-04-15 14:33:52.995090 anomalearn-0.0.2/anomalearn/algorithms/transformers/__init__.py
+-rw-r--r--   0        0        0     8482 2023-04-15 14:33:52.994090 anomalearn-0.0.2/anomalearn/algorithms/transformers/MinMaxScaler.py
+-rw-r--r--   0        0        0     8205 2023-04-15 14:33:52.993090 anomalearn-0.0.2/anomalearn/algorithms/transformers/StandardScaler.py
+-rw-r--r--   0        0        0       82 2023-04-15 14:33:52.993090 anomalearn-0.0.2/anomalearn/algorithms/tuning/__init__.py
+-rw-r--r--   0        0        0      759 2023-04-15 14:33:52.992089 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/__init__.py
+-rw-r--r--   0        0        0     1545 2023-04-15 14:33:52.991088 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/ForestSearch.py
+-rw-r--r--   0        0        0     1509 2023-04-15 14:33:52.990089 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/GaussianProcessesSearch.py
+-rw-r--r--   0        0        0     1532 2023-04-15 14:33:52.990089 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/GBRTSearch.py
+-rw-r--r--   0        0        0    15475 2023-04-15 14:33:52.989089 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/HyperparameterSearch.py
+-rw-r--r--   0        0        0     2681 2023-04-15 14:33:52.988090 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/HyperparameterSearchResults.py
+-rw-r--r--   0        0        0     5871 2023-04-15 14:33:52.987089 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/IHyperparameterSearch.py
+-rw-r--r--   0        0        0     2242 2023-04-15 14:33:52.987089 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/IHyperparameterSearchResults.py
+-rw-r--r--   0        0        0     7326 2023-04-15 14:33:52.986088 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/SkoptSearchABC.py
+-rw-r--r--   0        0        0     3694 2023-04-15 14:33:52.985087 anomalearn-0.0.2/anomalearn/algorithms/tuning/hyperparameter/TimeSeriesGridSearch.py
+-rw-r--r--   0        0        0     1781 2023-04-15 14:33:52.984087 anomalearn-0.0.2/anomalearn/algorithms/tuning/ICrossValidation.py
+-rw-r--r--   0        0        0      547 2023-04-15 14:33:52.984087 anomalearn-0.0.2/anomalearn/analysis/__init__.py
+-rw-r--r--   0        0        0    39539 2023-04-15 14:33:52.983087 anomalearn-0.0.2/anomalearn/analysis/dataset_simplicity.py
+-rw-r--r--   0        0        0     2199 2023-04-15 14:14:56.521712 anomalearn-0.0.2/anomalearn/analysis/decomposition.py
+-rw-r--r--   0        0        0     2069 2023-04-14 16:12:24.025662 anomalearn-0.0.2/anomalearn/analysis/stationarity.py
+-rw-r--r--   0        0        0     2104 2023-04-15 14:33:52.982087 anomalearn-0.0.2/anomalearn/applications/__init__.py
+-rw-r--r--   0        0        0    18318 2023-04-15 14:33:52.981087 anomalearn-0.0.2/anomalearn/applications/ExperimentLoader.py
+-rw-r--r--   0        0        0     7679 2023-04-15 14:33:52.979086 anomalearn-0.0.2/anomalearn/applications/IExperimentLoader.py
+-rw-r--r--   0        0        0      582 2023-04-15 14:33:52.978087 anomalearn-0.0.2/anomalearn/exceptions/__init__.py
+-rw-r--r--   0        0        0      258 2023-04-15 14:33:52.978087 anomalearn-0.0.2/anomalearn/exceptions/ClosedOpenRangeError.py
+-rw-r--r--   0        0        0      248 2023-04-15 14:33:52.977086 anomalearn-0.0.2/anomalearn/exceptions/ClosedRangeError.py
+-rw-r--r--   0        0        0      504 2023-04-15 14:33:52.976084 anomalearn-0.0.2/anomalearn/exceptions/InvalidInputShape.py
+-rw-r--r--   0        0        0      419 2023-04-15 14:33:52.976084 anomalearn-0.0.2/anomalearn/exceptions/NotTrainedError.py
+-rw-r--r--   0        0        0      258 2023-04-15 14:33:52.975084 anomalearn-0.0.2/anomalearn/exceptions/OpenClosedRangeError.py
+-rw-r--r--   0        0        0      246 2023-04-15 14:33:52.974084 anomalearn-0.0.2/anomalearn/exceptions/OpenRangeError.py
+-rw-r--r--   0        0        0      653 2023-04-15 14:33:52.974084 anomalearn-0.0.2/anomalearn/exceptions/RangeError.py
+-rw-r--r--   0        0        0      446 2023-04-15 14:33:52.973085 anomalearn-0.0.2/anomalearn/exceptions/SelectionError.py
+-rw-r--r--   0        0        0      620 2023-04-15 14:33:52.972085 anomalearn-0.0.2/anomalearn/input_validation/__init__.py
+-rw-r--r--   0        0        0     5598 2023-04-15 14:33:52.971085 anomalearn-0.0.2/anomalearn/input_validation/array_checks.py
+-rw-r--r--   0        0        0     5525 2023-04-15 14:33:52.971085 anomalearn-0.0.2/anomalearn/input_validation/attribute_checks.py
+-rw-r--r--   0        0        0      641 2023-04-15 14:30:42.900145 anomalearn-0.0.2/anomalearn/input_validation/colors.py
+-rw-r--r--   0        0        0     1100 2023-04-15 14:33:52.970084 anomalearn-0.0.2/anomalearn/reader/__init__.py
+-rw-r--r--   0        0        0     3484 2023-04-15 14:33:52.969085 anomalearn-0.0.2/anomalearn/reader/IDataMultipleReader.py
+-rw-r--r--   0        0        0     2368 2023-04-15 14:33:52.968086 anomalearn-0.0.2/anomalearn/reader/IDataReader.py
+-rw-r--r--   0        0        0      271 2023-04-15 14:30:43.090189 anomalearn-0.0.2/anomalearn/reader/IDatasetReader.py
+-rw-r--r--   0        0        0      885 2023-04-16 17:09:40.912583 anomalearn-0.0.2/anomalearn/reader/time_series/__init__.py
+-rw-r--r--   0        0        0      408 2023-04-17 13:01:37.758606 anomalearn-0.0.2/anomalearn/reader/time_series/config.py
+-rw-r--r--   0        0        0     8449 2023-04-16 17:09:40.638522 anomalearn-0.0.2/anomalearn/reader/time_series/ExathlonReader.py
+-rw-r--r--   0        0        0     4864 2023-04-16 17:09:40.788556 anomalearn-0.0.2/anomalearn/reader/time_series/GHLReader.py
+-rw-r--r--   0        0        0     4747 2023-04-16 17:09:40.764551 anomalearn-0.0.2/anomalearn/reader/time_series/KitsuneReader.py
+-rw-r--r--   0        0        0     2718 2023-04-16 17:09:40.890578 anomalearn-0.0.2/anomalearn/reader/time_series/MGABReader.py
+-rw-r--r--   0        0        0     5812 2023-04-16 17:09:40.813561 anomalearn-0.0.2/anomalearn/reader/time_series/NABReader.py
+-rw-r--r--   0        0        0     5929 2023-04-16 17:09:40.734544 anomalearn-0.0.2/anomalearn/reader/time_series/NASAReader.py
+-rw-r--r--   0        0        0     9343 2023-04-16 17:09:40.839567 anomalearn-0.0.2/anomalearn/reader/time_series/ODINTSReader.py
+-rw-r--r--   0        0        0     6913 2023-04-16 17:09:40.702537 anomalearn-0.0.2/anomalearn/reader/time_series/SMDReader.py
+-rw-r--r--   0        0        0      169 2023-04-14 14:11:01.637522 anomalearn-0.0.2/anomalearn/reader/time_series/time_series_config.ini
+-rw-r--r--   0        0        0     1189 2023-04-15 14:33:52.960083 anomalearn-0.0.2/anomalearn/reader/time_series/TSBenchmarkReader.py
+-rw-r--r--   0        0        0     2671 2023-04-15 14:33:52.959082 anomalearn-0.0.2/anomalearn/reader/time_series/TSMultipleReader.py
+-rw-r--r--   0        0        0     2136 2023-04-14 20:40:00.670307 anomalearn-0.0.2/anomalearn/reader/time_series/TSReader.py
+-rw-r--r--   0        0        0     4375 2023-04-20 15:54:43.108502 anomalearn-0.0.2/anomalearn/reader/time_series/UCRReader.py
+-rw-r--r--   0        0        0     5177 2023-04-16 17:09:40.671529 anomalearn-0.0.2/anomalearn/reader/time_series/YahooS5Reader.py
+-rw-r--r--   0        0        0     1212 2023-04-15 14:33:52.959082 anomalearn-0.0.2/anomalearn/utils/__init__.py
+-rw-r--r--   0        0        0      728 2023-04-15 14:30:44.353470 anomalearn-0.0.2/anomalearn/utils/arrays.py
+-rw-r--r--   0        0        0     2416 2023-04-15 14:33:52.958082 anomalearn-0.0.2/anomalearn/utils/estimation.py
+-rw-r--r--   0        0        0      857 2023-04-15 14:33:52.957082 anomalearn-0.0.2/anomalearn/utils/filesystem.py
+-rw-r--r--   0        0        0     1207 2023-04-15 14:33:52.956081 anomalearn-0.0.2/anomalearn/utils/json.py
+-rw-r--r--   0        0        0     1469 2023-04-15 14:33:52.955081 anomalearn-0.0.2/anomalearn/utils/lists.py
+-rw-r--r--   0        0        0     5751 2023-04-15 14:33:52.954083 anomalearn-0.0.2/anomalearn/utils/metrics.py
+-rw-r--r--   0        0        0     3534 2023-04-15 14:30:44.562517 anomalearn-0.0.2/anomalearn/utils/moving_functions.py
+-rw-r--r--   0        0        0     1978 2023-04-15 14:33:52.953081 anomalearn-0.0.2/anomalearn/utils/numpy.py
+-rw-r--r--   0        0        0     8591 2023-04-15 14:33:52.952082 anomalearn-0.0.2/anomalearn/utils/scikit.py
+-rw-r--r--   0        0        0      490 2023-04-15 14:33:52.951080 anomalearn-0.0.2/anomalearn/visualizer/__init__.py
+-rw-r--r--   0        0        0     7860 2023-04-15 14:33:52.950079 anomalearn-0.0.2/anomalearn/visualizer/bar_plots.py
+-rw-r--r--   0        0        0     4949 2023-04-15 14:33:52.950079 anomalearn-0.0.2/anomalearn/visualizer/box_plots.py
+-rw-r--r--   0        0        0    29454 2023-04-15 14:33:52.949080 anomalearn-0.0.2/anomalearn/visualizer/line_plots.py
+-rw-r--r--   0        0        0     6882 2023-04-15 14:33:52.948080 anomalearn-0.0.2/anomalearn/visualizer/pie_plots.py
+-rw-r--r--   0        0        0    11563 2023-04-15 14:33:52.947081 anomalearn-0.0.2/anomalearn/visualizer/scatter_plots.py
+-rw-r--r--   0        0        0      192 2023-04-15 14:33:52.946079 anomalearn-0.0.2/anomalearn/visualizer/time_series/__init__.py
+-rw-r--r--   0        0        0     3738 2023-04-15 14:33:52.945082 anomalearn-0.0.2/anomalearn/visualizer/time_series/correlation.py
+-rw-r--r--   0        0        0     3736 2023-04-15 14:33:52.945082 anomalearn-0.0.2/anomalearn/visualizer/time_series/decomposition.py
+-rw-r--r--   0        0        0    14112 2023-04-14 14:11:01.514495 anomalearn-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2157 2023-04-29 15:13:21.620405 anomalearn-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8454 2023-04-29 15:12:43.980486 anomalearn-0.0.2/README.md
+-rw-r--r--   0        0        0     9907 1970-01-01 00:00:00.000000 anomalearn-0.0.2/PKG-INFO
```

