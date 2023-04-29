# Comparing `tmp/goxlrutilityapi-1.0.0.dev7.tar.gz` & `tmp/goxlrutilityapi-1.0.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goxlrutilityapi-1.0.0.dev7.tar", last modified: Sat Apr 29 12:07:28 2023, max compression
+gzip compressed data, was "goxlrutilityapi-1.0.0.dev8.tar", last modified: Sat Apr 29 13:26:08 2023, max compression
```

## Comparing `goxlrutilityapi-1.0.0.dev7.tar` & `goxlrutilityapi-1.0.0.dev8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.594775 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 12:07:27.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/request.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13324 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9402 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:07:28.594775 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 12:07:28.000000 goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 12:07:28.598775 goxlrutilityapi-1.0.0.dev7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 12:07:12.000000 goxlrutilityapi-1.0.0.dev7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.258676 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-29 13:26:06.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 13:26:08.258676 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-29 13:26:08.000000 goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 13:26:08.262676 goxlrutilityapi-1.0.0.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-29 13:25:54.000000 goxlrutilityapi-1.0.0.dev8/setup.py
```

### Comparing `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/__main__.py` & `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/__main__.py`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/const.py` & `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """GoXLR Utility API: Constants"""
 
 from typing import Any, Final
 
-from .models import DefaultBaseModel
 from .models.patch import Patch
 from .models.request import Request
 from .models.response import Response
 from .models.status import Status
 
 # Connection
 DEFAULT_HOST: Final[str] = "localhost"
 DEFAULT_PORT: Final[int] = 14564
 
 # Mixer
-VOLUME_MAX: Final[int] = 254
+VOLUME_MAX: Final[int] = 255
 
 # Request/Response Keys
 KEY_DATA: Final[str] = "data"
 KEY_ID: Final[str] = "id"
 KEY_TYPE: Final[str] = "type"
 
 # Request/Response Types
@@ -27,11 +26,11 @@
 
 # Models
 MODEL_PATCH: type[Patch] = Patch
 MODEL_REQUEST: type[Request] = Request
 MODEL_RESPONSE: type[Response[Any]] = Response
 MODEL_STATUS: type[Status] = Status
 
-MODEL_MAP: Final[dict[str, type[DefaultBaseModel]]] = {
+MODEL_MAP: Final[dict[str, Any]] = {
     RESPONSE_TYPE_PATCH: MODEL_PATCH,
     RESPONSE_TYPE_STATUS: MODEL_STATUS,
 }
```

### Comparing `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/models/status.py` & `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/models/status.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,37 +7,37 @@
 
 from . import DefaultBaseModel
 
 
 class Config(DefaultBaseModel):
     """Config Model"""
 
-    daemon_version: Optional[str] = Field(None, alias="DaemonVersion")
-    autostart_enabled: Optional[bool] = Field(None, alias="AutostartEnabled")
-    show_tray_icon: Optional[bool] = Field(None, alias="ShowTrayIcon")
-    tts_enabled: Optional[bool] = Field(None, alias="TTSEnabled")
+    daemon_version: Optional[str] = Field(None)
+    autostart_enabled: Optional[bool] = Field(None)
+    show_tray_icon: Optional[bool] = Field(None)
+    tts_enabled: Optional[bool] = Field(None)
 
 
 class Versions(DefaultBaseModel):
     """Versions Model"""
 
-    firmware: Optional[list[int]] = Field(None, alias="Firmware")
-    fpga_count: Optional[int] = Field(None, alias="FPGACount")
-    dice: Optional[list[int]] = Field(None, alias="DICE")
+    firmware: Optional[list[int]] = Field(None)
+    fpga_count: Optional[int] = Field(None)
+    dice: Optional[list[int]] = Field(None)
 
 
 class UsbDevice(DefaultBaseModel):
     """USB Device Model"""
 
