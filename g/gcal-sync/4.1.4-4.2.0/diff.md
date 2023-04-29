# Comparing `tmp/gcal-sync-4.1.4.tar.gz` & `tmp/gcal-sync-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcal-sync-4.1.4.tar", last modified: Sat Apr  8 00:01:48 2023, max compression
+gzip compressed data, was "gcal-sync-4.2.0.tar", last modified: Sat Apr 29 21:56:05 2023, max compression
```

## Comparing `gcal-sync-4.1.4.tar` & `gcal-sync-4.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:01:48.874446 gcal-sync-4.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-08 00:01:48.874446 gcal-sync-4.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:01:48.874446 gcal-sync-4.1.4/gcal_sync/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23666 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/model.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/gcal_sync/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:01:48.874446 gcal-sync-4.1.4/gcal_sync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-08 00:01:48.000000 gcal-sync-4.1.4/gcal_sync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-08 00:01:48.000000 gcal-sync-4.1.4/gcal_sync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 00:01:48.000000 gcal-sync-4.1.4/gcal_sync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-08 00:01:48.000000 gcal-sync-4.1.4/gcal_sync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 00:01:48.000000 gcal-sync-4.1.4/gcal_sync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-08 00:01:48.874446 gcal-sync-4.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 00:01:48.874446 gcal-sync-4.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    26084 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25331 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    29841 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-04-08 00:01:35.000000 gcal-sync-4.1.4/tests/test_timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/gcal_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23258 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24793 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/gcal_sync/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/gcal_sync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-29 21:56:05.000000 gcal-sync-4.2.0/gcal_sync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 21:56:05.092392 gcal-sync-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27264 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26414 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29841 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34976 2023-04-29 21:55:52.000000 gcal-sync-4.2.0/tests/test_timeline.py
```

### Comparing `gcal-sync-4.1.4/LICENSE` & `gcal-sync-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/PKG-INFO` & `gcal-sync-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcal-sync
-Version: 4.1.4
+Version: 4.2.0
 Summary: A python library for syncing Google Calendar to local storage
 Home-page: https://github.com/allenporter/gcal_sync
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `gcal-sync-4.1.4/README.md` & `gcal-sync-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync/api.py` & `gcal-sync-4.2.0/gcal_sync/api.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync/auth.py` & `gcal-sync-4.2.0/gcal_sync/auth.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync/exceptions.py` & `gcal-sync-4.2.0/gcal_sync/exceptions.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync/model.py` & `gcal-sync-4.2.0/gcal_sync/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,24 +27,28 @@
     "Event",
     "DateOrDatetime",
     "EventStatusEnum",
     "EventTypeEnum",
     "VisibilityEnum",
     "ResponseStatus",
     "Attendee",
+    "Reminders",
+    "ReminderOverride",
+    "ReminderMethod",
     "AccessRole",
     "CalendarBasic",
 ]
 
 _LOGGER = logging.getLogger(__name__)
 
 DATE_STR_FORMAT = "%Y-%m-%d"
 EVENT_FIELDS = (
     "id,iCalUID,summary,start,end,description,location,transparency,status,eventType,"
-    "visibility,attendees,attendeesOmitted,recurrence,recurringEventId,originalStartTime"
+    "visibility,attendees,attendeesOmitted,recurrence,recurringEventId,originalStartTime,"
+    "reminders"
 )
 MIDNIGHT = datetime.time()
 ID_DELIM = "_"
 
 
 class AccessRole(str, Enum):
     """The effective access role of the caller."""
@@ -422,14 +426,48 @@
         """Configuration for IcsCalendarStream pydantic model."""
 
         json_encoders = DATA_TYPE.encode_property_json
         validate_assignment = True
         allow_population_by_field_name = True
 
 
+class ReminderMethod(str, Enum):
+    """The method to use to send a reminder."""
+
+    EMAIL = "email"
+    """Reminders are sent via email."""
+
+    POPUP = "popup"
+    """Reminders are sent via a UI popup."""
+
+
+class ReminderOverride(BaseModel):
+    """Reminder settings to use instead of calendar default."""
+
+    method: ReminderMethod
+    """The method used by this reminder."""
+
+    minutes: int
+    """Number of minutes before the start of the event to trigger."""
+
+
+class Reminders(BaseModel):
+    """Information about the event's reminders for the authenticated user."""
+
+    use_default: bool = Field(alias="useDefault", default=False)
+
+    overrides: list[ReminderOverride] = Field(default_factory=list)
+    """Reminders to use instead of the default reminders.
+
+    If the event doesn't use the default reminders, this lists the reminders
+    specific to the event, or, if not set, indicates that no reminders are
+    set for this event. The maximum number of override reminders is 5.
+    """
+
+
 class Event(BaseModel):
     """A single event on a calendar."""
 
     id: Optional[str] = None
     """Opaque identifier of the event."""
 
     ical_uuid: Optional[str] = Field(alias="iCalUID", default=None)
@@ -493,14 +531,16 @@
     """The id of the primary even to which this recurring event belongs."""
 
     original_start_time: Optional[DateOrDatetime] = Field(
         alias="originalStartTime", default=None
     )
     """A unique identifier for when this event would start in the original recurring event."""
 
+    reminders: Optional[Reminders] = None
+
     @property
     def computed_duration(self) -> datetime.timedelta:
         """Return the event duration."""
         return self.end.value - self.start.value
 
     @property
     def rrule(self) -> Iterable[Union[datetime.date, datetime.datetime]]:
```

