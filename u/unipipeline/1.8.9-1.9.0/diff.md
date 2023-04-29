# Comparing `tmp/unipipeline-1.8.9.tar.gz` & `tmp/unipipeline-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipipeline-1.8.9.tar", last modified: Sat Apr 29 13:35:06 2023, max compression
+gzip compressed data, was "unipipeline-1.9.0.tar", last modified: Sat Apr 29 18:20:25 2023, max compression
```

## Comparing `unipipeline-1.8.9.tar` & `unipipeline-1.9.0.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/
--rwxrwxr-x   0 master    (1000) master    (1000)     1063 2022-08-17 09:07:38.000000 unipipeline-1.8.9/LICENSE
--rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 13:35:06.376462 unipipeline-1.8.9/PKG-INFO
--rwxrwxr-x   0 master    (1000) master    (1000)    10229 2022-08-17 09:07:38.000000 unipipeline-1.8.9/README.md
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.8.9/example/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     1811 2022-06-22 10:47:54.000000 unipipeline-1.8.9/example/args.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/brokers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.9/example/brokers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      294 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/brokers/kafka_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      213 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/brokers/rmq_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)       86 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/brokers/uni_log_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      299 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/example_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)      295 2022-06-07 10:55:34.000000 unipipeline-1.8.9/example/example_cron_producer.py
--rw-rw-r--   0 master    (1000) master    (1000)      281 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/example_csi.py
--rw-rw-r--   0 master    (1000) master    (1000)      776 2022-08-17 09:07:38.000000 unipipeline-1.8.9/example/example_producer.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/messages/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.9/example/messages/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      115 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/messages/ender_after_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      135 2022-06-13 15:46:45.000000 unipipeline-1.8.9/example/messages/ender_after_cron_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      133 2022-06-13 15:46:17.000000 unipipeline-1.8.9/example/messages/ender_after_cron_input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      114 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/messages/ender_after_input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      118 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/messages/input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      111 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/messages/some_external_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/waitings/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.9/example/waitings/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      142 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/waitings/common_db_wating.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/workers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 20:36:10.000000 unipipeline-1.8.9/example/workers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      407 2023-02-23 10:59:56.000000 unipipeline-1.8.9/example/workers/auto_retry_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)      682 2022-06-13 15:46:56.000000 unipipeline-1.8.9/example/workers/ender_after_cron_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)      672 2022-06-21 08:44:39.000000 unipipeline-1.8.9/example/workers/ender_after_input_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1544 2022-06-24 18:53:05.000000 unipipeline-1.8.9/example/workers/input_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1028 2022-06-13 15:49:23.000000 unipipeline-1.8.9/example/workers/my_super_cron_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)       38 2023-04-29 13:35:06.376462 unipipeline-1.8.9/setup.cfg
--rwxrwxr-x   0 master    (1000) master    (1000)     1767 2023-04-29 13:33:34.000000 unipipeline-1.8.9/setup.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-11-22 19:50:31.000000 unipipeline-1.8.9/unipipeline/__init__.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/answer/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:16:22.000000 unipipeline-1.8.9/unipipeline/answer/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     1503 2022-06-07 15:42:31.000000 unipipeline-1.8.9/unipipeline/answer/uni_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      210 2022-06-24 18:50:54.000000 unipipeline-1.8.9/unipipeline/answer/uni_answer_params.py
--rw-rw-r--   0 master    (1000) master    (1000)     5142 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/args.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/brokers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.8.9/unipipeline/brokers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)    16198 2022-06-24 21:52:15.000000 unipipeline-1.8.9/unipipeline/brokers/uni_amqp_pika_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)    26084 2023-03-17 09:06:42.000000 unipipeline-1.8.9/unipipeline/brokers/uni_amqp_py_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     4031 2022-06-24 18:01:25.000000 unipipeline-1.8.9/unipipeline/brokers/uni_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      306 2022-06-24 20:56:59.000000 unipipeline-1.8.9/unipipeline/brokers/uni_broker_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)     6130 2023-04-29 13:27:24.000000 unipipeline-1.8.9/unipipeline/brokers/uni_kafka_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1915 2022-06-06 14:43:02.000000 unipipeline-1.8.9/unipipeline/brokers/uni_log_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     7198 2022-06-24 21:10:13.000000 unipipeline-1.8.9/unipipeline/brokers/uni_memory_broker.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/config/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:04:47.000000 unipipeline-1.8.9/unipipeline/config/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)    21472 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/config/uni_config.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/definitions/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:12:24.000000 unipipeline-1.8.9/unipipeline/definitions/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      511 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_broker_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      276 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_codec_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1243 2023-01-18 14:06:03.000000 unipipeline-1.8.9/unipipeline/definitions/uni_cron_task_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      697 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      179 2022-06-06 16:36:07.000000 unipipeline-1.8.9/unipipeline/definitions/uni_dynamic_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      161 2021-07-22 21:12:30.000000 unipipeline-1.8.9/unipipeline/definitions/uni_external_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      232 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_message_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     5911 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_module_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      158 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_service_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1128 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_waiting_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1127 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_worker_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      637 2022-06-24 21:10:13.000000 unipipeline-1.8.9/unipipeline/errors.py
--rw-rw-r--   0 master    (1000) master    (1000)      132 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/main.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/message/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.8.9/unipipeline/message/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      110 2021-07-22 21:11:39.000000 unipipeline-1.8.9/unipipeline/message/uni_cron_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      116 2022-06-06 16:35:13.000000 unipipeline-1.8.9/unipipeline/message/uni_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/message_meta/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.8.9/unipipeline/message_meta/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     2794 2022-06-24 18:03:59.000000 unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta.py
--rw-rw-r--   0 master    (1000) master    (1000)      340 2022-06-06 16:36:31.000000 unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta_err.py
--rw-rw-r--   0 master    (1000) master    (1000)      298 2022-06-06 16:15:06.000000 unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta_error_topic.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/modules/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.8.9/unipipeline/modules/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      416 2021-11-17 17:34:03.000000 unipipeline-1.8.9/unipipeline/modules/test_uni_util.py
--rw-rw-r--   0 master    (1000) master    (1000)     5102 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/modules/uni.py
--rw-rw-r--   0 master    (1000) master    (1000)     2160 2022-06-22 14:13:58.000000 unipipeline-1.8.9/unipipeline/modules/uni_cron_job.py
--rw-rw-r--   0 master    (1000) master    (1000)    21881 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/modules/uni_mediator.py
--rw-rw-r--   0 master    (1000) master    (1000)        0 2022-07-25 03:22:44.000000 unipipeline-1.8.9/unipipeline/py.typed
--rw-rw-r--   0 master    (1000) master    (1000)     1515 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/run.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/utils/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.8.9/unipipeline/utils/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      600 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/utils/complex_serializer.py
--rw-rw-r--   0 master    (1000) master    (1000)      111 2023-01-18 10:00:59.000000 unipipeline-1.8.9/unipipeline/utils/filter_camel.py
--rw-rw-r--   0 master    (1000) master    (1000)     2780 2022-06-07 15:42:12.000000 unipipeline-1.8.9/unipipeline/utils/sig.py
--rw-rw-r--   0 master    (1000) master    (1000)     2902 2021-07-22 21:03:59.000000 unipipeline-1.8.9/unipipeline/utils/uni_echo.py
--rw-rw-r--   0 master    (1000) master    (1000)      418 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/utils/uni_util.py
--rw-rw-r--   0 master    (1000) master    (1000)      737 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/utils/uni_util_color.py
--rw-rw-r--   0 master    (1000) master    (1000)      798 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/utils/uni_util_template.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/waiting/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/waiting/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      780 2022-06-06 15:35:18.000000 unipipeline-1.8.9/unipipeline/waiting/uni_postgres_waiting.py
--rw-rw-r--   0 master    (1000) master    (1000)      133 2021-06-09 18:57:22.000000 unipipeline-1.8.9/unipipeline/waiting/uni_wating.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/worker/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:17:42.000000 unipipeline-1.8.9/unipipeline/worker/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      899 2022-06-24 18:49:23.000000 unipipeline-1.8.9/unipipeline/worker/uni_msg_params.py
--rw-rw-r--   0 master    (1000) master    (1000)      910 2022-06-06 14:43:02.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     4896 2022-06-24 21:09:34.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)     1786 2022-06-24 18:53:45.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_manager.py
--rw-rw-r--   0 master    (1000) master    (1000)     1582 2022-06-24 21:10:13.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline.egg-info/
--rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/PKG-INFO
--rw-rw-r--   0 master    (1000) master    (1000)     3407 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 master    (1000) master    (1000)        1 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 master    (1000) master    (1000)       54 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/entry_points.txt
--rw-rw-r--   0 master    (1000) master    (1000)        1 2022-07-25 03:30:28.000000 unipipeline-1.8.9/unipipeline.egg-info/not-zip-safe
--rw-rw-r--   0 master    (1000) master    (1000)      143 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/requires.txt
--rw-rw-r--   0 master    (1000) master    (1000)       20 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/top_level.txt
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/
+-rwxrwxr-x   0 master    (1000) master    (1000)     1063 2022-08-17 09:07:38.000000 unipipeline-1.9.0/LICENSE
+-rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 18:20:25.683588 unipipeline-1.9.0/PKG-INFO
+-rwxrwxr-x   0 master    (1000) master    (1000)    10229 2022-08-17 09:07:38.000000 unipipeline-1.9.0/README.md
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.679588 unipipeline-1.9.0/example/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.9.0/example/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1811 2022-06-22 10:47:54.000000 unipipeline-1.9.0/example/args.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.679588 unipipeline-1.9.0/example/brokers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.0/example/brokers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      294 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/brokers/kafka_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      213 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/brokers/rmq_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)       86 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/brokers/uni_log_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      299 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/example_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      295 2022-06-07 10:55:34.000000 unipipeline-1.9.0/example/example_cron_producer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      281 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/example_csi.py
+-rw-rw-r--   0 master    (1000) master    (1000)      776 2022-08-17 09:07:38.000000 unipipeline-1.9.0/example/example_producer.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/example/messages/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.0/example/messages/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      115 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/messages/ender_after_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      135 2022-06-13 15:46:45.000000 unipipeline-1.9.0/example/messages/ender_after_cron_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      133 2022-06-13 15:46:17.000000 unipipeline-1.9.0/example/messages/ender_after_cron_input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      114 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/messages/ender_after_input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      118 2022-06-06 14:43:02.000000 unipipeline-1.9.0/example/messages/input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      111 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/messages/some_external_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/example/waitings/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.9.0/example/waitings/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      142 2021-11-22 19:50:31.000000 unipipeline-1.9.0/example/waitings/common_db_wating.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/example/workers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 20:36:10.000000 unipipeline-1.9.0/example/workers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      407 2023-02-23 10:59:56.000000 unipipeline-1.9.0/example/workers/auto_retry_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      682 2022-06-13 15:46:56.000000 unipipeline-1.9.0/example/workers/ender_after_cron_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      672 2022-06-21 08:44:39.000000 unipipeline-1.9.0/example/workers/ender_after_input_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1544 2023-04-29 16:22:20.000000 unipipeline-1.9.0/example/workers/input_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1028 2022-06-13 15:49:23.000000 unipipeline-1.9.0/example/workers/my_super_cron_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)       38 2023-04-29 18:20:25.683588 unipipeline-1.9.0/setup.cfg
+-rwxrwxr-x   0 master    (1000) master    (1000)     1767 2023-04-29 18:20:06.000000 unipipeline-1.9.0/setup.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-11-22 19:50:31.000000 unipipeline-1.9.0/unipipeline/__init__.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/answer/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:16:22.000000 unipipeline-1.9.0/unipipeline/answer/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1503 2022-06-07 15:42:31.000000 unipipeline-1.9.0/unipipeline/answer/uni_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      210 2022-06-24 18:50:54.000000 unipipeline-1.9.0/unipipeline/answer/uni_answer_params.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5142 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/args.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/brokers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.9.0/unipipeline/brokers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)    16198 2022-06-24 21:52:15.000000 unipipeline-1.9.0/unipipeline/brokers/uni_amqp_pika_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)    26095 2023-04-29 15:19:17.000000 unipipeline-1.9.0/unipipeline/brokers/uni_amqp_py_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     4031 2022-06-24 18:01:25.000000 unipipeline-1.9.0/unipipeline/brokers/uni_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      306 2022-06-24 20:56:59.000000 unipipeline-1.9.0/unipipeline/brokers/uni_broker_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)     6894 2023-04-29 16:21:17.000000 unipipeline-1.9.0/unipipeline/brokers/uni_kafka_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1915 2022-06-06 14:43:02.000000 unipipeline-1.9.0/unipipeline/brokers/uni_log_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     7198 2022-06-24 21:10:13.000000 unipipeline-1.9.0/unipipeline/brokers/uni_memory_broker.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/config/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:04:47.000000 unipipeline-1.9.0/unipipeline/config/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)    21472 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/config/uni_config.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/definitions/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:12:24.000000 unipipeline-1.9.0/unipipeline/definitions/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      511 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_broker_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      276 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_codec_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1243 2023-01-18 14:06:03.000000 unipipeline-1.9.0/unipipeline/definitions/uni_cron_task_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      697 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      179 2022-06-06 16:36:07.000000 unipipeline-1.9.0/unipipeline/definitions/uni_dynamic_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      161 2021-07-22 21:12:30.000000 unipipeline-1.9.0/unipipeline/definitions/uni_external_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      232 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_message_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5911 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_module_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      158 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_service_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1128 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_waiting_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1127 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/definitions/uni_worker_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      846 2023-04-29 18:15:03.000000 unipipeline-1.9.0/unipipeline/errors.py
+-rw-rw-r--   0 master    (1000) master    (1000)      132 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/main.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/message/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.9.0/unipipeline/message/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      110 2021-07-22 21:11:39.000000 unipipeline-1.9.0/unipipeline/message/uni_cron_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      116 2022-06-06 16:35:13.000000 unipipeline-1.9.0/unipipeline/message/uni_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/message_meta/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.9.0/unipipeline/message_meta/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2794 2022-06-24 18:03:59.000000 unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta.py
+-rw-rw-r--   0 master    (1000) master    (1000)      340 2022-06-06 16:36:31.000000 unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta_err.py
+-rw-rw-r--   0 master    (1000) master    (1000)      328 2023-04-29 18:17:11.000000 unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta_error_topic.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/modules/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.9.0/unipipeline/modules/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      416 2021-11-17 17:34:03.000000 unipipeline-1.9.0/unipipeline/modules/test_uni_util.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5102 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/modules/uni.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2160 2022-06-22 14:13:58.000000 unipipeline-1.9.0/unipipeline/modules/uni_cron_job.py
+-rw-rw-r--   0 master    (1000) master    (1000)    21881 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/modules/uni_mediator.py
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2022-07-25 03:22:44.000000 unipipeline-1.9.0/unipipeline/py.typed
+-rw-rw-r--   0 master    (1000) master    (1000)     1515 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/run.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/utils/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.9.0/unipipeline/utils/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      600 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/utils/complex_serializer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      111 2023-01-18 10:00:59.000000 unipipeline-1.9.0/unipipeline/utils/filter_camel.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2780 2022-06-07 15:42:12.000000 unipipeline-1.9.0/unipipeline/utils/sig.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2902 2021-07-22 21:03:59.000000 unipipeline-1.9.0/unipipeline/utils/uni_echo.py
+-rw-rw-r--   0 master    (1000) master    (1000)      418 2023-02-22 10:34:17.000000 unipipeline-1.9.0/unipipeline/utils/uni_util.py
+-rw-rw-r--   0 master    (1000) master    (1000)      737 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/utils/uni_util_color.py
+-rw-rw-r--   0 master    (1000) master    (1000)      798 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/utils/uni_util_template.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/waiting/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 20:24:04.000000 unipipeline-1.9.0/unipipeline/waiting/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      780 2022-06-06 15:35:18.000000 unipipeline-1.9.0/unipipeline/waiting/uni_postgres_waiting.py
+-rw-rw-r--   0 master    (1000) master    (1000)      133 2021-06-09 18:57:22.000000 unipipeline-1.9.0/unipipeline/waiting/uni_wating.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline/worker/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:17:42.000000 unipipeline-1.9.0/unipipeline/worker/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      899 2022-06-24 18:49:23.000000 unipipeline-1.9.0/unipipeline/worker/uni_msg_params.py
+-rw-rw-r--   0 master    (1000) master    (1000)      910 2022-06-06 14:43:02.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5272 2023-04-29 18:19:32.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1786 2023-04-29 18:05:31.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_manager.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1618 2023-04-29 18:10:58.000000 unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 18:20:25.683588 unipipeline-1.9.0/unipipeline.egg-info/
+-rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 master    (1000) master    (1000)     3407 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 master    (1000) master    (1000)        1 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 master    (1000) master    (1000)       54 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 master    (1000) master    (1000)        1 2022-07-25 03:30:28.000000 unipipeline-1.9.0/unipipeline.egg-info/not-zip-safe
+-rw-rw-r--   0 master    (1000) master    (1000)      143 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/requires.txt
+-rw-rw-r--   0 master    (1000) master    (1000)       20 2023-04-29 18:20:25.000000 unipipeline-1.9.0/unipipeline.egg-info/top_level.txt
```

### Comparing `unipipeline-1.8.9/LICENSE` & `unipipeline-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/PKG-INFO` & `unipipeline-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipipeline
-Version: 1.8.9
+Version: 1.9.0
 Summary: simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker
 Home-page: https://github.com/aliaksandr-master/unipipeline
 Author: Aliaksandr Master
 Author-email: alxe.master@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unipipeline-1.8.9/README.md` & `unipipeline-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/example/args.py` & `unipipeline-1.9.0/example/args.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/example/example_producer.py` & `unipipeline-1.9.0/example/example_producer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/example/workers/ender_after_cron_worker.py` & `unipipeline-1.9.0/example/workers/ender_after_cron_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/example/workers/ender_after_input_worker.py` & `unipipeline-1.9.0/example/workers/ender_after_input_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/example/workers/input_worker.py` & `unipipeline-1.9.0/example/workers/input_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/example/workers/my_super_cron_worker.py` & `unipipeline-1.9.0/example/workers/my_super_cron_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/setup.py` & `unipipeline-1.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="unipipeline",
