# Comparing `tmp/getdaft-0.0.9.tar.gz` & `tmp/getdaft-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getdaft-0.0.9.tar", max compression
+gzip compressed data
```

## Comparing `getdaft-0.0.9.tar` & `getdaft-0.1.0.tar`

### file list

```diff
@@ -1,67 +1,431 @@
--rw-r--r--   0        0        0    11357 2022-09-10 05:06:43.603694 getdaft-0.0.9/LICENSE
--rw-r--r--   0        0        0      409 2022-09-10 05:06:43.607694 getdaft-0.0.9/README.md
--rw-r--r--   0        0        0     2930 2022-09-10 05:06:43.607694 getdaft-0.0.9/build.py
--rw-r--r--   0        0        0      211 2022-09-10 05:07:52.448822 getdaft-0.0.9/daft/__init__.py
--rw-r--r--   0        0        0      483 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/config.py
--rw-r--r--   0        0        0       58 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/dataframe/__init__.py
--rw-r--r--   0        0        0    24700 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/dataframe/dataframe.py
--rw-r--r--   0        0        0     1617 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/dataframe/schema.py
--rw-r--r--   0        0        0     1487 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/datasources.py
--rw-r--r--   0        0        0        0 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/execution/__init__.py
--rw-r--r--   0        0        0     3282 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/execution/execution_plan.py
--rw-r--r--   0        0        0    12273 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/execution/logical_op_runners.py
--rw-r--r--   0        0        0    13477 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/execution/operators.py
--rw-r--r--   0        0        0     1651 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/execution/url_operators.py
--rw-r--r--   0        0        0        0 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/__init__.py
--rw-r--r--   0        0        0     3897 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/dataclasses.py
--rw-r--r--   0        0        0      102 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/datarepo/__init__.py
--rw-r--r--   0        0        0     1762 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/datarepo/client.py
--rw-r--r--   0        0        0     1046 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/datarepo/datarepo.py
--rw-r--r--   0        0        0      847 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/fields.py
--rw-r--r--   0        0        0    10351 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/schema.py
--rw-r--r--   0        0        0       76 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/__init__.py
--rw-r--r--   0        0        0     2743 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/backend.py
--rw-r--r--   0        0        0      151 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/backends/__init__.py
--rw-r--r--   0        0        0    11003 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/backends/aws_lambda.py
--rw-r--r--   0        0        0     8285 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/backends/docker.py
--rw-r--r--   0        0        0     6026 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/backends/multiprocessing.py
--rw-r--r--   0        0        0      118 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/definitions.py
--rw-r--r--   0        0        0     1846 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/endpoint.py
--rw-r--r--   0        0        0     2590 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/env.py
--rw-r--r--   0        0        0     1902 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/static/Dockerfile.aws_lambda
--rw-r--r--   0        0        0        0 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/static/__init__.py
--rw-r--r--   0        0        0      275 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/static/aws-lambda-entrypoint.py
--rw-r--r--   0        0        0      597 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/static/docker-entrypoint.py
--rw-r--r--   0        0        0      648 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/serving/static/multiprocessing-entrypoint.py
--rw-r--r--   0        0        0     2086 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/experimental/types.py
--rw-r--r--   0        0        0    24869 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/expressions.py
--rw-r--r--   0        0        0      600 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/filesystem.py
--rw-r--r--   0        0        0        0 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/__init__.py
--rw-r--r--   0        0        0      473 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/gpu.py
--rw-r--r--   0        0        0      197 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/hashing.pyd
--rw-r--r--   0        0        0     6661 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/hashing.pyx
--rw-r--r--   0        0        0     1545 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/rule.py
--rw-r--r--   0        0        0     1991 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/rule_runner.py
--rw-r--r--   0        0        0     3189 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/treenode.py
--rw-r--r--   0        0        0     1855 2022-09-10 05:06:43.607694 getdaft-0.0.9/daft/internal/xxhash.cc
--rw-r--r--   0        0        0   228839 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/internal/xxhash.h
--rw-r--r--   0        0        0      230 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/logging.py
--rw-r--r--   0        0        0        0 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/logical/__init__.py
--rw-r--r--   0        0        0    21417 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/logical/logical_plan.py
--rw-r--r--   0        0        0     7176 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/logical/optimizer.py
--rw-r--r--   0        0        0     5453 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/logical/schema.py
--rw-r--r--   0        0        0     1445 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/resource_request.py
--rw-r--r--   0        0        0        0 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/__init__.py
--rw-r--r--   0        0        0    28508 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/blocks.py
--rw-r--r--   0        0        0    15379 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/partitioning.py
--rw-r--r--   0        0        0      970 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/profiler.py
--rw-r--r--   0        0        0     7991 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/pyrunner.py
--rw-r--r--   0        0        0     9843 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/ray_runner.py
--rw-r--r--   0        0        0      235 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/runner.py
--rw-r--r--   0        0        0     4357 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/runners/shuffle_ops.py
--rw-r--r--   0        0        0     3915 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/udf.py
--rw-r--r--   0        0        0       80 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/viz/__init__.py
--rw-r--r--   0        0        0     2844 2022-09-10 05:06:43.611694 getdaft-0.0.9/daft/viz/dataframe_display.py
--rw-r--r--   0        0        0     3609 2022-09-10 05:07:52.444822 getdaft-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2498 1970-01-01 00:00:00.000000 getdaft-0.0.9/setup.py
--rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 getdaft-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      985 1970-01-01 00:00:00.000000 getdaft-0.1.0/Cargo.toml
+-rw-r--r--   0      501       20      834 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0      501       20      595 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0      501       20     1333 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/broken-link-checker.yml
+-rw-r--r--   0      501       20     3378 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/daft-profiling.yml
+-rw-r--r--   0      501       20     1627 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/notebook-checker.yml
+-rw-r--r--   0      501       20     2194 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/property-based-tests.yml
+-rw-r--r--   0      501       20    12537 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0      501       20     6168 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0      501       20     2638 2023-04-29 00:27:26.000000 getdaft-0.1.0/.github/workflows/ray-compatibility.yml
+-rw-r--r--   0      501       20      300 2023-04-29 00:27:26.000000 getdaft-0.1.0/.gitignore
+-rw-r--r--   0      501       20     2126 2023-04-29 00:27:26.000000 getdaft-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0      501       20      205 2023-04-29 00:27:26.000000 getdaft-0.1.0/.readthedocs.yaml
+-rw-r--r--   0      501       20     1550 2023-04-29 00:27:26.000000 getdaft-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0      501       20    11357 2023-04-29 00:27:26.000000 getdaft-0.1.0/LICENSE
+-rw-r--r--   0      501       20     1295 2023-04-29 00:27:26.000000 getdaft-0.1.0/Makefile
+-rw-r--r--   0      501       20     6094 2023-04-29 00:27:26.000000 getdaft-0.1.0/README.rst
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/benchmarking/__init__.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/benchmarking/tpch/__init__.py
+-rw-r--r--   0      501       20     9495 2023-04-29 00:27:26.000000 getdaft-0.1.0/benchmarking/tpch/__main__.py
+-rw-r--r--   0      501       20    12428 2023-04-29 00:27:26.000000 getdaft-0.1.0/benchmarking/tpch/answers.py
+-rw-r--r--   0      501       20    12140 2023-04-29 00:27:26.000000 getdaft-0.1.0/benchmarking/tpch/data_generation.py
+-rw-r--r--   0      501       20     4573 2023-04-29 00:27:26.000000 getdaft-0.1.0/benchmarking/tpch/pipelined_data_generation.py
+-rw-r--r--   0      501       20     1436 2023-04-29 00:27:26.000000 getdaft-0.1.0/ci/upload_wheels.sh
+-rw-r--r--   0      501       20      440 2023-04-29 00:27:26.000000 getdaft-0.1.0/codecov.yml
+-rw-r--r--   0      501       20     2092 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/__init__.py
+-rw-r--r--   0      501       20     6724 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/analytics.py
+-rw-r--r--   0      501       20     3935 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/api_annotations.py
+-rw-r--r--   0      501       20    10592 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/arrow_utils.py
+-rw-r--r--   0      501       20     6182 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/context.py
+-rw-r--r--   0      501       20     3403 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/convert.py
+-rw-r--r--   0      501       20       94 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/dataframe/__init__.py
+-rw-r--r--   0      501       20    49422 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/dataframe/dataframe.py
+-rw-r--r--   0      501       20      306 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/dataframe/preview.py
+-rw-r--r--   0      501       20      850 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/datasources.py
+-rw-r--r--   0      501       20     7213 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/datatype.py
+-rw-r--r--   0      501       20       84 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/errors.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/execution/__init__.py
+-rw-r--r--   0      501       20    24879 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/execution/execution_step.py
+-rw-r--r--   0      501       20     4116 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/execution/logical_op_runners.py
+-rw-r--r--   0      501       20    27790 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/execution/physical_plan.py
+-rw-r--r--   0      501       20     6110 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/execution/physical_plan_factory.py
+-rw-r--r--   0      501       20      170 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/expressions/__init__.py
+-rw-r--r--   0      501       20    23774 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/expressions/expressions.py
+-rw-r--r--   0      501       20      572 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/expressions/testing.py
+-rw-r--r--   0      501       20     5328 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/filesystem.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/internal/__init__.py
+-rw-r--r--   0      501       20      509 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/internal/gpu.py
+-rw-r--r--   0      501       20     1804 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/internal/rule.py
+-rw-r--r--   0      501       20     1965 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/internal/rule_runner.py
+-rw-r--r--   0      501       20     3490 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/internal/treenode.py
+-rw-r--r--   0      501       20      263 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/io/__init__.py
+-rw-r--r--   0      501       20     1428 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/io/_csv.py
+-rw-r--r--   0      501       20      951 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/io/_json.py
+-rw-r--r--   0      501       20     1952 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/io/common.py
+-rw-r--r--   0      501       20     1742 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/io/file_path.py
+-rw-r--r--   0      501       20      964 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/io/parquet.py
+-rw-r--r--   0      501       20      264 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logging.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logical/__init__.py
+-rw-r--r--   0      501       20     8601 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logical/aggregation_plan_builder.py
+-rw-r--r--   0      501       20    37523 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logical/logical_plan.py
+-rw-r--r--   0      501       20     1492 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logical/map_partition_ops.py
+-rw-r--r--   0      501       20    19131 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logical/optimizer.py
+-rw-r--r--   0      501       20     3531 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/logical/schema.py
+-rw-r--r--   0      501       20       99 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/pickle/__init__.py
+-rw-r--r--   0      501       20    34760 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/pickle/cloudpickle.py
+-rw-r--r--   0      501       20    34262 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/pickle/cloudpickle_fast.py
+-rw-r--r--   0      501       20      639 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/pickle/compat.py
+-rw-r--r--   0      501       20      312 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/pickle/pickle.py
+-rw-r--r--   0      501       20     2036 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/resource_request.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/__init__.py
+-rw-r--r--   0      501       20     5708 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/partitioning.py
+-rw-r--r--   0      501       20     1488 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/profiler.py
+-rw-r--r--   0      501       20    12834 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/pyrunner.py
+-rw-r--r--   0      501       20    26116 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/ray_runner.py
+-rw-r--r--   0      501       20      918 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/runner.py
+-rw-r--r--   0      501       20     3991 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/runners/runner_io.py
+-rw-r--r--   0      501       20    18192 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/series.py
+-rw-r--r--   0      501       20       82 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/table/__init__.py
+-rw-r--r--   0      501       20    12759 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/table/table.py
+-rw-r--r--   0      501       20     8761 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/table/table_io.py
+-rw-r--r--   0      501       20     7263 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/udf.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/udf_library/__init__.py
+-rw-r--r--   0      501       20     1579 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/udf_library/url_udfs.py
+-rw-r--r--   0      501       20     2697 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/utils.py
+-rw-r--r--   0      501       20      183 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/viz/__init__.py
+-rw-r--r--   0      501       20     1699 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/viz/dataframe_display.py
+-rw-r--r--   0      501       20     1517 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/viz/html_viz_hooks.py
+-rw-r--r--   0      501       20     5738 2023-04-29 00:27:26.000000 getdaft-0.1.0/daft/viz/repr.py
+-rw-r--r--   0      501       20      148 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/CONTRIBUTING.md
+-rw-r--r--   0      501       20      638 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/Makefile
+-rw-r--r--   0      501       20    71672 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/10-min.ipynb
+-rw-r--r--   0      501       20      389 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/custom-function-signatures.css
+-rw-r--r--   0      501       20      565 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/daft-favicon.png
+-rw-r--r--   0      501       20     7804 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/daft-logo.png
+-rw-r--r--   0      501       20    42148 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/daft_illustration.png
+-rw-r--r--   0      501       20     1901 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/header.css
+-rw-r--r--   0      501       20      343 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/icon-menu-close.svg
+-rw-r--r--   0      501       20      333 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/icon-menu-dots.svg
+-rw-r--r--   0      501       20      786 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_static/mobile-menu.js
+-rw-r--r--   0      501       20      856 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_templates/layout.html
+-rw-r--r--   0      501       20      994 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_templates/sections/header.html
+-rw-r--r--   0      501       20      957 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/_templates/sections/mobile-menu.html
+-rw-r--r--   0      501       20      325 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/context.rst
+-rw-r--r--   0      501       20     2564 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/dataframe.rst
+-rw-r--r--   0      501       20     3444 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/expressions.rst
+-rw-r--r--   0      501       20      784 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/groupby.rst
+-rw-r--r--   0      501       20      124 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/index.rst
+-rw-r--r--   0      501       20     1457 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/input_output.rst
+-rw-r--r--   0      501       20       88 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/api_docs/udf.rst
+-rw-r--r--   0      501       20     3547 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/conf.py
+-rw-r--r--   0      501       20     4964 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/dataframe_comparison.rst
+-rw-r--r--   0      501       20     1619 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/index.rst
+-rw-r--r--   0      501       20     1089 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/install.rst
+-rw-r--r--   0      501       20      743 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/index.rst
+-rw-r--r--   0      501       20     7586 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/key_concepts.rst
+-rw-r--r--   0      501       20     1398 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/tutorials.rst
+-rw-r--r--   0      501       20     1388 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/aggregations.rst
+-rw-r--r--   0      501       20     6686 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/dataframe-operations.rst
+-rw-r--r--   0      501       20     9024 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/expressions.rst
+-rw-r--r--   0      501       20     7829 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/intro-dataframes.rst
+-rw-r--r--   0      501       20      206 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/partitioning.rst
+-rw-r--r--   0      501       20     3190 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/read-write.rst
+-rw-r--r--   0      501       20     1257 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/scaling-up.rst
+-rw-r--r--   0      501       20     8689 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides/udf.rst
+-rw-r--r--   0      501       20     1551 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/learn/user_guides.rst
+-rw-r--r--   0      501       20     3575 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.13.rst
+-rw-r--r--   0      501       20     2241 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.14.rst
+-rw-r--r--   0      501       20     1913 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.16.rst
+-rw-r--r--   0      501       20     1750 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.17.rst
+-rw-r--r--   0      501       20     2100 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.18.rst
+-rw-r--r--   0      501       20     3647 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.19.rst
+-rw-r--r--   0      501       20     4240 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.20.rst
+-rw-r--r--   0      501       20     4633 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.21.rst
+-rw-r--r--   0      501       20     8016 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.22.rst
+-rw-r--r--   0      501       20     5385 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.23.rst
+-rw-r--r--   0      501       20    11759 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.0.24.rst
+-rw-r--r--   0      501       20     4750 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/0.1.0.rst
+-rw-r--r--   0      501       20      935 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/_template.rst
+-rw-r--r--   0      501       20      293 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/release_notes/index.rst
+-rw-r--r--   0      501       20     1316 2023-04-29 00:27:26.000000 getdaft-0.1.0/docs/source/telemetry.rst
+-rw-r--r--   0      501       20     1855 2023-04-29 00:27:26.000000 getdaft-0.1.0/pyproject.toml
+-rw-r--r--   0      501       20      397 2023-04-29 00:27:26.000000 getdaft-0.1.0/requirements-dev.txt
+-rw-r--r--   0      501       20       98 2023-04-29 00:27:26.000000 getdaft-0.1.0/rust-toolchain.toml
+-rw-r--r--   0      501       20     4411 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/from.rs
+-rw-r--r--   0      501       20      739 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/iterator.rs
+-rw-r--r--   0      501       20     3605 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/mod.rs
+-rw-r--r--   0      501       20      257 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/abs.rs
+-rw-r--r--   0      501       20      754 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/apply.rs
+-rw-r--r--   0      501       20      841 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arange.rs
+-rw-r--r--   0      501       20     6982 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arithmetic.rs
+-rw-r--r--   0      501       20     3038 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/comparison.rs
+-rw-r--r--   0      501       20       34 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/mod.rs
+-rw-r--r--   0      501       20       19 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/sort/mod.rs
+-rw-r--r--   0      501       20     3482 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/sort/primitive/common.rs
+-rw-r--r--   0      501       20      723 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/sort/primitive/indices.rs
+-rw-r--r--   0      501       20       47 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/sort/primitive/mod.rs
+-rw-r--r--   0      501       20     7664 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/arrow2/sort/primitive/sort.rs
+-rw-r--r--   0      501       20    10724 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/broadcast.rs
+-rw-r--r--   0      501       20     4109 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/cast.rs
+-rw-r--r--   0      501       20     9890 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/compare_agg.rs
+-rw-r--r--   0      501       20    47236 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/comparison.rs
+-rw-r--r--   0      501       20     1782 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/concat.rs
+-rw-r--r--   0      501       20     5819 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/concat_agg.rs
+-rw-r--r--   0      501       20     1429 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/count.rs
+-rw-r--r--   0      501       20      948 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/date.rs
+-rw-r--r--   0      501       20     2623 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/downcast.rs
+-rw-r--r--   0      501       20     4264 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/filter.rs
+-rw-r--r--   0      501       20     1301 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/float.rs
+-rw-r--r--   0      501       20     1300 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/full.rs
+-rw-r--r--   0      501       20     4117 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/groups.rs
+-rw-r--r--   0      501       20     1550 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/hash.rs
+-rw-r--r--   0      501       20    11122 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/if_else.rs
+-rw-r--r--   0      501       20     1191 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/len.rs
+-rw-r--r--   0      501       20     4506 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/list.rs
+-rw-r--r--   0      501       20     3378 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/list_agg.rs
+-rw-r--r--   0      501       20     1627 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/mean.rs
+-rw-r--r--   0      501       20     2595 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/mod.rs
+-rw-r--r--   0      501       20     1153 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/null.rs
+-rw-r--r--   0      501       20     3837 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/pairwise.rs
+-rw-r--r--   0      501       20      500 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/search_sorted.rs
+-rw-r--r--   0      501       20    17216 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/sort.rs
+-rw-r--r--   0      501       20     2388 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/sum.rs
+-rw-r--r--   0      501       20    11849 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/take.rs
+-rw-r--r--   0      501       20     5313 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/ops/utf8.rs
+-rw-r--r--   0      501       20      995 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/pseudo_arrow/compute.rs
+-rw-r--r--   0      501       20    13425 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/pseudo_arrow/mod.rs
+-rw-r--r--   0      501       20     2502 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/array/pseudo_arrow/python.rs
+-rw-r--r--   0      501       20     8951 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/datatypes/dtype.rs
+-rw-r--r--   0      501       20     1414 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/datatypes/field.rs
+-rw-r--r--   0      501       20     8267 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/datatypes/matching.rs
+-rw-r--r--   0      501       20     5816 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/datatypes/mod.rs
+-rw-r--r--   0      501       20     1083 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/datatypes/time_unit.rs
+-rw-r--r--   0      501       20      273 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/README.md
+-rw-r--r--   0      501       20     1474 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/arithmetic.rs
+-rw-r--r--   0      501       20    20798 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/expr.rs
+-rw-r--r--   0      501       20     1421 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/float/is_nan.rs
+-rw-r--r--   0      501       20      587 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/float/mod.rs
+-rw-r--r--   0      501       20     1112 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/list/explode.rs
+-rw-r--r--   0      501       20      597 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/list/mod.rs
+-rw-r--r--   0      501       20     1774 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/mod.rs
+-rw-r--r--   0      501       20     1178 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/numeric/abs.rs
+-rw-r--r--   0      501       20      580 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/numeric/mod.rs
+-rw-r--r--   0      501       20      676 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/python/mod.rs
+-rw-r--r--   0      501       20     2050 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/python/partial_udf.rs
+-rw-r--r--   0      501       20     2769 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/python/udf.rs
+-rw-r--r--   0      501       20     1339 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/temporal/day.rs
+-rw-r--r--   0      501       20     1367 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/temporal/day_of_week.rs
+-rw-r--r--   0      501       20     1425 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/temporal/mod.rs
+-rw-r--r--   0      501       20     1349 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/temporal/month.rs
+-rw-r--r--   0      501       20     1343 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/temporal/year.rs
+-rw-r--r--   0      501       20     1617 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/utf8/contains.rs
+-rw-r--r--   0      501       20     1617 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/utf8/endswith.rs
+-rw-r--r--   0      501       20     1336 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/utf8/length.rs
+-rw-r--r--   0      501       20     1524 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/utf8/mod.rs
+-rw-r--r--   0      501       20     1627 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/functions/utf8/startswith.rs
+-rw-r--r--   0      501       20     4959 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/lit.rs
+-rw-r--r--   0      501       20      233 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/mod.rs
+-rw-r--r--   0      501       20     5298 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/optimization.rs
+-rw-r--r--   0      501       20     1982 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/dsl/pyobject.rs
+-rw-r--r--   0      501       20     1428 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/error.rs
+-rw-r--r--   0      501       20     7735 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/ffi.rs
+-rw-r--r--   0      501       20     6022 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/kernels/hashing.rs
+-rw-r--r--   0      501       20       54 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/kernels/mod.rs
+-rw-r--r--   0      501       20    12159 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/kernels/search_sorted.rs
+-rw-r--r--   0      501       20     3917 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/kernels/utf8.rs
+-rw-r--r--   0      501       20     1050 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/lib.rs
+-rw-r--r--   0      501       20     4704 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/datatype.rs
+-rw-r--r--   0      501       20      307 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/error.rs
+-rw-r--r--   0      501       20    10179 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/expr.rs
+-rw-r--r--   0      501       20     1635 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/field.rs
+-rw-r--r--   0      501       20      701 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/mod.rs
+-rw-r--r--   0      501       20     2416 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/schema.rs
+-rw-r--r--   0      501       20     9035 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/series.rs
+-rw-r--r--   0      501       20    10114 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/python/table.rs
+-rw-r--r--   0      501       20     3016 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/schema.rs
+-rw-r--r--   0      501       20      674 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/from.rs
+-rw-r--r--   0      501       20     2235 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/mod.rs
+-rw-r--r--   0      501       20      879 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/abs.rs
+-rw-r--r--   0      501       20     6549 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/agg.rs
+-rw-r--r--   0      501       20     6303 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/arithmetic.rs
+-rw-r--r--   0      501       20     2563 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/broadcast.rs
+-rw-r--r--   0      501       20     6780 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/cast.rs
+-rw-r--r--   0      501       20     2609 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/comparison.rs
+-rw-r--r--   0      501       20     1139 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/concat.rs
+-rw-r--r--   0      501       20     1776 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/date.rs
+-rw-r--r--   0      501       20     7093 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/downcast.rs
+-rw-r--r--   0      501       20     1215 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/filter.rs
+-rw-r--r--   0      501       20      387 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/float.rs
+-rw-r--r--   0      501       20      344 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/full.rs
+-rw-r--r--   0      501       20      401 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/groups.rs
+-rw-r--r--   0      501       20      412 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/hash.rs
+-rw-r--r--   0      501       20     1006 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/if_else.rs
+-rw-r--r--   0      501       20      445 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/len.rs
+-rw-r--r--   0      501       20      901 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/list.rs
+-rw-r--r--   0      501       20     2072 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/mod.rs
+-rw-r--r--   0      501       20      461 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/not.rs
+-rw-r--r--   0      501       20      361 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/null.rs
+-rw-r--r--   0      501       20     1705 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/pairwise.rs
+-rw-r--r--   0      501       20      638 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/search_sorted.rs
+-rw-r--r--   0      501       20     1808 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/sort.rs
+-rw-r--r--   0      501       20     1738 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/take.rs
+-rw-r--r--   0      501       20     1514 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/series/ops/utf8.rs
+-rw-r--r--   0      501       20    16217 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/mod.rs
+-rw-r--r--   0      501       20     2154 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/agg.rs
+-rw-r--r--   0      501       20     3708 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/explode.rs
+-rw-r--r--   0      501       20     4408 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/groups.rs
+-rw-r--r--   0      501       20     2891 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/hash.rs
+-rw-r--r--   0      501       20     2451 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/joins/hash_join.rs
+-rw-r--r--   0      501       20     3728 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/joins/mod.rs
+-rw-r--r--   0      501       20      917 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/joins/naive_join.rs
+-rw-r--r--   0      501       20       99 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/mod.rs
+-rw-r--r--   0      501       20     3471 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/partition.rs
+-rw-r--r--   0      501       20     1600 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/search_sorted.rs
+-rw-r--r--   0      501       20      999 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/table/ops/sort.rs
+-rw-r--r--   0      501       20     4619 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/utils/arrow.rs
+-rw-r--r--   0      501       20       34 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/utils/mod.rs
+-rw-r--r--   0      501       20    10065 2023-04-29 00:27:26.000000 getdaft-0.1.0/src/utils/supertype.rs
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/__init__.py
+-rw-r--r--   0      501       20      299 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/__init__.py
+-rw-r--r--   0      501       20      544 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/1.sql
+-rw-r--r--   0      501       20      542 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/10.sql
+-rw-r--r--   0      501       20      703 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/2.sql
+-rw-r--r--   0      501       20      444 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/3.sql
+-rw-r--r--   0      501       20      371 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/4.sql
+-rw-r--r--   0      501       20      504 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/5.sql
+-rw-r--r--   0      501       20      259 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/6.sql
+-rw-r--r--   0      501       20      834 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/7.sql
+-rw-r--r--   0      501       20      815 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/8.sql
+-rw-r--r--   0      501       20      627 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/9.sql
+-rw-r--r--   0      501       20       48 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/assets/tpch-sqlite-queries/README.md
+-rw-r--r--   0      501       20      604 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/conftest.py
+-rw-r--r--   0      501       20     1241 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/test_df_arithmetic.py
+-rw-r--r--   0      501       20     1674 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/test_file_read.py
+-rw-r--r--   0      501       20     5592 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/test_groups_and_aggs.py
+-rw-r--r--   0      501       20     7280 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/test_join.py
+-rw-r--r--   0      501       20     2591 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/test_repartition.py
+-rw-r--r--   0      501       20     3993 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/benchmarks/test_sort.py
+-rw-r--r--   0      501       20     2324 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/__init__.py
+-rw-r--r--   0      501       20    13229 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/assets/311-service-requests.24.csv
+-rw-r--r--   0      501       20      255 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/assets/__init__.py
+-rw-r--r--   0      501       20      882 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/conftest.py
+-rw-r--r--   0      501       20     9268 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_aggregations.py
+-rw-r--r--   0      501       20     2979 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_computations.py
+-rw-r--r--   0      501       20     1798 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_count_rows.py
+-rw-r--r--   0      501       20     5608 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_dataloading.py
+-rw-r--r--   0      501       20      800 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_distinct.py
+-rw-r--r--   0      501       20     6049 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_filter.py
+-rw-r--r--   0      501       20     3810 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_joins.py
+-rw-r--r--   0      501       20     2878 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_literals.py
+-rw-r--r--   0      501       20    10311 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_pandas_cookbook.py
+-rw-r--r--   0      501       20     4149 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_sorting.py
+-rw-r--r--   0      501       20     1497 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/cookbook/test_write.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/__init__.py
+-rw-r--r--   0      501       20      751 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/conftest.py
+-rw-r--r--   0      501       20      805 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_accessors.py
+-rw-r--r--   0      501       20    10308 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_aggregations.py
+-rw-r--r--   0      501       20    12785 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_creation.py
+-rw-r--r--   0      501       20     1824 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_distinct.py
+-rw-r--r--   0      501       20     1428 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_explode.py
+-rw-r--r--   0      501       20     1097 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_filter.py
+-rw-r--r--   0      501       20     2435 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_getitem.py
+-rw-r--r--   0      501       20     4091 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_joins.py
+-rw-r--r--   0      501       20     4500 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_repr.py
+-rw-r--r--   0      501       20      815 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_select.py
+-rw-r--r--   0      501       20      656 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_show.py
+-rw-r--r--   0      501       20     6364 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_sort.py
+-rw-r--r--   0      501       20     2385 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_to_integrations.py
+-rw-r--r--   0      501       20      850 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/dataframe/test_with_column.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/__init__.py
+-rw-r--r--   0      501       20     1417 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/test_apply.py
+-rw-r--r--   0      501       20     3533 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/test_expressions.py
+-rw-r--r--   0      501       20     4259 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/test_expressions_projection.py
+-rw-r--r--   0      501       20     5019 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/test_udf.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/__init__.py
+-rw-r--r--   0      501       20     6290 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/conftest.py
+-rw-r--r--   0      501       20     1363 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_aggs.py
+-rw-r--r--   0      501       20     2335 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_arithmetic.py
+-rw-r--r--   0      501       20      853 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_compare.py
+-rw-r--r--   0      501       20      792 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_dt.py
+-rw-r--r--   0      501       20      531 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_float.py
+-rw-r--r--   0      501       20      684 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_if_else.py
+-rw-r--r--   0      501       20      422 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_is_null.py
+-rw-r--r--   0      501       20     1176 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_logical.py
+-rw-r--r--   0      501       20     1544 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/expressions/typing/test_str.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/integration/__init__.py
+-rw-r--r--   0      501       20     4193 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/integration/test_tpch.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/__init__.py
+-rw-r--r--   0      501       20     1116 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/conftest.py
+-rw-r--r--   0      501       20     1666 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_drop_projections.py
+-rw-r--r--   0      501       20     1847 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_drop_repartition.py
+-rw-r--r--   0      501       20     2463 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_fold_projections.py
+-rw-r--r--   0      501       20     7624 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_prune_columns.py
+-rw-r--r--   0      501       20     3456 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_pushdown_clauses_into_scan.py
+-rw-r--r--   0      501       20     1170 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_pushdown_limit.py
+-rw-r--r--   0      501       20     8453 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/optimizer/test_pushdown_predicates.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/property_based_testing/__init__.py
+-rw-r--r--   0      501       20     4575 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/property_based_testing/strategies.py
+-rw-r--r--   0      501       20     8895 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/property_based_testing/test_sort.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/ray/__init__.py
+-rw-r--r--   0      501       20     5375 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/ray/test_dask.py
+-rw-r--r--   0      501       20     8239 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/ray/test_datasets.py
+-rw-r--r--   0      501       20      278 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/__init__.py
+-rw-r--r--   0      501       20     9299 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_arithmetic.py
+-rw-r--r--   0      501       20     3377 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_cast.py
+-rw-r--r--   0      501       20    17207 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_comparisons.py
+-rw-r--r--   0      501       20     3759 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_concat.py
+-rw-r--r--   0      501       20     4591 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_filter.py
+-rw-r--r--   0      501       20      874 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_float.py
+-rw-r--r--   0      501       20     3344 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_hash.py
+-rw-r--r--   0      501       20    17239 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_if_else.py
+-rw-r--r--   0      501       20      889 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_numeric_ops.py
+-rw-r--r--   0      501       20     3418 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_series.py
+-rw-r--r--   0      501       20     6686 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_size_bytes.py
+-rw-r--r--   0      501       20     2188 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_slice.py
+-rw-r--r--   0      501       20     5495 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_sort.py
+-rw-r--r--   0      501       20     4015 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_take.py
+-rw-r--r--   0      501       20     1934 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_temporal_ops.py
+-rw-r--r--   0      501       20     4413 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/series/test_utf8_ops.py
+-rw-r--r--   0      501       20      694 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/__init__.py
+-rw-r--r--   0      501       20     1070 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_blackbox_kernels.py
+-rw-r--r--   0      501       20      426 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_broadcasts.py
+-rw-r--r--   0      501       20     2123 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_concat.py
+-rw-r--r--   0      501       20     4900 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_eval.py
+-rw-r--r--   0      501       20     3930 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_explodes.py
+-rw-r--r--   0      501       20     7413 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_filter.py
+-rw-r--r--   0      501       20    17426 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_from_py.py
+-rw-r--r--   0      501       20      842 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_head.py
+-rw-r--r--   0      501       20    10974 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_joins.py
+-rw-r--r--   0      501       20     7811 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_partitioning.py
+-rw-r--r--   0      501       20      654 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_size_bytes.py
+-rw-r--r--   0      501       20    10955 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_sorting.py
+-rw-r--r--   0      501       20    20923 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_table_aggs.py
+-rw-r--r--   0      501       20    10064 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_table_io.py
+-rw-r--r--   0      501       20     5061 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/test_take.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/utf8/__init__.py
+-rw-r--r--   0      501       20     1165 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/utf8/test_compares.py
+-rw-r--r--   0      501       20      321 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/table/utf8/test_length.py
+-rw-r--r--   0      501       20     3533 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/test_analytics.py
+-rw-r--r--   0      501       20      703 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/test_datatypes.py
+-rw-r--r--   0      501       20     3542 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/test_schema.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/udf_library/__init__.py
+-rw-r--r--   0      501       20     2288 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/udf_library/test_url_udfs.py
+-rw-r--r--   0      501       20      338 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests/utils.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests_legacy/__init__.py
+-rw-r--r--   0      501       20     6988 2023-04-29 00:27:26.000000 getdaft-0.1.0/tests_legacy/test_resource_requests.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/__init__.py
+-rw-r--r--   0      501       20     1633 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/patch_package_version.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/__init__.py
+-rw-r--r--   0      501       20        0 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/__init__.py
+-rw-r--r--   0      501       20     1125 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0      501       20       59 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/__init__.py
+-rw-r--r--   0      501       20     2499 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0      501       20     9514 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/cli/convert.py
+-rw-r--r--   0      501       20     3113 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/cli/pack.py
+-rw-r--r--   0      501       20      662 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0      501       20     1246 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/pkginfo.py
+-rw-r--r--   0      501       20      974 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/util.py
+-rw-r--r--   0      501       20     7125 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/_vendor/wheel/wheelfile.py
+-rw-r--r--   0      501       20      878 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/fix-and-copy-wheel.py
+-rw-r--r--   0      501       20     2981 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/tmpdirs.py
+-rw-r--r--   0      501       20     4469 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/tools.py
+-rw-r--r--   0      501       20     9484 2023-04-29 00:27:26.000000 getdaft-0.1.0/tools/wheels/wheeltools.py
+-rw-r--r--   0      501       20       19 2023-04-29 00:27:26.000000 getdaft-0.1.0/tutorials/.gitignore
+-rw-r--r--   0      501       20    12068 2023-04-29 00:27:26.000000 getdaft-0.1.0/tutorials/image_querying/top_n_red_color.ipynb
+-rw-r--r--   0      501       20    98730 2023-04-29 00:27:26.000000 getdaft-0.1.0/tutorials/mnist.ipynb
+-rw-r--r--   0      501       20    11847 2023-04-29 00:27:26.000000 getdaft-0.1.0/tutorials/text_to_image/text_to_image_generation.ipynb
+-rw-r--r--   0      501       20     9134 2023-04-29 00:27:26.000000 getdaft-0.1.0/tutorials/text_to_image/using_cloud_with_ray.ipynb
+-rw-r--r--   0      501       20    29684 2023-04-29 00:27:26.000000 getdaft-0.1.0/Cargo.lock
+-rw-r--r--   0        0        0     7275 1970-01-01 00:00:00.000000 getdaft-0.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `getdaft-0.0.9/LICENSE` & `getdaft-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `getdaft-0.0.9/daft/execution/execution_plan.py` & `getdaft-0.1.0/daft/internal/treenode.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,89 +1,109 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from io import StringIO
-from typing import ClassVar, List
-
-from daft.logical.logical_plan import LogicalPlan, OpLevel
-from daft.resource_request import ResourceRequest
-
-
-class ExecutionOp:
-    logical_ops: List[LogicalPlan]
-    num_partitions: int
-    data_deps: List[int]
-    is_global_op: ClassVar[bool] = False
-
-    def __init__(self, logical_ops: List[LogicalPlan], num_partitions: int) -> None:
-        self.logical_ops = logical_ops
-        self.num_partitions = num_partitions
-        all_deps = set()
-        for node in logical_ops:
-            for child in node._children():
-                all_deps.add(child.id())
-        self.data_deps = list(all_deps - {node.id() for node in logical_ops})
+import os
+import typing
+from typing import TYPE_CHECKING, Generic, List, TypeVar, cast
+
+from loguru import logger
+
+if TYPE_CHECKING:
+    from daft.internal.rule import Rule
+
+TreeNodeType = TypeVar("TreeNodeType", bound="TreeNode")
+
+
+class TreeNode(Generic[TreeNodeType]):
+    _registered_children: list[TreeNodeType]
+
+    def __init__(self) -> None:
+        self._registered_children: list[TreeNodeType] = []
 
