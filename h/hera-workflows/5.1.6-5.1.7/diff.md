# Comparing `tmp/hera_workflows-5.1.6.tar.gz` & `tmp/hera_workflows-5.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_workflows-5.1.6.tar", max compression
+gzip compressed data, was "hera_workflows-5.1.7.tar", max compression
```

## Comparing `hera_workflows-5.1.6.tar` & `hera_workflows-5.1.7.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0     1066 2023-04-25 10:18:01.094906 hera_workflows-5.1.6/LICENSE
--rw-r--r--   0        0        0    11696 2023-04-25 10:18:01.094906 hera_workflows-5.1.6/README.md
--rw-r--r--   0        0        0     3540 2023-04-25 10:18:21.495092 hera_workflows-5.1.6/pyproject.toml
--rw-r--r--   0        0        0      522 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/__init__.py
--rw-r--r--   0        0        0      310 2023-04-25 10:18:21.495092 hera_workflows-5.1.6/src/hera/_version.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/__init__.py
--rw-r--r--   0        0        0     3267 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.106907 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/models/sensor.pyi
--rw-r--r--   0        0        0    26811 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/events/service.py
--rw-r--r--   0        0        0      282 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/expr/__init__.py
--rw-r--r--   0        0        0    12021 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/expr/_node.py
--rw-r--r--   0        0        0      647 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/expr/_sprig.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/py.typed
--rw-r--r--   0        0        0      188 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/shared/__init__.py
--rw-r--r--   0        0        0      269 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/shared/_base_model.py
--rw-r--r--   0        0        0     4927 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/shared/_global_config.py
--rw-r--r--   0        0        0      513 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/shared/serialization.py
--rw-r--r--   0        0        0     4413 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/__init__.py
--rw-r--r--   0        0        0     2912 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/_context.py
--rw-r--r--   0        0        0    23864 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/_mixins.py
--rw-r--r--   0        0        0    32815 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/_unparse.py
--rw-r--r--   0        0        0       25 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/action.py
--rw-r--r--   0        0        0     1115 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/archive.py
--rw-r--r--   0        0        0     7697 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/artifact.py
--rw-r--r--   0        0        0     3446 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/container.py
--rw-r--r--   0        0        0     3988 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/container_set.py
--rw-r--r--   0        0        0     3763 2023-04-25 10:18:01.110906 hera_workflows-5.1.6/src/hera/workflows/cron_workflow.py
--rw-r--r--   0        0        0     2771 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/dag.py
--rw-r--r--   0        0        0     2186 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/data.py
--rw-r--r--   0        0        0     4855 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/env.py
--rw-r--r--   0        0        0     1329 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/env_from.py
--rw-r--r--   0        0        0      208 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/exceptions.py
--rw-r--r--   0        0        0     2291 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/http_template.py
--rw-r--r--   0        0        0       30 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/memoize.py
--rw-r--r--   0        0        0     6913 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/__init__.py
--rw-r--r--   0        0        0     1418 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/eventsource.py
--rw-r--r--   0        0        0      861 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/eventsource.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/google/__init__.py
--rw-r--r--   0        0        0      347 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/google/protobuf.py
--rw-r--r--   0        0        0      164 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/google/protobuf.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/grpc/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/grpc/gateway/__init__.py
--rw-r--r--   0        0        0      691 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/grpc/gateway/runtime.py
--rw-r--r--   0        0        0      470 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/grpc/gateway/runtime.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/events/__init__.py
--rw-r--r--   0        0        0   102993 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
--rw-r--r--   0        0        0    25271 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/workflow/__init__.py
--rw-r--r--   0        0        0   144549 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
--rw-r--r--   0        0        0    31958 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/core/__init__.py
--rw-r--r--   0        0        0   127883 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/core/v1.py
--rw-r--r--   0        0        0    18004 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/core/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/policy/__init__.py
--rw-r--r--   0        0        0     1751 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
--rw-r--r--   0        0        0      376 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0        0        0     3161 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
--rw-r--r--   0        0        0      105 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
--rw-r--r--   0        0        0        0 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0        0        0    22218 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
--rw-r--r--   0        0        0     2064 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
--rw-r--r--   0        0        0      144 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0        0        0      277 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
--rw-r--r--   0        0        0      108 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
--rw-r--r--   0        0        0     1453 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/sensor.py
--rw-r--r--   0        0        0      887 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/models/sensor.pyi
--rw-r--r--   0        0        0      722 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/operator.py
--rw-r--r--   0        0        0     4084 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/parameter.py
--rw-r--r--   0        0        0     1018 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/protocol.py
--rw-r--r--   0        0        0     2554 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/resource.py
--rw-r--r--   0        0        0     5262 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/resources.py
--rw-r--r--   0        0        0     1856 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/retry_strategy.py
--rw-r--r--   0        0        0     3707 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/runner.py
--rw-r--r--   0        0        0    14818 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/script.py
--rw-r--r--   0        0        0    49251 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/service.py
--rw-r--r--   0        0        0     9297 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/steps.py
--rw-r--r--   0        0        0     3266 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/suspend.py
--rw-r--r--   0        0        0    10501 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/task.py
--rw-r--r--   0        0        0       27 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/toleration.py
--rw-r--r--   0        0        0     2007 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/user_container.py
--rw-r--r--   0        0        0     2610 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/validators.py
--rw-r--r--   0        0        0    18656 2023-04-25 10:18:01.114907 hera_workflows-5.1.6/src/hera/workflows/volume.py
--rw-r--r--   0        0        0    15590 2023-04-25 10:18:01.118907 hera_workflows-5.1.6/src/hera/workflows/workflow.py
--rw-r--r--   0        0        0      911 2023-04-25 10:18:01.118907 hera_workflows-5.1.6/src/hera/workflows/workflow_status.py
--rw-r--r--   0        0        0     5925 2023-04-25 10:18:01.118907 hera_workflows-5.1.6/src/hera/workflows/workflow_template.py
--rw-r--r--   0        0        0    13280 1970-01-01 00:00:00.000000 hera_workflows-5.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-29 15:25:11.644935 hera_workflows-5.1.7/LICENSE
+-rw-r--r--   0        0        0    11696 2023-04-29 15:25:11.644935 hera_workflows-5.1.7/README.md
+-rw-r--r--   0        0        0     3540 2023-04-29 15:25:33.253157 hera_workflows-5.1.7/pyproject.toml
+-rw-r--r--   0        0        0      522 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/__init__.py
+-rw-r--r--   0        0        0      310 2023-04-29 15:25:33.257157 hera_workflows-5.1.7/src/hera/_version.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/__init__.py
+-rw-r--r--   0        0        0     3267 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.656935 hera_workflows-5.1.7/src/hera/events/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.660935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/models/sensor.pyi
+-rw-r--r--   0        0        0    26811 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/events/service.py
+-rw-r--r--   0        0        0      282 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/expr/__init__.py
+-rw-r--r--   0        0        0    12021 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/expr/_node.py
+-rw-r--r--   0        0        0      647 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/expr/_sprig.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/py.typed
+-rw-r--r--   0        0        0      188 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/shared/__init__.py
+-rw-r--r--   0        0        0      269 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/shared/_base_model.py
+-rw-r--r--   0        0        0     4927 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/shared/_global_config.py
+-rw-r--r--   0        0        0      513 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/shared/serialization.py
+-rw-r--r--   0        0        0     4413 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/__init__.py
+-rw-r--r--   0        0        0     2912 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/_context.py
+-rw-r--r--   0        0        0    23864 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/_mixins.py
+-rw-r--r--   0        0        0    32815 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/_unparse.py
+-rw-r--r--   0        0        0       25 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/action.py
+-rw-r--r--   0        0        0     1115 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/archive.py
+-rw-r--r--   0        0        0     7697 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/artifact.py
+-rw-r--r--   0        0        0     3446 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/container.py
+-rw-r--r--   0        0        0     3988 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/container_set.py
+-rw-r--r--   0        0        0     3763 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/cron_workflow.py
+-rw-r--r--   0        0        0     2771 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/dag.py
+-rw-r--r--   0        0        0     2186 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/data.py
+-rw-r--r--   0        0        0     4855 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/env.py
+-rw-r--r--   0        0        0     1329 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/env_from.py
+-rw-r--r--   0        0        0      208 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/exceptions.py
+-rw-r--r--   0        0        0     2291 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/http_template.py
+-rw-r--r--   0        0        0       30 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/memoize.py
+-rw-r--r--   0        0        0     6913 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/__init__.py
+-rw-r--r--   0        0        0     1418 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/eventsource.py
+-rw-r--r--   0        0        0      861 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/eventsource.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/google/__init__.py
+-rw-r--r--   0        0        0      347 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/google/protobuf.py
+-rw-r--r--   0        0        0      164 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/google/protobuf.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/grpc/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/grpc/gateway/__init__.py
+-rw-r--r--   0        0        0      691 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/grpc/gateway/runtime.py
+-rw-r--r--   0        0        0      470 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/grpc/gateway/runtime.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/events/__init__.py
+-rw-r--r--   0        0        0   102993 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.py
+-rw-r--r--   0        0        0    25271 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/workflow/__init__.py
+-rw-r--r--   0        0        0   144549 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py
+-rw-r--r--   0        0        0    31958 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/core/__init__.py
+-rw-r--r--   0        0        0   127883 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.py
+-rw-r--r--   0        0        0    18004 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/policy/__init__.py
+-rw-r--r--   0        0        0     1751 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py
+-rw-r--r--   0        0        0      376 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/policy/v1beta1.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0        0        0     3161 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py
+-rw-r--r--   0        0        0      105 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.pyi
+-rw-r--r--   0        0        0        0 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0        0        0    22218 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py
+-rw-r--r--   0        0        0     2064 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi
+-rw-r--r--   0        0        0      144 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0        0        0      277 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.py
+-rw-r--r--   0        0        0      108 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/util/intstr.pyi
+-rw-r--r--   0        0        0     1453 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/sensor.py
+-rw-r--r--   0        0        0      887 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/models/sensor.pyi
+-rw-r--r--   0        0        0      722 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/operator.py
+-rw-r--r--   0        0        0     4084 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/parameter.py
+-rw-r--r--   0        0        0     1018 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/protocol.py
+-rw-r--r--   0        0        0     2554 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/resource.py
+-rw-r--r--   0        0        0     5262 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/resources.py
+-rw-r--r--   0        0        0     1856 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/retry_strategy.py
+-rw-r--r--   0        0        0     3707 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/runner.py
+-rw-r--r--   0        0        0    14818 2023-04-29 15:25:11.664935 hera_workflows-5.1.7/src/hera/workflows/script.py
+-rw-r--r--   0        0        0    49251 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/service.py
+-rw-r--r--   0        0        0     9297 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/steps.py
+-rw-r--r--   0        0        0     3323 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/suspend.py
+-rw-r--r--   0        0        0    10501 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/task.py
+-rw-r--r--   0        0        0       27 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/toleration.py
+-rw-r--r--   0        0        0     2007 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/user_container.py
+-rw-r--r--   0        0        0     2610 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/validators.py
+-rw-r--r--   0        0        0    18656 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/volume.py
+-rw-r--r--   0        0        0    15572 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/workflow.py
+-rw-r--r--   0        0        0      911 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/workflow_status.py
+-rw-r--r--   0        0        0     5925 2023-04-29 15:25:11.668935 hera_workflows-5.1.7/src/hera/workflows/workflow_template.py
+-rw-r--r--   0        0        0    13280 1970-01-01 00:00:00.000000 hera_workflows-5.1.7/PKG-INFO
```

### Comparing `hera_workflows-5.1.6/LICENSE` & `hera_workflows-5.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/README.md` & `hera_workflows-5.1.7/README.md`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/pyproject.toml` & `hera_workflows-5.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "hera-workflows"  # project-name
 # The version is automatically substituted by the CI
-version = "5.1.6"
+version = "5.1.7"
 description = "Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows."
 authors = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 maintainers = ["Flaviu Vadan <flaviu.vadan@dynotx.com>", "Sambhav Kothari <sambhavs.email@gmail.com>", "Elliot Gunton <elliotgunton@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/argoproj-labs/hera"
 repository = "https://github.com/argoproj-labs/hera"
```

