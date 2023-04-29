# Comparing `tmp/goxlrutilityapi-1.0.0.dev5.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev5.tar", last modified: Fri Apr 28 23:17:40 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev6.tar", last modified: Sat Apr 29 01:57:34 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev5.tar` & `goxlrutilityapi-1.0.0.dev6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.842442 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-28 23:17:39.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13653 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:17:40.842442 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 23:17:40.000000 goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:17:40.846442 goxlrutilityapi-1.0.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-28 23:17:20.000000 goxlrutilityapi-1.0.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.083793 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 01:57:32.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13435 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 01:57:34.083793 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 01:57:34.000000 goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 01:57:34.087793 goxlrutilityapi-1.0.0.dev6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 01:57:15.000000 goxlrutilityapi-1.0.0.dev6/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/models/status.py`

 * *Files 23% similar despite different names*

```diff
@@ -45,27 +45,27 @@
     device_type: str
     usb_device: UsbDevice
 
 
 class FaderStatus(DefaultBaseModel):
     """Fader Status Model"""
 
-    channel: Optional[str] = Field(None, alias="Channel")
-    mute_type: Optional[str] = Field(None, alias="MuteType")
+    channel: str = Field(..., alias="Channel")
+    mute_type: str = Field(..., alias="MuteType")
     scribble: Optional[Any] = Field(None, alias="Scribble")
-    mute_state: Optional[str] = Field(None, alias="MuteState")
+    mute_state: str = Field(..., alias="MuteState")
 
 
 class FaderStatuses(DefaultBaseModel):
     """Fader Statuses Model"""
 
-    a: Optional[FaderStatus] = Field(None, alias="A")
-    b: Optional[FaderStatus] = Field(None, alias="B")
-    c: Optional[FaderStatus] = Field(None, alias="C")
-    d: Optional[FaderStatus] = Field(None, alias="D")
+    a: FaderStatus = Field(..., alias="A")
+    b: FaderStatus = Field(..., alias="B")
+    c: FaderStatus = Field(..., alias="C")
+    d: FaderStatus = Field(..., alias="D")
 
 
 class MicGains(DefaultBaseModel):
     """Mic Gains Model"""
 
     dynamic: Optional[int] = Field(None, alias="Dynamic")
     condenser: Optional[int] = Field(None, alias="Condenser")
@@ -168,32 +168,32 @@
     noise_gate: Optional[NoiseGate] = Field(None, alias="NoiseGate")
     compressor: Optional[Compressor] = Field(None, alias="Compressor")
 
 
 class Volumes(DefaultBaseModel):
     """Volumes Model"""
 
-    mic: Optional[int] = Field(None, alias="Mic")
-    line_in: Optional[int] = Field(None, alias="LineIn")
-    console: Optional[int] = Field(None, alias="Console")
-    system: Optional[int] = Field(None, alias="System")
-    game: Optional[int] = Field(None, alias="Game")
-    chat: Optional[int] = Field(None, alias="Chat")
-    sample: Optional[int] = Field(None, alias="Sample")
-    music: Optional[int] = Field(None, alias="Music")
-    headphones: Optional[int] = Field(None, alias="Headphones")
-    mic_monitor: Optional[int] = Field(None, alias="MicMonitor")
-    line_out: Optional[int] = Field(None, alias="LineOut")
+    mic: int = Field(..., alias="Mic")
+    line_in: int = Field(..., alias="LineIn")
+    console: int = Field(..., alias="Console")
+    system: int = Field(..., alias="System")
+    game: int = Field(..., alias="Game")
+    chat: int = Field(..., alias="Chat")
+    sample: int = Field(..., alias="Sample")
+    music: int = Field(..., alias="Music")
+    headphones: int = Field(..., alias="Headphones")
+    mic_monitor: int = Field(..., alias="MicMonitor")
+    line_out: int = Field(..., alias="LineOut")
 
 
 class Levels(DefaultBaseModel):
     """Levels Model"""
 
     submix_supported: Optional[bool] = Field(None, alias="SubmixSupported")
-    volumes: Optional[Volumes] = Field(None, alias="Volumes")
+    volumes: Volumes = Field(None, alias="Volumes")
     submix: Optional[Any] = Field(None, alias="Submix")
     bleep: Optional[int] = Field(None, alias="Bleep")
     deess: Optional[int] = Field(None, alias="Deess")
 
 
 class RouterItem(DefaultBaseModel):
     """Router Item Model"""
@@ -345,15 +345,15 @@
 class Mixer(DefaultBaseModel):
     """Mixer Model"""
 
     hardware: Hardware
     shutdown_commands: Optional[list]
     fader_status: Optional[FaderStatuses]
     mic_status: Optional[MicStatus]
-    levels: Optional[Levels]
+    levels: Levels
     router: Optional[Router]
     cough_button: Optional[CoughButton]
     lighting: Optional[Lighting]
     effects: Optional[Any]
     sampler: Optional[Any]
     settings: Optional[Settings]
     button_down: Optional[ButtonDown]
```

### Comparing `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi/websocket_client.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev5/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev6/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev5/pyproject.toml` & `goxlrutilityapi-1.0.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev5/setup.py` & `goxlrutilityapi-1.0.0.dev6/setup.py`

 * *Files identical despite different names*