-    def __repr__(self) -> str:
-        builder = StringIO()
-        builder.write(f"{self.__class__.__name__}(num_partitions={self.num_partitions})\n")
-        for op in self.logical_ops:
-            builder.write(f"\t{repr(op)}\n\n")
-        return builder.getvalue()
-
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.max_resources([lop.resource_request() for lop in self.logical_ops])
-
-
-class ForEachPartition(ExecutionOp):
-    ...
-
-
-class GlobalOp(ExecutionOp):
-    is_global_op: ClassVar[bool] = True
-    ...
-
-
-@dataclass
-class ExecutionPlan:
-    execution_ops: List[ExecutionOp]
-
-    def __repr__(self) -> str:
-        builder = StringIO()
-        builder.write(f"{self.__class__.__name__}\n")
-        for op in self.execution_ops:
-            op_str = repr(op)
-            for line in op_str.splitlines():
-                builder.write(f"\t{line}\n")
-        return builder.getvalue()
-
-    @classmethod
-    def plan_from_logical(cls, lplan: LogicalPlan) -> ExecutionPlan:
-        post_order = lplan.post_order()
-        for_each_so_far: List[LogicalPlan] = []
-        exec_plan: List[ExecutionOp] = []
-        for lop in post_order:
-            if lop.op_level() == OpLevel.ROW or lop.op_level() == OpLevel.PARTITION:
-                if len(for_each_so_far) > 0:
-                    if (for_each_so_far[-1].num_partitions() != lop.num_partitions()) or (len(lop._children()) == 0):
-                        exec_plan.append(
-                            ForEachPartition(for_each_so_far, num_partitions=for_each_so_far[-1].num_partitions())
-                        )
-                        for_each_so_far = []
-                        # assert for_each_so_far[-1].num_partitions() == lop.num_partitions()
-                for_each_so_far.append(lop)
-                # assert for_each_so_far[-1]
-            elif lop.op_level() == OpLevel.GLOBAL:
-                if len(for_each_so_far) > 0:
-                    exec_plan.append(
-                        ForEachPartition(for_each_so_far, num_partitions=for_each_so_far[-1].num_partitions())
-                    )
-                    for_each_so_far = []
-                exec_plan.append(GlobalOp([lop], num_partitions=lop.num_partitions()))
+    def _children(self) -> list[TreeNodeType]:
+        return self._registered_children
+
+    def _register_child(self, child: TreeNodeType) -> int:
+        self._registered_children.append(child)
+        return len(self._registered_children) - 1
+
+    def apply_and_trickle_down(self, rule: Rule[TreeNodeType]) -> TreeNodeType | None:
+        root = cast(TreeNodeType, self)
+        continue_looping = True
+        made_change = False
+
+        # Apply rule to self and its children
+        while continue_looping:
+            for child in root._children():
+                fn = rule.dispatch_fn(root, child)
+
+                if fn is None:
+                    continue
+                maybe_new_root = fn(root, child)
+
+                if maybe_new_root is not None:
+                    root = maybe_new_root
+                    made_change = True
+                    break
             else:
