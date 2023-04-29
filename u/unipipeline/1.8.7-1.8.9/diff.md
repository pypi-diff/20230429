# Comparing `tmp/unipipeline-1.8.7.tar.gz` & `tmp/unipipeline-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unipipeline-1.8.7.tar", last modified: Thu Feb 23 14:12:16 2023, max compression
+gzip compressed data, was "unipipeline-1.8.9.tar", last modified: Sat Apr 29 13:35:06 2023, max compression
```

## Comparing `unipipeline-1.8.7.tar` & `unipipeline-1.8.9.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/
--rwxrwxr-x   0 master    (1000) master    (1000)     1063 2022-08-17 09:07:38.000000 unipipeline-1.8.7/LICENSE
--rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-02-23 14:12:16.678580 unipipeline-1.8.7/PKG-INFO
--rwxrwxr-x   0 master    (1000) master    (1000)    10229 2022-08-17 09:07:38.000000 unipipeline-1.8.7/README.md
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.674579 unipipeline-1.8.7/example/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.8.7/example/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     1811 2022-06-22 10:47:54.000000 unipipeline-1.8.7/example/args.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.674579 unipipeline-1.8.7/example/brokers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.7/example/brokers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      294 2022-06-06 14:43:02.000000 unipipeline-1.8.7/example/brokers/kafka_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      213 2022-06-06 14:43:02.000000 unipipeline-1.8.7/example/brokers/rmq_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)       86 2021-11-22 19:50:31.000000 unipipeline-1.8.7/example/brokers/uni_log_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      299 2022-06-06 14:43:02.000000 unipipeline-1.8.7/example/example_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)      295 2022-06-07 10:55:34.000000 unipipeline-1.8.7/example/example_cron_producer.py
--rw-rw-r--   0 master    (1000) master    (1000)      281 2021-11-22 19:50:31.000000 unipipeline-1.8.7/example/example_csi.py
--rw-rw-r--   0 master    (1000) master    (1000)      776 2022-08-17 09:07:38.000000 unipipeline-1.8.7/example/example_producer.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.674579 unipipeline-1.8.7/example/messages/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.7/example/messages/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      115 2021-11-22 19:50:31.000000 unipipeline-1.8.7/example/messages/ender_after_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      135 2022-06-13 15:46:45.000000 unipipeline-1.8.7/example/messages/ender_after_cron_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      133 2022-06-13 15:46:17.000000 unipipeline-1.8.7/example/messages/ender_after_cron_input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      114 2021-11-22 19:50:31.000000 unipipeline-1.8.7/example/messages/ender_after_input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      118 2022-06-06 14:43:02.000000 unipipeline-1.8.7/example/messages/input_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      111 2021-11-22 19:50:31.000000 unipipeline-1.8.7/example/messages/some_external_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.674579 unipipeline-1.8.7/example/waitings/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.7/example/waitings/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      142 2021-11-22 19:50:31.000000 unipipeline-1.8.7/example/waitings/common_db_wating.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.674579 unipipeline-1.8.7/example/workers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 20:36:10.000000 unipipeline-1.8.7/example/workers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      407 2023-02-23 10:59:56.000000 unipipeline-1.8.7/example/workers/auto_retry_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)      682 2022-06-13 15:46:56.000000 unipipeline-1.8.7/example/workers/ender_after_cron_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)      672 2022-06-21 08:44:39.000000 unipipeline-1.8.7/example/workers/ender_after_input_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1544 2022-06-24 18:53:05.000000 unipipeline-1.8.7/example/workers/input_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1028 2022-06-13 15:49:23.000000 unipipeline-1.8.7/example/workers/my_super_cron_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)       38 2023-02-23 14:12:16.678580 unipipeline-1.8.7/setup.cfg
--rwxrwxr-x   0 master    (1000) master    (1000)     1767 2023-02-23 14:11:30.000000 unipipeline-1.8.7/setup.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.674579 unipipeline-1.8.7/unipipeline/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-11-22 19:50:31.000000 unipipeline-1.8.7/unipipeline/__init__.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/answer/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:16:22.000000 unipipeline-1.8.7/unipipeline/answer/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     1503 2022-06-07 15:42:31.000000 unipipeline-1.8.7/unipipeline/answer/uni_answer_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      210 2022-06-24 18:50:54.000000 unipipeline-1.8.7/unipipeline/answer/uni_answer_params.py
--rw-rw-r--   0 master    (1000) master    (1000)     5142 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/args.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/brokers/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.8.7/unipipeline/brokers/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)    16198 2022-06-24 21:52:15.000000 unipipeline-1.8.7/unipipeline/brokers/uni_amqp_pika_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)    26084 2023-02-23 14:10:57.000000 unipipeline-1.8.7/unipipeline/brokers/uni_amqp_py_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     4031 2022-06-24 18:01:25.000000 unipipeline-1.8.7/unipipeline/brokers/uni_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)      306 2022-06-24 20:56:59.000000 unipipeline-1.8.7/unipipeline/brokers/uni_broker_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)     5900 2022-06-24 21:10:13.000000 unipipeline-1.8.7/unipipeline/brokers/uni_kafka_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     1915 2022-06-06 14:43:02.000000 unipipeline-1.8.7/unipipeline/brokers/uni_log_broker.py
--rw-rw-r--   0 master    (1000) master    (1000)     7198 2022-06-24 21:10:13.000000 unipipeline-1.8.7/unipipeline/brokers/uni_memory_broker.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/config/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:04:47.000000 unipipeline-1.8.7/unipipeline/config/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)    21472 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/config/uni_config.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/definitions/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:12:24.000000 unipipeline-1.8.7/unipipeline/definitions/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      511 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_broker_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      276 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_codec_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1243 2023-01-18 14:06:03.000000 unipipeline-1.8.7/unipipeline/definitions/uni_cron_task_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      697 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      179 2022-06-06 16:36:07.000000 unipipeline-1.8.7/unipipeline/definitions/uni_dynamic_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      161 2021-07-22 21:12:30.000000 unipipeline-1.8.7/unipipeline/definitions/uni_external_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      232 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_message_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     5911 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_module_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      158 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_service_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1128 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_waiting_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)     1127 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/definitions/uni_worker_definition.py
--rw-rw-r--   0 master    (1000) master    (1000)      637 2022-06-24 21:10:13.000000 unipipeline-1.8.7/unipipeline/errors.py
--rw-rw-r--   0 master    (1000) master    (1000)      132 2021-07-22 20:24:04.000000 unipipeline-1.8.7/unipipeline/main.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/message/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.8.7/unipipeline/message/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      110 2021-07-22 21:11:39.000000 unipipeline-1.8.7/unipipeline/message/uni_cron_message.py
--rw-rw-r--   0 master    (1000) master    (1000)      116 2022-06-06 16:35:13.000000 unipipeline-1.8.7/unipipeline/message/uni_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/message_meta/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.8.7/unipipeline/message_meta/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)     2794 2022-06-24 18:03:59.000000 unipipeline-1.8.7/unipipeline/message_meta/uni_message_meta.py
--rw-rw-r--   0 master    (1000) master    (1000)      340 2022-06-06 16:36:31.000000 unipipeline-1.8.7/unipipeline/message_meta/uni_message_meta_err.py
--rw-rw-r--   0 master    (1000) master    (1000)      298 2022-06-06 16:15:06.000000 unipipeline-1.8.7/unipipeline/message_meta/uni_message_meta_error_topic.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/modules/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.8.7/unipipeline/modules/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      416 2021-11-17 17:34:03.000000 unipipeline-1.8.7/unipipeline/modules/test_uni_util.py
--rw-rw-r--   0 master    (1000) master    (1000)     5102 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/modules/uni.py
--rw-rw-r--   0 master    (1000) master    (1000)     2160 2022-06-22 14:13:58.000000 unipipeline-1.8.7/unipipeline/modules/uni_cron_job.py
--rw-rw-r--   0 master    (1000) master    (1000)    21881 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/modules/uni_mediator.py
--rw-rw-r--   0 master    (1000) master    (1000)        0 2022-07-25 03:22:44.000000 unipipeline-1.8.7/unipipeline/py.typed
--rw-rw-r--   0 master    (1000) master    (1000)     1515 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/run.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/utils/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.8.7/unipipeline/utils/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      600 2021-07-22 20:24:04.000000 unipipeline-1.8.7/unipipeline/utils/complex_serializer.py
--rw-rw-r--   0 master    (1000) master    (1000)      111 2023-01-18 10:00:59.000000 unipipeline-1.8.7/unipipeline/utils/filter_camel.py
--rw-rw-r--   0 master    (1000) master    (1000)     2780 2022-06-07 15:42:12.000000 unipipeline-1.8.7/unipipeline/utils/sig.py
--rw-rw-r--   0 master    (1000) master    (1000)     2902 2021-07-22 21:03:59.000000 unipipeline-1.8.7/unipipeline/utils/uni_echo.py
--rw-rw-r--   0 master    (1000) master    (1000)      418 2023-02-22 10:34:17.000000 unipipeline-1.8.7/unipipeline/utils/uni_util.py
--rw-rw-r--   0 master    (1000) master    (1000)      737 2021-07-22 20:24:04.000000 unipipeline-1.8.7/unipipeline/utils/uni_util_color.py
--rw-rw-r--   0 master    (1000) master    (1000)      798 2021-07-22 20:24:04.000000 unipipeline-1.8.7/unipipeline/utils/uni_util_template.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/waiting/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 20:24:04.000000 unipipeline-1.8.7/unipipeline/waiting/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      780 2022-06-06 15:35:18.000000 unipipeline-1.8.7/unipipeline/waiting/uni_postgres_waiting.py
--rw-rw-r--   0 master    (1000) master    (1000)      133 2021-06-09 18:57:22.000000 unipipeline-1.8.7/unipipeline/waiting/uni_wating.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline/worker/
--rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:17:42.000000 unipipeline-1.8.7/unipipeline/worker/__init__.py
--rw-rw-r--   0 master    (1000) master    (1000)      899 2022-06-24 18:49:23.000000 unipipeline-1.8.7/unipipeline/worker/uni_msg_params.py
--rw-rw-r--   0 master    (1000) master    (1000)      910 2022-06-06 14:43:02.000000 unipipeline-1.8.7/unipipeline/worker/uni_worker.py
--rw-rw-r--   0 master    (1000) master    (1000)     4896 2022-06-24 21:09:34.000000 unipipeline-1.8.7/unipipeline/worker/uni_worker_consumer.py
--rw-rw-r--   0 master    (1000) master    (1000)     1786 2022-06-24 18:53:45.000000 unipipeline-1.8.7/unipipeline/worker/uni_worker_consumer_manager.py
--rw-rw-r--   0 master    (1000) master    (1000)     1582 2022-06-24 21:10:13.000000 unipipeline-1.8.7/unipipeline/worker/uni_worker_consumer_message.py
-drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-02-23 14:12:16.678580 unipipeline-1.8.7/unipipeline.egg-info/
--rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-02-23 14:12:16.000000 unipipeline-1.8.7/unipipeline.egg-info/PKG-INFO
--rw-rw-r--   0 master    (1000) master    (1000)     3407 2023-02-23 14:12:16.000000 unipipeline-1.8.7/unipipeline.egg-info/SOURCES.txt
--rw-rw-r--   0 master    (1000) master    (1000)        1 2023-02-23 14:12:16.000000 unipipeline-1.8.7/unipipeline.egg-info/dependency_links.txt
--rw-rw-r--   0 master    (1000) master    (1000)       54 2023-02-23 14:12:16.000000 unipipeline-1.8.7/unipipeline.egg-info/entry_points.txt
--rw-rw-r--   0 master    (1000) master    (1000)        1 2022-07-25 03:30:28.000000 unipipeline-1.8.7/unipipeline.egg-info/not-zip-safe
--rw-rw-r--   0 master    (1000) master    (1000)      143 2023-02-23 14:12:16.000000 unipipeline-1.8.7/unipipeline.egg-info/requires.txt
--rw-rw-r--   0 master    (1000) master    (1000)       20 2023-02-23 14:12:16.000000 unipipeline-1.8.7/unipipeline.egg-info/top_level.txt
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/
+-rwxrwxr-x   0 master    (1000) master    (1000)     1063 2022-08-17 09:07:38.000000 unipipeline-1.8.9/LICENSE
+-rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 13:35:06.376462 unipipeline-1.8.9/PKG-INFO
+-rwxrwxr-x   0 master    (1000) master    (1000)    10229 2022-08-17 09:07:38.000000 unipipeline-1.8.9/README.md
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.8.9/example/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1811 2022-06-22 10:47:54.000000 unipipeline-1.8.9/example/args.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/brokers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.9/example/brokers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      294 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/brokers/kafka_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      213 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/brokers/rmq_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)       86 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/brokers/uni_log_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      299 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/example_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      295 2022-06-07 10:55:34.000000 unipipeline-1.8.9/example/example_cron_producer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      281 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/example_csi.py
+-rw-rw-r--   0 master    (1000) master    (1000)      776 2022-08-17 09:07:38.000000 unipipeline-1.8.9/example/example_producer.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/messages/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.9/example/messages/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      115 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/messages/ender_after_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      135 2022-06-13 15:46:45.000000 unipipeline-1.8.9/example/messages/ender_after_cron_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      133 2022-06-13 15:46:17.000000 unipipeline-1.8.9/example/messages/ender_after_cron_input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      114 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/messages/ender_after_input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      118 2022-06-06 14:43:02.000000 unipipeline-1.8.9/example/messages/input_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      111 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/messages/some_external_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/waitings/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-05 14:14:23.000000 unipipeline-1.8.9/example/waitings/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      142 2021-11-22 19:50:31.000000 unipipeline-1.8.9/example/waitings/common_db_wating.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/example/workers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 20:36:10.000000 unipipeline-1.8.9/example/workers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      407 2023-02-23 10:59:56.000000 unipipeline-1.8.9/example/workers/auto_retry_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      682 2022-06-13 15:46:56.000000 unipipeline-1.8.9/example/workers/ender_after_cron_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      672 2022-06-21 08:44:39.000000 unipipeline-1.8.9/example/workers/ender_after_input_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1544 2022-06-24 18:53:05.000000 unipipeline-1.8.9/example/workers/input_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1028 2022-06-13 15:49:23.000000 unipipeline-1.8.9/example/workers/my_super_cron_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)       38 2023-04-29 13:35:06.376462 unipipeline-1.8.9/setup.cfg
+-rwxrwxr-x   0 master    (1000) master    (1000)     1767 2023-04-29 13:33:34.000000 unipipeline-1.8.9/setup.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-11-22 19:50:31.000000 unipipeline-1.8.9/unipipeline/__init__.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/answer/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:16:22.000000 unipipeline-1.8.9/unipipeline/answer/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1503 2022-06-07 15:42:31.000000 unipipeline-1.8.9/unipipeline/answer/uni_answer_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      210 2022-06-24 18:50:54.000000 unipipeline-1.8.9/unipipeline/answer/uni_answer_params.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5142 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/args.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/brokers/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.8.9/unipipeline/brokers/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)    16198 2022-06-24 21:52:15.000000 unipipeline-1.8.9/unipipeline/brokers/uni_amqp_pika_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)    26084 2023-03-17 09:06:42.000000 unipipeline-1.8.9/unipipeline/brokers/uni_amqp_py_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     4031 2022-06-24 18:01:25.000000 unipipeline-1.8.9/unipipeline/brokers/uni_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)      306 2022-06-24 20:56:59.000000 unipipeline-1.8.9/unipipeline/brokers/uni_broker_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)     6130 2023-04-29 13:27:24.000000 unipipeline-1.8.9/unipipeline/brokers/uni_kafka_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1915 2022-06-06 14:43:02.000000 unipipeline-1.8.9/unipipeline/brokers/uni_log_broker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     7198 2022-06-24 21:10:13.000000 unipipeline-1.8.9/unipipeline/brokers/uni_memory_broker.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/config/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:04:47.000000 unipipeline-1.8.9/unipipeline/config/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)    21472 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/config/uni_config.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/definitions/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:12:24.000000 unipipeline-1.8.9/unipipeline/definitions/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      511 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_broker_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      276 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_codec_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1243 2023-01-18 14:06:03.000000 unipipeline-1.8.9/unipipeline/definitions/uni_cron_task_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      697 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      179 2022-06-06 16:36:07.000000 unipipeline-1.8.9/unipipeline/definitions/uni_dynamic_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      161 2021-07-22 21:12:30.000000 unipipeline-1.8.9/unipipeline/definitions/uni_external_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      232 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_message_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5911 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_module_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      158 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_service_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1128 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_waiting_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1127 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/definitions/uni_worker_definition.py
+-rw-rw-r--   0 master    (1000) master    (1000)      637 2022-06-24 21:10:13.000000 unipipeline-1.8.9/unipipeline/errors.py
+-rw-rw-r--   0 master    (1000) master    (1000)      132 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/main.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/message/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.8.9/unipipeline/message/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      110 2021-07-22 21:11:39.000000 unipipeline-1.8.9/unipipeline/message/uni_cron_message.py
+-rw-rw-r--   0 master    (1000) master    (1000)      116 2022-06-06 16:35:13.000000 unipipeline-1.8.9/unipipeline/message/uni_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/message_meta/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-24 21:16:55.000000 unipipeline-1.8.9/unipipeline/message_meta/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2794 2022-06-24 18:03:59.000000 unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta.py
+-rw-rw-r--   0 master    (1000) master    (1000)      340 2022-06-06 16:36:31.000000 unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta_err.py
+-rw-rw-r--   0 master    (1000) master    (1000)      298 2022-06-06 16:15:06.000000 unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta_error_topic.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/modules/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-13 18:33:01.000000 unipipeline-1.8.9/unipipeline/modules/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      416 2021-11-17 17:34:03.000000 unipipeline-1.8.9/unipipeline/modules/test_uni_util.py
+-rw-rw-r--   0 master    (1000) master    (1000)     5102 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/modules/uni.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2160 2022-06-22 14:13:58.000000 unipipeline-1.8.9/unipipeline/modules/uni_cron_job.py
+-rw-rw-r--   0 master    (1000) master    (1000)    21881 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/modules/uni_mediator.py
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2022-07-25 03:22:44.000000 unipipeline-1.8.9/unipipeline/py.typed
+-rw-rw-r--   0 master    (1000) master    (1000)     1515 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/run.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/utils/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-06-09 18:57:22.000000 unipipeline-1.8.9/unipipeline/utils/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      600 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/utils/complex_serializer.py
+-rw-rw-r--   0 master    (1000) master    (1000)      111 2023-01-18 10:00:59.000000 unipipeline-1.8.9/unipipeline/utils/filter_camel.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2780 2022-06-07 15:42:12.000000 unipipeline-1.8.9/unipipeline/utils/sig.py
+-rw-rw-r--   0 master    (1000) master    (1000)     2902 2021-07-22 21:03:59.000000 unipipeline-1.8.9/unipipeline/utils/uni_echo.py
+-rw-rw-r--   0 master    (1000) master    (1000)      418 2023-02-22 10:34:17.000000 unipipeline-1.8.9/unipipeline/utils/uni_util.py
+-rw-rw-r--   0 master    (1000) master    (1000)      737 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/utils/uni_util_color.py
+-rw-rw-r--   0 master    (1000) master    (1000)      798 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/utils/uni_util_template.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/waiting/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 20:24:04.000000 unipipeline-1.8.9/unipipeline/waiting/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      780 2022-06-06 15:35:18.000000 unipipeline-1.8.9/unipipeline/waiting/uni_postgres_waiting.py
+-rw-rw-r--   0 master    (1000) master    (1000)      133 2021-06-09 18:57:22.000000 unipipeline-1.8.9/unipipeline/waiting/uni_wating.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline/worker/
+-rw-rw-r--   0 master    (1000) master    (1000)        0 2021-07-22 21:17:42.000000 unipipeline-1.8.9/unipipeline/worker/__init__.py
+-rw-rw-r--   0 master    (1000) master    (1000)      899 2022-06-24 18:49:23.000000 unipipeline-1.8.9/unipipeline/worker/uni_msg_params.py
+-rw-rw-r--   0 master    (1000) master    (1000)      910 2022-06-06 14:43:02.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker.py
+-rw-rw-r--   0 master    (1000) master    (1000)     4896 2022-06-24 21:09:34.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1786 2022-06-24 18:53:45.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_manager.py
+-rw-rw-r--   0 master    (1000) master    (1000)     1582 2022-06-24 21:10:13.000000 unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_message.py
+drwxrwxr-x   0 master    (1000) master    (1000)        0 2023-04-29 13:35:06.376462 unipipeline-1.8.9/unipipeline.egg-info/
+-rw-rw-r--   0 master    (1000) master    (1000)    11100 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/PKG-INFO
+-rw-rw-r--   0 master    (1000) master    (1000)     3407 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/SOURCES.txt
+-rw-rw-r--   0 master    (1000) master    (1000)        1 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/dependency_links.txt
+-rw-rw-r--   0 master    (1000) master    (1000)       54 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/entry_points.txt
+-rw-rw-r--   0 master    (1000) master    (1000)        1 2022-07-25 03:30:28.000000 unipipeline-1.8.9/unipipeline.egg-info/not-zip-safe
+-rw-rw-r--   0 master    (1000) master    (1000)      143 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/requires.txt
+-rw-rw-r--   0 master    (1000) master    (1000)       20 2023-04-29 13:35:06.000000 unipipeline-1.8.9/unipipeline.egg-info/top_level.txt
```

### Comparing `unipipeline-1.8.7/LICENSE` & `unipipeline-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/PKG-INFO` & `unipipeline-1.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipipeline
-Version: 1.8.7
+Version: 1.8.9
 Summary: simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker
 Home-page: https://github.com/aliaksandr-master/unipipeline
 Author: Aliaksandr Master
 Author-email: alxe.master@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unipipeline-1.8.7/README.md` & `unipipeline-1.8.9/README.md`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/example/args.py` & `unipipeline-1.8.9/example/args.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/example/example_producer.py` & `unipipeline-1.8.9/example/example_producer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/example/workers/ender_after_cron_worker.py` & `unipipeline-1.8.9/example/workers/ender_after_cron_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/example/workers/ender_after_input_worker.py` & `unipipeline-1.8.9/example/workers/ender_after_input_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/example/workers/input_worker.py` & `unipipeline-1.8.9/example/workers/input_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/example/workers/my_super_cron_worker.py` & `unipipeline-1.8.9/example/workers/my_super_cron_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/setup.py` & `unipipeline-1.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="unipipeline",
-    version="1.8.7",
+    version="1.8.9",
     description="simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aliaksandr-master/unipipeline",
     author="Aliaksandr Master",
     author_email="alxe.master@gmail.com",
     license="MIT",
```

