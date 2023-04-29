# Comparing `tmp/blueskyapi-0.1.5.tar.gz` & `tmp/blueskyapi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blueskyapi-0.1.5.tar", max compression
+gzip compressed data, was "blueskyapi-0.2.0.tar", max compression
```

## Comparing `blueskyapi-0.1.5.tar` & `blueskyapi-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/LICENSE
--rw-r--r--   0        0        0      796 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/README.md
--rw-r--r--   0        0        0     1348 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       64 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/src/blueskyapi/__init__.py
--rw-r--r--   0        0        0      171 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/src/blueskyapi/__version__.py
--rw-r--r--   0        0        0     5448 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/src/blueskyapi/client.py
--rw-r--r--   0        0        0      339 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/src/blueskyapi/default_config.py
--rw-r--r--   0        0        0     1688 2023-02-02 15:00:16.437738 blueskyapi-0.1.5/src/blueskyapi/errors.py
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 blueskyapi-0.1.5/setup.py
--rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 blueskyapi-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-29 13:15:45.727007 blueskyapi-0.2.0/LICENSE
+-rw-r--r--   0        0        0      966 2023-04-29 13:15:45.727007 blueskyapi-0.2.0/README.md
+-rw-r--r--   0        0        0     1348 2023-04-29 13:15:45.731007 blueskyapi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-04-29 13:15:45.731007 blueskyapi-0.2.0/src/blueskyapi/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-29 13:15:45.731007 blueskyapi-0.2.0/src/blueskyapi/__version__.py
+-rw-r--r--   0        0        0     5792 2023-04-29 13:15:45.731007 blueskyapi-0.2.0/src/blueskyapi/client.py
+-rw-r--r--   0        0        0      339 2023-04-29 13:15:45.731007 blueskyapi-0.2.0/src/blueskyapi/default_config.py
+-rw-r--r--   0        0        0     1688 2023-04-29 13:15:45.731007 blueskyapi-0.2.0/src/blueskyapi/errors.py
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 blueskyapi-0.2.0/PKG-INFO
```

### Comparing `blueskyapi-0.1.5/LICENSE` & `blueskyapi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blueskyapi-0.1.5/pyproject.toml` & `blueskyapi-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blueskyapi"
-version = "0.1.5"
+version = "0.2.0"
 description = "Client for blueskyapi.io"
 authors = ["blueskyapi.io <contact@blueskyapi.io>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://blueskyapi.io"
 repository = "https://github.com/bluesky-api/python-client"
```

### Comparing `blueskyapi-0.1.5/src/blueskyapi/client.py` & `blueskyapi-0.2.0/src/blueskyapi/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,52 +69,57 @@
 
     def latest_forecast(
         self,
         lat: float,
         lon: float,
         forecast_distances: Iterable[int] = None,
         columns: Iterable[str] = None,
+        dataset: Optional[str] = None,
     ) -> pd.DataFrame:
         """Obtain the latest forecast.
 
         :param lat: Latitude for which to fetch the forecast.
         :param lon: Longitude for which to fetch the forecast.
         :param forecast_distances: Forecast distances to fetch data for (hours from ``forecast_moment``).
         :param columns: Which variables to fetch (see `this page for available variables <https://blueskyapi.io/docs/data>`_).
+        :param dataset: Which dataset to fetch data from (only for users on the Professional plan).
         """
         response = self._get(
             "/forecasts/latest",
             params=dict(
                 lat=lat,
                 lon=lon,
                 forecast_distances=_prepare_comma_separated_list(
                     forecast_distances, "forecast_distances"
                 ),
                 columns=_prepare_comma_separated_list(columns, "columns"),
+                dataset=dataset,
             ),
         )
         return _create_dataframe(response)
 
     def forecast_history(
         self,
         lat: float,
         lon: float,
         min_forecast_moment: Optional[Union[datetime, str]] = None,
         max_forecast_moment: Optional[Union[datetime, str]] = None,
         forecast_distances: Optional[Iterable[int]] = None,
         columns: Optional[Iterable[str]] = None,
+        dataset: Optional[str] = None,
     ) -> pd.DataFrame:
         """Obtain historical forecasts.
 
         :param lat: Latitude for which to fetch the forecasts.
         :param lon: Longitude for which to fetch the forecasts.
         :param min_forecast_moment: The first forecast moment to include.
         :param max_forecast_moment: The last forecast moment to include.
         :param forecast_distances: Forecast distances to return data for (hours from ``forecast_moment``).
         :param columns: Which variables to fetch (see `this page for available variables <https://blueskyapi.io/docs/data>`_).
+        :param dataset: Which dataset to fetch data from (only for users on the Professional plan).
         """
         response = self._get(
             "/forecasts/history",
             params=dict(
                 lat=lat,
                 lon=lon,
                 min_forecast_moment=_prepare_datetime(
@@ -123,14 +128,15 @@
                 max_forecast_moment=_prepare_datetime(
                     max_forecast_moment, "max_forecast_moment"
                 ),
                 forecast_distances=_prepare_comma_separated_list(
                     forecast_distances, "forecast_distances"
                 ),
                 columns=_prepare_comma_separated_list(columns, "columns"),
+                dataset=dataset,
             ),
         )
         return _create_dataframe(response)
 
     def _get(self, endpoint: str, params: dict = {}) -> bytes:
         url = self._url(endpoint)
         response = self.session.get(url, params=params)
```

### Comparing `blueskyapi-0.1.5/src/blueskyapi/errors.py` & `blueskyapi-0.2.0/src/blueskyapi/errors.py`

 * *Files identical despite different names*

### Comparing `blueskyapi-0.1.5/PKG-INFO` & `blueskyapi-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blueskyapi
-Version: 0.1.5
+Version: 0.2.0
 Summary: Client for blueskyapi.io
 Home-page: https://blueskyapi.io
 License: MIT
 Keywords: weather,data,api
 Author: blueskyapi.io
 Author-email: contact@blueskyapi.io
 Requires-Python: >=3.7.1,<4.0.0
@@ -18,23 +18,32 @@
 Requires-Dist: requests (>=2.0,<3.0)
 Project-URL: Documentation, https://blueskyapi.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/bluesky-api/python-client
 Description-Content-Type: text/markdown
 
 # python-client
 
-Python client for blueskyapi.io
-
 [![Tests Status](https://github.com/bluesky-api/python-client/workflows/Tests/badge.svg?branch=main&event=push)](https://github.com/bluesky-api/python-client/actions?query=workflow%3ATests+branch%3Amain+event%3Apush)
 [![Coverage Status](https://coveralls.io/repos/github/bluesky-api/python-client/badge.svg?branch=main)](https://coveralls.io/github/bluesky-api/python-client?branch=main)
 [![Stable Version](https://img.shields.io/pypi/v/blueskyapi?label=latest)](https://pypi.org/project/blueskyapi/)
 
+Python client for [blueskyapi.io](https://blueskyapi.io).
+
 ## Installation
 
-`pip install blueskyapi`
+```bash
+pip install blueskyapi
+```
+
+The package is also available on conda-forge:
+
+```bash
+conda config --add channels conda-forge
+conda install blueskyapi
+```
 
 ## Documentation
 
-This library is documented [here](https://blueskyapi.readthedocs.io/en/stable/).
+You can find the full documentation [here](https://blueskyapi.readthedocs.io/en/stable/).
 
 For available variables see the [blueskyapi.io data documentation](https://blueskyapi.io/docs/data).
```

