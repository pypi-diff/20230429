# Comparing `tmp/k8s_audit_filter-0.4.0-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22770 bytes, number of entries: 14
+Zip file size: 22947 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 k8s_audit_filter/__about__.py
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
 -rw-r--r--  2.0 unx     1141 b- defN 20-Feb-02 00:00 k8s_audit_filter/abstract_classes.py
 -rw-r--r--  2.0 unx     4417 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_data.py
--rw-r--r--  2.0 unx     3363 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
--rw-r--r--  2.0 unx     1079 b- defN 20-Feb-02 00:00 k8s_audit_filter/count_rules.py
--rw-r--r--  2.0 unx     2365 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
--rw-r--r--  2.0 unx     2176 b- defN 20-Feb-02 00:00 k8s_audit_filter/resourses_field.py
+-rw-r--r--  2.0 unx     3673 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
+-rw-r--r--  2.0 unx     1234 b- defN 20-Feb-02 00:00 k8s_audit_filter/count_rules.py
+-rw-r--r--  2.0 unx     2754 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
+-rw-r--r--  2.0 unx     2156 b- defN 20-Feb-02 00:00 k8s_audit_filter/resourses_field.py
 -rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
 -rw-r--r--  2.0 unx     2751 b- defN 20-Feb-02 00:00 k8s_audit_filter/utils.py
-?rw-r--r--  2.0 unx     5861 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1203 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/RECORD
-14 files, 60848 bytes uncompressed, 20756 bytes compressed:  65.9%
+?rw-r--r--  2.0 unx     5861 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.5.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.5.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.5.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1203 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.5.0.dist-info/RECORD
+14 files, 61682 bytes uncompressed, 20933 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
 Filename: k8s_audit_filter/utils.py
 Comment: 
 
-Filename: k8s_audit_filter-0.4.0.dist-info/METADATA
+Filename: k8s_audit_filter-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.4.0.dist-info/WHEEL
+Filename: k8s_audit_filter-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.5.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.4.0.dist-info/RECORD
+Filename: k8s_audit_filter-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.4.0"
+__version__ = "0.5.0"
```

## k8s_audit_filter/audit_filter.py

```diff
@@ -1,12 +1,13 @@
 import logging
+from copy import deepcopy
 
 import yaml
 
-from .rules import RuleFactory
+from k8s_audit_filter.rules import RuleFactory
 
 from typing import Any, List, Union  # noqa isort:skip
 
 
 from .abstract_classes import Factory, Rule  # noqa isort:skip
 
 logger = logging.getLogger(__name__)
@@ -30,19 +31,19 @@
         if not self.rules:
             return True  # no rules, no filter
         for rule in self.rules:
             try:
                 if rule.check_rule(log_line):
                     return True
             except Exception as e:
-                logger.error(
+                logger.warning(
                     f"Exception: {e}, Type: {e.__class__.__qualname__} "
                     f"Traceback: {e.__traceback__} Rule: {rule} with log line: {log_line}"
                 )
-                return True  # if rule check fails, we assume it should not be filtered
+                raise e  # if rule check fails, we assume it should not be filtered
         return False
 
     def add_rule(self, rule: dict):
         internal_rule = RuleFactory.create(rule)
         self.rules.append(internal_rule)
         self.config["rules"].append(internal_rule.as_dict)  # type: ignore
 
@@ -55,17 +56,22 @@
         self.rules.remove(internal_rule)
         self.config["rules"].remove(internal_rule.as_dict)  # type: ignore
 
     def remove_rules(self, rules: list):
         for rule in rules:
             self.remove_rule(rule)
 
-    def dump_config(self, path_to_config):
+    def dump_config(self, path_to_config, k8s_standard: bool = True):
+        config = deepcopy(self.config)
+        if k8s_standard:
+            for rule in config["rules"]:
+                if "codes" in rule:  # there is no codes field in k8s standard
+                    del rule["codes"]  # type: ignore
         with open(path_to_config, "w") as f:
-            yaml.dump(self.config, f)
+            yaml.dump(config, f, indent=4)
 
     @staticmethod
     def filter_with_rule(log_line: dict, rule: dict) -> bool:
         internal_rule: Rule = RuleFactory.create(rule)
         return internal_rule.check_rule(log_line)
```

## k8s_audit_filter/count_rules.py

```diff
@@ -26,19 +26,25 @@
 
 
 class GroupCountRule(CountRule):
     def get(self, instance: dict):
         return instance["user"]["groups"]
 
 
+class CodesCountRule(CountRule):
+    def get(self, instance: dict):
+        return [instance["responseStatus"]["code"]]
+
+
 class CountRuleFactory(Factory):
     mapping = {
         "level": LevelCountRule,
         "users": UserCountRule,
         "groups": GroupCountRule,
+        "codes": CodesCountRule,
     }
 
     @classmethod
     def create(cls, entity: str) -> CountRule:
         if entity not in cls.mapping:
             raise CountRuleException(
                 f"Invalid count rule. Unknown key {entity}. Must be one of {list(cls.mapping.keys())}"
```

## k8s_audit_filter/fields.py

```diff
@@ -60,22 +60,35 @@
     def check_match(self, target: dict) -> bool:
         for space in self.value:
             if target.get("objectRef") and target["objectRef"].get("namespace") == space:
                 return True
         return False
 
 
+class CodesField(Field):
+    def __init__(self, value: List[str]):
+        self.name = "codes"
+        self.value: List[str] = value
+
+    def check_match(self, target: dict) -> bool:
+        for code in self.value:
+            if target.get("responseStatus") and target["responseStatus"].get("code") == code:
+                return True
+        return False
+
+
 class FieldFactory(Factory):
     mapping = {
         "level": LevelField,
         "verbs": VerbsField,
         "users": UsersField,
         "userGroups": UserGroupsField,
         "namespaces": NamespacesField,
         "resources": ResourceField,
+        "codes": CodesField,
     }
 
     @classmethod
     def create(cls, entity: dict):
         result = []
         for key, vale in entity.items():
             if key in cls.mapping:
```

## k8s_audit_filter/resourses_field.py

```diff
@@ -7,39 +7,39 @@
     def __init__(self, value: str):
         self.name = "group"
         self.value: str = value
 
     def check_match(self, target: dict) -> bool:
         if not self.value:
             return True
-        if target["objectRef"].get("apiGroup") and target["objectRef"]["apiGroup"] == self.value:
+        if target.get("objectRef") and target["objectRef"].get("apiGroup") == self.value:
             return True
         return False
 
 
 class ResourceResourceSubField(Field):
     def __init__(self, value: List[str]):
         self.name = "resources"
         self.value: List[str] = value
 
     def check_match(self, target: dict) -> bool:
         for resource in self.value:
-            if target["objectRef"].get("resource") and target["objectRef"]["resource"] == resource:
+            if target.get("objectRef") and target["objectRef"].get("resource") == resource:
                 return True
         return False
 
 
 class ResourceNamesSubField(Field):
     def __init__(self, value: List[str]):
         self.name = "resourceNames"
         self.value: List[str] = value
 
     def check_match(self, target: dict) -> bool:
         for name in self.value:
-            if target["objectRef"].get("name") and target["objectRef"]["name"] == name:
+            if target.get("objectRef") and target["objectRef"].get("name") == name:
                 return True
         return False
 
 
 class ResourcesFieldsFactory(Factory):
     mapping = {
         "group": ResourceGroupSubField,
```

## Comparing `k8s_audit_filter-0.4.0.dist-info/METADATA` & `k8s_audit_filter-0.5.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.4.0
+Version: 0.5.0
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

## Comparing `k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.5.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `k8s_audit_filter-0.4.0.dist-info/RECORD` & `k8s_audit_filter-0.5.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-k8s_audit_filter/__about__.py,sha256=42STGor_9nKYXumfeV5tiyD_M8VdcddX7CEexmibPBk,22
+k8s_audit_filter/__about__.py,sha256=LBK46heutvn3KmsCrKIYu8RQikbfnjZaj2xFrXaeCzQ,22
 k8s_audit_filter/__init__.py,sha256=Ygyj50ubIBSq7rPmZA5toFWotAC4D3Mc6DzCq_07s2k,81
 k8s_audit_filter/abstract_classes.py,sha256=ilUK_T9Y1_pDxTdLpeOtDKnwHdj7fxPAhTKyhaLN8JI,1141
 k8s_audit_filter/audit_data.py,sha256=E50NSdbVB2uR6mtJP9AeteSx1A0Cmr4fOF50DazKZLo,4417
-k8s_audit_filter/audit_filter.py,sha256=cAKm8M2S29LRWe6Ndkmbh-FznLxMW7jwREG7Q14paUQ,3363
-k8s_audit_filter/count_rules.py,sha256=ZOJvjAaLY8XT5GIQrHCXjy8ZHt91fTcj5GmtS4xai5I,1079
-k8s_audit_filter/fields.py,sha256=lLR0F5cMMwSajYBidNGA1OtlpuhZQQ_0GniS0UlVj3Y,2365
-k8s_audit_filter/resourses_field.py,sha256=PekC5VuOJIlHB5ur2NlqNDbY4VpVATjUM8v85ul7FNs,2176
+k8s_audit_filter/audit_filter.py,sha256=SvykM8eXG8IQXXXglu_pEDhIYT8tTATPTNDHHygL-io,3673
+k8s_audit_filter/count_rules.py,sha256=i_77Kb4GzbSG4EQ05oisdE26yBZNAvz0_bB1_PEWQoM,1234
+k8s_audit_filter/fields.py,sha256=FuNLoHvGnXE_GMenKnAjO_eG3ChQuIW0EakNZIBg8y4,2754
+k8s_audit_filter/resourses_field.py,sha256=bFg1HwDZMAzqfq60HtUAdNmCKBL0OzMvomReG7HNtSE,2156
 k8s_audit_filter/rules.py,sha256=vuXE1etcQpnkhHUwcAIEw0Xf4GnSHecZWaZ8QPB-prY,1153
 k8s_audit_filter/utils.py,sha256=B9Md57gPehM0XqLY1w7sDG8BbwmP33esszUW4djeSko,2751
-k8s_audit_filter-0.4.0.dist-info/METADATA,sha256=2MJm38EWB135xtxpry7rfWBnjiBb63NKSgBjWGBJ7FE,5861
-k8s_audit_filter-0.4.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-k8s_audit_filter-0.4.0.dist-info/RECORD,,
+k8s_audit_filter-0.5.0.dist-info/METADATA,sha256=qayZKXB3BqObF_AG3jdIhXLwmHmGikAjb7sJQIKgYx4,5861
+k8s_audit_filter-0.5.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+k8s_audit_filter-0.5.0.dist-info/licenses/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+k8s_audit_filter-0.5.0.dist-info/RECORD,,
```