-    manufacturer_name: str = Field(None, alias="ManufacturerName")
-    product_name: str = Field(None, alias="ProductName")
-    version: list[int] = Field(None, alias="Version")
-    bus_number: int = Field(None, alias="BusNumber")
-    address: int = Field(None, alias="Address")
-    identifier: str = Field(None, alias="Identifier")
+    manufacturer_name: str
+    product_name: str
+    version: list[int]
+    bus_number: int
+    address: int
+    identifier: str
 
 
 class Hardware(DefaultBaseModel):
     """Hardware Model"""
 
     versions: Versions
     serial_number: str
@@ -101,16 +101,16 @@
     equalizer1_k_hz: Optional[int] = Field(None, alias="Equalizer1KHz")
     equalizer63_hz: Optional[int] = Field(None, alias="Equalizer63Hz")
 
 
 class Equaliser(DefaultBaseModel):
     """Equaliser Model"""
 
-    gain: Optional[Gain] = Field(None, alias="Gain")
-    frequency: Optional[Frequency] = Field(None, alias="Frequency")
+    gain: Optional[Gain] = Field(None)
+    frequency: Optional[Frequency] = Field(None)
 
 
 class Gain1(DefaultBaseModel):
     """Gain1 Model"""
 
     equalizer90_hz: Optional[int] = Field(None, alias="Equalizer90Hz")
     equalizer250_hz: Optional[int] = Field(None, alias="Equalizer250Hz")
@@ -130,47 +130,47 @@
     equalizer8_k_hz: Optional[int] = Field(None, alias="Equalizer8KHz")
     equalizer500_hz: Optional[int] = Field(None, alias="Equalizer500Hz")
 
 
 class EqualiserMini(DefaultBaseModel):
     """Equaliser Mini Model"""
 
-    gain: Optional[Gain1] = Field(None, alias="Gain")
-    frequency: Optional[Frequency1] = Field(None, alias="Frequency")
+    gain: Optional[Gain1] = Field(None)
+    frequency: Optional[Frequency1] = Field(None)
 
 
 class NoiseGate(DefaultBaseModel):
     """Noise Gate Model"""
 
-    threshold: Optional[int] = Field(None, alias="Threshold")
-    attack: Optional[int] = Field(None, alias="Attack")
-    release: Optional[int] = Field(None, alias="Release")
-    enabled: Optional[bool] = Field(None, alias="Enabled")
-    attenuation: Optional[int] = Field(None, alias="Attenuation")
+    threshold: Optional[int] = Field(None)
+    attack: Optional[int] = Field(None)
+    release: Optional[int] = Field(None)
+    enabled: Optional[bool] = Field(None)
+    attenuation: Optional[int] = Field(None)
 
 
 class Compressor(DefaultBaseModel):
     """Compressor Model"""
 
-    threshold: Optional[int] = Field(None, alias="Threshold")
-    ratio: Optional[int] = Field(None, alias="Ratio")
-    attack: Optional[int] = Field(None, alias="Attack")
-    release: Optional[int] = Field(None, alias="Release")
-    makeup_gain: Optional[int] = Field(None, alias="MakeupGain")
+    threshold: Optional[int] = Field(None)
+    ratio: Optional[int] = Field(None)
+    attack: Optional[int] = Field(None)
+    release: Optional[int] = Field(None)
+    makeup_gain: Optional[int] = Field(None)
 
 
 class MicStatus(DefaultBaseModel):
     """Mic Status Model"""
 
-    mic_type: Optional[str] = Field(None, alias="MicType")
-    mic_gains: Optional[MicGains] = Field(None, alias="MicGains")
-    equaliser: Optional[Equaliser] = Field(None, alias="Equaliser")
-    equaliser_mini: Optional[EqualiserMini] = Field(None, alias="EqualiserMini")
-    noise_gate: Optional[NoiseGate] = Field(None, alias="NoiseGate")
-    compressor: Optional[Compressor] = Field(None, alias="Compressor")
+    mic_type: Optional[str] = Field(None)
+    mic_gains: Optional[MicGains] = Field(None)
+    equaliser: Optional[Equaliser] = Field(None)
+    equaliser_mini: Optional[EqualiserMini] = Field(None)
+    noise_gate: Optional[NoiseGate] = Field(None)
+    compressor: Optional[Compressor] = Field(None)
 
 
 class Volumes(DefaultBaseModel):
     """Volumes Model"""
 
     mic: int = Field(..., alias="Mic")
     line_in: int = Field(..., alias="LineIn")
