# Comparing `tmp/rime_sdk-2.0.0rc8.tar.gz` & `tmp/rime_sdk-2.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.0.0rc8.tar", last modified: Mon Apr 24 20:27:54 2023, max compression
+gzip compressed data, was "rime_sdk-2.1.0rc0.tar", last modified: Sat Apr 29 15:16:57 2023, max compression
```

## Comparing `rime_sdk-2.0.0rc8.tar` & `rime_sdk-2.1.0rc0.tar`

### file list

```diff
@@ -1,483 +1,477 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.191983 rime_sdk-2.0.0rc8/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58976 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.191983 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    22506 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.195983 rime_sdk-2.0.0rc8/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16763 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    58724 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    24169 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.195983 rime_sdk-2.0.0rc8/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.195983 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    45876 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.199983 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30381 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26951 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54931 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60397 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    43937 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     9145 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
--rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/tags_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20220 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-24 20:27:50.000000 rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 20:27:54.191983 rime_sdk-2.0.0rc8/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31775 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 20:27:54.000000 rime_sdk-2.0.0rc8/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 20:27:54.255986 rime_sdk-2.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-24 20:27:07.000000 rime_sdk-2.0.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.627429 rime_sdk-2.1.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-29 15:16:57.627429 rime_sdk-2.1.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.563426 rime_sdk-2.1.0rc0/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59948 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.563426 rime_sdk-2.1.0rc0/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24290 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.567426 rime_sdk-2.1.0rc0/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17930 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59324 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24987 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.567426 rime_sdk-2.1.0rc0/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.567426 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    45262 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.571426 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30381 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21473 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24481 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26842 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21593 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14291 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29422 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55776 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57282 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54931 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60397 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.627429 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    43323 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13463 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16223 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9945 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13574 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17717 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6639 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9196 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4926 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5817 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/tags_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12899 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11706 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7807 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4359 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-04-29 15:16:52.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-04-29 15:16:53.000000 rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14716 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:16:57.563426 rime_sdk-2.1.0rc0/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-29 15:16:57.000000 rime_sdk-2.1.0rc0/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    31362 2023-04-29 15:16:57.000000 rime_sdk-2.1.0rc0/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:16:57.000000 rime_sdk-2.1.0rc0/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 15:16:57.000000 rime_sdk-2.1.0rc0/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-29 15:16:57.000000 rime_sdk-2.1.0rc0/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 15:16:57.000000 rime_sdk-2.1.0rc0/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:16:57.627429 rime_sdk-2.1.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-29 15:16:10.000000 rime_sdk-2.1.0rc0/setup.py
```

### Comparing `rime_sdk-2.0.0rc8/LICENSE` & `rime_sdk-2.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/PKG-INFO` & `rime_sdk-2.1.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.0.0rc8
+Version: 2.1.0rc0
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.0.0rc8/README.md` & `rime_sdk-2.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/__init__.py` & `rime_sdk-2.1.0rc0/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/client.py` & `rime_sdk-2.1.0rc0/rime_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,15 @@
                 # if grace period has ended throw an error
                 raise ValueError(message)
             else:
                 print(message)
         elif limit_status == RimeLimitStatusStatus.OK:
             pass
         else:
-            raise ValueError("Unexpected status value.")
+            raise ValueError(f"Unexpected status value: '{limit_status}'")
 
     def _check_stress_test_limit(self) -> None:
         """Check if creating another Stress Test would be within license limits.
 
         Raises:
             ValueError
                 This error is generated when a Stress Test cannot be created as
@@ -241,15 +241,15 @@
                 "You have reached the limit of Stress Test runs."
                 " Contact the Robust Intelligence team to"
                 " upgrade your license."
             )
         elif limit_status == RimeLimitStatusStatus.OK:
             pass
         else:
-            raise ValueError("Unexpected status value.")
+            raise ValueError(f"Unexpected status value: '{limit_status}'")
 
     def _check_version(self) -> str:
         """Check current RIME version and return client name."""
         api = swagger_client.RIMEInfoApi(self._api_client)
         with RESTErrorHandler():
             rime_info_response = api.r_ime_info_get_rime_info()
         server_version = rime_info_response.cluster_info_version
@@ -312,15 +312,20 @@
 
         Args:
             name: str
                 Name of the new Project.
             description: str
                 Description of the new Project.
             model_task: str
-                Machine Learning task associated with the Project.
+                Machine Learning task associated with the Project. Must be one of
+                "MODEL_TASK_REGRESSION", "MODEL_TASK_BINARY_CLASSIFICATION",
+                "MODEL_TASK_MULTICLASS_CLASSIFICATION",
+                "MODEL_TASK_NAMED_ENTITY_RECOGNITION", "MODEL_TASK_RANKING",
+                "MODEL_TASK_OBJECT_DETECTION", "MODEL_TASK_NATURAL_LANGUAGE_INFERENCE",
+                "MODEL_TASK_FILL_MASK".
             use_case: Optional[str]
                 Description of the use case of the Project.
             ethical_consideration: Optional[str]
                 Description of ethical considerations for this Project.
             profiling_config: Optional[dict]
                 Configuration for the data and model profiling across all test
                 runs.
@@ -917,14 +922,27 @@
                 test_run_config["model_id"] = _get_uuid(test_run_config["model_id"])
         if "run_time_info" in test_run_config:
             if "agent_id" in test_run_config["run_time_info"]:
                 if isinstance(test_run_config["run_time_info"]["agent_id"], str):
                     test_run_config["run_time_info"]["agent_id"] = _get_uuid(
                         test_run_config["run_time_info"]["agent_id"]
                     )
+        if (
+            "test_suite_config" in test_run_config
+            and "custom_tests" in test_run_config["test_suite_config"]
+        ):
+            if not isinstance(
+                test_run_config["test_suite_config"]["custom_tests"], list
+            ):
+                raise ValueError("The custom_tests configuration must be a list")
+            test_run_config["test_suite_config"]["custom_tests"] = [
+                json.dumps(test) if isinstance(test, dict) else test
+                for test in test_run_config["test_suite_config"]["custom_tests"]
+            ]
+
         cv_api = swagger_client.ConfigValidatorApi(self._api_client)
         with RESTErrorHandler():
             validate_body = ConfigvalidatorConfigTypeBody(
                 config_json=json.dumps(test_run_config),
             )
             cv_api.config_validator_validate_test_config(
                 config_type="CONFIG_TYPE_TEST_RUN", body=validate_body
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/data_collector.py` & `rime_sdk-2.1.0rc0/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.1.0rc0/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.1.0rc0/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.1.0rc0/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.1.0rc0/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/detection_event.py` & `rime_sdk-2.1.0rc0/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/firewall.py` & `rime_sdk-2.1.0rc0/rime_sdk/firewall.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Library defining the interface to firewall."""
 from datetime import timedelta
 from typing import Any, Dict, Iterator, List, Optional
 
 import pandas as pd
 
+from rime_sdk.internal.config_parser import (
+    convert_single_data_info_to_swagger,
+    convert_single_pred_info_to_swagger,
+)
 from rime_sdk.internal.constants import (
     MONITOR_TYPE_TO_SWAGGER,
     RISK_CATEGORY_TO_SWAGGER,
 )
 from rime_sdk.internal.decorators import prompt_confirmation
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.swagger_parser import parse_events_to_df
-from rime_sdk.internal.swagger_utils import (
-    get_data_location_swagger,
-    rest_to_timedelta,
-    timedelta_to_rest,
-)
+from rime_sdk.internal.swagger_utils import rest_to_timedelta, timedelta_to_rest
 from rime_sdk.internal.throttle_queue import ThrottleQueue
 from rime_sdk.internal.utils import convert_dict_to_html, make_link
 from rime_sdk.job import ContinuousTestJob
 from rime_sdk.monitor import Monitor
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
@@ -74,31 +74,37 @@
         """Return string representation of the object."""
         return f"Firewall({self._firewall_id})"
 
     def update_firewall(
         self,
         model_id: Optional[str] = None,
         ref_data_id: Optional[str] = None,
-        scheduled_ct_eval_data_location: Optional[Dict] = None,
-        scheduled_ct_eval_prediction_location: Optional[Dict] = None,
+        scheduled_ct_eval_data_integration_id: Optional[str] = None,
+        scheduled_ct_eval_data_info: Optional[dict] = None,
+        scheduled_ct_eval_pred_integration_id: Optional[str] = None,
+        scheduled_ct_eval_pred_info: Optional[dict] = None,
         update_rolling_window: bool = False,
         scheduled_ct_rolling_window_size: Optional[timedelta] = None,
         disable_scheduled_ct: Optional[bool] = False,
     ) -> RimeUpdateFirewallResponse:
         """Update the Firewall with specified model and reference data.
 
         Arguments:
             model_id: Optional[str]
                 The ID of the model to use for the Firewall.
             ref_data_id: Optional[str]
                 The ID of the reference data to use for the Firewall.
-            scheduled_ct_eval_data_location: Optional[Dict]
-                The location of the evaluation data for scheduled CT.
-            scheduled_ct_eval_prediction_location: Optional[Dict]
-                The location of the evaluation predictions for scheduled CT.
+            scheduled_ct_eval_data_integration_id: Optional[str]
+                The integration id of the evaluation data for scheduled CT.
+            scheduled_ct_eval_data_info: Optional[Dict]
+                The data info of the evaluation data for scheduled CT.
+            scheduled_ct_eval_pred_integration_id: Optional[str]
+                The integration id of the evaluation prediction for scheduled CT.
+            scheduled_ct_eval_pred_info: Optional[Dict]
+                The data info of the evaluation prediction for scheduled CT.
             update_rolling_window: bool
                 Specifies whether to update rolling window
             scheduled_ct_rolling_window_size: Optional[timedelta]
                 If `update_rolling_window` is True, the new rolling window size
                 will be set to this value. The rolling window for the firewall
                 is used to determine the reference set for scheduled CT if it is
                 not `None`.
@@ -122,108 +128,132 @@
         api = swagger_client.FirewallServiceApi(self._api_client)
         field_mask_list = []
         if model_id is not None:
             field_mask_list.append("modelId")
         if ref_data_id is not None:
             field_mask_list.append("refDataId")
         scheduled_ct_info = FirewallScheduledCTInfo()
-        if scheduled_ct_eval_data_location is not None:
-            field_mask_list.append("scheduledCtInfo.evalDataLocation")
-            scheduled_ct_info.eval_data_location = get_data_location_swagger(
-                scheduled_ct_eval_data_location
-            )
-        if scheduled_ct_eval_prediction_location is not None:
-            field_mask_list.append("scheduledCtInfo.evalPredLocation")
-            scheduled_ct_info.eval_pred_location = get_data_location_swagger(
-                scheduled_ct_eval_prediction_location
+        if scheduled_ct_eval_data_integration_id is not None:
+            field_mask_list.append("scheduledCtInfo.evalDataIntegrationId")
+            scheduled_ct_info.eval_data_integration_id = RimeUUID(
+                uuid=scheduled_ct_eval_data_integration_id
+            )
+        if scheduled_ct_eval_data_info is not None:
+            field_mask_list.append("scheduledCtInfo.evalDataInfo")
+            scheduled_ct_info.eval_data_info = convert_single_data_info_to_swagger(
+                scheduled_ct_eval_data_info
+            )
+        if scheduled_ct_eval_pred_integration_id is not None:
+            field_mask_list.append("scheduledCtInfo.evalPredIntegrationId")
+            scheduled_ct_info.eval_pred_integration_id = RimeUUID(
+                uuid=scheduled_ct_eval_pred_integration_id
+            )
+        if scheduled_ct_eval_pred_info is not None:
+            field_mask_list.append("scheduledCtInfo.evalPredInfo")
+            scheduled_ct_info.eval_pred_info = convert_single_pred_info_to_swagger(
+                scheduled_ct_eval_pred_info
             )
         if update_rolling_window:
             field_mask_list.append("scheduledCtInfo.rollingWindow")
             rolling_window = (
                 timedelta_to_rest(scheduled_ct_rolling_window_size)
                 if scheduled_ct_rolling_window_size
                 else None
             )
             scheduled_ct_info.rolling_window = rolling_window
         if disable_scheduled_ct:
             field_mask_list.append("scheduledCtInfo.disableScheduledCt")
             scheduled_ct_info.disable_scheduled_ct = disable_scheduled_ct
-        scheduled_ct_info_optional = None
-        if scheduled_ct_info != FirewallScheduledCTInfo():
-            scheduled_ct_info_optional = scheduled_ct_info
         if len(field_mask_list) == 0:
             raise ValueError(
                 "User must provide at least one of model_id, ref_data_id, "
                 "or scheduled CT paramaters."
             )
         req = FirewallFirewallFirewallIdUuidBody(
             firewall_id=RimeUUID(self._firewall_id),
             firewall=V1firewallfirewallFirewallIdUuidFirewall(
                 model_id=RimeUUID(model_id) if model_id is not None else None,
                 ref_data_id=ref_data_id,
-                scheduled_ct_info=scheduled_ct_info_optional,
+                scheduled_ct_info=scheduled_ct_info,
             ),
             mask=",".join(field_mask_list),
         )
         with RESTErrorHandler():
             resp = api.firewall_service_update_firewall(
                 firewall_firewall_id_uuid=self._firewall_id, body=req,
             )
         print(f"Firewall {self._firewall_id} updated successfully.")
         return resp
 
     def activate_ct_scheduling(
         self,
-        data_location: Dict,
-        prediction_location: Dict,
+        data_info: dict,
+        data_integration_id: Optional[str] = None,
+        pred_integration_id: Optional[str] = None,
+        pred_info: Optional[dict] = None,
         rolling_window_size: Optional[timedelta] = None,
     ) -> None:
         """Activate scheduled CT.
 
         Arguments:
