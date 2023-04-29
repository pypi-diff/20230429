# Comparing `tmp/netconf_tool-0.0.1.tar.gz` & `tmp/netconf_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netconf_tool-0.0.1.tar", last modified: Fri Apr 28 22:33:31 2023, max compression
+gzip compressed data, was "netconf_tool-0.0.2.tar", last modified: Sat Apr 29 18:06:22 2023, max compression
```

## Comparing `netconf_tool-0.0.1.tar` & `netconf_tool-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:33:31.210150 netconf_tool-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-28 22:33:31.210150 netconf_tool-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-28 22:33:13.000000 netconf_tool-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:33:31.210150 netconf_tool-0.0.1/netconf_tool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:33:13.000000 netconf_tool-0.0.1/netconf_tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-28 22:33:13.000000 netconf_tool-0.0.1/netconf_tool/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-28 22:33:13.000000 netconf_tool-0.0.1/netconf_tool/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 22:33:13.000000 netconf_tool-0.0.1/netconf_tool/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:33:31.210150 netconf_tool-0.0.1/netconf_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-28 22:33:31.000000 netconf_tool-0.0.1/netconf_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-28 22:33:31.000000 netconf_tool-0.0.1/netconf_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:33:31.000000 netconf_tool-0.0.1/netconf_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 22:33:31.000000 netconf_tool-0.0.1/netconf_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 22:33:31.000000 netconf_tool-0.0.1/netconf_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 22:33:31.000000 netconf_tool-0.0.1/netconf_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:33:31.210150 netconf_tool-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-28 22:33:13.000000 netconf_tool-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.193682 netconf_tool-0.0.2/netconf_tool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/operations/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/operations/get_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool/subscription/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/subscription/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool/yangcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/yangcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/netconf_tool/yangcli/get_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/netconf_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12920 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-29 18:06:22.000000 netconf_tool-0.0.2/netconf_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:06:22.197682 netconf_tool-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-29 18:06:05.000000 netconf_tool-0.0.2/setup.py
```

### Comparing `netconf_tool-0.0.1/netconf_tool/cli.py` & `netconf_tool-0.0.2/netconf_tool/subscription/rabbitmq.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,88 @@
 import click
-import json
-from pkg_resources import iter_entry_points
-from click_plugins import with_plugins
+import pika
+from pika.exceptions import AMQPConnectionError
+from loguru import logger
 from ncclient import manager
 from ncclient.transport.errors import SSHError, AuthenticationError
-from loguru import logger
-
-from netconf_tool.decorators import netconf_common_options
-from netconf_tool.helpers import parse_rfc3986_uri
+from netconf_tool.subscription import netconf_tool_cli_subscription
+from netconf_tool.decorators import common_netconf_options
 
 
-@with_plugins(iter_entry_points("netconf_tool.plugins"))
-@click.group()
-def cli():
-    """CLI Application with plugin based architecture to interact with NETCONF Servers"""
-
-
-@cli.command("list-server-capabilities")
+@netconf_tool_cli_subscription.command("rabbitmq")
+@common_netconf_options
+@click.option(
+    "--rabbitmq-host",
+    help="RabbitMQ Server to connect to",
+    type=str,
+    default="127.0.0.1",
+)
+@click.option(
+    "--rabbitmq-port", help="Port for RabbitMQ server", type=int, default=5672
+)
+@click.option(
+    "--rabbitmq-queue",
+    help="RabbitMQ Queue to create",
+    type=str,
+    default="netconf_tool",
+)
+@click.option("--rabbitmq-exchange", help="RabbitMQ Exchange", type=str, default="")
+@click.option(
+    "--rabbitmq-routing-key",
+    help="RabbitMQ Routing Key",
+    type=str,
+    default="all_events",
+)
+@click.option(
+    "--rabbitmq-username",
+    help="Username to authenticate if authentication is used",
+    type=str,
+)
 @click.option(
-    "--export-json",
-    help="Export server capabilities into RFC3986 compliant URIs into a JSON file",
+    "--rabbitmq-password",
+    help="Password to authenticate if authentication is used",
     type=str,
 )