-    version="1.8.9",
+    version="1.9.0",
     description="simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aliaksandr-master/unipipeline",
     author="Aliaksandr Master",
     author_email="alxe.master@gmail.com",
     license="MIT",
```

### Comparing `unipipeline-1.8.9/unipipeline/answer/uni_answer_message.py` & `unipipeline-1.9.0/unipipeline/answer/uni_answer_message.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/args.py` & `unipipeline-1.9.0/unipipeline/args.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/brokers/uni_amqp_pika_broker.py` & `unipipeline-1.9.0/unipipeline/brokers/uni_amqp_pika_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/brokers/uni_amqp_py_broker.py` & `unipipeline-1.9.0/unipipeline/brokers/uni_amqp_py_broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,15 @@
             self._connection = None
             self.echo.log_debug('close :: already closed')
             return
 
         try:
             with self._interaction():
                 self._connection.close()
-        except AMQPError as e:  # noqa
+        except (AMQPError, OSError) as e:  # noqa
             self.echo.log_warning(f'close :: error :: {str(e)}')
         self._connection = None
         self.echo.log_debug('close :: done')
 
     def add_consumer(self, consumer: UniBrokerConsumer) -> None:
         echo = self.echo.mk_child(f'topic[{consumer.topic}]')
         if self._consuming_enabled:
```

### Comparing `unipipeline-1.8.9/unipipeline/brokers/uni_broker.py` & `unipipeline-1.9.0/unipipeline/brokers/uni_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/brokers/uni_kafka_broker.py` & `unipipeline-1.9.0/unipipeline/brokers/uni_kafka_broker.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,53 +42,36 @@
         self._kfk_active_consumers: List[KafkaConsumer] = list()
 
         self._consuming_started = False
         self._interrupted = False
         self._in_processing = False
 
     def stop_consuming(self) -> None:    # TODO
+        self._interrupted = True
         self._end_consuming()
 
-    def _end_consuming(self) -> None:
+    def _end_consuming(self, force: bool = False) -> None:
         if not self._consuming_started:
             return
-        self._interrupted = True
-        if not self._in_processing:
-            for kfk_consumer in self._kfk_active_consumers:
-                kfk_consumer.close()
-            self._consuming_started = False
-            self.echo.log_info('consumption stopped')
+        if self._in_processing and not force:
+            return
+        for kfk_consumer in self._kfk_active_consumers:
+            kfk_consumer.close()
+        self._kfk_active_consumers.clear()
+        self._consuming_started = False
+        self.echo.log_info('consumption stopped')
 
     def get_topic_approximate_messages_count(self, topic: str) -> int:
         return 0  # TODO
 
     def initialize(self, topics: Set[str], answer_topic: Set[str]) -> None:
         pass  # TODO
 
     def connect(self) -> None:
-        if self._producer is not None:
-            if self._producer._closed:
-                self._producer.close()
-                self._producer = None
-            else:
-                return
-
-        # TODO: change default connection as producer yo abstract connection to kafka server
-        self._producer = KafkaProducer(
-            bootstrap_servers=self._bootstrap_servers,
-            api_version=self.config.api_version,
-            retries=self.config.retry_max_count,
-            acks=1,
-            **self._security_conf,
-        )
-
-        if not self._producer.bootstrap_connected():
-            raise ConnectionError()
-
-        self.echo.log_info('connected')
+        pass
 
     def close(self) -> None:
         if self._producer is not None:
             self._producer.close()
             self._producer = None
         for kfk_consumer in self._kfk_active_consumers:
             kfk_consumer.close()
@@ -114,53 +97,85 @@
         consumer = self._consumers[0]
         kfk_consumer = KafkaConsumer(
             consumer.topic,
             api_version=self.config.api_version,
             bootstrap_servers=self._bootstrap_servers,
             enable_auto_commit=False,
             group_id=consumer.group_id,
-            # fetch_max_wait_ms=1000 * 30,  # 30sec
-            # max_in_flight_requests_per_connection=3,
-            # max_poll_interval_ms=300_000,
-            # session_timeout_ms=10_000,
+            max_poll_records=1,
+            max_poll_interval_ms=10 * 60_000,
+            session_timeout_ms=10 * 60_000,
+            request_timeout_ms=10 * 60_000 + 5,
+            connections_max_idle_ms=10 * 60_000 + 15,
         )
 
         self._kfk_active_consumers.append(kfk_consumer)
 
         # TODO: retry
