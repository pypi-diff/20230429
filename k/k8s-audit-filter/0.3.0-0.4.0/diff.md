# Comparing `tmp/k8s_audit_filter-0.3.0-py3-none-any.whl.zip` & `tmp/k8s_audit_filter-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,16 @@
-Zip file size: 19607 bytes, number of entries: 11
+Zip file size: 22770 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       22 b- defN 20-Feb-02 00:00 k8s_audit_filter/__about__.py
 -rw-r--r--  2.0 unx       81 b- defN 20-Feb-02 00:00 k8s_audit_filter/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 20-Feb-02 00:00 k8s_audit_filter/abstract_classes.py
--rw-r--r--  2.0 unx     2654 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
--rw-r--r--  2.0 unx     2369 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
--rw-r--r--  2.0 unx     2180 b- defN 20-Feb-02 00:00 k8s_audit_filter/resourses_field.py
+-rw-r--r--  2.0 unx     1141 b- defN 20-Feb-02 00:00 k8s_audit_filter/abstract_classes.py
+-rw-r--r--  2.0 unx     4417 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_data.py
+-rw-r--r--  2.0 unx     3363 b- defN 20-Feb-02 00:00 k8s_audit_filter/audit_filter.py
+-rw-r--r--  2.0 unx     1079 b- defN 20-Feb-02 00:00 k8s_audit_filter/count_rules.py
+-rw-r--r--  2.0 unx     2365 b- defN 20-Feb-02 00:00 k8s_audit_filter/fields.py
+-rw-r--r--  2.0 unx     2176 b- defN 20-Feb-02 00:00 k8s_audit_filter/resourses_field.py
 -rw-r--r--  2.0 unx     1153 b- defN 20-Feb-02 00:00 k8s_audit_filter/rules.py
-?rw-r--r--  2.0 unx     5861 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      946 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.3.0.dist-info/RECORD
-11 files, 51619 bytes uncompressed, 17993 bytes compressed:  65.1%
+-rw-r--r--  2.0 unx     2751 b- defN 20-Feb-02 00:00 k8s_audit_filter/utils.py
+?rw-r--r--  2.0 unx     5861 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1203 b- defN 20-Feb-02 00:00 k8s_audit_filter-0.4.0.dist-info/RECORD
+14 files, 60848 bytes uncompressed, 20756 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -3,32 +3,41 @@
 
 Filename: k8s_audit_filter/__init__.py
 Comment: 
 
 Filename: k8s_audit_filter/abstract_classes.py
 Comment: 
 
+Filename: k8s_audit_filter/audit_data.py
+Comment: 
+
 Filename: k8s_audit_filter/audit_filter.py
 Comment: 
 
+Filename: k8s_audit_filter/count_rules.py
+Comment: 
+
 Filename: k8s_audit_filter/fields.py
 Comment: 
 
 Filename: k8s_audit_filter/resourses_field.py
 Comment: 
 
 Filename: k8s_audit_filter/rules.py
 Comment: 
 
-Filename: k8s_audit_filter-0.3.0.dist-info/METADATA
+Filename: k8s_audit_filter/utils.py
+Comment: 
+
+Filename: k8s_audit_filter-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: k8s_audit_filter-0.3.0.dist-info/WHEEL
+Filename: k8s_audit_filter-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: k8s_audit_filter-0.3.0.dist-info/licenses/LICENSE
+Filename: k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: k8s_audit_filter-0.3.0.dist-info/RECORD
+Filename: k8s_audit_filter-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8s_audit_filter/__about__.py

```diff
@@ -1 +1 @@
-__version__ = "0.3.0"
+__version__ = "0.4.0"
```

## k8s_audit_filter/abstract_classes.py

```diff
@@ -1,9 +1,10 @@
 from abc import ABC
-from typing import List, Union
+
+from typing import Any, List, Union  # noqa isort:skip
 
 
 class Field(ABC):
     __slots__ = ("name", "value")
 
     def __init__(self, value: Union[str, List[str], None]):
         self.name: Union[str, None] = None
@@ -42,9 +43,9 @@
     pass
 
 
 class Factory(ABC):
     mapping: dict = {}
 
     @classmethod
-    def create(cls, entity: dict):
+    def create(cls, entity: Any):
         raise NotImplementedError
```

## k8s_audit_filter/audit_filter.py

