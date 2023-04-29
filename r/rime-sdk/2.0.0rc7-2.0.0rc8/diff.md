# Comparing `tmp/rime_sdk-2.0.0rc7.tar.gz` & `tmp/rime_sdk-2.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.0.0rc7.tar", last modified: Mon Apr 17 02:24:05 2023, max compression
+gzip compressed data, was "rime_sdk-2.0.0rc8.tar", last modified: Mon Apr 24 20:27:54 2023, max compression
```

## Comparing `rime_sdk-2.0.0rc7.tar` & `rime_sdk-2.0.0rc8.tar`

### file list

```diff
@@ -1,477 +1,483 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.300397 rime_sdk-2.0.0rc7/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57906 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.300397 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    22506 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28424 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    55004 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    45249 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.304397 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9413 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20482 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26951 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    50274 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41732 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    43398 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9732 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-17 02:24:02.000000 rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 02:24:05.300397 rime_sdk-2.0.0rc7/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31354 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 02:24:05.000000 rime_sdk-2.0.0rc7/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 02:24:05.340397 rime_sdk-2.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-17 02:23:25.000000 rime_sdk-2.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.191983 rime_sdk-2.0.0rc8/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58976 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.191983 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22506 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.195983 rime_sdk-2.0.0rc8/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58724 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.195983 rime_sdk-2.0.0rc8/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.195983 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.199983 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30381 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26951 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54931 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60397 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    43937 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/tags_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.191983 rime_sdk-2.0.0rc8/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31775 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/setup.py
```

### Comparing `rime_sdk-2.0.0rc7/LICENSE` & `rime_sdk-2.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/PKG-INFO` & `rime_sdk-2.0.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.0.0rc7/README.md` & `rime_sdk-2.0.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/__init__.py` & `rime_sdk-2.0.0rc8/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/client.py` & `rime_sdk-2.0.0rc8/rime_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 
 import importlib_metadata
 import pandas as pd
 from urllib3.util import Retry
 
 from rime_sdk.firewall import Firewall
 from rime_sdk.image_builder import ImageBuilder
-from rime_sdk.internal.config_parser import (
-    _get_profiling_config_swagger,
-    convert_test_run_config_to_swagger,
-)
+from rime_sdk.internal.config_parser import _get_uuid
 from rime_sdk.internal.file_upload import FileUploadModule
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.security_config_parser import (
     convert_model_info_to_dict,
     model_info_from_dict,
 )
 from rime_sdk.internal.throttle_queue import ThrottleQueue
 from rime_sdk.job import BaseJob, ContinuousTestJob, FileScanJob, ImageBuilderJob, Job
 from rime_sdk.project import Project
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import ApiClient
 from rime_sdk.swagger.swagger_client.models import (
+    ConfigvalidatorConfigTypeBody,
     ListImagesRequestPipLibraryFilter,
     ManagedImagePackageRequirement,
     ManagedImagePackageType,
     ManagedImagePipRequirement,
     ProjectCreateProjectRequest,
     RimeActorRole,
     RimeCreateImageRequest,
@@ -358,26 +356,30 @@
             )
         if model_task not in VALID_MODEL_TASKS:
             raise ValueError(
                 f"Invalid model task: '{model_task}'. "
                 f"Expected one of: {VALID_MODEL_TASKS}"
             )
         with RESTErrorHandler():