+        exit_with_error = ''
         for consumer_record in kfk_consumer:
             self._in_processing = True
+            echo.log_info(f'consuming message [{consumer_record.offset}]. started')
 
             get_meta = functools.partial(
                 self.parse_message_body,
                 content=consumer_record.value,
                 compression=self.definition.compression,
                 content_type=self.definition.content_type,
                 unwrapped=consumer.unwrapped,
             )
 
             rejected = False
             try:
                 consumer.message_handler(get_meta)
-            except UniMessageRejectError:
+            except UniMessageRejectError as e:
                 rejected = True
-                kfk_consumer.commit()
-            if not rejected:
-                kfk_consumer.commit()
+                echo.log_warning(f'consuming message [{consumer_record.offset}]. reject {type(e).__name__}. {e}')
+            except Exception as e:  # noqa
+                echo.log_error(f'consuming message [{consumer_record.offset}]. error {type(e).__name__}. {e}')
+                raise
 
             self._in_processing = False
+            if not rejected:
+                try:
+                    kfk_consumer.commit()
+                except Exception as e:  # noqa
+                    exit_with_error = f'consuming message [{consumer_record.offset}]. error {type(e).__name__}. {e}'
+                    break
+                else:
+                    echo.log_info(f'consuming message [{consumer_record.offset}]. ok')
             if self._interrupted:
-                self._end_consuming()
                 break
 
-        for kfk_consumer in self._kfk_active_consumers:
-            kfk_consumer.close()
+        self._end_consuming(True)
+
+        if exit_with_error:
+            echo.exit_with_error(exit_with_error)
+
+    def _connect_producer(self) -> None:
+        if self._producer is not None:
+            if self._producer._closed:
+                self._producer.close()
+                self._producer = None
+            else:
+                return
+
+        # TODO: change default connection as producer yo abstract connection to kafka server
+        self._producer = KafkaProducer(
+            bootstrap_servers=self._bootstrap_servers,
+            api_version=self.config.api_version,
+            retries=self.config.retry_max_count,
+            acks=1,
+            **self._security_conf,
+        )
+
+        self.echo.log_info('connected')
 
     def _get_producer(self) -> KafkaProducer:
-        self.connect()
+        self._connect_producer()
         assert self._producer is not None
         return self._producer
 
     def publish(self, topic: str, meta_list: List[UniMessageMeta], alone: bool = False) -> None:
         # TODO: alone
         # TODO: ttl
         # TODO: retry
```

### Comparing `unipipeline-1.8.9/unipipeline/brokers/uni_log_broker.py` & `unipipeline-1.9.0/unipipeline/brokers/uni_log_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/brokers/uni_memory_broker.py` & `unipipeline-1.9.0/unipipeline/brokers/uni_memory_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/config/uni_config.py` & `unipipeline-1.9.0/unipipeline/config/uni_config.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/definitions/uni_cron_task_definition.py` & `unipipeline-1.9.0/unipipeline/definitions/uni_cron_task_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/definitions/uni_definition.py` & `unipipeline-1.9.0/unipipeline/definitions/uni_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/definitions/uni_module_definition.py` & `unipipeline-1.9.0/unipipeline/definitions/uni_module_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/definitions/uni_waiting_definition.py` & `unipipeline-1.9.0/unipipeline/definitions/uni_waiting_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/definitions/uni_worker_definition.py` & `unipipeline-1.9.0/unipipeline/definitions/uni_worker_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/errors.py` & `unipipeline-1.9.0/unipipeline/errors.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Optional
+
+
 class UniError(Exception):
     pass
 
 
 class UniAnswerDelayError(UniError):
     pass
 