@@ -184,19 +184,19 @@
     mic_monitor: int = Field(..., alias="MicMonitor")
     line_out: int = Field(..., alias="LineOut")
 
 
 class Levels(DefaultBaseModel):
     """Levels Model"""
 
-    submix_supported: Optional[bool] = Field(None, alias="SubmixSupported")
-    volumes: Volumes = Field(None, alias="Volumes")
-    submix: Optional[Any] = Field(None, alias="Submix")
-    bleep: Optional[int] = Field(None, alias="Bleep")
-    deess: Optional[int] = Field(None, alias="Deess")
+    submix_supported: Optional[bool] = Field(None)
+    volumes: Volumes
+    submix: Optional[Any] = Field(None)
+    bleep: Optional[int] = Field(None)
+    deess: Optional[int] = Field(None)
 
 
 class RouterItem(DefaultBaseModel):
     """Router Item Model"""
 
     headphones: Optional[bool] = Field(None, alias="Headphones")
     broadcast_mix: Optional[bool] = Field(None, alias="BroadcastMix")
@@ -217,31 +217,31 @@
     system: Optional[RouterItem] = Field(None, alias="System")
     samples: Optional[RouterItem] = Field(None, alias="Samples")
 
 
 class CoughButton(DefaultBaseModel):
     """Cough Button Model"""
 
-    is_toggle: Optional[bool] = Field(None, alias="IsToggle")
-    mute_type: Optional[str] = Field(None, alias="MuteType")
-    state: Optional[str] = Field(None, alias="State")
+    is_toggle: Optional[bool] = Field(None)
+    mute_type: Optional[str] = Field(None)
+    state: Optional[str] = Field(None)
 
 
 class Colours(DefaultBaseModel):
     """Colours Model"""
 
-    colour_one: Optional[str] = Field(None, alias="ColourOne")
-    colour_two: Optional[str] = Field(None, alias="ColourTwo")
+    colour_one: Optional[str] = Field(None)
+    colour_two: Optional[str] = Field(None)
 
 
 class Fader(DefaultBaseModel):
     """Fader Model"""
 
-    style: Optional[str] = Field(None, alias="Style")
-    colours: Optional[Colours] = Field(None, alias="Colours")
+    style: Optional[str] = Field(None)
+    colours: Optional[Colours] = Field(None)
 
 
 class Faders(DefaultBaseModel):
     """Faders Model"""
 
     a: Optional[Fader] = Field(None, alias="A")
     b: Optional[Fader] = Field(None, alias="B")
@@ -312,38 +312,38 @@
     mute_hold_duration: Optional[int]
     vc_mute_also_mute_cm: Optional[bool]
 
 
 class ButtonDown(DefaultBaseModel):
     """Button Down Model"""
 