### Comparing `hera_workflows-5.1.6/src/hera/__init__.py` & `hera_workflows-5.1.7/src/hera/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/__init__.py` & `hera_workflows-5.1.7/src/hera/events/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/eventsource.py` & `hera_workflows-5.1.7/src/hera/events/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/eventsource.pyi` & `hera_workflows-5.1.7/src/hera/events/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/grpc/gateway/runtime.py` & `hera_workflows-5.1.7/src/hera/events/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/argoproj/events/v1alpha1.py` & `hera_workflows-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/argoproj/events/v1alpha1.pyi` & `hera_workflows-5.1.7/src/hera/events/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/argoproj/workflow/v1alpha1.py` & `hera_workflows-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi` & `hera_workflows-5.1.7/src/hera/events/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/core/v1.py` & `hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/core/v1.pyi` & `hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/k8s/api/policy/v1beta1.py` & `hera_workflows-5.1.7/src/hera/events/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera_workflows-5.1.7/src/hera/events/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/sensor.py` & `hera_workflows-5.1.7/src/hera/events/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/models/sensor.pyi` & `hera_workflows-5.1.7/src/hera/events/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/events/service.py` & `hera_workflows-5.1.7/src/hera/events/service.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/expr/_node.py` & `hera_workflows-5.1.7/src/hera/expr/_node.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/expr/_sprig.py` & `hera_workflows-5.1.7/src/hera/expr/_sprig.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/shared/_global_config.py` & `hera_workflows-5.1.7/src/hera/shared/_global_config.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/shared/serialization.py` & `hera_workflows-5.1.7/src/hera/shared/serialization.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/__init__.py` & `hera_workflows-5.1.7/src/hera/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/_context.py` & `hera_workflows-5.1.7/src/hera/workflows/_context.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/_mixins.py` & `hera_workflows-5.1.7/src/hera/workflows/_mixins.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/_unparse.py` & `hera_workflows-5.1.7/src/hera/workflows/_unparse.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/archive.py` & `hera_workflows-5.1.7/src/hera/workflows/archive.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/artifact.py` & `hera_workflows-5.1.7/src/hera/workflows/artifact.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/container.py` & `hera_workflows-5.1.7/src/hera/workflows/container.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/container_set.py` & `hera_workflows-5.1.7/src/hera/workflows/container_set.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/cron_workflow.py` & `hera_workflows-5.1.7/src/hera/workflows/cron_workflow.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/dag.py` & `hera_workflows-5.1.7/src/hera/workflows/dag.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/data.py` & `hera_workflows-5.1.7/src/hera/workflows/data.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/env.py` & `hera_workflows-5.1.7/src/hera/workflows/env.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/env_from.py` & `hera_workflows-5.1.7/src/hera/workflows/env_from.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/http_template.py` & `hera_workflows-5.1.7/src/hera/workflows/http_template.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/__init__.py` & `hera_workflows-5.1.7/src/hera/workflows/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/eventsource.py` & `hera_workflows-5.1.7/src/hera/workflows/models/eventsource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/eventsource.pyi` & `hera_workflows-5.1.7/src/hera/workflows/models/eventsource.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/grpc/gateway/runtime.py` & `hera_workflows-5.1.7/src/hera/workflows/models/grpc/gateway/runtime.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/events/v1alpha1.py` & `hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi` & `hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/events/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py` & `hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi` & `hera_workflows-5.1.7/src/hera/workflows/models/io/argoproj/workflow/v1alpha1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/core/v1.py` & `hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/core/v1.pyi` & `hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/core/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py` & `hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/api/policy/v1beta1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py` & `hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/api/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py` & `hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi` & `hera_workflows-5.1.7/src/hera/workflows/models/io/k8s/apimachinery/pkg/apis/meta/v1.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/sensor.py` & `hera_workflows-5.1.7/src/hera/workflows/models/sensor.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/models/sensor.pyi` & `hera_workflows-5.1.7/src/hera/workflows/models/sensor.pyi`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/operator.py` & `hera_workflows-5.1.7/src/hera/workflows/operator.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/parameter.py` & `hera_workflows-5.1.7/src/hera/workflows/parameter.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/protocol.py` & `hera_workflows-5.1.7/src/hera/workflows/protocol.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/resource.py` & `hera_workflows-5.1.7/src/hera/workflows/resource.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/resources.py` & `hera_workflows-5.1.7/src/hera/workflows/resources.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/retry_strategy.py` & `hera_workflows-5.1.7/src/hera/workflows/retry_strategy.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/runner.py` & `hera_workflows-5.1.7/src/hera/workflows/runner.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/script.py` & `hera_workflows-5.1.7/src/hera/workflows/script.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/service.py` & `hera_workflows-5.1.7/src/hera/workflows/service.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/steps.py` & `hera_workflows-5.1.7/src/hera/workflows/steps.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/suspend.py` & `hera_workflows-5.1.7/src/hera/workflows/suspend.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,25 +6,28 @@
 
 See https://argoproj.github.io/argo-workflows/intermediate-inputs/
 for more on intermediate parameters.
 
 """
 from typing import List, Optional, Union
 
-from hera.workflows._mixins import TemplateMixin
+from hera.workflows._mixins import CallableTemplateMixin, TemplateMixin
 from hera.workflows.models import (
     Inputs,
     Outputs,
     SuspendTemplate as _ModelSuspendTemplate,
     Template as _ModelTemplate,
 )
 from hera.workflows.parameter import Parameter
 
 
-class Suspend(TemplateMixin):
+class Suspend(
+    TemplateMixin,
+    CallableTemplateMixin,
+):
     """The Suspend template allows the user to pause a workflow for a specified length of time
     given by `duration` or indefinitely (i.e. until manually resumed). The Suspend template also
     allows you to specify `intermediate_parameters` which will replicate the given parameters to
     the "inputs" and "outputs" of the template, resulting in a Suspend template that pauses and
     waits for values from the user for the given list of parameters.
     """
```

### Comparing `hera_workflows-5.1.6/src/hera/workflows/task.py` & `hera_workflows-5.1.7/src/hera/workflows/task.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/user_container.py` & `hera_workflows-5.1.7/src/hera/workflows/user_container.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/validators.py` & `hera_workflows-5.1.7/src/hera/workflows/validators.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/volume.py` & `hera_workflows-5.1.7/src/hera/workflows/volume.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/workflow.py` & `hera_workflows-5.1.7/src/hera/workflows/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     PersistentVolumeClaim,
     PodDisruptionBudgetSpec,
     PodDNSConfig,
     PodGC,
     PodSecurityContext,
     RetryStrategy,
     Synchronization,
-    Template,
+    Template as _ModelTemplate,
     Time,
     Toleration,
     TTLStrategy,
     VolumeClaimGC,
     Workflow as _ModelWorkflow,
     WorkflowCreateRequest,
     WorkflowLintRequest,
@@ -67,16 +67,16 @@
     ContextMixin,
     HookMixin,
     VolumeMixin,
 ):
     """The base Workflow class for Hera.
 
     Workflow implements the contextmanager interface so allows usage of `with`, under which
