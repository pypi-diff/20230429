# Comparing `tmp/pg_force_execute-0.0.3.tar.gz` & `tmp/pg_force_execute-0.0.4.tar.gz`

## Comparing `pg_force_execute-0.0.3.tar` & `pg_force_execute-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/pg_force_execute.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/LICENSE
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/README.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 pg_force_execute-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 pg_force_execute-0.0.4/pg_force_execute.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 pg_force_execute-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pg_force_execute-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 pg_force_execute-0.0.4/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 pg_force_execute-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 pg_force_execute-0.0.4/PKG-INFO
```

### Comparing `pg_force_execute-0.0.3/pg_force_execute.py` & `pg_force_execute-0.0.4/pg_force_execute.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,55 +4,63 @@
 
 import sqlalchemy as sa
 
 
 def pg_force_execute(query, conn, engine,
                      delay=datetime.timedelta(minutes=5),
                      check_interval=datetime.timedelta(seconds=1),
-                     cancel_timeout=datetime.timedelta(seconds=10),
+                     termination_thread_timeout=datetime.timedelta(seconds=10),
                      logger=logging.getLogger("pg_force_execute"),
 ):
+    cancel_exception = None
 
     def force_unblock(pid, exit):
-        exit.wait(timeout=delay.total_seconds())
+        nonlocal cancel_exception
 
-        # Repeatedly check for other backends that block `query`, and cancel them if
-        # they are. The repeat check is to avoid race conditions - if another backend
-        # blocks this backend just after pg_blocking_pids returns its PIDs. If it's
-        # determined that PostgreSQL forbids this case the looping can be removed
-        while not exit.wait(timeout=check_interval.total_seconds()):
-            logger.info('Cancelling queries blocking PID %s running %s', pid, query)
-            with engine.begin() as conn:
-                # pg_cancel_backend isn't strong enough - the blocking PIDs might not be
-                # actually running a query, so there is nothing to cancel. They might
-                # just be holding locks. To force release of the locks, we have to call
-                # pg_terminate_backend
-                cancelled_queries = conn.execute(
-                    sa.text("""
-                        SELECT
-                            activity.usename AS usename,
-                            activity.query AS query,
-                            age(clock_timestamp(), activity.query_start) AS age,
-                            pg_terminate_backend(pids.pid)
-                        FROM
-                            UNNEST(pg_blocking_pids(:pid)) AS pids(pid)
-                        INNER JOIN
-                            pg_stat_activity activity ON activity.pid = pids.pid;
-                    """), {"pid": pid},
-                ).fetchall()
-                if not cancelled_queries:
-                    logger.info('No blocking queries to cancel')
-                for cancelled_query in cancelled_queries:
-                    logger.error('Cancelled blocking query %s', cancelled_query)
+        try:
+            exit.wait(timeout=(delay - check_interval).total_seconds())
+
+            # Repeatedly check for other backends that block `query`, and cancel them if
+            # they are. The repeat check is to avoid race conditions - if another backend
+            # blocks this backend just after pg_blocking_pids returns its PIDs. If it's
+            # determined that PostgreSQL forbids this case the looping can be removed
+            while not exit.wait(timeout=check_interval.total_seconds()):
+                logger.info('Cancelling queries blocking PID %s running %s', pid, query)
+                with engine.begin() as conn:
+                    # pg_cancel_backend isn't strong enough - the blocking PIDs might not be
+                    # actually running a query, so there is nothing to cancel. They might
+                    # just be holding locks. To force release of the locks, we have to call
+                    # pg_terminate_backend
+                    cancelled_queries = conn.execute(
+                        sa.text("""
+                            SELECT
+                                activity.usename AS usename,
+                                activity.query AS query,
+                                age(clock_timestamp(), activity.query_start) AS age,
+                                pg_terminate_backend(pids.pid)
+                            FROM
+                                UNNEST(pg_blocking_pids(:pid)) AS pids(pid)
+                            INNER JOIN
+                                pg_stat_activity activity ON activity.pid = pids.pid;
+                        """), {"pid": pid},
+                    ).fetchall()
+                    if not cancelled_queries:
+                        logger.info('No blocking queries to cancel')
+                    for cancelled_query in cancelled_queries:
+                        logger.error('Cancelled blocking query %s', cancelled_query)
+        except Exception as e:
+            cancel_exception = e
 
     pid = conn.execute(
         sa.text('SELECT pg_backend_pid()')
     ).fetchall()[0][0]
     exit = Event()
     t = Thread(target=force_unblock, args=(pid, exit))
     t.start()
 
     try:
         return conn.execute(query)
     finally:
         exit.set()