-    fader1_mute: Optional[bool] = Field(None, alias="Fader1Mute")
-    fader2_mute: Optional[bool] = Field(None, alias="Fader2Mute")
-    fader3_mute: Optional[bool] = Field(None, alias="Fader3Mute")
-    fader4_mute: Optional[bool] = Field(None, alias="Fader4Mute")
-    bleep: Optional[bool] = Field(None, alias="Bleep")
-    cough: Optional[bool] = Field(None, alias="Cough")
-    effect_select1: Optional[bool] = Field(None, alias="EffectSelect1")
-    effect_select2: Optional[bool] = Field(None, alias="EffectSelect2")
-    effect_select3: Optional[bool] = Field(None, alias="EffectSelect3")
-    effect_select4: Optional[bool] = Field(None, alias="EffectSelect4")
-    effect_select5: Optional[bool] = Field(None, alias="EffectSelect5")
-    effect_select6: Optional[bool] = Field(None, alias="EffectSelect6")
-    effect_fx: Optional[bool] = Field(None, alias="EffectFx")
-    effect_megaphone: Optional[bool] = Field(None, alias="EffectMegaphone")
-    effect_robot: Optional[bool] = Field(None, alias="EffectRobot")
-    effect_hard_tune: Optional[bool] = Field(None, alias="EffectHardTune")
-    sampler_select_a: Optional[bool] = Field(None, alias="SamplerSelectA")
-    sampler_select_b: Optional[bool] = Field(None, alias="SamplerSelectB")
-    sampler_select_c: Optional[bool] = Field(None, alias="SamplerSelectC")
-    sampler_top_left: Optional[bool] = Field(None, alias="SamplerTopLeft")
-    sampler_top_right: Optional[bool] = Field(None, alias="SamplerTopRight")
-    sampler_bottom_left: Optional[bool] = Field(None, alias="SamplerBottomLeft")
-    sampler_bottom_right: Optional[bool] = Field(None, alias="SamplerBottomRight")
-    sampler_clear: Optional[bool] = Field(None, alias="SamplerClear")
+    fader1_mute: Optional[bool] = Field(None)
+    fader2_mute: Optional[bool] = Field(None)
+    fader3_mute: Optional[bool] = Field(None)
+    fader4_mute: Optional[bool] = Field(None)
+    bleep: Optional[bool] = Field(None)
+    cough: Optional[bool] = Field(None)
+    effect_select1: Optional[bool] = Field(None)
+    effect_select2: Optional[bool] = Field(None)
+    effect_select3: Optional[bool] = Field(None)
+    effect_select4: Optional[bool] = Field(None)
+    effect_select5: Optional[bool] = Field(None)
+    effect_select6: Optional[bool] = Field(None)
+    effect_fx: Optional[bool] = Field(None)
+    effect_megaphone: Optional[bool] = Field(None)
+    effect_robot: Optional[bool] = Field(None)
+    effect_hard_tune: Optional[bool] = Field(None)
+    sampler_select_a: Optional[bool] = Field(None)
+    sampler_select_b: Optional[bool] = Field(None)
+    sampler_select_c: Optional[bool] = Field(None)
+    sampler_top_left: Optional[bool] = Field(None)
+    sampler_top_right: Optional[bool] = Field(None)
+    sampler_bottom_left: Optional[bool] = Field(None)
+    sampler_bottom_right: Optional[bool] = Field(None)
+    sampler_clear: Optional[bool] = Field(None)
 
 
 class Mixer(DefaultBaseModel):
     """Mixer Model"""
 
     hardware: Hardware
     shutdown_commands: Optional[list]
```

### Comparing `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi/websocket_client.py` & `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi/websocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         response: Response[Status] = await self._send_message(
             Request(data=REQUEST_TYPE_GET_STATUS),
             wait_for_response=True,
             response_type=RESPONSE_TYPE_STATUS,
         )
         if response.data is None:
             raise BadMessageException("Message data is missing")
+        self._logger.debug("Status: %s", response.data)
         return response.data
 
     async def listen(
         self,
         patch_callback: Optional[Callable[[Response[Patch]], Awaitable[None]]] = None,
     ) -> None:
         """Listen for patches from GoXLR"""
@@ -209,15 +210,16 @@
                                 self._logger.debug(
                                     "Future already set for response ID: %s",
                                     message_id,
                                 )
 
                 if patch_callback is not None and message_type == RESPONSE_TYPE_PATCH:
                     try:
-                        await patch_callback(Response[Patch](**response.dict()))
+                        self._logger.debug("Patch response: %s", response)
+                        await patch_callback(response)
                     except (TypeError, ValidationError) as error:
                         raise BadMessageException(
                             f"Failed to create model patch response with data:\n{response.data}"
                         ) from error
 
         await self._listen_for_messages(callback=_message_callback)
```

### Comparing `goxlrutilityapi-1.0.0.dev7/goxlrutilityapi.egg-info/SOURCES.txt` & `goxlrutilityapi-1.0.0.dev8/goxlrutilityapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev7/pyproject.toml` & `goxlrutilityapi-1.0.0.dev8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `goxlrutilityapi-1.0.0.dev7/setup.py` & `goxlrutilityapi-1.0.0.dev8/setup.py`

 * *Files identical despite different names*