-            data_location: Dict
-                The location of the evaluation data for scheduled CT.
-            prediction_location: Dict
-                The location of the evaluation predictions for scheduled CT.
+            data_info: dict
+                The data info of the evaluation data for scheduled CT.
+            data_integration_id: Optional[str]
+                The integration id of the evaluation data for scheduled CT.
+            pred_integration_id: Optional[str]
+                The integration id of the evaluation prediction for scheduled CT.
+            pred_info: Optional[dict]
+                The prediction info of the evaluation data for scheduled CT.
             rolling_window_size: Optional[timedelta]
                 If `rolling_window_size` is not `None`, it is used to determine
                 the reference set for scheduled CT.
         """
         if self.is_scheduled_ct_enabled():
             raise ValueError(
                 "Scheduled CT is already enabled. Please use "
-                "`update_location_info` to update the location info."
+                "`update_scheduled_ct_info` to update the location info."
             )
         self.update_firewall(
-            scheduled_ct_eval_data_location=data_location,
-            scheduled_ct_eval_prediction_location=prediction_location,
+            scheduled_ct_eval_data_integration_id=data_integration_id,
+            scheduled_ct_eval_data_info=data_info,
+            scheduled_ct_eval_pred_integration_id=pred_integration_id,
+            scheduled_ct_eval_pred_info=pred_info,
             update_rolling_window=rolling_window_size is not None,
             scheduled_ct_rolling_window_size=rolling_window_size,
             disable_scheduled_ct=False,
         )
         print(f"Scheduled CT of Firewall {self._firewall_id} activated successfully.")
 
-    def update_location_info(
+    def update_scheduled_ct_info(
         self,
-        data_location: Optional[Dict] = None,
-        prediction_location: Optional[Dict] = None,
+        data_integration_id: Optional[str] = None,
+        data_info: Optional[dict] = None,
+        pred_integration_id: Optional[str] = None,
+        pred_info: Optional[dict] = None,
     ) -> None:
-        """Update location info for scheduled CT.
+        """Update scheduled CT.
 
         Arguments:
-            data_location: Optional[Dict]
-                If `data_location` is not `None`, the Firewall will use this
+            data_integration_id: Optional[str]
+                If `data_integration_id` is not `None`, the Firewall will use it
                 for scheduled CT.
-            prediction_location: Optional[Dict]
-                If `prediction_location` is not `None`, the Firewall will use this
+            data_info: Optional[dict]
+                If `data_info` is not `None`, the Firewall will use it for
+                scheduled CT.
+            pred_integration_id: Optional[str]
+                If `pred_integration_id` is not `None`, the Firewall will use it
                 for scheduled CT.
+            pred_info: Optional[dict]
+                If `pred_info` is not `None`, the Firewall will use it for scheduled CT.
         """
         self.update_firewall(
-            scheduled_ct_eval_data_location=data_location,
-            scheduled_ct_eval_prediction_location=prediction_location,
+            scheduled_ct_eval_data_integration_id=data_integration_id,
+            scheduled_ct_eval_data_info=data_info,
+            scheduled_ct_eval_pred_integration_id=pred_integration_id,
+            scheduled_ct_eval_pred_info=pred_info,
         )
         print(f"Location info of Firewall {self._firewall_id} updated successfully.")
 
     def deactivate_ct_scheduling(self) -> None:
         """Deactivate scheduled CT."""
         if not self.is_scheduled_ct_enabled():
             raise ValueError("Scheduled CT is already disabled.")
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/image_builder.py` & `rime_sdk-2.1.0rc0/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/config_parser.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/constants.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/decorators.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/file_upload.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/internal/utils.py` & `rime_sdk-2.1.0rc0/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/job.py` & `rime_sdk-2.1.0rc0/rime_sdk/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,18 +218,20 @@
                     print(
                         "\nLogs from failed job:\n"
                         + self._format_logs(response.result.chunk)
                     )
                 else:
                     print("No logs found.")
             except ApiException as e:
-                if e.status == HTTPStatus.NOT_FOUND:
-                    print("Unable to retrieve logs for failed job.")
-                else:
+                # if logs cannot be found do not raise an error.
+                # For most deployments logs cannot be read via this api.
+                if e.status != HTTPStatus.NOT_FOUND:
                     raise ValueError(e.reason) from None
+            # check for debug logs in the job
+            print(f"Debug Logs: {self._get_debug_logs(job)}")
 
         job_dict = job.to_dict()
         # Hide job data and archived logs in the return value because it can get ugly.
         for field in fields_to_be_removed:
             if field in job_dict:
                 del job_dict[field]
 
@@ -298,30 +300,49 @@
     def get_job_debug_logs_link(self) -> str:
         """Return a link to the archived logs for a failed Job."""
         api = swagger_client.JobReaderApi(self._api_client)
         with RESTErrorHandler():
             job: RimeJobMetadata = api.job_reader_get_job(
                 job_id=self._job_id, view=RimeJobView.FULL
             ).job
-            if job.status != StatedbJobStatus.FAILED:
-                raise ValueError(
-                    "Debug logs are only available for "
-                    "failed jobs, this job has status {}".format(job.status)
-                )
-            else:
+            return self._get_debug_logs(job)
+
+    def _get_debug_logs(self, job: RimeJobMetadata) -> str:
+        """Pretty print the archived logs for a failed Job."""
+        if job.status != StatedbJobStatus.FAILED:
+            return (
+                f"Debug logs are not available for this job."
+                f"They are only available for failed jobs, "
+                f"this job has status {job.status}"
+            )
+        else:
+            try:
                 expiration_time = datetime.fromtimestamp(
                     job.archived_job_logs.expiration_time.timestamp()
                 )
-                if (
-                    job.archived_job_logs.url.url != ""
-                    and datetime.now() < expiration_time
-                ):
-                    return job.archived_job_logs.url.url
+                if datetime.now() < expiration_time:
+                    return (
+                        f"Debug logs for the job can found in your blob "
+                        f"storage for your job {job.job_id},"
+                        f" at the following url {job.archived_job_logs.url}"
+                    )
                 else:
-                    raise ValueError("Debug logs are not available for this job")
+                    return (
+                        f"Debug logs for the job {job.job_id} maybe "
+                        f"available in your blob storage. RI platform only"
+                        f" has access to a presigned url which has "
+                        f"expired. However, the logs themselves might not "
+                        f"have expired. Please check your configured blob"
+                        f" storage. The logs maybe available in the "
+                        f"bucket configured under the following directory:"
+                        f" /logs/{job.job_id}. The expired url:"
+                        f"{job.archived_job_logs.url}"
+                    )
+            except AttributeError:
+                return "Debug logs are not available for this job"
 
 
 class Job(BaseJob):
     """This object provides an interface for monitoring a Stress Test Job in the RIME backend."""
 
     _job_type = RimeJobType.MODEL_STRESS_TEST
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/monitor.py` & `rime_sdk-2.1.0rc0/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/project.py` & `rime_sdk-2.1.0rc0/rime_sdk/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 from typing import Any, Dict, Iterator, List, NamedTuple, Optional
 
 from google.protobuf.field_mask_pb2 import FieldMask
 from google.protobuf.json_format import MessageToDict
 
 from rime_sdk.data_collector import DataCollector
 from rime_sdk.firewall import Firewall
-from rime_sdk.internal.config_parser import _get_individual_tests_config_swagger
+from rime_sdk.internal.config_parser import (
+    _get_individual_tests_config_swagger,
+    convert_single_data_info_to_swagger,
+    convert_single_pred_info_to_swagger,
+)
 from rime_sdk.internal.decorators import prompt_confirmation
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
-from rime_sdk.internal.swagger_utils import get_data_location_swagger, timedelta_to_rest
+from rime_sdk.internal.swagger_utils import parse_str_to_uuid, timedelta_to_rest
 from rime_sdk.internal.utils import (
     convert_dict_to_html,
     get_swagger_field_mask,
     make_link,
 )
 from rime_sdk.job import Job
 from rime_sdk.registry import Registry
@@ -326,34 +330,40 @@
                 break
 
     def create_firewall(
         self,
         model_id: str,
         ref_data_id: str,
         bin_size: timedelta,
-        scheduled_ct_eval_data_location: Optional[Dict] = None,
-        scheduled_ct_eval_prediction_location: Optional[Dict] = None,
+        scheduled_ct_eval_data_integration_id: Optional[str] = None,
+        scheduled_ct_eval_data_info: Optional[dict] = None,
+        scheduled_ct_eval_pred_integration_id: Optional[str] = None,
+        scheduled_ct_eval_pred_info: Optional[dict] = None,
         scheduled_ct_rolling_window_size: Optional[timedelta] = None,
     ) -> Firewall:
         """Create a Firewall in the current Project.
 
         Args:
             model_id: str
                 The model ID that this Firewall is testing. Model IDs are created
                 by the Registry.
             ref_data_id: str
                 The ID of the reference dataset that this Firewall compares
                 against during testing. Dataset IDs are created by the Registry.
             bin_size: timedelta
                 The length of each time bin to test over as a `timedelta` object.
                 Must have a minimum value of 1 hour.
-            scheduled_ct_eval_data_location: Optional[Dict]
-                The location of the dataset to be used for Scheduled CT evaluation.
-            scheduled_ct_eval_prediction_location: Optional[Dict]
-                The location of the predictions to be used for Scheduled CT evaluation.
+            scheduled_ct_eval_data_integration_id: Optional[str]
+                The integration ID will be used to fetch eval data.
+            scheduled_ct_eval_data_info: Optional[dict]
+                The data info needed to fetch eval data.
+            scheduled_ct_eval_pred_integration_id: Optional[str]
+                The integration ID will be used to fetch eval predictions.
+            scheduled_ct_eval_pred_info: Optional[dict]
+                The predcition info needed to fetch eval predictions.
             scheduled_ct_rolling_window_size: Optional[timedelta]
                 The size of the rolling window to be used for Scheduled CT evaluation.
 
         Returns:
             Firewall:
                 A ``Firewall`` object that is used to monitor the model.
 
@@ -373,45 +383,39 @@
         api = swagger_client.FirewallServiceApi(self._api_client)
         req = RimeCreateFirewallRequest(
             project_id=RimeUUID(uuid=self._project_id),
             model_id=RimeUUID(uuid=model_id),
             ref_data_id=ref_data_id,
             bin_size=timedelta_to_rest(bin_size),
         )
-        if (
-            scheduled_ct_eval_data_location is not None
-            or scheduled_ct_eval_prediction_location is not None
-        ):
-            if (
-                scheduled_ct_eval_data_location is None
-                or scheduled_ct_eval_prediction_location is None
-            ):
-                raise ValueError(
-                    "Data and prediction locations must both be provided for "
-                    "scheduled CT."
-                )
-            rolling_window = (
-                timedelta_to_rest(scheduled_ct_rolling_window_size)
-                if scheduled_ct_rolling_window_size is not None
+        rolling_window = (
+            timedelta_to_rest(scheduled_ct_rolling_window_size)
+            if scheduled_ct_rolling_window_size is not None
+            else None
+        )
+        if scheduled_ct_eval_data_info is not None:
+            eval_pred_info = (
+                convert_single_pred_info_to_swagger(scheduled_ct_eval_pred_info)
+                if scheduled_ct_eval_pred_info is not None
                 else None
             )
             req.scheduled_ct_parameters = CreateFirewallRequestScheduledCTParameters(
-                eval_data_location=get_data_location_swagger(
-                    scheduled_ct_eval_data_location
+                eval_data_integration_id=parse_str_to_uuid(
+                    scheduled_ct_eval_data_integration_id
                 ),
-                eval_pred_location=get_data_location_swagger(
-                    scheduled_ct_eval_prediction_location
+                eval_data_info=convert_single_data_info_to_swagger(
+                    scheduled_ct_eval_data_info,
                 ),
+                eval_pred_integration_id=parse_str_to_uuid(
+                    scheduled_ct_eval_pred_integration_id
+                ),
+                eval_pred_info=eval_pred_info,
                 rolling_window=rolling_window,
             )
-        elif scheduled_ct_rolling_window_size is not None:
-            raise ValueError(
-                "Scheduled CT rolling window size may only be initialized with "
-                "scheduled CT."
-            )
+
         with RESTErrorHandler():
             resp = api.firewall_service_create_firewall(body=req)
         return Firewall(self._api_client, resp.firewall_id.uuid)
 
     def _get_firewall_ids(self) -> List[RimeUUID]:
         api = swagger_client.ProjectServiceApi(self._api_client)
         with RESTErrorHandler():
@@ -787,14 +791,15 @@
     def register_dataset(
         self,
         name: str,
         data_config: dict,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
+        ct_info: Optional[dict] = None,
     ) -> str:
         """Register a new dataset in this Project.
 
         Args:
             name: str
                 The chosen name of the dataset.
             data_config: dict
