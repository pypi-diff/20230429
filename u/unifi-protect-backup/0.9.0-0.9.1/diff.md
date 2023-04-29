# Comparing `tmp/unifi_protect_backup-0.9.0.tar.gz` & `tmp/unifi_protect_backup-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_protect_backup-0.9.0.tar", max compression
+gzip compressed data, was "unifi_protect_backup-0.9.1.tar", max compression
```

## Comparing `unifi_protect_backup-0.9.0.tar` & `unifi_protect_backup-0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-03-24 15:36:51.912363 unifi_protect_backup-0.9.0/LICENSE
--rw-r--r--   0        0        0    15448 2023-03-24 15:36:51.912363 unifi_protect_backup-0.9.0/README.md
--rw-r--r--   0        0        0     2110 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/tests/test_unifi_protect_backup.py
--rw-r--r--   0        0        0      359 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/__init__.py
--rw-r--r--   0        0        0     6076 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/cli.py
--rw-r--r--   0        0        0     8967 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/downloader.py
--rw-r--r--   0        0        0     5277 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/event_listener.py
--rw-r--r--   0        0        0     6505 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/missing_event_checker.py
--rw-r--r--   0        0        0      540 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/notifications.py
--rw-r--r--   0        0        0     3427 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/purge.py
--rw-r--r--   0        0        0    12041 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/unifi_protect_backup_core.py
--rw-r--r--   0        0        0     6365 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/uploader.py
--rw-r--r--   0        0        0    16583 2023-03-24 15:36:51.916363 unifi_protect_backup-0.9.0/unifi_protect_backup/utils.py
--rw-r--r--   0        0        0    16582 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/LICENSE
+-rw-r--r--   0        0        0    17222 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/README.md
+-rw-r--r--   0        0        0     2110 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/tests/test_unifi_protect_backup.py
+-rw-r--r--   0        0        0      359 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/unifi_protect_backup/__init__.py
+-rw-r--r--   0        0        0     6416 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/unifi_protect_backup/cli.py
+-rw-r--r--   0        0        0     8972 2023-04-29 08:52:44.952642 unifi_protect_backup-0.9.1/unifi_protect_backup/downloader.py
+-rw-r--r--   0        0        0     5277 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/event_listener.py
+-rw-r--r--   0        0        0     6505 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/missing_event_checker.py
+-rw-r--r--   0        0        0      540 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/notifications.py
+-rw-r--r--   0        0        0     3682 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/purge.py
+-rw-r--r--   0        0        0    12499 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/unifi_protect_backup_core.py
+-rw-r--r--   0        0        0     6365 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/uploader.py
+-rw-r--r--   0        0        0    16583 2023-04-29 08:52:44.956642 unifi_protect_backup-0.9.1/unifi_protect_backup/utils.py
+-rw-r--r--   0        0        0    18356 1970-01-01 00:00:00.000000 unifi_protect_backup-0.9.1/PKG-INFO
```

### Comparing `unifi_protect_backup-0.9.0/LICENSE` & `unifi_protect_backup-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/README.md` & `unifi_protect_backup-0.9.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 #### Backing up to cloud storage:
 In order to backup to cloud storage you need to provide a `rclone.conf` file.
 
 If you do not already have a `rclone.conf` file you can create one as follows:
 ```
 $ docker run -it --rm -v $PWD:/root/.config/rclone --entrypoint rclone ghcr.io/ep1cman/unifi-protect-backup config
 ```