### Comparing `unipipeline-1.8.7/unipipeline/answer/uni_answer_message.py` & `unipipeline-1.8.9/unipipeline/answer/uni_answer_message.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/args.py` & `unipipeline-1.8.9/unipipeline/args.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/brokers/uni_amqp_pika_broker.py` & `unipipeline-1.8.9/unipipeline/brokers/uni_amqp_pika_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/brokers/uni_amqp_py_broker.py` & `unipipeline-1.8.9/unipipeline/brokers/uni_amqp_py_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/brokers/uni_broker.py` & `unipipeline-1.8.9/unipipeline/brokers/uni_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/brokers/uni_kafka_broker.py` & `unipipeline-1.8.9/unipipeline/brokers/uni_kafka_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,18 @@
         consumer = self._consumers[0]
         kfk_consumer = KafkaConsumer(
             consumer.topic,
             api_version=self.config.api_version,
             bootstrap_servers=self._bootstrap_servers,
             enable_auto_commit=False,
             group_id=consumer.group_id,
+            # fetch_max_wait_ms=1000 * 30,  # 30sec
+            # max_in_flight_requests_per_connection=3,
+            # max_poll_interval_ms=300_000,
+            # session_timeout_ms=10_000,
         )
 
         self._kfk_active_consumers.append(kfk_consumer)
 
         # TODO: retry
         for consumer_record in kfk_consumer:
             self._in_processing = True