@@ -803,14 +808,18 @@
                 of the `data_info` field in the `RegisterDataset` request.
             integration_id: Optional[str] = None,
                 Provide the integration ID for datasets that require an integration.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
+            ct_info: Optional[dict] = None,
+                An optional dictionary that contains the CT info.
+                The CT info must match the API specification of the `ct_info`
+                field in the `RegisterDataset` request.
 
         Returns:
             str:
                 The ID of the newly registered dataset.
 
         Raises:
             ValueError
@@ -832,23 +841,25 @@
         return self._registry.register_dataset(
             self.project_id,
             name,
             data_config,
             integration_id=integration_id,
             tags=tags,
             metadata=metadata,
+            ct_info=ct_info,
         )
 
     def register_dataset_from_file(
         self,
         name: str,
         remote_path: str,
         data_params: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
+        ct_info: Optional[dict] = None,
     ) -> str:
         """Register a new dataset in this Project.
 
         Args:
             name: str
                 The chosen name of the dataset.
             remote_path: str
@@ -870,15 +881,20 @@
         """
         data_config = {
             "connection_info": {"data_file": {"path": remote_path}},
         }
         if data_params is not None:
             data_config["data_params"] = data_params
         return self._registry.register_dataset(
-            self.project_id, name, data_config, tags=tags, metadata=metadata
+            self.project_id,
+            name,
+            data_config,
+            tags=tags,
+            metadata=metadata,
+            ct_info=ct_info,
         )
 
     def register_model(
         self,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/registry.py` & `rime_sdk-2.1.0rc0/rime_sdk/registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,21 @@
 
 from rime_sdk.internal.config_parser import (
     convert_model_info_to_swagger,
     convert_single_data_info_to_swagger,
     convert_single_pred_info_to_swagger,
 )
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
+from rime_sdk.internal.swagger_utils import serialize_datetime_to_proto_timestamp
 from rime_sdk.swagger import swagger_client
-from rime_sdk.swagger.swagger_client import ApiClient
+from rime_sdk.swagger.swagger_client import (
+    ApiClient,
+    DatasetCTDatasetType,
+    DatasetCTInfo,
+)
 from rime_sdk.swagger.swagger_client.models import (
     DatasetIdPredictionBody,
     ProjectIdUuidDatasetBody,
     ProjectIdUuidModelBody,
     RegistryMetadata,
     RimeGetDatasetResponse,
     RimeGetModelResponse,
@@ -48,14 +53,15 @@
         self,
         project_id: str,
         name: str,
         data_config: dict,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
+        ct_info: Optional[dict] = None,
     ) -> str:
         """Register a new dataset in a Project.
 
         Args:
             project_id: str
                 The ID of the Project in which to register the dataset.
             name: str
@@ -66,14 +72,18 @@
                 of the `data_info` field in the `RegisterDataset` request.
             integration_id: Optional[str] = None,
                 Provide the integration ID for datasets that require an integration.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
+            ct_info: Optional[dict] = None,
+                An optional dictionary that contains the CT info.
+                The CT info must match the API specification of the `ct_info`
+                field in the `RegisterDataset` request.
 
         Returns:
             str:
                 The ID of the newly registered dataset.
 
         Raises:
             ValueError
@@ -102,14 +112,22 @@
             metadata_str = json.dumps(metadata)
         if tags is not None or metadata_str is not None:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
 
         if integration_id is not None:
             req.integration_id = RimeUUID(uuid=integration_id)
 
+        if ct_info is not None:
+            req.ct_info = DatasetCTInfo(
+                firewall_id=RimeUUID(uuid=ct_info["firewall_id"]),
+                start_time=serialize_datetime_to_proto_timestamp(ct_info["start_time"]),
+                end_time=serialize_datetime_to_proto_timestamp(ct_info["end_time"]),
+                ct_dataset_type=DatasetCTDatasetType.USER_SPECIFIED,
+            )
+
         with RESTErrorHandler():
             api = swagger_client.RegistryServiceApi(self._api_client)
             res = api.registry_service_register_dataset(
                 body=req, project_id_uuid=project_id,
             )
 
             res = cast(RimeRegisterDatasetResponse, res)
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 # import models into sdk package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
+from rime_sdk.swagger.swagger_client.models.create_agent_request_azure_config import CreateAgentRequestAzureConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
 from rime_sdk.swagger.swagger_client.models.data_data_stream_id_uuid_body import DataDataStreamIdUuidBody
@@ -76,23 +77,17 @@
 from rime_sdk.swagger.swagger_client.models.featureflags_customer_name_body import FeatureflagsCustomerNameBody
 from rime_sdk.swagger.swagger_client.models.filescanning_file_scan_result import FilescanningFileScanResult
 from rime_sdk.swagger.swagger_client.models.filescanning_huggingface_model_info import FilescanningHuggingfaceModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_model_file_info import FilescanningModelFileInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_pytorch_model_info import FilescanningPytorchModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
-from rime_sdk.swagger.swagger_client.models.firewall_custom_loader_location import FirewallCustomLoaderLocation
-from rime_sdk.swagger.swagger_client.models.firewall_data_collector_location import FirewallDataCollectorLocation
-from rime_sdk.swagger.swagger_client.models.firewall_data_location import FirewallDataLocation
-from rime_sdk.swagger.swagger_client.models.firewall_delta_lake_location import FirewallDeltaLakeLocation
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
-from rime_sdk.swagger.swagger_client.models.firewall_location_args import FirewallLocationArgs
-from rime_sdk.swagger.swagger_client.models.firewall_location_params import FirewallLocationParams
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration import IntegrationIntegration
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
@@ -159,15 +154,15 @@
 from rime_sdk.swagger.swagger_client.models.project_id_uuid_dataset_body import ProjectIdUuidDatasetBody
 from rime_sdk.swagger.swagger_client.models.project_id_uuid_model_body import ProjectIdUuidModelBody
 from rime_sdk.swagger.swagger_client.models.project_list_projects_request_query import ProjectListProjectsRequestQuery
 from rime_sdk.swagger.swagger_client.models.project_list_projects_response import ProjectListProjectsResponse
 from rime_sdk.swagger.swagger_client.models.project_list_users_of_project_response import ProjectListUsersOfProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_owner_details import ProjectOwnerDetails
 from rime_sdk.swagger.swagger_client.models.project_project import ProjectProject
-from rime_sdk.swagger.swagger_client.models.project_project_with_owner_details import ProjectProjectWithOwnerDetails
+from rime_sdk.swagger.swagger_client.models.project_project_with_details import ProjectProjectWithDetails
 from rime_sdk.swagger.swagger_client.models.project_remove_user_from_project_response import ProjectRemoveUserFromProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_project_response import ProjectUpdateProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_user_of_project_response import ProjectUpdateUserOfProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_workspace_roles_for_project_response import ProjectUpdateWorkspaceRolesForProjectResponse
 from rime_sdk.swagger.swagger_client.models.projects_project_id_uuid_body import ProjectsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.protobuf_any import ProtobufAny
 from rime_sdk.swagger.swagger_client.models.protobuf_null_value import ProtobufNullValue
@@ -331,15 +326,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
 from rime_sdk.swagger.swagger_client.models.rime_suggestion import RimeSuggestion
 from rime_sdk.swagger.swagger_client.models.rime_sync_image_tag_response import RimeSyncImageTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_table_column import RimeTableColumn
 from rime_sdk.swagger.swagger_client.models.rime_table_column_type import RimeTableColumnType
 from rime_sdk.swagger.swagger_client.models.rime_tag import RimeTag
-from rime_sdk.swagger.swagger_client.models.rime_termination_reason import RimeTerminationReason
 from rime_sdk.swagger.swagger_client.models.rime_test_case_monitor_info import RimeTestCaseMonitorInfo
 from rime_sdk.swagger.swagger_client.models.rime_test_case_status import RimeTestCaseStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_metric import RimeTestMetric
 from rime_sdk.swagger.swagger_client.models.rime_test_metric_category import RimeTestMetricCategory
 from rime_sdk.swagger.swagger_client.models.rime_test_run_progress import RimeTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_test_task_status import RimeTestTaskStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_type import RimeTestType
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1-beta/jobs/cancel/{jobId}', 'POST',
+            '/v1/jobs/cancel/{jobId}', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='RimeCancelJobResponse',  # noqa: E501
@@ -207,15 +207,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1-beta/jobs/{jobId}', 'GET',
+            '/v1/jobs/{jobId}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='RimeGetJobResponse',  # noqa: E501
@@ -302,15 +302,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1-beta/jobs/{jobId}/project-id', 'GET',
+            '/v1/jobs/{jobId}/project-id', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='RimeGetProjectIDResponse',  # noqa: E501
@@ -397,15 +397,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1-beta/jobs/{jobId}/test-run-id', 'GET',
+            '/v1/jobs/{jobId}/test-run-id', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='RimeGetTestRunIDResponse',  # noqa: E501
@@ -423,15 +423,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
-        :param list[str] first_page_query_selected_statuses: Specifies a set of statuses. The query only returns results with a status in the specified set. Specify no statuses to return all results.   - JOB_STATUS_PENDING: Resources have been created for the job but the job has not started yet.  - JOB_STATUS_FAILED: Blanket status for user or system-related job failure. Check the Termination Reason for details.  - JOB_STATUS_REQUESTED: The job descriptor exists but has no resources allocated. Jobs that remain in this status without moving to the PENDING status are at risk of entering the FAILED status.  - JOB_STATUS_CANCELLED: Job has been cancelled. Cancelled jobs cannot be recovered.
+        :param list[str] first_page_query_selected_statuses: Specifies a set of statuses. The query only returns results with a status in the specified set. Specify no statuses to return all results.   - JOB_STATUS_PENDING: Resources have been created for the job but the job has not started yet.  - JOB_STATUS_FAILED: Blanket status for user or system-related job failure.  - JOB_STATUS_REQUESTED: The job descriptor exists but has no resources allocated. Jobs that remain in this status without moving to the PENDING status are at risk of entering the FAILED status.  - JOB_STATUS_CANCELLED: Job has been cancelled. Cancelled jobs cannot be recovered.
         :param list[str] first_page_query_selected_types: Specifies a set of types. The query only returns jobs with types in the specified set. Specify no types to return all results. Job types not tied to projects will not be returned.
         :param str page_token: The ListJobs query returns a pageToken after the first request.
         :param str page_size: The maximum number of Job objects to return in a single page.
         :param str view: Specifies how much information about each job to retrieve.   - JOB_VIEW_BASIC: Server responses only include basic information about the job, including type, status, and some job data.  - JOB_VIEW_FULL: Server responses include all available information about the job, including progress. Has greater performance requirements than the Basic view.
         :return: RimeListJobsForProjectResponse
                  If the method is called asynchronously,
                  returns the request thread.
@@ -450,15 +450,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project_with_http_info(project_id_uuid, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str project_id_uuid: Unique object ID. (required)
-        :param list[str] first_page_query_selected_statuses: Specifies a set of statuses. The query only returns results with a status in the specified set. Specify no statuses to return all results.   - JOB_STATUS_PENDING: Resources have been created for the job but the job has not started yet.  - JOB_STATUS_FAILED: Blanket status for user or system-related job failure. Check the Termination Reason for details.  - JOB_STATUS_REQUESTED: The job descriptor exists but has no resources allocated. Jobs that remain in this status without moving to the PENDING status are at risk of entering the FAILED status.  - JOB_STATUS_CANCELLED: Job has been cancelled. Cancelled jobs cannot be recovered.
+        :param list[str] first_page_query_selected_statuses: Specifies a set of statuses. The query only returns results with a status in the specified set. Specify no statuses to return all results.   - JOB_STATUS_PENDING: Resources have been created for the job but the job has not started yet.  - JOB_STATUS_FAILED: Blanket status for user or system-related job failure.  - JOB_STATUS_REQUESTED: The job descriptor exists but has no resources allocated. Jobs that remain in this status without moving to the PENDING status are at risk of entering the FAILED status.  - JOB_STATUS_CANCELLED: Job has been cancelled. Cancelled jobs cannot be recovered.
         :param list[str] first_page_query_selected_types: Specifies a set of types. The query only returns jobs with types in the specified set. Specify no types to return all results. Job types not tied to projects will not be returned.
         :param str page_token: The ListJobs query returns a pageToken after the first request.
         :param str page_size: The maximum number of Job objects to return in a single page.
         :param str view: Specifies how much information about each job to retrieve.   - JOB_VIEW_BASIC: Server responses only include basic information about the job, including type, status, and some job data.  - JOB_VIEW_FULL: Server responses include all available information about the job, including progress. Has greater performance requirements than the Basic view.
         :return: RimeListJobsForProjectResponse
                  If the method is called asynchronously,
                  returns the request thread.
@@ -514,15 +514,15 @@
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['rime-api-key']  # noqa: E501
 
         return self.api_client.call_api(
-            '/v1-beta/jobs/project/{projectId.uuid}', 'GET',
+            '/v1/jobs/project/{projectId.uuid}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='RimeListJobsForProjectResponse',  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # import models into model package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
+from rime_sdk.swagger.swagger_client.models.create_agent_request_azure_config import CreateAgentRequestAzureConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
 from rime_sdk.swagger.swagger_client.models.data_data_stream_id_uuid_body import DataDataStreamIdUuidBody
@@ -50,23 +51,17 @@
 from rime_sdk.swagger.swagger_client.models.featureflags_customer_name_body import FeatureflagsCustomerNameBody
 from rime_sdk.swagger.swagger_client.models.filescanning_file_scan_result import FilescanningFileScanResult
 from rime_sdk.swagger.swagger_client.models.filescanning_huggingface_model_info import FilescanningHuggingfaceModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_model_file_info import FilescanningModelFileInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_pytorch_model_info import FilescanningPytorchModelInfo
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
-from rime_sdk.swagger.swagger_client.models.firewall_custom_loader_location import FirewallCustomLoaderLocation
-from rime_sdk.swagger.swagger_client.models.firewall_data_collector_location import FirewallDataCollectorLocation
-from rime_sdk.swagger.swagger_client.models.firewall_data_location import FirewallDataLocation
-from rime_sdk.swagger.swagger_client.models.firewall_delta_lake_location import FirewallDeltaLakeLocation
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
-from rime_sdk.swagger.swagger_client.models.firewall_location_args import FirewallLocationArgs
-from rime_sdk.swagger.swagger_client.models.firewall_location_params import FirewallLocationParams
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration import IntegrationIntegration
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
@@ -133,15 +128,15 @@
 from rime_sdk.swagger.swagger_client.models.project_id_uuid_dataset_body import ProjectIdUuidDatasetBody
 from rime_sdk.swagger.swagger_client.models.project_id_uuid_model_body import ProjectIdUuidModelBody
 from rime_sdk.swagger.swagger_client.models.project_list_projects_request_query import ProjectListProjectsRequestQuery
 from rime_sdk.swagger.swagger_client.models.project_list_projects_response import ProjectListProjectsResponse
 from rime_sdk.swagger.swagger_client.models.project_list_users_of_project_response import ProjectListUsersOfProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_owner_details import ProjectOwnerDetails
 from rime_sdk.swagger.swagger_client.models.project_project import ProjectProject
-from rime_sdk.swagger.swagger_client.models.project_project_with_owner_details import ProjectProjectWithOwnerDetails
+from rime_sdk.swagger.swagger_client.models.project_project_with_details import ProjectProjectWithDetails
 from rime_sdk.swagger.swagger_client.models.project_remove_user_from_project_response import ProjectRemoveUserFromProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_project_response import ProjectUpdateProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_user_of_project_response import ProjectUpdateUserOfProjectResponse
 from rime_sdk.swagger.swagger_client.models.project_update_workspace_roles_for_project_response import ProjectUpdateWorkspaceRolesForProjectResponse
 from rime_sdk.swagger.swagger_client.models.projects_project_id_uuid_body import ProjectsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.protobuf_any import ProtobufAny
 from rime_sdk.swagger.swagger_client.models.protobuf_null_value import ProtobufNullValue
@@ -305,15 +300,14 @@
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
 from rime_sdk.swagger.swagger_client.models.rime_suggestion import RimeSuggestion
 from rime_sdk.swagger.swagger_client.models.rime_sync_image_tag_response import RimeSyncImageTagResponse
 from rime_sdk.swagger.swagger_client.models.rime_table_column import RimeTableColumn
 from rime_sdk.swagger.swagger_client.models.rime_table_column_type import RimeTableColumnType
 from rime_sdk.swagger.swagger_client.models.rime_tag import RimeTag
-from rime_sdk.swagger.swagger_client.models.rime_termination_reason import RimeTerminationReason
 from rime_sdk.swagger.swagger_client.models.rime_test_case_monitor_info import RimeTestCaseMonitorInfo
 from rime_sdk.swagger.swagger_client.models.rime_test_case_status import RimeTestCaseStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_metric import RimeTestMetric
 from rime_sdk.swagger.swagger_client.models.rime_test_metric_category import RimeTestMetricCategory
 from rime_sdk.swagger.swagger_client.models.rime_test_run_progress import RimeTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_test_task_status import RimeTestTaskStatus
 from rime_sdk.swagger.swagger_client.models.rime_test_type import RimeTestType
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_info_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_info_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,18 +46,16 @@
         self._firewall_id = None
         self._start_time = None
         self._end_time = None
         self._ct_dataset_type = None
         self.discriminator = None
         if firewall_id is not None:
             self.firewall_id = firewall_id
-        if start_time is not None:
-            self.start_time = start_time
-        if end_time is not None:
-            self.end_time = end_time
+        self.start_time = start_time
+        self.end_time = end_time
         if ct_dataset_type is not None:
             self.ct_dataset_type = ct_dataset_type
 
     @property
     def firewall_id(self):
         """Gets the firewall_id of this DatasetCTInfo.  # noqa: E501
 
@@ -94,14 +92,16 @@
         """Sets the start_time of this DatasetCTInfo.
 
         Start and end time are the start and end time of this dataset.  # noqa: E501
 
         :param start_time: The start_time of this DatasetCTInfo.  # noqa: E501
         :type: datetime
         """
+        if start_time is None:
+            raise ValueError("Invalid value for `start_time`, must not be `None`")  # noqa: E501
 
         self._start_time = start_time
 
     @property
     def end_time(self):
         """Gets the end_time of this DatasetCTInfo.  # noqa: E501
 
@@ -115,14 +115,16 @@
     def end_time(self, end_time):
         """Sets the end_time of this DatasetCTInfo.
 
 
         :param end_time: The end_time of this DatasetCTInfo.  # noqa: E501
         :type: datetime
         """
+        if end_time is None:
+            raise ValueError("Invalid value for `end_time`, must not be `None`")  # noqa: E501
 
         self._end_time = end_time
 
     @property
     def ct_dataset_type(self):
         """Gets the ct_dataset_type of this DatasetCTInfo.  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FirewallDataCollectorLocation(object):
+class TestrunDataCollectorInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'data_stream_id': 'dataStreamId'
     }
 
     def __init__(self, data_stream_id=None):  # noqa: E501
