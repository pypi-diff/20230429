# Comparing `tmp/pyadtpulse-1.0.2-py3-none-any.whl.zip` & `tmp/pyadtpulse-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 20545 bytes, number of entries: 11
--rw-r--r--  2.0 unx    31842 b- defN 23-Apr-18 03:32 pyadtpulse/__init__.py
+Zip file size: 21418 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    34446 b- defN 23-Apr-29 06:07 pyadtpulse/__init__.py
 -rw-r--r--  2.0 unx     1609 b- defN 23-Mar-28 16:07 pyadtpulse/const.py
--rw-r--r--  2.0 unx    24044 b- defN 23-Apr-18 03:32 pyadtpulse/site.py
+-rw-r--r--  2.0 unx    24957 b- defN 23-Apr-29 06:07 pyadtpulse/site.py
 -rw-r--r--  2.0 unx     4803 b- defN 23-Mar-28 16:07 pyadtpulse/util.py
--rw-r--r--  2.0 unx     5089 b- defN 23-Mar-28 16:07 pyadtpulse/zones.py
--rw-r--r--  2.0 unx      581 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3646 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.2.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      875 b- defN 23-Apr-18 03:36 pyadtpulse-1.0.2.dist-info/RECORD
-11 files, 72593 bytes uncompressed, 19071 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx     5847 b- defN 23-Apr-29 06:07 pyadtpulse/zones.py
+-rw-r--r--  2.0 unx      581 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     3680 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.3.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      875 b- defN 23-Apr-29 06:12 pyadtpulse-1.0.3.dist-info/RECORD
+11 files, 76902 bytes uncompressed, 19944 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pyadtpulse/util.py
 Comment: 
 
 Filename: pyadtpulse/zones.py
 Comment: 
 
-Filename: pyadtpulse-1.0.2.dist-info/LICENSE.md
+Filename: pyadtpulse-1.0.3.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyadtpulse-1.0.2.dist-info/METADATA
+Filename: pyadtpulse-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pyadtpulse-1.0.2.dist-info/WHEEL
+Filename: pyadtpulse-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyadtpulse-1.0.2.dist-info/top_level.txt
+Filename: pyadtpulse-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyadtpulse-1.0.2.dist-info/zip-safe
+Filename: pyadtpulse-1.0.3.dist-info/zip-safe
 Comment: 
 
-Filename: pyadtpulse-1.0.2.dist-info/RECORD
+Filename: pyadtpulse-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyadtpulse/__init__.py