-    any `hera.workflows.protocol.Templatable` object or `hera.workflows.models.Template` object
-    instantiated under the context will be added to the Workflow's list of templates.
+    any `hera.workflows.protocol.Templatable` object instantiated under the context will be
+    added to the Workflow's list of templates.
 
     Workflows can be created directly on your Argo cluster via `create`. They can also be dumped
     to yaml via `to_yaml` or built according to the Argo schema via `build` to get an OpenAPI model
     object.
     """
 
     # Workflow fields - https://argoproj.github.io/argo-workflows/fields/#workflow
@@ -131,16 +131,16 @@
     retry_strategy: Optional[RetryStrategy] = None
     scheduler_name: Optional[str] = None
     security_context: Optional[PodSecurityContext] = None
     service_account_name: Optional[str] = None
     shutdown: Optional[str] = None
     suspend: Optional[bool] = None
     synchronization: Optional[Synchronization] = None
-    template_defaults: Optional[Template] = None
-    templates: List[Union[Template, Templatable]] = []
+    template_defaults: Optional[_ModelTemplate] = None
+    templates: List[Union[_ModelTemplate, Templatable]] = []
     tolerations: Optional[List[Toleration]] = None
     ttl_strategy: Optional[TTLStrategy] = None
     volume_claim_gc: Optional[VolumeClaimGC] = None
     volume_claim_templates: Optional[List[PersistentVolumeClaim]] = None
     workflow_metadata: Optional[WorkflowMetadata] = None
     workflow_template_ref: Optional[WorkflowTemplateRef] = None
 
@@ -343,15 +343,15 @@
             WorkflowLintRequest(workflow=self.build()), namespace=self.namespace
         )
 
     def _add_sub(self, node: Any):
         """Adds any objects instantiated under the Workflow context manager that conform to the `Templatable` protocol
         or are Argo schema Template objects to the Workflow's list of templates.
         """
-        if not isinstance(node, (Templatable, *get_args(Template))):
+        if not isinstance(node, (Templatable, _ModelTemplate)):
             raise InvalidType(type(node))
         self.templates.append(node)
 
     def to_file(self, output_directory: Union[Path, str] = ".", name: str = "", *args, **kwargs) -> Path:
         """Writes the Workflow as an Argo schema Workflow object to a YAML file and returns the path to the file.
 
         Args:
```

### Comparing `hera_workflows-5.1.6/src/hera/workflows/workflow_status.py` & `hera_workflows-5.1.7/src/hera/workflows/workflow_status.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/src/hera/workflows/workflow_template.py` & `hera_workflows-5.1.7/src/hera/workflows/workflow_template.py`

 * *Files identical despite different names*

### Comparing `hera_workflows-5.1.6/PKG-INFO` & `hera_workflows-5.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera-workflows
-Version: 5.1.6
+Version: 5.1.7
 Summary: Hera is a Python framework for constructing and submitting Argo Workflows. The main goal of Hera is to make Argo Workflows more accessible by abstracting away some setup that is typically necessary for constructing Argo workflows.
 Home-page: https://github.com/argoproj-labs/hera
 License: MIT
 Author: Flaviu Vadan
 Author-email: flaviu.vadan@dynotx.com
 Maintainer: Flaviu Vadan
 Maintainer-email: flaviu.vadan@dynotx.com
```