-@netconf_common_options
-def cli_list_server_capabilities(
+def cli_subscription_rabbitmq(
     host: str,
     port: int,
     username: str,
     password: str,
     device_handler: str,
     hostkey_verify: bool,
-    export_json: str,
+    rabbitmq_host: str,
+    rabbitmq_port: int,
+    rabbitmq_queue: str,
+    rabbitmq_exchange: str,
+    rabbitmq_routing_key: str,
+    rabbitmq_username: str,
+    rabbitmq_password: str,
 ):
-    """Print or Export all NETCONF Server capabilities"""
-    logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
-    try:
-        with manager.connect(
-            host=host,
-            port=port,
-            username=username,
-            password=password,
-            device_params={"name": device_handler},
-            hostkey_verify=hostkey_verify,
-        ) as m:
-            logger.success(
-                f"Established NETCONF connection to {host}:{port} (Session ID: {m.session_id})"
-            )
-            server_capabilities = m.server_capabilities
-            if not export_json:
-                for capability in server_capabilities:
-                    print(capability)
-                exit()
-
-            capabilities = []
-            for capability in server_capabilities:
-                capability = parse_rfc3986_uri(uri=capability)
-                capabilities.append(capability)
+    """Create a local event listener using <create-subscription> and redirect to a rabbitmq host"""
+    parameters = pika.ConnectionParameters(rabbitmq_host, rabbitmq_port, "/")
 
-            logger.info(
-                f"Exporting {len(capabilities)} capabilities to JSON file: {export_json}"
-            )
-            with open(export_json, "w") as out_file:
-                json.dump(capabilities, out_file, indent=4)
-    except SSHError as err:
-        logger.error(err)
-    except AuthenticationError as err:
-        logger.error("Unable to authenticate to NETCONF server")
-    except Exception as err:
-        logger.error(f"Generic Exception caught: {err}")
+    if rabbitmq_username and rabbitmq_password:
+        parameters.credentials = pika.PlainCredentials(
+            rabbitmq_username, rabbitmq_password
+        )
 
+    try:
+        connection = pika.BlockingConnection()
+    except AMQPConnectionError as err:
+        logger.error(
+            f"Unable to establish connection to RabbitMQ server {rabbitmq_host}:{rabbitmq_password}"
+        )
+        exit()
+    channel = connection.channel()
+    channel.queue_declare(queue=rabbitmq_queue)
+
+    logger.info(
+        f"Checking if RabbitMQ Server {rabbitmq_host}:{rabbitmq_port} is available"
+    )
 
-@cli.command("create-subscription")
-@netconf_common_options
-def cli_create_subscription(
-    host: str,
-    port: int,
-    username: str,
-    password: str,
-    device_handler: str,
-    hostkey_verify: bool,
-):
-    """Subscribes to notifications/events in real-time and prints them to the screen for debugging/troubleshooting"""
     logger.info(f"Attempting to establish NETCONF session to {host}:{port}")
     try:
         with manager.connect(
             host=host,
             port=port,
             username=username,
             password=password,
@@ -100,16 +98,26 @@
             )
 
             try:
                 while True:
                     logger.info("Awaiting next NETCONF <notification/>")
                     event = m.take_notification()
 
-                    logger.info(event.notification_xml)
+                    # Publish to RabbitMQ Queue
+                    data = event.notification_xml
+                    channel.basic_publish(
+                        exchange=rabbitmq_exchange,
+                        routing_key=rabbitmq_routing_key,
+                        body=data,
+                    )
+                    logger.success(f"Published message to RabbitMQ Server:\n{data}")
             except KeyboardInterrupt:
                 logger.info("Stopping NETCONF Notification Subscription")
     except SSHError as err:
         logger.error(err)
+        exit()
     except AuthenticationError as err:
         logger.error("Unable to authenticate to NETCONF server")
+        exit()
     except Exception as err:
         logger.error(f"Generic Exception caught: {err}")
+        exit()
```

### Comparing `netconf_tool-0.0.1/setup.py` & `netconf_tool-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="netconf_tool",
-    version="0.0.1",
+    version="0.0.2",
     packages=find_packages(exclude=("dev")),
     include_package_data=True,
     description="Click CLI application to help with NETCONF development experience",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/BSpendlove/netconf-tool",
     install_requires=[
         "ncclient>=0.6.13",
         "loguru>=0.7.0",
         "click>=8.1.3",
         "click-plugins>=1.1.1",
+        "redis>=4.5.4",
+        "pika>=1.3.1",
+        "xmltodict>=0.13.0",
     ],
     entry_points="""
         [console_scripts]
         netconf-tool=netconf_tool.cli:cli
     """,
 )
```