```diff
@@ -1,20 +1,21 @@
 """Base Python Class for pyadtpulse."""
 
 import logging
 import asyncio
 import re
 import time
 from random import uniform
-from threading import RLock, Thread, Lock
+from threading import Lock, RLock, Thread
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import uvloop
 from aiohttp import (
     ClientConnectionError,
+    ClientConnectorError,
     ClientResponse,
     ClientResponseError,
     ClientSession,
 )
 from bs4 import BeautifulSoup
 
 from pyadtpulse.const import (
@@ -23,14 +24,15 @@
     ADT_DEFAULT_VERSION,
     ADT_DEVICE_URI,
     ADT_GATEWAY_OFFLINE_POLL_INTERVAL,
     ADT_HTTP_REFERER_URIS,
     ADT_LOGIN_URI,
     ADT_LOGOUT_URI,
     ADT_ORB_URI,
+    ADT_SUMMARY_URI,
     ADT_SYNC_CHECK_URI,
     ADT_SYSTEM_URI,
     ADT_TIMEOUT_INTERVAL,
     ADT_TIMEOUT_URI,
     API_PREFIX,
     DEFAULT_API_HOST,
 )
@@ -46,14 +48,16 @@
 
 if TYPE_CHECKING:
     from pyadtpulse.site import ADTPulseSite
 
 LOG = logging.getLogger(__name__)
 
 RECOVERABLE_ERRORS = [429, 500, 502, 503, 504]
+SYNC_CHECK_TASK_NAME = "ADT Pulse Sync Check Task"
+KEEPALIVE_TASK_NAME = "ADT Pulse Keepalive Task"
 
 
 class PyADTPulse:
     """Base object for ADT Pulse service."""
 
     __slots__ = (
         "_session",
@@ -71,14 +75,15 @@
         "_api_host",
         "_poll_interval",
         "_username",
         "_password",
         "_fingerprint",
         "_login_exception",
         "_gateway_online",
+        "_create_task_cb",
     )
     _api_version = ADT_DEFAULT_VERSION
     _class_threadlock = Lock()
 
     def __init__(
         self,
         username: str,
@@ -86,14 +91,15 @@
         fingerprint: str,
         service_host: str = DEFAULT_API_HOST,
         user_agent=ADT_DEFAULT_HTTP_HEADERS["User-Agent"],
         websession: Optional[ClientSession] = None,
         do_login: bool = True,
         poll_interval: float = ADT_DEFAULT_POLL_INTERVAL,
         debug_locks: bool = False,
+        create_task_cb=asyncio.create_task,
     ):
         """Create a PyADTPulse object.
 
         Args:
             username (str): Username.
             password (str): Password.
             fingerprint (str): 2FA fingerprint.
@@ -107,14 +113,18 @@
             do_login (bool, optional): login synchronously when creating object
                             Should be set to False for asynchronous usage
                             and async_login() should be called instead
                             Setting websession will override this
                             and not login
                         Defaults to True
             poll_interval (float, optional): number of seconds between update checks
+            debug_locks: (bool, optional): use debugging locks
+                        Defaults to False
+            create_task_cb (callback, optional): callback to use to create async tasks
+                        Defaults to asyncio.create_task()
         """
         self._gateway_online: bool = False
 
         self._session = websession
         if self._session is not None:
             self._session.headers.update(ADT_DEFAULT_HTTP_HEADERS)
 
@@ -128,32 +138,33 @@
         # FIXME use thread event/condition, regular condition?
         # defer initialization to make sure we have an event loop
         self._authenticated: Optional[asyncio.locks.Event] = None
         self._login_exception: Optional[BaseException] = None
 
         self._updates_exist: Optional[asyncio.locks.Event] = None
 
-        self._last_timeout_reset = time.time()
-
         self._loop: Optional[asyncio.AbstractEventLoop] = None
         self._session_thread: Optional[Thread] = None
         self._attribute_lock: Union[RLock, DebugRLock]
         if not debug_locks:
             self._attribute_lock = RLock()
         else:
             self._attribute_lock = DebugRLock("PyADTPulse._attribute_lock")
+        self._sync_timestamp = self._last_timeout_reset = time.time()
 
-        # FIXME: circular import, should be an ADTPulseSite
+        # fixme circular import, should be an ADTPulseSite
         if TYPE_CHECKING:
             self._sites: List[ADTPulseSite]
         else:
             self._sites: List[Any] = []
 
         self._api_host = service_host
         self._poll_interval = poll_interval
+        # FIXME: I have no idea how to type hint this
+        self._create_task_cb = create_task_cb
 
         # authenticate the user
         if do_login and self._session is None:
             self.login()
 
     def _init_login_info(self, username: str, password: str, fingerprint: str) -> None:
         if username is None or username == "":
@@ -289,15 +300,15 @@
                 return
 
             status_text = "ONLINE"
             if not status:
                 status_text = "OFFLINE"
                 self._poll_interval = ADT_GATEWAY_OFFLINE_POLL_INTERVAL
 
-            LOG.warning(
+            LOG.info(
                 f"ADT Pulse gateway {status_text}, poll interval={self._poll_interval}"
             )
             self._gateway_online = status
 
     async def _async_fetch_version(self) -> None:
         with PyADTPulse._class_threadlock:
             if PyADTPulse._api_version != ADT_DEFAULT_VERSION:
@@ -401,34 +412,38 @@
     # ... or perhaps better, just extract all from /system/settings.jsp
 
     def _close_response(self, response: Optional[ClientResponse]) -> None:
         if response is not None and not response.closed:
             response.close()
 
     async def _keepalive_task(self) -> None:
-        LOG.debug("creating Pulse keepalive task")
+        if self._timeout_task is not None:
+            task_name = self._timeout_task.get_name()
+        else:
+            task_name = f"{KEEPALIVE_TASK_NAME} - possible internal error"
+        LOG.debug(f"creating {task_name}")
         response = None
         with self._attribute_lock:
             if self._authenticated is None:
                 raise RuntimeError(
-                    "Keepalive task is runnng without an authenticated event"
+                    "Keepalive task is running without an authenticated event"
                 )
         while self._authenticated.is_set():
             try:
                 await asyncio.sleep(ADT_TIMEOUT_INTERVAL)
                 LOG.debug("Resetting timeout")
                 response = await self._async_query(ADT_TIMEOUT_URI, "POST")
                 if handle_response(
                     response, logging.INFO, "Failed resetting ADT Pulse cloud timeout"
                 ):
                     self._close_response(response)
                     continue
                 self._close_response(response)
             except asyncio.CancelledError:
-                LOG.debug("ADT Pulse timeout task cancelled")
+                LOG.debug(f"{task_name} cancelled")
                 self._close_response(response)
                 return
 
     def _pulse_session_thread(self) -> None:
         # lock is released in sync_loop()
         self._attribute_lock.acquire()
 
@@ -441,24 +456,31 @@
         self._loop = None
         self._session_thread = None
 
     async def _sync_loop(self) -> None:
         result = await self.async_login()
         self._attribute_lock.release()
         if result:
-            if self._sync_task is not None and self._timeout_task is not None:
+            if self._timeout_task is not None:
+                task_list = (self._timeout_task,)
                 try:
-                    await asyncio.wait((self._sync_task, self._timeout_task))
+                    await asyncio.wait(task_list)
+                except asyncio.CancelledError:
+                    pass
                 except Exception as e:
                     LOG.exception(
                         f"Received exception while waiting for ADT Pulse service {e}"
                     )
             else:
                 # we should never get here
                 raise RuntimeError("Background pyadtpulse tasks not created")
+        if self._authenticated is not None:
+            while self._authenticated.is_set():
+                # busy wait until logout is done
+                await asyncio.sleep(0.5)
 
     def login(self) -> None:
         """Login to ADT Pulse and generate access token.
 
         Raises:
             AuthenticationException if could not login
         """
@@ -528,14 +550,29 @@
                 "fingerprint": self._fingerprint,
                 "sun": "yes",
             },
             force_login=False,
             timeout=30,
         )
 
+        if not handle_response(
+            response,
+            logging.ERROR,
+            "Error encountered communicating with Pulse site on login",
+        ):
+            self._close_response(response)
+            return False
+        if str(response.url) != self.make_url(ADT_SUMMARY_URI):  # type: ignore
+            # more specifically:
+            # redirect to signin.jsp = username/password error
+            # redirect to mfaSignin.jsp = fingerprint error
+            LOG.error("Authentication error encountered logging into ADT Pulse")
+            self._close_response(response)
+            return False
+
         soup = await make_soup(
             response, logging.ERROR, "Could not log into ADT Pulse site"
         )
         if soup is None:
             return False
 
         # FIXME: should probably raise exceptions
@@ -559,41 +596,37 @@
             return False
         self._last_timeout_reset = time.time()
 
         # since we received fresh data on the status of the alarm, go ahead
         # and update the sites with the alarm status.
 
         self._sync_timestamp = time.time()
-        if self._sync_task is None:
-            self._sync_task = asyncio.create_task(
-                self._sync_check_task(), name="PyADTPulse sync check"
-            )
         if self._timeout_task is None:
-            self._timeout_task = asyncio.create_task(
-                self._keepalive_task(), name="PyADTPulse timeout"
+            self._timeout_task = self._create_task_cb(
+                self._keepalive_task(), name=f"{KEEPALIVE_TASK_NAME}"
             )
         if self._updates_exist is None:
             self._updates_exist = asyncio.locks.Event()
         await asyncio.sleep(0)
         return True
 
     async def async_logout(self) -> None:
         """Logout of ADT Pulse async."""
         LOG.info(f"Logging {self._username} out of ADT Pulse")
         if self._timeout_task is not None:
             try:
                 self._timeout_task.cancel()
             except asyncio.CancelledError:
-                LOG.debug("Pulse timeout task successfully cancelled")
+                LOG.debug(f"{KEEPALIVE_TASK_NAME} successfully cancelled")
                 await self._timeout_task
         if self._sync_task is not None:
             try:
                 self._sync_task.cancel()
             except asyncio.CancelledError:
-                LOG.debug("Pulse sync check task successfully cancelled")
+                LOG.debug(f"{SYNC_CHECK_TASK_NAME} successfully cancelled")
                 await self._sync_task
         self._timeout_task = self._sync_task = None
         await self._async_query(ADT_LOGOUT_URI, timeout=10)
         self._last_timeout_reset = time.time()
         if self._authenticated is not None:
             self._authenticated.clear()
 
@@ -606,26 +639,32 @@
 
         coro = self.async_logout()
         asyncio.run_coroutine_threadsafe(coro, self._loop)
         if sync_thread is not None:
             sync_thread.join()
 
     async def _sync_check_task(self) -> None:
-        LOG.debug("creating Pulse sync check task")
+        # this should never be true
+        if self._sync_task is not None:
+            task_name = self._sync_task.get_name()
+        else:
+            task_name = f"{SYNC_CHECK_TASK_NAME} - possible internal error"
+
+        LOG.debug(f"creating {task_name}")
         response = None
         if self._updates_exist is None:
             raise RuntimeError(
                 "Sync check task started without update event initialized"
             )
         while True:
             try:
                 if self.gateway_online:
                     pi = self.poll_interval
                 else:
-                    LOG.warning(
+                    LOG.info(
                         "Pulse gateway detected offline, polling every "
                         f"{ADT_GATEWAY_OFFLINE_POLL_INTERVAL} seconds"
                     )
                     pi = ADT_GATEWAY_OFFLINE_POLL_INTERVAL
 
                 await asyncio.sleep(pi)
                 response = await self._async_query(
@@ -667,40 +706,56 @@
                     continue
 
                 LOG.debug(f"Sync token {text} indicates no remote updates to process")
                 self._close_response(response)
                 self._sync_timestamp = time.time()
 
             except asyncio.CancelledError:
-                LOG.debug("ADT Pulse sync check task cancelled")
+                LOG.debug(f"{task_name} cancelled")
                 self._close_response(response)
                 return
 
     @property
     def updates_exist(self) -> bool:
         """Check if updated data exists.
 
         Returns:
             bool: True if updated data exists
         """
         with self._attribute_lock:
+            if self._sync_task is None:
+                if self._loop is None:
+                    raise RuntimeError(
+                        "ADT pulse sync function updates_exist() "
+                        "called from async session"
+                    )
+                coro = self._sync_check_task()
+                self._sync_task = self._loop.create_task(
+                    coro, name=f"{SYNC_CHECK_TASK_NAME}: Sync session"
+                )
             if self._updates_exist is None:
                 return False
 
             if self._updates_exist.is_set():
                 self._updates_exist.clear()
                 return True
             return False
 
     async def wait_for_update(self) -> None:
         """Wait for update.
 
         Blocks current async task until Pulse system
         signals an update
         """
+        with self._attribute_lock:
+            if self._sync_task is None:
+                coro = self._sync_check_task()
+                self._sync_task = self._create_task_cb(
+                    coro, name=f"{SYNC_CHECK_TASK_NAME}: Async session"
+                )
         if self._updates_exist is None:
             raise RuntimeError("Update event does not exist")
 
         await self._updates_exist.wait()
         self._updates_exist.clear()
 
     @property
@@ -797,23 +852,30 @@
                         response.raise_for_status()
                     await asyncio.sleep(2**retry + uniform(0.0, 1.0))
                     continue
 
                 response.raise_for_status()
                 # success, break loop
                 retry = 4
+            except (
+                asyncio.TimeoutError,
+                ClientConnectionError,
+                ClientConnectorError,
+            ) as ex:
+                LOG.warning(
+                    f"Error {ex} occurred making {method} request to {url}, retrying"
+                )
+                await asyncio.sleep(2**retry + uniform(0.0, 1.0))
+                continue
             except ClientResponseError as err:
                 code = err.code
                 LOG.exception(
                     f"Received HTTP error code {code} in request to ADT Pulse"
                 )
                 return None
-            except ClientConnectionError:
-                LOG.exception("An exception occurred in request to ADT Pulse")
-                return None
 
         # success!
         # FIXME? login uses redirects so final url is wrong
         if uri in ADT_HTTP_REFERER_URIS:
             if uri == ADT_DEVICE_URI:
                 referer = self.make_url(ADT_SYSTEM_URI)
             else:
```