-        t.join(timeout=cancel_timeout.total_seconds())
+        t.join(timeout=termination_thread_timeout.total_seconds())
+        if cancel_exception is not None:
+            raise cancel_exception
```

### Comparing `pg_force_execute-0.0.3/.gitignore` & `pg_force_execute-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.3/LICENSE` & `pg_force_execute-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_force_execute-0.0.3/pyproject.toml` & `pg_force_execute-0.0.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg-force-execute"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Department for International Trade", email="sre@digital.trade.gov.uk" },
 ]
-description = "Utility function to run a PostgreSQL query with SQLAlchemy, terminating any queries that block it"
+description = "Utility function to run a PostgreSQL query with SQLAlchemy, terminating any other clients that block it"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `pg_force_execute-0.0.3/PKG-INFO` & `pg_force_execute-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pg-force-execute
-Version: 0.0.3
-Summary: Utility function to run a PostgreSQL query with SQLAlchemy, terminating any queries that block it
+Version: 0.0.4
+Summary: Utility function to run a PostgreSQL query with SQLAlchemy, terminating any other clients that block it
 Project-URL: Source, https://github.com/uktrade/pg-force-execute
 Author-email: Department for International Trade <sre@digital.trade.gov.uk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -13,25 +13,27 @@
 Provides-Extra: dev
 Requires-Dist: psycopg2-binary>=2.8.6; extra == 'dev'
 Requires-Dist: pytest>=7.2.1; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # pg-force-execute
 
-Utility function to run a PostgreSQL query with SQLAlchemy, terminating any queries that continue to block it after a configurable delay.
+Utility function to run a PostgreSQL query with SQLAlchemy, terminating any other clients that continue to block it after a configurable delay.
+
+Using this function to run queries is somewhat of a last resort, but is useful in certain Extract Transform Load (ETL) pipeline contexts. For example, if it is more important to replace one table with another than to allow running queries on the table to complete, then this function can be used to run the relevant `ALTER TABLE RENAME TO` query.
 
 
 ## Installation
 
 ```bash
 pip install pg-force-execute
 ```
 
 
-## Usage
+## Example usage
 
 ```python
 import datetime
 import sqlalchemy as sa
 from pg_force_execute import pg_force_execute
 
 # Run postgresql locally should allow the below to run
@@ -47,14 +49,35 @@
         engine,         # SQLAlchemy engine that will create new connections to cancel blocking queries
         delay=datetime.timedelta(minutes=5),  # Amount of time to wait before cancelling queries
     )
     print(results.fetchall())
 ```
 
 
+## API
+
+The API a single function `pg_force_execute`.
+
+`pg_force_execute`(query, conn, engine, delay=datetime.timedelta(minutes=5), check_interval=datetime.timedelta(seconds=1), termination_thread_timeout=datetime.timedelta(seconds=10), logger=logging.getLogger("pg_force_execute"))
+
+- `query` - A SQLAlchemy text instance of the query to run
+
+- `conn` - A SQLAlchemy connection to run `query` on
+
+- `engine` - A SQLAlchemy engine to create a new connection that will be used to terminate backends blocking `query`
+
+- `delay` (optional) - How long to wait before attempting to terminate backends blocking `query`
+
+- `check_interval` (optional) - The interval between repeated attempted to terminate backends blocking `query`
+
+- `termination_thread_timeout` (optional) - How long to wait for the termination to complete
+
+- `logger` (optional) The Python logger instance through which to log
+
+
 ## Running tests locally
 
 ```bash
 pip install -e ".[dev]"  # Only needed once
 ./start-services.sh      # Only needed once
 pytest
 ```
```