@@ -39,8 +42,14 @@
 
 
 class UniSendingToUndefinedWorkerError(UniError):
     pass
 
 
 class UniMessageRejectError(UniError):
-    pass
+
+    def __init__(self, exc: Optional[Exception] = None) -> None:
+        self._exc = exc
+
+    @property
+    def rejection_exception(self) -> Optional[Exception]:
+        return self._exc
```

### Comparing `unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta.py` & `unipipeline-1.9.0/unipipeline/message_meta/uni_message_meta.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/modules/uni.py` & `unipipeline-1.9.0/unipipeline/modules/uni.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/modules/uni_cron_job.py` & `unipipeline-1.9.0/unipipeline/modules/uni_cron_job.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/modules/uni_mediator.py` & `unipipeline-1.9.0/unipipeline/modules/uni_mediator.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/run.py` & `unipipeline-1.9.0/unipipeline/run.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/utils/complex_serializer.py` & `unipipeline-1.9.0/unipipeline/utils/complex_serializer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/utils/sig.py` & `unipipeline-1.9.0/unipipeline/utils/sig.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/utils/uni_echo.py` & `unipipeline-1.9.0/unipipeline/utils/uni_echo.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/utils/uni_util_color.py` & `unipipeline-1.9.0/unipipeline/utils/uni_util_color.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/utils/uni_util_template.py` & `unipipeline-1.9.0/unipipeline/utils/uni_util_template.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/waiting/uni_postgres_waiting.py` & `unipipeline-1.9.0/unipipeline/waiting/uni_postgres_waiting.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/worker/uni_msg_params.py` & `unipipeline-1.9.0/unipipeline/worker/uni_msg_params.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/worker/uni_worker.py` & `unipipeline-1.9.0/unipipeline/worker/uni_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer.py` & `unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 import uuid
 from typing import TypeVar, Generic, Optional, Type, Any, Union, Dict, TYPE_CHECKING, Callable
 
 from unipipeline.answer.uni_answer_message import UniAnswerMessage
 from unipipeline.definitions.uni_worker_definition import UniWorkerDefinition
 from unipipeline.errors import UniMessagePayloadParsingError, \
