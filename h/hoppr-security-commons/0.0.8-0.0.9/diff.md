# Comparing `tmp/hoppr_security_commons-0.0.8.tar.gz` & `tmp/hoppr_security_commons-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoppr_security_commons-0.0.8.tar", max compression
+gzip compressed data, was "hoppr_security_commons-0.0.9.tar", max compression
```

## Comparing `hoppr_security_commons-0.0.8.tar` & `hoppr_security_commons-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1084 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/LICENSE.md
--rw-r--r--   0        0        0      615 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       56 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/__init__.py
--rw-r--r--   0        0        0     1100 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/README.md
--rw-r--r--   0        0        0        0 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/__init__.py
--rw-r--r--   0        0        0        0 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/__init__.py
--rw-r--r--   0        0        0      814 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/models.py
--rw-r--r--   0        0        0    12481 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/reporting.py
--rw-r--r--   0        0        0    13776 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/assets/vulnerabilities.css
--rw-r--r--   0        0        0    50446 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/package-lock.json
--rw-r--r--   0        0        0       56 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/package.json
--rw-r--r--   0        0        0      135 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/tailwind.config.js
--rw-r--r--   0        0        0     3241 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/vulnerabilities.html
--rw-r--r--   0        0        0       58 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/vulnerability.css
--rw-r--r--   0        0        0    10820 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/vulnerability_details.html
--rw-r--r--   0        0        0     7260 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/utils.py
--rw-r--r--   0        0        0     5438 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/vulnerability_combiner.py
--rw-r--r--   0        0        0     3688 2023-01-26 00:09:00.000000 hoppr_security_commons-0.0.8/security_commons/common/vulnerability_scanner.py
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.8/setup.py
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0      615 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/__init__.py
+-rw-r--r--   0        0        0     1100 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/__init__.py
+-rw-r--r--   0        0        0      814 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/models.py
+-rw-r--r--   0        0        0    12906 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/reporting.py
+-rw-r--r--   0        0        0    13776 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/assets/vulnerabilities.css
+-rw-r--r--   0        0        0    50446 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/package-lock.json
+-rw-r--r--   0        0        0       56 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/package.json
+-rw-r--r--   0        0        0      135 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/tailwind.config.js
+-rw-r--r--   0        0        0     3241 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerabilities.html
+-rw-r--r--   0        0        0       58 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerability.css
+-rw-r--r--   0        0        0    10820 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerability_details.html
+-rw-r--r--   0        0        0     7260 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/utils.py
+-rw-r--r--   0        0        0     5438 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/vulnerability_combiner.py
+-rw-r--r--   0        0        0     3688 2023-02-06 16:11:42.000000 hoppr_security_commons-0.0.9/security_commons/common/vulnerability_scanner.py
+-rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.9/setup.py
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 hoppr_security_commons-0.0.9/PKG-INFO
```

### Comparing `hoppr_security_commons-0.0.8/LICENSE.md` & `hoppr_security_commons-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/pyproject.toml` & `hoppr_security_commons-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hoppr-security-commons"
-version = "0.0.8"
+version = "0.0.9"
 description = "Common Library For hoppr-cop"
 authors = ["kganger <keith.e.ganger@lmco.com>"]
 license = "MIT"
 
 packages = [
     { include = "security_commons" },
 ]
```

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/README.md` & `hoppr_security_commons-0.0.9/security_commons/common/README.md`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/reporting/models.py` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/models.py`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/reporting/reporting.py` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/reporting.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # Copyright (c) 2022 Lockheed Martin CorporationØ
 import json
 import pkgutil
+import uuid
 from collections import defaultdict
 from pathlib import Path
 from typing import List, Optional
 
 import jinja2
 import typer
 from hoppr_cyclonedx_models.cyclonedx_1_4 import (
@@ -86,34 +87,43 @@
             bom.vulnerabilities = bom.vulnerabilities + vulnerabilities
         else:
             typer.echo(
                 "Cannot add vulnerabilities to a bom earlier than cyclone version 1.4"
             )
         return bom
 
+    @staticmethod
+    def link_vulnerabilities_to_bom(vulnerabilities: List[Vulnerability]) -> Bom_1_4:
+        """Creates/Adds the vulnerabilities found by various scanners to cyclone 1.4+ compliant VEX BOM"""
+        vex_bom = Bom_1_4(bomFormat="CycloneDX", specVersion="1.4", version=1)
+        vex_bom.serialNumber = f"urn:uuid:{uuid.uuid4()}"
+        vex_bom.vulnerabilties = vulnerabilities
+
+        return vex_bom
+
     def __add_purl_as_bom_ref_and_flatten(
         self, vulnerabilities: dict[str, Optional[list[Vulnerability]]]
     ) -> List[Vulnerability]:
         flattened_vulnerabilities: List[Vulnerability] = []
 
         for purl in vulnerabilities:
             for vuln in vulnerabilities[purl]:
                 vuln.affects = [] if vuln.affects is None else vuln.affects
                 vuln.affects.append(Affect(**{"ref": purl}))
                 flattened_vulnerabilities.append(vuln)
 
-        def get_score(vuln_to_score: Vulnerability) -> float:
-            best_rating = self.__get_best_rating(vuln_to_score.ratings)
-            if best_rating is None or best_rating.score is None:
-                return 0.0
-            return best_rating.score
-
-        flattened_vulnerabilities.sort(key=get_score, reverse=True)
+        flattened_vulnerabilities.sort(key=self.get_score, reverse=True)
         return flattened_vulnerabilities
 
+    def get_score(self, vuln_to_score: Vulnerability) -> float:
+        best_rating = self.__get_best_rating(vuln_to_score.ratings)
+        if best_rating is None or best_rating.score is None:
+            return 0.0
+        return best_rating.score
+
     def __get_fields_from_vulnerabilities(self, vulnerabilities: List[Vulnerability]):
         findings = []
 
         def get_fields(vuln: Vulnerability) -> List:
             tools = [] if vuln.tools is None else vuln.tools
             tools = list(map(lambda x: f"{x.vendor} {x.name}", tools))
             severity = self.__get_severity(vuln.ratings)
```

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/assets/vulnerabilities.css` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/assets/vulnerabilities.css`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/package-lock.json` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/package-lock.json`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/vulnerabilities.html` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerabilities.html`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/reporting/templates/vulnerability_details.html` & `hoppr_security_commons-0.0.9/security_commons/common/reporting/templates/vulnerability_details.html`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/utils.py` & `hoppr_security_commons-0.0.9/security_commons/common/utils.py`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/vulnerability_combiner.py` & `hoppr_security_commons-0.0.9/security_commons/common/vulnerability_combiner.py`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/security_commons/common/vulnerability_scanner.py` & `hoppr_security_commons-0.0.9/security_commons/common/vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `hoppr_security_commons-0.0.8/setup.py` & `hoppr_security_commons-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'rich>=12.5.1,<13.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'tinydb>=4.7.0,<5.0.0',
  'typer>=0.7.0,<0.8.0']
 
 setup_kwargs = {
     'name': 'hoppr-security-commons',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Common Library For hoppr-cop',
     'long_description': 'None',
     'author': 'kganger',
     'author_email': 'keith.e.ganger@lmco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hoppr_security_commons-0.0.8/PKG-INFO` & `hoppr_security_commons-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hoppr-security-commons
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common Library For hoppr-cop
 License: MIT
 Author: kganger
 Author-email: keith.e.ganger@lmco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