-                raise NotImplementedError()
+                continue_looping = False
 
-        if len(for_each_so_far) > 0:
-            exec_plan.append(ForEachPartition(for_each_so_far, num_partitions=for_each_so_far[-1].num_partitions()))
-            for_each_so_far = []
+        # Recursively apply_and_trickle_down to children
+        n_children = len(root._children())
+        for i in range(n_children):
+            maybe_new_child = root._registered_children[i].apply_and_trickle_down(rule)
+            if maybe_new_child is not None:
+                root._registered_children[i] = maybe_new_child
+                made_change = True
+
+        if made_change:
+            return root
+        else:
+            return None
+
+    def to_dot_file(self, filename: str | None = None) -> str:
+        dot_data = self.to_dot()
+        base_path = "log"
+        if filename is None:
+            os.makedirs(base_path, exist_ok=True)
+            filename = f"{base_path}/{hash(dot_data)}.dot"
+        with open(filename, "w") as f:
+            f.write(dot_data)
+        logger.info(f"Wrote Dot file to {filename}")
+        return filename
+
+    def to_dot(self) -> str:
+        try:
+            import pydot
+        except ImportError:
+            raise ImportError(
+                "Error while importing pydot: please manually install `pip install pydot` for tree visualizations"
+            )
+
+        graph: pydot.Graph = pydot.Dot("TreeNode", graph_type="digraph", bgcolor="white")  # type: ignore
+        counter = 0
+
+        def recurser(node: TreeNode) -> int:
+            nonlocal counter
+            desc = repr(node)
+            my_id = counter
+            myself = pydot.Node(my_id, label=f"{desc}")
+            graph.add_node(myself)
+            counter += 1
+            for child in node._children():
+                child_id = recurser(child)
+                edge = pydot.Edge(str(my_id), str(child_id), color="black")
+                graph.add_edge(edge)  # type: ignore
+            return my_id
+
+        recurser(self)
+        return graph.to_string()  # type: ignore
+
+    def post_order(self) -> list[TreeNodeType]:
+        nodes = []
+
+        def helper(curr: TreeNode[TreeNodeType]) -> None:
+            for child in curr._children():
+                helper(child)
+            nodes.append(curr)
 