-        """FirewallDataCollectorLocation - a model defined in Swagger"""  # noqa: E501
+        """TestrunDataCollectorInfo - a model defined in Swagger"""  # noqa: E501
         self._data_stream_id = None
         self.discriminator = None
         if data_stream_id is not None:
             self.data_stream_id = data_stream_id
 
     @property
     def data_stream_id(self):
-        """Gets the data_stream_id of this FirewallDataCollectorLocation.  # noqa: E501
+        """Gets the data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
 
 
-        :return: The data_stream_id of this FirewallDataCollectorLocation.  # noqa: E501
+        :return: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._data_stream_id
 
     @data_stream_id.setter
     def data_stream_id(self, data_stream_id):
-        """Sets the data_stream_id of this FirewallDataCollectorLocation.
+        """Sets the data_stream_id of this TestrunDataCollectorInfo.
 
 
-        :param data_stream_id: The data_stream_id of this FirewallDataCollectorLocation.  # noqa: E501
+        :param data_stream_id: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
         :type: RimeUUID
         """
 
         self._data_stream_id = data_stream_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FirewallDataCollectorLocation, dict):
+        if issubclass(TestrunDataCollectorInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FirewallDataCollectorLocation):
+        if not isinstance(other, TestrunDataCollectorInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FirewallDeltaLakeLocation(object):
+class TestrunDeltaLakeInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,38 +32,41 @@
     }
 
     attribute_map = {
         'table_name': 'tableName'
     }
 
     def __init__(self, table_name=None):  # noqa: E501
-        """FirewallDeltaLakeLocation - a model defined in Swagger"""  # noqa: E501
+        """TestrunDeltaLakeInfo - a model defined in Swagger"""  # noqa: E501
         self._table_name = None
         self.discriminator = None
-        if table_name is not None:
-            self.table_name = table_name
+        self.table_name = table_name
 
     @property
     def table_name(self):
-        """Gets the table_name of this FirewallDeltaLakeLocation.  # noqa: E501
+        """Gets the table_name of this TestrunDeltaLakeInfo.  # noqa: E501
 
+        The database table name to use.  # noqa: E501
 
-        :return: The table_name of this FirewallDeltaLakeLocation.  # noqa: E501
+        :return: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
         :rtype: str
         """
         return self._table_name
 
     @table_name.setter
     def table_name(self, table_name):
-        """Sets the table_name of this FirewallDeltaLakeLocation.
+        """Sets the table_name of this TestrunDeltaLakeInfo.
 
+        The database table name to use.  # noqa: E501
 
-        :param table_name: The table_name of this FirewallDeltaLakeLocation.  # noqa: E501
+        :param table_name: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
         :type: str
         """
+        if table_name is None:
+            raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
 
         self._table_name = table_name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -80,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FirewallDeltaLakeLocation, dict):
+        if issubclass(TestrunDeltaLakeInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FirewallDeltaLakeLocation):
+        if not isinstance(other, TestrunDeltaLakeInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_location_params.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FirewallLocationParams(object):
+class UsersUserIdUuidBody(object):
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
-        'data_params': 'TestrunDataInfoParams',
-        'pred_params': 'TestrunPredictionParams'
+        'user': 'V1usersuserIdUuidUser',
+        'mask': 'RimeUserWriteMask'
     }
 
     attribute_map = {
-        'data_params': 'dataParams',
-        'pred_params': 'predParams'
+        'user': 'user',
+        'mask': 'mask'
     }
 
-    def __init__(self, data_params=None, pred_params=None):  # noqa: E501
-        """FirewallLocationParams - a model defined in Swagger"""  # noqa: E501
-        self._data_params = None
-        self._pred_params = None
+    def __init__(self, user=None, mask=None):  # noqa: E501
+        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._user = None
+        self._mask = None
         self.discriminator = None
-        if data_params is not None:
-            self.data_params = data_params
-        if pred_params is not None:
-            self.pred_params = pred_params
+        if user is not None:
+            self.user = user
+        if mask is not None:
+            self.mask = mask
 
     @property
-    def data_params(self):
-        """Gets the data_params of this FirewallLocationParams.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
 
 
-        :return: The data_params of this FirewallLocationParams.  # noqa: E501
-        :rtype: TestrunDataInfoParams
+        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: V1usersuserIdUuidUser
         """
-        return self._data_params
+        return self._user
 
-    @data_params.setter
-    def data_params(self, data_params):
-        """Sets the data_params of this FirewallLocationParams.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserIdUuidBody.
 
 
-        :param data_params: The data_params of this FirewallLocationParams.  # noqa: E501
-        :type: TestrunDataInfoParams
+        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
+        :type: V1usersuserIdUuidUser
         """
 
-        self._data_params = data_params
+        self._user = user
 
     @property
-    def pred_params(self):
-        """Gets the pred_params of this FirewallLocationParams.  # noqa: E501
+    def mask(self):
+        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
 
 
-        :return: The pred_params of this FirewallLocationParams.  # noqa: E501
-        :rtype: TestrunPredictionParams
+        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :rtype: RimeUserWriteMask
         """
-        return self._pred_params
+        return self._mask
 
-    @pred_params.setter
-    def pred_params(self, pred_params):
-        """Sets the pred_params of this FirewallLocationParams.
+    @mask.setter
+    def mask(self, mask):
+        """Sets the mask of this UsersUserIdUuidBody.
 
 
-        :param pred_params: The pred_params of this FirewallLocationParams.  # noqa: E501
-        :type: TestrunPredictionParams
+        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
+        :type: RimeUserWriteMask
         """
 
