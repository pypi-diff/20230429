# Comparing `tmp/bmkg-1.0.3.tar.gz` & `tmp/bmkg-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmkg-1.0.3.tar", last modified: Thu Apr 27 17:09:21 2023, max compression
+gzip compressed data, was "bmkg-1.0.4.tar", last modified: Sat Apr 29 06:34:18 2023, max compression
```

## Comparing `bmkg-1.0.3.tar` & `bmkg-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 17:09:21.824301 bmkg-1.0.3/
--rw-rw-rw-   0        0        0     1066 2023-04-27 17:04:41.000000 bmkg-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      107 2023-04-27 17:04:41.000000 bmkg-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6312 2023-04-27 17:09:21.824301 bmkg-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4630 2023-04-27 17:04:41.000000 bmkg-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 17:09:21.793048 bmkg-1.0.3/bmkg/
--rw-rw-rw-   0        0        0     1479 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/base.py
--rw-rw-rw-   0        0        0     8862 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/client.py
--rw-rw-rw-   0        0        0     1431 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/constants.py
--rw-rw-rw-   0        0        0     4184 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/earthquake.py
--rw-rw-rw-   0        0        0     6098 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/enums.py
--rw-rw-rw-   0        0        0     1248 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/errors.py
--rw-rw-rw-   0        0        0     8356 2023-04-27 17:04:41.000000 bmkg-1.0.3/bmkg/forecast.py
-drwxrwxrwx   0        0        0        0 2023-04-27 17:09:21.808676 bmkg-1.0.3/bmkg.egg-info/
--rw-rw-rw-   0        0        0     6312 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 17:09:21.000000 bmkg-1.0.3/bmkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1450 2023-04-27 17:08:29.000000 bmkg-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 17:09:21.824301 bmkg-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-29 06:34:18.412115 bmkg-1.0.4/
+-rw-rw-rw-   0        0        0     1066 2023-04-27 17:04:41.000000 bmkg-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0      107 2023-04-27 17:04:41.000000 bmkg-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     6312 2023-04-29 06:34:18.396477 bmkg-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4630 2023-04-27 17:04:41.000000 bmkg-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-29 06:34:18.302725 bmkg-1.0.4/bmkg/
+-rw-rw-rw-   0        0        0     1478 2023-04-29 06:29:52.000000 bmkg-1.0.4/bmkg/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-04-29 06:09:07.000000 bmkg-1.0.4/bmkg/base.py
+-rw-rw-rw-   0        0        0     8848 2023-04-29 06:10:30.000000 bmkg-1.0.4/bmkg/client.py
+-rw-rw-rw-   0        0        0     1413 2023-04-29 06:10:48.000000 bmkg-1.0.4/bmkg/constants.py
+-rw-rw-rw-   0        0        0     4184 2023-04-29 06:09:07.000000 bmkg-1.0.4/bmkg/earthquake.py
+-rw-rw-rw-   0        0        0     6068 2023-04-29 06:10:30.000000 bmkg-1.0.4/bmkg/enums.py
+-rw-rw-rw-   0        0        0     1248 2023-04-29 06:09:07.000000 bmkg-1.0.4/bmkg/errors.py
+-rw-rw-rw-   0        0        0     8356 2023-04-29 06:09:07.000000 bmkg-1.0.4/bmkg/forecast.py
+drwxrwxrwx   0        0        0        0 2023-04-29 06:34:18.396477 bmkg-1.0.4/bmkg.egg-info/
+-rw-rw-rw-   0        0        0     6312 2023-04-29 06:34:17.000000 bmkg-1.0.4/bmkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-04-29 06:34:17.000000 bmkg-1.0.4/bmkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-29 06:34:17.000000 bmkg-1.0.4/bmkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-29 06:34:17.000000 bmkg-1.0.4/bmkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-29 06:34:17.000000 bmkg-1.0.4/bmkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1450 2023-04-29 06:05:25.000000 bmkg-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-29 06:34:18.412115 bmkg-1.0.4/setup.cfg
```

### Comparing `bmkg-1.0.3/LICENSE` & `bmkg-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.3/PKG-INFO` & `bmkg-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bmkg
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/bmkg
-Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.3.tar.gz
+Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.4.tar.gz
 Keywords: weather,forecast,indonesia,weather-api,weather-forecast,bmkg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `bmkg-1.0.3/README.md` & `bmkg-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.3/bmkg/__init__.py` & `bmkg-1.0.4/bmkg/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 SOFTWARE.
 """
 
 from .enums import AreaKind, Direction, ForecastKind, MMI, Province
 from .constants import METRIC, IMPERIAL
 from .client import Client
 
-__version__ = '1.0.3'
+__version__ = '1.0.4'
 __all__ = (
   'AreaKind', 'Client', 'Direction', 'ForecastKind', 'METRIC', 'MMI',
   'IMPERIAL', 'Province'
-)
+)
```