-Follow the interactive configuration proceed, this will create a `rclone.conf`
+Follow the interactive configuration process, this will create a `rclone.conf`
 file in your current directory.
 
 Finally, start the container:
 ```
 docker run \
   -e UFP_USERNAME='USERNAME' \
   -e UFP_PASSWORD='PASSWORD' \
@@ -123,14 +123,18 @@
   --retention TEXT                How long should event clips be backed up for. Format as per the
                                   `--max-age` argument of `rclone`
                                   (https://rclone.org/filtering/#max-age-don-t-transfer-any-file-
                                   older-than-this)  [default: 7d]
   --rclone-args TEXT              Optional extra arguments to pass to `rclone rcat` directly.
                                   Common usage for this would be to set a bandwidth limit, for
                                   example.
+  --rclone-purge-args TEXT        Optional extra arguments to pass to `rclone delete` directly.
+                                  Common usage for this would be to execute a permanent delete
+                                  instead of using the recycle bin on a destination.
+                                  Google Drive example: `--drive-use-trash=false`
   --detection-types TEXT          A comma separated list of which types of detections to backup.
                                   Valid options are: `motion`, `person`, `vehicle`, `ring`
                                   [default: motion,person,vehicle,ring]
   --ignore-camera TEXT            IDs of cameras for which events should not be backed up. Use
                                   multiple times to ignore multiple IDs. If being set as an
                                   environment variable the IDs should be separated by whitespace.
   --file-structure-format TEXT    A Python format string used to generate the file structure/name
@@ -194,14 +198,15 @@
 - `UFP_PASSWORD`
 - `UFP_ADDRESS`
 - `UFP_PORT`
 - `UFP_SSL_VERIFY`
 - `RCLONE_RETENTION`
 - `RCLONE_DESTINATION`
 - `RCLONE_ARGS`
+- `RCLONE_PURGE_ARGS`
 - `IGNORE_CAMERAS`
 - `DETECTION_TYPES`
 - `FILE_STRUCTURE_FORMAT`
 - `SQLITE_PATH`
 - `DOWNLOAD_BUFFER_SIZE`
 - `COLOR_LOGGING`
 - `PURGE_INTERVAL`
@@ -255,14 +260,53 @@
 ```
 
 To make this persist reboots add the following to `/etc/fstab`:
 ```
 tmpfs /mnt/tmpfs tmpfs nosuid,nodev,noatime 0 0
 ```
 
+# Running Backup Tool as a Service (LINUX ONLY)
+You can create a service that will run the docker or local version of this backup tool. The service can be configured to launch on boot. This is likely the preferred way you want to execute the tool once you have it completely configured and tested so it is continiously running.
+
+First create a service configuration file. You can replace `protectbackup` in the filename below with the name you wish to use for your service, if you change it remember to change the other locations in the following scripts as well.
+
+```
+sudo nano /lib/systemd/system/protectbackup.service
+```
+
+Next edit the content and fill in the 4 placeholders indicated by {}, replace these placeholders (including the leading `{` and trailing `}` characters) with the values you are using.
+
+```
+[Unit]
+Description=Unifi Protect Backup
+
+[Service]
+User={your machine username}
+Group={your machine user group, could be the same as the username}
+Restart=on-abort
+WorkingDirectory=/home/{your machine username}
+ExecStart={put your complete docker or local command here}
+
+[Install]
+WantedBy=multi-user.target
+```
+
+Now enable the service and then start the service.
+
+```
+sudo systemctl enable protectbackup.service
+sudo systemctl start protectbackup.service
+```
+
+To check the status of the service use this command.
+
+```
+sudo systemctl status protectbackup.service --no-pager
+```
+
 # Debugging
 
 If you need to debug your rclone setup, you can invoke rclone directly like so:
 
 ```
 docker run \
     --rm \
```

