# Comparing `tmp/tooljob-0.1.1.tar.gz` & `tmp/tooljob-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooljob-0.1.1.tar", last modified: Fri Apr 21 17:02:15 2023, max compression
+gzip compressed data, was "tooljob-0.1.2.tar", last modified: Fri Apr 28 23:06:17 2023, max compression
```

## Comparing `tooljob-0.1.1.tar` & `tooljob-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.1/.gitignore
--rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.1/README.md
--rw-r--r--   0        0        0      274 2023-02-26 19:46:21.973498 tooljob-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      147 2023-04-21 17:02:01.127171 tooljob-0.1.1/tooljob/__init__.py
--rw-r--r--   0        0        0    10649 2023-03-11 05:04:06.934849 tooljob-0.1.1/tooljob/batch_class.py
--rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.1/tooljob/py.typed
--rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.1/tooljob/spec/__init__.py
--rw-r--r--   0        0        0       95 2023-02-08 03:46:38.161669 tooljob-0.1.1/tooljob/spec/typedefs.py
--rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.1/tooljob/trackers/__init__.py
--rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.1/tooljob/trackers/bucket_tracker.py
--rw-r--r--   0        0        0     2924 2023-03-26 06:26:00.899974 tooljob-0.1.1/tooljob/trackers/file_tracker.py
--rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.1/tooljob/trackers/sql_tracker.py
--rw-r--r--   0        0        0      535 2023-02-26 07:49:26.664051 tooljob-0.1.1/tooljob/trackers/tracker.py
--rw-r--r--   0        0        0     1504 2023-03-11 04:42:48.891916 tooljob-0.1.1/tooljob/trackers/tracker_utils.py
--rw-r--r--   0        0        0      127 1970-01-01 00:00:00.000000 tooljob-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.2/.gitignore
+-rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.2/README.md
+-rw-r--r--   0        0        0      274 2023-02-26 19:46:21.973498 tooljob-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-04-28 23:05:54.968891 tooljob-0.1.2/tooljob/__init__.py
+-rw-r--r--   0        0        0    10754 2023-04-28 23:04:57.498088 tooljob-0.1.2/tooljob/batch_class.py
+-rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.2/tooljob/py.typed
+-rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.2/tooljob/spec/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-28 23:01:22.123067 tooljob-0.1.2/tooljob/spec/typedefs.py
+-rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.2/tooljob/trackers/__init__.py
+-rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.2/tooljob/trackers/bucket_tracker.py
+-rw-r--r--   0        0        0     2932 2023-04-28 23:01:49.155581 tooljob-0.1.2/tooljob/trackers/file_tracker.py
+-rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.2/tooljob/trackers/sql_tracker.py
+-rw-r--r--   0        0        0      535 2023-02-26 07:49:26.664051 tooljob-0.1.2/tooljob/trackers/tracker.py
+-rw-r--r--   0        0        0     1511 2023-04-28 23:05:06.236075 tooljob-0.1.2/tooljob/trackers/tracker_utils.py
+-rw-r--r--   0        0        0      127 1970-01-01 00:00:00.000000 tooljob-0.1.2/PKG-INFO
```

### Comparing `tooljob-0.1.1/README.md` & `tooljob-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.1/tooljob/batch_class.py` & `tooljob-0.1.2/tooljob/batch_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 from __future__ import annotations
 
 import concurrent
-import hashlib
-import json
 import time
 import typing
 
-from typing_extensions import Literal
-
 if typing.TYPE_CHECKING:
-    import polars as pl
+    from typing_extensions import Literal
 
+    import polars as pl
     import toolsql
 
-import toolstr
-import tooltime
-
 from . import spec
 from . import trackers
 
 
 class Batch:
-
     name: str | None = None
     parameters: typing.Sequence[str]
     jobs: typing.Sequence[spec.JobData] | None = None
 
     #
     # # manadatory implementations
     #
@@ -44,15 +37,14 @@
         tracker: str | None = None,
         output_dir: str | None = None,
         output_filetype: str | None = None,
         db_config: toolsql.DBConfig | None = None,
         bucket_path: str | None = None,
         name: str | None = None,
     ) -> None:
-
         self.name = name
         self.jobs = jobs
         self.tracker = trackers.create_tracker(
             tracker=tracker,
             output_dir=output_dir,
             output_filetype=output_filetype,
             db_config=db_config,
@@ -156,14 +148,17 @@
     #
     # # hashes
     #
 
     def get_job_hash(
         self, i: int | None = None, *, job_data: spec.JobData | None = None
     ) -> str:
+        import hashlib
+        import json
+
         if job_data is None:
             if i is None:
                 raise Exception('must specify i or job_hash')
             job_data = self.get_job_data(i)
         job_data_str = json.dumps(job_data, sort_keys=True)
         job_hash = hashlib.md5(job_data_str.encode()).hexdigest()
         return job_hash
@@ -185,14 +180,15 @@
     #
 
     def orchestrate_jobs(
         self,
         executor: Literal['serial', 'parallel'] = 'parallel',
         n_processes: int | None = None,
     ) -> None:
+        import tooltime
 
         self.print_status()
 
         remaining_jobs = self.get_remaining_jobs()
         if len(remaining_jobs) == 0:
             print('\nAll jobs already completed')
             return
@@ -287,30 +283,36 @@
             raise Exception('must specify indices or job_datas')
 
     #
     # # summary
     #
 
     def print_status(self) -> None:
+        import toolstr
+
         toolstr.print_text_box(str(type(self).__name__) + ' Job Summary')
         print('- n_jobs:', self.get_n_jobs())
         print('- n_remaining:', len(self.get_remaining_jobs()))
 
     def print_summary(self) -> None:
+        import toolstr
+
         toolstr.print_header('Parameters')
         for parameter in self.parameters:
             toolstr.print_bullet(key=parameter, value=getattr(self, parameter))
 
     def print_conclusion(
         self,
         start_time: int | float,
         end_time: int | float,
         jobs: typing.Sequence[int],
         **kwargs: typing.Any,
     ) -> None:
+        import toolstr
+        import tooltime
 
         print('end time: ', tooltime.timestamp_to_iso_pretty(end_time))
 
         done_jobs = len([self.tracker.is_job_complete(i) for i in jobs])
         print(done_jobs, 'jobs completed')
 
         duration = end_time - start_time
@@ -332,21 +334,20 @@
         )
         print(
             '- jobs per day:',
             toolstr.format(jobs_per_second * 86400, decimals=2),
         )
 
     def summarize_jobs_per_second(self, sample_time: int = 60) -> pl.DataFrame:
-
         import polars as pl
 
         names = [self.get_job_name(i) for i in range(self.get_n_jobs())]
         times = [self.get_job_end_time(i) for i in range(self.get_n_jobs())]
         df = pl.from_dict({'job': names, 'times': times})
-        df = df.with_column(
+        df = df.with_columns(
             (pl.col('times') / sample_time).cast(int).alias('sample')
         )
         df = df.with_columns(
             [
                 pl.col('job'),
                 pl.count().over('sample').alias('jobs_per_second')
                 / sample_time,
```

### Comparing `tooljob-0.1.1/tooljob/trackers/file_tracker.py` & `tooljob-0.1.2/tooljob/trackers/file_tracker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import annotations
 
 import os
 import typing
 
-import toolstr
-
 from .. import spec
 from . import tracker
 
 
 class FileTracker(tracker.Tracker):
 
     output_dir: str
@@ -89,14 +87,16 @@
         path = self.get_job_output_path(i)
         if os.path.isfile(path):
             return os.path.getmtime(path)
         else:
             return None
 
     def print_status(self) -> None:
+        import toolstr
+
         dirsize = 0
         for f in os.listdir(self.output_dir):
             path = os.path.join(self.output_dir, f)
             if os.path.isfile(path):
                 dirsize += os.path.getsize(path)
         print('- output_dir size:', toolstr.format_nbytes(dirsize))
```

### Comparing `tooljob-0.1.1/tooljob/trackers/sql_tracker.py` & `tooljob-0.1.2/tooljob/trackers/sql_tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.1/tooljob/trackers/tracker.py` & `tooljob-0.1.2/tooljob/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.1/tooljob/trackers/tracker_utils.py` & `tooljob-0.1.2/tooljob/trackers/tracker_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def create_tracker(
     tracker: str | None = None,
     output_dir: str | None = None,
     output_filetype: str | None = None,
     db_config: toolsql.DBConfig | None = None,
     bucket_path: str | None = None,
-    batch: batch_class.Batch = None,
+    batch: batch_class.Batch | None = None,
 ) -> tracker.Tracker:
 
     if tracker is None:
         pass
 
     if tracker == 'file':
         from . import file_tracker
```