## pyadtpulse/site.py

```diff
@@ -592,14 +592,31 @@
                         "Zone\xa0",
                     )
                 )
                 state = remove_prefix(
                     row.find("canvas", {"class": "p_ic_icon_device"}).get("icon"),
                     "devStat",
                 )
+                temp_status = row.find("td", {"class": "p_listRow"}).find_next(
+                    "td", {"class": "p_listRow"}
+                )
+
+                status = "Unknown"
+                if temp_status is not None:
+                    temp_status = temp_status.get_text()
+                    if temp_status is not None:
+                        temp_status = str(temp_status.replace("\xa0", ""))
+                        if temp_status.startswith("Trouble"):
+                            trouble_code = str(temp_status).split()
+                            if len(trouble_code) > 1:
+                                status = " ".join(trouble_code[1:])
+                            else:
+                                status = "Unknown trouble code"
+                        else:
+                            status = "Online"
 
                 # parse out last activity (required dealing with "Yesterday 1:52 PM")
                 #           last_activity = time.time()
 
                 # id:    [integer]
                 # name:  device name
                 # tags:  sensor,[doorWindow,motion,glass,co,fire]
@@ -613,18 +630,19 @@
 
                 # update device state from ORB info
                 if not self._zones:
                     LOG.warning("No zones exist")
                     return None
                 if state != "Unknown":
                     gateway_online = True
-                self._zones.update_last_activity_timestamp(zone, last_update)
-
-                LOG.debug(f"Set zone {zone} - to {state} with timestamp {last_update}")
-
+                self._zones.update_device_info(zone, state, status, last_update)
+                LOG.debug(
+                    f"Set zone {zone} - to {state}, status {status} "
+                    f"with timestamp {last_update}"
+                )
             self._adt_service._set_gateway_status(gateway_online)
             self._last_updated = datetime.now()
             return self._zones
 
     async def _async_update_zones(self) -> Optional[List[ADTPulseFlattendZone]]:
         """Update zones asynchronously.
```