-        return cls(exec_plan)
+        helper(self)
+        return typing.cast(List[TreeNodeType], nodes)
```

### Comparing `getdaft-0.0.9/daft/execution/logical_op_runners.py` & `getdaft-0.1.0/daft/runners/pyrunner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,286 +1,316 @@
-from abc import abstractmethod
-from bisect import bisect_right
-from itertools import accumulate
-from typing import Callable, ClassVar, Dict, List, Type, TypeVar
-
-from pyarrow import csv, json, parquet
-
-from daft.datasources import (
-    CSVSourceInfo,
-    InMemorySourceInfo,
-    JSONSourceInfo,
-    ParquetSourceInfo,
-    ScanType,
-)
-from daft.filesystem import get_filesystem_from_path
-from daft.logical.logical_plan import (
-    Coalesce,
-    Filter,
-    GlobalLimit,
-    Join,
-    LocalAggregate,
-    LocalLimit,
-    LogicalPlan,
-    PartitionScheme,
-    Projection,
-    Repartition,
-    Scan,
-    Sort,
+from __future__ import annotations
+
+import multiprocessing
+from concurrent import futures
+from dataclasses import dataclass
+from typing import Iterable
+
+import psutil
+import pyarrow as pa
+from loguru import logger
+
+from daft.datasources import SourceInfo
+from daft.execution import physical_plan, physical_plan_factory
+from daft.execution.execution_step import Instruction, MaterializedResult, PartitionTask
+from daft.execution.logical_op_runners import LogicalPartitionOpRunner
+from daft.filesystem import glob_path_with_stats
+from daft.internal.gpu import cuda_device_count
+from daft.internal.rule_runner import FixedPointPolicy, Once, RuleBatch, RuleRunner
+from daft.logical import logical_plan
+from daft.logical.optimizer import (
+    DropProjections,
+    DropRepartition,
+    FoldProjections,
+    PruneColumns,
+    PushDownClausesIntoScan,
+    PushDownLimit,
+    PushDownPredicates,
 )
-from daft.logical.schema import ExpressionList
+from daft.logical.schema import Schema
 from daft.resource_request import ResourceRequest
-from daft.runners.blocks import DataBlock
-from daft.runners.partitioning import PartitionSet, vPartition
-from daft.runners.shuffle_ops import (
-    CoalesceOp,
-    RepartitionHashOp,
-    RepartitionRandomOp,
-    ShuffleOp,
-    Shuffler,
-    SortOp,
+from daft.runners import runner_io
+from daft.runners.partitioning import (
+    PartID,
+    PartitionCacheEntry,
+    PartitionMetadata,
+    PartitionSet,
+    vPartitionSchemaInferenceOptions,
 )
+from daft.runners.profiler import profiler
+from daft.runners.runner import Runner
+from daft.table import Table
+
+
+@dataclass
+class LocalPartitionSet(PartitionSet[Table]):
+    _partitions: dict[PartID, Table]
+
+    def items(self) -> list[tuple[PartID, Table]]:
+        return sorted(self._partitions.items())
+
+    def _get_merged_vpartition(self) -> Table:
+        ids_and_partitions = self.items()
+        assert ids_and_partitions[0][0] == 0
+        assert ids_and_partitions[-1][0] + 1 == len(ids_and_partitions)
+        return Table.concat([part for id, part in ids_and_partitions])
+
+    def get_partition(self, idx: PartID) -> Table:
+        return self._partitions[idx]
+
+    def set_partition(self, idx: PartID, part: Table) -> None:
+        self._partitions[idx] = part
 
+    def delete_partition(self, idx: PartID) -> None:
+        del self._partitions[idx]
 
-class LogicalPartitionOpRunner:
-    @abstractmethod
-    def run_node_list(
+    def has_partition(self, idx: PartID) -> bool:
+        return idx in self._partitions
+
+    def __len__(self) -> int:
+        return sum(self.len_of_partitions())
+
+    def len_of_partitions(self) -> list[int]:
+        partition_ids = sorted(list(self._partitions.keys()))
+        return [len(self._partitions[pid]) for pid in partition_ids]
+
+    def num_partitions(self) -> int:
+        return len(self._partitions)
+
+    def wait(self) -> None:
+        pass
+
+
+class PyRunnerIO(runner_io.RunnerIO[Table]):
+    def glob_paths_details(
         self,
-        inputs: Dict[int, PartitionSet],
-        nodes: List[LogicalPlan],
-        num_partitions: int,
-        resource_request: ResourceRequest,
-    ):
-        raise NotImplementedError()
-
-    def run_node_list_single_partition(
-        self, inputs: Dict[int, vPartition], nodes: List[LogicalPlan], partition_id: int
-    ) -> vPartition:
-        part_set = {nid: part for nid, part in inputs.items()}
-        for node in nodes:
-            output = self.run_single_node(inputs=part_set, node=node, partition_id=partition_id)
-            part_set[node.id()] = output
-            for child in node._children():
-                del part_set[child.id()]
-        return output
-
-    def run_single_node(self, inputs: Dict[int, vPartition], node: LogicalPlan, partition_id: int) -> vPartition:
-        if isinstance(node, Scan):
-            return self._handle_scan(inputs, node, partition_id=partition_id)
-        elif isinstance(node, Projection):
-            return self._handle_projection(inputs, node, partition_id=partition_id)
-        elif isinstance(node, Filter):
-            return self._handle_filter(inputs, node, partition_id=partition_id)
-        elif isinstance(node, LocalLimit):
-            return self._handle_local_limit(inputs, node, partition_id=partition_id)
-        elif isinstance(node, LocalAggregate):
-            return self._handle_local_aggregate(inputs, node, partition_id=partition_id)
-        elif isinstance(node, Join):
-            return self._handle_join(inputs, node, partition_id=partition_id)
-        else:
-            raise NotImplementedError(f"{type(node)} not implemented")
-
-    def _handle_scan(self, inputs: Dict[int, vPartition], scan: Scan, partition_id: int) -> vPartition:
-        schema = scan.schema()
-        column_ids = [col.get_id() for col in schema.to_column_expressions()]
-        if scan._source_info.scan_type() == ScanType.IN_MEMORY:
-            assert isinstance(scan._source_info, InMemorySourceInfo)
-            table_len = [len(scan._source_info.data[key]) for key in scan._source_info.data][0]
-            partition_size = table_len // scan._source_info.num_partitions
-            start, end = (partition_size * partition_id, partition_size * (partition_id + 1))
-            data = {key: scan._source_info.data[key][start:end] for key in scan._source_info.data}
-            vpart = vPartition.from_pydict(data, schema=schema, partition_id=partition_id)
-            return vpart
-        elif scan._source_info.scan_type() == ScanType.CSV:
-            assert isinstance(scan._source_info, CSVSourceInfo)
-            path = scan._source_info.filepaths[partition_id]
-            fs = get_filesystem_from_path(path)
-            table = csv.read_csv(
-                fs.open(path, compression="infer"),
-                parse_options=csv.ParseOptions(
-                    delimiter=scan._source_info.delimiter,
+        source_path: str,
+        source_info: SourceInfo | None = None,
+    ) -> LocalPartitionSet:
+        files_info = glob_path_with_stats(source_path, source_info)
+
+        if len(files_info) == 0:
+            raise FileNotFoundError(f"No files found at {source_path}")
+
+        partition = Table.from_pydict(
+            {
+                "path": pa.array([file_info.path for file_info in files_info], type=pa.string()),
+                "size": pa.array([file_info.size for file_info in files_info], type=pa.int64()),
+                "type": pa.array([file_info.type for file_info in files_info], type=pa.string()),
+                "rows": pa.array([file_info.rows for file_info in files_info], type=pa.int64()),
+            },
+        )
+
+        # Make sure that the schema is consistent with what we expect
+        assert (
+            partition.schema() == PyRunnerIO.FS_LISTING_SCHEMA
+        ), f"Schema should be expected: {PyRunnerIO.FS_LISTING_SCHEMA}, but received: {partition.schema()}"
+
+        pset = LocalPartitionSet(
+            {
+                # Hardcoded to 1 partition
+                0: partition,
+            }
+        )
+        return pset
+
+    def get_schema_from_first_filepath(
+        self,
+        listing_details_partitions: PartitionSet[Table],
+        source_info: SourceInfo,
+        schema_inference_options: vPartitionSchemaInferenceOptions,
+    ) -> Schema:
+        # Naively retrieve the first filepath in the PartitionSet
+        nonempty_partitions = [
+            p
+            for p, p_len in zip(listing_details_partitions.values(), listing_details_partitions.len_of_partitions())
+            if p_len > 0
+        ]
+        if len(nonempty_partitions) == 0:
+            raise ValueError("No files to get schema from")
+        first_filepath = nonempty_partitions[0].to_pydict()[PyRunnerIO.FS_LISTING_PATH_COLUMN_NAME][0]
+
+        return runner_io.sample_schema(first_filepath, source_info, schema_inference_options)
+
+
+class LocalLogicalPartitionOpRunner(LogicalPartitionOpRunner):
+    ...
+
+
+class PyRunner(Runner):
+    def __init__(self, use_thread_pool: bool | None) -> None:
+        super().__init__()
+        self._use_thread_pool: bool = use_thread_pool if use_thread_pool is not None else True
+
+        self._optimizer = RuleRunner(
+            [
+                RuleBatch(
+                    "SinglePassPushDowns",
+                    Once,
+                    [
+                        DropRepartition(),
+                        PushDownPredicates(),
+                        PruneColumns(),
+                        FoldProjections(),
+                        PushDownClausesIntoScan(),
+                    ],
                 ),
-                read_options=csv.ReadOptions(
-                    column_names=[expr.name() for expr in schema],
-                    skip_rows_after_names=1 if scan._source_info.has_headers else 0,
+                RuleBatch(
+                    "PushDownLimitsAndRepartitions",
+                    FixedPointPolicy(3),
+                    [PushDownLimit(), DropRepartition(), DropProjections()],
                 ),
-            )
-            vpart = vPartition.from_arrow_table(table, column_ids=column_ids, partition_id=partition_id)
-            return vpart
-        elif scan._source_info.scan_type() == ScanType.JSON:
-            assert isinstance(scan._source_info, JSONSourceInfo)
-            path = scan._source_info.filepaths[partition_id]
-            fs = get_filesystem_from_path(path)
-            table = json.read_json(fs.open(path, compression="infer")).select([col.name() for col in schema])
-            vpart = vPartition.from_arrow_table(table, column_ids=column_ids, partition_id=partition_id)
-            return vpart
-        elif scan._source_info.scan_type() == ScanType.PARQUET:
-            assert isinstance(scan._source_info, ParquetSourceInfo)
-            table = parquet.read_table(scan._source_info.filepaths[partition_id])
-            vpart = vPartition.from_arrow_table(table, column_ids=column_ids, partition_id=partition_id)
-            return vpart
-        else:
-            raise NotImplementedError(f"PyRunner has not implemented scan: {scan._source_info.scan_type()}")
-
-    def _handle_projection(self, inputs: Dict[int, vPartition], proj: Projection, partition_id: int) -> vPartition:
-        child_id = proj._children()[0].id()
-        prev_partition = inputs[child_id]
-        return prev_partition.eval_expression_list(proj._projection)
-
-    def _handle_filter(self, inputs: Dict[int, vPartition], filter: Filter, partition_id: int) -> vPartition:
-        predicate = filter._predicate
-        child_id = filter._children()[0].id()
-        prev_partition = inputs[child_id]
-        return prev_partition.filter(predicate)
-
-    def _handle_local_limit(self, inputs: Dict[int, vPartition], limit: LocalLimit, partition_id: int) -> vPartition:
-        num = limit._num
-        child_id = limit._children()[0].id()
-        prev_partition = inputs[child_id]
-        return prev_partition.head(num)
-
-    def _handle_local_aggregate(
-        self, inputs: Dict[int, vPartition], agg: LocalAggregate, partition_id: int
-    ) -> vPartition:
-        child_id = agg._children()[0].id()
-        prev_partition = inputs[child_id]
-        return prev_partition.agg(agg._agg, group_by=agg._group_by)
-
-    def _handle_join(self, inputs: Dict[int, vPartition], join: Join, partition_id: int) -> vPartition:
-        left_id = join._children()[0].id()
-        right_id = join._children()[1].id()
-        left_partition = inputs[left_id]
-        right_partition = inputs[right_id]
-        return left_partition.join(
-            right_partition,
-            left_on=join._left_on,
-            right_on=join._right_on,
-            output_schema=join.schema(),
-            how=join._how.value,
+            ]
         )
 
+        self.num_cpus = multiprocessing.cpu_count()
+        self.num_gpus = cuda_device_count()
+        self.bytes_memory = psutil.virtual_memory().total
+
+    def optimize(self, plan: logical_plan.LogicalPlan) -> logical_plan.LogicalPlan:
+        # From PyRunner
+        return self._optimizer.optimize(plan)
+
+    def runner_io(self) -> PyRunnerIO:
+        return PyRunnerIO()
+
+    def run(self, logplan: logical_plan.LogicalPlan) -> PartitionCacheEntry:
+        logplan = self.optimize(logplan)
+        psets = {
+            key: entry.value.values()
+            for key, entry in self._part_set_cache._uuid_to_partition_set.items()
+            if entry.value is not None
+        }
+        plan = physical_plan_factory.get_materializing_physical_plan(logplan, psets)
+
+        with profiler("profile_PyRunner.run_{datetime.now().isoformat()}.json"):
+            partitions = self._physical_plan_to_partitions(plan)
+
+            result_pset = LocalPartitionSet({})
+            for i, partition in enumerate(partitions):
+                result_pset.set_partition(i, partition)
+
+            pset_entry = self.put_partition_set_into_cache(result_pset)
+            return pset_entry
+
+    def _physical_plan_to_partitions(self, plan: physical_plan.MaterializedPhysicalPlan) -> list[Table]:
+        inflight_tasks: dict[str, PartitionTask] = dict()
+        inflight_tasks_resources: dict[str, ResourceRequest] = dict()
+        future_to_task: dict[futures.Future, str] = dict()
+
+        result = []
+        next_step = None
+        with futures.ThreadPoolExecutor() as thread_pool:
+            try:
+                while True:
+                    # Get the next task to dispatch.
+                    if next_step is None:
+                        next_step = next(plan)
+
+                    # Try dispatching tasks (up to resource limits) until there are no more tasks to dispatch.
+                    while next_step is not None and self._can_admit_task(
+                        next_step.resource_request, inflight_tasks_resources.values()
+                    ):
+
+                        # Run the task in the main thread, instead of the thread pool, in certain conditions:
+                        # - Threading is disabled in runner config.
+                        # - Task is a no-op.
+                        # - Task requires GPU.
+                        # TODO(charles): Queue these up until the physical plan is blocked to avoid starving cluster.
+                        if (
+                            not self._use_thread_pool
+                            or len(next_step.instructions) == 0
+                            or (
+                                next_step.resource_request.num_gpus is not None
+                                and next_step.resource_request.num_gpus > 0
+                            )
+                        ):
+                            logger.debug("Running task synchronously in main thread: {next_step}", next_step=next_step)
+                            partitions = self.build_partitions(next_step.instructions, *next_step.inputs)
+                            next_step.set_result([PyMaterializedResult(partition) for partition in partitions])
+
+                        else:
+                            # Submit the task for execution.
+                            logger.debug("Submitting task for execution: {next_step}", next_step=next_step)
+                            future = thread_pool.submit(
+                                self.build_partitions, next_step.instructions, *next_step.inputs
+                            )
+                            # Register the inflight task and resources used.
+                            future_to_task[future] = next_step.id()
+                            inflight_tasks[next_step.id()] = next_step
+                            inflight_tasks_resources[next_step.id()] = next_step.resource_request
+
+                        # Get the next task to dispatch.
+                        next_step = next(plan)
+
+                    # Await at least task and process the results.
+                    assert (
+                        len(future_to_task) > 0
+                    ), f"Scheduler deadlocked! This should never happen. Please file an issue."
+                    done_set, _ = futures.wait(list(future_to_task.keys()), return_when=futures.FIRST_COMPLETED)
+                    for done_future in done_set:
+                        done_id = future_to_task.pop(done_future)
+                        del inflight_tasks_resources[done_id]
+                        done_task = inflight_tasks.pop(done_id)
+                        partitions = done_future.result()
+
+                        logger.debug(
+                            "Task completed: {done_id} -> {partitions}", done_id=done_id, partitions=partitions
+                        )
+                        done_task.set_result([PyMaterializedResult(partition) for partition in partitions])
+
+            except StopIteration as e:
+                result = e.value
+
+        return result
+
+    def _check_resource_requests(self, resource_request: ResourceRequest) -> None:
+        """Validates that the requested ResourceRequest is possible to run locally"""
+
+        if resource_request.num_cpus is not None and resource_request.num_cpus > self.num_cpus:
+            raise RuntimeError(f"Requested {resource_request.num_cpus} CPUs but found only {self.num_cpus} available")
+        if resource_request.num_gpus is not None and resource_request.num_gpus > self.num_gpus:
+            raise RuntimeError(f"Requested {resource_request.num_gpus} GPUs but found only {self.num_gpus} available")
+        if resource_request.memory_bytes is not None and resource_request.memory_bytes > self.bytes_memory:
+            raise RuntimeError(
+                f"Requested {resource_request.memory_bytes} bytes of memory but found only {self.bytes_memory} available"
+            )
 
-ReduceType = TypeVar("ReduceType")
+    def _can_admit_task(self, resource_request: ResourceRequest, inflight_resources: Iterable[ResourceRequest]) -> bool:
+        self._check_resource_requests(resource_request)
 
+        total_inflight_resources: ResourceRequest = sum(inflight_resources, ResourceRequest())
+        cpus_okay = (total_inflight_resources.num_cpus or 0) + (resource_request.num_cpus or 0) <= self.num_cpus
+        gpus_okay = (total_inflight_resources.num_gpus or 0) + (resource_request.num_gpus or 0) <= self.num_gpus
+        memory_okay = (total_inflight_resources.memory_bytes or 0) + (
+            resource_request.memory_bytes or 0
+        ) <= self.bytes_memory
 
-class LogicalGlobalOpRunner:
-    shuffle_ops: ClassVar[Dict[Type[ShuffleOp], Type[Shuffler]]]
+        return all((cpus_okay, gpus_okay, memory_okay))
 
-    def run_node_list(self, inputs: Dict[int, PartitionSet], nodes: List[LogicalPlan]) -> PartitionSet:
-        part_set = inputs.copy()
-        for node in nodes:
-            output = self.run_single_node(inputs=part_set, node=node)
-            part_set[node.id()] = output
-            for child in node._children():
-                del part_set[child.id()]
-        return output
-
-    def run_single_node(self, inputs: Dict[int, PartitionSet], node: LogicalPlan) -> PartitionSet:
-        if isinstance(node, GlobalLimit):
-            return self._handle_global_limit(inputs, node)
-        elif isinstance(node, Repartition):
-            return self._handle_repartition(inputs, node)
-        elif isinstance(node, Sort):
-            return self._handle_sort(inputs, node)
-        elif isinstance(node, Coalesce):
-            return self._handle_coalesce(inputs, node)
-        else:
-            raise NotImplementedError(f"{type(node)} not implemented")
-
-    @abstractmethod
-    def map_partitions(
-        self, pset: PartitionSet, func: Callable[[vPartition], vPartition], resource_request: ResourceRequest
-    ) -> PartitionSet:
-        raise NotImplementedError()
-
-    @abstractmethod
-    def reduce_partitions(self, pset: PartitionSet, func: Callable[[List[vPartition]], ReduceType]) -> ReduceType:
-        raise NotImplementedError()
-
-    def _get_shuffle_op_klass(self, t: Type[ShuffleOp]) -> Type[Shuffler]:
-        return self.__class__.shuffle_ops[t]
-
-    def _handle_global_limit(self, inputs: Dict[int, PartitionSet], limit: GlobalLimit) -> PartitionSet:
-        child_id = limit._children()[0].id()
-        prev_part = inputs[child_id]
-
-        num = limit._num
-        size_per_partition = prev_part.len_of_partitions()
-        total_size = sum(size_per_partition)
-        if total_size <= num:
-            return prev_part
-
-        cum_sum = list(accumulate(size_per_partition))
-        where_to_cut_idx = bisect_right(cum_sum, num)
-        count_so_far = cum_sum[where_to_cut_idx - 1]
-        remainder = num - count_so_far
-        assert remainder >= 0
-
-        def limit_map_func(part: vPartition) -> vPartition:
-            if part.partition_id < where_to_cut_idx:
-                return part
-            elif part.partition_id == where_to_cut_idx:
-                return part.head(remainder)
-            else:
-                return part.head(0)
-
-        return self.map_partitions(prev_part, limit_map_func, limit.resource_request())
-
-    def _handle_repartition(self, inputs: Dict[int, PartitionSet], repartition: Repartition) -> PartitionSet:
-
-        child_id = repartition._children()[0].id()
-        repartitioner: ShuffleOp
-        if repartition._scheme == PartitionScheme.RANDOM:
-            repartitioner = self._get_shuffle_op_klass(RepartitionRandomOp)(
-                expr_eval_resource_request=ResourceRequest.default()
-            )
-        elif repartition._scheme == PartitionScheme.HASH:
-            repartitioner = self._get_shuffle_op_klass(RepartitionHashOp)(
-                expr_eval_resource_request=repartition.resource_request(),
-                map_args={"exprs": repartition._partition_by.exprs},
-            )
-        else:
-            raise NotImplementedError()
-        prev_part = inputs[child_id]
-        return repartitioner.run(input=prev_part, num_target_partitions=repartition.num_partitions())
-
-    def _handle_sort(self, inputs: Dict[int, PartitionSet], sort: Sort) -> PartitionSet:
-
-        child_id = sort._children()[0].id()
-
-        SAMPLES_PER_PARTITION = 20
-        num_partitions = sort.num_partitions()
-        exprs: ExpressionList = sort._sort_by
-
-        def sample_map_func(part: vPartition) -> vPartition:
-            return part.sample(SAMPLES_PER_PARTITION).eval_expression_list(exprs)
-
-        def quantile_reduce_func(to_reduce: List[vPartition]) -> DataBlock:
-            merged = vPartition.merge_partitions(to_reduce, verify_partition_id=False)
-            first_column = list(merged.columns.values())[0]
-            return first_column.block.quantiles(num_partitions)
-
-        prev_part = inputs[child_id]
-        sampled_partitions = self.map_partitions(prev_part, sample_map_func, sort.resource_request())
-        boundaries = self.reduce_partitions(sampled_partitions, quantile_reduce_func)
-        expr = exprs.exprs[0]
-        sort_shuffle_op_klass = self._get_shuffle_op_klass(SortOp)
-        sort_op = sort_shuffle_op_klass(
-            expr_eval_resource_request=sort.resource_request(),
-            map_args={"expr": expr, "boundaries": boundaries, "desc": sort._desc},
-            reduce_args={"expr": expr, "desc": sort._desc},
-        )
+    @staticmethod
+    def build_partitions(instruction_stack: list[Instruction], *inputs: Table) -> list[Table]:
+        partitions = list(inputs)
+        for instruction in instruction_stack:
+            partitions = instruction.run(partitions)
 
-        return sort_op.run(input=prev_part, num_target_partitions=num_partitions)
+        return partitions
 
-    def _handle_coalesce(self, inputs: Dict[int, PartitionSet], coal: Coalesce) -> PartitionSet:
-        child_id = coal._children()[0].id()
-        num_partitions = coal.num_partitions()
-        prev_part = inputs[child_id]
-
-        coalesce_op_klass = self._get_shuffle_op_klass(CoalesceOp)
-
-        coalesce_op = coalesce_op_klass(
-            expr_eval_resource_request=ResourceRequest.default(),
-            map_args={"num_input_partitions": prev_part.num_partitions()},
-        )
-        return coalesce_op.run(input=prev_part, num_target_partitions=num_partitions)
+
+@dataclass(frozen=True)
+class PyMaterializedResult(MaterializedResult[Table]):
+    _partition: Table
+
+    def partition(self) -> Table:
+        return self._partition
+
+    def vpartition(self) -> Table:
+        return self._partition
+
+    def metadata(self) -> PartitionMetadata:
+        return PartitionMetadata.from_table(self._partition)
+
+    def cancel(self) -> None:
+        return None
+
+    def _noop(self, _: Table) -> None:
+        return None
```

### Comparing `getdaft-0.0.9/daft/internal/rule.py` & `getdaft-0.1.0/daft/internal/rule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,51 @@
-from typing import Callable, Dict, Generic, List, Optional, Tuple, Type, TypeVar
+from __future__ import annotations
+
+from typing import Callable, Generic, Optional, TypeVar
 
 from daft.internal.treenode import TreeNode
 
 TreeNodeType = TypeVar("TreeNodeType", bound="TreeNode")
 
 RuleFn = Callable[[TreeNodeType, TreeNodeType], Optional[TreeNodeType]]
 
 
-def get_all_subclasses(type: Type) -> List[Type]:
-    result = [type]
+def get_all_subclasses(input_type: type) -> list[type]:
+    result = [input_type]
 
-    def helper(t: Type):
+    def helper(t: type):
         subclasses = t.__subclasses__()
         result.extend(subclasses)
         for sc in subclasses:
             helper(sc)
 
-    helper(type)
+    helper(input_type)
     return result
 
 
 class Rule(Generic[TreeNodeType]):
     def __init__(self) -> None:
-        self._fn_registry: Dict[Tuple[Type[TreeNodeType], Type[TreeNodeType]], RuleFn] = dict()
+        self._fn_registry: dict[tuple[type[TreeNodeType], type[TreeNodeType]], RuleFn] = dict()
 
-    def register_fn(self, parent_type: Type, child_type: Type, fn: RuleFn, override: bool = False) -> None:
+    def register_fn(self, parent_type: type, child_type: type, fn: RuleFn, override: bool = False) -> None:
         for p_subclass in get_all_subclasses(parent_type):
             for c_subtype in get_all_subclasses(child_type):
                 type_tuple = (p_subclass, c_subtype)
-                if not override:
-                    assert type_tuple not in self._fn_registry
-                self._fn_registry[type_tuple] = fn
+                if type_tuple in self._fn_registry:
+                    if override:
+                        self._fn_registry[type_tuple] = fn
+                    else:
+                        raise ValueError(f"Rule already registered for {type_tuple}")
+                else:
+                    self._fn_registry[type_tuple] = fn
 
-    def dispatch_fn(self, parent: TreeNodeType, child: TreeNodeType) -> Optional[RuleFn]:
+    def dispatch_fn(self, parent: TreeNodeType, child: TreeNodeType) -> RuleFn | None:
         type_tuple = (type(parent), type(child))
+        if type_tuple not in self._fn_registry:
+            return None
         return self._fn_registry.get(type_tuple, None)
 
-    def apply(self, parent: TreeNodeType, child: TreeNodeType) -> Optional[TreeNodeType]:
+    def apply(self, parent: TreeNodeType, child: TreeNodeType) -> TreeNodeType | None:
         fn = self.dispatch_fn(parent, child)
-        if fn is not None:
-            return fn(parent, child)
-        else:
+        if fn is None:
             return None
+        return fn(parent, child)
```

### Comparing `getdaft-0.0.9/daft/internal/rule_runner.py` & `getdaft-0.1.0/daft/internal/rule_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from copy import deepcopy
+from __future__ import annotations
+
 from dataclasses import dataclass
-from typing import Generic, List, TypeVar
+from typing import Generic, TypeVar
 
 from loguru import logger
 
 from daft.internal.rule import Rule
 from daft.internal.treenode import TreeNode
 
 TreeNodeType = TypeVar("TreeNodeType", bound="TreeNode")
@@ -18,23 +19,22 @@
 Once = FixedPointPolicy(1)
 
 
 @dataclass
 class RuleBatch(Generic[TreeNodeType]):
     name: str
     mode: FixedPointPolicy
-    rules: List[Rule[TreeNodeType]]
+    rules: list[Rule[TreeNodeType]]
 
 
 class RuleRunner(Generic[TreeNodeType]):
-    def __init__(self, batches: List[RuleBatch[TreeNodeType]]) -> None:
+    def __init__(self, batches: list[RuleBatch[TreeNodeType]]) -> None:
         self._batches = batches
 
     def optimize(self, root: TreeNodeType) -> TreeNodeType:
-        root = deepcopy(root)
         for batch in self._batches:
             root = self._run_single_batch(root, batch)
         return root
 
     def __call__(self, root: TreeNodeType) -> TreeNodeType:
         return self.optimize(root)
```

### Comparing `getdaft-0.0.9/daft/logical/logical_plan.py` & `getdaft-0.1.0/daft/logical/logical_plan.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,81 @@
 from __future__ import annotations
 
 import itertools
+import pathlib
 from abc import abstractmethod
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from enum import Enum, IntEnum
-from typing import Any, List, Optional, Tuple
+from pprint import pformat
+from typing import Any, Generic, TypeVar
 
-from daft.datasources import SourceInfo
-from daft.execution.operators import ExpressionType
-from daft.expressions import ColumnExpression, Expression
+from daft.datasources import SourceInfo, StorageType
+from daft.datatype import DataType
+from daft.errors import ExpressionTypeError
+from daft.expressions import Expression, ExpressionsProjection, col
+from daft.expressions.testing import expr_structurally_equal
 from daft.internal.treenode import TreeNode
-from daft.logical.schema import ExpressionList
+from daft.logical.map_partition_ops import ExplodeOp, MapPartitionOp
+from daft.logical.schema import Schema
 from daft.resource_request import ResourceRequest
+from daft.runners.partitioning import PartitionCacheEntry
+from daft.table import Table
 
 
 class OpLevel(IntEnum):
     ROW = 1
     PARTITION = 2
     GLOBAL = 3
 
 
 class LogicalPlan(TreeNode["LogicalPlan"]):
     id_iter = itertools.count()
 
-    def __init__(self, schema: ExpressionList, partition_spec: PartitionSpec, op_level: OpLevel) -> None:
+    def __init__(
+        self,
+        schema: Schema,
+        partition_spec: PartitionSpec,
+        op_level: OpLevel,
+    ) -> None:
         super().__init__()
+        if not isinstance(schema, Schema):
+            raise ValueError(f"expected Schema Object for LogicalPlan but got {type(schema)}")
         self._schema = schema
         self._op_level = op_level
         self._partition_spec = partition_spec
         self._id = next(LogicalPlan.id_iter)
 
-    def schema(self) -> ExpressionList:
+    def schema(self) -> Schema:
         return self._schema
 
-    @abstractmethod
     def resource_request(self) -> ResourceRequest:
-        """Resources required to execute this LogicalPlan"""
+        """Returns a custom ResourceRequest if one has been attached to this LogicalPlan
+
+        Implementations should override this if they allow for customized ResourceRequests.
+        """
+        return ResourceRequest()
+
+    @abstractmethod
+    def required_columns(self) -> list[set[str]]:
         raise NotImplementedError()
 
     @abstractmethod
-    def required_columns(self) -> ExpressionList:
+    def input_mapping(self) -> list[dict[str, str]]:
         raise NotImplementedError()
 
     @abstractmethod
     def _local_eq(self, other: Any) -> bool:
         raise NotImplementedError()
 
     def is_eq(self, other: Any) -> bool:
         return (
             isinstance(other, LogicalPlan)
             and self._local_eq(other)
             and self.schema() == other.schema()
+            and self.partition_spec() == other.partition_spec()
             and self.num_partitions() == other.num_partitions()
             and all(
                 [self_child.is_eq(other_child) for self_child, other_child in zip(self._children(), other._children())]
             )
         )
 
     def __eq__(self, other: Any) -> bool:
@@ -80,322 +101,664 @@
         other_node_ids = set(map(LogicalPlan.id, other.post_order()))
         return self_node_ids.isdisjoint(other_node_ids)
 
     @abstractmethod
     def rebuild(self) -> LogicalPlan:
         raise NotImplementedError()
 
-
-class UnaryNode(LogicalPlan):
     @abstractmethod
-    def copy_with_new_input(self, new_input: UnaryNode) -> UnaryNode:
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
         raise NotImplementedError()
 
+    def pretty_print(
+        self,
+    ) -> str:
+        builder: list[str] = []
+
+        def helper(node: LogicalPlan, depth: int = 0, index: int = 0, prefix: str = "", header: str = ""):
+            children: list[LogicalPlan] = node._children()
+            obj_repr_lines = repr(node).splitlines()
+            builder.append(f"{header}{obj_repr_lines[0]}\n")
+
+            if len(children) > 0:
+                body_prefix = prefix + "│"
+            else:
+                body_prefix = prefix + " "
+
+            for line in obj_repr_lines[1:]:
+                builder.append(f"{body_prefix}{line}\n")
+            builder.append(f"{body_prefix}\n")
+
+            if len(children) < 2:
+                for child in children:
+                    has_grandchild = len(child._children()) > 0
+
+                    if has_grandchild:
+                        header = prefix + "├──"
+                    else:
+                        header = prefix + "└──"
+
+                    helper(child, depth=depth, index=index + 1, prefix=prefix, header=header)
+            else:
+
+                connector = "└─"
+                middle_child_header = "─┬─"
+
+                for i, child in enumerate(children):
+                    has_grandchild = len(child._children()) > 0
+                    if has_grandchild:
+                        final_header = "─┬─"
+                    else:
+                        final_header = "───"
+
+                    position = len(children) - i
+                    if i != len(children) - 1:
+                        next_child_prefix = prefix + ("   │  " * (position - 1))
+                    else:
+                        next_child_prefix = prefix + "      "
+                    header = (
+                        next_child_prefix[: -3 * position]
+                        + connector
+                        + (middle_child_header * (position - 1))
+                        + final_header
+                    )
+
+                    helper(child, depth=depth + 1, index=i, prefix=next_child_prefix, header=header)
+
+        helper(self, 0, 0, header="┌─")
+        return "".join(builder)
+
+    def _repr_helper(self, **fields: Any) -> str:
+
+        fields_to_print: dict[str, Any] = {}
+        if "output" not in fields:
+            fields_to_print["output"] = self.schema()
+
+        fields_to_print.update(fields)
+        fields_to_print["partitioning"] = self.partition_spec()
+        reduced_types = {}
+        for k, v in fields_to_print.items():
+            if isinstance(v, ExpressionsProjection):
+                v = list(v)
+            elif isinstance(v, Schema):
+                v = list([col(field.name) for field in v])
+            elif isinstance(v, PartitionSpec):
+                v = asdict(v)
+                if isinstance(v["by"], ExpressionsProjection):
+                    v["by"] = list(v["by"])
+            reduced_types[k] = v
+        to_render: list[str] = [f"{self.__class__.__name__}\n"]
+        space = "    "
+        for key, value in reduced_types.items():
+            repr_ed = pformat(value, width=80, compact=True).splitlines()
+            to_render.append(f"{space}{key}={repr_ed[0]}\n")
+            for line in repr_ed[1:]:
+                to_render.append(f"{space*2}{line}\n")
+
+        return "".join(to_render)
+
+
+class UnaryNode(LogicalPlan):
+    ...
+
 
 class BinaryNode(LogicalPlan):
     ...
 
 
-class Scan(LogicalPlan):
+class TabularFilesScan(UnaryNode):
     def __init__(
         self,
         *,
-        schema: ExpressionList,
+        schema: Schema,
         source_info: SourceInfo,
-        predicate: Optional[ExpressionList] = None,
-        columns: Optional[List[str]] = None,
+        predicate: ExpressionsProjection | None = None,
+        columns: list[str] | None = None,
+        filepaths_child: LogicalPlan,
+        filepaths_column_name: str,
+        num_partitions: int | None = None,
+        limit_rows: int | None = None,
     ) -> None:
-        schema = schema.resolve()
-        pspec = PartitionSpec(scheme=PartitionScheme.UNKNOWN, num_partitions=source_info.get_num_partitions())
+        if num_partitions is None:
+            num_partitions = filepaths_child.num_partitions()
+        pspec = PartitionSpec(scheme=PartitionScheme.UNKNOWN, num_partitions=num_partitions)
         super().__init__(schema, partition_spec=pspec, op_level=OpLevel.PARTITION)
 
         if predicate is not None:
-            self._predicate = predicate.resolve(schema)
+            self._predicate = predicate
         else:
-            self._predicate = ExpressionList([])
+            self._predicate = ExpressionsProjection([])
 
         if columns is not None:
-            new_schema = ExpressionList([ColumnExpression(c) for c in columns])
-            self._output_schema = new_schema.resolve(schema)
+            self._output_schema = Schema._from_field_name_and_types(
+                [(schema[col].name, schema[col].dtype) for col in columns]
+            )
         else:
             self._output_schema = schema
+
         self._column_names = columns
         self._columns = self._schema
         self._source_info = source_info
+        self._limit_rows = limit_rows
+
+        # TabularFilesScan has a single child node that provides the filepaths to read from.
+        assert (
+            filepaths_child.schema()[filepaths_column_name] is not None
+        ), f"TabularFileScan requires a child with '{filepaths_column_name}' column"
+        self._register_child(filepaths_child)
+        self._filepaths_column_name = filepaths_column_name
+
+    @property
+    def _filepaths_child(self) -> LogicalPlan:
+        child = self._children()[0]
+        return child
 
-    def schema(self) -> ExpressionList:
+    def schema(self) -> Schema:
         return self._output_schema
 
     def __repr__(self) -> str:
-        return f"Scan\n\toutput={self.schema()}\n\tpredicate={self._predicate}\n\tcolumns={self._columns}\n\t{self._source_info}"
+        return self._repr_helper(columns_pruned=len(self._columns) - len(self.schema()), source_info=self._source_info)
 
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.default()
+    def required_columns(self) -> list[set[str]]:
+        return [{self._filepaths_column_name} | self._predicate.required_columns()]
 
-    def required_columns(self) -> ExpressionList:
-        return self._predicate.required_columns()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [dict()]
 
     def _local_eq(self, other: Any) -> bool:
         return (
-            isinstance(other, Scan)
+            isinstance(other, TabularFilesScan)
             and self.schema() == other.schema()
             and self._predicate == other._predicate
             and self._columns == other._columns
             and self._source_info == other._source_info
+            and self._filepaths_column_name == other._filepaths_column_name
         )
 
     def rebuild(self) -> LogicalPlan:
-        return Scan(
-            schema=self.schema().unresolve(),
+        child = self._filepaths_child.rebuild()
+        return TabularFilesScan(
+            schema=self.schema(),
+            source_info=self._source_info,
+            predicate=self._predicate if self._predicate is not None else None,
+            columns=self._column_names,
+            filepaths_child=child,
+            filepaths_column_name=self._filepaths_column_name,
+        )
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return TabularFilesScan(
+            schema=self.schema(),
             source_info=self._source_info,
-            predicate=self._predicate.unresolve() if self._predicate is not None else None,
+            predicate=self._predicate,
             columns=self._column_names,
+            filepaths_child=new_children[0],
+            filepaths_column_name=self._filepaths_column_name,
+        )
+
+
+class InMemoryScan(UnaryNode):
+    def __init__(
+        self, cache_entry: PartitionCacheEntry, schema: Schema, partition_spec: PartitionSpec | None = None
+    ) -> None:
+
+        if partition_spec is None:
+            partition_spec = PartitionSpec(scheme=PartitionScheme.UNKNOWN, num_partitions=1)
+
+        super().__init__(schema=schema, partition_spec=partition_spec, op_level=OpLevel.GLOBAL)
+        self._cache_entry = cache_entry
+
+    def __repr__(self) -> str:
+        return self._repr_helper(cache_id=self._cache_entry.key)
+
+    def _local_eq(self, other: Any) -> bool:
+        return (
+            isinstance(other, InMemoryScan)
+            and self._cache_entry == other._cache_entry
+            and self.schema() == other.schema()
+        )
+
+    def required_columns(self) -> list[set[str]]:
+        return [set()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [dict()]
+
+    def rebuild(self) -> LogicalPlan:
+        # if we are rebuilding, this will be cached when this is ran
+        return InMemoryScan(
+            cache_entry=self._cache_entry,
+            schema=self.schema(),
+            partition_spec=self.partition_spec(),
+        )
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 0
+        return self
+
+
+class FileWrite(UnaryNode):
+    def __init__(
+        self,
+        input: LogicalPlan,
+        root_dir: str | pathlib.Path,
+        storage_type: StorageType,
+        partition_cols: ExpressionsProjection | None = None,
+        compression: str | None = None,
+    ) -> None:
+        assert (
+            storage_type == StorageType.PARQUET or storage_type == StorageType.CSV
+        ), "only parquet and csv is supported currently"
+        self._storage_type = storage_type
+        self._root_dir = root_dir
+        self._compression = compression
+        if partition_cols is not None:
+            self._partition_cols = partition_cols
+        else:
+            self._partition_cols = ExpressionsProjection([])
+        for field in input.schema():
+            assert not field.dtype._is_python_type(), f"we can currently only write out primitive types, got: {field}"
+
+        schema = Schema._from_field_name_and_types([("file_path", DataType.string())])
+
+        super().__init__(schema, input.partition_spec(), op_level=OpLevel.PARTITION)
+        self._register_child(input)
+
+    def __repr__(self) -> str:
+        return self._repr_helper()
+
+    def required_columns(self) -> list[set[str]]:
+        return [self._partition_cols.required_columns()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [dict()]
+
+    def _local_eq(self, other: Any) -> bool:
+        return (
+            isinstance(other, FileWrite)
+            and self.schema() == other.schema()
+            and self._storage_type == other._storage_type
+            and self._root_dir == other._root_dir
+            and self._compression == other._compression
+        )
+
+    def rebuild(self) -> LogicalPlan:
+        raise NotImplementedError("We can not rebuild a filewrite due to side effects")
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return FileWrite(
+            new_children[0],
+            root_dir=self._root_dir,
+            storage_type=self._storage_type,
+            partition_cols=self._partition_cols,
+            compression=self._compression,
         )
 
 
 class Filter(UnaryNode):
     """Which rows to keep"""
 
-    def __init__(self, input: LogicalPlan, predicate: ExpressionList) -> None:
-        super().__init__(
-            input.schema().to_column_expressions(), partition_spec=input.partition_spec(), op_level=OpLevel.PARTITION
-        )
+    def __init__(self, input: LogicalPlan, predicate: ExpressionsProjection) -> None:
+        super().__init__(input.schema(), partition_spec=input.partition_spec(), op_level=OpLevel.PARTITION)
         self._register_child(input)
-        self._predicate = predicate.resolve(input.schema())
 
-        resolved_type = self._predicate.exprs[0].resolved_type()
-        if not ExpressionType.is_logical(resolved_type):
-            raise ValueError(
-                f"Expected expression {self._predicate.exprs[0]} to resolve to type LOGICAL, but received: {resolved_type}"
-            )
+        self._predicate = predicate
+        predicate_schema = predicate.resolve_schema(input.schema())
+
+        for resolved_field, predicate_expr in zip(predicate_schema, predicate):
+            resolved_type = resolved_field.dtype
+            if resolved_type != DataType.bool():
+                raise ValueError(
+                    f"Expected expression {predicate_expr} to resolve to type Boolean, but received: {resolved_type}"
+                )
 
     def __repr__(self) -> str:
-        return f"Filter\n\toutput={self.schema()}\n\tpredicate={self._predicate}"
+        return self._repr_helper(predicate=self._predicate)
 
-    def resource_request(self) -> ResourceRequest:
-        return self._predicate.resource_request()
+    def required_columns(self) -> list[set[str]]:
+        return [self._predicate.required_columns()]
 
-    def required_columns(self) -> ExpressionList:
-        return self._predicate.required_columns()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [{name: name for name in self.schema().column_names()}]
 
     def _local_eq(self, other: Any) -> bool:
         return isinstance(other, Filter) and self.schema() == other.schema() and self._predicate == other._predicate
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> Filter:
-        raise NotImplementedError()
-
     def rebuild(self) -> LogicalPlan:
-        return Filter(input=self._children()[0].rebuild(), predicate=self._predicate.unresolve())
+        return Filter(input=self._children()[0].rebuild(), predicate=self._predicate)
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return Filter(input=new_children[0], predicate=self._predicate)
 
 
 class Projection(UnaryNode):
     """Which columns to keep"""
 
-    def __init__(self, input: LogicalPlan, projection: ExpressionList) -> None:
-        projection = projection.resolve(input_schema=input.schema())
-        super().__init__(projection, partition_spec=input.partition_spec(), op_level=OpLevel.ROW)
+    def __init__(
+        self,
+        input: LogicalPlan,
+        projection: ExpressionsProjection,
+        custom_resource_request: ResourceRequest = ResourceRequest(),
+    ) -> None:
+        schema = projection.resolve_schema(input.schema())
+        super().__init__(schema, partition_spec=input.partition_spec(), op_level=OpLevel.ROW)
         self._register_child(input)
         self._projection = projection
+        self._custom_resource_request = custom_resource_request
+
+    def resource_request(self) -> ResourceRequest:
+        return self._custom_resource_request
 
     def __repr__(self) -> str:
-        return f"Projection\n\toutput={self.schema()}"
+        return self._repr_helper(output=list(self._projection))
 
-    def resource_request(self) -> ResourceRequest:
-        return self._projection.resource_request()
+    def required_columns(self) -> list[set[str]]:
+        return [self._projection.required_columns()]
 
-    def required_columns(self) -> ExpressionList:
-        return self._projection.required_columns()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [self._projection.input_mapping()]
 
     def _local_eq(self, other: Any) -> bool:
         return (
             isinstance(other, Projection) and self.schema() == other.schema() and self._projection == other._projection
         )
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> Projection:
-        return Projection(new_input, self._projection)
-
     def rebuild(self) -> LogicalPlan:
-        return Projection(input=self._children()[0].rebuild(), projection=self._projection.unresolve())
+        return Projection(
+            input=self._children()[0].rebuild(),
+            projection=self._projection,
+            custom_resource_request=self.resource_request(),
+        )
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return Projection(new_children[0], self._projection, custom_resource_request=self.resource_request())
 
 
 class Sort(UnaryNode):
-    def __init__(self, input: LogicalPlan, sort_by: ExpressionList, desc: bool = False) -> None:
+    def __init__(
+        self, input: LogicalPlan, sort_by: ExpressionsProjection, descending: list[bool] | bool = False
+    ) -> None:
         pspec = PartitionSpec(scheme=PartitionScheme.RANGE, num_partitions=input.num_partitions(), by=sort_by)
-        super().__init__(input.schema().to_column_expressions(), partition_spec=pspec, op_level=OpLevel.GLOBAL)
+        super().__init__(input.schema(), partition_spec=pspec, op_level=OpLevel.GLOBAL)
         self._register_child(input)
-        assert len(sort_by.exprs) == 1, "we can only sort with 1 expression"
-        self._sort_by = sort_by.resolve(input_schema=input.schema())
-        self._desc = desc
+        self._sort_by = sort_by
 
-    def __repr__(self) -> str:
-        return f"Sort\n\toutput={self.schema()}\n\tsort_by={self._sort_by}\n\tdesc={self._desc}"
+        resolved_sort_by_schema = self._sort_by.resolve_schema(input.schema())
+        for f, sort_by_expr in zip(resolved_sort_by_schema, self._sort_by):
+            if f.dtype == DataType.null() or f.dtype == DataType.binary() or f.dtype == DataType.bool():
+                raise ExpressionTypeError(f"Cannot sort on expression {sort_by_expr} with type: {f.dtype}")
 
-    def resource_request(self) -> ResourceRequest:
-        return self._sort_by.resource_request()
+        if isinstance(descending, bool):
+            self._descending = [descending for _ in self._sort_by]
+        else:
+            self._descending = descending
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> Sort:
-        return Sort(new_input, sort_by=self._sort_by, desc=self._desc)
+    def __repr__(self) -> str:
+        return self._repr_helper(sort_by=self._sort_by, desc=self._descending)
+
+    def required_columns(self) -> list[set[str]]:
+        return [self._sort_by.required_columns()]
 
-    def required_columns(self) -> ExpressionList:
-        return self._sort_by.required_columns()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [{name: name for name in self.schema().column_names()}]
 
     def _local_eq(self, other: Any) -> bool:
         return (
             isinstance(other, Sort)
             and self.schema() == other.schema()
-            and self._sort_by == self._sort_by
-            and self._desc == self._desc
+            and self._sort_by == other._sort_by
+            and self._descending == other._descending
+        )
+
+    def rebuild(self) -> LogicalPlan:
+        return Sort(input=self._children()[0].rebuild(), sort_by=self._sort_by, descending=self._descending)
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return Sort(new_children[0], sort_by=self._sort_by, descending=self._descending)
+
+
+TMapPartitionOp = TypeVar("TMapPartitionOp", bound=MapPartitionOp)
+
+
+class MapPartition(UnaryNode, Generic[TMapPartitionOp]):
+    def __init__(self, input: LogicalPlan, map_partition_op: TMapPartitionOp) -> None:
+        self._map_partition_op = map_partition_op
+        super().__init__(
+            self._map_partition_op.get_output_schema(),
+            partition_spec=input.partition_spec(),
+            op_level=OpLevel.PARTITION,
+        )
+        self._register_child(input)
+
+    def __repr__(self) -> str:
+        return self._repr_helper(op=self._map_partition_op)
+
+    def _local_eq(self, other: Any) -> bool:
+        return (
+            isinstance(other, MapPartition)
+            and self.schema() == other.schema()
+            and self._map_partition_op == other._map_partition_op
+        )
+
+    def eval_partition(self, partition: Table) -> Table:
+        return self._map_partition_op.run(partition)
+
+
+class Explode(MapPartition[ExplodeOp]):
+    def __init__(self, input: LogicalPlan, explode_expressions: ExpressionsProjection):
+        map_partition_op = ExplodeOp(input.schema(), explode_columns=explode_expressions)
+        super().__init__(
+            input,
+            map_partition_op,
         )
 
+    def __repr__(self) -> str:
+        return self._repr_helper()
+
+    def required_columns(self) -> list[set[str]]:
+        return [self._map_partition_op.explode_columns.required_columns()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        explode_columns = self._map_partition_op.explode_columns.input_mapping().keys()
+        return [{name: name for name in self.schema().column_names() if name not in explode_columns}]
+
     def rebuild(self) -> LogicalPlan:
-        return Sort(input=self._children()[0].rebuild(), sort_by=self._sort_by.unresolve(), desc=self._desc)
+        return Explode(
+            self._children()[0].rebuild(),
+            self._map_partition_op.explode_columns,
+        )
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return Explode(new_children[0], explode_expressions=self._map_partition_op.explode_columns)
 
 
 class LocalLimit(UnaryNode):
     def __init__(self, input: LogicalPlan, num: int) -> None:
         super().__init__(input.schema(), partition_spec=input.partition_spec(), op_level=OpLevel.PARTITION)
         self._register_child(input)
         self._num = num
 
     def __repr__(self) -> str:
-        return f"LocalLimit\n\toutput={self.schema()}\n\tN={self._num}"
+        return self._repr_helper(num=self._num)
 
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.default()
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return LocalLimit(new_children[0], self._num)
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> LocalLimit:
-        raise NotImplementedError()
+    def required_columns(self) -> list[set[str]]:
+        return [set()]
 
-    def required_columns(self) -> ExpressionList:
-        raise NotImplementedError()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [{name: name for name in self.schema().column_names()}]
 
     def _local_eq(self, other: Any) -> bool:
-        return isinstance(other, LocalLimit) and self.schema() == other.schema() and self._num == self._num
+        return isinstance(other, LocalLimit) and self.schema() == other.schema() and self._num == other._num
 
     def rebuild(self) -> LogicalPlan:
         return LocalLimit(input=self._children()[0].rebuild(), num=self._num)
 
 
 class GlobalLimit(UnaryNode):
     def __init__(self, input: LogicalPlan, num: int) -> None:
         super().__init__(input.schema(), partition_spec=input.partition_spec(), op_level=OpLevel.GLOBAL)
         self._register_child(input)
         self._num = num
 
     def __repr__(self) -> str:
-        return f"GlobalLimit\n\toutput={self.schema()}\n\tN={self._num}"
+        return self._repr_helper(num=self._num)
 
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.default()
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return GlobalLimit(new_children[0], self._num)
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> GlobalLimit:
-        raise NotImplementedError()
+    def required_columns(self) -> list[set[str]]:
+        return [set()]
 
-    def required_columns(self) -> ExpressionList:
-        raise NotImplementedError()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [{name: name for name in self.schema().column_names()}]
 
     def _local_eq(self, other: Any) -> bool:
-        return isinstance(other, GlobalLimit) and self.schema() == other.schema() and self._num == self._num
+        return isinstance(other, GlobalLimit) and self.schema() == other.schema() and self._num == other._num
 
     def rebuild(self) -> LogicalPlan:
         return GlobalLimit(input=self._children()[0].rebuild(), num=self._num)
 
 
+class LocalCount(UnaryNode):
+    def __init__(self, input: LogicalPlan) -> None:
+        schema = Schema._from_field_name_and_types([("count", DataType.int64())])
+        super().__init__(schema, partition_spec=input.partition_spec(), op_level=OpLevel.PARTITION)
+        self._register_child(input)
+
+    def __repr__(self) -> str:
+        return self._repr_helper()
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return LocalCount(new_children[0])
+
+    def required_columns(self) -> list[set[str]]:
+        # HACK: Arbitrarily return the first column in the child to ensure that
+        # at least one column is computed by the optimizer
+        return [{self._children()[0].schema().column_names()[0]}]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return []
+
+    def _local_eq(self, other: Any) -> bool:
+        return isinstance(other, LocalCount) and self.schema() == other.schema()
+
+    def rebuild(self) -> LogicalPlan:
+        return LocalCount(input=self._children()[0].rebuild())
+
+
 class PartitionScheme(Enum):
     UNKNOWN = "UNKNOWN"
     RANGE = "RANGE"
     HASH = "HASH"
     RANDOM = "RANDOM"
 
+    def __repr__(self) -> str:
+        return self.value
+
 
 @dataclass(frozen=True)
 class PartitionSpec:
     scheme: PartitionScheme
     num_partitions: int
-    by: Optional[ExpressionList] = None
+    by: ExpressionsProjection | None = None
 
 
 class Repartition(UnaryNode):
     def __init__(
-        self, input: LogicalPlan, partition_by: ExpressionList, num_partitions: int, scheme: PartitionScheme
+        self, input: LogicalPlan, partition_by: ExpressionsProjection, num_partitions: int, scheme: PartitionScheme
     ) -> None:
         pspec = PartitionSpec(
-            scheme=scheme, num_partitions=num_partitions, by=partition_by if len(partition_by) > 0 else None
+            scheme=scheme,
+            num_partitions=num_partitions,
+            by=partition_by if len(partition_by) > 0 else None,
         )
-        super().__init__(input.schema().to_column_expressions(), partition_spec=pspec, op_level=OpLevel.GLOBAL)
+        super().__init__(input.schema(), partition_spec=pspec, op_level=OpLevel.GLOBAL)
         self._register_child(input)
-        self._partition_by = partition_by.resolve(self.schema())
+        self._partition_by = partition_by
         self._scheme = scheme
-        if scheme == PartitionScheme.RANDOM and len(partition_by.names) > 0:
-            raise ValueError("Can not pass in random partitioning and partition_by args")
+        if scheme in (PartitionScheme.RANDOM, PartitionScheme.UNKNOWN) and len(partition_by.to_name_set()) > 0:
+            raise ValueError(f"Can not pass in {scheme} and partition_by args")
 
     def __repr__(self) -> str:
-        return (
-            f"Repartition\n\toutput={self.schema()}\n\tpartition_by={self._partition_by}"
-            f"\n\tnum_partitions={self.num_partitions()}\n\tscheme={self._scheme}"
+        return self._repr_helper(
+            partition_by=self._partition_by, num_partitions=self.num_partitions(), scheme=self._scheme
         )
 
-    def resource_request(self) -> ResourceRequest:
-        return self._partition_by.resource_request()
-
-    def copy_with_new_input(self, new_input: LogicalPlan) -> Repartition:
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
         return Repartition(
-            input=new_input,
+            input=new_children[0],
             partition_by=self._partition_by,
             num_partitions=self.num_partitions(),
             scheme=self._scheme,
         )
 
-    def required_columns(self) -> ExpressionList:
-        raise NotImplementedError()
+    def required_columns(self) -> list[set[str]]:
+        return [self._partition_by.required_columns()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [{name: name for name in self.schema().column_names()}]
 
     def _local_eq(self, other: Any) -> bool:
         return (
             isinstance(other, Repartition)
             and self.schema() == other.schema()
             and self._partition_by == other._partition_by
             and self._scheme == other._scheme
         )
 
     def rebuild(self) -> LogicalPlan:
         return Repartition(
             input=self._children()[0].rebuild(),
-            partition_by=self._partition_by.unresolve(),
+            partition_by=self._partition_by,
             num_partitions=self.num_partitions(),
             scheme=self._scheme,
         )
 
 
 class Coalesce(UnaryNode):
     def __init__(self, input: LogicalPlan, num_partitions: int) -> None:
         pspec = PartitionSpec(
             scheme=PartitionScheme.UNKNOWN,
             num_partitions=num_partitions,
         )
-        super().__init__(input.schema().to_column_expressions(), partition_spec=pspec, op_level=OpLevel.GLOBAL)
+        super().__init__(input.schema(), partition_spec=pspec, op_level=OpLevel.GLOBAL)
         self._register_child(input)
         if num_partitions > input.num_partitions():
             raise ValueError(
                 f"Coalesce can only reduce the number of partitions: {num_partitions} vs {input.num_partitions()}"
             )
 
     def __repr__(self) -> str:
-        return f"Coalesce\n\toutput={self.schema()}" f"\n\tnum_partitions={self.num_partitions()}"
+        return self._repr_helper(num_partitions=self.num_partitions())
 
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.default()
-
-    def copy_with_new_input(self, new_input: LogicalPlan) -> Coalesce:
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
         return Coalesce(
-            input=new_input,
+            input=new_children[0],
             num_partitions=self.num_partitions(),
         )
 
-    def required_columns(self) -> ExpressionList:
-        raise NotImplementedError()
+    def required_columns(self) -> list[set[str]]:
+        return [set()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [{name: name for name in self.schema().column_names()}]
 
     def _local_eq(self, other: Any) -> bool:
         return (
             isinstance(other, Coalesce)
             and self.schema() == other.schema()
             and self.num_partitions() == other.num_partitions()
         )
@@ -407,115 +770,157 @@
         )
 
 
 class LocalAggregate(UnaryNode):
     def __init__(
         self,
         input: LogicalPlan,
-        agg: List[Tuple[Expression, str]],
-        group_by: Optional[ExpressionList] = None,
+        agg: list[Expression],
+        group_by: ExpressionsProjection | None = None,
     ) -> None:
-
-        cols_to_agg = ExpressionList([e for e, _ in agg]).resolve(input.schema())
-        schema = cols_to_agg.to_column_expressions()
+        self._cols_to_agg = ExpressionsProjection(agg)
         self._group_by = group_by
 
         if group_by is not None:
-            self._group_by = group_by.resolve(input.schema())
-            schema = self._group_by.union(schema)
+            group_and_agg_cols = ExpressionsProjection(list(group_by) + agg)
+            schema = group_and_agg_cols.resolve_schema(input.schema())
+        else:
+            schema = self._cols_to_agg.resolve_schema(input.schema())
 
         super().__init__(schema, partition_spec=input.partition_spec(), op_level=OpLevel.PARTITION)
         self._register_child(input)
-        self._agg = [(e, op) for e, (_, op) in zip(cols_to_agg, agg)]
+        self._agg = agg
 
     def __repr__(self) -> str:
-        return f"LocalAggregate\n\toutput={self.schema()}\n\tgroup_by={self._group_by}"
+        return self._repr_helper(agg=self._agg, group_by=self._group_by)
 
-    def resource_request(self) -> ResourceRequest:
-        req = ResourceRequest.default()
-        if self._group_by is not None:
-            req = self._group_by.resource_request()
-        req = ResourceRequest.max_resources([expr.resource_request() for expr, _ in self._agg] + [req])
-        return req
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return LocalAggregate(new_children[0], agg=self._agg, group_by=self._group_by)
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> LocalAggregate:
-        raise NotImplementedError()
+    def required_columns(self) -> list[set[str]]:
+        required_cols = set(self._cols_to_agg.required_columns())
+        if self._group_by is not None:
+            required_cols = required_cols | set(self._group_by.required_columns())
+        return [required_cols]
 
-    def required_columns(self) -> ExpressionList:
-        raise NotImplementedError()
+    def input_mapping(self) -> list[dict[str, str]]:
+        if self._group_by is not None:
+            return [self._group_by.input_mapping()]
+        else:
+            return []
 
     def _local_eq(self, other: Any) -> bool:
         return (
             isinstance(other, LocalAggregate)
             and self.schema() == other.schema()
-            and self._agg == other._agg
+            and all(expr_structurally_equal(l, r) for l, r in zip(self._agg, other._agg))
             and self._group_by == other._group_by
         )
 
     def rebuild(self) -> LogicalPlan:
         return LocalAggregate(
             input=self._children()[0].rebuild(),
-            agg=[(e._unresolve(), op) for e, op in self._agg],
-            group_by=self._group_by.unresolve() if self._group_by is not None else None,
+            agg=self._agg,
+            group_by=self._group_by if self._group_by is not None else None,
         )
 
 
+class LocalDistinct(UnaryNode):
+    def __init__(
+        self,
+        input: LogicalPlan,
+        group_by: ExpressionsProjection,
+    ) -> None:
+
+        self._group_by = group_by
+        schema = group_by.resolve_schema(input.schema())
+        super().__init__(schema, partition_spec=input.partition_spec(), op_level=OpLevel.PARTITION)
+        self._register_child(input)
+
+    def __repr__(self) -> str:
+        return self._repr_helper(group_by=self._group_by)
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return LocalDistinct(new_children[0], group_by=self._group_by)
+
+    def required_columns(self) -> list[set[str]]:
+        return [self._group_by.required_columns()]
+
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [self._group_by.input_mapping()]
+
+    def _local_eq(self, other: Any) -> bool:
+        return (
+            isinstance(other, LocalDistinct) and self.schema() == other.schema() and self._group_by == other._group_by
+        )
+
+    def rebuild(self) -> LogicalPlan:
+        return LocalDistinct(input=self._children()[0].rebuild(), group_by=self._group_by)
+
+
 class HTTPRequest(LogicalPlan):
     def __init__(
         self,
-        schema: ExpressionList,
+        schema: Schema,
     ) -> None:
-        self._output_schema = schema.resolve()
+        self._output_schema = schema
         pspec = PartitionSpec(scheme=PartitionScheme.UNKNOWN, num_partitions=1)
         super().__init__(schema, partition_spec=pspec, op_level=OpLevel.ROW)
 
-    def schema(self) -> ExpressionList:
+    def schema(self) -> Schema:
         return self._output_schema
 
     def __repr__(self) -> str:
-        return f"HTTPRequest\n\toutput={self.schema()}"
+        return self._repr_helper()
 
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.default()
+    def required_columns(self) -> list[set[str]]:
+        raise NotImplementedError()
 
-    def required_columns(self) -> ExpressionList:
+    def input_mapping(self) -> list[dict[str, str]]:
         raise NotImplementedError()
 
     def _local_eq(self, other: Any) -> bool:
         return isinstance(other, HTTPRequest) and self.schema() == other.schema()
 
     def rebuild(self) -> LogicalPlan:
-        return HTTPRequest(schema=self.schema().unresolve())
+        return HTTPRequest(schema=self.schema())
+
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 0
+        return self
 
 
 class HTTPResponse(UnaryNode):
     def __init__(
         self,
         input: LogicalPlan,
     ) -> None:
         self._schema = input.schema()
         super().__init__(self._schema, partition_spec=input.partition_spec(), op_level=OpLevel.ROW)
 
-    def schema(self) -> ExpressionList:
+    def schema(self) -> Schema:
         return self._schema
 
     def __repr__(self) -> str:
-        return f"HTTPResponse\n\toutput={self.schema()}"
+        return self._repr_helper()
 
-    def resource_request(self) -> ResourceRequest:
-        return ResourceRequest.default()
+    def required_columns(self) -> list[set[str]]:
+        raise NotImplementedError()
 
-    def required_columns(self) -> ExpressionList:
+    def input_mapping(self) -> list[dict[str, str]]:
         raise NotImplementedError()
 
     def _local_eq(self, other: Any) -> bool:
         return isinstance(other, HTTPResponse) and self.schema() == other.schema()
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> HTTPResponse:
-        raise NotImplementedError()
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 1
+        return HTTPResponse(new_children[0])
 
     def rebuild(self) -> LogicalPlan:
         return HTTPResponse(
             input=self._children()[0].rebuild(),
         )
 
 
@@ -526,81 +931,101 @@
 
 
 class Join(BinaryNode):
     def __init__(
         self,
         left: LogicalPlan,
         right: LogicalPlan,
-        left_on: ExpressionList,
-        right_on: ExpressionList,
+        left_on: ExpressionsProjection,
+        right_on: ExpressionsProjection,
         how: JoinType = JoinType.INNER,
     ) -> None:
         assert len(left_on) == len(right_on), "left_on and right_on must match size"
 
         if not left.is_disjoint(right):
             right = right.rebuild()
             assert left.is_disjoint(right)
         num_partitions: int
-        self._left_on = left_on.resolve(left.schema())
-        self._right_on = right_on.resolve(right.schema())
+        self._left_on = left_on
+        self._right_on = right_on
+
+        for schema, exprs in ((left.schema(), self._left_on), (right.schema(), self._right_on)):
+            resolved_schema = exprs.resolve_schema(schema)
+            for f, expr in zip(resolved_schema, exprs):
+                if f.dtype == DataType.null():
+                    raise ExpressionTypeError(f"Cannot join on null type expression: {expr}")
+
         self._how = how
-        schema: ExpressionList
+        output_schema: Schema
         if how == JoinType.LEFT:
             num_partitions = left.num_partitions()
             raise NotImplementedError()
         elif how == JoinType.RIGHT:
             num_partitions = right.num_partitions()
             raise NotImplementedError()
         elif how == JoinType.INNER:
-            num_partitions = min(left.num_partitions(), right.num_partitions())
-            right_id_set = self._right_on.to_id_set()
-            filtered_right = [e for e in right.schema() if e.get_id() not in right_id_set]
-            schema = left.schema().union(ExpressionList(filtered_right), strict=False, rename_dup="right.")
+            num_partitions = max(left.num_partitions(), right.num_partitions())
+            right_drop_set = {r.name() for l, r in zip(left_on, right_on) if l.name() == r.name()}
+            left_columns = ExpressionsProjection.from_schema(left.schema())
+            right_columns = ExpressionsProjection([col(f.name) for f in right.schema() if f.name not in right_drop_set])
+            unioned_expressions = left_columns.union(right_columns, rename_dup="right.")
+            self._left_columns = left_columns
+            self._right_columns = ExpressionsProjection(list(unioned_expressions)[len(self._left_columns) :])
+            self._output_projection = unioned_expressions
+            output_schema = self._left_columns.resolve_schema(left.schema()).union(
+                self._right_columns.resolve_schema(right.schema())
+            )
 
-        left = Repartition(left, partition_by=self._left_on, num_partitions=num_partitions, scheme=PartitionScheme.HASH)
-        right = Repartition(
-            right, partition_by=self._right_on, num_partitions=num_partitions, scheme=PartitionScheme.HASH
+        left_pspec = PartitionSpec(scheme=PartitionScheme.HASH, num_partitions=num_partitions, by=self._left_on)
+        right_pspec = PartitionSpec(scheme=PartitionScheme.HASH, num_partitions=num_partitions, by=self._right_on)
+
+        new_left = Repartition(
+            left, partition_by=self._left_on, num_partitions=num_partitions, scheme=PartitionScheme.HASH
         )
 
-        super().__init__(
-            schema.to_column_expressions(), partition_spec=left.partition_spec(), op_level=OpLevel.PARTITION
+        if num_partitions == 1 and left.num_partitions() == 1:
+            left = left
+        elif left.partition_spec() != left_pspec:
+            left = new_left
+
+        new_right = Repartition(
+            right, partition_by=self._right_on, num_partitions=num_partitions, scheme=PartitionScheme.HASH
         )
+        if num_partitions == 1 and right.num_partitions() == 1:
+            right = right
+        elif right.partition_spec() != right_pspec:
+            right = new_right
+
+        super().__init__(output_schema, partition_spec=left.partition_spec(), op_level=OpLevel.PARTITION)
         self._register_child(left)
         self._register_child(right)
 
     def __repr__(self) -> str:
-        return (
-            f"Join\n\toutput={self.schema()}"
-            f"\n\tnum_partitions={self.num_partitions()}"
-            f"\n\tleft_on={self._left_on}"
-            f"\n\tright_on={self._right_on}"
-        )
+        return self._repr_helper(left_on=self._left_on, right_on=self._right_on, num_partitions=self.num_partitions())
 
-    def resource_request(self) -> ResourceRequest:
-        # Note that this join creates two Repartition LogicalPlans using the left_on and right_on ExpressionLists
-        # The Repartition LogicalPlans will have the (potentially) expensive ResourceRequests, but the Join itself
-        # after repartitioning is done should be relatively cheap.
-        return ResourceRequest.default()
+    def copy_with_new_children(self, new_children: list[LogicalPlan]) -> LogicalPlan:
+        assert len(new_children) == 2
+        return Join(new_children[0], new_children[1], left_on=self._left_on, right_on=self._right_on, how=self._how)
 
-    def copy_with_new_input(self, new_input: LogicalPlan) -> Coalesce:
-        raise NotImplementedError()
+    def required_columns(self) -> list[set[str]]:
+        return [self._left_on.required_columns(), self._right_on.required_columns()]
 
-    def required_columns(self) -> ExpressionList:
-        raise NotImplementedError()
+    def input_mapping(self) -> list[dict[str, str]]:
+        return [self._left_columns.input_mapping(), self._right_columns.input_mapping()]
 
     def _local_eq(self, other: Any) -> bool:
         return (
             isinstance(other, Join)
             and self.schema() == other.schema()
             and self._left_on == other._left_on
             and self._right_on == other._right_on
             and self.num_partitions() == other.num_partitions()
         )
 
     def rebuild(self) -> LogicalPlan:
         return Join(
             left=self._children()[0].rebuild(),
             right=self._children()[1].rebuild(),
-            left_on=self._left_on.unresolve(),
-            right_on=self._right_on.unresolve(),
+            left_on=self._left_on,
+            right_on=self._right_on,
             how=self._how,
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `getdaft-0.0.9/daft/runners/profiler.py` & `getdaft-0.1.0/daft/runners/profiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,44 @@
-import contextlib
+from __future__ import annotations
+
 import os
 from contextlib import contextmanager
 from typing import TYPE_CHECKING
 
 from loguru import logger
 
 if TYPE_CHECKING:
     from viztracer import VizTracer
 
+ACTIVE = False
+
 
-def profiler(filename: str) -> "VizTracer":
+@contextmanager
+def profiler(filename: str) -> VizTracer:
     if int(os.environ.get("DAFT_PROFILING", 0)) == 1:
-        from viztracer import VizTracer
+        from viztracer import VizTracer, get_tracer
+
+        global ACTIVE
+        if not ACTIVE:
+            tracer = get_tracer()
+            if tracer is None or tracer.output_file != filename:
+                tracer = VizTracer(output_file=filename, tracer_entries=10_000_000)
+            ACTIVE = True
+            with tracer:
+                yield tracer
+            ACTIVE = False
+            return
+        else:
+            tracer = get_tracer()
+            logger.warning(
+                f"profiler({filename}) not created. Another profiler({tracer.output_file}) is already active."
+            )
 
-        return VizTracer(output_file=filename, tracer_entries=10_000_000)
-    else:
-        return contextlib.nullcontext()
+    yield None
+    return
 
 
 import time
 
 
 @contextmanager
 def timingcontext(name: str):
```