### Comparing `bmkg-1.0.3/bmkg/base.py` & `bmkg-1.0.4/bmkg/base.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.3/bmkg/client.py` & `bmkg-1.0.4/bmkg/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from aiohttp import ClientSession, ClientTimeout, TCPConnector
-from typing import Iterable, Optional, Self, Union
+from typing import Iterable, Optional, Union
 from xml.etree.ElementTree import fromstring
 from enum import auto
 
 from .earthquake import FeltEarthquake, LatestEarthquake, RecentEarthquake
 from .constants import METRIC, VALID_UNITS
 from .base import CustomizableUnit
 from .forecast import Weather
@@ -230,15 +230,15 @@
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

### Comparing `bmkg-1.0.3/bmkg/constants.py` & `bmkg-1.0.4/bmkg/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 from re import compile
 from enum import auto
 
-METRIC = auto('METRIC')
-IMPERIAL = auto('IMPERIAL')
+METRIC = auto()
+IMPERIAL = auto()
 
 AFFECTED_REGION_REGEX = compile(r'^([IVX]+\s*\-\s*)?([IVX]+) (.*?)$')
 PROVINCE_PREFIX_REGEX = compile(r'^d\.?(k\.?)?i\.?')
 VALID_UNITS = (METRIC, IMPERIAL)
 XML_NAMESPACES = {"xml": "http://www.w3.org/XML/1998/namespace"}
```

### Comparing `bmkg-1.0.3/bmkg/earthquake.py` & `bmkg-1.0.4/bmkg/earthquake.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.3/bmkg/enums.py` & `bmkg-1.0.4/bmkg/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-from typing import Optional, Self, Union
+from typing import Optional, Union
 
 from .base import BasicEnum
 from .constants import PROVINCE_PREFIX_REGEX
 from .errors import Error
 
 class AreaKind(BasicEnum):
   """Represents kinds of areas."""
@@ -70,15 +70,15 @@
   NORTH_SULAWESI = "SulawesiUtara"
   WEST_SUMATERA = "SumateraBarat"
   SOUTH_SUMATERA = "SumateraSelatan"
   NORTH_SUMATERA = "SumateraUtara"
   INDONESIA = "Indonesia"
   
   @classmethod
-  def _missing_(self, name: Optional[str]) -> Self:
+  def _missing_(self, name: Optional[str]):
     if name is None:
       return self.INDONESIA
     
     name = PROVINCE_PREFIX_REGEX.sub('', name.lower().lstrip()).replace(' ', '')
     
     for e in Province:
       n = e.name.lower()
@@ -182,15 +182,15 @@
   LIGHT_RAIN = "60"
   RAIN = "61"
   HEAVY_RAIN = "63"
   ISOLATED_SHOWER = "80"
   SEVERE_THUNDERSTORM = "95"
   
   @classmethod
-  def _missing_(self, name: str) -> Self:
+  def _missing_(self, name: str):
     if name == "2":
       return WeatherKind.PARTLY_CLOUDY
     elif name == "97":
       return WeatherKind.SEVERE_THUNDERSTORM
 
 class MMI(BasicEnum):
   """Represents an earthquake's MMI (Modified Mercalli Intensity) scale."""
@@ -204,12 +204,12 @@
   STRONG = "VI"
   VERY_STRONG = "VII"
   SEVERE = "VIII"
   VIOLENT = "IX"
   EXTREME = "X"
   
   @classmethod
-  def _missing_(self, value: str) -> Self:
+  def _missing_(self, value: str):
     if value == "III":
       return self.WEAK
     elif value == "XI" or value == "XII":
       return self.EXTREME
```

### Comparing `bmkg-1.0.3/bmkg/errors.py` & `bmkg-1.0.4/bmkg/errors.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.3/bmkg/forecast.py` & `bmkg-1.0.4/bmkg/forecast.py`

 * *Files identical despite different names*

### Comparing `bmkg-1.0.3/bmkg.egg-info/PKG-INFO` & `bmkg-1.0.4/bmkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: bmkg
-Version: 1.0.3
+Version: 1.0.4
 Summary: Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API.
 Author: null8626
 License: MIT
 Project-URL: repository, https://github.com/null8626/bmkg
-Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.3.tar.gz
+Project-URL: download_url, https://github.com/null8626/bmkg/archive/1.0.4.tar.gz
 Keywords: weather,forecast,indonesia,weather-api,weather-forecast,bmkg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: aiohttp
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `bmkg-1.0.3/pyproject.toml` & `bmkg-1.0.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "bmkg"
-version = "1.0.3"
+version = "1.0.4"
 description = "Unofficial Python wrapper for the BMKG (Meteorology, Climatology, and Geophysical Agency) API."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [{ name = "null8626" }]
 keywords = ["weather", "forecast", "indonesia", "weather-api", "weather-forecast", "bmkg"]
 dependencies = ["aiohttp>=3.0.0"]
 classifiers = [
@@ -34,8 +34,8 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.7"
 
 [project.urls]
 repository = "https://github.com/null8626/bmkg"
-download_url = "https://github.com/null8626/bmkg/archive/1.0.3.tar.gz"
+download_url = "https://github.com/null8626/bmkg/archive/1.0.4.tar.gz"
```

