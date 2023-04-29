# Comparing `tmp/tooljob-0.1.2.tar.gz` & `tmp/tooljob-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooljob-0.1.2.tar", last modified: Fri Apr 28 23:06:17 2023, max compression
+gzip compressed data, was "tooljob-0.1.3.tar", last modified: Sat Apr 29 17:53:27 2023, max compression
```

## Comparing `tooljob-0.1.2.tar` & `tooljob-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.2/.gitignore
--rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.2/README.md
--rw-r--r--   0        0        0      274 2023-02-26 19:46:21.973498 tooljob-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      147 2023-04-28 23:05:54.968891 tooljob-0.1.2/tooljob/__init__.py
--rw-r--r--   0        0        0    10754 2023-04-28 23:04:57.498088 tooljob-0.1.2/tooljob/batch_class.py
--rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.2/tooljob/py.typed
--rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.2/tooljob/spec/__init__.py
--rw-r--r--   0        0        0      124 2023-04-28 23:01:22.123067 tooljob-0.1.2/tooljob/spec/typedefs.py
--rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.2/tooljob/trackers/__init__.py
--rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.2/tooljob/trackers/bucket_tracker.py
--rw-r--r--   0        0        0     2932 2023-04-28 23:01:49.155581 tooljob-0.1.2/tooljob/trackers/file_tracker.py
--rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.2/tooljob/trackers/sql_tracker.py
--rw-r--r--   0        0        0      535 2023-02-26 07:49:26.664051 tooljob-0.1.2/tooljob/trackers/tracker.py
--rw-r--r--   0        0        0     1511 2023-04-28 23:05:06.236075 tooljob-0.1.2/tooljob/trackers/tracker_utils.py
--rw-r--r--   0        0        0      127 1970-01-01 00:00:00.000000 tooljob-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      217 2023-02-26 19:33:55.835763 tooljob-0.1.3/.gitignore
+-rw-r--r--   0        0        0      742 2023-02-26 02:20:54.175448 tooljob-0.1.3/README.md
+-rw-r--r--   0        0        0      274 2023-02-26 19:46:21.973498 tooljob-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-04-29 17:53:03.211684 tooljob-0.1.3/tooljob/__init__.py
+-rw-r--r--   0        0        0    12952 2023-04-29 16:07:02.844212 tooljob-0.1.3/tooljob/batch_class.py
+-rw-r--r--   0        0        0        0 2023-04-10 03:48:04.176428 tooljob-0.1.3/tooljob/py.typed
+-rw-r--r--   0        0        0       68 2023-02-26 07:21:03.717968 tooljob-0.1.3/tooljob/spec/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-28 23:01:22.123067 tooljob-0.1.3/tooljob/spec/typedefs.py
+-rw-r--r--   0        0        0       29 2023-02-26 07:48:30.506903 tooljob-0.1.3/tooljob/trackers/__init__.py
+-rw-r--r--   0        0        0      197 2023-02-26 06:53:20.062932 tooljob-0.1.3/tooljob/trackers/bucket_tracker.py
+-rw-r--r--   0        0        0     2932 2023-04-28 23:01:49.155581 tooljob-0.1.3/tooljob/trackers/file_tracker.py
+-rw-r--r--   0        0        0     5358 2023-02-26 19:46:45.227524 tooljob-0.1.3/tooljob/trackers/sql_tracker.py
+-rw-r--r--   0        0        0      535 2023-02-26 07:49:26.664051 tooljob-0.1.3/tooljob/trackers/tracker.py
+-rw-r--r--   0        0        0     1514 2023-04-28 23:07:49.016212 tooljob-0.1.3/tooljob/trackers/tracker_utils.py
+-rw-r--r--   0        0        0      127 1970-01-01 00:00:00.000000 tooljob-0.1.3/PKG-INFO
```

### Comparing `tooljob-0.1.2/README.md` & `tooljob-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.2/tooljob/batch_class.py` & `tooljob-0.1.3/tooljob/batch_class.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import time
 import typing
 
 if typing.TYPE_CHECKING:
     from typing_extensions import Literal
 
     import polars as pl