@@ -135,14 +139,15 @@
             )
 
             rejected = False
             try:
                 consumer.message_handler(get_meta)
             except UniMessageRejectError:
                 rejected = True
+                kfk_consumer.commit()
             if not rejected:
                 kfk_consumer.commit()
 
             self._in_processing = False
             if self._interrupted:
                 self._end_consuming()
                 break
```

### Comparing `unipipeline-1.8.7/unipipeline/brokers/uni_log_broker.py` & `unipipeline-1.8.9/unipipeline/brokers/uni_log_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/brokers/uni_memory_broker.py` & `unipipeline-1.8.9/unipipeline/brokers/uni_memory_broker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/config/uni_config.py` & `unipipeline-1.8.9/unipipeline/config/uni_config.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/definitions/uni_cron_task_definition.py` & `unipipeline-1.8.9/unipipeline/definitions/uni_cron_task_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/definitions/uni_definition.py` & `unipipeline-1.8.9/unipipeline/definitions/uni_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/definitions/uni_module_definition.py` & `unipipeline-1.8.9/unipipeline/definitions/uni_module_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/definitions/uni_waiting_definition.py` & `unipipeline-1.8.9/unipipeline/definitions/uni_waiting_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/definitions/uni_worker_definition.py` & `unipipeline-1.8.9/unipipeline/definitions/uni_worker_definition.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/errors.py` & `unipipeline-1.8.9/unipipeline/errors.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/message_meta/uni_message_meta.py` & `unipipeline-1.8.9/unipipeline/message_meta/uni_message_meta.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/modules/uni.py` & `unipipeline-1.8.9/unipipeline/modules/uni.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/modules/uni_cron_job.py` & `unipipeline-1.8.9/unipipeline/modules/uni_cron_job.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/modules/uni_mediator.py` & `unipipeline-1.8.9/unipipeline/modules/uni_mediator.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/run.py` & `unipipeline-1.8.9/unipipeline/run.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/utils/complex_serializer.py` & `unipipeline-1.8.9/unipipeline/utils/complex_serializer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/utils/sig.py` & `unipipeline-1.8.9/unipipeline/utils/sig.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/utils/uni_echo.py` & `unipipeline-1.8.9/unipipeline/utils/uni_echo.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/utils/uni_util_color.py` & `unipipeline-1.8.9/unipipeline/utils/uni_util_color.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/utils/uni_util_template.py` & `unipipeline-1.8.9/unipipeline/utils/uni_util_template.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/waiting/uni_postgres_waiting.py` & `unipipeline-1.8.9/unipipeline/waiting/uni_postgres_waiting.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/worker/uni_msg_params.py` & `unipipeline-1.8.9/unipipeline/worker/uni_msg_params.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/worker/uni_worker.py` & `unipipeline-1.8.9/unipipeline/worker/uni_worker.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/worker/uni_worker_consumer.py` & `unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/worker/uni_worker_consumer_manager.py` & `unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_manager.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline/worker/uni_worker_consumer_message.py` & `unipipeline-1.8.9/unipipeline/worker/uni_worker_consumer_message.py`

 * *Files identical despite different names*

### Comparing `unipipeline-1.8.7/unipipeline.egg-info/PKG-INFO` & `unipipeline-1.8.9/unipipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unipipeline
-Version: 1.8.7
+Version: 1.8.9
 Summary: simple way to build the declarative and distributed data pipelines with python. it supports rabbitmq or kafka as a broker
 Home-page: https://github.com/aliaksandr-master/unipipeline
 Author: Aliaksandr Master
 Author-email: alxe.master@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `unipipeline-1.8.7/unipipeline.egg-info/SOURCES.txt` & `unipipeline-1.8.9/unipipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

