# Comparing `tmp/pysigma_backend_sentinelone-0.1.0.tar.gz` & `tmp/pysigma_backend_sentinelone-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_sentinelone-0.1.0.tar", max compression
+gzip compressed data, was "pysigma_backend_sentinelone-0.1.1.tar", max compression
```

## Comparing `pysigma_backend_sentinelone-0.1.0.tar` & `pysigma_backend_sentinelone-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-26 04:50:33.903443 pysigma_backend_sentinelone-0.1.0/LICENSE
--rw-r--r--   0        0        0      574 2023-04-26 04:50:33.903443 pysigma_backend_sentinelone-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       98 2023-04-26 04:50:33.903443 pysigma_backend_sentinelone-0.1.0/sigma/backends/sentinelone/__init__.py
--rw-r--r--   0        0        0     7794 2023-04-26 04:50:33.903443 pysigma_backend_sentinelone-0.1.0/sigma/backends/sentinelone/sentinelone.py
--rw-r--r--   0        0        0      112 2023-04-26 04:50:33.903443 pysigma_backend_sentinelone-0.1.0/sigma/pipelines/sentinelone/__init__.py
--rw-r--r--   0        0        0    13082 2023-04-26 04:50:33.903443 pysigma_backend_sentinelone-0.1.0/sigma/pipelines/sentinelone/sentinelone.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_sentinelone-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/LICENSE
+-rw-r--r--   0        0        0      574 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       98 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/backends/sentinelone/__init__.py
+-rw-r--r--   0        0        0     7792 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/backends/sentinelone/sentinelone.py
+-rw-r--r--   0        0        0      112 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/pipelines/sentinelone/__init__.py
+-rw-r--r--   0        0        0    14568 2023-04-29 03:10:09.489647 pysigma_backend_sentinelone-0.1.1/sigma/pipelines/sentinelone/sentinelone.py
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 pysigma_backend_sentinelone-0.1.1/PKG-INFO
```

### Comparing `pysigma_backend_sentinelone-0.1.0/LICENSE` & `pysigma_backend_sentinelone-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysigma_backend_sentinelone-0.1.0/pyproject.toml` & `pysigma_backend_sentinelone-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pySigma-backend-sentinelone"
-version = "0.1.0"
+version = "0.1.1"
 description = "pySigma SentinelOne backend"
 authors = ["Cori Smith <cs2718281@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/7RedViolin/pySigma-backend-sentinelone"
 packages = [
     { include = "sigma" }
 ]
```

### Comparing `pysigma_backend_sentinelone-0.1.0/sigma/backends/sentinelone/sentinelone.py` & `pysigma_backend_sentinelone-0.1.1/sigma/backends/sentinelone/sentinelone.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     field_escape_quote : ClassVar[bool] = True
     field_escape_pattern : ClassVar[Pattern] = re.compile("\\s")
 
     str_quote       : ClassVar[str] = '"'
     escape_char     : ClassVar[str] = "\\"
     wildcard_multi  : ClassVar[str] = "*"
     wildcard_single : ClassVar[str] = "*"
-    add_escaped     : ClassVar[str] = "\\"
+    add_escaped     : ClassVar[str] = ""
     filter_chars    : ClassVar[str] = ""
     bool_values     : ClassVar[Dict[bool, str]] = {
         True: "true",
         False: "false",
     }
 
     startswith_expression : ClassVar[str] = "{field} startswithCIS {value}"
```

### Comparing `pysigma_backend_sentinelone-0.1.0/sigma/pipelines/sentinelone/sentinelone.py` & `pysigma_backend_sentinelone-0.1.1/sigma/pipelines/sentinelone/sentinelone.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,113 @@
 from sigma.processing.conditions import LogsourceCondition
 from sigma.processing.transformations import AddConditionTransformation, FieldMappingTransformation, DetectionItemFailureTransformation, RuleFailureTransformation, SetStateTransformation, ChangeLogsourceTransformation
 from sigma.processing.conditions import LogsourceCondition, IncludeFieldCondition, ExcludeFieldCondition, RuleProcessingItemAppliedCondition
 from sigma.processing.pipeline import ProcessingItem, ProcessingPipeline
+from sigma.rule import SigmaDetectionItem
+from sigma.exceptions import SigmaTransformationError
+
+class InvalidFieldTransformation(DetectionItemFailureTransformation):
+    """
+    Overrides the apply_detection_item() method from DetectionItemFailureTransformation to also include the field name
+    in the error message
+    """
+
+    def apply_detection_item(self, detection_item: SigmaDetectionItem) -> None:
+        field_name = detection_item.field
+        self.message = f"Invalid SigmaDetectionItem field name encountered: {field_name}. " + self.message
+        raise SigmaTransformationError(self.message)
 
 def sentinelone_pipeline() -> ProcessingPipeline:
 
+    general_supported_fields = [
+        'ObjectType',
+        'EventType'
+    ]
+
+    translation_dict = {
+        'process_creation':{                
+            "ProcessId":"TgtProcPID",
+            "Image":"TgtProcImagePath",
+            "Description":"TgtProcDisplayName", #Not sure whether this should be Description or Product???
+            "Product":"TgtProcDisplayName",
+            "Company":"TgtProcPublisher",
+            "CommandLine":"TgtProcCmdLine",
+            "CurrentDirectory":"TgtProcImagePath",
+            "User":"TgtProcUser",
+            "TerminalSessionId":"TgtProcSessionId",
+            "IntegrityLevel":"TgtProcIntegrityLevel",
+            "md5":"TgtProcMd5",
+            "sha1":"TgtProcSha1",
+            "sha256":"TgtProcSha256",
+            "ParentProcessId":"SrcProcPID",
+            "ParentImage":"SrcProcImagePath",
+            "ParentCommandLine":"SrcProcCmdLine",
+        },
+        'file':{
+            "Image": "SrcProcImagePath",
+            "CommandLine":"SrcProcCmdLine",
+            "ParentImage":"SrcProcParentImagePath",
+            "ParentCommandLine":"SrcProcParentCmdline",
+            "TargetFilename":"TgtFilePath", 
+            "SourceFilename":"TgtFileOldPath",
+            "User":"SrcProcUser"
+        },
+        'image_load':{
+            "ImageLoaded":"ModulePath",
+            "Image": "SrcProcImagePath",
+            "CommandLine":"SrcProcCmdLine",
+            "ParentImage":"SrcProcParentImagePath",
+            "ParentCommandLine":"SrcProcParentCmdline",
+            "sha1":"ModuleSha1",
+            "md5": "ModuleMd5"
+        },
+        'pipe_creation':{
+            "PipeName":"NamedPipeName",
+            "Image": "SrcProcImagePath",
+            "CommandLine":"SrcProcCmdLine",
+            "ParentImage":"SrcProcParentImagePath",
+            "ParentCommandLine":"SrcProcParentCmdline",
+        },
+        'registry':{
+            "Image": "SrcProcImagePath",
+            "CommandLine":"SrcProcCmdLine",
+            "ParentImage":"SrcProcParentImagePath",
+            "ParentCommandLine":"SrcProcParentCmdline",
+            "TargetObject": "RegistryKeyPath",
+            "Details": "RegistryValue"
+        },
+        'dns':{
+            "Image": "SrcProcImagePath",
+            "CommandLine":"SrcProcCmdLine",
+            "ParentImage":"SrcProcParentImagePath",
+            "ParentCommandLine":"SrcProcParentCmdline",
+            "query": "DnsRequest",
+            "answer":"DnsResponse",
+            "QueryName": "DnsRequest",
+            "record_type":"DnsResponse"
+        },
+        'network':{
+            "Image": "SrcProcImagePath",
+            "CommandLine":"SrcProcCmdLine",
+            "ParentImage":"SrcProcParentImagePath",
+            "ParentCommandLine":"SrcProcParentCmdline",
+            "DestinationHostname":["Url", "DnsRequest"],
+            "DestinationPort":"DstPort",
+            "DestinationIp":"DstIP",
+            "User":"SrcProcUser",
+            "SourceIp":"SrcIP",
+            "SourcePort":"SrcPort",
+            "Protocol":"NetProtocolName",
+            "dst_ip":"DstIP",
+            "src_ip":"SrcIP",
+            "dst_port":"DstPort",
+            "src_port":"SrcPort"
+        }
+    }
+
     os_filter = [
         # Add EndpointOS = Linux
         ProcessingItem(
             identifier="s1_linux_product",
             transformation=AddConditionTransformation({
                 "EndpointOS": "linux"
             }),
@@ -147,144 +246,73 @@
         )
     ]
 
     field_mappings = [
         # Process Creation
         ProcessingItem(
             identifier="s1_process_creation_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "ProcessId":"TgtProcPID",
-                "Image":"TgtProcName",
-                "Description":"TgtProcDisplayName", #Not sure whether this should be Description or Product???
-                "Product":"TgtProcDisplayName",
-                "Company":"TgtProcPublisher",
-                "CommandLine":"TgtProcCmdLine",
-                "CurrentDirectory":"TgtProcImagePath",
-                "User":"TgtProcUser",
-                "TerminalSessionId":"TgtProcSessionId",
-                "IntegrityLevel":"TgtProcIntegrityLevel",
-                "md5":"TgtProcMd5",
-                "sha1":"TgtProcSha1",
-                "sha256":"TgtProcSha256",
-                "ParentProcessId":"SrcProcPID",
-                "ParentImage":"SrcProcName",
-                "ParentCommandLine":"SrcProcCmdLine",
-            }),
+            transformation=FieldMappingTransformation(translation_dict['process_creation']),
             rule_conditions=[
                 LogsourceCondition(category="process_creation")
             ]
         ),
         # File Stuff
         ProcessingItem(
             identifier="s1_file_change_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "Image": "SrcProcName",
-                "CommandLine":"SrcProcCmdLine",
-                "ParentImage":"SrcProcParentName",
-                "ParentCommandLine":"SrcProcParentCmdline",
-                "TargetFilename":"TgtFilePath", 
-                "SourceFilename":"TgtFileOldPath",
-                "User":"SrcProcUser"
-            }),
+            transformation=FieldMappingTransformation(translation_dict['file']),
             rule_condition_linking=any,
             rule_conditions=[
                 LogsourceCondition(category="file_change"),
                 LogsourceCondition(category="file_rename"),
                 LogsourceCondition(category="file_delete"),
                 LogsourceCondition(category="file_event")
             ]
         ),
         # Module Load Stuff
         ProcessingItem(
             identifier="s1_image_load_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "ImageLoaded":"ModulePath",
-                "Image": "SrcProcName",
-                "CommandLine":"SrcProcCmdLine",
-                "ParentImage":"SrcProcParentName",
-                "ParentCommandLine":"SrcProcParentCmdline",
-                "sha1":"ModuleSha1",
-                "md5": "ModuleMd5"
-            }),
+            transformation=FieldMappingTransformation(translation_dict['image_load']),
             rule_conditions=[
                 LogsourceCondition(category="image_load")
             ]
         ),
         # Pipe Creation Stuff
         ProcessingItem(
             identifier="s1_pipe_creation_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "PipeName":"NamedPipeName",
-                "Image": "SrcProcName",
-                "CommandLine":"SrcProcCmdLine",
-                "ParentImage":"SrcProcParentName",
-                "ParentCommandLine":"SrcProcParentCmdline",
-            }),
+            transformation=FieldMappingTransformation(translation_dict['pipe_creation']),
             rule_conditions=[
                 LogsourceCondition(category="pipe_creation")
             ]
         ),
         # Registry Stuff
         ProcessingItem(
             identifier="s1_registry_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "Image": "SrcProcName",
-                "CommandLine":"SrcProcCmdLine",
-                "ParentImage":"SrcProcParentName",
-                "ParentCommandLine":"SrcProcParentCmdline",
-                "TargetObject": "RegistryKeyPath",
-                "Details": "RegistryValue"
-            }),
+            transformation=FieldMappingTransformation(translation_dict['registry']),
             rule_condition_linking=any,
             rule_conditions=[
                 LogsourceCondition(category="registry_add"),
                 LogsourceCondition(category="registry_delete"),
                 LogsourceCondition(category="registry_event"),
                 LogsourceCondition(category="registry_set")
             ]
         ),
         # DNS Stuff
         ProcessingItem(
             identifier="s1_dns_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "Image": "SrcProcName",
-                "CommandLine":"SrcProcCmdLine",
-                "ParentImage":"SrcProcParentName",
-                "ParentCommandLine":"SrcProcParentCmdline",
-                "query": "DnsRequest",
-                "answer":"DnsResponse",
-                "QueryName": "DnsRequest",
-                "record_type":"DnsResponse"
-            }),
+            transformation=FieldMappingTransformation(translation_dict['dns']),
             rule_condition_linking=any,
             rule_conditions=[
                 LogsourceCondition(category="dns_query"),
                 LogsourceCondition(category="dns")
             ]
         ),
         # Network Stuff
         ProcessingItem(
             identifier="s1_network_fieldmapping",
-            transformation=FieldMappingTransformation({
-                "Image": "SrcProcName",
-                "CommandLine":"SrcProcCmdLine",
-                "ParentImage":"SrcProcParentName",
-                "ParentCommandLine":"SrcProcParentCmdline",
-                "DestinationHostname":["Url", "DnsRequest"],
-                "DestinationPort":"DstPort",
-                "DestinationIp":"DstIP",
-                "User":"SrcProcUser",
-                "SourceIp":"SrcIP",
-                "SourcePort":"SrcPort",
-                "Protocol":"NetProtocolName",
-                "dst_ip":"DstIP",
-                "src_ip":"SrcIP",
-                "dst_port":"DstPort",
-                "src_port":"SrcPort"
-            }),
+            transformation=FieldMappingTransformation(translation_dict['network']),
             rule_condition_linking=any,
             rule_conditions=[
                 LogsourceCondition(category="network_connection"),
                 LogsourceCondition(category="firewall")
             ]
         )
     ]
