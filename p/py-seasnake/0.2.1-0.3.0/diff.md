# Comparing `tmp/py_seasnake-0.2.1.tar.gz` & `tmp/py_seasnake-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_seasnake-0.2.1.tar", max compression
+gzip compressed data, was "py_seasnake-0.3.0.tar", max compression
```

## Comparing `py_seasnake-0.2.1.tar` & `py_seasnake-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1070 2023-04-21 21:00:11.124489 py_seasnake-0.2.1/LICENSE
--rw-r--r--   0        0        0      745 2023-04-24 00:19:44.535505 py_seasnake-0.2.1/README.md
--rw-r--r--   0        0        0     1281 2023-04-24 04:21:04.129917 py_seasnake-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       87 2023-04-24 03:53:16.507223 py_seasnake-0.2.1/seasnake/__init__.py
--rw-r--r--   0        0        0     3841 2023-04-24 04:19:17.435833 py_seasnake-0.2.1/seasnake/auth.py
--rw-r--r--   0        0        0     3737 2023-04-23 23:24:46.487674 py_seasnake-0.2.1/seasnake/base.py
--rw-r--r--   0        0        0     2799 2023-04-24 00:35:16.376053 py_seasnake-0.2.1/seasnake/projects.py
--rw-r--r--   0        0        0      386 2023-04-20 15:10:20.566010 py_seasnake-0.2.1/seasnake/summaries/__init__.py
--rw-r--r--   0        0        0     2686 2023-04-24 02:28:36.470201 py_seasnake-0.2.1/seasnake/summaries/benthic_lit.py
--rw-r--r--   0        0        0     2800 2023-04-24 02:29:09.113535 py_seasnake-0.2.1/seasnake/summaries/benthic_photo_quadrat.py
--rw-r--r--   0        0        0     2679 2023-04-24 02:29:37.511042 py_seasnake-0.2.1/seasnake/summaries/benthic_pit.py
--rw-r--r--   0        0        0     3518 2023-04-24 02:30:11.893367 py_seasnake-0.2.1/seasnake/summaries/bleaching.py
--rw-r--r--   0        0        0     2467 2023-04-24 02:30:40.146808 py_seasnake-0.2.1/seasnake/summaries/fish_belt.py
--rw-r--r--   0        0        0     2770 2023-04-24 02:31:04.924193 py_seasnake-0.2.1/seasnake/summaries/habitat_complexity.py
--rw-r--r--   0        0        0     2360 2023-04-24 02:31:07.718517 py_seasnake-0.2.1/seasnake/summaries/sample_event.py
--rw-r--r--   0        0        0     1802 1970-01-01 00:00:00.000000 py_seasnake-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-29 21:40:45.713848 py_seasnake-0.3.0/LICENSE
+-rw-r--r--   0        0        0      745 2023-04-29 21:40:45.713848 py_seasnake-0.3.0/README.md
+-rw-r--r--   0        0        0     1311 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/__init__.py
+-rw-r--r--   0        0        0     3840 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/auth.py
+-rw-r--r--   0        0        0     9230 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/base.py
+-rw-r--r--   0        0        0     1445 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/io.py
+-rw-r--r--   0        0        0     2775 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/projects.py
+-rw-r--r--   0        0        0      386 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/__init__.py
+-rw-r--r--   0        0        0     3114 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/base.py
+-rw-r--r--   0        0        0     2853 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/benthic_lit.py
+-rw-r--r--   0        0        0     2979 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/benthic_photo_quadrat.py
+-rw-r--r--   0        0        0     2854 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/benthic_pit.py
+-rw-r--r--   0        0        0     3741 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/bleaching.py
+-rw-r--r--   0        0        0     2654 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/fish_belt.py
+-rw-r--r--   0        0        0     2957 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/habitat_complexity.py
+-rw-r--r--   0        0        0     2356 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/summaries/sample_event.py
+-rw-r--r--   0        0        0      606 2023-04-29 21:40:45.717848 py_seasnake-0.3.0/seasnake/timer.py
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 py_seasnake-0.3.0/PKG-INFO
```

### Comparing `py_seasnake-0.2.1/LICENSE` & `py_seasnake-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.2.1/README.md` & `py_seasnake-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `py_seasnake-0.2.1/pyproject.toml` & `py_seasnake-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "py-seasnake"
 packages = [
     { include = "seasnake" },
 ]
-version = "0.2.1"
+version = "0.3.0"
 description = "A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease."
 authors = ["Dustin Sampson <gridcell@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gridcell.github.io/py-seasnake/"
 repository = "https://github.com/gridcell/py-seasnake"
 documentation = "https://gridcell.github.io/py-seasnake/"
 keywords = ["MERMAID", "coral", "fish", "API"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-pandas = "^2.0.0"
 PyJWT = "^2.6.0"
 mkdocs-material = "^9.1.6"
 mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 requests = "^2.28.2"
+geopandas = "^0.12.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 black = "^23.3.0"
 isort = "^5.12.0"
 ruff = "^0.0.261"
 mypy = "^1.2.0"
 pytest-mypy = "^0.10.3"
 pandas-stubs = "^1.5.3"
 mkdocs = "^1.4.2"
 pytest-ruff = "^0.0.5"
 types-requests = "^2.28.11.17"
+requests-mock = "^1.10.0"
 
 [tool.poetry.group.examples.dependencies]
 jupyterlab = "^3.6.3"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py_seasnake-0.2.1/seasnake/auth.py` & `py_seasnake-0.3.0/seasnake/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import datetime
+import time
 import webbrowser
 from typing import Optional
-import requests
-import time
 
 import jwt
-
+import requests
 
 AUTH0_DOMAIN = "datamermaid.auth0.com"
 RESPONSE_TYPE = "token"
 SCOPE = "openid,profile,email"
 CLIENT_ID = "gFlPNhqS1h8QR3THF8R9fVePQudzGcKD"
 AUDIENCE = "https://api.datamermaid.org"
```