-        self._pred_params = pred_params
+        self._mask = mask
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FirewallLocationParams, dict):
+        if issubclass(UsersUserIdUuidBody, dict):
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
-        if not isinstance(other, FirewallLocationParams):
+        if not isinstance(other, UsersUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,94 +24,146 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'eval_data_location': 'FirewallDataLocation',
-        'eval_pred_location': 'FirewallDataLocation',
+        'eval_data_integration_id': 'RimeUUID',
+        'eval_data_info': 'TestrunSingleDataInfo',
+        'eval_pred_integration_id': 'RimeUUID',
+        'eval_pred_info': 'TestrunPredInfo',
         'rolling_window': 'str',
         'last_ct_scheduled': 'datetime',
         'activated_time': 'datetime',
         'disable_scheduled_ct': 'bool'
     }
 
     attribute_map = {
-        'eval_data_location': 'evalDataLocation',
-        'eval_pred_location': 'evalPredLocation',
+        'eval_data_integration_id': 'evalDataIntegrationId',
+        'eval_data_info': 'evalDataInfo',
+        'eval_pred_integration_id': 'evalPredIntegrationId',
+        'eval_pred_info': 'evalPredInfo',
         'rolling_window': 'rollingWindow',
         'last_ct_scheduled': 'lastCtScheduled',
         'activated_time': 'activatedTime',
         'disable_scheduled_ct': 'disableScheduledCt'
     }
 
-    def __init__(self, eval_data_location=None, eval_pred_location=None, rolling_window=None, last_ct_scheduled=None, activated_time=None, disable_scheduled_ct=None):  # noqa: E501
+    def __init__(self, eval_data_integration_id=None, eval_data_info=None, eval_pred_integration_id=None, eval_pred_info=None, rolling_window=None, last_ct_scheduled=None, activated_time=None, disable_scheduled_ct=None):  # noqa: E501
         """FirewallScheduledCTInfo - a model defined in Swagger"""  # noqa: E501
-        self._eval_data_location = None
-        self._eval_pred_location = None
+        self._eval_data_integration_id = None
+        self._eval_data_info = None
+        self._eval_pred_integration_id = None
+        self._eval_pred_info = None
         self._rolling_window = None
         self._last_ct_scheduled = None
         self._activated_time = None
         self._disable_scheduled_ct = None
         self.discriminator = None
-        if eval_data_location is not None:
-            self.eval_data_location = eval_data_location
-        if eval_pred_location is not None:
-            self.eval_pred_location = eval_pred_location
+        if eval_data_integration_id is not None:
+            self.eval_data_integration_id = eval_data_integration_id
+        if eval_data_info is not None:
+            self.eval_data_info = eval_data_info
+        if eval_pred_integration_id is not None:
+            self.eval_pred_integration_id = eval_pred_integration_id
+        if eval_pred_info is not None:
+            self.eval_pred_info = eval_pred_info
         if rolling_window is not None:
             self.rolling_window = rolling_window
         if last_ct_scheduled is not None:
             self.last_ct_scheduled = last_ct_scheduled
         if activated_time is not None:
             self.activated_time = activated_time
         if disable_scheduled_ct is not None:
             self.disable_scheduled_ct = disable_scheduled_ct
 
     @property
-    def eval_data_location(self):
-        """Gets the eval_data_location of this FirewallScheduledCTInfo.  # noqa: E501
+    def eval_data_integration_id(self):
+        """Gets the eval_data_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
 
 
-        :return: The eval_data_location of this FirewallScheduledCTInfo.  # noqa: E501
-        :rtype: FirewallDataLocation
+        :return: The eval_data_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._eval_data_location
+        return self._eval_data_integration_id
 
-    @eval_data_location.setter
-    def eval_data_location(self, eval_data_location):
-        """Sets the eval_data_location of this FirewallScheduledCTInfo.
+    @eval_data_integration_id.setter
+    def eval_data_integration_id(self, eval_data_integration_id):
+        """Sets the eval_data_integration_id of this FirewallScheduledCTInfo.
 
 
-        :param eval_data_location: The eval_data_location of this FirewallScheduledCTInfo.  # noqa: E501
-        :type: FirewallDataLocation
+        :param eval_data_integration_id: The eval_data_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._eval_data_location = eval_data_location
+        self._eval_data_integration_id = eval_data_integration_id
 
     @property
-    def eval_pred_location(self):
-        """Gets the eval_pred_location of this FirewallScheduledCTInfo.  # noqa: E501
+    def eval_data_info(self):
+        """Gets the eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
 
 
-        :return: The eval_pred_location of this FirewallScheduledCTInfo.  # noqa: E501
-        :rtype: FirewallDataLocation
+        :return: The eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
+        :rtype: TestrunSingleDataInfo
         """
-        return self._eval_pred_location
+        return self._eval_data_info
 
-    @eval_pred_location.setter
-    def eval_pred_location(self, eval_pred_location):
-        """Sets the eval_pred_location of this FirewallScheduledCTInfo.
+    @eval_data_info.setter
+    def eval_data_info(self, eval_data_info):
+        """Sets the eval_data_info of this FirewallScheduledCTInfo.
 
 
-        :param eval_pred_location: The eval_pred_location of this FirewallScheduledCTInfo.  # noqa: E501
-        :type: FirewallDataLocation
+        :param eval_data_info: The eval_data_info of this FirewallScheduledCTInfo.  # noqa: E501
+        :type: TestrunSingleDataInfo
         """
 
-        self._eval_pred_location = eval_pred_location
+        self._eval_data_info = eval_data_info
+
+    @property
+    def eval_pred_integration_id(self):
+        """Gets the eval_pred_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
+
+
+        :return: The eval_pred_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._eval_pred_integration_id
+
+    @eval_pred_integration_id.setter
+    def eval_pred_integration_id(self, eval_pred_integration_id):
+        """Sets the eval_pred_integration_id of this FirewallScheduledCTInfo.
+
+
+        :param eval_pred_integration_id: The eval_pred_integration_id of this FirewallScheduledCTInfo.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._eval_pred_integration_id = eval_pred_integration_id
+
+    @property
+    def eval_pred_info(self):
+        """Gets the eval_pred_info of this FirewallScheduledCTInfo.  # noqa: E501
+
+
+        :return: The eval_pred_info of this FirewallScheduledCTInfo.  # noqa: E501
+        :rtype: TestrunPredInfo
+        """
+        return self._eval_pred_info
+
+    @eval_pred_info.setter
+    def eval_pred_info(self, eval_pred_info):
+        """Sets the eval_pred_info of this FirewallScheduledCTInfo.
+
+
+        :param eval_pred_info: The eval_pred_info of this FirewallScheduledCTInfo.  # noqa: E501
+        :type: TestrunPredInfo
+        """
+
+        self._eval_pred_info = eval_pred_info
 
     @property
     def rolling_window(self):
         """Gets the rolling_window of this FirewallScheduledCTInfo.  # noqa: E501
 
         Providing this value overwrites any existing reference data set.  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     CUSTOM = "INTEGRATION_TYPE_CUSTOM"
     DATABRICKS = "INTEGRATION_TYPE_DATABRICKS"
     AWS_ACCESS_KEY = "INTEGRATION_TYPE_AWS_ACCESS_KEY"
     AWS_ROLE_ARN = "INTEGRATION_TYPE_AWS_ROLE_ARN"
     HUGGINGFACE = "INTEGRATION_TYPE_HUGGINGFACE"
     GCS = "INTEGRATION_TYPE_GCS"
     AZURE_CLIENT_SECRET = "INTEGRATION_TYPE_AZURE_CLIENT_SECRET"
+    AZURE_WORKLOAD_IDENTITY = "INTEGRATION_TYPE_AZURE_WORKLOAD_IDENTITY"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/model_model_path_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/model_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'project': 'ProjectProjectWithOwnerDetails'
+        'project': 'ProjectProjectWithDetails'
     }
 
     attribute_map = {
         'project': 'project'
     }
 
     def __init__(self, project=None):  # noqa: E501
@@ -44,25 +44,25 @@
 
     @property
     def project(self):
         """Gets the project of this ProjectGetProjectResponse.  # noqa: E501
 
 
         :return: The project of this ProjectGetProjectResponse.  # noqa: E501
-        :rtype: ProjectProjectWithOwnerDetails
+        :rtype: ProjectProjectWithDetails
         """
         return self._project
 
     @project.setter
     def project(self, project):
         """Sets the project of this ProjectGetProjectResponse.
 
 
         :param project: The project of this ProjectGetProjectResponse.  # noqa: E501
-        :type: ProjectProjectWithOwnerDetails
+        :type: ProjectProjectWithDetails
         """
 
         self._project = project
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'projects': 'list[ProjectProjectWithOwnerDetails]',
+        'projects': 'list[ProjectProjectWithDetails]',
         'next_page_token': 'str',
         'has_more': 'bool'
     }
 
     attribute_map = {
         'projects': 'projects',
         'next_page_token': 'nextPageToken',
@@ -54,25 +54,25 @@
 
     @property
     def projects(self):
         """Gets the projects of this ProjectListProjectsResponse.  # noqa: E501
 
 
         :return: The projects of this ProjectListProjectsResponse.  # noqa: E501
-        :rtype: list[ProjectProjectWithOwnerDetails]
+        :rtype: list[ProjectProjectWithDetails]
         """
         return self._projects
 
     @projects.setter
     def projects(self, projects):
         """Sets the projects of this ProjectListProjectsResponse.
 
 
         :param projects: The projects of this ProjectListProjectsResponse.  # noqa: E501
-        :type: list[ProjectProjectWithOwnerDetails]
+        :type: list[ProjectProjectWithDetails]
         """
 
         self._projects = projects
 
     @property
     def next_page_token(self):
         """Gets the next_page_token of this ProjectListProjectsResponse.  # noqa: E501
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,88 +11,114 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProjectProjectWithOwnerDetails(object):
+class ProjectProjectWithDetails(object):
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
         'project': 'ProjectProject',
-        'owner_details': 'ProjectOwnerDetails'
+        'owner_details': 'ProjectOwnerDetails',
+        'last_updated_time': 'datetime'
     }
 
     attribute_map = {
         'project': 'project',
-        'owner_details': 'ownerDetails'
+        'owner_details': 'ownerDetails',
+        'last_updated_time': 'lastUpdatedTime'
     }
 
-    def __init__(self, project=None, owner_details=None):  # noqa: E501
-        """ProjectProjectWithOwnerDetails - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, project=None, owner_details=None, last_updated_time=None):  # noqa: E501
+        """ProjectProjectWithDetails - a model defined in Swagger"""  # noqa: E501
         self._project = None
         self._owner_details = None
+        self._last_updated_time = None
         self.discriminator = None
         if project is not None:
             self.project = project
         if owner_details is not None:
             self.owner_details = owner_details
+        if last_updated_time is not None:
+            self.last_updated_time = last_updated_time
 
     @property
     def project(self):
-        """Gets the project of this ProjectProjectWithOwnerDetails.  # noqa: E501
+        """Gets the project of this ProjectProjectWithDetails.  # noqa: E501
 
 
-        :return: The project of this ProjectProjectWithOwnerDetails.  # noqa: E501
+        :return: The project of this ProjectProjectWithDetails.  # noqa: E501
         :rtype: ProjectProject
         """
         return self._project
 
     @project.setter
     def project(self, project):
-        """Sets the project of this ProjectProjectWithOwnerDetails.
+        """Sets the project of this ProjectProjectWithDetails.
 
 
-        :param project: The project of this ProjectProjectWithOwnerDetails.  # noqa: E501
+        :param project: The project of this ProjectProjectWithDetails.  # noqa: E501
         :type: ProjectProject
         """
 
         self._project = project
 
     @property
     def owner_details(self):
-        """Gets the owner_details of this ProjectProjectWithOwnerDetails.  # noqa: E501
+        """Gets the owner_details of this ProjectProjectWithDetails.  # noqa: E501
 
 
-        :return: The owner_details of this ProjectProjectWithOwnerDetails.  # noqa: E501
+        :return: The owner_details of this ProjectProjectWithDetails.  # noqa: E501
         :rtype: ProjectOwnerDetails
         """
         return self._owner_details
 
     @owner_details.setter
     def owner_details(self, owner_details):