+    import toolcli
     import toolsql
 
 from . import spec
 from . import trackers
 
 
 class Batch:
     name: str | None = None
-    parameters: typing.Sequence[str]
     jobs: typing.Sequence[spec.JobData] | None = None
 
     #
     # # manadatory implementations
     #
 
     def execute_job(self, i: int) -> typing.Any:
@@ -36,17 +36,21 @@
         jobs: typing.Sequence[spec.JobData] | None = None,
         tracker: str | None = None,
         output_dir: str | None = None,
         output_filetype: str | None = None,
         db_config: toolsql.DBConfig | None = None,
         bucket_path: str | None = None,
         name: str | None = None,
+        styles: toolcli.StyleTheme | None = None,
+        verbose: bool = False,
     ) -> None:
         self.name = name
         self.jobs = jobs
+        self.styles = styles
+        self.verbose = verbose
         self.tracker = trackers.create_tracker(
             tracker=tracker,
             output_dir=output_dir,
             output_filetype=output_filetype,
             db_config=db_config,
             bucket_path=bucket_path,
             batch=self,
@@ -180,26 +184,32 @@
     #
 
     def orchestrate_jobs(
         self,
         executor: Literal['serial', 'parallel'] = 'parallel',
         n_processes: int | None = None,
     ) -> None:
+        import toolstr
         import tooltime
 
         self.print_status()
 
         remaining_jobs = self.get_remaining_jobs()
         if len(remaining_jobs) == 0:
             print('\nAll jobs already completed')
             return
 
         start_time = time.time()
-        print('\n\nRunning remaining jobs...\n')
-        print('start time: ', tooltime.timestamp_to_iso_pretty(start_time))
+        print('\nRunning remaining jobs...\n')
+        toolstr.print_bullet(
+            key='start time',
+            value=tooltime.timestamp_to_iso_pretty(start_time),
+            bullet_str='',
+            styles=self.styles,
+        )
 
         # execute jobs
         if executor == 'serial':
             self.serial_execute(jobs=remaining_jobs)
         elif executor == 'parallel':
             self.parallel_execute(jobs=remaining_jobs, n_processes=n_processes)
         else:
@@ -285,62 +295,130 @@
     #
     # # summary
     #
 
     def print_status(self) -> None:
         import toolstr
 
-        toolstr.print_text_box(str(type(self).__name__) + ' Job Summary')
-        print('- n_jobs:', self.get_n_jobs())
-        print('- n_remaining:', len(self.get_remaining_jobs()))
+        if self.styles is not None:
+            title_style = self.styles.get('metavar')
+        else:
+            title_style = None
 
-    def print_summary(self) -> None:
-        import toolstr
+        if self.name is None:
+            name = str(type(self).__name__)
+        else:
+            name = self.name
+        if self.styles is not None:
+            style = self.styles.get('content')
+        else:
+            style = None
+        toolstr.print_text_box(
+            toolstr.add_style(name + ' Job Summary', style=title_style),
+            style=style,
+        )
+        toolstr.print_bullet(
+            key='n_jobs', value=self.get_n_jobs(), styles=self.styles
+        )
+        toolstr.print_bullet(
+            key='n_remaining',
+            value=len(self.get_remaining_jobs()),
+            styles=self.styles,
+        )
+
+        self.print_additional_status()
 
-        toolstr.print_header('Parameters')
-        for parameter in self.parameters:
-            toolstr.print_bullet(key=parameter, value=getattr(self, parameter))
+        if self.verbose:
+            import types
+
+            print()
+            print()
+            toolstr.print_header(
+                toolstr.add_style('Parameters', title_style), style=style
+            )
+            for parameter in vars(self).keys():
+                value = getattr(self, parameter)
+                if (
+                    not parameter.startswith('_')
+                    and not isinstance(value, types.MethodType)
+                    and parameter not in ['styles', 'tracker']
+                ):
+                    toolstr.print_bullet(
+                        key=parameter,
+                        value=value,
+                        styles=self.styles,
+                    )
+            print()
+
+    def print_additional_status(self) -> None:
+        pass
 
     def print_conclusion(
         self,
         start_time: int | float,
         end_time: int | float,
         jobs: typing.Sequence[int],
-        **kwargs: typing.Any,
     ) -> None:
         import toolstr
         import tooltime
 
-        print('end time: ', tooltime.timestamp_to_iso_pretty(end_time))
+        toolstr.print_bullet(
+            key='end time',
+            value='  ' + tooltime.timestamp_to_iso_pretty(end_time),
+            bullet_str='',
+            styles=self.styles,
+        )
 
         done_jobs = len([self.tracker.is_job_complete(i) for i in jobs])
+        print()
         print(done_jobs, 'jobs completed')
 
         duration = end_time - start_time
         seconds_per_job = duration / done_jobs
         jobs_per_second = done_jobs / duration
         print()
-        print('- duration:', toolstr.format(duration, decimals=3), 'seconds')
-        print(
-            '- seconds per job:',
-            toolstr.format(seconds_per_job, decimals=3),
-        )
-        print(
-            '- jobs per minute:',
-            toolstr.format(jobs_per_second * 86400 / 24 / 60, decimals=2),
-        )
-        print(
-            '- jobs per hour:',
-            toolstr.format(jobs_per_second * 86400 / 24, decimals=2),
-        )
-        print(
-            '- jobs per day:',
-            toolstr.format(jobs_per_second * 86400, decimals=2),
+        toolstr.print_bullet(
+            key='duration',
+            value=toolstr.format(duration, decimals=3) + ' seconds',
+            styles=self.styles,
+        )
+        toolstr.print_bullet(
+            key='seconds per job',
+            value=toolstr.format(seconds_per_job, decimals=3),
+            styles=self.styles,
+        )
+        toolstr.print_bullet(
+            key='jobs per minute',
+            value=toolstr.format(jobs_per_second * 86400 / 24 / 60, decimals=2),
+            styles=self.styles,
+        )
+        toolstr.print_bullet(
+            key='jobs per hour',
+            value=toolstr.format(jobs_per_second * 86400 / 24, decimals=2),
+            styles=self.styles,
+        )
+        toolstr.print_bullet(
+            key='jobs per day',
+            value=toolstr.format(jobs_per_second * 86400, decimals=2),
+            styles=self.styles,
+        )
+        self.print_additional_conclusion(
+            start_time=start_time,
+            end_time=end_time,
+            jobs=jobs,
         )
 
+    def print_additional_conclusion(
+        self,
+        start_time: int | float,
+        end_time: int | float,
+        jobs: typing.Sequence[int],
+    ) -> None:
+        pass
+
     def summarize_jobs_per_second(self, sample_time: int = 60) -> pl.DataFrame:
         import polars as pl
 
         names = [self.get_job_name(i) for i in range(self.get_n_jobs())]
         times = [self.get_job_end_time(i) for i in range(self.get_n_jobs())]
         df = pl.from_dict({'job': names, 'times': times})
         df = df.with_columns(
```

### Comparing `tooljob-0.1.2/tooljob/trackers/file_tracker.py` & `tooljob-0.1.3/tooljob/trackers/file_tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.2/tooljob/trackers/sql_tracker.py` & `tooljob-0.1.3/tooljob/trackers/sql_tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.2/tooljob/trackers/tracker.py` & `tooljob-0.1.3/tooljob/trackers/tracker.py`

 * *Files identical despite different names*

### Comparing `tooljob-0.1.2/tooljob/trackers/tracker_utils.py` & `tooljob-0.1.3/tooljob/trackers/tracker_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import typing
 
-from . import tracker
-
 if typing.TYPE_CHECKING:
 
     import toolsql
 
     from .. import batch_class
+    from . import tracker
 
 
 def create_tracker(
     tracker: str | None = None,
     output_dir: str | None = None,
     output_filetype: str | None = None,
     db_config: toolsql.DBConfig | None = None,
```