### Comparing `py_seasnake-0.2.1/seasnake/projects.py` & `py_seasnake-0.3.0/seasnake/projects.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,19 @@
         """
         Get a list of your projects.
 
         This method retrieves a list of your projects.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, Project    
-        
+        from seasnake import MermaidAuth, Project
+
         auth = MermaidAuth()
         project = Project(token=auth.get_token())
         print(project.my_projects())
         ```
         """
 
         url = "/projects/"
@@ -46,29 +46,29 @@
         include_test_projects: bool = False,
     ) -> DataFrame:
         """
         Searches all MERMAID projects and filters results based on the specified criteria.
 
         Args:
             name (Optional[str], optional): A name or list of names to search for in
-            projects. Defaults to None.
+                projects. Defaults to None.
             countries (Union[None, str, List[str]], optional): A country to search for
-            in projects. Defaults to None.
+                in projects. Defaults to None.
             tags (Union[None, str, List[str]], optional): A tag or list of tags to search
-            for in projects. Defaults to None.
+                for in projects. Defaults to None.
             include_test_projects (bool, optional): Whether to include test projects in
-            the search results. Defaults to False.
+                the search results. Defaults to False.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import Project    
-        
+        from seasnake import Project
+
         project = Project()
         print(project.search_projects(tags=["WCS Fiji""]))
         ```
         """
 
         url = "/projects/"
