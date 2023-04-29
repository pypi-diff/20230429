# Comparing `tmp/python-weather-1.0.0.tar.gz` & `tmp/python-weather-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-weather-1.0.0.tar", last modified: Thu Apr 27 17:25:51 2023, max compression
+gzip compressed data, was "python-weather-1.0.1.tar", last modified: Sat Apr 29 06:28:53 2023, max compression
```

## Comparing `python-weather-1.0.0.tar` & `python-weather-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:25:51.886263 python-weather-1.0.0/
--rw-rw-rw-   0        0        0     1106 2023-04-07 14:23:45.000000 python-weather-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      107 2023-04-25 12:21:36.000000 python-weather-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3760 2023-04-27 17:25:51.886263 python-weather-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2176 2023-04-27 17:25:05.000000 python-weather-1.0.0/README.md
--rw-rw-rw-   0        0        0     1437 2023-04-27 17:12:14.000000 python-weather-1.0.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-27 17:25:51.839392 python-weather-1.0.0/python_weather/
--rw-rw-rw-   0        0        0     1503 2023-04-24 06:22:15.000000 python-weather-1.0.0/python_weather/__init__.py
--rw-rw-rw-   0        0        0     5663 2023-04-24 15:06:57.000000 python-weather-1.0.0/python_weather/base.py
--rw-rw-rw-   0        0        0     5697 2023-04-23 09:54:58.000000 python-weather-1.0.0/python_weather/client.py
--rw-rw-rw-   0        0        0     1313 2023-04-23 08:55:28.000000 python-weather-1.0.0/python_weather/constants.py
--rw-rw-rw-   0        0        0    10164 2023-04-24 15:21:41.000000 python-weather-1.0.0/python_weather/enums.py
--rw-rw-rw-   0        0        0     1262 2023-04-16 12:24:11.000000 python-weather-1.0.0/python_weather/errors.py
--rw-rw-rw-   0        0        0    12805 2023-04-24 15:16:05.000000 python-weather-1.0.0/python_weather/forecast.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:25:51.886263 python-weather-1.0.0/python_weather.egg-info/
--rw-rw-rw-   0        0        0     3760 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      412 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 17:25:51.000000 python-weather-1.0.0/python_weather.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 17:25:51.886263 python-weather-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 06:28:53.821119 python-weather-1.0.1/
+-rw-rw-rw-   0        0        0     1106 2023-04-07 14:23:45.000000 python-weather-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      107 2023-04-25 12:21:36.000000 python-weather-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3760 2023-04-29 06:28:53.819121 python-weather-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2176 2023-04-29 06:26:46.000000 python-weather-1.0.1/README.md
+-rw-rw-rw-   0        0        0     1437 2023-04-29 06:15:32.000000 python-weather-1.0.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-29 06:28:53.720462 python-weather-1.0.1/python_weather/
+-rw-rw-rw-   0        0        0     1503 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/__init__.py
+-rw-rw-rw-   0        0        0     5663 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/base.py
+-rw-rw-rw-   0        0        0     5683 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/client.py
+-rw-rw-rw-   0        0        0     1295 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/constants.py
+-rw-rw-rw-   0        0        0    10134 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/enums.py
+-rw-rw-rw-   0        0        0     1262 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/errors.py
+-rw-rw-rw-   0        0        0    12805 2023-04-29 06:25:45.000000 python-weather-1.0.1/python_weather/forecast.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:28:53.815120 python-weather-1.0.1/python_weather.egg-info/
+-rw-rw-rw-   0        0        0     3760 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-04-29 06:28:53.000000 python-weather-1.0.1/python_weather.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-29 06:28:52.000000 python-weather-1.0.1/python_weather.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-29 06:28:53.821119 python-weather-1.0.1/setup.cfg
```

### Comparing `python-weather-1.0.0/LICENSE` & `python-weather-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.0/PKG-INFO` & `python-weather-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 1.0.0
+Version: 1.0.1
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/python-weather
-Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.0.tar.gz
+Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.1.tar.gz
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-weather-1.0.0/README.md` & `python-weather-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.0/pyproject.toml` & `python-weather-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "python-weather"
-version = "1.0.0"
+version = "1.0.1"
 description = "A free and asynchronous weather API wrapper made in Python, for Python."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "forecast", "weather-api", "weather-forecast"]
 dependencies = ["aiohttp==3.8.4"]
 classifiers = [
@@ -34,8 +34,8 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/null8626/python-weather"
-download_url = "https://github.com/null8626/python-weather/archive/1.0.0.tar.gz"
+download_url = "https://github.com/null8626/python-weather/archive/1.0.1.tar.gz"
```

### Comparing `python-weather-1.0.0/python_weather/__init__.py` & `python-weather-1.0.1/python_weather/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 """
 
 from .enums import Kind, Locale, Phase, Ultraviolet, WindDirection
 from .constants import METRIC, IMPERIAL
 from .client import Client
 from .errors import Error
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 __all__ = (
   'METRIC', 'IMPERIAL', 'Client', 'Error', 'Kind', 'Locale', 'Phase',
   'Ultraviolet', 'WindDirection'
 )
```

### Comparing `python-weather-1.0.0/python_weather/base.py` & `python-weather-1.0.1/python_weather/base.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.0/python_weather/client.py` & `python-weather-1.0.1/python_weather/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from aiohttp import ClientSession, ClientTimeout, TCPConnector
 from urllib.parse import quote_plus
-from typing import Optional, Self
+from typing import Optional
 from asyncio import sleep
 from enum import auto
 
 from .constants import METRIC, VALID_UNITS
 from .base import CustomizableBase
 from .forecast import Weather
 from .errors import Error
@@ -144,15 +144,15 @@
     """|coro|
     Closes the :class:`Client` object. Nothing will happen if it's already closed.
     """
     
     if not self.__session.closed:
       await self.__session.close()
   
-  async def __aenter__(self) -> Self:
+  async def __aenter__(self):
     """|coro|
     `async with` handler. Does nothing. Returns `self`
     """
     
     return self
   
   async def __aexit__(self, *_, **__):
```

### Comparing `python-weather-1.0.0/python_weather/constants.py` & `python-weather-1.0.1/python_weather/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from re import compile
 from enum import auto
 
-METRIC = auto('METRIC')
-IMPERIAL = auto('IMPERIAL')
+METRIC = auto()
+IMPERIAL = auto()
 
 LATLON_REGEX = compile(r'^Lat (\-?[\d\.]+) and Lon (\-?[\d\.]+)$')
 VALID_UNITS = (METRIC, IMPERIAL)
```

### Comparing `python-weather-1.0.0/python_weather/enums.py` & `python-weather-1.0.1/python_weather/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from typing import Union, Self
 from enum import Enum, auto
+from typing import Union
 
 from .errors import Error
 
 class BasicEnum(Enum):
   __slots__ = ()
   
   def __repr__(self) -> str:
@@ -48,15 +48,15 @@
   LOW = auto()
   MODERATE = auto()
   HIGH = auto()
   VERY_HIGH = auto()
   EXTREME = auto()
   
   @classmethod
-  def _missing_(self, index: int) -> Self:
+  def _missing_(self, index: int):
     if index <= 2:
       return self.LOW
     elif index <= 5:
       return self.MODERATE
     elif index <= 7:
       return self.HIGH
     elif index <= 10:
@@ -82,15 +82,15 @@
   SOUTHWEST = "SW"
   WEST_SOUTHWEST = "WSW"
   WEST = "W"
   WEST_NORTHWEST = "WNW"
   NORTHWEST = "NW"
   NORTH_NORTHWEST = "NNW"
   
-  def _new(value: str, degrees: float) -> Self:
+  def _new(value: str, degrees: float):
     enum = WindDirection(value)
     enum.__degrees = degrees
     
     return enum
   
   def __repr__(self) -> str:
     """:class:`str`: The string representation of this object."""
@@ -273,15 +273,15 @@
   HEAVY_RAIN = 302
   LIGHT_SNOW_SHOWERS = 323
   HEAVY_SNOW_SHOWERS = 335
   THUNDERY_HEAVY_RAIN = 389
   THUNDERY_SNOW_SHOWERS = 392
   
   @classmethod
-  def _missing_(self, value: int) -> Self:
+  def _missing_(self, value: int):
     if value == 248 or value == 260:
       return self.FOG
     elif value == 263 or value == 353:
       return self.LIGHT_SHOWERS
     elif value == 362 or value == 365 or value == 374:
       return self.LIGHT_SLEET_SHOWERS
     elif value == 185 or value == 281 or value == 284 or value == 311 or value == 314 or value == 317 or value == 350 or value == 377:
```

### Comparing `python-weather-1.0.0/python_weather/errors.py` & `python-weather-1.0.1/python_weather/errors.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.0/python_weather/forecast.py` & `python-weather-1.0.1/python_weather/forecast.py`

 * *Files identical despite different names*

### Comparing `python-weather-1.0.0/python_weather.egg-info/PKG-INFO` & `python-weather-1.0.1/python_weather.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: python-weather
-Version: 1.0.0
+Version: 1.0.1
 Summary: A free and asynchronous weather API wrapper made in Python, for Python.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/python-weather
-Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.0.tar.gz
+Project-URL: download_url, https://github.com/null8626/python-weather/archive/1.0.1.tar.gz
 Keywords: weather,forecast,weather-api,weather-forecast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