-        """Sets the owner_details of this ProjectProjectWithOwnerDetails.
+        """Sets the owner_details of this ProjectProjectWithDetails.
 
 
-        :param owner_details: The owner_details of this ProjectProjectWithOwnerDetails.  # noqa: E501
+        :param owner_details: The owner_details of this ProjectProjectWithDetails.  # noqa: E501
         :type: ProjectOwnerDetails
         """
 
         self._owner_details = owner_details
 
+    @property
+    def last_updated_time(self):
+        """Gets the last_updated_time of this ProjectProjectWithDetails.  # noqa: E501
+
+
+        :return: The last_updated_time of this ProjectProjectWithDetails.  # noqa: E501
+        :rtype: datetime
+        """
+        return self._last_updated_time
+
+    @last_updated_time.setter
+    def last_updated_time(self, last_updated_time):
+        """Sets the last_updated_time of this ProjectProjectWithDetails.
+
+
+        :param last_updated_time: The last_updated_time of this ProjectProjectWithDetails.  # noqa: E501
+        :type: datetime
+        """
+
+        self._last_updated_time = last_updated_time
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -106,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProjectProjectWithOwnerDetails, dict):
+        if issubclass(ProjectProjectWithDetails, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProjectProjectWithOwnerDetails):
+        if not isinstance(other, ProjectProjectWithDetails):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,39 +27,44 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'name': 'str',
         'local_config': 'CreateAgentRequestLocalConfig',
         'aws_config': 'CreateAgentRequestAWSConfig',
-        'gcp_config': 'CreateAgentRequestGCPConfig'
+        'gcp_config': 'CreateAgentRequestGCPConfig',
+        'azure_config': 'CreateAgentRequestAzureConfig'
     }
 
     attribute_map = {
         'name': 'name',
         'local_config': 'localConfig',
         'aws_config': 'awsConfig',
-        'gcp_config': 'gcpConfig'
+        'gcp_config': 'gcpConfig',
+        'azure_config': 'azureConfig'
     }
 
-    def __init__(self, name=None, local_config=None, aws_config=None, gcp_config=None):  # noqa: E501
+    def __init__(self, name=None, local_config=None, aws_config=None, gcp_config=None, azure_config=None):  # noqa: E501
         """RimeCreateAgentRequest - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._local_config = None
         self._aws_config = None
         self._gcp_config = None
+        self._azure_config = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if local_config is not None:
             self.local_config = local_config
         if aws_config is not None:
             self.aws_config = aws_config
         if gcp_config is not None:
             self.gcp_config = gcp_config
+        if azure_config is not None:
+            self.azure_config = azure_config
 
     @property
     def name(self):
         """Gets the name of this RimeCreateAgentRequest.  # noqa: E501
 
         Agent name given by the user.  # noqa: E501
 
@@ -139,14 +144,35 @@
 
         :param gcp_config: The gcp_config of this RimeCreateAgentRequest.  # noqa: E501
         :type: CreateAgentRequestGCPConfig
         """
 
         self._gcp_config = gcp_config
 
+    @property
+    def azure_config(self):
+        """Gets the azure_config of this RimeCreateAgentRequest.  # noqa: E501
+
+
+        :return: The azure_config of this RimeCreateAgentRequest.  # noqa: E501
+        :rtype: CreateAgentRequestAzureConfig
+        """
+        return self._azure_config
+
+    @azure_config.setter
+    def azure_config(self, azure_config):
+        """Sets the azure_config of this RimeCreateAgentRequest.
+
+
+        :param azure_config: The azure_config of this RimeCreateAgentRequest.  # noqa: E501
+        :type: CreateAgentRequestAzureConfig
+        """
+
+        self._azure_config = azure_config
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,15 +25,14 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'job_id': 'str',
-        'termination_reason': 'RimeTerminationReason',
         'job_type': 'RimeJobType',
         'status': 'StatedbJobStatus',
         'start_time': 'datetime',
         'creation_time': 'datetime',
         'completion_time': 'datetime',
         'running_time_secs': 'float',
         'job_data': 'RimeJobData',
@@ -42,33 +41,31 @@
         'agent_id': 'RimeUUID',
         'archived_job_logs': 'StatedbArchivedJobLogs',
         'error_msg': 'str'
     }
 
     attribute_map = {
         'job_id': 'jobId',
-        'termination_reason': 'terminationReason',
         'job_type': 'jobType',
         'status': 'status',
         'start_time': 'startTime',
         'creation_time': 'creationTime',
         'completion_time': 'completionTime',
         'running_time_secs': 'runningTimeSecs',
         'job_data': 'jobData',
         'job_progress_str': 'jobProgressStr',
         'cancellation_requested': 'cancellationRequested',
         'agent_id': 'agentId',
         'archived_job_logs': 'archivedJobLogs',
         'error_msg': 'errorMsg'
     }
 
-    def __init__(self, job_id=None, termination_reason=None, job_type=None, status=None, start_time=None, creation_time=None, completion_time=None, running_time_secs=None, job_data=None, job_progress_str=None, cancellation_requested=None, agent_id=None, archived_job_logs=None, error_msg=None):  # noqa: E501
+    def __init__(self, job_id=None, job_type=None, status=None, start_time=None, creation_time=None, completion_time=None, running_time_secs=None, job_data=None, job_progress_str=None, cancellation_requested=None, agent_id=None, archived_job_logs=None, error_msg=None):  # noqa: E501
         """RimeJobMetadata - a model defined in Swagger"""  # noqa: E501
         self._job_id = None
-        self._termination_reason = None
         self._job_type = None
         self._status = None
         self._start_time = None
         self._creation_time = None
         self._completion_time = None
         self._running_time_secs = None
         self._job_data = None
@@ -76,16 +73,14 @@
         self._cancellation_requested = None
         self._agent_id = None
         self._archived_job_logs = None
         self._error_msg = None
         self.discriminator = None
         if job_id is not None:
             self.job_id = job_id
-        if termination_reason is not None:
-            self.termination_reason = termination_reason
         if job_type is not None:
             self.job_type = job_type
         if status is not None:
             self.status = status
         if start_time is not None:
             self.start_time = start_time
         if creation_time is not None:
@@ -127,35 +122,14 @@
         :param job_id: The job_id of this RimeJobMetadata.  # noqa: E501
         :type: str
         """
 
         self._job_id = job_id
 
     @property
-    def termination_reason(self):
-        """Gets the termination_reason of this RimeJobMetadata.  # noqa: E501
-
-
-        :return: The termination_reason of this RimeJobMetadata.  # noqa: E501
-        :rtype: RimeTerminationReason
-        """
-        return self._termination_reason
-
-    @termination_reason.setter
-    def termination_reason(self, termination_reason):
-        """Sets the termination_reason of this RimeJobMetadata.
-
-
-        :param termination_reason: The termination_reason of this RimeJobMetadata.  # noqa: E501
-        :type: RimeTerminationReason
-        """
-
-        self._termination_reason = termination_reason
-
-    @property
     def job_type(self):
         """Gets the job_type of this RimeJobMetadata.  # noqa: E501
 
 
         :return: The job_type of this RimeJobMetadata.  # noqa: E501
         :rtype: RimeJobType
         """
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_termination_reason.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,44 +11,43 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTerminationReason(object):
+class RiskscoreRiskCategoryType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "TERMINATION_REASON_UNSPECIFIED"
-    NOT_TERMINATED = "TERMINATION_REASON_NOT_TERMINATED"
-    OOMKILLED = "TERMINATION_REASON_OOMKILLED"
-    COMPLETED = "TERMINATION_REASON_COMPLETED"
-    GENERIC_ERROR = "TERMINATION_REASON_GENERIC_ERROR"
-    INTERNAL_ERROR = "TERMINATION_REASON_INTERNAL_ERROR"
+    UNSPECIFIED = "RISK_CATEGORY_TYPE_UNSPECIFIED"
+    OPERATIONAL_HEALTH = "RISK_CATEGORY_TYPE_OPERATIONAL_HEALTH"
+    BIAS_RISK = "RISK_CATEGORY_TYPE_BIAS_RISK"
+    SECURITY_RISK = "RISK_CATEGORY_TYPE_SECURITY_RISK"
+    CUSTOM = "RISK_CATEGORY_TYPE_CUSTOM"
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
-        """RimeTerminationReason - a model defined in Swagger"""  # noqa: E501
+        """RiskscoreRiskCategoryType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -64,15 +63,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTerminationReason, dict):
+        if issubclass(RiskscoreRiskCategoryType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -80,15 +79,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTerminationReason):
+        if not isinstance(other, RiskscoreRiskCategoryType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     """
     UNSPECIFIED = "TEST_TASK_STATUS_UNSPECIFIED"
     PENDING = "TEST_TASK_STATUS_PENDING"
     RUNNING = "TEST_TASK_STATUS_RUNNING"
     COMPLETED = "TEST_TASK_STATUS_COMPLETED"
     FAILED = "TEST_TASK_STATUS_FAILED"
     CANCELLED = "TEST_TASK_STATUS_CANCELLED"
+    GARBAGE_COLLECTED = "TEST_TASK_STATUS_GARBAGE_COLLECTED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,43 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RiskscoreRiskCategoryType(object):
+class SecurityEventDetailsSecurityEventType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "RISK_CATEGORY_TYPE_UNSPECIFIED"
-    OPERATIONAL_HEALTH = "RISK_CATEGORY_TYPE_OPERATIONAL_HEALTH"
-    BIAS_RISK = "RISK_CATEGORY_TYPE_BIAS_RISK"
-    SECURITY_RISK = "RISK_CATEGORY_TYPE_SECURITY_RISK"
-    CUSTOM = "RISK_CATEGORY_TYPE_CUSTOM"
+    UNSPECIFIED = "SECURITY_EVENT_TYPE_UNSPECIFIED"
+    DATA_POISONING = "SECURITY_EVENT_TYPE_DATA_POISONING"
+    MODEL_EVASION = "SECURITY_EVENT_TYPE_MODEL_EVASION"
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
-        """RiskscoreRiskCategoryType - a model defined in Swagger"""  # noqa: E501
+        """SecurityEventDetailsSecurityEventType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -63,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RiskscoreRiskCategoryType, dict):
+        if issubclass(SecurityEventDetailsSecurityEventType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -79,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RiskscoreRiskCategoryType):
+        if not isinstance(other, SecurityEventDetailsSecurityEventType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,41 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SecurityEventDetailsSecurityEventType(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "SECURITY_EVENT_TYPE_UNSPECIFIED"
-    DATA_POISONING = "SECURITY_EVENT_TYPE_DATA_POISONING"
-    MODEL_EVASION = "SECURITY_EVENT_TYPE_MODEL_EVASION"
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
-        """SecurityEventDetailsSecurityEventType - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SecurityEventDetailsSecurityEventType, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SecurityEventDetailsSecurityEventType):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/tags_name_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/tags_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_collector_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,64 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataCollectorInfo(object):
+class TestrunDataFileInfo(object):
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
-        'data_stream_id': 'RimeUUID'
+        'path': 'str'
     }
 
     attribute_map = {
-        'data_stream_id': 'dataStreamId'
+        'path': 'path'
     }
 
-    def __init__(self, data_stream_id=None):  # noqa: E501
-        """TestrunDataCollectorInfo - a model defined in Swagger"""  # noqa: E501
-        self._data_stream_id = None
+    def __init__(self, path=None):  # noqa: E501
+        """TestrunDataFileInfo - a model defined in Swagger"""  # noqa: E501
+        self._path = None
         self.discriminator = None
-        if data_stream_id is not None:
-            self.data_stream_id = data_stream_id
+        self.path = path
 
     @property
-    def data_stream_id(self):
-        """Gets the data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
+    def path(self):
+        """Gets the path of this TestrunDataFileInfo.  # noqa: E501
 
+        The path to the data file.  # noqa: E501
 
-        :return: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The path of this TestrunDataFileInfo.  # noqa: E501
+        :rtype: str
         """
-        return self._data_stream_id
+        return self._path
 
-    @data_stream_id.setter
-    def data_stream_id(self, data_stream_id):
-        """Sets the data_stream_id of this TestrunDataCollectorInfo.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this TestrunDataFileInfo.
 
+        The path to the data file.  # noqa: E501
 
-        :param data_stream_id: The data_stream_id of this TestrunDataCollectorInfo.  # noqa: E501
-        :type: RimeUUID
+        :param path: The path of this TestrunDataFileInfo.  # noqa: E501
+        :type: str
         """
+        if path is None:
+            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._data_stream_id = data_stream_id
+        self._path = path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataCollectorInfo, dict):
+        if issubclass(TestrunDataFileInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataCollectorInfo):
+        if not isinstance(other, TestrunDataFileInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_file_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,64 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDataFileInfo(object):
+class TestrunresultGetTestRunResponse(object):
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
-        'path': 'str'
+        'test_run': 'TestrunresultTestRunDetail'
     }
 
     attribute_map = {
-        'path': 'path'
+        'test_run': 'testRun'
     }
 
-    def __init__(self, path=None):  # noqa: E501
-        """TestrunDataFileInfo - a model defined in Swagger"""  # noqa: E501
-        self._path = None
+    def __init__(self, test_run=None):  # noqa: E501
+        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_run = None
         self.discriminator = None
-        self.path = path
+        if test_run is not None:
+            self.test_run = test_run
 
     @property
-    def path(self):
-        """Gets the path of this TestrunDataFileInfo.  # noqa: E501
+    def test_run(self):
+        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
 
-        The path to the data file.  # noqa: E501
 
-        :return: The path of this TestrunDataFileInfo.  # noqa: E501
-        :rtype: str
+        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :rtype: TestrunresultTestRunDetail
         """
-        return self._path
+        return self._test_run
 
-    @path.setter
-    def path(self, path):
-        """Sets the path of this TestrunDataFileInfo.
+    @test_run.setter
+    def test_run(self, test_run):
+        """Sets the test_run of this TestrunresultGetTestRunResponse.
 
-        The path to the data file.  # noqa: E501
 
-        :param path: The path of this TestrunDataFileInfo.  # noqa: E501
-        :type: str
+        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :type: TestrunresultTestRunDetail
         """
-        if path is None:
-            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._path = path
+        self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -83,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDataFileInfo, dict):
+        if issubclass(TestrunresultGetTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDataFileInfo):
+        if not isinstance(other, TestrunresultGetTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_info_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,79 +25,71 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'label_col': 'str',
-        'pred_col': 'str',
         'timestamp_col': 'str',
         'class_names': 'list[str]',
         'ranking_info': 'DataInfoParamsRankingInfo',
         'nrows': 'str',
         'nrows_per_time_bin': 'str',
         'sample': 'bool',
         'categorical_features': 'list[str]',
         'protected_features': 'list[str]',
         'features_not_in_model': 'list[str]',
         'text_features': 'list[str]',
         'image_features': 'list[str]',
         'intersections': 'list[DataInfoParamsFeatureIntersection]',
         'loading_kwargs': 'str',
         'feature_type_path': 'str',
-        'pred_path': 'str',
         'image_load_path': 'str'
     }
 
     attribute_map = {
         'label_col': 'labelCol',
-        'pred_col': 'predCol',
         'timestamp_col': 'timestampCol',
         'class_names': 'classNames',
         'ranking_info': 'rankingInfo',
         'nrows': 'nrows',
         'nrows_per_time_bin': 'nrowsPerTimeBin',
         'sample': 'sample',
         'categorical_features': 'categoricalFeatures',
         'protected_features': 'protectedFeatures',
         'features_not_in_model': 'featuresNotInModel',
         'text_features': 'textFeatures',
         'image_features': 'imageFeatures',
         'intersections': 'intersections',
         'loading_kwargs': 'loadingKwargs',
         'feature_type_path': 'featureTypePath',
-        'pred_path': 'predPath',
         'image_load_path': 'imageLoadPath'
     }
 
-    def __init__(self, label_col=None, pred_col=None, timestamp_col=None, class_names=None, ranking_info=None, nrows=None, nrows_per_time_bin=None, sample=None, categorical_features=None, protected_features=None, features_not_in_model=None, text_features=None, image_features=None, intersections=None, loading_kwargs=None, feature_type_path=None, pred_path=None, image_load_path=None):  # noqa: E501
+    def __init__(self, label_col=None, timestamp_col=None, class_names=None, ranking_info=None, nrows=None, nrows_per_time_bin=None, sample=None, categorical_features=None, protected_features=None, features_not_in_model=None, text_features=None, image_features=None, intersections=None, loading_kwargs=None, feature_type_path=None, image_load_path=None):  # noqa: E501
         """TestrunDataInfoParams - a model defined in Swagger"""  # noqa: E501
         self._label_col = None
-        self._pred_col = None
         self._timestamp_col = None
         self._class_names = None
         self._ranking_info = None
         self._nrows = None
         self._nrows_per_time_bin = None
         self._sample = None
         self._categorical_features = None
         self._protected_features = None
         self._features_not_in_model = None
         self._text_features = None
         self._image_features = None
         self._intersections = None
         self._loading_kwargs = None
         self._feature_type_path = None
-        self._pred_path = None
         self._image_load_path = None
         self.discriminator = None
         if label_col is not None:
             self.label_col = label_col
-        if pred_col is not None:
-            self.pred_col = pred_col
         if timestamp_col is not None:
             self.timestamp_col = timestamp_col
         if class_names is not None:
             self.class_names = class_names
         if ranking_info is not None:
             self.ranking_info = ranking_info
         if nrows is not None:
@@ -118,16 +110,14 @@
             self.image_features = image_features
         if intersections is not None:
             self.intersections = intersections
         if loading_kwargs is not None:
             self.loading_kwargs = loading_kwargs
         if feature_type_path is not None:
             self.feature_type_path = feature_type_path
-        if pred_path is not None:
-            self.pred_path = pred_path
         if image_load_path is not None:
             self.image_load_path = image_load_path
 
     @property
     def label_col(self):
         """Gets the label_col of this TestrunDataInfoParams.  # noqa: E501
 
@@ -147,37 +137,14 @@
         :param label_col: The label_col of this TestrunDataInfoParams.  # noqa: E501
         :type: str
         """
 
         self._label_col = label_col
 
     @property
-    def pred_col(self):
-        """Gets the pred_col of this TestrunDataInfoParams.  # noqa: E501
-
-        Column to look at for predictions.  # noqa: E501
-
-        :return: The pred_col of this TestrunDataInfoParams.  # noqa: E501
-        :rtype: str
-        """
-        return self._pred_col
-
-    @pred_col.setter
-    def pred_col(self, pred_col):
-        """Sets the pred_col of this TestrunDataInfoParams.
-
-        Column to look at for predictions.  # noqa: E501
-
-        :param pred_col: The pred_col of this TestrunDataInfoParams.  # noqa: E501
-        :type: str
-        """
-
-        self._pred_col = pred_col
-
-    @property
     def timestamp_col(self):
         """Gets the timestamp_col of this TestrunDataInfoParams.  # noqa: E501
 
         Column to look at for CT timestamp.  # noqa: E501
 
         :return: The timestamp_col of this TestrunDataInfoParams.  # noqa: E501
         :rtype: str
@@ -488,37 +455,14 @@
         :param feature_type_path: The feature_type_path of this TestrunDataInfoParams.  # noqa: E501
         :type: str
         """
 
         self._feature_type_path = feature_type_path
 
     @property
-    def pred_path(self):
-        """Gets the pred_path of this TestrunDataInfoParams.  # noqa: E501
-
-        Path to a CSV file or Parquet file containing the predictions.  # noqa: E501
-
-        :return: The pred_path of this TestrunDataInfoParams.  # noqa: E501
-        :rtype: str
-        """
-        return self._pred_path
-
-    @pred_path.setter
-    def pred_path(self, pred_path):
-        """Sets the pred_path of this TestrunDataInfoParams.
-
-        Path to a CSV file or Parquet file containing the predictions.  # noqa: E501
-
-        :param pred_path: The pred_path of this TestrunDataInfoParams.  # noqa: E501
-        :type: str
-        """
-
-        self._pred_path = pred_path
-
-    @property
     def image_load_path(self):
         """Gets the image_load_path of this TestrunDataInfoParams.  # noqa: E501
 
         Path to a CSV file that contains images to load for image_features.  # noqa: E501
 
         :return: The image_load_path of this TestrunDataInfoParams.  # noqa: E501
         :rtype: str
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_delta_lake_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,64 +11,43 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunDeltaLakeInfo(object):
+class TestrunTestSensitivity(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
+    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
+    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
+    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'table_name': 'str'
     }
 
     attribute_map = {
-        'table_name': 'tableName'
     }
 
-    def __init__(self, table_name=None):  # noqa: E501
-        """TestrunDeltaLakeInfo - a model defined in Swagger"""  # noqa: E501
-        self._table_name = None
+    def __init__(self):  # noqa: E501
+        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        self.table_name = table_name
-
-    @property
-    def table_name(self):
-        """Gets the table_name of this TestrunDeltaLakeInfo.  # noqa: E501
-
-        The database table name to use.  # noqa: E501
-
-        :return: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
-        :rtype: str
-        """
-        return self._table_name
-
-    @table_name.setter
-    def table_name(self, table_name):
-        """Sets the table_name of this TestrunDeltaLakeInfo.
-
-        The database table name to use.  # noqa: E501
-
-        :param table_name: The table_name of this TestrunDeltaLakeInfo.  # noqa: E501
-        :type: str
-        """
-        if table_name is None:
-            raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
-
-        self._table_name = table_name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -83,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunDeltaLakeInfo, dict):
+        if issubclass(TestrunTestSensitivity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunDeltaLakeInfo):
+        if not isinstance(other, TestrunTestSensitivity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_prediction_params.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,27 +24,32 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'pred_col': 'str'
+        'pred_col': 'str',
+        'timestamp_col': 'str'
     }
 
     attribute_map = {
-        'pred_col': 'predCol'
+        'pred_col': 'predCol',
+        'timestamp_col': 'timestampCol'
     }
 
-    def __init__(self, pred_col=None):  # noqa: E501
+    def __init__(self, pred_col=None, timestamp_col=None):  # noqa: E501
         """TestrunPredictionParams - a model defined in Swagger"""  # noqa: E501
         self._pred_col = None
+        self._timestamp_col = None
         self.discriminator = None
         if pred_col is not None:
             self.pred_col = pred_col
+        if timestamp_col is not None:
+            self.timestamp_col = timestamp_col
 
     @property
     def pred_col(self):
         """Gets the pred_col of this TestrunPredictionParams.  # noqa: E501
 
         Column used for predictions.  # noqa: E501
 
@@ -61,14 +66,37 @@
 
         :param pred_col: The pred_col of this TestrunPredictionParams.  # noqa: E501
         :type: str
         """
 
         self._pred_col = pred_col
 
+    @property
+    def timestamp_col(self):
+        """Gets the timestamp_col of this TestrunPredictionParams.  # noqa: E501
+
+        Column used for CT timestamp.  # noqa: E501
+
+        :return: The timestamp_col of this TestrunPredictionParams.  # noqa: E501
+        :rtype: str
+        """
+        return self._timestamp_col
+
+    @timestamp_col.setter
+    def timestamp_col(self, timestamp_col):
+        """Sets the timestamp_col of this TestrunPredictionParams.
+
+        Column used for CT timestamp.  # noqa: E501
+
+        :param timestamp_col: The timestamp_col of this TestrunPredictionParams.  # noqa: E501
+        :type: str
+        """
+
+        self._timestamp_col = timestamp_col
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_single_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,43 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestSensitivity(object):
+class TestrunresultRenameTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
-    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
-    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
-    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'test_run': 'TestrunresultTestRunDetail'
     }
 
     attribute_map = {
+        'test_run': 'testRun'
     }
 
-    def __init__(self):  # noqa: E501
-        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, test_run=None):  # noqa: E501
+        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_run = None
         self.discriminator = None
+        if test_run is not None:
+            self.test_run = test_run
+
+    @property
+    def test_run(self):
+        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+
+
+        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+        :rtype: TestrunresultTestRunDetail
+        """
+        return self._test_run
+
+    @test_run.setter
+    def test_run(self, test_run):
+        """Sets the test_run of this TestrunresultRenameTestRunResponse.
+
+
+        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+        :type: TestrunresultTestRunDetail
+        """
+
+        self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -62,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestSensitivity, dict):
+        if issubclass(TestrunresultRenameTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestSensitivity):
+        if not isinstance(other, TestrunresultRenameTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultRenameTestRunResponse(object):
+class UserPrivateInfo(object):
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
-        'test_run': 'TestrunresultTestRunDetail'
+        'favorite_projects': 'list[UserFavoriteProjects]'
     }
 
     attribute_map = {
-        'test_run': 'testRun'
+        'favorite_projects': 'favoriteProjects'
     }
 
-    def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_run = None
+    def __init__(self, favorite_projects=None):  # noqa: E501
+        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
+        self._favorite_projects = None
         self.discriminator = None
-        if test_run is not None:
-            self.test_run = test_run
+        if favorite_projects is not None:
+            self.favorite_projects = favorite_projects
 
     @property
-    def test_run(self):
-        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+    def favorite_projects(self):
+        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :rtype: TestrunresultTestRunDetail
+        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :rtype: list[UserFavoriteProjects]
         """
-        return self._test_run
+        return self._favorite_projects
 
-    @test_run.setter
-    def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultRenameTestRunResponse.
+    @favorite_projects.setter
+    def favorite_projects(self, favorite_projects):
+        """Sets the favorite_projects of this UserPrivateInfo.
 
 
-        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :type: TestrunresultTestRunDetail
+        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :type: list[UserFavoriteProjects]
         """
 
-        self._test_run = test_run
+        self._favorite_projects = favorite_projects
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultRenameTestRunResponse, dict):
+        if issubclass(UserPrivateInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultRenameTestRunResponse):
+        if not isinstance(other, UserPrivateInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,61 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserPrivateInfo(object):
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
-        'favorite_projects': 'list[UserFavoriteProjects]'
+        'project_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
-        'favorite_projects': 'favoriteProjects'
+        'project_id': 'projectId',
+        'user': 'user'
     }
 