```

### Comparing `py_seasnake-0.2.1/seasnake/summaries/benthic_lit.py` & `py_seasnake-0.3.0/seasnake/summaries/benthic_pit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,86 +1,87 @@
-from ..base import DataFrame, MermaidBase, requires_token
+from .base import BaseSummary, DataFrame, requires_token
 
 
-class BenthicLIT(MermaidBase):
+class BenthicPIT(BaseSummary):
     """
-    A class for handling Benthic Line Intercept Transect (LIT) data from MERMAID.
+    A class for handling Benthic Point Intercept Transect (PIT) data from MERMAID.
 
-    The BenthicLIT class is responsible for fetching Benthic LIT data, including observations,
+    The BenthicPIT class is responsible for fetching Benthic PIT data, including observations,
     observations aggregated by sample units, and observations aggregated by sample events,
     for a specified project.
     """
 
     @requires_token
     def observations(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic LIT observations.
+        Retrieves a project's Benthic PIT observations.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic LIT observations.
+            project_id (str): The ID of the project for which to fetch Benthic PIT observations.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, BenthicLIT    
-        
+        from seasnake import MermaidAuth, BenthicPIT
+
         auth = MermaidAuth()
-        benthic_lit = BenthicLIT(token=auth.get_token())
+        benthic_pit = BenthicPIT(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
-        print(benthic_lit.observations(project_id))
+        print(benthic_pit.sample_events(project_id))
         ```
         """
-
-        url = f"/projects/{project_id}/benthiclits/obstransectbenthiclits/"
-        return self.data_frame_from_url(url)
+        url = f"/projects/{project_id}/benthicpits/obstransectbenthicpits/"
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic LIT observations aggregated by sample units.
+        Retrieves a project's Benthic PIT observations aggregated by sample units.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic LIT sample units.
+            project_id (str): The ID of the project for which to fetch Benthic PIT sample units.
 
         Returns:
             DataFrame
-        
         Examples:
         ```
-        from seasnake import MermaidAuth, BenthicLIT    
-        
+        from seasnake import MermaidAuth, BenthicPIT
+
         auth = MermaidAuth()
-        benthic_lit = BenthicLIT(token=auth.get_token())
+        benthic_pit = BenthicPIT(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
-        print(benthic_lit.sample_units(project_id))
+        print(benthic_pit.sample_events(project_id))
         ```
         """
 
-        url = f"/projects/{project_id}/benthiclits/sampleunits/"
-        return self.data_frame_from_url(url)
+        url = f"/projects/{project_id}/benthicpits/sampleunits/"
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic LIT observations aggregated by sample events.
+        Retrieves a project's Benthic PIT observations aggregated by sample events.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic LIT sample events.
+            project_id (str): The ID of the project for which to fetch Benthic PIT sample events.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, BenthicLIT    
-        
+        from seasnake import MermaidAuth, BenthicPIT
+
         auth = MermaidAuth()
-        benthic_lit = BenthicLIT(token=auth.get_token())
+        benthic_pit = BenthicPIT(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
-        print(benthic_lit.sample_events(project_id))
+        print(benthic_pit.sample_events(project_id))
         ```
         """
 
-        url = f"/projects/{project_id}/benthiclits/sampleevents/"
-        return self.data_frame_from_url(url)
+        url = f"/projects/{project_id}/benthicpits/sampleevents/"
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
```

### Comparing `py_seasnake-0.2.1/seasnake/summaries/benthic_pit.py` & `py_seasnake-0.3.0/seasnake/summaries/benthic_lit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,89 @@
-from ..base import DataFrame, MermaidBase, requires_token
+from .base import BaseSummary, DataFrame, requires_token
 
 
-class BenthicPIT(MermaidBase):
+class BenthicLIT(BaseSummary):
     """
-    A class for handling Benthic Point Intercept Transect (PIT) data from MERMAID.
+    A class for handling Benthic Line Intercept Transect (LIT) data from MERMAID.
 
-    The BenthicPIT class is responsible for fetching Benthic PIT data, including observations,
+    The BenthicLIT class is responsible for fetching Benthic LIT data, including observations,
     observations aggregated by sample units, and observations aggregated by sample events,
     for a specified project.
     """
 
     @requires_token
     def observations(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic PIT observations.
+        Retrieves a project's Benthic LIT observations.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic PIT observations.
+            project_id (str): The ID of the project for which to fetch Benthic LIT observations.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, BenthicPIT    
-        
+        from seasnake import MermaidAuth, BenthicLIT
+
         auth = MermaidAuth()
-        benthic_pit = BenthicPIT(token=auth.get_token())
+        benthic_lit = BenthicLIT(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
-        print(benthic_pit.sample_events(project_id))
+        print(benthic_lit.observations(project_id))
         ```
         """
-        url = f"/projects/{project_id}/benthicpits/obstransectbenthicpits/"
-        return self.data_frame_from_url(url)
+
+        url = f"/projects/{project_id}/benthiclits/obstransectbenthiclits/"
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic PIT observations aggregated by sample units.
+        Retrieves a project's Benthic LIT observations aggregated by sample units.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic PIT sample units.
+            project_id (str): The ID of the project for which to fetch Benthic LIT sample units.
 
         Returns:
             DataFrame
+
         Examples:
         ```
-        from seasnake import MermaidAuth, BenthicPIT    
-        
+        from seasnake import MermaidAuth, BenthicLIT
+
         auth = MermaidAuth()
-        benthic_pit = BenthicPIT(token=auth.get_token())
+        benthic_lit = BenthicLIT(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
-        print(benthic_pit.sample_events(project_id))
+        print(benthic_lit.sample_units(project_id))
         ```
         """
 
-        url = f"/projects/{project_id}/benthicpits/sampleunits/"
-        return self.data_frame_from_url(url)
+        url = f"/projects/{project_id}/benthiclits/sampleunits/"
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
-        Retrieves a project's Benthic PIT observations aggregated by sample events.
+        Retrieves a project's Benthic LIT observations aggregated by sample events.
 
         Args:
-            project_id (str): The ID of the project for which to fetch Benthic PIT sample events.
+            project_id (str): The ID of the project for which to fetch Benthic LIT sample events.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, BenthicPIT    
-        
+        from seasnake import MermaidAuth, BenthicLIT
+
         auth = MermaidAuth()
-        benthic_pit = BenthicPIT(token=auth.get_token())
+        benthic_lit = BenthicLIT(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
-        print(benthic_pit.sample_events(project_id))
+        print(benthic_lit.sample_events(project_id))
         ```
         """
 
-        url = f"/projects/{project_id}/benthicpits/sampleevents/"
-        return self.data_frame_from_url(url)
+        url = f"/projects/{project_id}/benthiclits/sampleevents/"
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
```

### Comparing `py_seasnake-0.2.1/seasnake/summaries/bleaching.py` & `py_seasnake-0.3.0/seasnake/summaries/bleaching.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ..base import DataFrame, MermaidBase, requires_token
+from .base import BaseSummary, DataFrame, requires_token
 
 
-class Bleaching(MermaidBase):
+class Bleaching(BaseSummary):
     """
     A class for handling coral bleaching data from MERMAID.
 
     The Bleaching class is responsible for fetching bleaching data, including observations,
     observations aggregated by sample units, and observations aggregated by sample events,
     for a specified project.
     """
@@ -16,97 +16,101 @@
         Retrieves a project's Bleaching colonies bleached observations.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching observations.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, Bleaching    
-        
+        from seasnake import MermaidAuth, Bleaching
+
         auth = MermaidAuth()
         bleaching = Bleaching(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(bleaching.colonies_bleached_observations(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/bleachingqcs/obscoloniesbleacheds/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def percent_cover_observations(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Bleaching percent cover of hard coral, macroalgae and
         soft coral observations.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching observations.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, Bleaching    
-        
+        from seasnake import MermaidAuth, Bleaching
+
         auth = MermaidAuth()
         bleaching = Bleaching(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(bleaching.percent_cover_observations(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/bleachingqcs/obsquadratbenthicpercents/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Bleaching observations aggregated by sample units.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching sample units.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, Bleaching    
-        
+        from seasnake import MermaidAuth, Bleaching
+
         auth = MermaidAuth()
         bleaching = Bleaching(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(bleaching.sample_units(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/bleachingqcs/sampleunits/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Bleaching observations aggregated by sample events.
 
         Args:
             project_id (str): The ID of the project for which to fetch Bleaching sample events.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, Bleaching    
-        
+        from seasnake import MermaidAuth, Bleaching
+
         auth = MermaidAuth()
         bleaching = Bleaching(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(bleaching.sample_events(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/bleachingqcs/sampleevents/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
```

### Comparing `py_seasnake-0.2.1/seasnake/summaries/fish_belt.py` & `py_seasnake-0.3.0/seasnake/summaries/fish_belt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,81 +1,84 @@
-from ..base import DataFrame, MermaidBase, requires_token
+from .base import BaseSummary, DataFrame, requires_token
 
 
-class FishBeltTransect(MermaidBase):
+class FishBeltTransect(BaseSummary):
     @requires_token
     def observations(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Fish Belt Transect observations.
 
         Args:
             project_id (str): The ID of the project for which to fetch
-            Fish Belt Transect observations.
+                Fish Belt Transect observations.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, FishBeltTransect    
-        
+        from seasnake import MermaidAuth, FishBeltTransect
+
         auth = MermaidAuth()
         fish_belt = FishBeltTransect(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(fish_belt.observations(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/beltfishes/obstransectbeltfishes/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Fish Belt Transect observations aggregated by sample units.
 
         Args:
             project_id (str): The ID of the project for which to fetch
-            Fish Belt Transect sample units.
+                Fish Belt Transect sample units.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, FishBeltTransect    
-        
+        from seasnake import MermaidAuth, FishBeltTransect
+
         auth = MermaidAuth()
         fish_belt = FishBeltTransect(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(fish_belt.sample_units(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/beltfishes/sampleunits/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's Fish Belt Transect observations aggregated by sample events.
 
         Args:
             project_id (str): The ID of the project for which to fetch
-            Fish Belt Transect sample events.
+                Fish Belt Transect sample events.
 
         Returns:
             DataFrame
 
         Examples:
         ```
-        from seasnake import MermaidAuth, FishBeltTransect    
-        
+        from seasnake import MermaidAuth, FishBeltTransect
+
         auth = MermaidAuth()
         fish_belt = FishBeltTransect(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(fish_belt.sample_events(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/beltfishes/sampleevents/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
```

### Comparing `py_seasnake-0.2.1/seasnake/summaries/habitat_complexity.py` & `py_seasnake-0.3.0/seasnake/summaries/habitat_complexity.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ..base import DataFrame, MermaidBase, requires_token
+from .base import BaseSummary, DataFrame, requires_token
 
 
-class HabitatComplexity(MermaidBase):
+class HabitatComplexity(BaseSummary):
     """
     A class for handling habitat complexity data from MERMAID.
 
     The HabitatComplexity class is responsible for fetching habitat complexity
     data, including observations, observations aggregated by sample units, and
     observations aggregated by sample events, for a specified project.
     """
@@ -13,77 +13,80 @@
     @requires_token
     def observations(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's habitat complexity observations.
 
         Args:
             project_id (str): The ID of the project for which to fetch
-            habitat complexity observations.
+                habitat complexity observations.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, HabitatComplexity    
-        
+        from seasnake import MermaidAuth, HabitatComplexity
+
         auth = MermaidAuth()
         hc = HabitatComplexity(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(hc.observations(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/habitatcomplexities/obshabitatcomplexities/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_units(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's habitat complexity observations aggregated by sample units.
 
         Args:
             project_id (str): The ID of the project for which to fetch
-            habitat complexity sample units.
+                habitat complexity sample units.
 
         Returns:
             DataFrame
 
         Examples:
         ```
-        from seasnake import MermaidAuth, HabitatComplexity    
-        
+        from seasnake import MermaidAuth, HabitatComplexity
+
         auth = MermaidAuth()
         hc = HabitatComplexity(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(hc.sample_units(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/habitatcomplexities/sampleunits/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
 
     @requires_token
     def sample_events(self, project_id: str) -> DataFrame:
         """
         Retrieves a project's habitat complexity observations aggregated by sample events.
 
         Args:
             project_id (str): The ID of the project for which to fetch
-            habitat complexity sample events.
+                habitat complexity sample events.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import MermaidAuth, HabitatComplexity    
-        
+        from seasnake import MermaidAuth, HabitatComplexity
+
         auth = MermaidAuth()
         hc = HabitatComplexity(token=auth.get_token())
         project_id = "AAAAAAAA-BBBB-CCCC-DDDD-EEEEEEEEEEEE"
         print(hc.sample_events(project_id))
         ```
         """
 
         url = f"/projects/{project_id}/habitatcomplexities/sampleevents/"
-        return self.data_frame_from_url(url)
+        df = self.read_cache(url)
+        return self.to_cache(url, self.data_frame_from_url(url)) if df is None else df
```

### Comparing `py_seasnake-0.2.1/seasnake/summaries/sample_event.py` & `py_seasnake-0.3.0/seasnake/summaries/sample_event.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,24 @@
         This method retrieves summary information about Sample Events and returns the result as
         a pandas DataFrame. By default, it limits the columns included in the DataFrame and
         flattens the `protocols` (or sample methods) column. However, these behaviors can be
         changed using the input parameters.
 
         Args:
             limit_columns (bool, optional): Whether to limit the columns included
-            in the DataFrame. Defaults to True.
+                in the DataFrame. Defaults to True.
             flatten (bool, optional): Whether to flatten the 'protocols' column in
-            the DataFrame. Defaults to True.
+                the DataFrame. Defaults to True.
 
         Returns:
             DataFrame
-        
+
         Examples:
         ```
-        from seasnake import SampleEvent    
+        from seasnake import SampleEvent
 
         sample_event = SampleEvent()
         print(sample_event.summary())
         ```
         """
         columns = [
             "project",
```

### Comparing `py_seasnake-0.2.1/PKG-INFO` & `py_seasnake-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: py-seasnake
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python wrapper for accessing and managing MERMAID (Marine Ecological Research Management Aid) data with ease.
 Home-page: https://gridcell.github.io/py-seasnake/
 License: MIT
 Keywords: MERMAID,coral,fish,API
 Author: Dustin Sampson
 Author-email: gridcell@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
+Requires-Dist: geopandas (>=0.12.2,<0.13.0)
 Requires-Dist: mkdocs-material (>=9.1.6,<10.0.0)
 Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Documentation, https://gridcell.github.io/py-seasnake/
 Project-URL: Repository, https://github.com/gridcell/py-seasnake
 Description-Content-Type: text/markdown
 
 SeaSnake
 --------
```