## pyadtpulse/zones.py

```diff
@@ -138,14 +138,39 @@
             key (int): zone id to change
             dt (datetime): timestamp to set
         """
         temp = self._get_zonedata(key)
         temp.last_activity_timestamp = dt.timestamp()
         self.__setitem__(key, temp)
 
+    def update_device_info(
+        self,
+        key: int,
+        state: str,
+        status: str = "Online",
+        last_activity: datetime = datetime.now(),
+    ) -> None:
+        """Update the device info.
+
+        Convenience method to update all common device info
+        at once.
+
+        Args:
+            key (int): zone id
+            state (str): state
+            status (str, optional): status. Defaults to "Online".
+            last_activity (datetime, optional): last_activity_datetime.
+                Defaults to datetime.now().
+        """
+        temp = self._get_zonedata(key)
+        temp.state = state
+        temp.status = status
+        temp.last_activity_timestamp = last_activity.timestamp()
+        self.__setitem__(key, temp)
+
     def flatten(self) -> List[ADTPulseFlattendZone]:
         """Flattens ADTPulseZones into a list of ADTPulseFlattenedZones.
 
         Returns:
             List[ADTPulseFlattendZone]
         """
         result: List[ADTPulseFlattendZone] = []
```

## Comparing `pyadtpulse-1.0.2.dist-info/LICENSE.md` & `pyadtpulse-1.0.3.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyadtpulse-1.0.2.dist-info/METADATA` & `pyadtpulse-1.0.3.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyadtpulse
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python interface for ADT Pulse security systems
 Home-page: https://github.com/rsnodgrass/pyadtpulse
 Author: 
 Author-email: 
 License: Apache Software License
 Keywords: security system,adt,home automation,security alarm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