### Comparing `gcal-sync-4.1.4/gcal_sync/store.py` & `gcal-sync-4.2.0/gcal_sync/store.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync/sync.py` & `gcal-sync-4.2.0/gcal_sync/sync.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync/timeline.py` & `gcal-sync-4.2.0/gcal_sync/timeline.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/gcal_sync.egg-info/PKG-INFO` & `gcal-sync-4.2.0/gcal_sync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcal-sync
-Version: 4.1.4
+Version: 4.2.0
 Summary: A python library for syncing Google Calendar to local storage
 Home-page: https://github.com/allenporter/gcal_sync
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `gcal-sync-4.1.4/gcal_sync.egg-info/SOURCES.txt` & `gcal-sync-4.2.0/gcal_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/setup.cfg` & `gcal-sync-4.2.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = gcal-sync
-version = 4.1.4
+version = 4.2.0
 description = A python library for syncing Google Calendar to local storage
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/gcal_sync
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `gcal-sync-4.1.4/tests/test_api.py` & `gcal-sync-4.2.0/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 from gcal_sync.model import (
     EVENT_FIELDS,
     AccessRole,
     Calendar,
     CalendarBasic,
     DateOrDatetime,
     Event,
+    ReminderMethod,
+    ReminderOverride,
+    Reminders,
 )
 from gcal_sync.sync import CalendarEventSyncManager
 
 from .conftest import ApiRequest, ApiResult
 
 EVENT_LIST_PARAMS = (
     "maxResults=1000&singleEvents=true&orderBy=startTime"
@@ -831,7 +834,44 @@
 
     sync = await event_sync_manager_cb()
     with pytest.raises(ValueError, match="Event does not exist"):
         await sync.store_service.async_delete_event(
             ical_uuid="some-event-id@google.com",
             event_id="some-event-id",
         )
+
+
+async def test_create_event_with_reminder(
+    calendar_service_cb: Callable[[], Awaitable[GoogleCalendarService]],
+    json_request: ApiRequest,
+) -> None:
+    """Test create event API when setting a reminder."""
+
+    start_date = datetime.date(2022, 4, 15)
+    end_date = start_date + datetime.timedelta(days=2)
+
+    event = Event(
+        summary="Summary",
+        description="Description",
+        start=DateOrDatetime(date=start_date),
+        end=DateOrDatetime(date=end_date),
+        reminders=Reminders(
+            overrides=[
+                ReminderOverride(
+                    method=ReminderMethod.POPUP,
+                    minutes=7,
+                )
+            ],
+        ),
+    )
+
+    calendar_service = await calendar_service_cb()
+    await calendar_service.async_create_event("calendar-id", event)
+    assert json_request() == [
+        {
+            "summary": "Summary",
+            "description": "Description",
+            "start": {"date": "2022-04-15"},
+            "end": {"date": "2022-04-17"},
+            "reminders": {"overrides": [{"method": "popup", "minutes": 7}]},
+        }
+    ]
```

### Comparing `gcal-sync-4.1.4/tests/test_auth.py` & `gcal-sync-4.2.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/tests/test_model.py` & `gcal-sync-4.2.0/tests/test_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     AccessRole,
     Attendee,
     Calendar,
     DateOrDatetime,
     Event,
     EventStatusEnum,
     EventTypeEnum,
+    ReminderMethod,
+    ReminderOverride,
     ResponseStatus,
     SyntheticEventId,
     VisibilityEnum,
 )
 
 SUMMARY = "test summary"
 LOS_ANGELES = zoneinfo.ZoneInfo("America/Los_Angeles")
@@ -804,7 +806,49 @@
     assert event.end.date_time == datetime.datetime(
         2022, 4, 12, 17, 0, 0, tzinfo=tzinfo
     )
     assert event.end.timezone is None
     assert event.end.value == datetime.datetime(2022, 4, 12, 17, 0, 0, tzinfo=tzinfo)
 
     assert event.timespan.duration == datetime.timedelta(minutes=30)
+
+
+def test_reminders() -> None:
+    """Test event reminders."""
+
+    event = Event.parse_obj(
+        {
+            "id": "some-event-id",
+            "summary": "Event summary",
+            "start": {
+                "date": "2022-04-12",
+            },
+            "end": {
+                "date": "2022-04-13",
+            },
+            "reminders": {
+                "useDefault": True,
+                "overrides": [
+                    {
+                        "method": "email",
+                        "minutes": 5,
+                    },
+                    {
+                        "method": "popup",
+                        "minutes": 3,
+                    },
+                ],
+            },
+        }
+    )
+    assert event.reminders
+    assert event.reminders.use_default
+    assert event.reminders.overrides == [
+        ReminderOverride(
+            method=ReminderMethod.EMAIL,
+            minutes=5,
+        ),
+        ReminderOverride(
+            method=ReminderMethod.POPUP,
+            minutes=3,
+        ),
+    ]
```

### Comparing `gcal-sync-4.1.4/tests/test_store.py` & `gcal-sync-4.2.0/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/tests/test_sync.py` & `gcal-sync-4.2.0/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `gcal-sync-4.1.4/tests/test_timeline.py` & `gcal-sync-4.2.0/tests/test_timeline.py`

 * *Files identical despite different names*