```diff
@@ -1,43 +1,34 @@
 import logging
-from typing import Union
 
 import yaml
 
-from .abstract_classes import Rule
 from .rules import RuleFactory
 
+from typing import Any, List, Union  # noqa isort:skip
+
+
+from .abstract_classes import Factory, Rule  # noqa isort:skip
+
 logger = logging.getLogger(__name__)
 
 
 class AuditFilterException(Exception):
     pass
 
 
 class AuditFilter:
     def __init__(self, config: Union[dict, str, None] = None):
-        if isinstance(config, str) and ("yaml" in config or "yml" in config):
-            with open(config) as f:
-                policy = yaml.safe_load(f)
-            if "apiVersion" not in policy or policy["apiVersion"] != "audit.k8s.io/v1":
-                raise AuditFilterException(
-                    "Invalid policy, missing version or version does not match 'audit.k8s.io/v1'"
-                )
-            if "kind" not in policy or policy["kind"] != "Policy":
-                raise AuditFilterException("Invalid policy, missing kind or kind does not match 'Policy'")
-            self.rules = [RuleFactory.create(rule) for rule in policy["rules"]]
-            self.config: list = policy["rules"]
-        elif isinstance(config, dict):
-            self.rules = [RuleFactory.create(rule) for rule in config["rules"]]
-            self.config: list = config["rules"]  # type: ignore
-        elif config is None:
-            self.rules = []  # type: ignore
-            self.config: list = []  # type: ignore
-        else:
-            raise AuditFilterException("Invalid config")
+        self.config = {
+            "apiVersion": "audit.k8s.io/v1",
+            "kind": "Policy",
+            "rules": [],
+        }
+        self.rules = PolicyFactory.create(config)
+        self.config["rules"] = [rule.as_dict for rule in self.rules]
 
     def filter(self, log_line: dict) -> bool:
         if not self.rules:
             return True  # no rules, no filter
         for rule in self.rules:
             try:
                 if rule.check_rule(log_line):
@@ -49,22 +40,66 @@
                 )
                 return True  # if rule check fails, we assume it should not be filtered
         return False
 
     def add_rule(self, rule: dict):
         internal_rule = RuleFactory.create(rule)
         self.rules.append(internal_rule)
-        self.config.append(internal_rule.as_dict)  # type: ignore
+        self.config["rules"].append(internal_rule.as_dict)  # type: ignore
 
     def add_rules(self, rules: list):
         for rule in rules:
             self.add_rule(rule)
 
     def remove_rule(self, rule: dict):
         internal_rule = RuleFactory.create(rule)
         self.rules.remove(internal_rule)
-        self.config.remove(internal_rule.as_dict)  # type: ignore
+        self.config["rules"].remove(internal_rule.as_dict)  # type: ignore
+
+    def remove_rules(self, rules: list):
+        for rule in rules:
+            self.remove_rule(rule)
+
+    def dump_config(self, path_to_config):
+        with open(path_to_config, "w") as f:
+            yaml.dump(self.config, f)
 
     @staticmethod
     def filter_with_rule(log_line: dict, rule: dict) -> bool:
         internal_rule: Rule = RuleFactory.create(rule)
         return internal_rule.check_rule(log_line)
+
+
+def from_yaml(config: str) -> List[Rule]:
+    if not ("yaml" in config or "yml" in config):
+        raise AuditFilterException("Invalid config, must be yaml")
+    with open(config) as f:
+        policy = yaml.safe_load(f)
+    if "apiVersion" not in policy or policy["apiVersion"] != "audit.k8s.io/v1":
+        raise AuditFilterException("Invalid policy, missing version or version does not match 'audit.k8s.io/v1'")
+    if "kind" not in policy or policy["kind"] != "Policy":
+        raise AuditFilterException("Invalid policy, missing kind or kind does not match 'Policy'")
+    return [RuleFactory.create(rule) for rule in policy["rules"]]
+
+
+def from_dict(config: dict) -> List[Rule]:
+    return [RuleFactory.create(rule) for rule in config["rules"]]
+
+
+def empty_config(config: None) -> list:
+    return []
+
+
+class PolicyFactory(Factory):
+    mapping = {
+        str: from_yaml,
+        dict: from_dict,
+        None: empty_config,
+    }
+
+    @classmethod
+    def create(cls, entity: Any):
+        if type(entity) in cls.mapping:
+            return cls.mapping[type(entity)](entity)
+        if entity is None:
+            return cls.mapping[None](entity)
+        raise AuditFilterException(f"Invalid config type {type(entity)}")
```

## k8s_audit_filter/fields.py

```diff
@@ -71,15 +71,15 @@
         "users": UsersField,
         "userGroups": UserGroupsField,
         "namespaces": NamespacesField,
         "resources": ResourceField,
     }
 
     @classmethod
-    def create(cls, entities: dict):
+    def create(cls, entity: dict):
         result = []
-        for key, vale in entities.items():
+        for key, vale in entity.items():
             if key in cls.mapping:
                 result.append(cls.mapping[key](vale))
                 continue
             raise FieldException(f"Invalid field {key} for Rule")
         return result
```

## k8s_audit_filter/resourses_field.py

```diff
@@ -44,17 +44,17 @@
     mapping = {
         "group": ResourceGroupSubField,
         "resources": ResourceResourceSubField,
         "resourceNames": ResourceNamesSubField,
     }
 
     @classmethod
-    def create(cls, entities: dict):
+    def create(cls, entity: dict):
         fields = []
-        for key, value in entities.items():
+        for key, value in entity.items():
             if key in cls.mapping:
                 fields.append(cls.mapping[key](value))
                 continue
             raise FieldException(f"Invalid subfield {key} for Resource field")
         return fields
```

## Comparing `k8s_audit_filter-0.3.0.dist-info/METADATA` & `k8s_audit_filter-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8s-audit-filter
-Version: 0.3.0
+Version: 0.4.0
 Summary: A tool to filter k8s audit logs
 Project-URL: Homepage, https://github.com/petrishutin/k8s-audit-filter
 Project-URL: Tracker, https://github.com/petrishutin/k8s-audit-filter/issues
 Author-email: Petr Ishutinr <ishutinpetrdev@gmail.com>
 License-File: LICENSE
 Keywords: audit,filter,k8s
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

## Comparing `k8s_audit_filter-0.3.0.dist-info/licenses/LICENSE` & `k8s_audit_filter-0.4.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