-Requires-Dist: requests (>=2.0)
+Requires-Dist: aiohttp (>=3.8.1)
+Requires-Dist: uvloop (==0.16.0)
 
 # pyadtpulse - Python interface for ADT Pulse
 
 Python client interface to the ADT Pulse security system.
 
 [![PyPi](https://img.shields.io/pypi/v/pyadtpulse.svg)](https://pypi.python.org/pypi/pyadtpulse)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

## Comparing `pyadtpulse-1.0.2.dist-info/RECORD` & `pyadtpulse-1.0.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyadtpulse/__init__.py,sha256=7jWHJ33ba3uIrwnXmfpggMYO5SMtH5SVcfd4MlhlukM,31842
+pyadtpulse/__init__.py,sha256=b5xr7SUiaZV2a6F7LpnKHgwbjpRU-3-_eHfEqYAXfGE,34446
 pyadtpulse/const.py,sha256=q3xJ93olyh9pNKvywARCwsu9qnr-E8O3SkD8Z4BEGBw,1609
-pyadtpulse/site.py,sha256=rXSy25p6n_uofeCwfZ0foCfALJ5Dct0TCu72pF1afpQ,24044
+pyadtpulse/site.py,sha256=L5fb9tXag8JQPPNVSOr-PNTYy5pJPVtdSPV2lmqnYoU,24957
 pyadtpulse/util.py,sha256=aTsrbEWoYkaAxnN0pU_ZoQ6eqyWTx-4_Ukihq8wwb88,4803
-pyadtpulse/zones.py,sha256=ZLdySMMGxMSvKGHqe9cDvFgchXlXnuCc-FFNRQSLqhE,5089
-pyadtpulse-1.0.2.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
-pyadtpulse-1.0.2.dist-info/METADATA,sha256=sjO12kMl0nnNhdyP78_UPvOMHp7CCvkvUU7UK2Pn4zg,3646
-pyadtpulse-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyadtpulse-1.0.2.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
-pyadtpulse-1.0.2.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pyadtpulse-1.0.2.dist-info/RECORD,,
+pyadtpulse/zones.py,sha256=6EADUsVXp0n-0WEEhjHzBoOd8bPZcqtl2TZvEfikaZM,5847
+pyadtpulse-1.0.3.dist-info/LICENSE.md,sha256=xnvwFqV8goAjucf1NpUuktsL7oj7PGSCWMg_1FpLwgY,581
+pyadtpulse-1.0.3.dist-info/METADATA,sha256=gdZjc3eEq-HUUDNxyn9iHqEcd8iNdTWQRh-Yj-l2ZcI,3680
+pyadtpulse-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyadtpulse-1.0.3.dist-info/top_level.txt,sha256=XUh_mjSYRt1I22U4qT370qb3b9avAb-CguvsPEM1dXU,11
+pyadtpulse-1.0.3.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pyadtpulse-1.0.3.dist-info/RECORD,,
```

