# Comparing `tmp/tungstenkit-0.0.1a4.tar.gz` & `tmp/tungstenkit-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tungstenkit-0.0.1a4.tar", max compression
+gzip compressed data, was "tungstenkit-0.0.1a5.tar", max compression
```

## Comparing `tungstenkit-0.0.1a4.tar` & `tungstenkit-0.0.1a5.tar`

### file list

```diff
@@ -1,161 +1,161 @@
--rw-r--r--   0        0        0     4188 2023-04-28 21:51:41.640810 tungstenkit-0.0.1a4/README.md
--rw-r--r--   0        0        0     3063 2023-04-28 21:55:52.190179 tungstenkit-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-12 05:26:24.578907 tungstenkit-0.0.1a4/tungstenkit/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 11:27:04.215980 tungstenkit-0.0.1a4/tungstenkit/_internal/__init__.py
--rw-r--r--   0        0        0       58 2023-02-07 06:53:27.734918 tungstenkit-0.0.1a4/tungstenkit/_internal/build/__init__.py
--rw-r--r--   0        0        0    13058 2023-04-28 18:27:19.471277 tungstenkit-0.0.1a4/tungstenkit/_internal/build/build_context.py
--rw-r--r--   0        0        0      223 2023-04-24 16:30:27.472608 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/__init__.py
--rw-r--r--   0        0        0     6665 2023-04-25 22:04:09.248549 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_dockerfile.py
--rw-r--r--   0        0        0      385 2023-02-10 06:16:31.369855 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/__init__.py
--rw-r--r--   0        0        0      483 2023-04-03 17:09:07.281170 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/base_image.py
--rw-r--r--   0        0        0      238 2023-02-03 13:23:06.852208 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/conda_image.py
--rw-r--r--   0        0        0     2552 2023-04-25 15:45:06.334442 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py
--rw-r--r--   0        0        0      369 2023-02-03 13:23:05.848222 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/custom_image.py
--rw-r--r--   0        0        0     1622 2023-04-25 15:45:09.366456 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/python_image.py
--rw-r--r--   0        0        0      574 2023-04-03 17:26:01.449366 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/shared.py
--rw-r--r--   0        0        0      652 2023-04-25 18:28:28.772596 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/model_dockerfile.py
--rw-r--r--   0        0        0     7737 2023-04-26 09:30:54.665084 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/__init__.py
--rw-r--r--   0        0        0     1008 2023-04-03 17:26:01.453366 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py
--rw-r--r--   0        0        0     3604 2023-03-17 13:39:39.007137 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py
--rw-r--r--   0        0        0     1593 2023-04-03 17:26:01.453366 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py
--rw-r--r--   0        0        0     4315 2023-04-25 16:00:10.821612 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py
--rw-r--r--   0        0        0     6509 2023-04-25 16:00:24.149556 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py
--rw-r--r--   0        0        0      723 2023-03-02 10:07:30.852064 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py
--rw-r--r--   0        0        0      924 2023-04-03 13:59:33.174626 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py
--rw-r--r--   0        0        0      257 2023-04-24 16:30:30.360576 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/task_dockerfile_writer.py
--rw-r--r--   0        0        0     1373 2023-04-03 17:26:01.465366 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/template_args.py
--rw-r--r--   0        0        0      345 2023-02-12 21:59:14.371233 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/base.j2
--rw-r--r--   0        0        0      951 2023-02-12 17:14:40.197221 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2
--rw-r--r--   0        0        0      834 2023-03-21 06:01:49.179458 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/install_python.j2
--rw-r--r--   0        0        0      824 2023-04-05 13:37:23.666139 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2
--rw-r--r--   0        0        0     1905 2023-04-05 14:02:38.279713 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2
--rw-r--r--   0        0        0     1218 2023-04-28 21:55:56.382137 tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml
--rw-r--r--   0        0        0     2152 2023-04-28 17:49:52.968551 tungstenkit-0.0.1a4/tungstenkit/_internal/build/model.py
--rw-r--r--   0        0        0        0 2023-02-13 09:01:23.964824 tungstenkit-0.0.1a4/tungstenkit/_internal/cli/__init__.py
--rw-r--r--   0        0        0     2653 2023-04-25 17:53:42.896244 tungstenkit-0.0.1a4/tungstenkit/_internal/cli/callbacks.py
--rw-r--r--   0        0        0     2280 2023-04-28 12:06:18.125313 tungstenkit-0.0.1a4/tungstenkit/_internal/cli/login_command.py
--rw-r--r--   0        0        0     1428 2023-04-25 16:20:56.732517 tungstenkit-0.0.1a4/tungstenkit/_internal/cli/main.py
--rw-r--r--   0        0        0    12392 2023-04-28 17:51:02.888358 tungstenkit-0.0.1a4/tungstenkit/_internal/cli/model_commands.py
--rw-r--r--   0        0        0      653 2023-04-25 16:20:49.040623 tungstenkit-0.0.1a4/tungstenkit/_internal/cli/options.py
--rw-r--r--   0        0        0      144 2023-04-10 05:38:12.075265 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/__init__.py
--rw-r--r--   0        0        0      146 2023-02-09 07:22:19.492062 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/__init__.py
--rw-r--r--   0        0        0      565 2023-04-25 12:02:57.458961 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/__init__.py
--rw-r--r--   0        0        0       78 2023-03-14 12:22:52.854155 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/common.py
--rw-r--r--   0        0        0       97 2023-02-09 03:17:21.967897 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/datapoint.py
--rw-r--r--   0        0        0      423 2023-02-13 06:50:50.484042 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/dataset.py
--rw-r--r--   0        0        0      124 2023-04-25 12:02:57.474961 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/instance.py
--rw-r--r--   0        0        0     1138 2023-04-26 10:04:16.305870 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/model.py
--rw-r--r--   0        0        0      101 2023-02-13 06:51:09.771865 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/namespace.py
--rw-r--r--   0        0        0      174 2023-03-14 12:23:08.698032 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/project.py
--rw-r--r--   0        0        0      698 2023-04-12 06:34:07.841749 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/storage.py
--rw-r--r--   0        0        0       85 2023-02-09 04:53:43.633954 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/token.py
--rw-r--r--   0        0        0      256 2023-02-13 06:51:15.491812 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/user.py
--rw-r--r--   0        0        0    16927 2023-04-26 10:05:16.953589 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py
--rw-r--r--   0        0        0     9376 2023-04-27 06:50:07.991992 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/tungsten_client.py
--rw-r--r--   0        0        0      178 2023-04-10 05:38:12.075265 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/__init__.py
--rw-r--r--   0        0        0      574 2023-04-10 05:38:12.075265 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/schemas.py
--rw-r--r--   0        0        0     4453 2023-04-24 08:06:41.328580 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py
--rw-r--r--   0        0        0     4000 2023-04-10 06:02:24.420686 tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py
--rw-r--r--   0        0        0     4074 2023-04-28 18:30:37.365234 tungstenkit-0.0.1a4/tungstenkit/_internal/configs.py
--rw-r--r--   0        0        0     2111 2023-04-28 14:15:17.428906 tungstenkit-0.0.1a4/tungstenkit/_internal/constants.py
--rw-r--r--   0        0        0     4887 2023-04-26 13:57:54.276814 tungstenkit-0.0.1a4/tungstenkit/_internal/containerized_services.py
--rw-r--r--   0        0        0      132 2023-04-27 06:50:07.991992 tungstenkit-0.0.1a4/tungstenkit/_internal/contexts.py
--rw-r--r--   0        0        0     9936 2023-04-28 17:02:36.105097 tungstenkit-0.0.1a4/tungstenkit/_internal/io.py
--rw-r--r--   0        0        0     6498 2023-04-12 05:26:24.578907 tungstenkit-0.0.1a4/tungstenkit/_internal/io_schema.py
--rw-r--r--   0        0        0       94 2023-04-07 07:59:05.613312 tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/__init__.py
--rw-r--r--   0        0        0     6745 2023-04-25 14:42:36.889081 tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_blob_store.py
--rw-r--r--   0        0        0     9003 2023-04-26 09:39:05.108000 tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_model.py
--rw-r--r--   0        0        0    14814 2023-04-26 09:37:49.508733 tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_model_store.py
--rw-r--r--   0        0        0     3014 2023-04-25 18:01:07.563193 tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_store.py
--rw-r--r--   0        0        0     2955 2023-04-25 17:48:40.214249 tungstenkit-0.0.1a4/tungstenkit/_internal/logging.py
--rw-r--r--   0        0        0    10513 2023-04-28 18:08:32.747439 tungstenkit-0.0.1a4/tungstenkit/_internal/model.py
--rw-r--r--   0        0        0        0 2023-02-14 13:15:15.626409 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/__init__.py
--rw-r--r--   0        0        0       67 2023-01-30 10:16:13.468188 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/__init__.py
--rw-r--r--   0        0        0     5083 2023-04-27 06:50:07.991992 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/404.html
--rw-r--r--   0        0        0      401 2023-04-27 06:50:07.995992 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_buildManifest.js
--rw-r--r--   0        0        0       77 2023-04-27 06:50:07.995992 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_ssgManifest.js
--rw-r--r--   0        0        0  1564405 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js
--rw-r--r--   0        0        0    78390 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js
--rw-r--r--   0        0        0   452205 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js
--rw-r--r--   0        0        0   141074 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js
--rw-r--r--   0        0        0    90428 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js
--rw-r--r--   0        0        0   142467 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js
--rw-r--r--   0        0        0      250 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
--rw-r--r--   0        0        0    32188 2023-04-27 06:50:07.995992 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js
--rw-r--r--   0        0        0    91460 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
--rw-r--r--   0        0        0     3853 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js
--rw-r--r--   0        0        0     1914 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css
--rw-r--r--   0        0        0    39283 2023-04-26 10:13:28.758764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css
--rw-r--r--   0        0        0   256670 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico
--rw-r--r--   0        0        0    27067 2023-04-27 06:50:07.995992 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/index.html
--rw-r--r--   0        0        0     2956 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/logo.svg
--rw-r--r--   0        0        0     1375 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/next.svg
--rw-r--r--   0        0        0     1138 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg
--rw-r--r--   0        0        0    27505 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png
--rw-r--r--   0        0        0    18388 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png
--rw-r--r--   0        0        0      629 2023-04-26 10:13:28.762764 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg
--rw-r--r--   0        0        0     3255 2023-04-18 13:20:10.338766 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/schemas.py
--rw-r--r--   0        0        0     5725 2023-04-14 10:49:02.037984 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/server.py
--rw-r--r--   0        0        0      156 2023-04-10 05:38:12.075265 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/__init__.py
--rw-r--r--   0        0        0     7170 2023-04-18 13:20:10.338766 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/example_service.py
--rw-r--r--   0        0        0     5594 2023-04-13 14:22:32.794579 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/file_service.py
--rw-r--r--   0        0        0    12106 2023-04-13 17:06:12.849464 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/prediction_service.py
--rw-r--r--   0        0        0        0 2022-12-02 07:28:29.250316 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/__init__.py
--rw-r--r--   0        0        0       32 2023-04-25 18:27:55.560955 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/__main__.py
--rw-r--r--   0        0        0     2885 2023-04-27 07:09:08.014172 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/cli.py
--rw-r--r--   0        0        0     3546 2023-04-25 18:25:38.462452 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/config.py
--rw-r--r--   0        0        0      144 2023-04-10 05:38:12.075265 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/enums.py
--rw-r--r--   0        0        0       70 2023-01-15 09:23:17.905346 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/event_buses/__init__.py
--rw-r--r--   0        0        0      772 2023-03-07 08:48:11.104474 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py
--rw-r--r--   0        0        0      125 2023-01-15 09:06:48.071148 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/event_buses/event.py
--rw-r--r--   0        0        0      337 2023-04-05 11:32:16.811393 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/event_buses/factory.py
--rw-r--r--   0        0        0      511 2023-03-07 08:48:11.104474 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/event_buses/local_event_bus.py
--rw-r--r--   0        0        0       78 2023-04-05 11:33:13.647015 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/__init__.py
--rw-r--r--   0        0        0      209 2023-04-05 08:24:39.049920 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/abstract_file_uploader.py
--rw-r--r--   0        0        0        7 2023-04-05 09:55:45.817798 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/azure_file_uploader.py
--rw-r--r--   0        0        0      602 2023-04-05 11:32:10.899432 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py
--rw-r--r--   0        0        0      675 2023-04-19 10:09:19.217932 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py
--rw-r--r--   0        0        0     1839 2023-04-24 08:15:46.317244 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py
--rw-r--r--   0        0        0        7 2023-04-05 09:55:48.669776 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/s3_file_uploader.py
--rw-r--r--   0        0        0        7 2023-02-13 05:39:52.330371 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/grpc_server.py
--rw-r--r--   0        0        0     5544 2023-04-28 15:16:56.731413 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/http_server.py
--rw-r--r--   0        0        0      563 2023-04-28 20:04:11.220512 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/ids.py
--rw-r--r--   0        0        0      184 2023-03-10 08:15:44.563699 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/__init__.py
--rw-r--r--   0        0        0      526 2023-03-10 10:28:34.439655 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py
--rw-r--r--   0        0        0      348 2023-04-05 11:32:19.263377 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/factory.py
--rw-r--r--   0        0        0     3215 2023-04-28 19:25:33.347431 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py
--rw-r--r--   0        0        0      131 2023-03-10 08:16:28.027487 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/shared.py
--rw-r--r--   0        0        0       69 2023-04-05 13:33:48.323591 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/prediction_worker/__init__.py
--rw-r--r--   0        0        0    11275 2023-04-25 15:44:35.290282 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py
--rw-r--r--   0        0        0     9827 2023-04-28 20:33:35.216347 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py
--rw-r--r--   0        0        0      248 2023-03-08 05:27:59.017205 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/__init__.py
--rw-r--r--   0        0        0     1487 2023-04-28 20:11:30.491234 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py
--rw-r--r--   0        0        0      396 2023-04-05 11:32:24.583341 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/factory.py
--rw-r--r--   0        0        0    10448 2023-04-28 20:12:34.854550 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py
--rw-r--r--   0        0        0      474 2023-03-23 09:39:52.133108 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/shared.py
--rw-r--r--   0        0        0     1365 2023-04-05 13:35:13.575019 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/schema.py
--rw-r--r--   0        0        0      503 2023-03-14 11:50:55.120955 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/server_exceptions.py
--rw-r--r--   0        0        0        0 2023-02-14 13:16:38.205743 tungstenkit-0.0.1a4/tungstenkit/_internal/servers/task_server/__init__.py
--rw-r--r--   0        0        0     9316 2023-02-13 09:03:58.840144 tungstenkit-0.0.1a4/tungstenkit/_internal/task.py
--rw-r--r--   0        0        0        0 2022-12-12 14:08:42.288364 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1472 2023-04-07 06:05:22.869660 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/avatar.py
--rw-r--r--   0        0        0     2996 2023-04-27 06:50:07.995992 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/console.py
--rw-r--r--   0        0        0      937 2023-04-25 14:56:13.508246 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/context.py
--rw-r--r--   0        0        0    15016 2023-04-27 06:50:07.995992 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/docker.py
--rw-r--r--   0        0        0     2068 2023-04-24 18:40:40.842492 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/file.py
--rw-r--r--   0        0        0     6213 2023-04-28 18:09:09.711232 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/imports.py
--rw-r--r--   0        0        0     1700 2023-04-19 12:12:54.181017 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/json.py
--rw-r--r--   0        0        0     2910 2023-04-13 17:16:31.352883 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/markdown.py
--rw-r--r--   0        0        0      551 2023-03-31 05:42:18.425644 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/pydantic.py
--rw-r--r--   0        0        0     1241 2023-04-25 17:26:28.359663 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/regex.py
--rw-r--r--   0        0        0    12774 2023-04-24 08:10:20.099223 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/requests.py
--rw-r--r--   0        0        0     2037 2023-03-21 12:04:05.879224 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/serialize.py
--rw-r--r--   0        0        0      676 2023-03-31 05:42:18.425644 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/string.py
--rw-r--r--   0        0        0      648 2023-02-13 07:53:40.261858 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/typing.py
--rw-r--r--   0        0        0     1946 2023-04-25 13:04:36.028376 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/uri.py
--rw-r--r--   0        0        0     6332 2023-04-25 15:44:54.098381 tungstenkit-0.0.1a4/tungstenkit/_internal/utils/version.py
--rw-r--r--   0        0        0      353 2023-02-13 09:02:21.976585 tungstenkit-0.0.1a4/tungstenkit/_versions.py
--rw-r--r--   0        0        0     2171 2023-04-25 16:13:58.553412 tungstenkit-0.0.1a4/tungstenkit/exceptions.py
--rw-r--r--   0        0        0      166 2023-04-28 17:02:17.929235 tungstenkit-0.0.1a4/tungstenkit/io.py
--rw-r--r--   0        0        0      171 2023-03-06 13:15:12.614188 tungstenkit-0.0.1a4/tungstenkit/model.py
--rw-r--r--   0        0        0     7284 1970-01-01 00:00:00.000000 tungstenkit-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     4086 2023-04-28 23:29:56.390539 tungstenkit-0.0.1a5/README.md
+-rw-r--r--   0        0        0     3063 2023-04-28 23:31:19.538575 tungstenkit-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-11 17:07:01.860571 tungstenkit-0.0.1a5/tungstenkit/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:48.957419 tungstenkit-0.0.1a5/tungstenkit/_internal/__init__.py
+-rw-r--r--   0        0        0       58 2023-02-17 08:39:48.957863 tungstenkit-0.0.1a5/tungstenkit/_internal/build/__init__.py
+-rw-r--r--   0        0        0    13058 2023-04-28 23:27:15.780413 tungstenkit-0.0.1a5/tungstenkit/_internal/build/build_context.py
+-rw-r--r--   0        0        0      223 2023-04-26 21:31:10.277468 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-26 21:31:10.277684 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_dockerfile.py
+-rw-r--r--   0        0        0      385 2023-02-17 08:39:48.959447 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-09 10:35:04.753993 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/base_image.py
+-rw-r--r--   0        0        0      238 2023-02-17 08:39:48.959971 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/conda_image.py
+-rw-r--r--   0        0        0     2552 2023-04-26 21:31:10.278022 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py
+-rw-r--r--   0        0        0      369 2023-02-17 08:39:48.960423 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/custom_image.py
+-rw-r--r--   0        0        0     1622 2023-04-26 21:31:10.278341 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/python_image.py
+-rw-r--r--   0        0        0      574 2023-04-09 10:35:04.754747 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/shared.py
+-rw-r--r--   0        0        0      652 2023-04-26 21:31:10.278501 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/model_dockerfile.py
+-rw-r--r--   0        0        0     7737 2023-04-26 21:31:10.278850 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/__init__.py
+-rw-r--r--   0        0        0     1008 2023-04-09 10:35:04.755489 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py
+-rw-r--r--   0        0        0     3604 2023-03-30 23:07:07.733066 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py
+-rw-r--r--   0        0        0     1593 2023-04-09 10:35:04.755732 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py
+-rw-r--r--   0        0        0     4315 2023-04-26 21:31:10.279190 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py
+-rw-r--r--   0        0        0     6509 2023-04-26 21:31:10.279501 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py
+-rw-r--r--   0        0        0      723 2023-02-17 08:39:48.962919 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py
+-rw-r--r--   0        0        0      924 2023-04-09 10:35:04.756528 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py
+-rw-r--r--   0        0        0      257 2023-04-26 21:31:10.279771 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/task_dockerfile_writer.py
+-rw-r--r--   0        0        0     1373 2023-04-09 10:35:04.757025 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/template_args.py
+-rw-r--r--   0        0        0      345 2023-02-17 08:39:48.964092 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/base.j2
+-rw-r--r--   0        0        0      951 2023-02-17 08:39:48.964269 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2
+-rw-r--r--   0        0        0      834 2023-03-30 23:07:07.735005 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_python.j2
+-rw-r--r--   0        0        0      824 2023-04-09 10:35:04.757393 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2
+-rw-r--r--   0        0        0     1905 2023-04-09 10:35:04.757672 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2
+-rw-r--r--   0        0        0     1218 2023-04-28 23:31:24.056305 tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml
+-rw-r--r--   0        0        0     2152 2023-04-26 21:31:10.280640 tungstenkit-0.0.1a5/tungstenkit/_internal/build/model.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:48.966251 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     2653 2023-04-26 21:31:10.280844 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/callbacks.py
+-rw-r--r--   0        0        0     2280 2023-04-28 23:27:15.781189 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/login_command.py
+-rw-r--r--   0        0        0     1428 2023-04-26 21:31:10.281426 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/main.py
+-rw-r--r--   0        0        0    12392 2023-04-28 23:27:15.782080 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/model_commands.py
+-rw-r--r--   0        0        0      653 2023-04-26 21:31:10.281918 tungstenkit-0.0.1a5/tungstenkit/_internal/cli/options.py
+-rw-r--r--   0        0        0      144 2023-04-09 22:57:33.217617 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/__init__.py
+-rw-r--r--   0        0        0      146 2023-04-09 10:35:04.759933 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/__init__.py
+-rw-r--r--   0        0        0      565 2023-04-26 21:31:10.282274 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/__init__.py
+-rw-r--r--   0        0        0       78 2023-04-09 10:35:04.760862 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/common.py
+-rw-r--r--   0        0        0       97 2023-04-09 10:35:04.761036 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/datapoint.py
+-rw-r--r--   0        0        0      423 2023-04-09 10:35:04.761184 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/dataset.py
+-rw-r--r--   0        0        0      124 2023-04-26 21:31:10.282618 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/instance.py
+-rw-r--r--   0        0        0     1138 2023-04-26 21:31:10.283727 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/model.py
+-rw-r--r--   0        0        0      101 2023-04-09 10:35:04.761619 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/namespace.py
+-rw-r--r--   0        0        0      174 2023-04-09 10:35:04.761763 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/project.py
+-rw-r--r--   0        0        0      698 2023-04-17 13:32:38.408872 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/storage.py
+-rw-r--r--   0        0        0       85 2023-04-09 10:35:04.762055 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/token.py
+-rw-r--r--   0        0        0      256 2023-04-09 10:35:04.762195 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/user.py
+-rw-r--r--   0        0        0    16927 2023-04-26 21:31:10.284175 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py
+-rw-r--r--   0        0        0     9376 2023-04-27 00:19:46.503001 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_client.py
+-rw-r--r--   0        0        0      178 2023-04-09 22:56:23.933893 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/__init__.py
+-rw-r--r--   0        0        0      574 2023-04-09 22:44:42.545013 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/schemas.py
+-rw-r--r--   0        0        0     4453 2023-04-26 21:31:10.285036 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py
+-rw-r--r--   0        0        0     4000 2023-04-11 16:43:31.229639 tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py
+-rw-r--r--   0        0        0     4074 2023-04-28 23:27:15.782456 tungstenkit-0.0.1a5/tungstenkit/_internal/configs.py
+-rw-r--r--   0        0        0     2111 2023-04-28 23:27:15.782804 tungstenkit-0.0.1a5/tungstenkit/_internal/constants.py
+-rw-r--r--   0        0        0     4887 2023-04-26 21:31:10.286049 tungstenkit-0.0.1a5/tungstenkit/_internal/containerized_services.py
+-rw-r--r--   0        0        0      132 2023-04-26 22:02:15.494035 tungstenkit-0.0.1a5/tungstenkit/_internal/contexts.py
+-rw-r--r--   0        0        0     9936 2023-04-28 23:27:15.784185 tungstenkit-0.0.1a5/tungstenkit/_internal/io.py
+-rw-r--r--   0        0        0     6498 2023-04-11 17:20:16.148322 tungstenkit-0.0.1a5/tungstenkit/_internal/io_schema.py
+-rw-r--r--   0        0        0       94 2023-04-09 10:35:04.764738 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/__init__.py
+-rw-r--r--   0        0        0     6745 2023-04-26 21:31:10.287336 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_blob_store.py
+-rw-r--r--   0        0        0     9003 2023-04-26 21:31:10.287658 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model.py
+-rw-r--r--   0        0        0    14814 2023-04-26 21:31:10.288022 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model_store.py
+-rw-r--r--   0        0        0     3014 2023-04-26 21:31:10.288307 tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_store.py
+-rw-r--r--   0        0        0     2955 2023-04-26 23:19:48.588616 tungstenkit-0.0.1a5/tungstenkit/_internal/logging.py
+-rw-r--r--   0        0        0    10513 2023-04-28 23:27:15.785158 tungstenkit-0.0.1a5/tungstenkit/_internal/model.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.007358 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/__init__.py
+-rw-r--r--   0        0        0       67 2023-03-06 16:17:19.313885 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/__init__.py
+-rw-r--r--   0        0        0     5083 2023-04-26 21:40:01.486422 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/404.html
+-rw-r--r--   0        0        0      401 2023-04-26 21:40:00.038750 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_buildManifest.js
+-rw-r--r--   0        0        0       77 2023-04-26 21:40:00.038529 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/9J0J94uaBN6r2ZngrgX1w/_ssgManifest.js
+-rw-r--r--   0        0        0  1564405 2023-04-26 21:40:00.044383 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js
+-rw-r--r--   0        0        0    78390 2023-04-26 21:40:00.039266 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js
+-rw-r--r--   0        0        0   452205 2023-04-26 21:40:00.041443 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js
+-rw-r--r--   0        0        0   141074 2023-04-26 21:40:00.039764 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js
+-rw-r--r--   0        0        0    90428 2023-04-26 21:40:00.041155 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js
+-rw-r--r--   0        0        0   142467 2023-04-26 21:40:00.042918 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js
+-rw-r--r--   0        0        0      250 2023-04-26 21:40:00.042591 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_error-3f6d1c55bb8051ab.js
+-rw-r--r--   0        0        0    32188 2023-04-26 21:40:00.042788 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js
+-rw-r--r--   0        0        0    91460 2023-04-26 21:40:00.040708 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0        0        0     3853 2023-04-26 21:40:00.041574 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js
+-rw-r--r--   0        0        0     1914 2023-04-26 21:40:00.041630 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css
+-rw-r--r--   0        0        0    39283 2023-04-26 21:40:00.042000 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css
+-rw-r--r--   0        0        0   256670 2023-04-26 21:40:00.061924 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico
+-rw-r--r--   0        0        0    27067 2023-04-26 21:40:01.469688 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/index.html
+-rw-r--r--   0        0        0     2956 2023-04-26 21:40:00.060165 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/logo.svg
+-rw-r--r--   0        0        0     1375 2023-04-26 21:40:00.060165 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/next.svg
+-rw-r--r--   0        0        0     1138 2023-04-26 21:40:00.060279 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg
+-rw-r--r--   0        0        0    27505 2023-04-26 21:40:00.060754 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png
+-rw-r--r--   0        0        0    18388 2023-04-26 21:40:00.060785 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png
+-rw-r--r--   0        0        0      629 2023-04-26 21:40:00.060638 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg
+-rw-r--r--   0        0        0     3255 2023-04-18 14:30:25.906560 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/schemas.py
+-rw-r--r--   0        0        0     5725 2023-04-17 13:32:38.450673 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/server.py
+-rw-r--r--   0        0        0      156 2023-04-10 03:44:40.979762 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/__init__.py
+-rw-r--r--   0        0        0     7170 2023-04-18 14:30:25.907462 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/example_service.py
+-rw-r--r--   0        0        0     5594 2023-04-17 13:32:38.451856 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/file_service.py
+-rw-r--r--   0        0        0    12106 2023-04-17 13:32:38.452749 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/prediction_service.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.007650 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-26 21:31:10.290945 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/__main__.py
+-rw-r--r--   0        0        0     2885 2023-04-28 03:17:20.449371 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/cli.py
+-rw-r--r--   0        0        0     3546 2023-04-26 21:31:10.291554 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/config.py
+-rw-r--r--   0        0        0      144 2023-04-09 18:07:13.836271 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/enums.py
+-rw-r--r--   0        0        0       70 2023-04-09 10:35:04.768748 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/__init__.py
+-rw-r--r--   0        0        0      772 2023-04-09 10:35:04.768945 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py
+-rw-r--r--   0        0        0      125 2023-04-09 10:35:04.769155 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/event.py
+-rw-r--r--   0        0        0      337 2023-04-09 18:14:24.800665 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/factory.py
+-rw-r--r--   0        0        0      511 2023-04-09 10:35:04.769485 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/local_event_bus.py
+-rw-r--r--   0        0        0       78 2023-04-09 10:35:04.769721 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/__init__.py
+-rw-r--r--   0        0        0      209 2023-04-09 10:35:04.769876 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/abstract_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-04-09 10:35:04.770021 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/azure_file_uploader.py
+-rw-r--r--   0        0        0      602 2023-04-09 10:35:04.770162 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py
+-rw-r--r--   0        0        0      675 2023-04-26 21:31:10.292540 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py
+-rw-r--r--   0        0        0     1839 2023-04-26 21:31:10.292849 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-04-09 10:35:04.770768 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/s3_file_uploader.py
+-rw-r--r--   0        0        0        7 2023-02-17 08:39:49.008624 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/grpc_server.py
+-rw-r--r--   0        0        0     5544 2023-04-26 21:31:10.293182 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/http_server.py
+-rw-r--r--   0        0        0      563 2023-04-28 23:27:15.786706 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/ids.py
+-rw-r--r--   0        0        0      184 2023-04-09 10:35:04.771472 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/__init__.py
+-rw-r--r--   0        0        0      526 2023-04-09 10:35:04.771700 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py
+-rw-r--r--   0        0        0      348 2023-04-09 18:14:24.863856 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/factory.py
+-rw-r--r--   0        0        0     3215 2023-04-28 23:27:15.787098 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py
+-rw-r--r--   0        0        0      131 2023-04-09 10:35:04.772211 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/shared.py
+-rw-r--r--   0        0        0       69 2023-04-09 10:35:04.772454 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/__init__.py
+-rw-r--r--   0        0        0    11275 2023-04-26 22:31:57.812867 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py
+-rw-r--r--   0        0        0     9827 2023-04-28 23:27:15.787490 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py
+-rw-r--r--   0        0        0      248 2023-04-09 10:35:04.773162 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/__init__.py
+-rw-r--r--   0        0        0     1487 2023-04-28 23:27:15.788210 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py
+-rw-r--r--   0        0        0      396 2023-04-09 18:14:24.863983 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/factory.py
+-rw-r--r--   0        0        0    10448 2023-04-28 23:27:15.788639 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py
+-rw-r--r--   0        0        0      474 2023-04-09 10:35:04.774049 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/shared.py
+-rw-r--r--   0        0        0     1365 2023-04-09 10:35:04.774342 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/schema.py
+-rw-r--r--   0        0        0      503 2023-03-15 00:25:51.895356 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/server_exceptions.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.016050 tungstenkit-0.0.1a5/tungstenkit/_internal/servers/task_server/__init__.py
+-rw-r--r--   0        0        0     9316 2023-02-17 08:39:49.016381 tungstenkit-0.0.1a5/tungstenkit/_internal/task.py
+-rw-r--r--   0        0        0        0 2023-02-17 08:39:49.019727 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1472 2023-04-09 10:35:04.774544 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/avatar.py
+-rw-r--r--   0        0        0     2996 2023-04-26 23:35:59.492013 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/console.py
+-rw-r--r--   0        0        0      937 2023-04-26 21:31:10.295291 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/context.py
+-rw-r--r--   0        0        0    15016 2023-04-26 23:33:26.063956 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/docker.py
+-rw-r--r--   0        0        0     2068 2023-04-26 21:31:10.295914 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/file.py
+-rw-r--r--   0        0        0     6213 2023-04-28 23:27:15.789532 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/imports.py
+-rw-r--r--   0        0        0     1700 2023-04-17 13:32:38.460136 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/json.py
+-rw-r--r--   0        0        0     2910 2023-04-17 13:32:38.461086 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/markdown.py
+-rw-r--r--   0        0        0      551 2023-03-31 00:24:18.313560 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/pydantic.py
+-rw-r--r--   0        0        0     1241 2023-04-26 21:31:10.296085 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/regex.py
+-rw-r--r--   0        0        0    12774 2023-04-26 21:31:10.296375 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/requests.py
+-rw-r--r--   0        0        0     2037 2023-03-30 23:07:07.750471 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/serialize.py
+-rw-r--r--   0        0        0      676 2023-03-31 00:17:55.349782 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/string.py
+-rw-r--r--   0        0        0      648 2023-02-17 08:39:49.021077 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/typing.py
+-rw-r--r--   0        0        0     1946 2023-04-26 21:31:10.296913 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/uri.py
+-rw-r--r--   0        0        0     6332 2023-04-26 21:31:10.297213 tungstenkit-0.0.1a5/tungstenkit/_internal/utils/version.py
+-rw-r--r--   0        0        0      353 2023-02-17 08:39:49.021416 tungstenkit-0.0.1a5/tungstenkit/_versions.py
+-rw-r--r--   0        0        0     2171 2023-04-26 21:31:10.297501 tungstenkit-0.0.1a5/tungstenkit/exceptions.py
+-rw-r--r--   0        0        0      166 2023-04-28 23:27:15.790414 tungstenkit-0.0.1a5/tungstenkit/io.py
+-rw-r--r--   0        0        0      171 2023-02-17 08:39:49.021956 tungstenkit-0.0.1a5/tungstenkit/model.py
+-rw-r--r--   0        0        0     7182 1970-01-01 00:00:00.000000 tungstenkit-0.0.1a5/PKG-INFO
```

### Comparing `tungstenkit-0.0.1a4/README.md` & `tungstenkit-0.0.1a5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Tungstenkit
-**Tungstenkit** is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models. The key features of Tungsten models are:
+**Tungstenkit** is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models. Key features of Tungsten models are:
 
 - **Easy**: [Require only a few lines of Python code.](#build-a-tungsten-model)
 - **Versatile**: Support multiple usages:
     - [RESTful API server](#run-it-as-a-restful-api-server)
     - [GUI application](#run-it-as-a-gui-application)
     - [Serverless function](#run-it-as-a-serverless-function)
     - CLI application (coming soon)
@@ -124,14 +124,14 @@
 
 ![tungsten-platform-model-demo](https://github.com/tungsten-ai/assets/blob/main/common/platform-model-demo.gif?raw=true "Tungsten Platform Model Demo")
 
 
 # Prerequisites
 - Python 3.7+
 - [Docker](https://docs.docker.com/engine/install/)
-- (Optional) [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker) for running GPU models locally. It enables using GPUs in Docker containers. However, you can build and push GPU models without it.
+- (Optional) [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker) for running GPU models locally. 
 
 
 # Installation
 ```shell
 pip install tungstenkit
 ```
```

### Comparing `tungstenkit-0.0.1a4/pyproject.toml` & `tungstenkit-0.0.1a5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.0.1a4"
+version = "0.0.1a5"
 description = "Tungstenkit is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models."
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://tungsten-ai.github.io/docs"
 readme = ["README.md"]
 packages = [{include = "tungstenkit"}]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/build_context.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/build_context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_dockerfile.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/cuda_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/python_image.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/python_image.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/base_images/shared.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/base_images/shared.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/model_dockerfile.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/model_dockerfile.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/__init__.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/base_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/common.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/tf_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/gpu_packages/torch_collection.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/pip_requirement.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/python/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/template_args.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/template_args.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_conda.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/install_python.j2` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/install_python.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_tungsten.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/templates/setup_user.j2`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/dockerfile/tungstenkit/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tungstenkit"
-version = "0.0.1a4"
+version = "0.0.1a5"
 description = "Tungstenkit is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models."
 authors = ["Tungsten Contributors <foss@tungsten-ai.com>"]
 homepage = "https://tungsten-ai.github.io/docs"
 packages = [{include = "tungstenkit"}]
 
 [tool.poetry.scripts]
 tungsten = "tungstenkit._internal.cli.main:main"
```

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/build/model.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/build/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/cli/callbacks.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/callbacks.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/cli/login_command.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/login_command.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/cli/main.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/cli/model_commands.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/model_commands.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/cli/options.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/cli/options.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/__init__.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/model.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/schemas/storage.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/schemas/storage.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten/tungsten_client.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten/tungsten_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/schemas.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_api_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/clients/tungsten_model/tungsten_model_client.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/configs.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/configs.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/constants.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/containerized_services.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/containerized_services.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/io.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/io.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/io_schema.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/io_schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_blob_store.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_blob_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_model.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_model_store.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_model_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/local_store/local_store.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/local_store/local_store.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/logging.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/logging.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/model.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/model.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/404.html` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/404.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/370-54e89ea530a46e74.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/925e0f50.7ec97e0b40c95885.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/d6e1aeb5-bf16fef9f0637571.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/framework-73b8966a3c579ab0.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/main-6260d066cf2cd7b1.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/_app-a5d327f8245a7cb7.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/pages/index-d22c2e2ad4a0676a.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/chunks/webpack-b98be2d55f37c35c.js`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/6c93262152699231.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/_next/static/css/e19e5222d7a223c1.css`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/index.html` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/index.html`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/logo.svg` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/logo.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/next.svg` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/next.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/thirteen.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungstenWithoutText.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/tungsten_greyed_out_logo.png`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/frontend/vercel.svg`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/schemas.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/schemas.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/server.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/example_service.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/example_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/file_service.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/file_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/demo_server/services/prediction_service.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/demo_server/services/prediction_service.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/cli.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/cli.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/config.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/config.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/event_buses/abstract_event_bus.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/factory.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/in_memory_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/file_uploaders/local_fs_file_uploader.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/http_server.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/http_server.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/ids.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/ids.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/abstract_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/input_queues/local_input_queue.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/subproc.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/prediction_worker/worker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/abstract_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/result_caches/local_result_cache.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/servers/model_server/schema.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/servers/model_server/schema.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/task.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/task.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/avatar.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/console.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/console.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/context.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/docker.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/docker.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/file.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/file.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/imports.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/imports.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/json.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/json.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/markdown.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/markdown.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/pydantic.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/regex.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/regex.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/requests.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/requests.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/serialize.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/serialize.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/string.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/string.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/typing.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/typing.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/uri.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/uri.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/_internal/utils/version.py` & `tungstenkit-0.0.1a5/tungstenkit/_internal/utils/version.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/tungstenkit/exceptions.py` & `tungstenkit-0.0.1a5/tungstenkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tungstenkit-0.0.1a4/PKG-INFO` & `tungstenkit-0.0.1a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tungstenkit
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Tungstenkit is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models.
 Home-page: https://tungsten-ai.github.io/docs
 Author: Tungsten Contributors
 Author-email: foss@tungsten-ai.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -64,15 +64,15 @@
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Requires-Dist: uvicorn (>=0.17.6,<1.0.0)
 Requires-Dist: w3lib (>=2.1.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Tungstenkit
-**Tungstenkit** is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models. The key features of Tungsten models are:
+**Tungstenkit** is an open-source tool for building and using versatile and standardized ML model containers, Tungsten models. Key features of Tungsten models are:
 
 - **Easy**: [Require only a few lines of Python code.](#build-a-tungsten-model)
 - **Versatile**: Support multiple usages:
     - [RESTful API server](#run-it-as-a-restful-api-server)
     - [GUI application](#run-it-as-a-gui-application)
     - [Serverless function](#run-it-as-a-serverless-function)
     - CLI application (coming soon)
@@ -193,14 +193,14 @@
 
 ![tungsten-platform-model-demo](https://github.com/tungsten-ai/assets/blob/main/common/platform-model-demo.gif?raw=true "Tungsten Platform Model Demo")
 
 
 # Prerequisites
 - Python 3.7+
 - [Docker](https://docs.docker.com/engine/install/)
-- (Optional) [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker) for running GPU models locally. It enables using GPUs in Docker containers. However, you can build and push GPU models without it.
+- (Optional) [nvidia-docker](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker) for running GPU models locally. 
 
 
 # Installation
 ```shell
 pip install tungstenkit
 ```
```