-    def __init__(self, favorite_projects=None):  # noqa: E501
-        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
-        self._favorite_projects = None
+    def __init__(self, project_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+        self._project_id = None
+        self._user = None
         self.discriminator = None
-        if favorite_projects is not None:
-            self.favorite_projects = favorite_projects
+        if project_id is not None:
+            self.project_id = project_id
+        if user is not None:
+            self.user = user
 
     @property
-    def favorite_projects(self):
-        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
+    def project_id(self):
+        """Gets the project_id of this UsersUserUserIdUuidBody.  # noqa: E501
 
+        Uniquely specifies a Project.  # noqa: E501
 
-        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
-        :rtype: list[UserFavoriteProjects]
+        :return: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :rtype: object
         """
-        return self._favorite_projects
+        return self._project_id
 
-    @favorite_projects.setter
-    def favorite_projects(self, favorite_projects):
-        """Sets the favorite_projects of this UserPrivateInfo.
+    @project_id.setter
+    def project_id(self, project_id):
+        """Sets the project_id of this UsersUserUserIdUuidBody.
 
+        Uniquely specifies a Project.  # noqa: E501
 
-        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
-        :type: list[UserFavoriteProjects]
+        :param project_id: The project_id of this UsersUserUserIdUuidBody.  # noqa: E501
+        :type: object
         """
 
-        self._favorite_projects = favorite_projects
+        self._project_id = project_id
+
+    @property
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody.  # noqa: E501
+
+
+        :return: The user of this UsersUserUserIdUuidBody.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        """
+        return self._user
+
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody.
+
+
+        :param user: The user of this UsersUserUserIdUuidBody.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        """
+
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserPrivateInfo, dict):
+        if issubclass(UsersUserUserIdUuidBody, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserPrivateInfo):
+        if not isinstance(other, UsersUserUserIdUuidBody):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,87 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserIdUuidBody(object):
+class UsersUserUserIdUuidBody1(object):
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
-        'user': 'V1usersuserIdUuidUser',
-        'mask': 'RimeUserWriteMask'
+        'workspace_id': 'object',
+        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
     }
 
     attribute_map = {
-        'user': 'user',
-        'mask': 'mask'
+        'workspace_id': 'workspaceId',
+        'user': 'user'
     }
 
-    def __init__(self, user=None, mask=None):  # noqa: E501
-        """UsersUserIdUuidBody - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, user=None):  # noqa: E501
+        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
+        self._workspace_id = None
         self._user = None
-        self._mask = None
         self.discriminator = None
+        if workspace_id is not None:
+            self.workspace_id = workspace_id
         if user is not None:
             self.user = user
-        if mask is not None:
-            self.mask = mask
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserIdUuidBody.  # noqa: E501
+    def workspace_id(self):
+        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: V1usersuserIdUuidUser
+        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: object
         """
-        return self._user
+        return self._workspace_id
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserIdUuidBody.
+    @workspace_id.setter
+    def workspace_id(self, workspace_id):
+        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param user: The user of this UsersUserIdUuidBody.  # noqa: E501
-        :type: V1usersuserIdUuidUser
+        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: object
         """
 
-        self._user = user
+        self._workspace_id = workspace_id
 
     @property
-    def mask(self):
-        """Gets the mask of this UsersUserIdUuidBody.  # noqa: E501
+    def user(self):
+        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
 
 
-        :return: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :rtype: RimeUserWriteMask
+        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
-        return self._mask
+        return self._user
 
-    @mask.setter
-    def mask(self, mask):
-        """Sets the mask of this UsersUserIdUuidBody.
+    @user.setter
+    def user(self, user):
+        """Sets the user of this UsersUserUserIdUuidBody1.
 
 
-        :param mask: The mask of this UsersUserIdUuidBody.  # noqa: E501
-        :type: RimeUserWriteMask
+        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
         """
 
-        self._mask = mask
+        self._user = user
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UsersUserIdUuidBody, dict):
+        if issubclass(UsersUserUserIdUuidBody1, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UsersUserIdUuidBody):
+        if not isinstance(other, UsersUserUserIdUuidBody1):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

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

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,89 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UsersUserUserIdUuidBody1(object):
+class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
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
-        'workspace_id': 'object',
-        'user': 'V1projectsprojectIdUuidroleusersuserUserIdUuidUser'
+        'user_id': 'object',
+        'user_role': 'RimeActorRole'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'user': 'user'
+        'user_id': 'userId',
+        'user_role': 'userRole'
     }
 
-    def __init__(self, workspace_id=None, user=None):  # noqa: E501
-        """UsersUserUserIdUuidBody1 - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._user = None
+    def __init__(self, user_id=None, user_role=None):  # noqa: E501
+        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
+        self._user_id = None
+        self._user_role = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if user is not None:
-            self.user = user
+        if user_id is not None:
+            self.user_id = user_id
+        if user_role is not None:
+            self.user_role = user_role
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def user_id(self):
+        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
         :rtype: object
         """
-        return self._workspace_id
+        return self._user_id
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this UsersUserUserIdUuidBody1.
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
         Unique ID of an object in RIME.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this UsersUserUserIdUuidBody1.  # noqa: E501
+        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
         :type: object
         """
 
-        self._workspace_id = workspace_id
+        self._user_id = user_id
 
     @property
-    def user(self):
-        """Gets the user of this UsersUserUserIdUuidBody1.  # noqa: E501
+    def user_role(self):
+        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
 
-        :return: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :rtype: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._user
+        return self._user_role
 
-    @user.setter
-    def user(self, user):
-        """Sets the user of this UsersUserUserIdUuidBody1.
+    @user_role.setter
+    def user_role(self, user_role):
+        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
 
-        :param user: The user of this UsersUserUserIdUuidBody1.  # noqa: E501
-        :type: V1projectsprojectIdUuidroleusersuserUserIdUuidUser
+        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._user = user
+        self._user_role = user_role
 
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
-        if issubclass(UsersUserUserIdUuidBody1, dict):
+        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
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
-        if not isinstance(other, UsersUserUserIdUuidBody1):
+        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,91 +11,91 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class WorkspaceIdUuidUsersBody(object):
+class CreateAgentRequestAzureConfig(object):
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
-        'workspace_id': 'object',
-        'users': 'list[RimeUserWithRole]'
+        'azure_client_id': 'str',
+        'azure_tenant_id': 'str'
     }
 
     attribute_map = {
-        'workspace_id': 'workspaceId',
-        'users': 'users'
+        'azure_client_id': 'azureClientId',
+        'azure_tenant_id': 'azureTenantId'
     }
 
-    def __init__(self, workspace_id=None, users=None):  # noqa: E501
-        """WorkspaceIdUuidUsersBody - a model defined in Swagger"""  # noqa: E501
-        self._workspace_id = None
-        self._users = None
+    def __init__(self, azure_client_id=None, azure_tenant_id=None):  # noqa: E501
+        """CreateAgentRequestAzureConfig - a model defined in Swagger"""  # noqa: E501
+        self._azure_client_id = None
+        self._azure_tenant_id = None
         self.discriminator = None
-        if workspace_id is not None:
-            self.workspace_id = workspace_id
-        if users is not None:
-            self.users = users
+        if azure_client_id is not None:
+            self.azure_client_id = azure_client_id
+        if azure_tenant_id is not None:
+            self.azure_tenant_id = azure_tenant_id
 
     @property
-    def workspace_id(self):
-        """Gets the workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
+    def azure_client_id(self):
+        """Gets the azure_client_id of this CreateAgentRequestAzureConfig.  # noqa: E501
 
-        Unique ID of an object in RIME.  # noqa: E501
+        Azure workload Identity Client ID.  # noqa: E501
 
-        :return: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :rtype: object
+        :return: The azure_client_id of this CreateAgentRequestAzureConfig.  # noqa: E501
+        :rtype: str
         """
-        return self._workspace_id
+        return self._azure_client_id
 
-    @workspace_id.setter
-    def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this WorkspaceIdUuidUsersBody.
+    @azure_client_id.setter
+    def azure_client_id(self, azure_client_id):
+        """Sets the azure_client_id of this CreateAgentRequestAzureConfig.
 
-        Unique ID of an object in RIME.  # noqa: E501
+        Azure workload Identity Client ID.  # noqa: E501
 
-        :param workspace_id: The workspace_id of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :type: object
+        :param azure_client_id: The azure_client_id of this CreateAgentRequestAzureConfig.  # noqa: E501
+        :type: str
         """
 
-        self._workspace_id = workspace_id
+        self._azure_client_id = azure_client_id
 
     @property
-    def users(self):
-        """Gets the users of this WorkspaceIdUuidUsersBody.  # noqa: E501
+    def azure_tenant_id(self):
+        """Gets the azure_tenant_id of this CreateAgentRequestAzureConfig.  # noqa: E501
 
-        List of Users to add to the Workspace.  # noqa: E501
+        Azure workload Identity Tenant ID.  # noqa: E501
 
-        :return: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :rtype: list[RimeUserWithRole]
+        :return: The azure_tenant_id of this CreateAgentRequestAzureConfig.  # noqa: E501
+        :rtype: str
         """
-        return self._users
+        return self._azure_tenant_id
 
-    @users.setter
-    def users(self, users):
-        """Sets the users of this WorkspaceIdUuidUsersBody.
+    @azure_tenant_id.setter
+    def azure_tenant_id(self, azure_tenant_id):
+        """Sets the azure_tenant_id of this CreateAgentRequestAzureConfig.
 
-        List of Users to add to the Workspace.  # noqa: E501
+        Azure workload Identity Tenant ID.  # noqa: E501
 
-        :param users: The users of this WorkspaceIdUuidUsersBody.  # noqa: E501
-        :type: list[RimeUserWithRole]
+        :param azure_tenant_id: The azure_tenant_id of this CreateAgentRequestAzureConfig.  # noqa: E501
+        :type: str
         """
 
-        self._users = users
+        self._azure_tenant_id = azure_tenant_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -110,15 +110,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(WorkspaceIdUuidUsersBody, dict):
+        if issubclass(CreateAgentRequestAzureConfig, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -126,15 +126,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, WorkspaceIdUuidUsersBody):
+        if not isinstance(other, CreateAgentRequestAzureConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.1.0rc0/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/test_batch.py` & `rime_sdk-2.1.0rc0/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk/test_run.py` & `rime_sdk-2.1.0rc0/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.0.0rc8/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.1.0rc0/rime_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.0.0rc8
+Version: 2.1.0rc0
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.0.0rc8/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.1.0rc0/rime_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 rime_sdk/swagger/swagger_client/models/__init__.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
 rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
 rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
 rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
 rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
 rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
 rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
@@ -100,23 +101,17 @@
 rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
 rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
 rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
 rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
 rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
-rime_sdk/swagger/swagger_client/models/firewall_custom_loader_location.py
-rime_sdk/swagger/swagger_client/models/firewall_data_collector_location.py
-rime_sdk/swagger/swagger_client/models/firewall_data_location.py
-rime_sdk/swagger/swagger_client/models/firewall_delta_lake_location.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
-rime_sdk/swagger/swagger_client/models/firewall_location_args.py
-rime_sdk/swagger/swagger_client/models/firewall_location_params.py
 rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
 rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
 rime_sdk/swagger/swagger_client/models/googlerpc_status.py
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
 rime_sdk/swagger/swagger_client/models/integration_integration.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
 rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
@@ -183,15 +178,15 @@
 rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
 rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
 rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
 rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
 rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
 rime_sdk/swagger/swagger_client/models/project_owner_details.py
 rime_sdk/swagger/swagger_client/models/project_project.py
-rime_sdk/swagger/swagger_client/models/project_project_with_owner_details.py
+rime_sdk/swagger/swagger_client/models/project_project_with_details.py
 rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
 rime_sdk/swagger/swagger_client/models/project_update_project_response.py
 rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
 rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
 rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/protobuf_any.py
 rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
@@ -355,15 +350,14 @@
 rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
 rime_sdk/swagger/swagger_client/models/rime_subject_type.py
 rime_sdk/swagger/swagger_client/models/rime_suggestion.py
 rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
 rime_sdk/swagger/swagger_client/models/rime_table_column.py
 rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
 rime_sdk/swagger/swagger_client/models/rime_tag.py
-rime_sdk/swagger/swagger_client/models/rime_termination_reason.py
 rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
 rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
 rime_sdk/swagger/swagger_client/models/rime_test_metric.py
 rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
 rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
 rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
 rime_sdk/swagger/swagger_client/models/rime_test_type.py
```

### Comparing `rime_sdk-2.0.0rc8/setup.py` & `rime_sdk-2.1.0rc0/setup.py`

 * *Files identical despite different names*

