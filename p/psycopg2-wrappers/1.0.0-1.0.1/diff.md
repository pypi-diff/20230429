# Comparing `tmp/psycopg2-wrappers-1.0.0.tar.gz` & `tmp/psycopg2-wrappers-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psycopg2-wrappers-1.0.0.tar", last modified: Sat Apr 29 14:01:13 2023, max compression
+gzip compressed data, was "psycopg2-wrappers-1.0.1.tar", last modified: Sat Apr 29 15:22:11 2023, max compression
```

## Comparing `psycopg2-wrappers-1.0.0.tar` & `psycopg2-wrappers-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 14:01:13.377617 psycopg2-wrappers-1.0.0/
--rw-rw-rw-   0        0        0     1088 2023-04-29 13:35:23.000000 psycopg2-wrappers-1.0.0/LICENCE
--rw-rw-rw-   0        0        0       43 2023-04-29 13:35:23.000000 psycopg2-wrappers-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9319 2023-04-29 14:01:13.380614 psycopg2-wrappers-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     8896 2023-04-29 13:35:09.000000 psycopg2-wrappers-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 14:01:13.316617 psycopg2-wrappers-1.0.0/examples/
--rw-rw-rw-   0        0        0        0 2023-04-29 09:08:08.000000 psycopg2-wrappers-1.0.0/examples/__init__.py
--rw-rw-rw-   0        0        0     1527 2023-04-29 09:08:08.000000 psycopg2-wrappers-1.0.0/examples/example_native_query_executor.py
--rw-rw-rw-   0        0        0     1332 2023-04-29 09:55:59.000000 psycopg2-wrappers-1.0.0/examples/example_simple_query_executor.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:01:13.359616 psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/
--rw-rw-rw-   0        0        0     9319 2023-04-29 14:01:13.000000 psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      559 2023-04-29 14:01:13.000000 psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 14:01:13.000000 psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-29 14:01:13.000000 psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-29 14:01:13.000000 psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 13:35:23.000000 psycopg2-wrappers-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0      118 2023-04-29 14:01:13.390615 psycopg2-wrappers-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-04-29 13:54:33.000000 psycopg2-wrappers-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:01:13.371616 psycopg2-wrappers-1.0.0/src/
--rw-rw-rw-   0        0        0     1904 2023-04-24 20:57:02.000000 psycopg2-wrappers-1.0.0/src/DatabaseConnector.py
--rw-rw-rw-   0        0        0     3857 2023-04-29 09:08:08.000000 psycopg2-wrappers-1.0.0/src/NativeQueryExecutor.py
--rw-rw-rw-   0        0        0     2576 2023-04-29 09:08:08.000000 psycopg2-wrappers-1.0.0/src/SimpleQueryExecutor.py
--rw-rw-rw-   0        0        0        0 2023-04-24 19:50:41.000000 psycopg2-wrappers-1.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 14:01:13.376615 psycopg2-wrappers-1.0.0/tests/
--rw-rw-rw-   0        0        0      611 2023-04-28 12:41:58.000000 psycopg2-wrappers-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2938 2023-04-29 09:08:08.000000 psycopg2-wrappers-1.0.0/tests/test_native_query_executor.py
--rw-rw-rw-   0        0        0     2265 2023-04-29 09:08:08.000000 psycopg2-wrappers-1.0.0/tests/test_simple_query_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:11.909580 psycopg2-wrappers-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-29 15:22:11.909580 psycopg2-wrappers-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:11.905580 psycopg2-wrappers-1.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/examples/example_native_query_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/examples/example_simple_query_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:11.909580 psycopg2-wrappers-1.0.1/psycopg2_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/psycopg2_wrapper/DatabaseConnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/psycopg2_wrapper/NativeQueryExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/psycopg2_wrapper/SimpleQueryExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/psycopg2_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:11.909580 psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-04-29 15:22:11.000000 psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-29 15:22:11.000000 psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 15:22:11.000000 psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-29 15:22:11.000000 psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-29 15:22:11.000000 psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 15:22:11.909580 psycopg2-wrappers-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 15:22:11.909580 psycopg2-wrappers-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/tests/test_native_query_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-29 15:22:01.000000 psycopg2-wrappers-1.0.1/tests/test_simple_query_executor.py
```

### Comparing `psycopg2-wrappers-1.0.0/PKG-INFO` & `psycopg2-wrappers-1.0.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,258 +1,246 @@
-Metadata-Version: 2.1
-Name: psycopg2-wrappers
-Version: 1.0.0
-Summary: psycopg2-wrapper is a wrapper for psycopg2 that makes it easier to use.
-Author: zestones
-Author-email: idrissbenguezzou@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Psycopg2-Wrapper
-
-Psycopg2-Wrapper is a Python library that provides a simple and easy-to-use interface for executing SQL queries using Psycopg2. It is designed to make it easy for developers to interact with PostgreSQL databases from Python applications.
-
-
-<!-- Add badges to showcase important information -->
-<p align="left">
-    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/zestones/psycopg2-wrapper/CI">
-    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/zestones/psycopg2-wrapper">
-    <img alt="GitHub license" src="https://img.shields.io/github/license/zestones/psycopg2-wrapper">
-</p>
-
-
-## Features
-
-- Simple and easy-to-use interface for executing SQL queries using Psycopg2.
-- Supports all standard SQL statements, including SELECT, INSERT, UPDATE, and DELETE.
-- Provides methods for executing single and multiple queries, fetching results, and committing changes to the database.
-- Built-in support for connection pooling.
-- Lightweight and easy to install, with no external dependencies.
-
-## Installation
-
-To install Psycopg2-Wrapper, you can use pip:
-
-```
-pip install psycopg2-wrapper
-```
-
-## Usage
-
-To use Psycopg2-Wrapper in your Python application, you first need to import one of the query executor classes from the `psycopg2_wrapper` module:
-
-```python
-from psycopg2_wrapper import SimpleQueryExecutor, NativeQueryExecutor
-```
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;">Configuration</summary>
-
-Before you can execute SQL queries using Psycopg2-Wrapper, you need to configure the connection to the PostgreSQL server. You can do this by creating a configuration dictionary with the following fields:
-
-```python
-config = {
-    "host": "localhost",
-    "port": "5432", # if not specified, default port 5432 will be used
-    "database": "mydatabase",
-    "user": "myusername",
-    "password": "mypassword"
-}
-```
-
-- `host`: The hostname of the PostgreSQL server.
-- `port`: The port number of the PostgreSQL server.
-- `database`: The name of the PostgreSQL database to connect to.
-- `user`: The username to use for authentication.
-- `password`: The password to use for authentication.
-
-Check out the [Psycopg2 documentation](https://www.psycopg.org/docs/module.html) for more information about the configuration options.
-</details>
-
----
-
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;"> NativeQueryExecutor </summary>
-
-The `NativeQueryExecutor` class allows you to execute native SQL queries using Psycopg2. You can create an instance of the class and use its `execute_query` method to execute SQL queries:
-
-```python
-# create a NativeQueryExecutor instance
-query_executor = NativeQueryExecutor(config)
-```	
-
-The `NativeQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
-
-This class implements the following methods for executing SQL queries:
-
-Query to read data from the database:
-```python
-def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
-def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
-def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
-```
-
-And query to write/modify data to the database:
-
-```python
-def execute_and_commit(self, sql: str, params: tuple = None) -> None:
-def execute_many_and_commit(self, sql: str, params: list) -> None:
-```
-
-<details>
-<summary style="font-weight: bold; font-size: 1em;">Read data from the database</summary>
-
-### Execute and fetchone
-
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchone(query_data_query, param)
-```
-The `execute_and_fetchone` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-The method returns a tuple containing the results of the query.
-
-### Execute and fetchmany
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchmany(query_data_query, param, 4)
-```
-The `execute_and_fetchmany` method takes three parameters: the **SQL query** to execute, **an optional tuple of parameters** to pass to the query, and **an optional size** parameter that specifies the maximum number of rows to fetch.
-
-
-### Execute and fetchall
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchall(query_data_query)
-```
-The `execute_and_fetchall` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-
----
-
-</details>
-
-
-
-<details>
-<summary style="font-weight: bold; font-size: 1em;">Write/modify data to the database</summary>
-
-### Execute and commit
-````python
-# the sql query
-query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
-# the parameters of the query
-param = (1, 'John')
-# execute the query and commit the changes
-query_executor.execute_and_commit(query_data_query, param)
-````
-The `execute_and_commit` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-
-### Execute many and commit
-````python
-# the sql query
-query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
-# the parameters of the query
-params = [(1, 'John'), (2, 'Jane'), (3, 'Jack')]
-# execute the query and commit the changes
-query_executor.execute_many_and_commit(query_data_query, params)
-````
-The `execute_many_and_commit` method takes two parameters: the **SQL query** to execute, and **a list of tuples of parameters** to pass to the query.
-
-Check out the [NativeQueryExecutor example](./examples/example_native_query_executor.py) for more examples of how to use the `NativeQueryExecutor` class.
-</details>
-</details>
-
----
-
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;">SimpleQueryExecutor</summary>
-
-The `SimpleQueryExecutor` class extends the `NativeQueryExecutor` class and provides methods for executing simple SQL queries. Here are some usage examples:
-
-First we start by instantiating the `SimpleQueryExecutor` class:
-```python
-# Define database configuration
-config = {
-    'host': 'localhost',
-    'port': 5432,
-    'database': 'my_database',
-    'user': 'my_user',
-    'password': 'my_password'
-}
-# Create an instance of SimpleQueryExecutor
-query_executor = SimpleQueryExecutor(config)
-```
-
-The `SimpleQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
-
-### Creating a table
-```python
-
-# Define the columns for the new table
-columns = {
-    'id': 'SERIAL PRIMARY KEY',
-    'name': 'VARCHAR(255)',
-    'age': 'INTEGER'
-}
-
-# Create the new table
-query_executor.create_table('my_table', columns)
-```
-
-The `create_table` method takes two parameters: the name of the table to create, and a dictionary of column names and their data types.
-
-### Selecting data from a table
-
-```python
-# Select all columns from the 'my_table' table
-results = query_executor.select_data('my_table')
-print(results)
-
-# Select only the 'name' and 'age' columns from the 'my_table' table
-results = query_executor.select_data('my_table', columns=['name', 'age'])
-print(results)
-
-# Select only the 'name' column from the 'my_table' table where age is greater than or equal to 18
-results = query_executor.select_data('my_table', columns=['name'], where='age >= 18')
-print(results)
-```
-The `select_data` method takes three parameters: the **name of the table** to select data from, a **list of column names to select**, and **an optional `where_clause` parameter** to filter the results.
-
-
-### Inserting data into a table
-
-```python
-# Define the data to insert
-data = {
-    'name': 'John',
-    'age': 25
-}
-
-# Insert the data into the 'my_table' table
-query_executor.insert_data('my_table', data)
-```
-The `insert_data` method takes two parameters: **the name of the table** to insert data into, and **a dictionary of column names and their corresponding values**.
-
-
-### Dropping a table
-
-```python
-# Drop the 'my_table' table
-query_executor.drop_table('my_table')
-```
-The `drop_table` method takes one parameter: **the name of the table** to drop.
-
-For more examples of how to use the `SimpleQueryExecutor` class, check out the [SimpleQueryExecutor example](./examples/example_simple_query_executor.py).
-</details>
+# Psycopg2-Wrapper
+
+Psycopg2-Wrapper is a Python library that provides a simple and easy-to-use interface for executing SQL queries using Psycopg2. It is designed to make it easy for developers to interact with PostgreSQL databases from Python applications.
+
+
+<!-- Add badges to showcase important information -->
+<p align="left">
+    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/zestones/psycopg2-wrapper/CI">
+    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/zestones/psycopg2-wrapper">
+    <img alt="GitHub license" src="https://img.shields.io/github/license/zestones/psycopg2-wrapper">
+</p>
+
+
+## Features
+
+- Simple and easy-to-use interface for executing SQL queries using Psycopg2.
+- Supports all standard SQL statements, including SELECT, INSERT, UPDATE, and DELETE.
+- Provides methods for executing single and multiple queries, fetching results, and committing changes to the database.
+- Built-in support for connection pooling.
+- Lightweight and easy to install, with no external dependencies.
+
+## Installation
+
+To install Psycopg2-Wrapper, you can use pip:
+
+```
+pip install psycopg2-wrapper
+```
+
+## Usage
+
+To use Psycopg2-Wrapper in your Python application, you first need to import one of the query executor classes from the `psycopg2_wrapper` module:
+
+```python
+from psycopg2_wrapper import SimpleQueryExecutor, NativeQueryExecutor
+```
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;">Configuration</summary>
+
+Before you can execute SQL queries using Psycopg2-Wrapper, you need to configure the connection to the PostgreSQL server. You can do this by creating a configuration dictionary with the following fields:
+
+```python
+config = {
+    "host": "localhost",
+    "port": "5432", # if not specified, default port 5432 will be used
+    "database": "mydatabase",
+    "user": "myusername",
+    "password": "mypassword"
+}
+```
+
+- `host`: The hostname of the PostgreSQL server.
+- `port`: The port number of the PostgreSQL server.
+- `database`: The name of the PostgreSQL database to connect to.
+- `user`: The username to use for authentication.
+- `password`: The password to use for authentication.
+
+Check out the [Psycopg2 documentation](https://www.psycopg.org/docs/module.html) for more information about the configuration options.
+</details>
+
+---
+
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;"> NativeQueryExecutor </summary>
+
+The `NativeQueryExecutor` class allows you to execute native SQL queries using Psycopg2. You can create an instance of the class and use its `execute_query` method to execute SQL queries:
+
+```python
+# create a NativeQueryExecutor instance
+query_executor = NativeQueryExecutor(config)
+```	
+
+The `NativeQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
+
+This class implements the following methods for executing SQL queries:
+
+Query to read data from the database:
+```python
+def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
+def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
+def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
+```
+
+And query to write/modify data to the database:
+
+```python
+def execute_and_commit(self, sql: str, params: tuple = None) -> None:
+def execute_many_and_commit(self, sql: str, params: list) -> None:
+```
+
+<details>
+<summary style="font-weight: bold; font-size: 1em;">Read data from the database</summary>
+
+### Execute and fetchone
+
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchone(query_data_query, param)
+```
+The `execute_and_fetchone` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+The method returns a tuple containing the results of the query.
+
+### Execute and fetchmany
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchmany(query_data_query, param, 4)
+```
+The `execute_and_fetchmany` method takes three parameters: the **SQL query** to execute, **an optional tuple of parameters** to pass to the query, and **an optional size** parameter that specifies the maximum number of rows to fetch.
+
+
+### Execute and fetchall
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchall(query_data_query)
+```
+The `execute_and_fetchall` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+
+---
+
+</details>
+
+
+
+<details>
+<summary style="font-weight: bold; font-size: 1em;">Write/modify data to the database</summary>
+
+### Execute and commit
+````python
+# the sql query
+query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
+# the parameters of the query
+param = (1, 'John')
+# execute the query and commit the changes
+query_executor.execute_and_commit(query_data_query, param)
+````
+The `execute_and_commit` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+
+### Execute many and commit
+````python
+# the sql query
+query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
+# the parameters of the query
+params = [(1, 'John'), (2, 'Jane'), (3, 'Jack')]
+# execute the query and commit the changes
+query_executor.execute_many_and_commit(query_data_query, params)
+````
+The `execute_many_and_commit` method takes two parameters: the **SQL query** to execute, and **a list of tuples of parameters** to pass to the query.
+
+Check out the [NativeQueryExecutor example](./examples/example_native_query_executor.py) for more examples of how to use the `NativeQueryExecutor` class.
+</details>
+</details>
+
+---
+
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;">SimpleQueryExecutor</summary>
+
+The `SimpleQueryExecutor` class extends the `NativeQueryExecutor` class and provides methods for executing simple SQL queries. Here are some usage examples:
+
+First we start by instantiating the `SimpleQueryExecutor` class:
+```python
+# Define database configuration
+config = {
+    'host': 'localhost',
+    'port': 5432,
+    'database': 'my_database',
+    'user': 'my_user',
+    'password': 'my_password'
+}
+# Create an instance of SimpleQueryExecutor
+query_executor = SimpleQueryExecutor(config)
+```
+
+The `SimpleQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
+
+### Creating a table
+```python
+
+# Define the columns for the new table
+columns = {
+    'id': 'SERIAL PRIMARY KEY',
+    'name': 'VARCHAR(255)',
+    'age': 'INTEGER'
+}
+
+# Create the new table
+query_executor.create_table('my_table', columns)
+```
+
+The `create_table` method takes two parameters: the name of the table to create, and a dictionary of column names and their data types.
+
+### Selecting data from a table
+
+```python
+# Select all columns from the 'my_table' table
+results = query_executor.select_data('my_table')
+print(results)
+
+# Select only the 'name' and 'age' columns from the 'my_table' table
+results = query_executor.select_data('my_table', columns=['name', 'age'])
+print(results)
+
+# Select only the 'name' column from the 'my_table' table where age is greater than or equal to 18
+results = query_executor.select_data('my_table', columns=['name'], where='age >= 18')
+print(results)
+```
+The `select_data` method takes three parameters: the **name of the table** to select data from, a **list of column names to select**, and **an optional `where_clause` parameter** to filter the results.
+
+
+### Inserting data into a table
+
+```python
+# Define the data to insert
+data = {
+    'name': 'John',
+    'age': 25
+}
+
+# Insert the data into the 'my_table' table
+query_executor.insert_data('my_table', data)
+```
+The `insert_data` method takes two parameters: **the name of the table** to insert data into, and **a dictionary of column names and their corresponding values**.
+
+
+### Dropping a table
+
+```python
+# Drop the 'my_table' table
+query_executor.drop_table('my_table')
+```
+The `drop_table` method takes one parameter: **the name of the table** to drop.
+
+For more examples of how to use the `SimpleQueryExecutor` class, check out the [SimpleQueryExecutor example](./examples/example_simple_query_executor.py).
+</details>
```

### Comparing `psycopg2-wrappers-1.0.0/README.md` & `psycopg2-wrappers-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,246 +1,258 @@
-# Psycopg2-Wrapper
-
-Psycopg2-Wrapper is a Python library that provides a simple and easy-to-use interface for executing SQL queries using Psycopg2. It is designed to make it easy for developers to interact with PostgreSQL databases from Python applications.
-
-
-<!-- Add badges to showcase important information -->
-<p align="left">
-    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/zestones/psycopg2-wrapper/CI">
-    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/zestones/psycopg2-wrapper">
-    <img alt="GitHub license" src="https://img.shields.io/github/license/zestones/psycopg2-wrapper">
-</p>
-
-
-## Features
-
-- Simple and easy-to-use interface for executing SQL queries using Psycopg2.
-- Supports all standard SQL statements, including SELECT, INSERT, UPDATE, and DELETE.
-- Provides methods for executing single and multiple queries, fetching results, and committing changes to the database.
-- Built-in support for connection pooling.
-- Lightweight and easy to install, with no external dependencies.
-
-## Installation
-
-To install Psycopg2-Wrapper, you can use pip:
-
-```
-pip install psycopg2-wrapper
-```
-
-## Usage
-
-To use Psycopg2-Wrapper in your Python application, you first need to import one of the query executor classes from the `psycopg2_wrapper` module:
-
-```python
-from psycopg2_wrapper import SimpleQueryExecutor, NativeQueryExecutor
-```
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;">Configuration</summary>
-
-Before you can execute SQL queries using Psycopg2-Wrapper, you need to configure the connection to the PostgreSQL server. You can do this by creating a configuration dictionary with the following fields:
-
-```python
-config = {
-    "host": "localhost",
-    "port": "5432", # if not specified, default port 5432 will be used
-    "database": "mydatabase",
-    "user": "myusername",
-    "password": "mypassword"
-}
-```
-
-- `host`: The hostname of the PostgreSQL server.
-- `port`: The port number of the PostgreSQL server.
-- `database`: The name of the PostgreSQL database to connect to.
-- `user`: The username to use for authentication.
-- `password`: The password to use for authentication.
-
-Check out the [Psycopg2 documentation](https://www.psycopg.org/docs/module.html) for more information about the configuration options.
-</details>
-
----
-
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;"> NativeQueryExecutor </summary>
-
-The `NativeQueryExecutor` class allows you to execute native SQL queries using Psycopg2. You can create an instance of the class and use its `execute_query` method to execute SQL queries:
-
-```python
-# create a NativeQueryExecutor instance
-query_executor = NativeQueryExecutor(config)
-```	
-
-The `NativeQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
-
-This class implements the following methods for executing SQL queries:
-
-Query to read data from the database:
-```python
-def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
-def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
-def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
-```
-
-And query to write/modify data to the database:
-
-```python
-def execute_and_commit(self, sql: str, params: tuple = None) -> None:
-def execute_many_and_commit(self, sql: str, params: list) -> None:
-```
-
-<details>
-<summary style="font-weight: bold; font-size: 1em;">Read data from the database</summary>
-
-### Execute and fetchone
-
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchone(query_data_query, param)
-```
-The `execute_and_fetchone` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-The method returns a tuple containing the results of the query.
-
-### Execute and fetchmany
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchmany(query_data_query, param, 4)
-```
-The `execute_and_fetchmany` method takes three parameters: the **SQL query** to execute, **an optional tuple of parameters** to pass to the query, and **an optional size** parameter that specifies the maximum number of rows to fetch.
-
-
-### Execute and fetchall
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchall(query_data_query)
-```
-The `execute_and_fetchall` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-
----
-
-</details>
-
-
-
-<details>
-<summary style="font-weight: bold; font-size: 1em;">Write/modify data to the database</summary>
-
-### Execute and commit
-````python
-# the sql query
-query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
-# the parameters of the query
-param = (1, 'John')
-# execute the query and commit the changes
-query_executor.execute_and_commit(query_data_query, param)
-````
-The `execute_and_commit` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-
-### Execute many and commit
-````python
-# the sql query
-query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
-# the parameters of the query
-params = [(1, 'John'), (2, 'Jane'), (3, 'Jack')]
-# execute the query and commit the changes
-query_executor.execute_many_and_commit(query_data_query, params)
-````
-The `execute_many_and_commit` method takes two parameters: the **SQL query** to execute, and **a list of tuples of parameters** to pass to the query.
-
-Check out the [NativeQueryExecutor example](./examples/example_native_query_executor.py) for more examples of how to use the `NativeQueryExecutor` class.
-</details>
-</details>
-
----
-
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;">SimpleQueryExecutor</summary>
-
-The `SimpleQueryExecutor` class extends the `NativeQueryExecutor` class and provides methods for executing simple SQL queries. Here are some usage examples:
-
-First we start by instantiating the `SimpleQueryExecutor` class:
-```python
-# Define database configuration
-config = {
-    'host': 'localhost',
-    'port': 5432,
-    'database': 'my_database',
-    'user': 'my_user',
-    'password': 'my_password'
-}
-# Create an instance of SimpleQueryExecutor
-query_executor = SimpleQueryExecutor(config)
-```
-
-The `SimpleQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
-
-### Creating a table
-```python
-
-# Define the columns for the new table
-columns = {
-    'id': 'SERIAL PRIMARY KEY',
-    'name': 'VARCHAR(255)',
-    'age': 'INTEGER'
-}
-
-# Create the new table
-query_executor.create_table('my_table', columns)
-```
-
-The `create_table` method takes two parameters: the name of the table to create, and a dictionary of column names and their data types.
-
-### Selecting data from a table
-
-```python
-# Select all columns from the 'my_table' table
-results = query_executor.select_data('my_table')
-print(results)
-
-# Select only the 'name' and 'age' columns from the 'my_table' table
-results = query_executor.select_data('my_table', columns=['name', 'age'])
-print(results)
-
-# Select only the 'name' column from the 'my_table' table where age is greater than or equal to 18
-results = query_executor.select_data('my_table', columns=['name'], where='age >= 18')
-print(results)
-```
-The `select_data` method takes three parameters: the **name of the table** to select data from, a **list of column names to select**, and **an optional `where_clause` parameter** to filter the results.
-
-
-### Inserting data into a table
-
-```python
-# Define the data to insert
-data = {
-    'name': 'John',
-    'age': 25
-}
-
-# Insert the data into the 'my_table' table
-query_executor.insert_data('my_table', data)
-```
-The `insert_data` method takes two parameters: **the name of the table** to insert data into, and **a dictionary of column names and their corresponding values**.
-
-
-### Dropping a table
-
-```python
-# Drop the 'my_table' table
-query_executor.drop_table('my_table')
-```
-The `drop_table` method takes one parameter: **the name of the table** to drop.
-
-For more examples of how to use the `SimpleQueryExecutor` class, check out the [SimpleQueryExecutor example](./examples/example_simple_query_executor.py).
-</details>
+Metadata-Version: 2.1
+Name: psycopg2-wrappers
+Version: 1.0.1
+Summary: psycopg2-wrapper is a wrapper for psycopg2 that makes it easier to use.
+Author: zestones
+Author-email: idrissbenguezzou@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Psycopg2-Wrapper
+
+Psycopg2-Wrapper is a Python library that provides a simple and easy-to-use interface for executing SQL queries using Psycopg2. It is designed to make it easy for developers to interact with PostgreSQL databases from Python applications.
+
+
+<!-- Add badges to showcase important information -->
+<p align="left">
+    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/zestones/psycopg2-wrapper/CI">
+    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/zestones/psycopg2-wrapper">
+    <img alt="GitHub license" src="https://img.shields.io/github/license/zestones/psycopg2-wrapper">
+</p>
+
+
+## Features
+
+- Simple and easy-to-use interface for executing SQL queries using Psycopg2.
+- Supports all standard SQL statements, including SELECT, INSERT, UPDATE, and DELETE.
+- Provides methods for executing single and multiple queries, fetching results, and committing changes to the database.
+- Built-in support for connection pooling.
+- Lightweight and easy to install, with no external dependencies.
+
+## Installation
+
+To install Psycopg2-Wrapper, you can use pip:
+
+```
+pip install psycopg2-wrapper
+```
+
+## Usage
+
+To use Psycopg2-Wrapper in your Python application, you first need to import one of the query executor classes from the `psycopg2_wrapper` module:
+
+```python
+from psycopg2_wrapper import SimpleQueryExecutor, NativeQueryExecutor
+```
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;">Configuration</summary>
+
+Before you can execute SQL queries using Psycopg2-Wrapper, you need to configure the connection to the PostgreSQL server. You can do this by creating a configuration dictionary with the following fields:
+
+```python
+config = {
+    "host": "localhost",
+    "port": "5432", # if not specified, default port 5432 will be used
+    "database": "mydatabase",
+    "user": "myusername",
+    "password": "mypassword"
+}
+```
+
+- `host`: The hostname of the PostgreSQL server.
+- `port`: The port number of the PostgreSQL server.
+- `database`: The name of the PostgreSQL database to connect to.
+- `user`: The username to use for authentication.
+- `password`: The password to use for authentication.
+
+Check out the [Psycopg2 documentation](https://www.psycopg.org/docs/module.html) for more information about the configuration options.
+</details>
+
+---
+
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;"> NativeQueryExecutor </summary>
+
+The `NativeQueryExecutor` class allows you to execute native SQL queries using Psycopg2. You can create an instance of the class and use its `execute_query` method to execute SQL queries:
+
+```python
+# create a NativeQueryExecutor instance
+query_executor = NativeQueryExecutor(config)
+```	
+
+The `NativeQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
+
+This class implements the following methods for executing SQL queries:
+
+Query to read data from the database:
+```python
+def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
+def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
+def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
+```
+
+And query to write/modify data to the database:
+
+```python
+def execute_and_commit(self, sql: str, params: tuple = None) -> None:
+def execute_many_and_commit(self, sql: str, params: list) -> None:
+```
+
+<details>
+<summary style="font-weight: bold; font-size: 1em;">Read data from the database</summary>
+
+### Execute and fetchone
+
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchone(query_data_query, param)
+```
+The `execute_and_fetchone` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+The method returns a tuple containing the results of the query.
+
+### Execute and fetchmany
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchmany(query_data_query, param, 4)
+```
+The `execute_and_fetchmany` method takes three parameters: the **SQL query** to execute, **an optional tuple of parameters** to pass to the query, and **an optional size** parameter that specifies the maximum number of rows to fetch.
+
+
+### Execute and fetchall
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchall(query_data_query)
+```
+The `execute_and_fetchall` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+
+---
+
+</details>
+
+
+
+<details>
+<summary style="font-weight: bold; font-size: 1em;">Write/modify data to the database</summary>
+
+### Execute and commit
+````python
+# the sql query
+query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
+# the parameters of the query
+param = (1, 'John')
+# execute the query and commit the changes
+query_executor.execute_and_commit(query_data_query, param)
+````
+The `execute_and_commit` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+
+### Execute many and commit
+````python
+# the sql query
+query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
+# the parameters of the query
+params = [(1, 'John'), (2, 'Jane'), (3, 'Jack')]
+# execute the query and commit the changes
+query_executor.execute_many_and_commit(query_data_query, params)
+````
+The `execute_many_and_commit` method takes two parameters: the **SQL query** to execute, and **a list of tuples of parameters** to pass to the query.
+
+Check out the [NativeQueryExecutor example](./examples/example_native_query_executor.py) for more examples of how to use the `NativeQueryExecutor` class.
+</details>
+</details>
+
+---
+
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;">SimpleQueryExecutor</summary>
+
+The `SimpleQueryExecutor` class extends the `NativeQueryExecutor` class and provides methods for executing simple SQL queries. Here are some usage examples:
+
+First we start by instantiating the `SimpleQueryExecutor` class:
+```python
+# Define database configuration
+config = {
+    'host': 'localhost',
+    'port': 5432,
+    'database': 'my_database',
+    'user': 'my_user',
+    'password': 'my_password'
+}
+# Create an instance of SimpleQueryExecutor
+query_executor = SimpleQueryExecutor(config)
+```
+
+The `SimpleQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
+
+### Creating a table
+```python
+
+# Define the columns for the new table
+columns = {
+    'id': 'SERIAL PRIMARY KEY',
+    'name': 'VARCHAR(255)',
+    'age': 'INTEGER'
+}
+
+# Create the new table
+query_executor.create_table('my_table', columns)
+```
+
+The `create_table` method takes two parameters: the name of the table to create, and a dictionary of column names and their data types.
+
+### Selecting data from a table
+
+```python
+# Select all columns from the 'my_table' table
+results = query_executor.select_data('my_table')
+print(results)
+
+# Select only the 'name' and 'age' columns from the 'my_table' table
+results = query_executor.select_data('my_table', columns=['name', 'age'])
+print(results)
+
+# Select only the 'name' column from the 'my_table' table where age is greater than or equal to 18
+results = query_executor.select_data('my_table', columns=['name'], where='age >= 18')
+print(results)
+```
+The `select_data` method takes three parameters: the **name of the table** to select data from, a **list of column names to select**, and **an optional `where_clause` parameter** to filter the results.
+
+
+### Inserting data into a table
+
+```python
+# Define the data to insert
+data = {
+    'name': 'John',
+    'age': 25
+}
+
+# Insert the data into the 'my_table' table
+query_executor.insert_data('my_table', data)
+```
+The `insert_data` method takes two parameters: **the name of the table** to insert data into, and **a dictionary of column names and their corresponding values**.
+
+
+### Dropping a table
+
+```python
+# Drop the 'my_table' table
+query_executor.drop_table('my_table')
+```
+The `drop_table` method takes one parameter: **the name of the table** to drop.
+
+For more examples of how to use the `SimpleQueryExecutor` class, check out the [SimpleQueryExecutor example](./examples/example_simple_query_executor.py).
+</details>
```

### Comparing `psycopg2-wrappers-1.0.0/examples/example_native_query_executor.py` & `psycopg2-wrappers-1.0.1/examples/example_native_query_executor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import sys
-import os
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-
-from src.NativeQueryExecutor import NativeQueryExecutor
-
-# database parameters 
-DATABASE_PARAMS = {
-    "host": "localhost",
-    "port": 5432,
-    "user": "postgres",
-    "password": "pwd",
-    "database": "mydatabase" # create a database named "mydatabase" before running this script
-}
-
-
-# create a NativeQueryExecutor instance
-query_executor = NativeQueryExecutor(config=DATABASE_PARAMS)
-
-# create a table in the database
-create_table_query = """
-					CREATE TABLE example_table (
-						id INT PRIMARY KEY,
-						name VARCHAR(50),
-						age INT
-					)
-					"""
-query_executor.execute_and_commit(create_table_query)
-
-
-# insert some data
-insert_data_query = """
-                    INSERT INTO example_table (id, name, age)
-                    VALUES (%s, %s, %s)
-                    """
-    
-# each row is a tuple of values to be inserted
-params = [
-    (1, 'Alice', 25),
-    (2, 'Bob', 30),
-    (3, 'Charlie', 35)
-]
-query_executor.execute_many_and_commit(insert_data_query, params)
-
-# query the table
-query_data_query = "SELECT * FROM example_table"
-result = query_executor.execute_and_fetchall(query_data_query)
-
-# print the result 
-print("id\t|name\t|age")
-print("------------------")
-for row in result:
-	print("{}\t|{}\t|{}".format(row[0], row[1], row[2]))
-
- 
-# delete the table
-drop_table_query = "DROP TABLE example_table"
+import sys
+import os
+
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+
+from psycopg2_wrapper.NativeQueryExecutor import NativeQueryExecutor
+
+# database parameters 
+DATABASE_PARAMS = {
+    "host": "localhost",
+    "port": 5432,
+    "user": "postgres",
+    "password": "pwd",
+    "database": "mydatabase" # create a database named "mydatabase" before running this script
+}
+
+
+# create a NativeQueryExecutor instance
+query_executor = NativeQueryExecutor(config=DATABASE_PARAMS)
+
+# create a table in the database
+create_table_query = """
+					CREATE TABLE example_table (
+						id INT PRIMARY KEY,
+						name VARCHAR(50),
+						age INT
+					)
+					"""
+query_executor.execute_and_commit(create_table_query)
+
+
+# insert some data
+insert_data_query = """
+                    INSERT INTO example_table (id, name, age)
+                    VALUES (%s, %s, %s)
+                    """
+    
+# each row is a tuple of values to be inserted
+params = [
+    (1, 'Alice', 25),
+    (2, 'Bob', 30),
+    (3, 'Charlie', 35)
+]
+query_executor.execute_many_and_commit(insert_data_query, params)
+
+# query the table
+query_data_query = "SELECT * FROM example_table"
+result = query_executor.execute_and_fetchall(query_data_query)
+
+# print the result 
+print("id\t|name\t|age")
+print("------------------")
+for row in result:
+	print("{}\t|{}\t|{}".format(row[0], row[1], row[2]))
+
+ 
+# delete the table
+drop_table_query = "DROP TABLE example_table"
 query_executor.execute_and_commit(drop_table_query)
```

### Comparing `psycopg2-wrappers-1.0.0/examples/example_simple_query_executor.py` & `psycopg2-wrappers-1.0.1/examples/example_simple_query_executor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import sys
-import os
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
-
-from src.SimpleQueryExecutor import SimpleQueryExecutor
-
-# database parameters 
-DATABASE_PARAMS = {
-    "host": "localhost",
-    "port": 5432,
-    "user": "postgres",
-    "password": "pwd",
-    "database": "mydatabase" # create a database named "mydatabase" before running this script
-}
-
-
-# create an instance of the SimpleQueryExecutor class
-query_executor = SimpleQueryExecutor(config=DATABASE_PARAMS)
-
-# create a new table with two columns (id and name)
-query_executor.create_table(table_name='users', columns={'id': 'SERIAL PRIMARY KEY', 'name': 'VARCHAR(255)', 'age': 'INT'})
-
-# insert some data into the table
-query_executor.insert_data(table_name='users', data={'name': 'John', 'age': 25})
-query_executor.insert_data(table_name='users', data={'name': 'Mary', 'age': 30})
-query_executor.insert_data(table_name='users', data={'name': 'Bob', 'age': 35})
-
-# Select only the name and age columns for users aged 30 or older
-results = query_executor.select_data(table_name='users', columns=['name', 'age'], where='age >= 30')
-
-# print the results
-print("name\t|age")
-print("---------------")
-for row in results:
-    print("{}\t|{}".format(row[0], row[1]))
-
-# drop the table
+import sys
+import os
+
+sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+
+from psycopg2_wrapper.SimpleQueryExecutor import SimpleQueryExecutor
+
+# database parameters 
+DATABASE_PARAMS = {
+    "host": "localhost",
+    "port": 5432,
+    "user": "postgres",
+    "password": "pwd",
+    "database": "mydatabase" # create a database named "mydatabase" before running this script
+}
+
+
+# create an instance of the SimpleQueryExecutor class
+query_executor = SimpleQueryExecutor(config=DATABASE_PARAMS)
+
+# create a new table with two columns (id and name)
+query_executor.create_table(table_name='users', columns={'id': 'SERIAL PRIMARY KEY', 'name': 'VARCHAR(255)', 'age': 'INT'})
+
+# insert some data into the table
+query_executor.insert_data(table_name='users', data={'name': 'John', 'age': 25})
+query_executor.insert_data(table_name='users', data={'name': 'Mary', 'age': 30})
+query_executor.insert_data(table_name='users', data={'name': 'Bob', 'age': 35})
+
+# Select only the name and age columns for users aged 30 or older
+results = query_executor.select_data(table_name='users', columns=['name', 'age'], where='age >= 30')
+
+# print the results
+print("name\t|age")
+print("---------------")
+for row in results:
+    print("{}\t|{}".format(row[0], row[1]))
+
+# drop the table
 query_executor.drop_table('users')
```

### Comparing `psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/PKG-INFO` & `psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-Metadata-Version: 2.1
-Name: psycopg2-wrappers
-Version: 1.0.0
-Summary: psycopg2-wrapper is a wrapper for psycopg2 that makes it easier to use.
-Author: zestones
-Author-email: idrissbenguezzou@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
-# Psycopg2-Wrapper
-
-Psycopg2-Wrapper is a Python library that provides a simple and easy-to-use interface for executing SQL queries using Psycopg2. It is designed to make it easy for developers to interact with PostgreSQL databases from Python applications.
-
-
-<!-- Add badges to showcase important information -->
-<p align="left">
-    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/zestones/psycopg2-wrapper/CI">
-    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/zestones/psycopg2-wrapper">
-    <img alt="GitHub license" src="https://img.shields.io/github/license/zestones/psycopg2-wrapper">
-</p>
-
-
-## Features
-
-- Simple and easy-to-use interface for executing SQL queries using Psycopg2.
-- Supports all standard SQL statements, including SELECT, INSERT, UPDATE, and DELETE.
-- Provides methods for executing single and multiple queries, fetching results, and committing changes to the database.
-- Built-in support for connection pooling.
-- Lightweight and easy to install, with no external dependencies.
-
-## Installation
-
-To install Psycopg2-Wrapper, you can use pip:
-
-```
-pip install psycopg2-wrapper
-```
-
-## Usage
-
-To use Psycopg2-Wrapper in your Python application, you first need to import one of the query executor classes from the `psycopg2_wrapper` module:
-
-```python
-from psycopg2_wrapper import SimpleQueryExecutor, NativeQueryExecutor
-```
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;">Configuration</summary>
-
-Before you can execute SQL queries using Psycopg2-Wrapper, you need to configure the connection to the PostgreSQL server. You can do this by creating a configuration dictionary with the following fields:
-
-```python
-config = {
-    "host": "localhost",
-    "port": "5432", # if not specified, default port 5432 will be used
-    "database": "mydatabase",
-    "user": "myusername",
-    "password": "mypassword"
-}
-```
-
-- `host`: The hostname of the PostgreSQL server.
-- `port`: The port number of the PostgreSQL server.
-- `database`: The name of the PostgreSQL database to connect to.
-- `user`: The username to use for authentication.
-- `password`: The password to use for authentication.
-
-Check out the [Psycopg2 documentation](https://www.psycopg.org/docs/module.html) for more information about the configuration options.
-</details>
-
----
-
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;"> NativeQueryExecutor </summary>
-
-The `NativeQueryExecutor` class allows you to execute native SQL queries using Psycopg2. You can create an instance of the class and use its `execute_query` method to execute SQL queries:
-
-```python
-# create a NativeQueryExecutor instance
-query_executor = NativeQueryExecutor(config)
-```	
-
-The `NativeQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
-
-This class implements the following methods for executing SQL queries:
-
-Query to read data from the database:
-```python
-def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
-def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
-def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
-```
-
-And query to write/modify data to the database:
-
-```python
-def execute_and_commit(self, sql: str, params: tuple = None) -> None:
-def execute_many_and_commit(self, sql: str, params: list) -> None:
-```
-
-<details>
-<summary style="font-weight: bold; font-size: 1em;">Read data from the database</summary>
-
-### Execute and fetchone
-
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchone(query_data_query, param)
-```
-The `execute_and_fetchone` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-The method returns a tuple containing the results of the query.
-
-### Execute and fetchmany
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchmany(query_data_query, param, 4)
-```
-The `execute_and_fetchmany` method takes three parameters: the **SQL query** to execute, **an optional tuple of parameters** to pass to the query, and **an optional size** parameter that specifies the maximum number of rows to fetch.
-
-
-### Execute and fetchall
-```python
-# the sql query
-query_data_query = "SELECT * FROM example_table WHERE id = %s"
-# the parameters of the query
-param = (1,)
-# execute the query and fetch the results
-result = query_executor.execute_and_fetchall(query_data_query)
-```
-The `execute_and_fetchall` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-
----
-
-</details>
-
-
-
-<details>
-<summary style="font-weight: bold; font-size: 1em;">Write/modify data to the database</summary>
-
-### Execute and commit
-````python
-# the sql query
-query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
-# the parameters of the query
-param = (1, 'John')
-# execute the query and commit the changes
-query_executor.execute_and_commit(query_data_query, param)
-````
-The `execute_and_commit` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
-
-### Execute many and commit
-````python
-# the sql query
-query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
-# the parameters of the query
-params = [(1, 'John'), (2, 'Jane'), (3, 'Jack')]
-# execute the query and commit the changes
-query_executor.execute_many_and_commit(query_data_query, params)
-````
-The `execute_many_and_commit` method takes two parameters: the **SQL query** to execute, and **a list of tuples of parameters** to pass to the query.
-
-Check out the [NativeQueryExecutor example](./examples/example_native_query_executor.py) for more examples of how to use the `NativeQueryExecutor` class.
-</details>
-</details>
-
----
-
-<details>
-<summary style="font-weight: bold; font-size: 1.2em;">SimpleQueryExecutor</summary>
-
-The `SimpleQueryExecutor` class extends the `NativeQueryExecutor` class and provides methods for executing simple SQL queries. Here are some usage examples:
-
-First we start by instantiating the `SimpleQueryExecutor` class:
-```python
-# Define database configuration
-config = {
-    'host': 'localhost',
-    'port': 5432,
-    'database': 'my_database',
-    'user': 'my_user',
-    'password': 'my_password'
-}
-# Create an instance of SimpleQueryExecutor
-query_executor = SimpleQueryExecutor(config)
-```
-
-The `SimpleQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
-
-### Creating a table
-```python
-
-# Define the columns for the new table
-columns = {
-    'id': 'SERIAL PRIMARY KEY',
-    'name': 'VARCHAR(255)',
-    'age': 'INTEGER'
-}
-
-# Create the new table
-query_executor.create_table('my_table', columns)
-```
-
-The `create_table` method takes two parameters: the name of the table to create, and a dictionary of column names and their data types.
-
-### Selecting data from a table
-
-```python
-# Select all columns from the 'my_table' table
-results = query_executor.select_data('my_table')
-print(results)
-
-# Select only the 'name' and 'age' columns from the 'my_table' table
-results = query_executor.select_data('my_table', columns=['name', 'age'])
-print(results)
-
-# Select only the 'name' column from the 'my_table' table where age is greater than or equal to 18
-results = query_executor.select_data('my_table', columns=['name'], where='age >= 18')
-print(results)
-```
-The `select_data` method takes three parameters: the **name of the table** to select data from, a **list of column names to select**, and **an optional `where_clause` parameter** to filter the results.
-
-
-### Inserting data into a table
-
-```python
-# Define the data to insert
-data = {
-    'name': 'John',
-    'age': 25
-}
-
-# Insert the data into the 'my_table' table
-query_executor.insert_data('my_table', data)
-```
-The `insert_data` method takes two parameters: **the name of the table** to insert data into, and **a dictionary of column names and their corresponding values**.
-
-
-### Dropping a table
-
-```python
-# Drop the 'my_table' table
-query_executor.drop_table('my_table')
-```
-The `drop_table` method takes one parameter: **the name of the table** to drop.
-
-For more examples of how to use the `SimpleQueryExecutor` class, check out the [SimpleQueryExecutor example](./examples/example_simple_query_executor.py).
-</details>
+Metadata-Version: 2.1
+Name: psycopg2-wrappers
+Version: 1.0.1
+Summary: psycopg2-wrapper is a wrapper for psycopg2 that makes it easier to use.
+Author: zestones
+Author-email: idrissbenguezzou@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
+# Psycopg2-Wrapper
+
+Psycopg2-Wrapper is a Python library that provides a simple and easy-to-use interface for executing SQL queries using Psycopg2. It is designed to make it easy for developers to interact with PostgreSQL databases from Python applications.
+
+
+<!-- Add badges to showcase important information -->
+<p align="left">
+    <img alt="GitHub Workflow Status" src="https://img.shields.io/github/workflow/status/zestones/psycopg2-wrapper/CI">
+    <img alt="GitHub release (latest SemVer)" src="https://img.shields.io/github/v/release/zestones/psycopg2-wrapper">
+    <img alt="GitHub license" src="https://img.shields.io/github/license/zestones/psycopg2-wrapper">
+</p>
+
+
+## Features
+
+- Simple and easy-to-use interface for executing SQL queries using Psycopg2.
+- Supports all standard SQL statements, including SELECT, INSERT, UPDATE, and DELETE.
+- Provides methods for executing single and multiple queries, fetching results, and committing changes to the database.
+- Built-in support for connection pooling.
+- Lightweight and easy to install, with no external dependencies.
+
+## Installation
+
+To install Psycopg2-Wrapper, you can use pip:
+
+```
+pip install psycopg2-wrapper
+```
+
+## Usage
+
+To use Psycopg2-Wrapper in your Python application, you first need to import one of the query executor classes from the `psycopg2_wrapper` module:
+
+```python
+from psycopg2_wrapper import SimpleQueryExecutor, NativeQueryExecutor
+```
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;">Configuration</summary>
+
+Before you can execute SQL queries using Psycopg2-Wrapper, you need to configure the connection to the PostgreSQL server. You can do this by creating a configuration dictionary with the following fields:
+
+```python
+config = {
+    "host": "localhost",
+    "port": "5432", # if not specified, default port 5432 will be used
+    "database": "mydatabase",
+    "user": "myusername",
+    "password": "mypassword"
+}
+```
+
+- `host`: The hostname of the PostgreSQL server.
+- `port`: The port number of the PostgreSQL server.
+- `database`: The name of the PostgreSQL database to connect to.
+- `user`: The username to use for authentication.
+- `password`: The password to use for authentication.
+
+Check out the [Psycopg2 documentation](https://www.psycopg.org/docs/module.html) for more information about the configuration options.
+</details>
+
+---
+
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;"> NativeQueryExecutor </summary>
+
+The `NativeQueryExecutor` class allows you to execute native SQL queries using Psycopg2. You can create an instance of the class and use its `execute_query` method to execute SQL queries:
+
+```python
+# create a NativeQueryExecutor instance
+query_executor = NativeQueryExecutor(config)
+```	
+
+The `NativeQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
+
+This class implements the following methods for executing SQL queries:
+
+Query to read data from the database:
+```python
+def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
+def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
+def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
+```
+
+And query to write/modify data to the database:
+
+```python
+def execute_and_commit(self, sql: str, params: tuple = None) -> None:
+def execute_many_and_commit(self, sql: str, params: list) -> None:
+```
+
+<details>
+<summary style="font-weight: bold; font-size: 1em;">Read data from the database</summary>
+
+### Execute and fetchone
+
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchone(query_data_query, param)
+```
+The `execute_and_fetchone` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+The method returns a tuple containing the results of the query.
+
+### Execute and fetchmany
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchmany(query_data_query, param, 4)
+```
+The `execute_and_fetchmany` method takes three parameters: the **SQL query** to execute, **an optional tuple of parameters** to pass to the query, and **an optional size** parameter that specifies the maximum number of rows to fetch.
+
+
+### Execute and fetchall
+```python
+# the sql query
+query_data_query = "SELECT * FROM example_table WHERE id = %s"
+# the parameters of the query
+param = (1,)
+# execute the query and fetch the results
+result = query_executor.execute_and_fetchall(query_data_query)
+```
+The `execute_and_fetchall` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+
+---
+
+</details>
+
+
+
+<details>
+<summary style="font-weight: bold; font-size: 1em;">Write/modify data to the database</summary>
+
+### Execute and commit
+````python
+# the sql query
+query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
+# the parameters of the query
+param = (1, 'John')
+# execute the query and commit the changes
+query_executor.execute_and_commit(query_data_query, param)
+````
+The `execute_and_commit` method takes two parameters: the **SQL query** to execute, and **an optional tuple of parameters** to pass to the query.
+
+### Execute many and commit
+````python
+# the sql query
+query_data_query = "INSERT INTO example_table (id, name) VALUES (%s, %s)"
+# the parameters of the query
+params = [(1, 'John'), (2, 'Jane'), (3, 'Jack')]
+# execute the query and commit the changes
+query_executor.execute_many_and_commit(query_data_query, params)
+````
+The `execute_many_and_commit` method takes two parameters: the **SQL query** to execute, and **a list of tuples of parameters** to pass to the query.
+
+Check out the [NativeQueryExecutor example](./examples/example_native_query_executor.py) for more examples of how to use the `NativeQueryExecutor` class.
+</details>
+</details>
+
+---
+
+<details>
+<summary style="font-weight: bold; font-size: 1.2em;">SimpleQueryExecutor</summary>
+
+The `SimpleQueryExecutor` class extends the `NativeQueryExecutor` class and provides methods for executing simple SQL queries. Here are some usage examples:
+
+First we start by instantiating the `SimpleQueryExecutor` class:
+```python
+# Define database configuration
+config = {
+    'host': 'localhost',
+    'port': 5432,
+    'database': 'my_database',
+    'user': 'my_user',
+    'password': 'my_password'
+}
+# Create an instance of SimpleQueryExecutor
+query_executor = SimpleQueryExecutor(config)
+```
+
+The `SimpleQueryExecutor` class takes a configuration dictionary as described [here](#configuration).
+
+### Creating a table
+```python
+
+# Define the columns for the new table
+columns = {
+    'id': 'SERIAL PRIMARY KEY',
+    'name': 'VARCHAR(255)',
+    'age': 'INTEGER'
+}
+
+# Create the new table
+query_executor.create_table('my_table', columns)
+```
+
+The `create_table` method takes two parameters: the name of the table to create, and a dictionary of column names and their data types.
+
+### Selecting data from a table
+
+```python
+# Select all columns from the 'my_table' table
+results = query_executor.select_data('my_table')
+print(results)
+
+# Select only the 'name' and 'age' columns from the 'my_table' table
+results = query_executor.select_data('my_table', columns=['name', 'age'])
+print(results)
+
+# Select only the 'name' column from the 'my_table' table where age is greater than or equal to 18
+results = query_executor.select_data('my_table', columns=['name'], where='age >= 18')
+print(results)
+```
+The `select_data` method takes three parameters: the **name of the table** to select data from, a **list of column names to select**, and **an optional `where_clause` parameter** to filter the results.
+
+
+### Inserting data into a table
+
+```python
+# Define the data to insert
+data = {
+    'name': 'John',
+    'age': 25
+}
+
+# Insert the data into the 'my_table' table
+query_executor.insert_data('my_table', data)
+```
+The `insert_data` method takes two parameters: **the name of the table** to insert data into, and **a dictionary of column names and their corresponding values**.
+
+
+### Dropping a table
+
+```python
+# Drop the 'my_table' table
+query_executor.drop_table('my_table')
+```
+The `drop_table` method takes one parameter: **the name of the table** to drop.
+
+For more examples of how to use the `SimpleQueryExecutor` class, check out the [SimpleQueryExecutor example](./examples/example_simple_query_executor.py).
+</details>
```

### Comparing `psycopg2-wrappers-1.0.0/psycopg2_wrappers.egg-info/SOURCES.txt` & `psycopg2-wrappers-1.0.1/psycopg2_wrappers.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 LICENCE
 MANIFEST.in
 README.md
 requirements.txt
-setup.cfg
 setup.py
 examples/__init__.py
 examples/example_native_query_executor.py
 examples/example_simple_query_executor.py
+psycopg2_wrapper/DatabaseConnector.py
+psycopg2_wrapper/NativeQueryExecutor.py
+psycopg2_wrapper/SimpleQueryExecutor.py
+psycopg2_wrapper/__init__.py
 psycopg2_wrappers.egg-info/PKG-INFO
 psycopg2_wrappers.egg-info/SOURCES.txt
 psycopg2_wrappers.egg-info/dependency_links.txt
 psycopg2_wrappers.egg-info/requires.txt
 psycopg2_wrappers.egg-info/top_level.txt
-src/DatabaseConnector.py
-src/NativeQueryExecutor.py
-src/SimpleQueryExecutor.py
-src/__init__.py
 tests/__init__.py
 tests/test_native_query_executor.py
 tests/test_simple_query_executor.py
```

### Comparing `psycopg2-wrappers-1.0.0/setup.py` & `psycopg2-wrappers-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-with open('requirements.txt') as f:
-    install_requires = f.read().splitlines()
-
-setup(
-    name='psycopg2-wrappers',
-    version='1.0.0',  # current_version
-    description='psycopg2-wrapper is a wrapper for psycopg2 that makes it easier to use.',
-    author='zestones',
-    author_email='idrissbenguezzou@gmail.com',
-    packages=find_packages(),
-    install_requires=install_requires,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
+from setuptools import setup, find_packages
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+with open('requirements.txt') as f:
+    install_requires = f.read().splitlines()
+
+setup(
+    name='psycopg2-wrappers',
+    version='1.0.1',  # current_version
+    description='psycopg2-wrapper is a wrapper for psycopg2 that makes it easier to use.',
+    author='zestones',
+    author_email='idrissbenguezzou@gmail.com',
+    packages=find_packages(),
+    install_requires=install_requires,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
 )
```

### Comparing `psycopg2-wrappers-1.0.0/src/DatabaseConnector.py` & `psycopg2-wrappers-1.0.1/psycopg2_wrapper/DatabaseConnector.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import psycopg2
-
-
-class DatabaseConnector:
-    """
-    This class is a wrapper around the psycopg2 library to simplify the connection and execution of SQL queries.
-    The class is designed to be inherited by all DAO classes in the project.
-    """
-
-    def __init__(self, db_params: dict) -> None:
-        """
-        Constructor that stores the database parameters to establish a connection.
-
-        Parameters:
-        ----------
-        db_params (dict): A dictionary containing the database parameters.
-            The dict is retrieved from the config.ini file.
-
-        Format:
-        -------
-        {
-            "database": "database_name",
-            "user": "username",
-            "password": "password",
-            "host": "host",
-            "port": "port"
-        }
-        """
-        # check if a key is missing and set it to None
-        keys = ["database", "user", "password", "host", "port"]                
-        self.db_params = {key: db_params.get(key, None) for key in keys}
-
-    def connect(self) -> psycopg2.extensions.connection:
-        """
-        Create a connection to the database.
-
-        Returns:
-        -------
-        returns a connection object.
-        """
-        conn = psycopg2.connect(
-            host=self.db_params["host"],
-            database=self.db_params['database'],
-            user=self.db_params["user"],
-            password=self.db_params["password"],
-            port=self.db_params["port"]
-        )
-
-        return conn
-
-    def close(self, cursor: psycopg2.extensions.cursor, conn: psycopg2.extensions.connection) -> None:
-        """
-        Close the cursor and connection objects.
-
-        Parameters:
-        ----------
-        - cursor: The cursor object to close.
-        - conn: The connection object to close.
-        """
-        cursor.close()
-        conn.close()
+import psycopg2
+
+
+class DatabaseConnector:
+    """
+    This class is a wrapper around the psycopg2 library to simplify the connection and execution of SQL queries.
+    The class is designed to be inherited by all DAO classes in the project.
+    """
+
+    def __init__(self, db_params: dict) -> None:
+        """
+        Constructor that stores the database parameters to establish a connection.
+
+        Parameters:
+        ----------
+        db_params (dict): A dictionary containing the database parameters.
+            The dict is retrieved from the config.ini file.
+
+        Format:
+        -------
+        {
+            "database": "database_name",
+            "user": "username",
+            "password": "password",
+            "host": "host",
+            "port": "port"
+        }
+        """
+        # check if a key is missing and set it to None
+        keys = ["database", "user", "password", "host", "port"]                
+        self.db_params = {key: db_params.get(key, None) for key in keys}
+
+    def connect(self) -> psycopg2.extensions.connection:
+        """
+        Create a connection to the database.
+
+        Returns:
+        -------
+        returns a connection object.
+        """
+        conn = psycopg2.connect(
+            host=self.db_params["host"],
+            database=self.db_params['database'],
+            user=self.db_params["user"],
+            password=self.db_params["password"],
+            port=self.db_params["port"]
+        )
+
+        return conn
+
+    def close(self, cursor: psycopg2.extensions.cursor, conn: psycopg2.extensions.connection) -> None:
+        """
+        Close the cursor and connection objects.
+
+        Parameters:
+        ----------
+        - cursor: The cursor object to close.
+        - conn: The connection object to close.
+        """
+        cursor.close()
+        conn.close()
```

### Comparing `psycopg2-wrappers-1.0.0/src/NativeQueryExecutor.py` & `psycopg2-wrappers-1.0.1/psycopg2_wrapper/NativeQueryExecutor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-from src.DatabaseConnector import DatabaseConnector
-
-class NativeQueryExecutor:
-    """
-    This class is responsible for executing SQL queries. 
-    It takes an instance of DatabaseConnector to establish a database connection.
-    """
-
-    def __init__(self, config: dict) -> None:
-        """
-        Constructor that takes an instance of DatabaseConnector to establish a database connection.
-
-        Parameters:
-        db_conn (DatabaseConnector): An instance of DatabaseConnector.
-        """
-        self.conn = DatabaseConnector(db_params=config)
-
-
-    def execute(self, sql: str, params: tuple = None) -> tuple:
-        """
-        Execute a SQL query.
-        
-        Parameters:
-        ----------
-        - sql: The SQL query to execute.
-        - params: The parameters to pass to the query.
-        
-        Returns:
-        -------
-        returns a cursor object and a connection object.
-        """
-        conn = self.conn.connect()
-        cursor = conn.cursor()
-
-        if params is None: cursor.execute(sql)
-        else: cursor.execute(sql, params)
-
-        return cursor, conn
-
-
-    def execute_and_commit(self, sql: str, params: tuple = None) -> None:
-        """
-        Execute a SQL query and commit the changes to the database.
-        
-        Parameters:
-        ----------
-        - sql: The SQL query to execute.
-        - params: The parameters to pass to the query.
-        """
-        cursor, conn = self.execute(sql, params)
-        conn.commit()  
-        self.conn.close(cursor, conn)
-        
-        
-    def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
-        """
-        Execute a SQL query and fetch the first result.
-        
-        Parameters:
-        ----------
-        - sql: The SQL query to execute.
-        - params: The parameters to pass to the query.
-        
-        Returns:
-        -------
-        returns a tuple with the result.
-        """
-        cursor, conn = self.execute(sql, params)
-        result = cursor.fetchone()
-
-        self.conn.close(cursor, conn)        
-        return result
-    
-    
-    def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
-        """
-        Execute a SQL query and fetch all the results.
-        
-        Parameters:
-        ----------
-        - sql: The SQL query to execute.
-        - params: The parameters to pass to the query.
-        
-        Returns:
-        -------
-        returns a list with the results.
-        """
-        cursor, conn = self.execute(sql, params)
-        result = cursor.fetchall()
-        
-        self.conn.close(cursor, conn)
-        return result
-    
-    
-    def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
-        """
-        Execute a SQL query and fetch a number of results.
-        
-        Parameters:
-        ----------
-        - sql: The SQL query to execute.
-        - params: The parameters to pass to the query.
-        - size: The number of results to fetch.
-        
-        Returns:
-        -------
-        returns a list with the results.
-        """
-        cursor, conn = self.execute(sql, params)
-        result = cursor.fetchmany(size)
-
-        self.conn.close(cursor, conn)
-        return result
-    
-    
-    def execute_many_and_commit(self, sql: str, params: list) -> None:
-        """
-        Execute a SQL query with multiple parameters.
-        
-        Parameters:
-        ----------
-        - sql: The SQL query to execute.
-        - params: A list of parameters to pass to the query.
-        """
-        conn = self.conn.connect()
-        cursor = conn.cursor()
-        
-        cursor.executemany(sql, params)
-        conn.commit()
-        
+from psycopg2_wrapper.DatabaseConnector import DatabaseConnector
+
+class NativeQueryExecutor:
+    """
+    This class is responsible for executing SQL queries. 
+    It takes an instance of DatabaseConnector to establish a database connection.
+    """
+
+    def __init__(self, config: dict) -> None:
+        """
+        Constructor that takes an instance of DatabaseConnector to establish a database connection.
+
+        Parameters:
+        db_conn (DatabaseConnector): An instance of DatabaseConnector.
+        """
+        self.conn = DatabaseConnector(db_params=config)
+
+
+    def execute(self, sql: str, params: tuple = None) -> tuple:
+        """
+        Execute a SQL query.
+        
+        Parameters:
+        ----------
+        - sql: The SQL query to execute.
+        - params: The parameters to pass to the query.
+        
+        Returns:
+        -------
+        returns a cursor object and a connection object.
+        """
+        conn = self.conn.connect()
+        cursor = conn.cursor()
+
+        if params is None: cursor.execute(sql)
+        else: cursor.execute(sql, params)
+
+        return cursor, conn
+
+
+    def execute_and_commit(self, sql: str, params: tuple = None) -> None:
+        """
+        Execute a SQL query and commit the changes to the database.
+        
+        Parameters:
+        ----------
+        - sql: The SQL query to execute.
+        - params: The parameters to pass to the query.
+        """
+        cursor, conn = self.execute(sql, params)
+        conn.commit()  
+        self.conn.close(cursor, conn)
+        
+        
+    def execute_and_fetchone(self, sql: str, params: tuple = None) -> tuple:
+        """
+        Execute a SQL query and fetch the first result.
+        
+        Parameters:
+        ----------
+        - sql: The SQL query to execute.
+        - params: The parameters to pass to the query.
+        
+        Returns:
+        -------
+        returns a tuple with the result.
+        """
+        cursor, conn = self.execute(sql, params)
+        result = cursor.fetchone()
+
+        self.conn.close(cursor, conn)        
+        return result
+    
+    
+    def execute_and_fetchall(self, sql: str, params: tuple = None) -> list:
+        """
+        Execute a SQL query and fetch all the results.
+        
+        Parameters:
+        ----------
+        - sql: The SQL query to execute.
+        - params: The parameters to pass to the query.
+        
+        Returns:
+        -------
+        returns a list with the results.
+        """
+        cursor, conn = self.execute(sql, params)
+        result = cursor.fetchall()
+        
+        self.conn.close(cursor, conn)
+        return result
+    
+    
+    def execute_and_fetchmany(self, sql: str, params: tuple = None, size: int = 2) -> list:
+        """
+        Execute a SQL query and fetch a number of results.
+        
+        Parameters:
+        ----------
+        - sql: The SQL query to execute.
+        - params: The parameters to pass to the query.
+        - size: The number of results to fetch.
+        
+        Returns:
+        -------
+        returns a list with the results.
+        """
+        cursor, conn = self.execute(sql, params)
+        result = cursor.fetchmany(size)
+
+        self.conn.close(cursor, conn)
+        return result
+    
+    
+    def execute_many_and_commit(self, sql: str, params: list) -> None:
+        """
+        Execute a SQL query with multiple parameters.
+        
+        Parameters:
+        ----------
+        - sql: The SQL query to execute.
+        - params: A list of parameters to pass to the query.
+        """
+        conn = self.conn.connect()
+        cursor = conn.cursor()
+        
+        cursor.executemany(sql, params)
+        conn.commit()
+        
         self.conn.close(cursor, conn)
```

### Comparing `psycopg2-wrappers-1.0.0/src/SimpleQueryExecutor.py` & `psycopg2-wrappers-1.0.1/psycopg2_wrapper/SimpleQueryExecutor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-from src.NativeQueryExecutor import NativeQueryExecutor
-from src.DatabaseConnector import DatabaseConnector
-
-
-class SimpleQueryExecutor(NativeQueryExecutor):
-    """
-    This class is responsible for executing SQL queries.
-    It extends the NativeQueryExecutor class to execute simple SQL queries.
-    """
-    
-    def __init__(self, config: dict) -> None:
-        """
-        Constructor that stores the DatabaseConnector instance.
-        """
-        super().__init__(config)
-
-
-    def create_table(self, table_name: str, columns: dict) -> None:
-        """
-        Create a new table in the database.
-
-        Parameters:
-        ----------
-        - table_name: The name of the table to create.
-        - columns: A dictionary containing the names and data types of the columns.
-        """
-        sql = f"CREATE TABLE {table_name} ({','.join([f'{col_name} {data_type}' for col_name, data_type in columns.items()])})"
-        self.execute_and_commit(sql)
-
-
-    def select_data(self, table_name: str, columns: list = None, where: str = None) -> list:
-        """
-        Select data from a table in the database.
-
-        Parameters:
-        ----------
-        - table_name: The name of the table to select from.
-        - columns: A list of column names to select.
-        - where: A WHERE clause to filter the results.
-
-        Returns:
-        -------
-        returns a list of tuples containing the selected data.
-        """
-        col_names = '*' if columns is None else ','.join(columns)
-        sql = f"SELECT {col_names} FROM {table_name}"
-        
-        if where is not None:
-            sql += f" WHERE {where}"
-        
-        return self.execute_and_fetchall(sql)
-    
-    
-    def insert_data(self, table_name: str, data: dict) -> None:
-        """
-        Insert data into a table in the database.
-
-        Parameters:
-        ----------
-        - table_name: The name of the table to insert into.
-        - data: A dictionary containing the column names and values to insert.
-        """
-        sql = f"INSERT INTO {table_name} ({','.join(data.keys())}) VALUES ({','.join(['%s' for _ in range(len(data))])})"
-        self.execute_and_commit(sql, tuple(data.values()))
-        
-
-    def drop_table(self, table_name: str) -> None:
-        """
-        Drop a table from the database.
-
-        Parameters:
-        ----------
-        - table_name: The name of the table to drop.
-        """
-        sql = f"DROP TABLE IF EXISTS {table_name}"
-        self.execute_and_commit(sql)
+from psycopg2_wrapper.NativeQueryExecutor import NativeQueryExecutor
+from psycopg2_wrapper.DatabaseConnector import DatabaseConnector
+
+
+class SimpleQueryExecutor(NativeQueryExecutor):
+    """
+    This class is responsible for executing SQL queries.
+    It extends the NativeQueryExecutor class to execute simple SQL queries.
+    """
+    
+    def __init__(self, config: dict) -> None:
+        """
+        Constructor that stores the DatabaseConnector instance.
+        """
+        super().__init__(config)
+
+
+    def create_table(self, table_name: str, columns: dict) -> None:
+        """
+        Create a new table in the database.
+
+        Parameters:
+        ----------
+        - table_name: The name of the table to create.
+        - columns: A dictionary containing the names and data types of the columns.
+        """
+        sql = f"CREATE TABLE {table_name} ({','.join([f'{col_name} {data_type}' for col_name, data_type in columns.items()])})"
+        self.execute_and_commit(sql)
+
+
+    def select_data(self, table_name: str, columns: list = None, where: str = None) -> list:
+        """
+        Select data from a table in the database.
+
+        Parameters:
+        ----------
+        - table_name: The name of the table to select from.
+        - columns: A list of column names to select.
+        - where: A WHERE clause to filter the results.
+
+        Returns:
+        -------
+        returns a list of tuples containing the selected data.
+        """
+        col_names = '*' if columns is None else ','.join(columns)
+        sql = f"SELECT {col_names} FROM {table_name}"
+        
+        if where is not None:
+            sql += f" WHERE {where}"
+        
+        return self.execute_and_fetchall(sql)
+    
+    
+    def insert_data(self, table_name: str, data: dict) -> None:
+        """
+        Insert data into a table in the database.
+
+        Parameters:
+        ----------
+        - table_name: The name of the table to insert into.
+        - data: A dictionary containing the column names and values to insert.
+        """
+        sql = f"INSERT INTO {table_name} ({','.join(data.keys())}) VALUES ({','.join(['%s' for _ in range(len(data))])})"
+        self.execute_and_commit(sql, tuple(data.values()))
+        
+
+    def drop_table(self, table_name: str) -> None:
+        """
+        Drop a table from the database.
+
+        Parameters:
+        ----------
+        - table_name: The name of the table to drop.
+        """
+        sql = f"DROP TABLE IF EXISTS {table_name}"
+        self.execute_and_commit(sql)
```

### Comparing `psycopg2-wrappers-1.0.0/tests/test_native_query_executor.py` & `psycopg2-wrappers-1.0.1/tests/test_native_query_executor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-from src.NativeQueryExecutor import NativeQueryExecutor
-from src.DatabaseConnector import DatabaseConnector
-
-import pytest
-import psycopg2
-
-from . import DATABASE_PARAMS
-
-@pytest.fixture(scope="session")
-def db_params():
-    # create a test database and return the database parameters
-    conn = psycopg2.connect(
-        host=DATABASE_PARAMS["host"],
-        user=DATABASE_PARAMS["user"],
-        password=DATABASE_PARAMS["password"]
-    )
-    
-    conn.set_isolation_level(0)
-    cur = conn.cursor()
-    cur.execute(f"CREATE DATABASE {DATABASE_PARAMS['database']}")
-    conn.close()
-    
-    return DATABASE_PARAMS
-
-
-@pytest.fixture(scope="function")
-def query_execution(db_params):
-    # create a NativeQueryExecutor instance for the test database
-    return NativeQueryExecutor(db_params)
-
-
-def test_execute_and_commit(query_execution):
-
-    sql = "CREATE TABLE test_table (id SERIAL PRIMARY KEY, name TEXT)"
-    query_execution.execute_and_commit(sql)
-
-    sql = "INSERT INTO test_table (name) VALUES (%s)"
-    params = ("test_name",)
-    query_execution.execute_and_commit(sql, params)
-
-    sql = "SELECT name FROM test_table WHERE id=1"
-    result = query_execution.execute_and_fetchone(sql)
-    assert result == ("test_name",)
-
-
-def test_execute_and_fetchone(query_execution):
-    
-    sql = "SELECT name FROM test_table WHERE id=1"
-    result = query_execution.execute_and_fetchone(sql)
-    
-    assert result == ("test_name",)
-
-
-def test_execute_and_fetchall(query_execution):
-    
-    sql = "SELECT name FROM test_table"
-    result = query_execution.execute_and_fetchall(sql)
-    
-    assert result == [("test_name",)]
-
-
-def test_execute_and_fetchmany(query_execution):
-    # test the execute_and_fetchmany method
-    sql = "SELECT name FROM test_table"
-    result = query_execution.execute_and_fetchmany(sql, size=1)
-    assert result == [("test_name",)]
-
-
-def test_execute_many_and_commit(query_execution):
-
-    # test the execute_many_and_commit method
-    sql = "INSERT INTO test_table (name) VALUES (%s)"
-    params = [("test_name_2",), ("test_name_3",)]
-    query_execution.execute_many_and_commit(sql, params)
-
-    sql = "SELECT name FROM test_table ORDER BY id"
-    result = query_execution.execute_and_fetchall(sql)
-    assert result == [("test_name",), ("test_name_2",), ("test_name_3",)]
-
-
-@pytest.fixture(scope="session", autouse=True)
-def drop_test_db(request):
-    # drop the test database after all tests are finished
-    def finalizer():
-
-        conn = psycopg2.connect(
-            host=DATABASE_PARAMS["host"],
-            user=DATABASE_PARAMS["user"],
-            password=DATABASE_PARAMS["password"]
-        )
-
-        conn.set_isolation_level(0)
-        cur = conn.cursor()
-        cur.execute(f"DROP DATABASE IF EXISTS {DATABASE_PARAMS['database']}")
-        conn.close()
-
+from psycopg2_wrapper.NativeQueryExecutor import NativeQueryExecutor
+from psycopg2_wrapper.DatabaseConnector import DatabaseConnector
+
+import pytest
+import psycopg2
+
+from . import DATABASE_PARAMS
+
+@pytest.fixture(scope="session")
+def db_params():
+    # create a test database and return the database parameters
+    conn = psycopg2.connect(
+        host=DATABASE_PARAMS["host"],
+        user=DATABASE_PARAMS["user"],
+        password=DATABASE_PARAMS["password"]
+    )
+    
+    conn.set_isolation_level(0)
+    cur = conn.cursor()
+    cur.execute(f"CREATE DATABASE {DATABASE_PARAMS['database']}")
+    conn.close()
+    
+    return DATABASE_PARAMS
+
+
+@pytest.fixture(scope="function")
+def query_execution(db_params):
+    # create a NativeQueryExecutor instance for the test database
+    return NativeQueryExecutor(db_params)
+
+
+def test_execute_and_commit(query_execution):
+
+    sql = "CREATE TABLE test_table (id SERIAL PRIMARY KEY, name TEXT)"
+    query_execution.execute_and_commit(sql)
+
+    sql = "INSERT INTO test_table (name) VALUES (%s)"
+    params = ("test_name",)
+    query_execution.execute_and_commit(sql, params)
+
+    sql = "SELECT name FROM test_table WHERE id=1"
+    result = query_execution.execute_and_fetchone(sql)
+    assert result == ("test_name",)
+
+
+def test_execute_and_fetchone(query_execution):
+    
+    sql = "SELECT name FROM test_table WHERE id=1"
+    result = query_execution.execute_and_fetchone(sql)
+    
+    assert result == ("test_name",)
+
+
+def test_execute_and_fetchall(query_execution):
+    
+    sql = "SELECT name FROM test_table"
+    result = query_execution.execute_and_fetchall(sql)
+    
+    assert result == [("test_name",)]
+
+
+def test_execute_and_fetchmany(query_execution):
+    # test the execute_and_fetchmany method
+    sql = "SELECT name FROM test_table"
+    result = query_execution.execute_and_fetchmany(sql, size=1)
+    assert result == [("test_name",)]
+
+
+def test_execute_many_and_commit(query_execution):
+
+    # test the execute_many_and_commit method
+    sql = "INSERT INTO test_table (name) VALUES (%s)"
+    params = [("test_name_2",), ("test_name_3",)]
+    query_execution.execute_many_and_commit(sql, params)
+
+    sql = "SELECT name FROM test_table ORDER BY id"
+    result = query_execution.execute_and_fetchall(sql)
+    assert result == [("test_name",), ("test_name_2",), ("test_name_3",)]
+
+
+@pytest.fixture(scope="session", autouse=True)
+def drop_test_db(request):
+    # drop the test database after all tests are finished
+    def finalizer():
+
+        conn = psycopg2.connect(
+            host=DATABASE_PARAMS["host"],
+            user=DATABASE_PARAMS["user"],
+            password=DATABASE_PARAMS["password"]
+        )
+
+        conn.set_isolation_level(0)
+        cur = conn.cursor()
+        cur.execute(f"DROP DATABASE IF EXISTS {DATABASE_PARAMS['database']}")
+        conn.close()
+
     request.addfinalizer(finalizer)
```

### Comparing `psycopg2-wrappers-1.0.0/tests/test_simple_query_executor.py` & `psycopg2-wrappers-1.0.1/tests/test_simple_query_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-import pytest
-import psycopg2
-
-from src.SimpleQueryExecutor import SimpleQueryExecutor
-from src.DatabaseConnector import DatabaseConnector
-
-from . import DATABASE_PARAMS
-
-
-@pytest.fixture(scope="session")
-def db_params():
-    # create a test database and return the database parameters
-    conn = psycopg2.connect(
-        host=DATABASE_PARAMS["host"],
-        user=DATABASE_PARAMS["user"],
-        password=DATABASE_PARAMS["password"]
-    )
-    
-    conn.set_isolation_level(0)
-    cur = conn.cursor()
-    cur.execute(f"CREATE DATABASE {DATABASE_PARAMS['database']}")
-    conn.close()
-    
-    return DATABASE_PARAMS
-
-
-@pytest.fixture(scope="function")
-def query_executor(db_params):
-    query_executor = SimpleQueryExecutor(config=db_params)
-    yield query_executor
-
-
-def test_create_table(query_executor):
-    query_executor.create_table("test_table", {"id": "INTEGER PRIMARY KEY", "name": "TEXT"})
-    assert len(query_executor.select_data("test_table")) == 0
-
-
-def test_select_data(query_executor):
-    data = {"id": 1, "name": "John"}
-    query_executor.insert_data("test_table", data)
-    assert query_executor.select_data("test_table", where="id=1") == [(1, "John")]
-
-
-def test_insert_data(query_executor):
-    data = {"id": 2, "name": "Jane"}
-    query_executor.insert_data("test_table", data)
-    assert query_executor.select_data("test_table", where="id=2") == [(2, "Jane")]
-
-
-def test_drop_table(query_executor):
-    query_executor.create_table("test_table_2", {"id": "INTEGER PRIMARY KEY", "name": "TEXT"})
-    query_executor.drop_table("test_table_2")
-    with pytest.raises(Exception):
-        query_executor.select_data("test_table_2")
-        
-
-@pytest.fixture(scope="session", autouse=True)
-def drop_test_db(request):
-    # drop the test database after all tests are finished
-    def finalizer():
-
-        conn = psycopg2.connect(
-            host=DATABASE_PARAMS["host"],
-            user=DATABASE_PARAMS["user"],
-            password=DATABASE_PARAMS["password"]
-        )
-
-        conn.set_isolation_level(0)
-        cur = conn.cursor()
-        cur.execute(f"DROP DATABASE IF EXISTS {DATABASE_PARAMS['database']}")
-        conn.close()
-
+import pytest
+import psycopg2
+
+from psycopg2_wrapper.SimpleQueryExecutor import SimpleQueryExecutor
+from psycopg2_wrapper.DatabaseConnector import DatabaseConnector
+
+from . import DATABASE_PARAMS
+
+
+@pytest.fixture(scope="session")
+def db_params():
+    # create a test database and return the database parameters
+    conn = psycopg2.connect(
+        host=DATABASE_PARAMS["host"],
+        user=DATABASE_PARAMS["user"],
+        password=DATABASE_PARAMS["password"]
+    )
+    
+    conn.set_isolation_level(0)
+    cur = conn.cursor()
+    cur.execute(f"CREATE DATABASE {DATABASE_PARAMS['database']}")
+    conn.close()
+    
+    return DATABASE_PARAMS
+
+
+@pytest.fixture(scope="function")
+def query_executor(db_params):
+    query_executor = SimpleQueryExecutor(config=db_params)
+    yield query_executor
+
+
+def test_create_table(query_executor):
+    query_executor.create_table("test_table", {"id": "INTEGER PRIMARY KEY", "name": "TEXT"})
+    assert len(query_executor.select_data("test_table")) == 0
+
+
+def test_select_data(query_executor):
+    data = {"id": 1, "name": "John"}
+    query_executor.insert_data("test_table", data)
+    assert query_executor.select_data("test_table", where="id=1") == [(1, "John")]
+
+
+def test_insert_data(query_executor):
+    data = {"id": 2, "name": "Jane"}
+    query_executor.insert_data("test_table", data)
+    assert query_executor.select_data("test_table", where="id=2") == [(2, "Jane")]
+
+
+def test_drop_table(query_executor):
+    query_executor.create_table("test_table_2", {"id": "INTEGER PRIMARY KEY", "name": "TEXT"})
+    query_executor.drop_table("test_table_2")
+    with pytest.raises(Exception):
+        query_executor.select_data("test_table_2")
+        
+
+@pytest.fixture(scope="session", autouse=True)
+def drop_test_db(request):
+    # drop the test database after all tests are finished
+    def finalizer():
+
+        conn = psycopg2.connect(
+            host=DATABASE_PARAMS["host"],
+            user=DATABASE_PARAMS["user"],
+            password=DATABASE_PARAMS["password"]
+        )
+
+        conn.set_isolation_level(0)
+        cur = conn.cursor()
+        cur.execute(f"DROP DATABASE IF EXISTS {DATABASE_PARAMS['database']}")
+        conn.close()
+
     request.addfinalizer(finalizer)
```