-    UniAnswerMessagePayloadParsingError, UniSendingToUndefinedWorkerError
+    UniAnswerMessagePayloadParsingError, UniSendingToUndefinedWorkerError, UniMessageRejectError
 from unipipeline.message.uni_message import UniMessage
 from unipipeline.message_meta.uni_message_meta import UniMessageMeta, UniMessageMetaErrTopic, UniAnswerParams
 from unipipeline.worker.uni_msg_params import UniGettingAnswerParams, UniSendingParams, TUniSendingMessagePayloadUnion, TUniSendingWorkerUnion
 from unipipeline.worker.uni_worker import UniWorker
 from unipipeline.worker.uni_worker_consumer_manager import UniWorkerConsumerManager
 from unipipeline.worker.uni_worker_consumer_message import UniWorkerConsumerMessage
 
@@ -86,14 +86,21 @@
 
         except UniMessagePayloadParsingError as e:
             self._uni_echo.log_warning(f'answer payload is invalid! message {meta.id} was skipped')
             self._mediator.move_to_error_topic(self._definition, meta, UniMessageMetaErrTopic.MESSAGE_PAYLOAD_ERR, e)
             self._current_meta = None
             return
 
+        except UniMessageRejectError as e:
+            self._uni_echo.log_warning(f'rejected message {meta.id}')
+            if e.rejection_exception is not None:
+                self._mediator.move_to_error_topic(self._definition, meta, UniMessageMetaErrTopic.USER_ERROR, e.rejection_exception)
+            self._current_meta = None
+            raise
+
         self._uni_echo.log_debug(f'processing successfully done {meta.id}')
         if meta.need_answer and self._definition.need_answer:
             try:
                 self._mediator.answer_to(self._definition.name, meta, result, unwrapped=self._definition.answer_unwrapped)
             except UniSendingToUndefinedWorkerError:
                 pass
```

### Comparing `unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_manager.py` & `unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_manager.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_message.py` & `unipipeline-1.9.0/unipipeline/worker/uni_worker_consumer_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 class UniWorkerConsumerMessage(Generic[TInputMsgPayload]):
     def __init__(self, message_input: Type[TInputMsgPayload], meta: UniMessageMeta) -> None:
         self._meta = meta
         self._message_input_payload_type = message_input
         self._message_payload_cache: Optional[TInputMsgPayload] = None
         self._acknowledged_or_rejected = False
 
-    def reject(self) -> None:
-        raise UniMessageRejectError()
+    def reject(self, exc: Optional[Exception] = None) -> None:
+        raise UniMessageRejectError(exc)
 
     @property
     def id(self) -> UUID:
         return self._meta.id
 
     @property
     def date_created(self) -> datetime:
```

### Comparing `unipipeline-1.8.9/unipipeline.egg-info/PKG-INFO` & `unipipeline-1.9.0/unipipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipipeline
-Version: 1.8.9
+Version: 1.9.0
 Summary: simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker
 Home-page: https://github.com/aliaksandr-master/unipipeline
 Author: Aliaksandr Master
 Author-email: alxe.master@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unipipeline-1.8.9/unipipeline.egg-info/SOURCES.txt` & `unipipeline-1.9.0/unipipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