### Comparing `unifi_protect_backup-0.9.0/pyproject.toml` & `unifi_protect_backup-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "unifi_protect_backup"
-version = "0.9.0"
+version = "0.9.1"
 homepage = "https://github.com/ep1cman/unifi-protect-backup"
 description = "Python tool to backup unifi event clips in realtime."
 authors = ["sebastian.goscik <sebastian@goscik.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
```

### Comparing `unifi_protect_backup-0.9.0/tests/test_unifi_protect_backup.py` & `unifi_protect_backup-0.9.1/tests/test_unifi_protect_backup.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/cli.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,22 @@
     '--rclone-args',
     default='',
     envvar='RCLONE_ARGS',
     help="Optional extra arguments to pass to `rclone rcat` directly. Common usage for this would "
     "be to set a bandwidth limit, for example.",
 )
 @click.option(
+    '--rclone-purge-args',
+    default='',
+    envvar='RCLONE_PURGE_ARGS',
+    help="Optional extra arguments to pass to `rclone delete` directly. Common usage for this would "
+    "be to execute a permanent delete instead of using the recycle bin on a destination. "
+    "Google Drive example: `--drive-use-trash=false`",
+)
+@click.option(
     '--detection-types',
     envvar='DETECTION_TYPES',
     default=','.join(DETECTION_TYPES),
     show_default=True,
     help="A comma separated list of which types of detections to backup. "
     f"Valid options are: {', '.join([f'`{t}`' for t in DETECTION_TYPES])}",
     callback=_parse_detection_types,
```

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/downloader.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,41 +115,42 @@
                 # but often longer)
                 time_since_event_ended = datetime.utcnow().replace(tzinfo=timezone.utc) - event.end
                 sleep_time = (timedelta(seconds=5 * 1.5) - time_since_event_ended).total_seconds()
                 if sleep_time > 0:
                     self.logger.debug(f"  Sleeping ({sleep_time}s) to ensure clip is ready to download...")
                     await asyncio.sleep(sleep_time)
 
-                video = await self._download(event)
-                if video is None:
+                try:
+                    video = await self._download(event)
+                    assert video is not None
+                except Exception as e:
                     # Increment failure count
                     if event.id not in self._failures:
                         self._failures[event.id] = 1
                     else:
                         self._failures[event.id] += 1
-                    self.logger.warning(f"Event failed download attempt {self._failures[event.id]}")
+                    self.logger.warning(f"Event failed download attempt {self._failures[event.id]}", exc_info=e)
 
                     if self._failures[event.id] >= 10:
                         self.logger.error(
                             "Event has failed to download 10 times in a row. Permanently ignoring this event"
                         )
 
                         # ignore event
-                        self.logger.extra_debug(f"Ignoring event '{event.id}'")
                         await self._db.execute(
                             "INSERT INTO events VALUES "
                             f"('{event.id}', '{event.type}', '{event.camera_id}',"
                             f"'{event.start.timestamp()}', '{event.end.timestamp()}')"
                         )
                         await self._db.commit()
 
                     continue
 
                 # Remove successfully downloaded event from failures list
-                elif event.id in self._failures:
+                if event.id in self._failures:
                     del self._failures[event.id]
 
                 # Get the actual length of the downloaded video using ffprobe
                 if self._has_ffprobe:
                     await self._check_video_length(video, duration)
 
                 await self.upload_queue.put((event, video))
```

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/event_listener.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/event_listener.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/missing_event_checker.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/missing_event_checker.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/notifications.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/notifications.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/purge.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/purge.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from dateutil.relativedelta import relativedelta
 
 from unifi_protect_backup.utils import run_command, wait_until
 
 logger = logging.getLogger(__name__)
 
 
-async def delete_file(file_path):
+async def delete_file(file_path, rclone_purge_args):
     """Deletes `file_path` via rclone."""
-    returncode, stdout, stderr = await run_command(f'rclone delete -vv "{file_path}"')
+    returncode, stdout, stderr = await run_command(f'rclone delete -vv "{file_path}" {rclone_purge_args}')
     if returncode != 0:
         logger.error(f" Failed to delete file: '{file_path}'")
 
 
 async def tidy_empty_dirs(base_dir_path):
     """Deletes any empty directories in `base_dir_path` via rclone."""
     returncode, stdout, stderr = await run_command(f'rclone rmdirs -vv --ignore-errors --leave-root "{base_dir_path}"')
@@ -31,27 +31,30 @@
 
     def __init__(
         self,
         db: aiosqlite.Connection,
         retention: relativedelta,
         rclone_destination: str,
         interval: relativedelta = relativedelta(days=1),
+        rclone_purge_args: str = "",
     ):
         """Init.
 
         Args:
             db (aiosqlite.Connection): Async SQlite database connection to purge clips from
             retention (relativedelta): How long clips should be kept
             rclone_destination (str): What rclone destination the clips are stored in
             interval (relativedelta): How often to purge old clips
+            rclone_purge_args (str): Optional extra arguments to pass to `rclone delete` directly.
         """
         self._db: aiosqlite.Connection = db
         self.retention: relativedelta = retention
         self.rclone_destination: str = rclone_destination
         self.interval: relativedelta = interval
+        self.rclone_purge_args: str = rclone_purge_args
 
     async def start(self):
         """Main loop - runs forever."""
         while True:
             try:
                 deleted_a_file = False
 
@@ -64,15 +67,15 @@
 
                         logger.info(f"Purging event: {event_id}.")
 
                         # For every backup for this event
                         async with self._db.execute(f"SELECT * FROM backups WHERE id = '{event_id}'") as backup_cursor:
                             async for _, remote, file_path in backup_cursor:
                                 logger.debug(f" Deleted: {remote}:{file_path}")
-                                await delete_file(f"{remote}:{file_path}")
+                                await delete_file(f"{remote}:{file_path}", self.rclone_purge_args)
                                 deleted_a_file = True
 
                         # delete event from database
                         # entries in the `backups` table are automatically deleted by sqlite triggers
                         await self._db.execute(f"DELETE FROM events WHERE id = '{event_id}'")
                         await self._db.commit()
```

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/unifi_protect_backup_core.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/unifi_protect_backup_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         address: str,
         username: str,
         password: str,
         verify_ssl: bool,
         rclone_destination: str,
         retention: str,
         rclone_args: str,
+        rclone_purge_args: str,
         detection_types: List[str],
         ignore_cameras: List[str],
         file_structure_format: str,
         verbose: int,
         download_buffer_size: int,
         purge_interval: str,
         apprise_notifiers: str,
@@ -83,57 +84,64 @@
                                     {rclone remote}:{path on remote}. E.g.
                                     `gdrive:/backups/unifi_protect`
             retention (str): How long should event clips be backed up for. Format as per the
                             `--max-age` argument of `rclone`
                             (https://rclone.org/filtering/#max-age-don-t-transfer-any-file-older-than-this)
             rclone_args (str): A bandwidth limit which is passed to the `--bwlimit` argument of
                                    `rclone` (https://rclone.org/docs/#bwlimit-bandwidth-spec)
+            rclone_purge_args (str): Optional extra arguments to pass to `rclone delete` directly.
             detection_types (List[str]): List of which detection types to backup.
             ignore_cameras (List[str]): List of camera IDs for which to not backup events.
             file_structure_format (str): A Python format string for output file path.
             verbose (int): How verbose to setup logging, see :func:`setup_logging` for details.
             download_buffer_size (int): How many bytes big the download buffer should be
             purge_interval (str): How often to check for files to delete
             apprise_notifiers (str): Apprise URIs for notifications
             skip_missing (bool): If initial missing events should be ignored
             sqlite_path (str): Path where to find/create sqlite database
             color_logging (bool): Whether to add color to logging output or not
         """
-        for notifier in apprise_notifiers:
-            notifications.add_notification_service(notifier)
-
         self.color_logging = color_logging
         setup_logging(verbose, self.color_logging)
 
+        for notifier in apprise_notifiers:
+            try:
+                notifications.add_notification_service(notifier)
+            except Exception as e:
+                logger.error(f"Error occurred when setting up logger `{notifier}`", exc_info=e)
+                raise
+
         logger.debug("Config:")
         logger.debug(f"  {address=}")
         logger.debug(f"  {port=}")
         logger.debug(f"  {username=}")
         if verbose < 5:
             logger.debug("  password=REDACTED")
         else:
             logger.debug(f"  {password=}")
 
         logger.debug(f"  {verify_ssl=}")
         logger.debug(f"  {rclone_destination=}")
         logger.debug(f"  {retention=}")
         logger.debug(f"  {rclone_args=}")
+        logger.debug(f"  {rclone_purge_args=}")
         logger.debug(f"  {ignore_cameras=}")
         logger.debug(f"  {verbose=}")
         logger.debug(f"  {detection_types=}")
         logger.debug(f"  {file_structure_format=}")
         logger.debug(f"  {sqlite_path=}")
         logger.debug(f"  download_buffer_size={human_readable_size(download_buffer_size)}")
         logger.debug(f"  {purge_interval=}")
         logger.debug(f"  {apprise_notifiers=}")
         logger.debug(f"  {skip_missing=}")
 
         self.rclone_destination = rclone_destination
         self.retention = parse_rclone_retention(retention)
         self.rclone_args = rclone_args
+        self.rclone_purge_args = rclone_purge_args
         self.file_structure_format = file_structure_format
 
         self.address = address
         self.port = port
         self.username = username
         self.password = password
         self.verify_ssl = verify_ssl
@@ -230,15 +238,17 @@
             #   This will connect to the unifi protect websocket and listen for events. When one is detected it will
             #   be added to the queue of events to download
             event_listener = EventListener(download_queue, self._protect, self.detection_types, self.ignore_cameras)
             tasks.append(event_listener.start())
 
             # Create purge task
             #   This will, every midnight, purge old backups from the rclone remotes and database
-            purge = Purge(self._db, self.retention, self.rclone_destination, self._purge_interval)
+            purge = Purge(
+                self._db, self.retention, self.rclone_destination, self._purge_interval, self.rclone_purge_args
+            )
             tasks.append(purge.start())
 
             # Create missing event task
             #   This will check all the events within the retention period, if any have been missed and not backed up
             #   they will be added to the event queue
             missing = MissingEventChecker(
                 self._protect,
```

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/uploader.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/uploader.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/unifi_protect_backup/utils.py` & `unifi_protect_backup-0.9.1/unifi_protect_backup/utils.py`

 * *Files identical despite different names*

### Comparing `unifi_protect_backup-0.9.0/PKG-INFO` & `unifi_protect_backup-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi-protect-backup
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python tool to backup unifi event clips in realtime.
 Home-page: https://github.com/ep1cman/unifi-protect-backup
 License: MIT
 Author: sebastian.goscik
 Author-email: sebastian@goscik.com
 Requires-Python: >=3.9.0,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -103,15 +103,15 @@
 #### Backing up to cloud storage:
 In order to backup to cloud storage you need to provide a `rclone.conf` file.
 
 If you do not already have a `rclone.conf` file you can create one as follows:
 ```
 $ docker run -it --rm -v $PWD:/root/.config/rclone --entrypoint rclone ghcr.io/ep1cman/unifi-protect-backup config
 ```
-Follow the interactive configuration proceed, this will create a `rclone.conf`
+Follow the interactive configuration process, this will create a `rclone.conf`
 file in your current directory.
 
 Finally, start the container:
 ```
 docker run \
   -e UFP_USERNAME='USERNAME' \
   -e UFP_PASSWORD='PASSWORD' \
@@ -151,14 +151,18 @@
   --retention TEXT                How long should event clips be backed up for. Format as per the
                                   `--max-age` argument of `rclone`
                                   (https://rclone.org/filtering/#max-age-don-t-transfer-any-file-
                                   older-than-this)  [default: 7d]
   --rclone-args TEXT              Optional extra arguments to pass to `rclone rcat` directly.
                                   Common usage for this would be to set a bandwidth limit, for
                                   example.
+  --rclone-purge-args TEXT        Optional extra arguments to pass to `rclone delete` directly.
+                                  Common usage for this would be to execute a permanent delete
+                                  instead of using the recycle bin on a destination.
+                                  Google Drive example: `--drive-use-trash=false`
   --detection-types TEXT          A comma separated list of which types of detections to backup.
                                   Valid options are: `motion`, `person`, `vehicle`, `ring`
                                   [default: motion,person,vehicle,ring]
   --ignore-camera TEXT            IDs of cameras for which events should not be backed up. Use
                                   multiple times to ignore multiple IDs. If being set as an
                                   environment variable the IDs should be separated by whitespace.
   --file-structure-format TEXT    A Python format string used to generate the file structure/name
@@ -222,14 +226,15 @@
 - `UFP_PASSWORD`
 - `UFP_ADDRESS`
 - `UFP_PORT`
 - `UFP_SSL_VERIFY`
 - `RCLONE_RETENTION`
 - `RCLONE_DESTINATION`
 - `RCLONE_ARGS`
+- `RCLONE_PURGE_ARGS`
 - `IGNORE_CAMERAS`
 - `DETECTION_TYPES`
 - `FILE_STRUCTURE_FORMAT`
 - `SQLITE_PATH`
 - `DOWNLOAD_BUFFER_SIZE`
 - `COLOR_LOGGING`
 - `PURGE_INTERVAL`
@@ -283,14 +288,53 @@
 ```
 
 To make this persist reboots add the following to `/etc/fstab`:
 ```
 tmpfs /mnt/tmpfs tmpfs nosuid,nodev,noatime 0 0
 ```
 
+# Running Backup Tool as a Service (LINUX ONLY)
+You can create a service that will run the docker or local version of this backup tool. The service can be configured to launch on boot. This is likely the preferred way you want to execute the tool once you have it completely configured and tested so it is continiously running.
+
+First create a service configuration file. You can replace `protectbackup` in the filename below with the name you wish to use for your service, if you change it remember to change the other locations in the following scripts as well.
+
+```
+sudo nano /lib/systemd/system/protectbackup.service
+```
+
+Next edit the content and fill in the 4 placeholders indicated by {}, replace these placeholders (including the leading `{` and trailing `}` characters) with the values you are using.
+
+```
+[Unit]
+Description=Unifi Protect Backup
+
+[Service]
+User={your machine username}
+Group={your machine user group, could be the same as the username}
+Restart=on-abort
+WorkingDirectory=/home/{your machine username}
+ExecStart={put your complete docker or local command here}
+
+[Install]
+WantedBy=multi-user.target
+```
+
+Now enable the service and then start the service.
+
+```
+sudo systemctl enable protectbackup.service
+sudo systemctl start protectbackup.service
+```
+
+To check the status of the service use this command.
+
+```
+sudo systemctl status protectbackup.service --no-pager
+```
+
 # Debugging
 
 If you need to debug your rclone setup, you can invoke rclone directly like so:
 
 ```
 docker run \
     --rm \
```

