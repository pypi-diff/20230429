# Comparing `tmp/pyecotrend-ista-2.0.8.tar.gz` & `tmp/pyecotrend-ista-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecotrend-ista-2.0.8.tar", last modified: Tue Apr 25 08:14:18 2023, max compression
+gzip compressed data, was "pyecotrend-ista-2.0.9.tar", last modified: Wed Apr 26 07:39:33 2023, max compression
```

## Comparing `pyecotrend-ista-2.0.8.tar` & `pyecotrend-ista-2.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.753484 pyecotrend-ista-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.753484 pyecotrend-ista-2.0.8/src/pyecotrend_ista/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/helper_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/ista_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    23317 2023-04-25 08:14:02.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista/pyecotrend_ista.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:14:18.757484 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 08:14:18.000000 pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:39:33.607851 pyecotrend-ista-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-26 07:39:33.607851 pyecotrend-ista-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:39:33.607851 pyecotrend-ista-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:39:33.603850 pyecotrend-ista-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:39:33.603850 pyecotrend-ista-2.0.9/src/pyecotrend_ista/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5115 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista/helper_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista/ista_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-04-26 07:39:17.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista/pyecotrend_ista.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:39:33.607851 pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-26 07:39:33.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-26 07:39:33.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:39:33.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-26 07:39:33.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 07:39:33.000000 pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/top_level.txt
```

### Comparing `pyecotrend-ista-2.0.8/LICENSE` & `pyecotrend-ista-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.8/PKG-INFO` & `pyecotrend-ista-2.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
@@ -30,16 +30,14 @@
 [![PyPI version](https://badge.fury.io/py/pyecotrend-ista.svg)](https://badge.fury.io/py/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista)](https://pepy.tech/project/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista/month)](https://pepy.tech/project/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista/week)](https://pepy.tech/project/pyecotrend-ista)
 
 [![GitHub issues](https://img.shields.io/github/issues/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista/issues)
 [![GitHub forks](https://img.shields.io/github/forks/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista)
 [![GitHub stars](https://img.shields.io/github/stars/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista)
 [![GitHub license](https://img.shields.io/github/license/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=appveyor)](https://github.com/psf/black)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Ludy87/pyecotrend-ista.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/Ludy87/pyecotrend-ista/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Ludy87/pyecotrend-ista.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/Ludy87/pyecotrend-ista/context:python)
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ludy87)
 
 [✨ Wishlist from Amazon ✨](https://smile.amazon.de/registry/wishlist/2MX8QK8VE9MV1)
 
 ---
 Unofficial python library for the pyecotrend-ista API
```

### Comparing `pyecotrend-ista-2.0.8/README.md` & `pyecotrend-ista-2.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 [![PyPI version](https://badge.fury.io/py/pyecotrend-ista.svg)](https://badge.fury.io/py/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista)](https://pepy.tech/project/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista/month)](https://pepy.tech/project/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista/week)](https://pepy.tech/project/pyecotrend-ista)
 
 [![GitHub issues](https://img.shields.io/github/issues/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista/issues)
 [![GitHub forks](https://img.shields.io/github/forks/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista)
 [![GitHub stars](https://img.shields.io/github/stars/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista)
 [![GitHub license](https://img.shields.io/github/license/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=appveyor)](https://github.com/psf/black)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Ludy87/pyecotrend-ista.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/Ludy87/pyecotrend-ista/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Ludy87/pyecotrend-ista.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/Ludy87/pyecotrend-ista/context:python)
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ludy87)
 
 [✨ Wishlist from Amazon ✨](https://smile.amazon.de/registry/wishlist/2MX8QK8VE9MV1)
 
 ---
 Unofficial python library for the pyecotrend-ista API
```

### Comparing `pyecotrend-ista-2.0.8/setup.py` & `pyecotrend-ista-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyecotrend-ista-2.0.8/src/pyecotrend_ista/helper_object.py` & `pyecotrend-ista-2.0.9/src/pyecotrend_ista/ista_object.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,151 +1,169 @@
 from __future__ import annotations
 
-from dataclasses import dataclass
-from typing import Dict, List, Optional
+from dataclasses import dataclass, field
+from typing import Any, List, Optional
 
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 
 
 @dataclass_json
 @dataclass
-class AverageConsumption(DataClassJsonMixin):
-    averageConsumptionValue: float
-    residentConsumptionValue: float
-    averageConsumptionPercentage: int
-    residentConsumptionPercentage: int
-    additionalAverageConsumptionValue: float
-    additionalResidentConsumptionValue: float
-    additionalAverageConsumptionPercentage: int
-    additionalResidentConsumptionPercentage: int
+class Resident(DataClassJsonMixin):
+    movedOut: bool
+    moveOutDate: Any
+    invalid: bool
+    invalidDate: Any
 
-    def replace_point(self):
-        for _field in self.__dataclass_fields__.values():
-            if _field.name in [
-                "averageConsumptionValue",
-                "residentConsumptionValue",
-                "additionalAverageConsumptionValue",
-                "additionalResidentConsumptionValue",
-            ]:
-                if isinstance(getattr(self, _field.name), str):
-                    setattr(self, _field.name, float(getattr(self, _field.name).replace(",", ".")))
 
-    def __post_init__(self):
-        self.replace_point()
+@dataclass_json
+@dataclass
+class Date(DataClassJsonMixin):
+    month: int
+    year: int
+
+    def __str__(self) -> str:
+        return self.schema().dumps(self.to_dict())
 
 
 @dataclass_json
 @dataclass
-class ComparedConsumption:
-    lastYearValue: float
-    period: Date
-    smiley: str
-    comparedPercentage: int
-    comparedValue: float
+class AcerageConsumption(DataClassJsonMixin):
+    averageConsumptionValue: float
+    residentConsumptionValue: float
+    averageConsumptionPercentage: float
+    residentConsumptionPercentage: float
+    additionalAverageConsumptionValue: float
+    additionalResidentConsumptionValue: float
+    additionalAverageConsumptionPercentage: float
+    additionalResidentConsumptionPercentage: float
 
     def replace_point(self):
         for _field in self.__dataclass_fields__.values():
-            if _field.name in ["lastYearValue", "comparedValue"]:
-                if isinstance(getattr(self, _field.name), str):
-                    setattr(self, _field.name, float(getattr(self, _field.name).replace(",", ".")))
-                else:
-                    setattr(self, _field.name, float(getattr(self, _field.name)))
+            if isinstance(getattr(self, _field.name), str):
+                setattr(self, _field.name, float(getattr(self, _field.name).replace(",", ".")))
 
     def __post_init__(self):
         self.replace_point()
 
 
 @dataclass_json
 @dataclass
-class Consumption(DataClassJsonMixin):
-    type: str
-    value: float
-    unit: str
-    additionalValue: float
-    additionalUnit: str
-    estimated: bool
-    comparedConsumption: Optional[ComparedConsumption]
-    comparedCost: Optional[ComparedConsumption]
-    averageConsumption: Optional[AverageConsumption]  # field(default_factory=AverageConsumption)
+class Readings(DataClassJsonMixin):
+    type: Optional[str] = None
+    value: Optional[float] = None
+    unit: Optional[str] = None
+    additionalValue: Optional[float] = None
+    additionalUnit: Optional[str] = None
+    averageConsumption: Optional[AcerageConsumption] = None
 
     def replace_point(self):
-        for _field in self.__dataclass_fields__.values():
-            if _field.name in ["value", "additionalValue"]:
-                if isinstance(getattr(self, _field.name), str):
-                    setattr(self, _field.name, float(getattr(self, _field.name).replace(",", ".")))
+        if isinstance(self.additionalValue, str):
+            self.additionalValue = float(self.additionalValue.replace(",", "."))
+        if isinstance(self.value, str):
+            self.value = float(self.value.replace(",", "."))
 
     def __post_init__(self):
         self.replace_point()
 
 
 @dataclass_json
 @dataclass
-class Cost(DataClassJsonMixin):
-    type: str
-    value: int
-    unit: str
-    estimated: bool
-    comparedCost: Optional[ComparedConsumption]
+class Consumptions(DataClassJsonMixin):
+    date: Optional[Date]
+    readings: Optional[List[Readings]]
+    exception: Optional[str]
 
 
 @dataclass_json
 @dataclass
-class Date(DataClassJsonMixin):
-    month: int
-    year: int
+class CostsByEnergyType(DataClassJsonMixin):
+    type: Optional[str]
+    value: Optional[int]
+    unit: Optional[str]
 
+    def replace_point(self):
+        if isinstance(self.value, int):
+            self.value = float(self.value)
+        elif isinstance(self.value, str):
+            self.value = float(self.value.replace(",", "."))
 
-@dataclass_json
-@dataclass
-class LastValue(DataClassJsonMixin):
-    heating: Optional[float] = None
-    warmwater: Optional[float] = None
-    water: Optional[float] = None
-    month: Optional[int] = None
-    year: Optional[int] = None
+    def __post_init__(self):
+        self.replace_point()
 
 
 @dataclass_json
 @dataclass
-class LastCosts(DataClassJsonMixin):
-    heating: Optional[float] = None
-    warmwater: Optional[float] = None
-    water: Optional[float] = None
-    month: Optional[int] = None
-    year: Optional[int] = None
-    unit: Optional[str] = None
+class Costs(DataClassJsonMixin):
+    date: Date
+    costsByEnergyType: Optional[List[CostsByEnergyType]]
+    exception: Optional[str]
 
 
 @dataclass_json
 @dataclass
-class CombinedData(DataClassJsonMixin):
-    date: Date
-    consumptions: List[Consumption]
-    costs: List[Cost]
+class Co2EmissionsBillingPeriods(DataClassJsonMixin):
+    currentBillingPeriod: Any
+    previousBillingPeriod: Any
 
 
 @dataclass_json
 @dataclass
-class TotalAdditionalValues(DataClassJsonMixin):
-    heating: Optional[float] = None
-    warmwater: Optional[float] = None
-    water: Optional[float] = None
+class IstaResult(DataClassJsonMixin):
+    consumptionUnitId: Optional[str] = None
+    resident: Optional[Resident] = None
+    co2Emissions: Optional[str] = None
+    co2EmissionsBillingPeriods: Optional[Co2EmissionsBillingPeriods] = None
+    costs: Optional[List[Costs]] = field(default_factory=list)
+    consumptions: Optional[List[Consumptions]] = field(default_factory=list)
 
 
 @dataclass_json
 @dataclass
-class SumByYear(DataClassJsonMixin):
-    heating: Optional[Dict[int, float]] = None
-    warmwater: Optional[Dict[int, float]] = None
-    water: Optional[Dict[int, float]] = None
+class CostConsumptions(DataClassJsonMixin):
+    supportCode: str
+    consumptionUnitId: str
+    entity_id: str
+    date: Date
+    type: str
+    consumption_additionalUnit: str
+    consumption_additionalValue: float
+    consumption_unit: str
+    consumption_value: float
+    hasCost: bool = False
+    cost_unit: Optional[str] = None
+    cost_value: Optional[int] = None
 
 
 @dataclass_json
 @dataclass
-class CustomRaw(DataClassJsonMixin):
-    consum_types: Optional[List[str]]
-    combined_data: List[CombinedData]
-    total_additional_values: TotalAdditionalValues
-    last_value: LastValue
-    all_dates: List[Date]
-    sum_by_year: SumByYear
-    last_costs: Optional[LastCosts]
+class ResultAccount(DataClassJsonMixin):
+    firstName: str
+    lastName: str
+    email: str
+    keycloakId: Optional[str]
+    country: str
+    locale: str
+    authcode: Optional[str]
+    tos: str
+    tosUpdated: str
+    privacy: Optional[str]
+    mobileNumber: str
+    transitionMobileNumber: str
+    unconfirmedPhoneNumber: str
+    password: Optional[str]
+    enabled: bool
+    consumptionUnitUuids: Optional[List[str]]
+    residentTimeRangeUuids: Optional[List[str]]
+    ads: bool
+    marketing: bool
+    fcmToken: str
+    betaPhase: Optional[str]
+    notificationMethod: str
+    emailConfirmed: bool
+    isDemo: bool
+    userGroup: str
+    mobileLoginStatus: str
+    residentAndConsumptionUuidsMap: dict
+    activeConsumptionUnit: str
+    supportCode: str
+    notificationMethodEmailConfirmed: bool
```

### Comparing `pyecotrend-ista-2.0.8/src/pyecotrend_ista/pyecotrend_ista.py` & `pyecotrend-ista-2.0.9/src/pyecotrend_ista/pyecotrend_ista.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from asyncio import TimeoutError, sleep
 from random import randint
 from typing import Any, Dict
 
 import aiohttp
 
 from .const import ACCOUNT_URL, CONSUMPTIONS_URL, LOGIN_HEADER, LOGIN_URL, MAX_RETRIES, REFRESH_TOKEN_URL, RETRY_DELAY, VERSION
-from .exception_classes import Error, LoginError, ServerError
+from .exception_classes import Error, InternalServerError, LoginError, ServerError
 from .helper_object import CustomRaw
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class PyEcotrendIsta:
     def __init__(self, email: str, password: str, logger, hass_dir: str | None = None) -> None:
@@ -79,15 +79,18 @@
                         json_str_resp = await response.json()
                         self._accessToken = json_str_resp["accessToken"]
                         self._refreshToken = json_str_resp["refreshToken"]
                         self._accessTokenExpiresIn = json_str_resp["accessTokenExpiresIn"]
                     elif response.status == 401:
                         raise LoginError((await response.json()).get("key", None))
                     elif response.status == 500:
-                        continue
+                        if isinstance(response.reason, str) and response.reason == "Internal Server Error":
+                            raise InternalServerError(response.reason)
+                        raise ServerError()
+                        # continue
                     elif response.status != 200:
                         raise Error(await response.json())
                     else:
                         raise Exception("Unknow Error", response.status, await response.text())
         return self._accessToken
 
     async def __refresh(self) -> None:
@@ -194,15 +197,20 @@
                     self._accessToken = await self.__login()
                 except LoginError as error:
                     # Login failed
                     self._accessToken = None
                     self._LOGGER.error(error)
                     raise LoginError(error)
                 except ServerError:
-                    await sleep(RETRY_DELAY)
+                    if retryCounter < MAX_RETRIES:
+                        await sleep(RETRY_DELAY)
+                    else:
+                        raise ServerError()
+                except InternalServerError as error:
+                    raise Exception(error.msg)
                 except Error as err:
                     raise Exception(err)
                 if not self._accessToken:
                     await sleep(RETRY_DELAY)
                 else:
                     await self.__setAccount()
         return self._accessToken
@@ -304,14 +312,20 @@
                                     else (
                                         float(reading["additionalValue"].replace(",", "."))
                                         if reading["additionalValue"] is not None
                                         else 0.0
                                     ),
                                     1,
                                 )
+                                if reading["type"] == "warmwater":
+                                    sum_by_year["ww"] = reading["unit"]
+                                elif reading["type"] == "water":
+                                    sum_by_year["w"] = reading["unit"]
+                                else:
+                                    sum_by_year["h"] = reading["additionalUnit"]
 
             indices_to_delete_costs = []
             for i, costs in enumerate(c_raw["costs"]):
                 new_readings = list()
                 if select_month is None and select_year is None:
                     for reading in costs["costsByEnergyType"]:
                         if filter_none and reading["type"] is not None:
@@ -368,49 +382,108 @@
                             "consumptions": consumption_entry["readings"],
                             "costs": cost_entry["costsByEnergyType"],
                         }
 
                         combined_data.append(combined_entry)
 
             total_additional_values = {}
+            total_additional_custom_values = {}
             for consumption_unit in consumptions:
                 for reading in consumption_unit["readings"]:
-                    if reading["type"] is None or reading["value"] is None:
+                    if reading["type"] is None or reading["value"] is None or reading["additionalValue"] is None:
                         continue
+
+                    if reading["type"] not in total_additional_custom_values:
+                        total_additional_custom_values[reading["type"]] = 0.0
+                    total_additional_custom_values[reading["type"]] += round(
+                        float(reading["additionalValue"].replace(",", "."))
+                        if reading["type"] == "warmwater" or reading["type"] == "water"
+                        else (
+                            float(reading["value"].replace(",", "."))
+                            if reading["value"] is not None
+                            else 0.0
+                        ),
+                        1,
+                    )
+                    if reading["type"] == "warmwater":
+                        total_additional_custom_values["ww"] = reading["additionalUnit"]
+                    elif reading["type"] == "water":
+                        total_additional_custom_values["w"] = reading["additionalUnit"]
+                    elif reading["type"] == "heating":
+                        total_additional_custom_values["h"] = reading["unit"]
+
                     if reading["type"] not in total_additional_values:
                         total_additional_values[reading["type"]] = 0.0
                     total_additional_values[reading["type"]] += round(
                         float(reading["value"].replace(",", "."))
                         if reading["type"] == "warmwater" or reading["type"] == "water"
                         else (
                             float(reading["additionalValue"].replace(",", "."))
                             if reading["additionalValue"] is not None
                             else 0.0
                         ),
                         1,
                     )
+                    if reading["type"] == "warmwater":
+                        total_additional_values["ww"] = reading["unit"]
+                    elif reading["type"] == "water":
+                        total_additional_values["w"] = reading["unit"]
+                    elif reading["type"] == "heating":
+                        total_additional_values["h"] = reading["additionalUnit"]
 
             last_value = None
+            last_custom_value = None
             if consumptions:
                 if last_value is None:
                     last_value = {}
+                if last_custom_value is None:
+                    last_custom_value = {}
                 for reading in consumptions[0]["readings"]:
-                    if reading["type"] is None:
+                    if reading["type"] is None or reading["value"] is None or reading["additionalValue"] is None:
                         continue
+
+                    if reading["type"] not in last_custom_value:
+                        last_custom_value[reading["type"]] = 0.0
+                    last_custom_value[reading["type"]] += (
+                        float(reading["additionalValue"].replace(",", "."))
+                        if reading["type"] == "warmwater" or reading["type"] == "water"
+                        else (
+                            float(reading["value"].replace(",", "."))
+                            if reading["value"] is not None
+                            else 0.0
+                        )
+                    )
+                    if reading["type"] == "warmwater":
+                        last_custom_value["ww"] = reading["additionalUnit"]
+                    elif reading["type"] == "water":
+                        last_custom_value["w"] = reading["additionalUnit"]
+                    elif reading["type"] == "heating":
+                        last_custom_value["h"] = reading["unit"]
+
                     if reading["type"] not in last_value:
                         last_value[reading["type"]] = 0.0
                     last_value[reading["type"]] += (
                         float(reading["value"].replace(",", "."))
                         if reading["type"] == "warmwater" or reading["type"] == "water"
                         else (
                             float(reading["additionalValue"].replace(",", "."))
                             if reading["additionalValue"] is not None
                             else 0.0
                         )
                     )
+                    if reading["type"] == "warmwater":
+                        last_value["ww"] = reading["unit"]
+                    elif reading["type"] == "water":
+                        last_value["w"] = reading["unit"]
+                    elif reading["type"] == "heating":
+                        last_value["h"] = reading["additionalUnit"]
+
+                last_custom_value["month"] = consumptions[0]["date"]["month"]
+                last_custom_value["year"] = consumptions[0]["date"]["year"]
+
                 last_value["month"] = consumptions[0]["date"]["month"]
                 last_value["year"] = consumptions[0]["date"]["year"]
 
             last_costs = None
             if costs:
                 if last_costs is None:
                     last_costs = {}
@@ -440,15 +513,17 @@
                 last_costs["year"] = costs[0]["date"]["year"]
 
             return CustomRaw.from_dict(
                 {
                     "consum_types": consum_types,
                     "combined_data": None,  # combined_data,
                     "total_additional_values": total_additional_values,
+                    "total_additional_custom_values": total_additional_custom_values,
                     "last_value": last_value,
+                    "last_custom_value": last_custom_value,
                     "last_costs": last_costs,
                     "all_dates": None,  # all_dates,
                     "sum_by_year": sum_by_year,
                 }
             ).to_dict()
         return c_raw
```

### Comparing `pyecotrend-ista-2.0.8/src/pyecotrend_ista.egg-info/PKG-INFO` & `pyecotrend-ista-2.0.9/src/pyecotrend_ista.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecotrend-ista
-Version: 2.0.8
+Version: 2.0.9
 Summary: Python ecotrend-ista Api
 Home-page: https://github.com/Ludy87/pyecotrend-ista
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyecotrend-ista/issues
 Keywords: python api ecotrend ista
@@ -30,16 +30,14 @@
 [![PyPI version](https://badge.fury.io/py/pyecotrend-ista.svg)](https://badge.fury.io/py/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista)](https://pepy.tech/project/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista/month)](https://pepy.tech/project/pyecotrend-ista) [![Downloads](https://pepy.tech/badge/pyecotrend-ista/week)](https://pepy.tech/project/pyecotrend-ista)
 
 [![GitHub issues](https://img.shields.io/github/issues/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista/issues)
 [![GitHub forks](https://img.shields.io/github/forks/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista)
 [![GitHub stars](https://img.shields.io/github/stars/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista)
 [![GitHub license](https://img.shields.io/github/license/Ludy87/pyecotrend-ista?style=for-the-badge&logo=appveyor)](https://github.com/Ludy87/pyecotrend-ista/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge&logo=appveyor)](https://github.com/psf/black)
-[![Total alerts](https://img.shields.io/lgtm/alerts/g/Ludy87/pyecotrend-ista.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/Ludy87/pyecotrend-ista/alerts/)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/Ludy87/pyecotrend-ista.svg?logo=lgtm&logoWidth=18&style=for-the-badge)](https://lgtm.com/projects/g/Ludy87/pyecotrend-ista/context:python)
 
 [!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/ludy87)
 
 [✨ Wishlist from Amazon ✨](https://smile.amazon.de/registry/wishlist/2MX8QK8VE9MV1)
 
 ---
 Unofficial python library for the pyecotrend-ista API
```