@@ -326,18 +354,30 @@
             rule_condition_negation=True,
             rule_conditions=[
                 RuleProcessingItemAppliedCondition("s1_logsource")
             ]
         )
     ]
 
+    unsupported_field_name = [
+        ProcessingItem(
+            identifier='s1_fail_field_not_supported',
+            transformation=InvalidFieldTransformation("This pipeline only supports the following fields:\n{" + 
+            '}, {'.join(sorted(set(sum([list(translation_dict[x].keys()) for x in translation_dict.keys()],[])))) + '}'),
+            field_name_conditions=[
+                ExcludeFieldCondition(fields=list(set(sum([list(translation_dict[x].keys()) for x in translation_dict.keys()],[]))) + general_supported_fields)
+            ]
+        )
+    ]
+
     return ProcessingPipeline(
         name="SentinelOne pipeline",
         priority=50,
         items = [
+            *unsupported_field_name,
             *os_filter,
             *object_event_type_filter,
             *field_mappings,
             *change_logsource_info,
-            *unsupported_rule_types
+            *unsupported_rule_types,
         ]
     )
```

### Comparing `pysigma_backend_sentinelone-0.1.0/PKG-INFO` & `pysigma_backend_sentinelone-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysigma-backend-sentinelone
-Version: 0.1.0
+Version: 0.1.1
 Summary: pySigma SentinelOne backend
 Home-page: https://github.com/7RedViolin/pySigma-backend-sentinelone
 License: MIT
 Author: Cori Smith
 Author-email: cs2718281@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