-            swagger_profiling = (
-                _get_profiling_config_swagger(profiling_config)
-                if profiling_config is not None
-                else None
-            )
+            if profiling_config:
+                with RESTErrorHandler():
+                    cv_api = swagger_client.ConfigValidatorApi(self._api_client)
+                    validate_body = ConfigvalidatorConfigTypeBody(
+                        config_json=json.dumps(profiling_config),
+                    )
+                    cv_api.config_validator_validate_test_config(
+                        config_type="CONFIG_TYPE_PROFILING", body=validate_body
+                    )
             body = ProjectCreateProjectRequest(
                 name=name,
                 description=description,
                 model_task=model_task,
                 use_case=use_case,
                 ethical_consideration=ethical_consideration,
-                profiling_config=swagger_profiling,
+                profiling_config=profiling_config,
             )
             response = api.project_service_create_project(body=body)
 
             if general_access_role != "ACTOR_ROLE_NONE":
                 role_pairs = [
                     RimeParentRoleSubjectRolePair(
                         parent_role=RimeActorRole.ADMIN,
@@ -906,20 +908,35 @@
         self._check_stress_test_limit()
         # TODO(blaine): Add config validation service.
         if not isinstance(test_run_config, dict):
             raise ValueError("The configuration must be a dictionary")
         # TODO (VAL-316): do proper runtime validation of all of the types in the config
         if project_id and not self._project_exists(project_id):
             raise ValueError("Project id {} does not exist".format(project_id))
-        swagger_test_run_config = convert_test_run_config_to_swagger(test_run_config)
-        req = StresstestsProjectIdUuidBody(
-            test_run_config=swagger_test_run_config,
-            experimental_fields=exp_fields if exp_fields else None,
-        )
+        if "model_id" in test_run_config:
+            if isinstance(test_run_config["model_id"], str):
+                test_run_config["model_id"] = _get_uuid(test_run_config["model_id"])
+        if "run_time_info" in test_run_config:
+            if "agent_id" in test_run_config["run_time_info"]:
+                if isinstance(test_run_config["run_time_info"]["agent_id"], str):
+                    test_run_config["run_time_info"]["agent_id"] = _get_uuid(
+                        test_run_config["run_time_info"]["agent_id"]
+                    )
+        cv_api = swagger_client.ConfigValidatorApi(self._api_client)
         with RESTErrorHandler():
+            validate_body = ConfigvalidatorConfigTypeBody(
+                config_json=json.dumps(test_run_config),
+            )
+            cv_api.config_validator_validate_test_config(
+                config_type="CONFIG_TYPE_TEST_RUN", body=validate_body
+            )
+            req = StresstestsProjectIdUuidBody(
+                test_run_config=test_run_config,
+                experimental_fields=exp_fields if exp_fields else None,
+            )
             Client._throttler.throttle(
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_stress_test(
                 body=req, project_id_uuid=project_id,
             ).job
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/data_collector.py` & `rime_sdk-2.0.0rc8/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/detection_event.py` & `rime_sdk-2.0.0rc8/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/firewall.py` & `rime_sdk-2.0.0rc8/rime_sdk/firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/image_builder.py` & `rime_sdk-2.0.0rc8/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/constants.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/decorators.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/file_upload.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/internal/utils.py` & `rime_sdk-2.0.0rc8/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/job.py` & `rime_sdk-2.0.0rc8/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/monitor.py` & `rime_sdk-2.0.0rc8/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/project.py` & `rime_sdk-2.0.0rc8/rime_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """Library defining the interface to a Project."""
+import json
 from datetime import timedelta
 from http import HTTPStatus
 from typing import Any, Dict, Iterator, List, NamedTuple, Optional
 
 from google.protobuf.field_mask_pb2 import FieldMask
 from google.protobuf.json_format import MessageToDict
 
 from rime_sdk.data_collector import DataCollector
 from rime_sdk.firewall import Firewall
-from rime_sdk.internal.config_parser import (
-    _get_data_profiling_swagger,
-    _get_model_profiling_swagger,
-    _get_test_suite_config_swagger,
-)
+from rime_sdk.internal.config_parser import _get_individual_tests_config_swagger
 from rime_sdk.internal.decorators import prompt_confirmation
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.swagger_utils import get_data_location_swagger, timedelta_to_rest
 from rime_sdk.internal.utils import (
     convert_dict_to_html,
     get_swagger_field_mask,
     make_link,
@@ -27,14 +24,15 @@
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
     CreateFirewallRequestScheduledCTParameters,
     RimeCreateFirewallRequest,
     RimeUUID,
 )
 from rime_sdk.swagger.swagger_client.models import (
+    ConfigvalidatorConfigTypeBody,
     DigestConfigDigestFrequency,
     NotificationDigestConfig,
     NotificationJobActionConfig,
     NotificationMonitoringConfig,
     NotificationNotificationType,
     NotificationObjectType,
     NotificationWebhookConfig,
@@ -882,14 +880,15 @@
     def register_model(
         self,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
+        integration_id: Optional[str] = None,
     ) -> str:
         """Register a new model in this Project.
 
         Args:
             name: str
                 The chosen name of the model.
             model_config: Optional[dict] = None,
@@ -899,14 +898,17 @@
                 request.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the model.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
+            integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration for access.
 
         Returns:
             str:
                 The ID of the newly registered model.
 
         Raises:
             ValueError
@@ -936,37 +938,42 @@
         return self._registry.register_model(
             self.project_id,
             name,
             model_config=model_config,
             tags=tags,
             metadata=metadata,
             external_id=external_id,
+            integration_id=integration_id,
         )
 
     def register_model_from_path(
         self,
         name: str,
         remote_path: str,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
+        integration_id: Optional[str] = None,
     ) -> str:
         """Register a new model in this Project.
 
         Args:
             name: str
                 The chosen name of the model.
             remote_path: str
                 The path to the model artifact.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the model.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
+            integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration for access.
 
         Returns:
             str:
                 The ID of the newly registered model.
 
         Raises:
             ValueError
@@ -985,14 +992,15 @@
         return self._registry.register_model(
             self.project_id,
             name,
             model_config,
             tags=tags,
             metadata=metadata,
             external_id=external_id,
+            integration_id=integration_id,
         )
 
     def register_predictions(
         self,
         dataset_id: str,
         model_id: str,
         pred_config: dict,
@@ -1354,32 +1362,91 @@
         Raises:
             ValueError:
                 This error is generated when the request to the Registry
                 service fails.
         """
         self._registry.delete_predictions(model_id, dataset_id)
 
+    def update_stress_test_categories(self, categories: List[str]) -> None:
+        """Update the project's stress test categories.
+
+        Args:
+            categories: List[str]
+                The list of stress test categories to update.
+
+        Returns:
+            None
+
+        Raises:
+            ValueError
+                This error is generated when the request to the Project service fails.
+        """
+        project = ProjectProject(stress_test_categories=categories)
+        body = ProjectsProjectIdUuidBody(
+            project_id=RimeUUID(uuid=self._project_id),
+            project=project,
+            mask=get_swagger_field_mask(project),
+        )
+        api = swagger_client.ProjectServiceApi(self._api_client)
+        with RESTErrorHandler():
+            api.project_service_update_project(
+                body=body, project_id_uuid=self._project_id
+            )
+
+    def update_continuous_test_categories(self, categories: List[str]) -> None:
+        """Update the project's continuous test categories.
+
+        Args:
+            categories: List[str]
+                The list of continuous test categories to update.
+
+        Returns:
+            None
+
+        Raises:
+            ValueError
+                This error is generated when the request to the Project service fails.
+        """
+        project = ProjectProject(continuous_test_categories=categories)
+        body = ProjectsProjectIdUuidBody(
+            project_id=RimeUUID(uuid=self._project_id),
+            project=project,
+            mask=get_swagger_field_mask(project),
+        )
+        api = swagger_client.ProjectServiceApi(self._api_client)
+        with RESTErrorHandler():
+            api.project_service_update_project(
+                body=body, project_id_uuid=self._project_id
+            )
+
     def update_model_profiling_config(self, model_profiling_config: dict) -> None:
         """Update the project's model profiling configuration.
 
         Args:
             model_profiling_config: dict
                 Model profiling configuration with which to update the project.
 
         Returns:
             None
 
         Raises:
             ValueError
                 This error is generated when the request to the Project service fails.
         """
-        swagger_model_profiling = _get_model_profiling_swagger(model_profiling_config)
+        with RESTErrorHandler():
+            cv_api = swagger_client.ConfigValidatorApi(self._api_client)
+            validate_body = ConfigvalidatorConfigTypeBody(
+                config_json=json.dumps(model_profiling_config),
+            )
+            cv_api.config_validator_validate_test_config(
+                config_type="CONFIG_TYPE_MODEL_PROFILING", body=validate_body
+            )
         project = ProjectProject(
             profiling_config=TestrunProfilingConfig(
-                model_profiling=swagger_model_profiling
+                model_profiling=model_profiling_config
             )
         )
         body = ProjectsProjectIdUuidBody(
             project_id=RimeUUID(uuid=self._project_id),
             project=project,
             mask=get_swagger_field_mask(project),
         )
@@ -1399,18 +1466,25 @@
         Returns:
             None
 
         Raises:
             ValueError
                 This error is generated when the request to the Project service fails.
         """
-        swagger_data_profiling = _get_data_profiling_swagger(data_profiling_config)
+        with RESTErrorHandler():
+            cv_api = swagger_client.ConfigValidatorApi(self._api_client)
+            validate_body = ConfigvalidatorConfigTypeBody(
+                config_json=json.dumps(data_profiling_config),
+            )
+            cv_api.config_validator_validate_test_config(
+                config_type="CONFIG_TYPE_DATA_PROFILING", body=validate_body
+            )
         project = ProjectProject(
             profiling_config=TestrunProfilingConfig(
-                data_profiling=swagger_data_profiling
+                data_profiling=data_profiling_config
             )
         )
         body = ProjectsProjectIdUuidBody(
             project_id=RimeUUID(uuid=self._project_id),
             project=project,
             mask=get_swagger_field_mask(project),
         )
@@ -1430,19 +1504,35 @@
         Returns:
             None
 
         Raises:
             ValueError
                 This error is generated when the request to the Project service fails.
         """
-        swagger_test_suite_config = _get_test_suite_config_swagger(test_suite_config)
-        project = ProjectProject(project_test_suite_config=swagger_test_suite_config)
-        body = ProjectsProjectIdUuidBody(
-            project_id=RimeUUID(uuid=self._project_id),
-            project=project,
-            mask=get_swagger_field_mask(project),
-        )
-        api = swagger_client.ProjectServiceApi(self._api_client)
+        cv_api = swagger_client.ConfigValidatorApi(self._api_client)
+        # We allow users to specify the individual tests config as a dict, but the BE
+        # expects a JSON string.
+        if "individual_tests_config" in test_suite_config:
+            # Allow the user to pass in a JSON string as well as a dict.
+            if isinstance(test_suite_config["individual_tests_config"], dict):
+                test_suite_config[
+                    "individual_tests_config"
+                ] = _get_individual_tests_config_swagger(
+                    test_suite_config["individual_tests_config"]
+                )
         with RESTErrorHandler():
+            validate_body = ConfigvalidatorConfigTypeBody(
+                config_json=json.dumps(test_suite_config),
+            )
+            cv_api.config_validator_validate_test_config(
+                config_type="CONFIG_TYPE_TEST_SUITE", body=validate_body
+            )
+            project = ProjectProject(project_test_suite_config=test_suite_config)
+            body = ProjectsProjectIdUuidBody(
+                project_id=RimeUUID(uuid=self._project_id),
+                project=project,
+                mask=get_swagger_field_mask(project),
+            )
+            api = swagger_client.ProjectServiceApi(self._api_client)
             api.project_service_update_project(
                 body=body, project_id_uuid=self._project_id
             )
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/registry.py` & `rime_sdk-2.0.0rc8/rime_sdk/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,15 @@
         self,
         project_id: str,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
+        integration_id: Optional[str] = None,
     ) -> str:
         """Register a new model in a Project.
 
         Args:
             project_id: str
                 The ID of the Project in which to register the model.
             name: str
@@ -139,14 +140,17 @@
                 request.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the model.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
+            integration_id: Optional[str] = None,
+                Provide the integration ID for models that require an
+                integration for access.
 
         Returns:
             str:
                 The ID of the newly registered model.
 
         Raises:
             ValueError
@@ -194,14 +198,16 @@
         metadata_str: Optional[str] = None
         if metadata:
             metadata_str = json.dumps(metadata)
         if tags or metadata_str:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
         if external_id:
             req.external_id = external_id
+        if integration_id is not None:
+            req.integration_id = RimeUUID(uuid=integration_id)
 
         with RESTErrorHandler():
             api = swagger_client.RegistryServiceApi(self._api_client)
             res = api.registry_service_register_model(
                 body=req, project_id_uuid=project_id,
             )
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
 from rime_sdk.swagger.swagger_client.api.agent_manager_api import AgentManagerApi
+from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
@@ -38,14 +39,15 @@
 # import ApiClient
 from rime_sdk.swagger.swagger_client.api_client import ApiClient
 from rime_sdk.swagger.swagger_client.configuration import Configuration
 # import models into sdk package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
+from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
@@ -67,14 +69,15 @@
 from rime_sdk.swagger.swagger_client.models.detection_event_type import DetectionEventType
 from rime_sdk.swagger.swagger_client.models.detection_metric_degradation_event_details import DetectionMetricDegradationEventDetails
 from rime_sdk.swagger.swagger_client.models.detection_resolution import DetectionResolution
 from rime_sdk.swagger.swagger_client.models.detection_security_event_details import DetectionSecurityEventDetails
 from rime_sdk.swagger.swagger_client.models.difference_from_target_difference import DifferenceFromTargetDifference
 from rime_sdk.swagger.swagger_client.models.difference_from_target_target import DifferenceFromTargetTarget
 from rime_sdk.swagger.swagger_client.models.digest_config_digest_frequency import DigestConfigDigestFrequency
+from rime_sdk.swagger.swagger_client.models.featureflags_customer_name_body import FeatureflagsCustomerNameBody
 from rime_sdk.swagger.swagger_client.models.filescanning_file_scan_result import FilescanningFileScanResult
 from rime_sdk.swagger.swagger_client.models.filescanning_huggingface_model_info import FilescanningHuggingfaceModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_model_file_info import FilescanningModelFileInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_pytorch_model_info import FilescanningPytorchModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_custom_loader_location import FirewallCustomLoaderLocation
@@ -179,15 +182,14 @@
 from rime_sdk.swagger.swagger_client.models.rename_test_run_id_body import RenameTestRunIdBody
 from rime_sdk.swagger.swagger_client.models.resetpassword_user_id_uuid_body import ResetpasswordUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.rime_api_token_info import RimeAPITokenInfo
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_agent import RimeAgent
 from rime_sdk.swagger.swagger_client.models.rime_agent_status import RimeAgentStatus
-from rime_sdk.swagger.swagger_client.models.rime_archived_job_logs import RimeArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.rime_cancel_job_response import RimeCancelJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_category_metric import RimeCategoryMetric
 from rime_sdk.swagger.swagger_client.models.rime_category_test_result import RimeCategoryTestResult
 from rime_sdk.swagger.swagger_client.models.rime_config_type import RimeConfigType
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_request_integration_variable import RimeConfigureIntegrationRequestIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_response import RimeConfigureIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_job_progress import RimeContinuousTestJobProgress
@@ -199,14 +201,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_create_custom_monitor_response import RimeCreateCustomMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_request import RimeCreateFirewallRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_response import RimeCreateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_image_request import RimeCreateImageRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_image_response import RimeCreateImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_request import RimeCreateIntegrationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_response import RimeCreateIntegrationResponse
+from rime_sdk.swagger.swagger_client.models.rime_create_model_card_request import RimeCreateModelCardRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_response import RimeCreateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_request import RimeCreateNotificationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_response import RimeCreateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_user_request import RimeCreateUserRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_user_response import RimeCreateUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_request import RimeCreateWorkspaceRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_response import RimeCreateWorkspaceResponse
@@ -339,14 +342,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_test_metric_category import RimeTestMetricCategory
 from rime_sdk.swagger.swagger_client.models.rime_test_run_progress import RimeTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_test_task_status import RimeTestTaskStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_type import RimeTestType
 from rime_sdk.swagger.swagger_client.models.rime_time_interval import RimeTimeInterval
 from rime_sdk.swagger.swagger_client.models.rime_token_type import RimeTokenType
 from rime_sdk.swagger.swagger_client.models.rime_uuid import RimeUUID
+from rime_sdk.swagger.swagger_client.models.rime_update_build_info_request import RimeUpdateBuildInfoRequest
 from rime_sdk.swagger.swagger_client.models.rime_update_build_info_response import RimeUpdateBuildInfoResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_firewall_response import RimeUpdateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_integration_response import RimeUpdateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_model_card_response import RimeUpdateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_monitor_response import RimeUpdateMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_notification_response import RimeUpdateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_user_of_workspace_response import RimeUpdateUserOfWorkspaceResponse
@@ -371,19 +375,21 @@
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
+from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.stresstests_project_id_uuid_body import StresstestsProjectIdUuidBody
+from rime_sdk.swagger.swagger_client.models.tags_name_body import TagsNameBody
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_category_summary_metric import TestRunMetricsCategorySummaryMetric
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_model_perf_metric import TestRunMetricsModelPerfMetric
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
 from rime_sdk.swagger.swagger_client.models.testrun_connection_info import TestrunConnectionInfo
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
 from rime_sdk.swagger.swagger_client.models.testrun_data_collector_info import TestrunDataCollectorInfo
@@ -395,15 +401,14 @@
 from rime_sdk.swagger.swagger_client.models.testrun_delta_lake_info import TestrunDeltaLakeInfo
 from rime_sdk.swagger.swagger_client.models.testrun_hugging_face_data_info import TestrunHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.testrun_model_profiling import TestrunModelProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_pred_info import TestrunPredInfo
 from rime_sdk.swagger.swagger_client.models.testrun_prediction_params import TestrunPredictionParams
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import TestrunProfilingConfig
 from rime_sdk.swagger.swagger_client.models.testrun_single_data_info import TestrunSingleDataInfo
-from rime_sdk.swagger.swagger_client.models.testrun_test_category import TestrunTestCategory
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
@@ -434,9 +439,10 @@
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body1 import UsersUserUserIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.v1betaintegrationsintegration_id_uuid_integration import V1betaintegrationsintegrationIdUuidIntegration
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
+from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_tags_body import WorkspaceIdUuidTagsBody
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
 from rime_sdk.swagger.swagger_client.api.agent_manager_api import AgentManagerApi
+from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,60 +16,60 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from rime_sdk.swagger.swagger_client.api_client import ApiClient
 
 
-class AgentManagerApi(object):
+class ImageRegistryApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def agent_manager_create_agent(self, body, **kwargs):  # noqa: E501
-        """CreateAgent  # noqa: E501
+    def image_registry_create_image(self, body, **kwargs):  # noqa: E501
+        """CreateImage  # noqa: E501
 
-        Creates agent and returns the configuration for installing the agent.  # noqa: E501
+        Creates a new Managed Image with a unique name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_create_agent(body, async_req=True)
+        >>> thread = api.image_registry_create_image(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeCreateAgentRequest body: (required)
-        :return: RimeCreateAgentResponse
+        :param RimeCreateImageRequest body: (required)
+        :return: RimeCreateImageResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.agent_manager_create_agent_with_http_info(body, **kwargs)  # noqa: E501
+            return self.image_registry_create_image_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.agent_manager_create_agent_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.image_registry_create_image_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def agent_manager_create_agent_with_http_info(self, body, **kwargs):  # noqa: E501
-        """CreateAgent  # noqa: E501
+    def image_registry_create_image_with_http_info(self, body, **kwargs):  # noqa: E501
+        """CreateImage  # noqa: E501
 
-        Creates agent and returns the configuration for installing the agent.  # noqa: E501
+        Creates a new Managed Image with a unique name.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_create_agent_with_http_info(body, async_req=True)
+        >>> thread = api.image_registry_create_image_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeCreateAgentRequest body: (required)
-        :return: RimeCreateAgentResponse
+        :param RimeCreateImageRequest body: (required)
+        :return: RimeCreateImageResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -77,22 +77,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method agent_manager_create_agent" % key
+                    " to method image_registry_create_image" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `agent_manager_create_agent`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `image_registry_create_image`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -112,92 +112,92 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/agents', 'POST',
+            '/v1/images', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeCreateAgentResponse',  # noqa: E501
+            response_type='RimeCreateImageResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def agent_manager_deactivate_agent(self, agent_id_uuid, **kwargs):  # noqa: E501
-        """DeactivateAgent  # noqa: E501
+    def image_registry_delete_image(self, name, **kwargs):  # noqa: E501
+        """DeleteImage  # noqa: E501
 
-        Deactivates the agent by setting its status to deactivated and revoking the agent's API Token. An error is returned if the deactivation fails.  # noqa: E501
+        Deletes a specified Managed Image.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_deactivate_agent(agent_id_uuid, async_req=True)
+        >>> thread = api.image_registry_delete_image(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str agent_id_uuid: Unique object ID. (required)
-        :return: RimeDeactivateAgentResponse
+        :param str name: Name of existing Managed Image to delete. (required)
+        :return: RimeDeleteImageResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.agent_manager_deactivate_agent_with_http_info(agent_id_uuid, **kwargs)  # noqa: E501
+            return self.image_registry_delete_image_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.agent_manager_deactivate_agent_with_http_info(agent_id_uuid, **kwargs)  # noqa: E501
+            (data) = self.image_registry_delete_image_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def agent_manager_deactivate_agent_with_http_info(self, agent_id_uuid, **kwargs):  # noqa: E501
-        """DeactivateAgent  # noqa: E501
+    def image_registry_delete_image_with_http_info(self, name, **kwargs):  # noqa: E501
+        """DeleteImage  # noqa: E501
 
-        Deactivates the agent by setting its status to deactivated and revoking the agent's API Token. An error is returned if the deactivation fails.  # noqa: E501
+        Deletes a specified Managed Image.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_deactivate_agent_with_http_info(agent_id_uuid, async_req=True)
+        >>> thread = api.image_registry_delete_image_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str agent_id_uuid: Unique object ID. (required)
-        :return: RimeDeactivateAgentResponse
+        :param str name: Name of existing Managed Image to delete. (required)
+        :return: RimeDeleteImageResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['agent_id_uuid']  # noqa: E501
+        all_params = ['name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method agent_manager_deactivate_agent" % key
+                    " to method image_registry_delete_image" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'agent_id_uuid' is set
-        if ('agent_id_uuid' not in params or
-                params['agent_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `agent_id_uuid` when calling `agent_manager_deactivate_agent`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `image_registry_delete_image`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'agent_id_uuid' in params:
-            path_params['agentId.uuid'] = params['agent_id_uuid']  # noqa: E501
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -207,92 +207,92 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/agents/deactivate/{agentId.uuid}', 'PUT',
+            '/v1/images/{name}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeDeactivateAgentResponse',  # noqa: E501
+            response_type='RimeDeleteImageResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def agent_manager_delete_agent(self, agent_id_uuid, **kwargs):  # noqa: E501
-        """DeleteAgent  # noqa: E501
+    def image_registry_get_image(self, name, **kwargs):  # noqa: E501
+        """GetImage  # noqa: E501
 
-        Deletes a specified agent. Must be called on an already deactivated agent. An error is returned if the deletion fails or if the agent is not in a deletable state.  # noqa: E501
+        Returns the definition of a specified Managed Image.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_delete_agent(agent_id_uuid, async_req=True)
+        >>> thread = api.image_registry_get_image(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str agent_id_uuid: Unique object ID. (required)
-        :return: RimeDeleteAgentResponse
+        :param str name: Name of the existing Managed Image. (required)
+        :return: RimeGetImageResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.agent_manager_delete_agent_with_http_info(agent_id_uuid, **kwargs)  # noqa: E501
+            return self.image_registry_get_image_with_http_info(name, **kwargs)  # noqa: E501
         else:
-            (data) = self.agent_manager_delete_agent_with_http_info(agent_id_uuid, **kwargs)  # noqa: E501
+            (data) = self.image_registry_get_image_with_http_info(name, **kwargs)  # noqa: E501
             return data
 
-    def agent_manager_delete_agent_with_http_info(self, agent_id_uuid, **kwargs):  # noqa: E501
-        """DeleteAgent  # noqa: E501
+    def image_registry_get_image_with_http_info(self, name, **kwargs):  # noqa: E501
+        """GetImage  # noqa: E501
 
-        Deletes a specified agent. Must be called on an already deactivated agent. An error is returned if the deletion fails or if the agent is not in a deletable state.  # noqa: E501
+        Returns the definition of a specified Managed Image.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_delete_agent_with_http_info(agent_id_uuid, async_req=True)
+        >>> thread = api.image_registry_get_image_with_http_info(name, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str agent_id_uuid: Unique object ID. (required)
-        :return: RimeDeleteAgentResponse
+        :param str name: Name of the existing Managed Image. (required)
+        :return: RimeGetImageResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['agent_id_uuid']  # noqa: E501
+        all_params = ['name']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method agent_manager_delete_agent" % key
+                    " to method image_registry_get_image" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'agent_id_uuid' is set
-        if ('agent_id_uuid' not in params or
-                params['agent_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `agent_id_uuid` when calling `agent_manager_delete_agent`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `image_registry_get_image`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'agent_id_uuid' in params:
-            path_params['agentId.uuid'] = params['agent_id_uuid']  # noqa: E501
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -302,94 +302,94 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/agents/{agentId.uuid}', 'DELETE',
+            '/v1/images/{name}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeDeleteAgentResponse',  # noqa: E501
+            response_type='RimeGetImageResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def agent_manager_get_agent(self, agent_id_uuid, **kwargs):  # noqa: E501
-        """GetAgent  # noqa: E501
+    def image_registry_list_images(self, **kwargs):  # noqa: E501
+        """ListImages  # noqa: E501
 
-        Returns the agent that matches the specified ID.  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_get_agent(agent_id_uuid, async_req=True)
+        >>> thread = api.image_registry_list_images(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str agent_id_uuid: Unique object ID. (required)
-        :return: RimeGetAgentResponse
+        :param str page_token: Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.
+        :param str page_size: The maximum number of Image objects to return in a single page.
+        :return: RimeListImagesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.agent_manager_get_agent_with_http_info(agent_id_uuid, **kwargs)  # noqa: E501
+            return self.image_registry_list_images_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.agent_manager_get_agent_with_http_info(agent_id_uuid, **kwargs)  # noqa: E501
+            (data) = self.image_registry_list_images_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def agent_manager_get_agent_with_http_info(self, agent_id_uuid, **kwargs):  # noqa: E501
-        """GetAgent  # noqa: E501
+    def image_registry_list_images_with_http_info(self, **kwargs):  # noqa: E501
+        """ListImages  # noqa: E501
 
-        Returns the agent that matches the specified ID.  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_get_agent_with_http_info(agent_id_uuid, async_req=True)
+        >>> thread = api.image_registry_list_images_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str agent_id_uuid: Unique object ID. (required)
-        :return: RimeGetAgentResponse
+        :param str page_token: Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.
+        :param str page_size: The maximum number of Image objects to return in a single page.
+        :return: RimeListImagesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['agent_id_uuid']  # noqa: E501
+        all_params = ['page_token', 'page_size']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method agent_manager_get_agent" % key
+                    " to method image_registry_list_images" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'agent_id_uuid' is set
-        if ('agent_id_uuid' not in params or
-                params['agent_id_uuid'] is None):
-            raise ValueError("Missing the required parameter `agent_id_uuid` when calling `agent_manager_get_agent`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'agent_id_uuid' in params:
-            path_params['agentId.uuid'] = params['agent_id_uuid']  # noqa: E501
 
         query_params = []
+        if 'page_token' in params:
+            query_params.append(('pageToken', params['page_token']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('pageSize', params['page_size']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
@@ -397,126 +397,217 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/agents/{agentId.uuid}', 'GET',
+            '/v1/images', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeGetAgentResponse',  # noqa: E501
+            response_type='RimeListImagesResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def agent_manager_list_agents(self, **kwargs):  # noqa: E501
-        """ListAgents  # noqa: E501
+    def image_registry_list_images2(self, body, **kwargs):  # noqa: E501
+        """ListImages  # noqa: E501
 
-        Returns a paginated list of agents.  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_list_agents(async_req=True)
+        >>> thread = api.image_registry_list_images2(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str page_size: The maximum number of Agent objects to return in a single page.
-        :param str page_token: Specifies a page of the list returned by a ListAgents query. The ListAgents query returns a pageToken when there is more than one page of results. Specify either this field or the firstPageQuery field.
-        :param list[str] first_page_query_agent_status_types: Specifies a set of agent status types. The query filters for results that match the specified types.   - AGENT_STATUS_PENDING: Resources have been created for the agent but the agent has not started yet.  - AGENT_STATUS_ACTIVE: Agent can run jobs.  - AGENT_STATUS_UNRESPONSIVE: No agent heartbeat for three minutes.  - AGENT_STATUS_DEACTIVATED: Agent can no longer run jobs and can be deleted.
-        :param list[str] first_page_query_agent_ids: Specifies a set of agent IDs. The query filters for results that match the specified IDs.
-        :return: RimeListAgentsResponse
+        :param RimeListImagesRequest body: (required)
+        :return: RimeListImagesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.agent_manager_list_agents_with_http_info(**kwargs)  # noqa: E501
+            return self.image_registry_list_images2_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.agent_manager_list_agents_with_http_info(**kwargs)  # noqa: E501
+            (data) = self.image_registry_list_images2_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def agent_manager_list_agents_with_http_info(self, **kwargs):  # noqa: E501
-        """ListAgents  # noqa: E501
+    def image_registry_list_images2_with_http_info(self, body, **kwargs):  # noqa: E501
+        """ListImages  # noqa: E501
 
-        Returns a paginated list of agents.  # noqa: E501
+        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.agent_manager_list_agents_with_http_info(async_req=True)
+        >>> thread = api.image_registry_list_images2_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str page_size: The maximum number of Agent objects to return in a single page.
-        :param str page_token: Specifies a page of the list returned by a ListAgents query. The ListAgents query returns a pageToken when there is more than one page of results. Specify either this field or the firstPageQuery field.
-        :param list[str] first_page_query_agent_status_types: Specifies a set of agent status types. The query filters for results that match the specified types.   - AGENT_STATUS_PENDING: Resources have been created for the agent but the agent has not started yet.  - AGENT_STATUS_ACTIVE: Agent can run jobs.  - AGENT_STATUS_UNRESPONSIVE: No agent heartbeat for three minutes.  - AGENT_STATUS_DEACTIVATED: Agent can no longer run jobs and can be deleted.
-        :param list[str] first_page_query_agent_ids: Specifies a set of agent IDs. The query filters for results that match the specified IDs.
-        :return: RimeListAgentsResponse
+        :param RimeListImagesRequest body: (required)
+        :return: RimeListImagesResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['page_size', 'page_token', 'first_page_query_agent_status_types', 'first_page_query_agent_ids']  # noqa: E501
+        all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method agent_manager_list_agents" % key
+                    " to method image_registry_list_images2" % key
                 )
             params[key] = val
         del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `image_registry_list_images2`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'page_size' in params:
-            query_params.append(('pageSize', params['page_size']))  # noqa: E501
-        if 'page_token' in params:
-            query_params.append(('pageToken', params['page_token']))  # noqa: E501
-        if 'first_page_query_agent_status_types' in params:
-            query_params.append(('firstPageQuery.agentStatusTypes', params['first_page_query_agent_status_types']))  # noqa: E501
-            collection_formats['firstPageQuery.agentStatusTypes'] = 'multi'  # noqa: E501
-        if 'first_page_query_agent_ids' in params:
-            query_params.append(('firstPageQuery.agentIds', params['first_page_query_agent_ids']))  # noqa: E501
-            collection_formats['firstPageQuery.agentIds'] = 'multi'  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
+        if 'body' in params:
+            body_params = params['body']
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/images/list', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeListImagesResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def image_registry_update_build_info(self, body, **kwargs):  # noqa: E501
+        """UpdateBuildInfo updates the information about an image after an image build for it has completed.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.image_registry_update_build_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeUpdateBuildInfoRequest body: (required)
+        :return: RimeUpdateBuildInfoResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.image_registry_update_build_info_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.image_registry_update_build_info_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def image_registry_update_build_info_with_http_info(self, body, **kwargs):  # noqa: E501
+        """UpdateBuildInfo updates the information about an image after an image build for it has completed.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.image_registry_update_build_info_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeUpdateBuildInfoRequest body: (required)
+        :return: RimeUpdateBuildInfoResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method image_registry_update_build_info" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `image_registry_update_build_info`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/agents', 'GET',
+            '/internal/images/update-info', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeListAgentsResponse',  # noqa: E501
+            response_type='RimeUpdateBuildInfoResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,60 +16,60 @@
 
 # python 2 and python 3 compatibility library
 import six
 
 from rime_sdk.swagger.swagger_client.api_client import ApiClient
 
 
-class ImageRegistryApi(object):
+class NotificationSettingApi(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     Ref: https://github.com/swagger-api/swagger-codegen
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
-    def image_registry_create_image(self, body, **kwargs):  # noqa: E501
-        """CreateImage  # noqa: E501
+    def notification_setting_create_notification(self, body, **kwargs):  # noqa: E501
+        """CreateNotification  # noqa: E501
 
-        Creates a new Managed Image with a unique name.  # noqa: E501
+        Creates a new notification setting.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_create_image(body, async_req=True)
+        >>> thread = api.notification_setting_create_notification(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeCreateImageRequest body: (required)
-        :return: RimeCreateImageResponse
+        :param RimeCreateNotificationRequest body: (required)
+        :return: RimeCreateNotificationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.image_registry_create_image_with_http_info(body, **kwargs)  # noqa: E501
+            return self.notification_setting_create_notification_with_http_info(body, **kwargs)  # noqa: E501
         else:
-            (data) = self.image_registry_create_image_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.notification_setting_create_notification_with_http_info(body, **kwargs)  # noqa: E501
             return data
 
-    def image_registry_create_image_with_http_info(self, body, **kwargs):  # noqa: E501
-        """CreateImage  # noqa: E501
+    def notification_setting_create_notification_with_http_info(self, body, **kwargs):  # noqa: E501
+        """CreateNotification  # noqa: E501
 
-        Creates a new Managed Image with a unique name.  # noqa: E501
+        Creates a new notification setting.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_create_image_with_http_info(body, async_req=True)
+        >>> thread = api.notification_setting_create_notification_with_http_info(body, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeCreateImageRequest body: (required)
-        :return: RimeCreateImageResponse
+        :param RimeCreateNotificationRequest body: (required)
+        :return: RimeCreateNotificationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['body']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
@@ -77,22 +77,22 @@
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method image_registry_create_image" % key
+                    " to method notification_setting_create_notification" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `image_registry_create_image`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `notification_setting_create_notification`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
 
@@ -112,92 +112,92 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/images', 'POST',
+            '/v1/notif-settings', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeCreateImageResponse',  # noqa: E501
+            response_type='RimeCreateNotificationResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def image_registry_delete_image(self, name, **kwargs):  # noqa: E501
-        """DeleteImage  # noqa: E501
+    def notification_setting_delete_notification(self, id_uuid, **kwargs):  # noqa: E501
+        """DeleteNotification  # noqa: E501
 
-        Deletes a specified Managed Image.  # noqa: E501
+        Hard-delete a notification setting.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_delete_image(name, async_req=True)
+        >>> thread = api.notification_setting_delete_notification(id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: Name of existing Managed Image to delete. (required)
-        :return: RimeDeleteImageResponse
+        :param str id_uuid: Unique object ID. (required)
+        :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.image_registry_delete_image_with_http_info(name, **kwargs)  # noqa: E501
+            return self.notification_setting_delete_notification_with_http_info(id_uuid, **kwargs)  # noqa: E501
         else:
-            (data) = self.image_registry_delete_image_with_http_info(name, **kwargs)  # noqa: E501
+            (data) = self.notification_setting_delete_notification_with_http_info(id_uuid, **kwargs)  # noqa: E501
             return data
 
-    def image_registry_delete_image_with_http_info(self, name, **kwargs):  # noqa: E501
-        """DeleteImage  # noqa: E501
+    def notification_setting_delete_notification_with_http_info(self, id_uuid, **kwargs):  # noqa: E501
+        """DeleteNotification  # noqa: E501
 
-        Deletes a specified Managed Image.  # noqa: E501
+        Hard-delete a notification setting.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_delete_image_with_http_info(name, async_req=True)
+        >>> thread = api.notification_setting_delete_notification_with_http_info(id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: Name of existing Managed Image to delete. (required)
-        :return: RimeDeleteImageResponse
+        :param str id_uuid: Unique object ID. (required)
+        :return: object
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name']  # noqa: E501
+        all_params = ['id_uuid']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method image_registry_delete_image" % key
+                    " to method notification_setting_delete_notification" % key
                 )
             params[key] = val
         del params['kwargs']
-        # verify the required parameter 'name' is set
-        if ('name' not in params or
-                params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `image_registry_delete_image`")  # noqa: E501
+        # verify the required parameter 'id_uuid' is set
+        if ('id_uuid' not in params or
+                params['id_uuid'] is None):
+            raise ValueError("Missing the required parameter `id_uuid` when calling `notification_setting_delete_notification`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
-        if 'name' in params:
-            path_params['name'] = params['name']  # noqa: E501
+        if 'id_uuid' in params:
+            path_params['id.uuid'] = params['id_uuid']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -207,185 +207,100 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/images/{name}', 'DELETE',
+            '/v1/notif-settings/{id.uuid}', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeDeleteImageResponse',  # noqa: E501
+            response_type='object',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def image_registry_get_image(self, name, **kwargs):  # noqa: E501
-        """GetImage  # noqa: E501
+    def notification_setting_list_notifications(self, **kwargs):  # noqa: E501
+        """ListNotifications  # noqa: E501
 
-        Returns the definition of a specified Managed Image.  # noqa: E501
+        Lists notification settings with options to filter by project or the type of notification.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_get_image(name, async_req=True)
+        >>> thread = api.notification_setting_list_notifications(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: Name of the existing Managed Image. (required)
-        :return: RimeGetImageResponse
+        :param list[str] list_notifications_query_object_types: Specifies a set of object types. Filters results by the specified set of object types.   - OBJECT_TYPE_UNSPECIFIED: Unspecified is an invalid object type - do not use.  - OBJECT_TYPE_PROJECT: Used for notifications associated with an project. The Notification object ID is the Project ID.
+        :param list[str] list_notifications_query_object_ids: Specifies a set of object IDs. Filters results by the specified set of object IDs.
+        :param str page_token: Specifies a page of the list returned by a ListNotifications query. The ListNotifications query returns a pageToken when there is more than one page of results. Specify either this field or the listNotificationsQuery field.
+        :param str page_size: The maximum number of Notification objects to return in a single page.
+        :return: RimeListNotificationsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.image_registry_get_image_with_http_info(name, **kwargs)  # noqa: E501
+            return self.notification_setting_list_notifications_with_http_info(**kwargs)  # noqa: E501
         else:
-            (data) = self.image_registry_get_image_with_http_info(name, **kwargs)  # noqa: E501
+            (data) = self.notification_setting_list_notifications_with_http_info(**kwargs)  # noqa: E501
             return data
 
-    def image_registry_get_image_with_http_info(self, name, **kwargs):  # noqa: E501
-        """GetImage  # noqa: E501
+    def notification_setting_list_notifications_with_http_info(self, **kwargs):  # noqa: E501
+        """ListNotifications  # noqa: E501
 
-        Returns the definition of a specified Managed Image.  # noqa: E501
+        Lists notification settings with options to filter by project or the type of notification.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_get_image_with_http_info(name, async_req=True)
+        >>> thread = api.notification_setting_list_notifications_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str name: Name of the existing Managed Image. (required)
-        :return: RimeGetImageResponse
+        :param list[str] list_notifications_query_object_types: Specifies a set of object types. Filters results by the specified set of object types.   - OBJECT_TYPE_UNSPECIFIED: Unspecified is an invalid object type - do not use.  - OBJECT_TYPE_PROJECT: Used for notifications associated with an project. The Notification object ID is the Project ID.
+        :param list[str] list_notifications_query_object_ids: Specifies a set of object IDs. Filters results by the specified set of object IDs.
+        :param str page_token: Specifies a page of the list returned by a ListNotifications query. The ListNotifications query returns a pageToken when there is more than one page of results. Specify either this field or the listNotificationsQuery field.
+        :param str page_size: The maximum number of Notification objects to return in a single page.
+        :return: RimeListNotificationsResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['name']  # noqa: E501
+        all_params = ['list_notifications_query_object_types', 'list_notifications_query_object_ids', 'page_token', 'page_size']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method image_registry_get_image" % key
-                )
-            params[key] = val
-        del params['kwargs']
-        # verify the required parameter 'name' is set
-        if ('name' not in params or
-                params['name'] is None):
-            raise ValueError("Missing the required parameter `name` when calling `image_registry_get_image`")  # noqa: E501
-
-        collection_formats = {}
-
-        path_params = {}
-        if 'name' in params:
-            path_params['name'] = params['name']  # noqa: E501
-
-        query_params = []
-
-        header_params = {}
-
-        form_params = []
-        local_var_files = {}
-
-        body_params = None
-        # HTTP header `Accept`
-        header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # Authentication setting
-        auth_settings = ['rime-api-key']  # noqa: E501
-
-        return self.api_client.call_api(
-            '/v1/images/{name}', 'GET',
-            path_params,
-            query_params,
-            header_params,
-            body=body_params,
-            post_params=form_params,
-            files=local_var_files,
-            response_type='RimeGetImageResponse',  # noqa: E501
-            auth_settings=auth_settings,
-            async_req=params.get('async_req'),
-            _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
-            _request_timeout=params.get('_request_timeout'),
-            collection_formats=collection_formats)
-
-    def image_registry_list_images(self, **kwargs):  # noqa: E501
-        """ListImages  # noqa: E501
-
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_list_images(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str page_token: Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.
-        :param str page_size: The maximum number of Image objects to return in a single page.
-        :return: RimeListImagesResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-        kwargs['_return_http_data_only'] = True
-        if kwargs.get('async_req'):
-            return self.image_registry_list_images_with_http_info(**kwargs)  # noqa: E501
-        else:
-            (data) = self.image_registry_list_images_with_http_info(**kwargs)  # noqa: E501
-            return data
-
-    def image_registry_list_images_with_http_info(self, **kwargs):  # noqa: E501
-        """ListImages  # noqa: E501
-
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_list_images_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req bool
-        :param str page_token: Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.
-        :param str page_size: The maximum number of Image objects to return in a single page.
-        :return: RimeListImagesResponse
-                 If the method is called asynchronously,
-                 returns the request thread.
-        """
-
-        all_params = ['page_token', 'page_size']  # noqa: E501
-        all_params.append('async_req')
-        all_params.append('_return_http_data_only')
-        all_params.append('_preload_content')
-        all_params.append('_request_timeout')
-
-        params = locals()
-        for key, val in six.iteritems(params['kwargs']):
-            if key not in all_params:
-                raise TypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method image_registry_list_images" % key
+                    " to method notification_setting_list_notifications" % key
                 )
             params[key] = val
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
+        if 'list_notifications_query_object_types' in params:
+            query_params.append(('listNotificationsQuery.objectTypes', params['list_notifications_query_object_types']))  # noqa: E501
+            collection_formats['listNotificationsQuery.objectTypes'] = 'multi'  # noqa: E501
+        if 'list_notifications_query_object_ids' in params:
+            query_params.append(('listNotificationsQuery.objectIds', params['list_notifications_query_object_ids']))  # noqa: E501
+            collection_formats['listNotificationsQuery.objectIds'] = 'multi'  # noqa: E501
         if 'page_token' in params:
             query_params.append(('pageToken', params['page_token']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('pageSize', params['page_size']))  # noqa: E501
 
         header_params = {}
 
@@ -397,90 +312,98 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/images', 'GET',
+            '/v1/notif-settings', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeListImagesResponse',  # noqa: E501
+            response_type='RimeListNotificationsResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def image_registry_list_images2(self, body, **kwargs):  # noqa: E501
-        """ListImages  # noqa: E501
+    def notification_setting_update_notification(self, body, notification_id_uuid, **kwargs):  # noqa: E501
+        """UpdateNotification  # noqa: E501
 
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Updates an existing notification setting. The ID in the provided notification is used to identify it.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_list_images2(body, async_req=True)
+        >>> thread = api.notification_setting_update_notification(body, notification_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeListImagesRequest body: (required)
-        :return: RimeListImagesResponse
+        :param NotifsettingsNotificationIdUuidBody body: (required)
+        :param str notification_id_uuid: Unique object ID. (required)
+        :return: RimeUpdateNotificationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
-            return self.image_registry_list_images2_with_http_info(body, **kwargs)  # noqa: E501
+            return self.notification_setting_update_notification_with_http_info(body, notification_id_uuid, **kwargs)  # noqa: E501
         else:
-            (data) = self.image_registry_list_images2_with_http_info(body, **kwargs)  # noqa: E501
+            (data) = self.notification_setting_update_notification_with_http_info(body, notification_id_uuid, **kwargs)  # noqa: E501
             return data
 
-    def image_registry_list_images2_with_http_info(self, body, **kwargs):  # noqa: E501
-        """ListImages  # noqa: E501
+    def notification_setting_update_notification_with_http_info(self, body, notification_id_uuid, **kwargs):  # noqa: E501
+        """UpdateNotification  # noqa: E501
 
-        List all Managed Images that match a specified set of constraints.  [Python pagination example](#tag/JobReader/operation/JobReader_ListJobs)  # noqa: E501
+        Updates an existing notification setting. The ID in the provided notification is used to identify it.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.image_registry_list_images2_with_http_info(body, async_req=True)
+        >>> thread = api.notification_setting_update_notification_with_http_info(body, notification_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param RimeListImagesRequest body: (required)
-        :return: RimeListImagesResponse
+        :param NotifsettingsNotificationIdUuidBody body: (required)
+        :param str notification_id_uuid: Unique object ID. (required)
+        :return: RimeUpdateNotificationResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['body']  # noqa: E501
+        all_params = ['body', 'notification_id_uuid']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
             if key not in all_params:
                 raise TypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method image_registry_list_images2" % key
+                    " to method notification_setting_update_notification" % key
                 )
             params[key] = val
         del params['kwargs']
         # verify the required parameter 'body' is set
         if ('body' not in params or
                 params['body'] is None):
-            raise ValueError("Missing the required parameter `body` when calling `image_registry_list_images2`")  # noqa: E501
+            raise ValueError("Missing the required parameter `body` when calling `notification_setting_update_notification`")  # noqa: E501
+        # verify the required parameter 'notification_id_uuid' is set
+        if ('notification_id_uuid' not in params or
+                params['notification_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `notification_id_uuid` when calling `notification_setting_update_notification`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
+        if 'notification_id_uuid' in params:
+            path_params['notification.id.uuid'] = params['notification_id_uuid']  # noqa: E501
 
         query_params = []
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
@@ -496,21 +419,21 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1/images/list', 'POST',
+            '/v1/notif-settings/{notification.id.uuid}', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
-            response_type='RimeListImagesResponse',  # noqa: E501
+            response_type='RimeUpdateNotificationResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,113 @@
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
+    def model_card_service_create_model_card(self, body, **kwargs):  # noqa: E501
+        """CreateModelCard  # noqa: E501
+
+        Create a new Model Card.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.model_card_service_create_model_card(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeCreateModelCardRequest body: (required)
+        :return: RimeCreateModelCardResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.model_card_service_create_model_card_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.model_card_service_create_model_card_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def model_card_service_create_model_card_with_http_info(self, body, **kwargs):  # noqa: E501
+        """CreateModelCard  # noqa: E501
+
+        Create a new Model Card.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.model_card_service_create_model_card_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeCreateModelCardRequest body: (required)
+        :return: RimeCreateModelCardResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method model_card_service_create_model_card" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `model_card_service_create_model_card`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1-beta/modelcards', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeCreateModelCardResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def model_card_service_delete_model_card(self, model_card_id_uuid, **kwargs):  # noqa: E501
         """DeleteModelCard  # noqa: E501
 
         Delete Model Card.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.model_card_service_delete_model_card(model_card_id_uuid, async_req=True)
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -337,14 +337,117 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def results_reader_get_test_config(self, test_run_id, config_name, **kwargs):  # noqa: E501
+        """GetTestConfig  # noqa: E501
+
+        Returns the test configuration of the specified test run as bytes.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.results_reader_get_test_config(test_run_id, config_name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str test_run_id: Uniquely specifies a Test Run. (required)
+        :param str config_name: The name of the test config requested. (required)
+        :return: TestrunresultGetTestConfigResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.results_reader_get_test_config_with_http_info(test_run_id, config_name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.results_reader_get_test_config_with_http_info(test_run_id, config_name, **kwargs)  # noqa: E501
+            return data
+
+    def results_reader_get_test_config_with_http_info(self, test_run_id, config_name, **kwargs):  # noqa: E501
+        """GetTestConfig  # noqa: E501
+
+        Returns the test configuration of the specified test run as bytes.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.results_reader_get_test_config_with_http_info(test_run_id, config_name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str test_run_id: Uniquely specifies a Test Run. (required)
+        :param str config_name: The name of the test config requested. (required)
+        :return: TestrunresultGetTestConfigResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['test_run_id', 'config_name']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method results_reader_get_test_config" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'test_run_id' is set
+        if ('test_run_id' not in params or
+                params['test_run_id'] is None):
+            raise ValueError("Missing the required parameter `test_run_id` when calling `results_reader_get_test_config`")  # noqa: E501
+        # verify the required parameter 'config_name' is set
+        if ('config_name' not in params or
+                params['config_name'] is None):
+            raise ValueError("Missing the required parameter `config_name` when calling `results_reader_get_test_config`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'test_run_id' in params:
+            path_params['testRunId'] = params['test_run_id']  # noqa: E501
+        if 'config_name' in params:
+            path_params['configName'] = params['config_name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/test-runs/{testRunId}/test-config/{configName}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='TestrunresultGetTestConfigResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def results_reader_get_test_run(self, test_run_id, **kwargs):  # noqa: E501
         """GetTestRun  # noqa: E501
 
         Returns the test run result detail for a given Test Run ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.results_reader_get_test_run(test_run_id, async_req=True)
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -234,14 +234,121 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def workspace_service_create_workspace_tag(self, body, workspace_id_uuid, **kwargs):  # noqa: E501
+        """CreateWorkspaceTag  # noqa: E501
+
+        Creates a new tag within a Workspace.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_create_workspace_tag(body, workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param WorkspaceIdUuidTagsBody body: (required)
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :return: RimeCreateWorkspaceTagResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.workspace_service_create_workspace_tag_with_http_info(body, workspace_id_uuid, **kwargs)  # noqa: E501
+        else:
+            (data) = self.workspace_service_create_workspace_tag_with_http_info(body, workspace_id_uuid, **kwargs)  # noqa: E501
+            return data
+
+    def workspace_service_create_workspace_tag_with_http_info(self, body, workspace_id_uuid, **kwargs):  # noqa: E501
+        """CreateWorkspaceTag  # noqa: E501
+
+        Creates a new tag within a Workspace.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_create_workspace_tag_with_http_info(body, workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param WorkspaceIdUuidTagsBody body: (required)
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :return: RimeCreateWorkspaceTagResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body', 'workspace_id_uuid']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method workspace_service_create_workspace_tag" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `workspace_service_create_workspace_tag`")  # noqa: E501
+        # verify the required parameter 'workspace_id_uuid' is set
+        if ('workspace_id_uuid' not in params or
+                params['workspace_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_create_workspace_tag`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'workspace_id_uuid' in params:
+            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/workspace/{workspaceId.uuid}/tags', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeCreateWorkspaceTagResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def workspace_service_delete_workspace(self, workspace_id_uuid, **kwargs):  # noqa: E501
         """DeleteWorkspace  # noqa: E501
 
         Deletes an existing Workspace by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_delete_workspace(workspace_id_uuid, async_req=True)
@@ -329,14 +436,117 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def workspace_service_delete_workspace_tag(self, workspace_id_uuid, name, **kwargs):  # noqa: E501
+        """DeleteWorkspaceTag  # noqa: E501
+
+        Deletes an existing tag within a Workspace by tag name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_delete_workspace_tag(workspace_id_uuid, name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :param str name: Name of the tag. (required)
+        :return: RimeDeleteWorkspaceTagResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.workspace_service_delete_workspace_tag_with_http_info(workspace_id_uuid, name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.workspace_service_delete_workspace_tag_with_http_info(workspace_id_uuid, name, **kwargs)  # noqa: E501
+            return data
+
+    def workspace_service_delete_workspace_tag_with_http_info(self, workspace_id_uuid, name, **kwargs):  # noqa: E501
+        """DeleteWorkspaceTag  # noqa: E501
+
+        Deletes an existing tag within a Workspace by tag name.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_delete_workspace_tag_with_http_info(workspace_id_uuid, name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :param str name: Name of the tag. (required)
+        :return: RimeDeleteWorkspaceTagResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['workspace_id_uuid', 'name']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method workspace_service_delete_workspace_tag" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'workspace_id_uuid' is set
+        if ('workspace_id_uuid' not in params or
+                params['workspace_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_delete_workspace_tag`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `workspace_service_delete_workspace_tag`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'workspace_id_uuid' in params:
+            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/workspace/{workspaceId.uuid}/tags/{name}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeDeleteWorkspaceTagResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def workspace_service_get_workspace(self, workspace_id_uuid, **kwargs):  # noqa: E501
         """GetWorkspace  # noqa: E501
 
         Return a Workspace by ID.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_get_workspace(workspace_id_uuid, async_req=True)
@@ -527,14 +737,109 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def workspace_service_list_workspace_tags(self, workspace_id_uuid, **kwargs):  # noqa: E501
+        """ListWorkspaceTags  # noqa: E501
+
+        Lists all tags created within a Workspace.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_list_workspace_tags(workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :return: RimeListWorkspaceTagsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.workspace_service_list_workspace_tags_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
+        else:
+            (data) = self.workspace_service_list_workspace_tags_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
+            return data
+
+    def workspace_service_list_workspace_tags_with_http_info(self, workspace_id_uuid, **kwargs):  # noqa: E501
+        """ListWorkspaceTags  # noqa: E501
+
+        Lists all tags created within a Workspace.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_list_workspace_tags_with_http_info(workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :return: RimeListWorkspaceTagsResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['workspace_id_uuid']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method workspace_service_list_workspace_tags" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'workspace_id_uuid' is set
+        if ('workspace_id_uuid' not in params or
+                params['workspace_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_list_workspace_tags`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'workspace_id_uuid' in params:
+            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/workspace/{workspaceId.uuid}/tags', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeListWorkspaceTagsResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def workspace_service_list_workspaces(self, **kwargs):  # noqa: E501
         """ListWorkspaces  # noqa: E501
 
         List Workspaces with optional filter.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_list_workspaces(async_req=True)
@@ -946,7 +1251,122 @@
             response_type='RimeUpdateWorkspaceResponse',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def workspace_service_update_workspace_tag(self, body, workspace_id_uuid, name, **kwargs):  # noqa: E501
+        """UpdateWorkspaceTag  # noqa: E501
+
+        Updates an existing tag within a Workspace.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_update_workspace_tag(body, workspace_id_uuid, name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param TagsNameBody body: (required)
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :param str name: Name of the tag. (required)
+        :return: RimeUpdateWorkspaceTagResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.workspace_service_update_workspace_tag_with_http_info(body, workspace_id_uuid, name, **kwargs)  # noqa: E501
+        else:
+            (data) = self.workspace_service_update_workspace_tag_with_http_info(body, workspace_id_uuid, name, **kwargs)  # noqa: E501
+            return data
+
+    def workspace_service_update_workspace_tag_with_http_info(self, body, workspace_id_uuid, name, **kwargs):  # noqa: E501
+        """UpdateWorkspaceTag  # noqa: E501
+
+        Updates an existing tag within a Workspace.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_update_workspace_tag_with_http_info(body, workspace_id_uuid, name, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param TagsNameBody body: (required)
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :param str name: Name of the tag. (required)
+        :return: RimeUpdateWorkspaceTagResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body', 'workspace_id_uuid', 'name']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method workspace_service_update_workspace_tag" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `workspace_service_update_workspace_tag`")  # noqa: E501
+        # verify the required parameter 'workspace_id_uuid' is set
+        if ('workspace_id_uuid' not in params or
+                params['workspace_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_update_workspace_tag`")  # noqa: E501
+        # verify the required parameter 'name' is set
+        if ('name' not in params or
+                params['name'] is None):
+            raise ValueError("Missing the required parameter `name` when calling `workspace_service_update_workspace_tag`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'workspace_id_uuid' in params:
+            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
+        if 'name' in params:
+            path_params['name'] = params['name']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/workspace/{workspaceId.uuid}/tags/{name}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeUpdateWorkspaceTagResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from __future__ import absolute_import
 
 # import models into model package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
+from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
@@ -42,14 +43,15 @@
 from rime_sdk.swagger.swagger_client.models.detection_event_type import DetectionEventType
 from rime_sdk.swagger.swagger_client.models.detection_metric_degradation_event_details import DetectionMetricDegradationEventDetails
 from rime_sdk.swagger.swagger_client.models.detection_resolution import DetectionResolution
 from rime_sdk.swagger.swagger_client.models.detection_security_event_details import DetectionSecurityEventDetails
 from rime_sdk.swagger.swagger_client.models.difference_from_target_difference import DifferenceFromTargetDifference
 from rime_sdk.swagger.swagger_client.models.difference_from_target_target import DifferenceFromTargetTarget
 from rime_sdk.swagger.swagger_client.models.digest_config_digest_frequency import DigestConfigDigestFrequency
+from rime_sdk.swagger.swagger_client.models.featureflags_customer_name_body import FeatureflagsCustomerNameBody
 from rime_sdk.swagger.swagger_client.models.filescanning_file_scan_result import FilescanningFileScanResult
 from rime_sdk.swagger.swagger_client.models.filescanning_huggingface_model_info import FilescanningHuggingfaceModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_model_file_info import FilescanningModelFileInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_pytorch_model_info import FilescanningPytorchModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_custom_loader_location import FirewallCustomLoaderLocation
@@ -154,15 +156,14 @@
 from rime_sdk.swagger.swagger_client.models.rename_test_run_id_body import RenameTestRunIdBody
 from rime_sdk.swagger.swagger_client.models.resetpassword_user_id_uuid_body import ResetpasswordUserIdUuidBody
 from rime_sdk.swagger.swagger_client.models.rime_api_token_info import RimeAPITokenInfo
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_agent import RimeAgent
 from rime_sdk.swagger.swagger_client.models.rime_agent_status import RimeAgentStatus
-from rime_sdk.swagger.swagger_client.models.rime_archived_job_logs import RimeArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.rime_cancel_job_response import RimeCancelJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_category_metric import RimeCategoryMetric
 from rime_sdk.swagger.swagger_client.models.rime_category_test_result import RimeCategoryTestResult
 from rime_sdk.swagger.swagger_client.models.rime_config_type import RimeConfigType
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_request_integration_variable import RimeConfigureIntegrationRequestIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_response import RimeConfigureIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_job_progress import RimeContinuousTestJobProgress
@@ -174,14 +175,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_create_custom_monitor_response import RimeCreateCustomMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_request import RimeCreateFirewallRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_response import RimeCreateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_image_request import RimeCreateImageRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_image_response import RimeCreateImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_request import RimeCreateIntegrationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_response import RimeCreateIntegrationResponse
+from rime_sdk.swagger.swagger_client.models.rime_create_model_card_request import RimeCreateModelCardRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_response import RimeCreateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_request import RimeCreateNotificationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_notification_response import RimeCreateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_user_request import RimeCreateUserRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_user_response import RimeCreateUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_request import RimeCreateWorkspaceRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_workspace_response import RimeCreateWorkspaceResponse
@@ -314,14 +316,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_test_metric_category import RimeTestMetricCategory
 from rime_sdk.swagger.swagger_client.models.rime_test_run_progress import RimeTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_test_task_status import RimeTestTaskStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_type import RimeTestType
 from rime_sdk.swagger.swagger_client.models.rime_time_interval import RimeTimeInterval
 from rime_sdk.swagger.swagger_client.models.rime_token_type import RimeTokenType
 from rime_sdk.swagger.swagger_client.models.rime_uuid import RimeUUID
+from rime_sdk.swagger.swagger_client.models.rime_update_build_info_request import RimeUpdateBuildInfoRequest
 from rime_sdk.swagger.swagger_client.models.rime_update_build_info_response import RimeUpdateBuildInfoResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_firewall_response import RimeUpdateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_integration_response import RimeUpdateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_model_card_response import RimeUpdateModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_monitor_response import RimeUpdateMonitorResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_notification_response import RimeUpdateNotificationResponse
 from rime_sdk.swagger.swagger_client.models.rime_update_user_of_workspace_response import RimeUpdateUserOfWorkspaceResponse
@@ -346,19 +349,21 @@
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_run_time_info import RuntimeinfoRunTimeInfo
 from rime_sdk.swagger.swagger_client.models.schemadatacollector_prediction import SchemadatacollectorPrediction
 from rime_sdk.swagger.swagger_client.models.schemaintegration_integration_variable import SchemaintegrationIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.schemamonitor_config import SchemamonitorConfig
 from rime_sdk.swagger.swagger_client.models.schemanotification_config import SchemanotificationConfig
 from rime_sdk.swagger.swagger_client.models.security_event_details_flagged_datapoint import SecurityEventDetailsFlaggedDatapoint
 from rime_sdk.swagger.swagger_client.models.security_event_details_security_event_type import SecurityEventDetailsSecurityEventType
+from rime_sdk.swagger.swagger_client.models.statedb_archived_job_logs import StatedbArchivedJobLogs
 from rime_sdk.swagger.swagger_client.models.statedb_job_status import StatedbJobStatus
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_datapoints_response import StreamResultOfRimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_latest_logs_response import StreamResultOfRimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.stream_result_of_rime_get_predictions_response import StreamResultOfRimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.stresstests_project_id_uuid_body import StresstestsProjectIdUuidBody
+from rime_sdk.swagger.swagger_client.models.tags_name_body import TagsNameBody
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_category_summary_metric import TestRunMetricsCategorySummaryMetric
 from rime_sdk.swagger.swagger_client.models.test_run_metrics_model_perf_metric import TestRunMetricsModelPerfMetric
 from rime_sdk.swagger.swagger_client.models.test_run_progress_test_batch_progress import TestRunProgressTestBatchProgress
 from rime_sdk.swagger.swagger_client.models.testrun_annotated_test_config import TestrunAnnotatedTestConfig
 from rime_sdk.swagger.swagger_client.models.testrun_connection_info import TestrunConnectionInfo
 from rime_sdk.swagger.swagger_client.models.testrun_custom_metric import TestrunCustomMetric
 from rime_sdk.swagger.swagger_client.models.testrun_data_collector_info import TestrunDataCollectorInfo
@@ -370,15 +375,14 @@
 from rime_sdk.swagger.swagger_client.models.testrun_delta_lake_info import TestrunDeltaLakeInfo
 from rime_sdk.swagger.swagger_client.models.testrun_hugging_face_data_info import TestrunHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.testrun_model_profiling import TestrunModelProfiling
 from rime_sdk.swagger.swagger_client.models.testrun_pred_info import TestrunPredInfo
 from rime_sdk.swagger.swagger_client.models.testrun_prediction_params import TestrunPredictionParams
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import TestrunProfilingConfig
 from rime_sdk.swagger.swagger_client.models.testrun_single_data_info import TestrunSingleDataInfo
-from rime_sdk.swagger.swagger_client.models.testrun_test_category import TestrunTestCategory
 from rime_sdk.swagger.swagger_client.models.testrun_test_category_type import TestrunTestCategoryType
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_config import TestrunTestRunConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_run_incremental_config import TestrunTestRunIncrementalConfig
 from rime_sdk.swagger.swagger_client.models.testrun_test_sensitivity import TestrunTestSensitivity
 from rime_sdk.swagger.swagger_client.models.testrun_test_suite_config import TestrunTestSuiteConfig
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_batch_result_response import TestrunresultGetBatchResultResponse
 from rime_sdk.swagger.swagger_client.models.testrunresult_get_feature_result_response import TestrunresultGetFeatureResultResponse
@@ -409,9 +413,10 @@
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body1 import UsersUserUserIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.v1betaintegrationsintegration_id_uuid_integration import V1betaintegrationsintegrationIdUuidIntegration
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
+from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_tags_body import WorkspaceIdUuidTagsBody
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,26 +78,26 @@
 
         self._firewall_id = firewall_id
 
     @property
     def start_time(self):
         """Gets the start_time of this DatasetCTInfo.  # noqa: E501
 
-        start and end time are the start and end time of this dataset. this should is used by scheduled ct when registering new datasets.  # noqa: E501
+        Start and end time are the start and end time of this dataset.  # noqa: E501
 
         :return: The start_time of this DatasetCTInfo.  # noqa: E501
         :rtype: datetime
         """
         return self._start_time
 
     @start_time.setter
     def start_time(self, start_time):
         """Sets the start_time of this DatasetCTInfo.
 
-        start and end time are the start and end time of this dataset. this should is used by scheduled ct when registering new datasets.  # noqa: E501
+        Start and end time are the start and end time of this dataset.  # noqa: E501
 
         :param start_time: The start_time of this DatasetCTInfo.  # noqa: E501
         :type: datetime
         """
 
         self._start_time = start_time
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_data_location.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_location.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,87 +11,63 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FirewallDeltaLakeLocation(object):
+class NotificationWebhookConfig(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'table_name': 'str',
-        'time_col': 'str'
+        'webhook': 'str'
     }
 
     attribute_map = {
-        'table_name': 'tableName',
-        'time_col': 'timeCol'
+        'webhook': 'webhook'
     }
 
-    def __init__(self, table_name=None, time_col=None):  # noqa: E501
-        """FirewallDeltaLakeLocation - a model defined in Swagger"""  # noqa: E501
-        self._table_name = None
-        self._time_col = None
+    def __init__(self, webhook=None):  # noqa: E501
+        """NotificationWebhookConfig - a model defined in Swagger"""  # noqa: E501
+        self._webhook = None
         self.discriminator = None
-        if table_name is not None:
-            self.table_name = table_name
-        if time_col is not None:
-            self.time_col = time_col
+        if webhook is not None:
+            self.webhook = webhook
 
     @property
-    def table_name(self):
-        """Gets the table_name of this FirewallDeltaLakeLocation.  # noqa: E501
+    def webhook(self):
+        """Gets the webhook of this NotificationWebhookConfig.  # noqa: E501
 
+        The URL of the destination webhook. It is not a strict requirement, but it is recommended that webhooks be preauthenticated by including a secure token in the URL.  # noqa: E501
 
-        :return: The table_name of this FirewallDeltaLakeLocation.  # noqa: E501
+        :return: The webhook of this NotificationWebhookConfig.  # noqa: E501
         :rtype: str
         """
-        return self._table_name
+        return self._webhook
 
-    @table_name.setter
-    def table_name(self, table_name):
-        """Sets the table_name of this FirewallDeltaLakeLocation.
+    @webhook.setter
+    def webhook(self, webhook):
+        """Sets the webhook of this NotificationWebhookConfig.
 
+        The URL of the destination webhook. It is not a strict requirement, but it is recommended that webhooks be preauthenticated by including a secure token in the URL.  # noqa: E501
 
-        :param table_name: The table_name of this FirewallDeltaLakeLocation.  # noqa: E501
+        :param webhook: The webhook of this NotificationWebhookConfig.  # noqa: E501
         :type: str
         """
 
-        self._table_name = table_name
-
-    @property
-    def time_col(self):
-        """Gets the time_col of this FirewallDeltaLakeLocation.  # noqa: E501
-
-
-        :return: The time_col of this FirewallDeltaLakeLocation.  # noqa: E501
-        :rtype: str
-        """
-        return self._time_col
-
-    @time_col.setter
-    def time_col(self, time_col):
-        """Sets the time_col of this FirewallDeltaLakeLocation.
-
-
-        :param time_col: The time_col of this FirewallDeltaLakeLocation.  # noqa: E501
-        :type: str
-        """
-
-        self._time_col = time_col
+        self._webhook = webhook
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +82,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FirewallDeltaLakeLocation, dict):
+        if issubclass(NotificationWebhookConfig, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +98,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FirewallDeltaLakeLocation):
+        if not isinstance(other, NotificationWebhookConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_args.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_args.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_location_params.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 
     """
     allowed enum values
     """
     UNSPECIFIED = "INTEGRATION_TYPE_UNSPECIFIED"
     CUSTOM = "INTEGRATION_TYPE_CUSTOM"
     DATABRICKS = "INTEGRATION_TYPE_DATABRICKS"
-    AWS_S3_ACCESS_KEY = "INTEGRATION_TYPE_AWS_S3_ACCESS_KEY"
-    AWS_S3_ROLE_ARN = "INTEGRATION_TYPE_AWS_S3_ROLE_ARN"
+    AWS_ACCESS_KEY = "INTEGRATION_TYPE_AWS_ACCESS_KEY"
+    AWS_ROLE_ARN = "INTEGRATION_TYPE_AWS_ROLE_ARN"
     HUGGINGFACE = "INTEGRATION_TYPE_HUGGINGFACE"
     GCS = "INTEGRATION_TYPE_GCS"
+    AZURE_CLIENT_SECRET = "INTEGRATION_TYPE_AZURE_CLIENT_SECRET"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,40 +32,43 @@
         'model_id': 'RimeUUID',
         'project_ids': 'list[RimeUUID]',
         'creator_id': 'RimeUUID',
         'creation_time': 'datetime',
         'external_id': 'str',
         'user_metadata': 'RegistryMetadata',
         'model_info': 'ModelModelInfo',
-        'validity_status': 'RegistryValidityStatus'
+        'validity_status': 'RegistryValidityStatus',
+        'integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'name': 'name',
         'model_id': 'modelId',
         'project_ids': 'projectIds',
         'creator_id': 'creatorId',
         'creation_time': 'creationTime',
         'external_id': 'externalId',
         'user_metadata': 'userMetadata',
         'model_info': 'modelInfo',
-        'validity_status': 'validityStatus'
+        'validity_status': 'validityStatus',
+        'integration_id': 'integrationId'
     }
 
-    def __init__(self, name=None, model_id=None, project_ids=None, creator_id=None, creation_time=None, external_id=None, user_metadata=None, model_info=None, validity_status=None):  # noqa: E501
+    def __init__(self, name=None, model_id=None, project_ids=None, creator_id=None, creation_time=None, external_id=None, user_metadata=None, model_info=None, validity_status=None, integration_id=None):  # noqa: E501
         """ModelModel - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._model_id = None
         self._project_ids = None
         self._creator_id = None
         self._creation_time = None
         self._external_id = None
         self._user_metadata = None
         self._model_info = None
         self._validity_status = None
+        self._integration_id = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if model_id is not None:
             self.model_id = model_id
         if project_ids is not None:
             self.project_ids = project_ids
@@ -77,14 +80,16 @@
             self.external_id = external_id
         if user_metadata is not None:
             self.user_metadata = user_metadata
         if model_info is not None:
             self.model_info = model_info
         if validity_status is not None:
             self.validity_status = validity_status
+        if integration_id is not None:
+            self.integration_id = integration_id
 
     @property
     def name(self):
         """Gets the name of this ModelModel.  # noqa: E501
 
         Name and model_id are both enforced to be unique. Name is user specified. Model_id is internally generated.  # noqa: E501
 
@@ -273,14 +278,35 @@
 
         :param validity_status: The validity_status of this ModelModel.  # noqa: E501
         :type: RegistryValidityStatus
         """
 
         self._validity_status = validity_status
 
+    @property
+    def integration_id(self):
+        """Gets the integration_id of this ModelModel.  # noqa: E501
+
+
+        :return: The integration_id of this ModelModel.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._integration_id
+
+    @integration_id.setter
+    def integration_id(self, integration_id):
+        """Sets the integration_id of this ModelModel.
+
+
+        :param integration_id: The integration_id of this ModelModel.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._integration_id = integration_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/model_model_path_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,63 +11,64 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NotificationWebhookConfig(object):
+class TestrunDeltaLakeInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'webhook': 'str'
+        'table_name': 'str'
     }
 
     attribute_map = {
-        'webhook': 'webhook'
+        'table_name': 'tableName'
     }
 
-    def __init__(self, webhook=None):  # noqa: E501
-        """NotificationWebhookConfig - a model defined in Swagger"""  # noqa: E501
-        self._webhook = None
+    def __init__(self, table_name=None):  # noqa: E501
+        """TestrunDeltaLakeInfo - a model defined in Swagger"""  # noqa: E501
+        self._table_name = None
         self.discriminator = None
-        if webhook is not None:
-            self.webhook = webhook
+        self.table_name = table_name
 
     @property
-    def webhook(self):
-        """Gets the webhook of this NotificationWebhookConfig.  # noqa: E501
+    def table_name(self):
+        """Gets the table_name of this TestrunDeltaLakeInfo.  # noqa: E501
 
-        The URL of the destination webhook. It is not a strict requirement, but it is recommended that webhooks be preauthenticated by including a secure token in the URL.  # noqa: E501
+        The database table name to use.  # noqa: E501
 
-        :return: The webhook of this NotificationWebhookConfig.  # noqa: E501
+        :return: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
         :rtype: str
         """
-        return self._webhook
+        return self._table_name
 
-    @webhook.setter
-    def webhook(self, webhook):
-        """Sets the webhook of this NotificationWebhookConfig.
+    @table_name.setter
+    def table_name(self, table_name):
+        """Sets the table_name of this TestrunDeltaLakeInfo.
 
-        The URL of the destination webhook. It is not a strict requirement, but it is recommended that webhooks be preauthenticated by including a secure token in the URL.  # noqa: E501
+        The database table name to use.  # noqa: E501
 
-        :param webhook: The webhook of this NotificationWebhookConfig.  # noqa: E501
+        :param table_name: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
         :type: str
         """
+        if table_name is None:
+            raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
 
-        self._webhook = webhook
+        self._table_name = table_name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -82,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NotificationWebhookConfig, dict):
+        if issubclass(TestrunDeltaLakeInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -98,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NotificationWebhookConfig):
+        if not isinstance(other, TestrunDeltaLakeInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,42 +28,47 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'external_id': 'str',
-        'model_info': 'ModelModelInfo'
+        'model_info': 'ModelModelInfo',
+        'integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
         'external_id': 'externalId',
-        'model_info': 'modelInfo'
+        'model_info': 'modelInfo',
+        'integration_id': 'integrationId'
     }
 
-    def __init__(self, project_id=None, name=None, metadata=None, external_id=None, model_info=None):  # noqa: E501
+    def __init__(self, project_id=None, name=None, metadata=None, external_id=None, model_info=None, integration_id=None):  # noqa: E501
         """ProjectIdUuidModelBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._name = None
         self._metadata = None
         self._external_id = None
         self._model_info = None
+        self._integration_id = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         self.name = name
         if metadata is not None:
             self.metadata = metadata
         if external_id is not None:
             self.external_id = external_id
         if model_info is not None:
             self.model_info = model_info
+        if integration_id is not None:
+            self.integration_id = integration_id
 
     @property
     def project_id(self):
         """Gets the project_id of this ProjectIdUuidModelBody.  # noqa: E501
 
         Uniquely specifies a Project.  # noqa: E501
 
@@ -170,14 +175,35 @@
 
         :param model_info: The model_info of this ProjectIdUuidModelBody.  # noqa: E501
         :type: ModelModelInfo
         """
 
         self._model_info = model_info
 
+    @property
+    def integration_id(self):
+        """Gets the integration_id of this ProjectIdUuidModelBody.  # noqa: E501
+
+
+        :return: The integration_id of this ProjectIdUuidModelBody.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._integration_id
+
+    @integration_id.setter
+    def integration_id(self, integration_id):
+        """Sets the integration_id of this ProjectIdUuidModelBody.
+
+
+        :param integration_id: The integration_id of this ProjectIdUuidModelBody.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._integration_id = integration_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,15 +39,17 @@
         'model_task': 'RimeModelTask',
         'tags': 'list[str]',
         'firewall_ids': 'list[RimeUUID]',
         'project_test_suite_config': 'TestrunTestSuiteConfig',
         'profiling_config': 'TestrunProfilingConfig',
         'run_time_info': 'RuntimeinfoRunTimeInfo',
         'is_published': 'bool',
-        'last_test_run_time': 'datetime'
+        'last_test_run_time': 'datetime',
+        'stress_test_categories': 'list[TestrunTestCategoryType]',
+        'continuous_test_categories': 'list[TestrunTestCategoryType]'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'description': 'description',
         'use_case': 'useCase',
@@ -58,18 +60,20 @@
         'model_task': 'modelTask',
         'tags': 'tags',
         'firewall_ids': 'firewallIds',
         'project_test_suite_config': 'projectTestSuiteConfig',
         'profiling_config': 'profilingConfig',
         'run_time_info': 'runTimeInfo',
         'is_published': 'isPublished',
-        'last_test_run_time': 'lastTestRunTime'
+        'last_test_run_time': 'lastTestRunTime',
+        'stress_test_categories': 'stressTestCategories',
+        'continuous_test_categories': 'continuousTestCategories'
     }
 
-    def __init__(self, id=None, name=None, description=None, use_case=None, ethical_consideration=None, creation_time=None, owner_id=None, workspace_id=None, model_task=None, tags=None, firewall_ids=None, project_test_suite_config=None, profiling_config=None, run_time_info=None, is_published=None, last_test_run_time=None):  # noqa: E501
+    def __init__(self, id=None, name=None, description=None, use_case=None, ethical_consideration=None, creation_time=None, owner_id=None, workspace_id=None, model_task=None, tags=None, firewall_ids=None, project_test_suite_config=None, profiling_config=None, run_time_info=None, is_published=None, last_test_run_time=None, stress_test_categories=None, continuous_test_categories=None):  # noqa: E501
         """ProjectProject - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._name = None
         self._description = None
         self._use_case = None
         self._ethical_consideration = None
         self._creation_time = None
@@ -79,14 +83,16 @@
         self._tags = None
         self._firewall_ids = None
         self._project_test_suite_config = None
         self._profiling_config = None
         self._run_time_info = None
         self._is_published = None
         self._last_test_run_time = None
+        self._stress_test_categories = None
+        self._continuous_test_categories = None
         self.discriminator = None
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if description is not None:
             self.description = description
@@ -112,14 +118,18 @@
             self.profiling_config = profiling_config
         if run_time_info is not None:
             self.run_time_info = run_time_info
         if is_published is not None:
             self.is_published = is_published
         if last_test_run_time is not None:
             self.last_test_run_time = last_test_run_time
+        if stress_test_categories is not None:
+            self.stress_test_categories = stress_test_categories
+        if continuous_test_categories is not None:
+            self.continuous_test_categories = continuous_test_categories
 
     @property
     def id(self):
         """Gets the id of this ProjectProject.  # noqa: E501
 
 
         :return: The id of this ProjectProject.  # noqa: E501
@@ -457,14 +467,60 @@
 
         :param last_test_run_time: The last_test_run_time of this ProjectProject.  # noqa: E501
         :type: datetime
         """
 
         self._last_test_run_time = last_test_run_time
 
+    @property
+    def stress_test_categories(self):
+        """Gets the stress_test_categories of this ProjectProject.  # noqa: E501
+
+        List of test categories to be run in Stress Testing.  # noqa: E501
+
+        :return: The stress_test_categories of this ProjectProject.  # noqa: E501
+        :rtype: list[TestrunTestCategoryType]
+        """
+        return self._stress_test_categories
+
+    @stress_test_categories.setter
+    def stress_test_categories(self, stress_test_categories):
+        """Sets the stress_test_categories of this ProjectProject.
+
+        List of test categories to be run in Stress Testing.  # noqa: E501
+
+        :param stress_test_categories: The stress_test_categories of this ProjectProject.  # noqa: E501
+        :type: list[TestrunTestCategoryType]
+        """
+
+        self._stress_test_categories = stress_test_categories
+
+    @property
+    def continuous_test_categories(self):
+        """Gets the continuous_test_categories of this ProjectProject.  # noqa: E501
+
+        List of test categories to be run in Continuous Testing.  # noqa: E501
+
+        :return: The continuous_test_categories of this ProjectProject.  # noqa: E501
+        :rtype: list[TestrunTestCategoryType]
+        """
+        return self._continuous_test_categories
+
+    @continuous_test_categories.setter
+    def continuous_test_categories(self, continuous_test_categories):
+        """Sets the continuous_test_categories of this ProjectProject.
+
+        List of test categories to be run in Continuous Testing.  # noqa: E501
+
+        :param continuous_test_categories: The continuous_test_categories of this ProjectProject.  # noqa: E501
+        :type: list[TestrunTestCategoryType]
+        """
+
+        self._continuous_test_categories = continuous_test_categories
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeArchivedJobLogs(object):
+class StatedbArchivedJobLogs(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'url': 'url',
         'expiration_time': 'expirationTime'
     }
 
     def __init__(self, url=None, expiration_time=None):  # noqa: E501
-        """RimeArchivedJobLogs - a model defined in Swagger"""  # noqa: E501
+        """StatedbArchivedJobLogs - a model defined in Swagger"""  # noqa: E501
         self._url = None
         self._expiration_time = None
         self.discriminator = None
         if url is not None:
             self.url = url
         if expiration_time is not None:
             self.expiration_time = expiration_time
 
     @property
     def url(self):
-        """Gets the url of this RimeArchivedJobLogs.  # noqa: E501
+        """Gets the url of this StatedbArchivedJobLogs.  # noqa: E501
 
 
-        :return: The url of this RimeArchivedJobLogs.  # noqa: E501
+        :return: The url of this StatedbArchivedJobLogs.  # noqa: E501
         :rtype: RimeSafeURL
         """
         return self._url
 
     @url.setter
     def url(self, url):
-        """Sets the url of this RimeArchivedJobLogs.
+        """Sets the url of this StatedbArchivedJobLogs.
 
 
-        :param url: The url of this RimeArchivedJobLogs.  # noqa: E501
+        :param url: The url of this StatedbArchivedJobLogs.  # noqa: E501
         :type: RimeSafeURL
         """
 
         self._url = url
 
     @property
     def expiration_time(self):
-        """Gets the expiration_time of this RimeArchivedJobLogs.  # noqa: E501
+        """Gets the expiration_time of this StatedbArchivedJobLogs.  # noqa: E501
 
 
-        :return: The expiration_time of this RimeArchivedJobLogs.  # noqa: E501
+        :return: The expiration_time of this StatedbArchivedJobLogs.  # noqa: E501
         :rtype: datetime
         """
         return self._expiration_time
 
     @expiration_time.setter
     def expiration_time(self, expiration_time):
-        """Sets the expiration_time of this RimeArchivedJobLogs.
+        """Sets the expiration_time of this StatedbArchivedJobLogs.
 
 
-        :param expiration_time: The expiration_time of this RimeArchivedJobLogs.  # noqa: E501
+        :param expiration_time: The expiration_time of this StatedbArchivedJobLogs.  # noqa: E501
         :type: datetime
         """
 
         self._expiration_time = expiration_time
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeArchivedJobLogs, dict):
+        if issubclass(StatedbArchivedJobLogs, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeArchivedJobLogs):
+        if not isinstance(other, StatedbArchivedJobLogs):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeConfigType(object):
+class RimeTokenType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "CONFIG_TYPE_UNSPECIFIED"
-    TEST_RUN = "CONFIG_TYPE_TEST_RUN"
-    TEST_SUITE = "CONFIG_TYPE_TEST_SUITE"
-    TEST_RUN_INCREMENTAL = "CONFIG_TYPE_TEST_RUN_INCREMENTAL"
+    UNSPECIFIED = "TOKEN_TYPE_UNSPECIFIED"
+    USER = "TOKEN_TYPE_USER"
+    AGENT = "TOKEN_TYPE_AGENT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeConfigType - a model defined in Swagger"""  # noqa: E501
+        """RimeTokenType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeConfigType, dict):
+        if issubclass(RimeTokenType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeConfigType):
+        if not isinstance(other, RimeTokenType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,146 +11,119 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeCreateWorkspaceRequest(object):
+class RimeListImagesRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'name': 'str',
-        'agent_ids': 'list[RimeUUID]',
-        'default_agent_id': 'RimeUUID',
-        'description': 'str'
+        'page_token': 'str',
+        'page_size': 'str',
+        'pip_libraries': 'list[ListImagesRequestPipLibraryFilter]'
     }
 
     attribute_map = {
-        'name': 'name',
-        'agent_ids': 'agentIds',
-        'default_agent_id': 'defaultAgentId',
-        'description': 'description'
+        'page_token': 'pageToken',
+        'page_size': 'pageSize',
+        'pip_libraries': 'pipLibraries'
     }
 
-    def __init__(self, name=None, agent_ids=None, default_agent_id=None, description=None):  # noqa: E501
-        """RimeCreateWorkspaceRequest - a model defined in Swagger"""  # noqa: E501
-        self._name = None
-        self._agent_ids = None
-        self._default_agent_id = None
-        self._description = None
+    def __init__(self, page_token=None, page_size=None, pip_libraries=None):  # noqa: E501
+        """RimeListImagesRequest - a model defined in Swagger"""  # noqa: E501
+        self._page_token = None
+        self._page_size = None
+        self._pip_libraries = None
         self.discriminator = None
-        self.name = name
-        if agent_ids is not None:
-            self.agent_ids = agent_ids
-        if default_agent_id is not None:
-            self.default_agent_id = default_agent_id
-        if description is not None:
-            self.description = description
+        if page_token is not None:
+            self.page_token = page_token
+        if page_size is not None:
+            self.page_size = page_size
+        if pip_libraries is not None:
+            self.pip_libraries = pip_libraries
 
     @property
-    def name(self):
-        """Gets the name of this RimeCreateWorkspaceRequest.  # noqa: E501
+    def page_token(self):
+        """Gets the page_token of this RimeListImagesRequest.  # noqa: E501
 
-        Name of the Workspace.  # noqa: E501
+        Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.  # noqa: E501
 
-        :return: The name of this RimeCreateWorkspaceRequest.  # noqa: E501
+        :return: The page_token of this RimeListImagesRequest.  # noqa: E501
         :rtype: str
         """
-        return self._name
+        return self._page_token
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this RimeCreateWorkspaceRequest.
+    @page_token.setter
+    def page_token(self, page_token):
+        """Sets the page_token of this RimeListImagesRequest.
 
-        Name of the Workspace.  # noqa: E501
+        Specifies a page of the list returned by a ListImages query. The ListImages query returns a pageToken when there is more than one page of results.  # noqa: E501
 
-        :param name: The name of this RimeCreateWorkspaceRequest.  # noqa: E501
+        :param page_token: The page_token of this RimeListImagesRequest.  # noqa: E501
         :type: str
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._page_token = page_token
 
     @property
-    def agent_ids(self):
-        """Gets the agent_ids of this RimeCreateWorkspaceRequest.  # noqa: E501
+    def page_size(self):
+        """Gets the page_size of this RimeListImagesRequest.  # noqa: E501
 
-        List of Agent IDs to be added to the Workspace.  # noqa: E501
+        The maximum number of Image objects to return in a single page.  # noqa: E501
 
-        :return: The agent_ids of this RimeCreateWorkspaceRequest.  # noqa: E501
-        :rtype: list[RimeUUID]
-        """
-        return self._agent_ids
-
-    @agent_ids.setter
-    def agent_ids(self, agent_ids):
-        """Sets the agent_ids of this RimeCreateWorkspaceRequest.
-
-        List of Agent IDs to be added to the Workspace.  # noqa: E501
-
-        :param agent_ids: The agent_ids of this RimeCreateWorkspaceRequest.  # noqa: E501
-        :type: list[RimeUUID]
-        """
-
-        self._agent_ids = agent_ids
-
-    @property
-    def default_agent_id(self):
-        """Gets the default_agent_id of this RimeCreateWorkspaceRequest.  # noqa: E501
-
-
-        :return: The default_agent_id of this RimeCreateWorkspaceRequest.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The page_size of this RimeListImagesRequest.  # noqa: E501
+        :rtype: str
         """
-        return self._default_agent_id
+        return self._page_size
 
-    @default_agent_id.setter
-    def default_agent_id(self, default_agent_id):
-        """Sets the default_agent_id of this RimeCreateWorkspaceRequest.
+    @page_size.setter
+    def page_size(self, page_size):
+        """Sets the page_size of this RimeListImagesRequest.
 
+        The maximum number of Image objects to return in a single page.  # noqa: E501
 
-        :param default_agent_id: The default_agent_id of this RimeCreateWorkspaceRequest.  # noqa: E501
-        :type: RimeUUID
+        :param page_size: The page_size of this RimeListImagesRequest.  # noqa: E501
+        :type: str
         """
 
-        self._default_agent_id = default_agent_id
+        self._page_size = page_size
 
     @property
-    def description(self):
-        """Gets the description of this RimeCreateWorkspaceRequest.  # noqa: E501
+    def pip_libraries(self):
+        """Gets the pip_libraries of this RimeListImagesRequest.  # noqa: E501
 
-        Description of the Workspace.  # noqa: E501
+        Optional. Filters the list for libraries that are installed on the Managed Image. The filter is only active when the list is not empty. When this filter is specified, do not include a pageToken field in the request.  # noqa: E501
 
-        :return: The description of this RimeCreateWorkspaceRequest.  # noqa: E501
-        :rtype: str
+        :return: The pip_libraries of this RimeListImagesRequest.  # noqa: E501
+        :rtype: list[ListImagesRequestPipLibraryFilter]
         """
-        return self._description
+        return self._pip_libraries
 
-    @description.setter
-    def description(self, description):
-        """Sets the description of this RimeCreateWorkspaceRequest.
+    @pip_libraries.setter
+    def pip_libraries(self, pip_libraries):
+        """Sets the pip_libraries of this RimeListImagesRequest.
 
-        Description of the Workspace.  # noqa: E501
+        Optional. Filters the list for libraries that are installed on the Managed Image. The filter is only active when the list is not empty. When this filter is specified, do not include a pageToken field in the request.  # noqa: E501
 
-        :param description: The description of this RimeCreateWorkspaceRequest.  # noqa: E501
-        :type: str
+        :param pip_libraries: The pip_libraries of this RimeListImagesRequest.  # noqa: E501
+        :type: list[ListImagesRequestPipLibraryFilter]
         """
 
-        self._description = description
+        self._pip_libraries = pip_libraries
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -165,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeCreateWorkspaceRequest, dict):
+        if issubclass(RimeListImagesRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -181,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeCreateWorkspaceRequest):
+        if not isinstance(other, RimeListImagesRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         'creation_time': 'datetime',
         'completion_time': 'datetime',
         'running_time_secs': 'float',
         'job_data': 'RimeJobData',
         'job_progress_str': 'str',
         'cancellation_requested': 'bool',
         'agent_id': 'RimeUUID',
-        'archived_job_logs': 'RimeArchivedJobLogs',
+        'archived_job_logs': 'StatedbArchivedJobLogs',
         'error_msg': 'str'
     }
 
     attribute_map = {
         'job_id': 'jobId',
         'termination_reason': 'terminationReason',
         'job_type': 'jobType',
@@ -375,25 +375,25 @@
 
     @property
     def archived_job_logs(self):
         """Gets the archived_job_logs of this RimeJobMetadata.  # noqa: E501
 
 
         :return: The archived_job_logs of this RimeJobMetadata.  # noqa: E501
-        :rtype: RimeArchivedJobLogs
+        :rtype: StatedbArchivedJobLogs
         """
         return self._archived_job_logs
 
     @archived_job_logs.setter
     def archived_job_logs(self, archived_job_logs):
         """Sets the archived_job_logs of this RimeJobMetadata.
 
 
         :param archived_job_logs: The archived_job_logs of this RimeJobMetadata.  # noqa: E501
-        :type: RimeArchivedJobLogs
+        :type: StatedbArchivedJobLogs
         """
 
         self._archived_job_logs = archived_job_logs
 
     @property
     def error_msg(self):
         """Gets the error_msg of this RimeJobMetadata.  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,41 +11,34 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTokenType(object):
+class RimeUpdateWorkspaceResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "TOKEN_TYPE_UNSPECIFIED"
-    USER = "TOKEN_TYPE_USER"
-    AGENT = "TOKEN_TYPE_AGENT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTokenType - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTokenType, dict):
+        if issubclass(RimeUpdateWorkspaceResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTokenType):
+        if not isinstance(other, RimeUpdateWorkspaceResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateWorkspaceResponse(object):
+class RimeUpsertFeatureFlagsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateWorkspaceResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpsertFeatureFlagsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateWorkspaceResponse, dict):
+        if issubclass(RimeUpsertFeatureFlagsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateWorkspaceResponse):
+        if not isinstance(other, RimeUpsertFeatureFlagsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,34 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpsertFeatureFlagsResponse(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpsertFeatureFlagsResponse - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpsertFeatureFlagsResponse, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpsertFeatureFlagsResponse):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,43 +28,48 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'name': 'str',
         'agent_ids': 'list[RimeUUID]',
         'default_agent_id': 'RimeUUID',
         'workspace_id': 'RimeUUID',
-        'description': 'str'
+        'description': 'str',
+        'results_retention_in_days': 'int'
     }
 
     attribute_map = {
         'name': 'name',
         'agent_ids': 'agentIds',
         'default_agent_id': 'defaultAgentId',
         'workspace_id': 'workspaceId',
-        'description': 'description'
+        'description': 'description',
+        'results_retention_in_days': 'resultsRetentionInDays'
     }
 
-    def __init__(self, name=None, agent_ids=None, default_agent_id=None, workspace_id=None, description=None):  # noqa: E501
+    def __init__(self, name=None, agent_ids=None, default_agent_id=None, workspace_id=None, description=None, results_retention_in_days=None):  # noqa: E501
         """RimeWorkspace - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._agent_ids = None
         self._default_agent_id = None
         self._workspace_id = None
         self._description = None
+        self._results_retention_in_days = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if agent_ids is not None:
             self.agent_ids = agent_ids
         if default_agent_id is not None:
             self.default_agent_id = default_agent_id
         if workspace_id is not None:
             self.workspace_id = workspace_id
         if description is not None:
             self.description = description
+        if results_retention_in_days is not None:
+            self.results_retention_in_days = results_retention_in_days
 
     @property
     def name(self):
         """Gets the name of this RimeWorkspace.  # noqa: E501
 
         Name of the Workspace.  # noqa: E501
 
@@ -169,14 +174,35 @@
 
         :param description: The description of this RimeWorkspace.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
+    @property
+    def results_retention_in_days(self):
+        """Gets the results_retention_in_days of this RimeWorkspace.  # noqa: E501
+
+
+        :return: The results_retention_in_days of this RimeWorkspace.  # noqa: E501
+        :rtype: int
+        """
+        return self._results_retention_in_days
+
+    @results_retention_in_days.setter
+    def results_retention_in_days(self, results_retention_in_days):
+        """Sets the results_retention_in_days of this RimeWorkspace.
+
+
+        :param results_retention_in_days: The results_retention_in_days of this RimeWorkspace.  # noqa: E501
+        :type: int
+        """
+
+        self._results_retention_in_days = results_retention_in_days
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'name': 'bool',
         'agent_ids': 'bool',
         'default_agent_id': 'bool',
-        'description': 'bool'
+        'description': 'bool',
+        'results_retention_in_days': 'bool'
     }
 
     attribute_map = {
         'name': 'name',
         'agent_ids': 'agentIds',
         'default_agent_id': 'defaultAgentId',
-        'description': 'description'
+        'description': 'description',
+        'results_retention_in_days': 'resultsRetentionInDays'
     }
 
-    def __init__(self, name=None, agent_ids=None, default_agent_id=None, description=None):  # noqa: E501
+    def __init__(self, name=None, agent_ids=None, default_agent_id=None, description=None, results_retention_in_days=None):  # noqa: E501
         """RimeWorkspaceWriteMask - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._agent_ids = None
         self._default_agent_id = None
         self._description = None
+        self._results_retention_in_days = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if agent_ids is not None:
             self.agent_ids = agent_ids
         if default_agent_id is not None:
             self.default_agent_id = default_agent_id
         if description is not None:
             self.description = description
+        if results_retention_in_days is not None:
+            self.results_retention_in_days = results_retention_in_days
 
     @property
     def name(self):
         """Gets the name of this RimeWorkspaceWriteMask.  # noqa: E501
 
         Specifies whether to update name.  # noqa: E501
 
@@ -145,14 +150,37 @@
 
         :param description: The description of this RimeWorkspaceWriteMask.  # noqa: E501
         :type: bool
         """
 
         self._description = description
 
+    @property
+    def results_retention_in_days(self):
+        """Gets the results_retention_in_days of this RimeWorkspaceWriteMask.  # noqa: E501
+
+        Specifies whether to results retention in days.  # noqa: E501
+
+        :return: The results_retention_in_days of this RimeWorkspaceWriteMask.  # noqa: E501
+        :rtype: bool
+        """
+        return self._results_retention_in_days
+
+    @results_retention_in_days.setter
+    def results_retention_in_days(self, results_retention_in_days):
+        """Sets the results_retention_in_days of this RimeWorkspaceWriteMask.
+
+        Specifies whether to results retention in days.  # noqa: E501
+
+        :param results_retention_in_days: The results_retention_in_days of this RimeWorkspaceWriteMask.  # noqa: E501
+        :type: bool
+        """
+
+        self._results_retention_in_days = results_retention_in_days
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,18 +56,16 @@
         self._range_lower_bound = None
         self._range_upper_bound = None
         self._run_subset_performance = None
         self._run_subset_performance_drift = None
         self._run_overall_performance = None
         self._metadata = None
         self.discriminator = None
-        if name is not None:
-            self.name = name
-        if file_path is not None:
-            self.file_path = file_path
+        self.name = name
+        self.file_path = file_path
         if range_lower_bound is not None:
             self.range_lower_bound = range_lower_bound
         if range_upper_bound is not None:
             self.range_upper_bound = range_upper_bound
         if run_subset_performance is not None:
             self.run_subset_performance = run_subset_performance
         if run_subset_performance_drift is not None:
@@ -93,14 +91,16 @@
         """Sets the name of this TestrunCustomMetric.
 
         Name of the custom metric.  # noqa: E501
 
         :param name: The name of this TestrunCustomMetric.  # noqa: E501
         :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
         self._name = name
 
     @property
     def file_path(self):
         """Gets the file_path of this TestrunCustomMetric.  # noqa: E501
 
@@ -116,14 +116,16 @@
         """Sets the file_path of this TestrunCustomMetric.
 
         Path to the file with metric definition.  # noqa: E501
 
         :param file_path: The file_path of this TestrunCustomMetric.  # noqa: E501
         :type: str
         """
+        if file_path is None:
+            raise ValueError("Invalid value for `file_path`, must not be `None`")  # noqa: E501
 
         self._file_path = file_path
 
     @property
     def range_lower_bound(self):
         """Gets the range_lower_bound of this TestrunCustomMetric.  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,119 +11,119 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataCollectorInfo(object):
+class TestrunresultListTestRunsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data_stream_id': 'RimeUUID',
-        'start_time': 'str',
-        'end_time': 'str'
+        'test_runs': 'list[TestrunresultTestRunDetail]',
+        'next_page_token': 'str',
+        'has_more': 'bool'
     }
 
     attribute_map = {
-        'data_stream_id': 'dataStreamId',
-        'start_time': 'startTime',
-        'end_time': 'endTime'
+        'test_runs': 'testRuns',
+        'next_page_token': 'nextPageToken',
+        'has_more': 'hasMore'
     }
 
-    def __init__(self, data_stream_id=None, start_time=None, end_time=None):  # noqa: E501
-        """TestrunDataCollectorInfo - a model defined in Swagger"""  # noqa: E501
-        self._data_stream_id = None
-        self._start_time = None
-        self._end_time = None
+    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
+        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_runs = None
+        self._next_page_token = None
+        self._has_more = None
         self.discriminator = None
-        if data_stream_id is not None:
-            self.data_stream_id = data_stream_id
-        self.start_time = start_time
-        self.end_time = end_time
+        if test_runs is not None:
+            self.test_runs = test_runs
+        if next_page_token is not None:
+            self.next_page_token = next_page_token
+        if has_more is not None:
+            self.has_more = has_more
 
     @property
-    def data_stream_id(self):
-        """Gets the data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
+    def test_runs(self):
+        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
 
+        The details of the test runs.  # noqa: E501
 
-        :return: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :rtype: list[TestrunresultTestRunDetail]
         """
-        return self._data_stream_id
+        return self._test_runs
 
-    @data_stream_id.setter
-    def data_stream_id(self, data_stream_id):
-        """Sets the data_stream_id of this TestrunDataCollectorInfo.
+    @test_runs.setter
+    def test_runs(self, test_runs):
+        """Sets the test_runs of this TestrunresultListTestRunsResponse.
 
+        The details of the test runs.  # noqa: E501
 
-        :param data_stream_id: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
-        :type: RimeUUID
+        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :type: list[TestrunresultTestRunDetail]
         """
 
-        self._data_stream_id = data_stream_id
+        self._test_runs = test_runs
 
     @property
-    def start_time(self):
-        """Gets the start_time of this TestrunDataCollectorInfo.  # noqa: E501
+    def next_page_token(self):
+        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
 
-        The start time in seconds.  # noqa: E501
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :return: The start_time of this TestrunDataCollectorInfo.  # noqa: E501
+        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :rtype: str
         """
-        return self._start_time
+        return self._next_page_token
 
-    @start_time.setter
-    def start_time(self, start_time):
-        """Sets the start_time of this TestrunDataCollectorInfo.
+    @next_page_token.setter
+    def next_page_token(self, next_page_token):
+        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
 
-        The start time in seconds.  # noqa: E501
+        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
 
-        :param start_time: The start_time of this TestrunDataCollectorInfo.  # noqa: E501
+        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
         :type: str
         """
-        if start_time is None:
-            raise ValueError("Invalid value for `start_time`, must not be `None`")  # noqa: E501
 
-        self._start_time = start_time
+        self._next_page_token = next_page_token
 
     @property
-    def end_time(self):
-        """Gets the end_time of this TestrunDataCollectorInfo.  # noqa: E501
+    def has_more(self):
+        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
 
-        The end time in seconds.  # noqa: E501
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The end_time of this TestrunDataCollectorInfo.  # noqa: E501
-        :rtype: str
+        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :rtype: bool
         """
-        return self._end_time
+        return self._has_more
 
-    @end_time.setter
-    def end_time(self, end_time):
-        """Sets the end_time of this TestrunDataCollectorInfo.
+    @has_more.setter
+    def has_more(self, has_more):
+        """Sets the has_more of this TestrunresultListTestRunsResponse.
 
-        The end time in seconds.  # noqa: E501
+        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param end_time: The end_time of this TestrunDataCollectorInfo.  # noqa: E501
-        :type: str
+        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :type: bool
         """
-        if end_time is None:
-            raise ValueError("Invalid value for `end_time`, must not be `None`")  # noqa: E501
 
-        self._end_time = end_time
+        self._has_more = has_more
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +138,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataCollectorInfo, dict):
+        if issubclass(TestrunresultListTestRunsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +154,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataCollectorInfo):
+        if not isinstance(other, TestrunresultListTestRunsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,117 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestCategory(object):
+class TestrunTestRunIncrementalConfig(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'type': 'TestrunTestCategoryType',
-        'run_st': 'bool',
-        'run_ct': 'bool'
+        'eval_dataset_id': 'str',
+        'run_time_info': 'RuntimeinfoRunTimeInfo'
     }
 
     attribute_map = {
-        'type': 'type',
-        'run_st': 'runSt',
-        'run_ct': 'runCt'
+        'eval_dataset_id': 'evalDatasetId',
+        'run_time_info': 'runTimeInfo'
     }
 
-    def __init__(self, type=None, run_st=None, run_ct=None):  # noqa: E501
-        """TestrunTestCategory - a model defined in Swagger"""  # noqa: E501
-        self._type = None
-        self._run_st = None
-        self._run_ct = None
+    def __init__(self, eval_dataset_id=None, run_time_info=None):  # noqa: E501
+        """TestrunTestRunIncrementalConfig - a model defined in Swagger"""  # noqa: E501
+        self._eval_dataset_id = None
+        self._run_time_info = None
         self.discriminator = None
-        if type is not None:
-            self.type = type
-        if run_st is not None:
-            self.run_st = run_st
-        if run_ct is not None:
-            self.run_ct = run_ct
+        if eval_dataset_id is not None:
+            self.eval_dataset_id = eval_dataset_id
+        if run_time_info is not None:
+            self.run_time_info = run_time_info
 
     @property
-    def type(self):
-        """Gets the type of this TestrunTestCategory.  # noqa: E501
+    def eval_dataset_id(self):
+        """Gets the eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
 
+        Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :return: The type of this TestrunTestCategory.  # noqa: E501
-        :rtype: TestrunTestCategoryType
+        :return: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
+        :rtype: str
         """
-        return self._type
+        return self._eval_dataset_id
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this TestrunTestCategory.
+    @eval_dataset_id.setter
+    def eval_dataset_id(self, eval_dataset_id):
+        """Sets the eval_dataset_id of this TestrunTestRunIncrementalConfig.
 
+        Uniquely specifies an evaluation Dataset.  # noqa: E501
 
-        :param type: The type of this TestrunTestCategory.  # noqa: E501
-        :type: TestrunTestCategoryType
+        :param eval_dataset_id: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
+        :type: str
         """
 
-        self._type = type
+        self._eval_dataset_id = eval_dataset_id
 
     @property
-    def run_st(self):
-        """Gets the run_st of this TestrunTestCategory.  # noqa: E501
+    def run_time_info(self):
+        """Gets the run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
 
-        Specifies whether to run this test in Stress Testing.  # noqa: E501
 
-        :return: The run_st of this TestrunTestCategory.  # noqa: E501
-        :rtype: bool
+        :return: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
+        :rtype: RuntimeinfoRunTimeInfo
         """
-        return self._run_st
+        return self._run_time_info
 
-    @run_st.setter
-    def run_st(self, run_st):
-        """Sets the run_st of this TestrunTestCategory.
+    @run_time_info.setter
+    def run_time_info(self, run_time_info):
+        """Sets the run_time_info of this TestrunTestRunIncrementalConfig.
 
-        Specifies whether to run this test in Stress Testing.  # noqa: E501
 
-        :param run_st: The run_st of this TestrunTestCategory.  # noqa: E501
-        :type: bool
+        :param run_time_info: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
+        :type: RuntimeinfoRunTimeInfo
         """
 
-        self._run_st = run_st
-
-    @property
-    def run_ct(self):
-        """Gets the run_ct of this TestrunTestCategory.  # noqa: E501
-
-        Specifies whether to run this test in Continuous Testing.  # noqa: E501
-
-        :return: The run_ct of this TestrunTestCategory.  # noqa: E501
-        :rtype: bool
-        """
-        return self._run_ct
-
-    @run_ct.setter
-    def run_ct(self, run_ct):
-        """Sets the run_ct of this TestrunTestCategory.
-
-        Specifies whether to run this test in Continuous Testing.  # noqa: E501
-
-        :param run_ct: The run_ct of this TestrunTestCategory.  # noqa: E501
-        :type: bool
-        """
-
-        self._run_ct = run_ct
+        self._run_time_info = run_time_info
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -136,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestCategory, dict):
+        if issubclass(TestrunTestRunIncrementalConfig, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -152,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestCategory):
+        if not isinstance(other, TestrunTestRunIncrementalConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,44 +29,49 @@
     """
     swagger_types = {
         'run_name': 'str',
         'model_id': 'RimeUUID',
         'data_info': 'TestrunDataInfo',
         'run_time_info': 'RuntimeinfoRunTimeInfo',
         'profiling_config': 'TestrunProfilingConfig',
-        'test_suite_config': 'TestrunTestSuiteConfig'
+        'test_suite_config': 'TestrunTestSuiteConfig',
+        'categories': 'list[TestrunTestCategoryType]'
     }
 
     attribute_map = {
         'run_name': 'runName',
         'model_id': 'modelId',
         'data_info': 'dataInfo',
         'run_time_info': 'runTimeInfo',
         'profiling_config': 'profilingConfig',
-        'test_suite_config': 'testSuiteConfig'
+        'test_suite_config': 'testSuiteConfig',
+        'categories': 'categories'
     }
 
-    def __init__(self, run_name=None, model_id=None, data_info=None, run_time_info=None, profiling_config=None, test_suite_config=None):  # noqa: E501
+    def __init__(self, run_name=None, model_id=None, data_info=None, run_time_info=None, profiling_config=None, test_suite_config=None, categories=None):  # noqa: E501
         """TestrunTestRunConfig - a model defined in Swagger"""  # noqa: E501
         self._run_name = None
         self._model_id = None
         self._data_info = None
         self._run_time_info = None
         self._profiling_config = None
         self._test_suite_config = None
+        self._categories = None
         self.discriminator = None
         self.run_name = run_name
         self.model_id = model_id
         self.data_info = data_info
         if run_time_info is not None:
             self.run_time_info = run_time_info
         if profiling_config is not None:
             self.profiling_config = profiling_config
         if test_suite_config is not None:
             self.test_suite_config = test_suite_config
+        if categories is not None:
+            self.categories = categories
 
     @property
     def run_name(self):
         """Gets the run_name of this TestrunTestRunConfig.  # noqa: E501
 
         Name for this Test Run.  # noqa: E501
 
@@ -194,14 +199,37 @@
 
         :param test_suite_config: The test_suite_config of this TestrunTestRunConfig.  # noqa: E501
         :type: TestrunTestSuiteConfig
         """
 
         self._test_suite_config = test_suite_config
 
+    @property
+    def categories(self):
+        """Gets the categories of this TestrunTestRunConfig.  # noqa: E501
+
+        List of test categories to be run.  # noqa: E501
+
+        :return: The categories of this TestrunTestRunConfig.  # noqa: E501
+        :rtype: list[TestrunTestCategoryType]
+        """
+        return self._categories
+
+    @categories.setter
+    def categories(self, categories):
+        """Sets the categories of this TestrunTestRunConfig.
+
+        List of test categories to be run.  # noqa: E501
+
+        :param categories: The categories of this TestrunTestRunConfig.  # noqa: E501
+        :type: list[TestrunTestCategoryType]
+        """
+
+        self._categories = categories
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestRunIncrementalConfig(object):
+class UsersUserUserIdUuidBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'eval_dataset_id': 'str',
-        'run_time_info': 'RuntimeinfoRunTimeInfo'
+        'project_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
-        'eval_dataset_id': 'evalDatasetId',
-        'run_time_info': 'runTimeInfo'
+        'project_id': 'projectId',
+        'user': 'user'
     }
 
-    def __init__(self, eval_dataset_id=None, run_time_info=None):  # noqa: E501
-        """TestrunTestRunIncrementalConfig - a model defined in Swagger"""  # noqa: E501
-        self._eval_dataset_id = None
-        self._run_time_info = None
+    def __init__(self, project_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._project_id = None
+        self._user = None
         self.discriminator = None
-        if eval_dataset_id is not None:
-            self.eval_dataset_id = eval_dataset_id
-        if run_time_info is not None:
-            self.run_time_info = run_time_info
+        if project_id is not None:
+            self.project_id = project_id
+        if user is not None:
+            self.user = user
 
     @property
-    def eval_dataset_id(self):
-        """Gets the eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
+    def project_id(self):
+        """Gets the project_id of this UsersUserUserIdUuidBody.  # noqa: E501
 
-        Uniquely specifies an evaluation Dataset.  # noqa: E501
+        Uniquely specifies a Project.  # noqa: E501
 
-        :return: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :rtype: str
+        :return: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :rtype: object
         """
-        return self._eval_dataset_id
+        return self._project_id
 
-    @eval_dataset_id.setter
-    def eval_dataset_id(self, eval_dataset_id):
-        """Sets the eval_dataset_id of this TestrunTestRunIncrementalConfig.
+    @project_id.setter
+    def project_id(self, project_id):
+        """Sets the project_id of this UsersUserUserIdUuidBody.
 
-        Uniquely specifies an evaluation Dataset.  # noqa: E501
+        Uniquely specifies a Project.  # noqa: E501
 
-        :param eval_dataset_id: The eval_dataset_id of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :type: str
+        :param project_id: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :type: object
         """
 
-        self._eval_dataset_id = eval_dataset_id
+        self._project_id = project_id
 
     @property
-    def run_time_info(self):
-        """Gets the run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody.  # noqa: E501
 
 
-        :return: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :rtype: RuntimeinfoRunTimeInfo
+        :return: The user of this UsersUserUserIdUuidBody.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._run_time_info
+        return self._user
 
-    @run_time_info.setter
-    def run_time_info(self, run_time_info):
-        """Sets the run_time_info of this TestrunTestRunIncrementalConfig.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody.
 
 
-        :param run_time_info: The run_time_info of this TestrunTestRunIncrementalConfig.  # noqa: E501
-        :type: RuntimeinfoRunTimeInfo
+        :param user: The user of this UsersUserUserIdUuidBody.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._run_time_info = run_time_info
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestRunIncrementalConfig, dict):
+        if issubclass(UsersUserUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestRunIncrementalConfig):
+        if not isinstance(other, UsersUserUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,72 +24,44 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'categories': 'list[TestrunTestCategory]',
         'global_test_sensitivity': 'TestrunTestSensitivity',
         'individual_tests_config': 'str',
         'custom_tests': 'list[str]',
         'global_exclude_columns': 'list[str]'
     }
 
     attribute_map = {
-        'categories': 'categories',
         'global_test_sensitivity': 'globalTestSensitivity',
         'individual_tests_config': 'individualTestsConfig',
         'custom_tests': 'customTests',
         'global_exclude_columns': 'globalExcludeColumns'
     }
 
-    def __init__(self, categories=None, global_test_sensitivity=None, individual_tests_config=None, custom_tests=None, global_exclude_columns=None):  # noqa: E501
+    def __init__(self, global_test_sensitivity=None, individual_tests_config=None, custom_tests=None, global_exclude_columns=None):  # noqa: E501
         """TestrunTestSuiteConfig - a model defined in Swagger"""  # noqa: E501
-        self._categories = None
         self._global_test_sensitivity = None
         self._individual_tests_config = None
         self._custom_tests = None
         self._global_exclude_columns = None
         self.discriminator = None
-        if categories is not None:
-            self.categories = categories
         if global_test_sensitivity is not None:
             self.global_test_sensitivity = global_test_sensitivity
         if individual_tests_config is not None:
             self.individual_tests_config = individual_tests_config
         if custom_tests is not None:
             self.custom_tests = custom_tests
         if global_exclude_columns is not None:
             self.global_exclude_columns = global_exclude_columns
 
     @property
-    def categories(self):
-        """Gets the categories of this TestrunTestSuiteConfig.  # noqa: E501
-
-        List of test categories to be run.  # noqa: E501
-
-        :return: The categories of this TestrunTestSuiteConfig.  # noqa: E501
-        :rtype: list[TestrunTestCategory]
-        """
-        return self._categories
-
-    @categories.setter
-    def categories(self, categories):
-        """Sets the categories of this TestrunTestSuiteConfig.
-
-        List of test categories to be run.  # noqa: E501
-
-        :param categories: The categories of this TestrunTestSuiteConfig.  # noqa: E501
-        :type: list[TestrunTestCategory]
-        """
-
-        self._categories = categories
-
-    @property
     def global_test_sensitivity(self):
         """Gets the global_test_sensitivity of this TestrunTestSuiteConfig.  # noqa: E501
 
 
         :return: The global_test_sensitivity of this TestrunTestSuiteConfig.  # noqa: E501
         :rtype: TestrunTestSensitivity
         """
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,119 +11,117 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultListTestRunsResponse(object):
+class TestrunresultTestCaseDisplay(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_runs': 'list[TestrunresultTestRunDetail]',
-        'next_page_token': 'str',
-        'has_more': 'bool'
+        'table_info': 'str',
+        'details': 'str',
+        'details_layout': 'list[str]'
     }
 
     attribute_map = {
-        'test_runs': 'testRuns',
-        'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'table_info': 'tableInfo',
+        'details': 'details',
+        'details_layout': 'detailsLayout'
     }
 
-    def __init__(self, test_runs=None, next_page_token=None, has_more=None):  # noqa: E501
-        """TestrunresultListTestRunsResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_runs = None
-        self._next_page_token = None
-        self._has_more = None
+    def __init__(self, table_info=None, details=None, details_layout=None):  # noqa: E501
+        """TestrunresultTestCaseDisplay - a model defined in Swagger"""  # noqa: E501
+        self._table_info = None
+        self._details = None
+        self._details_layout = None
         self.discriminator = None
-        if test_runs is not None:
-            self.test_runs = test_runs
-        if next_page_token is not None:
-            self.next_page_token = next_page_token
-        if has_more is not None:
-            self.has_more = has_more
+        if table_info is not None:
+            self.table_info = table_info
+        if details is not None:
+            self.details = details
+        if details_layout is not None:
+            self.details_layout = details_layout
 
     @property
-    def test_runs(self):
-        """Gets the test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def table_info(self):
+        """Gets the table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        The details of the test runs.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :return: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: list[TestrunresultTestRunDetail]
+        :return: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: str
         """
-        return self._test_runs
+        return self._table_info
 
-    @test_runs.setter
-    def test_runs(self, test_runs):
-        """Sets the test_runs of this TestrunresultListTestRunsResponse.
+    @table_info.setter
+    def table_info(self, table_info):
+        """Sets the table_info of this TestrunresultTestCaseDisplay.
 
-        The details of the test runs.  # noqa: E501
+        Table info contains information for displaying the test case in a table in the FE.  # noqa: E501
 
-        :param test_runs: The test_runs of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: list[TestrunresultTestRunDetail]
+        :param table_info: The table_info of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: str
         """
 
-        self._test_runs = test_runs
+        self._table_info = table_info
 
     @property
-    def next_page_token(self):
-        """Gets the next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def details(self):
+        """Gets the details of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :return: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :return: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :rtype: str
         """
-        return self._next_page_token
+        return self._details
 
-    @next_page_token.setter
-    def next_page_token(self, next_page_token):
-        """Sets the next_page_token of this TestrunresultListTestRunsResponse.
+    @details.setter
+    def details(self, details):
+        """Sets the details of this TestrunresultTestCaseDisplay.
 
-        A token representing the next page from the list returned by a ListTestRuns query.  # noqa: E501
+        Details includes ML-specified details for the test case. This can include graphs, HTML, etc.  # noqa: E501
 
-        :param next_page_token: The next_page_token of this TestrunresultListTestRunsResponse.  # noqa: E501
+        :param details: The details of this TestrunresultTestCaseDisplay.  # noqa: E501
         :type: str
         """
 
-        self._next_page_token = next_page_token
+        self._details = details
 
     @property
-    def has_more(self):
-        """Gets the has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
+    def details_layout(self):
+        """Gets the details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :return: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :rtype: bool
+        :return: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :rtype: list[str]
         """
-        return self._has_more
+        return self._details_layout
 
-    @has_more.setter
-    def has_more(self, has_more):
-        """Sets the has_more of this TestrunresultListTestRunsResponse.
+    @details_layout.setter
+    def details_layout(self, details_layout):
+        """Sets the details_layout of this TestrunresultTestCaseDisplay.
 
-        A Boolean that specifies whether there are more test runs to return.  # noqa: E501
 
-        :param has_more: The has_more of this TestrunresultListTestRunsResponse.  # noqa: E501
-        :type: bool
+        :param details_layout: The details_layout of this TestrunresultTestCaseDisplay.  # noqa: E501
+        :type: list[str]
         """
 
-        self._has_more = has_more
+        self._details_layout = details_layout
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +136,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultListTestRunsResponse, dict):
+        if issubclass(TestrunresultTestCaseDisplay, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -154,15 +152,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultListTestRunsResponse):
+        if not isinstance(other, TestrunresultTestCaseDisplay):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,42 +11,45 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class RimeConfigType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
+    UNSPECIFIED = "CONFIG_TYPE_UNSPECIFIED"
+    TEST_RUN = "CONFIG_TYPE_TEST_RUN"
+    TEST_SUITE = "CONFIG_TYPE_TEST_SUITE"
+    TEST_RUN_INCREMENTAL = "CONFIG_TYPE_TEST_RUN_INCREMENTAL"
+    PROFILING = "CONFIG_TYPE_PROFILING"
+    DATA_PROFILING = "CONFIG_TYPE_DATA_PROFILING"
+    MODEL_PROFILING = "CONFIG_TYPE_MODEL_PROFILING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+        """RimeConfigType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +65,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(RimeConfigType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +81,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, RimeConfigType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,89 +11,91 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody(object):
+class WorkspaceIdUuidUsersBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'project_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'workspace_id': 'object',
+        'users': 'list[RimeUserWithRole]'
     }
 
     attribute_map = {
-        'project_id': 'projectId',
-        'user': 'user'
+        'workspace_id': 'workspaceId',
+        'users': 'users'
     }
 
-    def __init__(self, project_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
-        self._project_id = None
-        self._user = None
+    def __init__(self, workspace_id=None, users=None):  # noqa: E501
+        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
+        self._users = None
         self.discriminator = None
-        if project_id is not None:
-            self.project_id = project_id
-        if user is not None:
-            self.user = user
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
+        if users is not None:
+            self.users = users
 
     @property
-    def project_id(self):
-        """Gets the project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
-        Uniquely specifies a Project.  # noqa: E501
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :rtype: object
         """
-        return self._project_id
+        return self._workspace_id
 
-    @project_id.setter
-    def project_id(self, project_id):
-        """Sets the project_id of this UsersUserUserIdUuidBody.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
 
-        Uniquely specifies a Project.  # noqa: E501
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param project_id: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
         :type: object
         """
 
-        self._project_id = project_id
+        self._workspace_id = workspace_id
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody.  # noqa: E501
+    def users(self):
+        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
 
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :return: The user of this UsersUserUserIdUuidBody.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :rtype: list[RimeUserWithRole]
         """
-        return self._user
+        return self._users
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody.
+    @users.setter
+    def users(self, users):
+        """Sets the users of this WorkspaceIdUuidUsersBody.
 
+        List of Users to add to the Workspace.  # noqa: E501
 
-        :param user: The user of this UsersUserUserIdUuidBody.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :type: list[RimeUserWithRole]
         """
 
-        self._user = user
+        self._users = users
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +110,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserUserIdUuidBody, dict):
+        if issubclass(WorkspaceIdUuidUsersBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +126,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserUserIdUuidBody):
+        if not isinstance(other, WorkspaceIdUuidUsersBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,43 +28,48 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'name': 'str',
         'agent_ids': 'list[RimeUUID]',
         'default_agent_id': 'RimeUUID',
         'workspace_id': 'object',
-        'description': 'str'
+        'description': 'str',
+        'results_retention_in_days': 'int'
     }
 
     attribute_map = {
         'name': 'name',
         'agent_ids': 'agentIds',
         'default_agent_id': 'defaultAgentId',
         'workspace_id': 'workspaceId',
-        'description': 'description'
+        'description': 'description',
+        'results_retention_in_days': 'resultsRetentionInDays'
     }
 
-    def __init__(self, name=None, agent_ids=None, default_agent_id=None, workspace_id=None, description=None):  # noqa: E501
+    def __init__(self, name=None, agent_ids=None, default_agent_id=None, workspace_id=None, description=None, results_retention_in_days=None):  # noqa: E501
         """V1workspaceworkspaceWorkspaceIdUuidWorkspace - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._agent_ids = None
         self._default_agent_id = None
         self._workspace_id = None
         self._description = None
+        self._results_retention_in_days = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if agent_ids is not None:
             self.agent_ids = agent_ids
         if default_agent_id is not None:
             self.default_agent_id = default_agent_id
         if workspace_id is not None:
             self.workspace_id = workspace_id
         if description is not None:
             self.description = description
+        if results_retention_in_days is not None:
+            self.results_retention_in_days = results_retention_in_days
 
     @property
     def name(self):
         """Gets the name of this V1workspaceworkspaceWorkspaceIdUuidWorkspace.  # noqa: E501
 
         Name of the Workspace.  # noqa: E501
 
@@ -171,14 +176,35 @@
 
         :param description: The description of this V1workspaceworkspaceWorkspaceIdUuidWorkspace.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
+    @property
+    def results_retention_in_days(self):
+        """Gets the results_retention_in_days of this V1workspaceworkspaceWorkspaceIdUuidWorkspace.  # noqa: E501
+
+
+        :return: The results_retention_in_days of this V1workspaceworkspaceWorkspaceIdUuidWorkspace.  # noqa: E501
+        :rtype: int
+        """
+        return self._results_retention_in_days
+
+    @results_retention_in_days.setter
+    def results_retention_in_days(self, results_retention_in_days):
+        """Sets the results_retention_in_days of this V1workspaceworkspaceWorkspaceIdUuidWorkspace.
+
+
+        :param results_retention_in_days: The results_retention_in_days of this V1workspaceworkspaceWorkspaceIdUuidWorkspace.  # noqa: E501
+        :type: int
+        """
+
+        self._results_retention_in_days = results_retention_in_days
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,91 +11,92 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WorkspaceIdUuidUsersBody(object):
+class WorkspaceIdUuidTagsBody(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'workspace_id': 'object',
-        'users': 'list[RimeUserWithRole]'
+        'name': 'str'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
-        'users': 'users'
+        'name': 'name'
     }
 
-    def __init__(self, workspace_id=None, users=None):  # noqa: E501
-        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, name=None):  # noqa: E501
+        """WorkspaceIdUuidTagsBody - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
-        self._users = None
+        self._name = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
-        if users is not None:
-            self.users = users
+        self.name = name
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        """Gets the workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :return: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
         :rtype: object
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
+        """Sets the workspace_id of this WorkspaceIdUuidTagsBody.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
+        :param workspace_id: The workspace_id of this WorkspaceIdUuidTagsBody.  # noqa: E501
         :type: object
         """
 
         self._workspace_id = workspace_id
 
     @property
-    def users(self):
-        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+    def name(self):
+        """Gets the name of this WorkspaceIdUuidTagsBody.  # noqa: E501
 
-        List of Users to add to the Workspace.  # noqa: E501
+        Name of the tag.  # noqa: E501
 
-        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :rtype: list[RimeUserWithRole]
+        :return: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :rtype: str
         """
-        return self._users
+        return self._name
 
-    @users.setter
-    def users(self, users):
-        """Sets the users of this WorkspaceIdUuidUsersBody.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this WorkspaceIdUuidTagsBody.
 
-        List of Users to add to the Workspace.  # noqa: E501
+        Name of the tag.  # noqa: E501
 
-        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :type: list[RimeUserWithRole]
+        :param name: The name of this WorkspaceIdUuidTagsBody.  # noqa: E501
+        :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._users = users
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +111,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkspaceIdUuidUsersBody, dict):
+        if issubclass(WorkspaceIdUuidTagsBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +127,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkspaceIdUuidUsersBody):
+        if not isinstance(other, WorkspaceIdUuidTagsBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/test_batch.py` & `rime_sdk-2.0.0rc8/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk/test_run.py` & `rime_sdk-2.0.0rc8/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc7/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.0.0rc8/rime_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.0.0rc7
+Version: 2.0.0rc8
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.0.0rc7/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.0.0rc8/rime_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 rime_sdk/swagger/__init__.py
 rime_sdk/swagger/swagger_client/__init__.py
 rime_sdk/swagger/swagger_client/api_client.py
 rime_sdk/swagger/swagger_client/configuration.py
 rime_sdk/swagger/swagger_client/rest.py
 rime_sdk/swagger/swagger_client/api/__init__.py
 rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+rime_sdk/swagger/swagger_client/api/config_validator_api.py
 rime_sdk/swagger/swagger_client/api/data_collector_api.py
 rime_sdk/swagger/swagger_client/api/detection_api.py
 rime_sdk/swagger/swagger_client/api/feature_flag_api.py
 rime_sdk/swagger/swagger_client/api/file_scanning_api.py
 rime_sdk/swagger/swagger_client/api/file_upload_api.py
 rime_sdk/swagger/swagger_client/api/firewall_service_api.py
 rime_sdk/swagger/swagger_client/api/image_registry_api.py
@@ -62,14 +63,15 @@
 rime_sdk/swagger/swagger_client/api/rime_info_api.py
 rime_sdk/swagger/swagger_client/api/user_api.py
 rime_sdk/swagger/swagger_client/api/workspace_service_api.py
 rime_sdk/swagger/swagger_client/models/__init__.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
 rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
 rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
 rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
 rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
@@ -91,14 +93,15 @@
 rime_sdk/swagger/swagger_client/models/detection_event_type.py
 rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
 rime_sdk/swagger/swagger_client/models/detection_resolution.py
 rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
 rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
 rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
 rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
 rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
 rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
 rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
 rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
 rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
@@ -203,15 +206,14 @@
 rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
 rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/rime_actor_role.py
 rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_agent.py
 rime_sdk/swagger/swagger_client/models/rime_agent_status.py
 rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
-rime_sdk/swagger/swagger_client/models/rime_archived_job_logs.py
 rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
 rime_sdk/swagger/swagger_client/models/rime_category_metric.py
 rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
 rime_sdk/swagger/swagger_client/models/rime_config_type.py
 rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
 rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
@@ -223,14 +225,15 @@
 rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
@@ -362,14 +365,15 @@
 rime_sdk/swagger/swagger_client/models/rime_test_metric.py
 rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
 rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
 rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
 rime_sdk/swagger/swagger_client/models/rime_test_type.py
 rime_sdk/swagger/swagger_client/models/rime_time_interval.py
 rime_sdk/swagger/swagger_client/models/rime_token_type.py
+rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
 rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
 rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
@@ -395,19 +399,21 @@
 rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
 rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
 rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
 rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
 rime_sdk/swagger/swagger_client/models/schemanotification_config.py
 rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
 rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
 rime_sdk/swagger/swagger_client/models/statedb_job_status.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
 rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+rime_sdk/swagger/swagger_client/models/tags_name_body.py
 rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
 rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
 rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
 rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
 rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
 rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
 rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
@@ -419,15 +425,14 @@
 rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
 rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
 rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
 rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
 rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
 rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
 rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
-rime_sdk/swagger/swagger_client/models/testrun_test_category.py
 rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
 rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
 rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
 rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
@@ -458,9 +463,10 @@
 rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
 rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
 rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
 rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
 rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
 rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
 rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
```

### Comparing `rime_sdk-2.0.0rc7/setup.py` & `rime_sdk-2.0.0rc8/setup.py`

 * *Files identical despite different names*

