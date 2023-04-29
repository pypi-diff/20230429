# Comparing `tmp/iam_actions-1.2.20230428.tar.gz` & `tmp/iam_actions-1.2.20230429.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230428.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230429.tar", max compression
```

## Comparing `iam_actions-1.2.20230428.tar` & `iam_actions-1.2.20230429.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/LICENSE
--rw-r--r--   0        0        0     2302 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/README.md
--rw-r--r--   0        0        0      228 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/__init__.py
--rw-r--r--   0        0        0  4233746 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-04-28 02:27:06.169616 iam_actions-1.2.20230428/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545011 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/policies.json
--rw-r--r--   0        0        0   190316 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   528566 2023-04-28 02:29:08.345723 iam_actions-1.2.20230428/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-04-28 02:29:09.361723 iam_actions-1.2.20230428/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230428/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230428/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/LICENSE
+-rw-r--r--   0        0        0     2302 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/README.md
+-rw-r--r--   0        0        0      228 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4240120 2023-04-29 02:26:21.126970 iam_actions-1.2.20230429/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-04-29 02:24:59.433844 iam_actions-1.2.20230429/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545330 2023-04-29 02:26:21.126970 iam_actions-1.2.20230429/iam_actions/policies.json
+-rw-r--r--   0        0        0   193320 2023-04-29 02:26:21.126970 iam_actions-1.2.20230429/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   528875 2023-04-29 02:26:21.126970 iam_actions-1.2.20230429/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-04-29 02:26:21.887013 iam_actions-1.2.20230429/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230429/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230429/PKG-INFO
```

### Comparing `iam_actions-1.2.20230428/LICENSE` & `iam_actions-1.2.20230429/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/README.md` & `iam_actions-1.2.20230429/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/actions.json` & `iam_actions-1.2.20230429/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996432420321628%*

 * *Differences: {"'aoss'": "{'APIAccessAll': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *           "'APIAccessAll'), ('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *           "('orphan', False), ('resources', [])]), 'DashboardsAccessAll': "*

 * *           "OrderedDict([('access_level', 'Undocumented'), ('action', 'DashboardsAccessAll'), "*

 * *           "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', False), "*

 * *           "('resources', [])])}",*

 * * "'athena'": "{'Can […]*

```diff
@@ -2925,14 +2925,22 @@
             "orphan": false,
             "resources": [
                 "ThemeResource"
             ]
         }
     },
     "aoss": {
+        "APIAccessAll": {
+            "access_level": "Undocumented",
+            "action": "APIAccessAll",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchGetCollection": {
             "access_level": "Read",
             "action": "BatchGetCollection",
             "condition_keys": [],
             "description": "Grants permission to get attributes for one or more collections",
             "orphan": false,
             "resources": []
@@ -2984,14 +2992,22 @@
             "access_level": "Write",
             "action": "CreateVpcEndpoint",
             "condition_keys": [],
             "description": "Grants permission to create an OpenSearch-Serverless-managed interface VPC endpoint",
             "orphan": false,
             "resources": []
         },
+        "DashboardsAccessAll": {
+            "access_level": "Undocumented",
+            "action": "DashboardsAccessAll",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteAccessPolicy": {
             "access_level": "Write",
             "action": "DeleteAccessPolicy",
             "condition_keys": [],
             "description": "Grants permission to delete a data access policy",
             "orphan": false,
             "resources": []
@@ -7947,14 +7963,30 @@
             "condition_keys": [],
             "description": "Grants permission to get information about one or more query executions",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
+        "CancelCapacityReservation": {
+            "access_level": "Undocumented",
+            "action": "CancelCapacityReservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateCapacityReservation": {
+            "access_level": "Undocumented",
+            "action": "CreateCapacityReservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateDataCatalog": {
             "access_level": "Write",
             "action": "CreateDataCatalog",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -8103,14 +8135,30 @@
             "condition_keys": [],
             "description": "Grants permission to get a calculation execution status",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
+        "GetCapacityAssignmentConfiguration": {
+            "access_level": "Undocumented",
+            "action": "GetCapacityAssignmentConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetCapacityReservation": {
+            "access_level": "Undocumented",
+            "action": "GetCapacityReservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetDataCatalog": {
             "access_level": "Read",
             "action": "GetDataCatalog",
             "condition_keys": [],
             "description": "Grants permission to get a datacatalog",
             "orphan": false,
             "resources": [
@@ -8261,14 +8309,22 @@
             "condition_keys": [],
             "description": "Grants permission to return a list of calculation executions",
             "orphan": false,
             "resources": [
                 "workgroup"
             ]
         },
+        "ListCapacityReservations": {
+            "access_level": "Undocumented",
+            "action": "ListCapacityReservations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListDataCatalogs": {
             "access_level": "List",
             "action": "ListDataCatalogs",
             "condition_keys": [],
             "description": "Grants permission to return a list of datacatalogs for the specified AWS account",
             "orphan": false,
             "resources": []
@@ -8384,14 +8440,22 @@
             "access_level": "List",
             "action": "ListWorkGroups",
             "condition_keys": [],
             "description": "Grants permission to return a list of workgroups for the specified AWS account",
             "orphan": false,
             "resources": []
         },
+        "PutCapacityAssignmentConfiguration": {
+            "access_level": "Undocumented",
+            "action": "PutCapacityAssignmentConfiguration",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "StartCalculationExecution": {
             "access_level": "Write",
             "action": "StartCalculationExecution",
             "condition_keys": [],
             "description": "Grants permission to start a calculation execution",
             "orphan": false,
             "resources": [
@@ -8471,14 +8535,22 @@
             "description": "Grants permission to remove a tag from a resource",
             "orphan": false,
             "resources": [
                 "datacatalog",
                 "workgroup"
             ]
         },
+        "UpdateCapacityReservation": {
+            "access_level": "Undocumented",
+            "action": "UpdateCapacityReservation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateDataCatalog": {
             "access_level": "Write",
             "action": "UpdateDataCatalog",
             "condition_keys": [],
             "description": "Grants permission to update a datacatalog",
             "orphan": false,
             "resources": [
@@ -29311,20 +29383,24 @@
                 "OrganizationConformancePack",
                 "StoredQuery"
             ]
         }
     },
     "connect": {
         "ActivateEvaluationForm": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ActivateEvaluationForm",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to activate an evaluation form in the specified Amazon Connect instance. After the evaluation form is activated, it is available to start new evaluations based on the form",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "AssociateApprovedOrigin": {
             "access_level": "Write",
             "action": "AssociateApprovedOrigin",
             "condition_keys": [
                 "connect:InstanceId"
             ],
@@ -29537,20 +29613,24 @@
             "description": "Grants permission to create a contact flow module in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact-flow-module"
             ]
         },
         "CreateEvaluationForm": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateEvaluationForm",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to create an evaluation form in the specified Amazon Connect instance. The form can be used to define questions related to agent performance, and create sections to organize such questions. Question and section identifiers cannot be duplicated within the same evaluation form",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "CreateHoursOfOperation": {
             "access_level": "Write",
             "action": "CreateHoursOfOperation",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
@@ -29760,28 +29840,37 @@
             "description": "Grants permission to create a vocabulary in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "vocabulary"
             ]
         },
         "DeactivateEvaluationForm": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeactivateEvaluationForm",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to deactivate an evaluation form in the specified Amazon Connect instance. After a form is deactivated, it is no longer available for users to start new evaluations based on the form",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "DeleteContactEvaluation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteContactEvaluation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to delete a contact evaluation in the specified Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "contact-evaluation"
+            ]
         },
         "DeleteContactFlow": {
             "access_level": "Write",
             "action": "DeleteContactFlow",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -29802,20 +29891,25 @@
             "description": "Grants permission to delete a contact flow module in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact-flow-module"
             ]
         },
         "DeleteEvaluationForm": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteEvaluationForm",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to delete an evaluation form in the specified Amazon Connect instance. If the version property is provided, only the specified version of the evaluation form is deleted",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "DeleteHoursOfOperation": {
             "access_level": "Write",
             "action": "DeleteHoursOfOperation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -29989,20 +30083,25 @@
             "description": "Grants permission to describe a contact in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact"
             ]
         },
         "DescribeContactEvaluation": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeContactEvaluation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to describe a contact evaluation in the specified Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "contact-evaluation"
+            ]
         },
         "DescribeContactFlow": {
             "access_level": "Read",
             "action": "DescribeContactFlow",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -30023,20 +30122,25 @@
             "description": "Grants permission to describe a contact flow module in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact-flow-module"
             ]
         },
         "DescribeEvaluationForm": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeEvaluationForm",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:ResourceTag/${TagKey}",
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to describe an evaluation form in the specified Amazon Connect instance. If the version property is not provided, the latest version of the evaluation form is described",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "DescribeForecastingPlanningSchedulingIntegration": {
             "access_level": "Read",
             "action": "DescribeForecastingPlanningSchedulingIntegration",
             "condition_keys": [
                 "connect:InstanceId"
             ],
@@ -30516,20 +30620,24 @@
             "description": "Grants permission to view the Lex bots of an existing Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
         "ListContactEvaluations": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListContactEvaluations",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to list contact evaluations in the specified Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ListContactFlowModules": {
             "access_level": "List",
             "action": "ListContactFlowModules",
             "condition_keys": [],
             "description": "Grants permission to list contact flow module resources in an Amazon Connect instance",
             "orphan": false,
@@ -30568,28 +30676,36 @@
             "description": "Grants permission to list default vocabularies associated with a Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
         "ListEvaluationFormVersions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListEvaluationFormVersions",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to list versions of an evaluation form in the specified Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "ListEvaluationForms": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListEvaluationForms",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to list evaluation forms in the specified Amazon Connect instance",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "instance"
+            ]
         },
         "ListHoursOfOperations": {
             "access_level": "List",
             "action": "ListHoursOfOperations",
             "condition_keys": [
                 "connect:InstanceId"
             ],
@@ -30822,16 +30938,18 @@
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}"
             ],
             "description": "Grants permission to list tags for an Amazon Connect resource",
             "orphan": false,
             "resources": [
                 "agent-status",
+                "contact-evaluation",
                 "contact-flow",
                 "contact-flow-module",
+                "evaluation-form",
                 "hierarchy-group",
                 "hours-of-operation",
                 "integration-association",
                 "phone-number",
                 "queue",
                 "quick-connect",
                 "routing-profile",
@@ -31047,20 +31165,24 @@
             "orphan": false,
             "resources": [
                 "contact",
                 "contact-flow"
             ]
         },
         "StartContactEvaluation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartContactEvaluation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to start an empty evaluation in the specified Amazon Connect instance, using the given evaluation form for the particular contact. The evaluation form version used for the contact evaluation corresponds to the currently activated version. If no version is activated for the evaluation form, the contact evaluation cannot be started",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "contact-evaluation"
+            ]
         },
         "StartContactRecording": {
             "access_level": "Write",
             "action": "StartContactRecording",
             "condition_keys": [],
             "description": "Grants permission to start recording for the specified contact",
             "orphan": false,
@@ -31157,20 +31279,24 @@
             "description": "Grants permission to disable forecasting, planning, and scheduling integration on an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
         "SubmitContactEvaluation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "SubmitContactEvaluation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to submit a contact evaluation in the specified Amazon Connect instance. Answers included in the request are merged with existing answers for the given evaluation. If no answers or notes are passed, the evaluation is submitted with the existing answers and notes. You can delete an answer or note by passing an empty object ({}) to the question identifier",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "contact-evaluation"
+            ]
         },
         "SuspendContactRecording": {
             "access_level": "Write",
             "action": "SuspendContactRecording",
             "condition_keys": [],
             "description": "Grants permission to suspend recording for the specified contact",
             "orphan": false,
@@ -31185,16 +31311,18 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to tag an Amazon Connect resource",
             "orphan": false,
             "resources": [
                 "agent-status",
+                "contact-evaluation",
                 "contact-flow",
                 "contact-flow-module",
+                "evaluation-form",
                 "hierarchy-group",
                 "hours-of-operation",
                 "instance",
                 "integration-association",
                 "phone-number",
                 "queue",
                 "quick-connect",
@@ -31229,16 +31357,18 @@
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to untag an Amazon Connect resource",
             "orphan": false,
             "resources": [
                 "agent-status",
+                "contact-evaluation",
                 "contact-flow",
                 "contact-flow-module",
+                "evaluation-form",
                 "hierarchy-group",
                 "hours-of-operation",
                 "instance",
                 "integration-association",
                 "phone-number",
                 "queue",
                 "quick-connect",
@@ -31287,20 +31417,24 @@
             "description": "Grants permission to create or update the contact attributes associated with the specified contact",
             "orphan": false,
             "resources": [
                 "contact"
             ]
         },
         "UpdateContactEvaluation": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateContactEvaluation",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to update details about a contact evaluation in the specified Amazon Connect instance. A contact evaluation must be in the draft state. Answers included in the request are merged with existing answers for the given evaluation. An answer or note can be deleted by passing an empty object ({}) to the question identifier",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "contact-evaluation"
+            ]
         },
         "UpdateContactFlowContent": {
             "access_level": "Write",
             "action": "UpdateContactFlowContent",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -31372,20 +31506,24 @@
             "description": "Grants permission to update the schedule of a contact that is already scheduled in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "contact"
             ]
         },
         "UpdateEvaluationForm": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateEvaluationForm",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "connect:InstanceId"
+            ],
+            "description": "Grants permission to update details about a specific evaluation form version in the specified Amazon Connect instance. Question and section identifiers cannot be duplicated within the same evaluation form",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "evaluation-form"
+            ]
         },
         "UpdateHoursOfOperation": {
             "access_level": "Write",
             "action": "UpdateHoursOfOperation",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
@@ -57546,14 +57684,22 @@
             "condition_keys": [],
             "description": "Grants permission to view information about domain and node health, the standby Availability Zone, number of nodes per Availability Zone, and shard count per node",
             "orphan": false,
             "resources": [
                 "domain"
             ]
         },
+        "DescribeDomainNodes": {
+            "access_level": "Undocumented",
+            "action": "DescribeDomainNodes",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeDomains": {
             "access_level": "List",
             "action": "DescribeDomains",
             "condition_keys": [],
             "description": "Grants permission to view a description of the domain configuration for up to five specified OpenSearch Service domains",
             "orphan": false,
             "resources": [
@@ -69602,18 +69748,18 @@
             "action": "SendSecurityTelemetry",
             "condition_keys": [],
             "description": "Grants permission to send security telemetry for a specific GuardDuty account in a Region",
             "orphan": false,
             "resources": []
         },
         "StartMalwareScan": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "StartMalwareScan",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to initiate a new malware scan",
             "orphan": false,
             "resources": []
         },
         "StartMonitoringMembers": {
             "access_level": "Write",
             "action": "StartMonitoringMembers",
             "condition_keys": [],
@@ -81393,52 +81539,59 @@
             "action": "CreateConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create an MSK configuration",
             "orphan": false,
             "resources": []
         },
         "CreateVpcConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "CreateVpcConnection",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to create a MSK VPC connection",
             "orphan": false,
             "resources": []
         },
         "DeleteCluster": {
             "access_level": "Write",
             "action": "DeleteCluster",
             "condition_keys": [],
             "description": "Grants permission to delete an MSK cluster",
             "orphan": false,
             "resources": []
         },
         "DeleteClusterPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteClusterPolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a cluster resource-based policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "DeleteConfiguration": {
             "access_level": "Write",
             "action": "DeleteConfiguration",
             "condition_keys": [],
             "description": "Grants permission to delete the specified MSK configuration",
             "orphan": false,
             "resources": []
         },
         "DeleteVpcConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteVpcConnection",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a MSK VPC connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-connection"
+            ]
         },
         "DescribeCluster": {
             "access_level": "Read",
             "action": "DescribeCluster",
             "condition_keys": [],
             "description": "Grants permission to describe an MSK cluster",
             "orphan": false,
@@ -81477,52 +81630,58 @@
             "description": "Grants permission to describe an MSK configuration revision",
             "orphan": false,
             "resources": [
                 "configuration"
             ]
         },
         "DescribeVpcConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeVpcConnection",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a MSK VPC connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "vpc-connection"
+            ]
         },
         "GetBootstrapBrokers": {
             "access_level": "Read",
             "action": "GetBootstrapBrokers",
             "condition_keys": [],
             "description": "Grants permission to get connection details for the brokers in an MSK cluster",
             "orphan": false,
             "resources": []
         },
         "GetClusterPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetClusterPolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a cluster resource-based policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "GetCompatibleKafkaVersions": {
             "access_level": "List",
             "action": "GetCompatibleKafkaVersions",
             "condition_keys": [],
             "description": "Grants permission to get a list of the Apache Kafka versions to which you can update an MSK cluster",
             "orphan": false,
             "resources": []
         },
         "ListClientVpcConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListClientVpcConnections",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all MSK VPC connections created for a cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "ListClusterOperations": {
             "access_level": "List",
             "action": "ListClusterOperations",
             "condition_keys": [],
             "description": "Grants permission to return a list of all the operations that have been performed on the specified MSK cluster",
             "orphan": false,
@@ -81591,68 +81750,74 @@
             "description": "Grants permission to list tags of an MSK resource",
             "orphan": false,
             "resources": [
                 "cluster"
             ]
         },
         "ListVpcConnections": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListVpcConnections",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list all MSK VPC connections that this account uses",
             "orphan": false,
             "resources": []
         },
         "PutClusterPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutClusterPolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create or update the resource-based policy for a cluster",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "RebootBroker": {
             "access_level": "Write",
             "action": "RebootBroker",
             "condition_keys": [],
             "description": "Grants permission to reboot broker",
             "orphan": false,
             "resources": []
         },
         "RejectClientVpcConnection": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "RejectClientVpcConnection",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to reject a MSK VPC connection",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "cluster"
+            ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to tag an MSK resource",
             "orphan": false,
             "resources": [
-                "cluster"
+                "cluster",
+                "vpc-connection"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags from an MSK resource",
             "orphan": false,
             "resources": [
-                "cluster"
+                "cluster",
+                "vpc-connection"
             ]
         },
         "UpdateBrokerCount": {
             "access_level": "Write",
             "action": "UpdateBrokerCount",
             "condition_keys": [],
             "description": "Grants permission to update the number of brokers of the MSK cluster",
@@ -81698,15 +81863,17 @@
             "description": "Grants permission to create a new revision of the MSK configuration",
             "orphan": false,
             "resources": []
         },
         "UpdateConnectivity": {
             "access_level": "Write",
             "action": "UpdateConnectivity",
-            "condition_keys": [],
+            "condition_keys": [
+                "kafka:publicAccessEnabled"
+            ],
             "description": "Grants permission to update the connectivity settings for the MSK cluster",
             "orphan": false,
             "resources": []
         },
         "UpdateMonitoring": {
             "access_level": "Write",
             "action": "UpdateMonitoring",
@@ -97307,457 +97474,468 @@
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an app",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "apps"
+            ]
         },
         "CreateCampaign": {
             "access_level": "Write",
             "action": "CreateCampaign",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a campaign for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "CreateEmailTemplate": {
             "access_level": "Write",
             "action": "CreateEmailTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an email template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "template"
+            ]
         },
         "CreateExportJob": {
             "access_level": "Write",
             "action": "CreateExportJob",
             "condition_keys": [],
             "description": "Grants permission to create an export job that exports endpoint definitions to Amazon S3",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "CreateImportJob": {
             "access_level": "Write",
             "action": "CreateImportJob",
             "condition_keys": [],
             "description": "Grants permission to import endpoint definitions from to create a segment",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "CreateInAppTemplate": {
             "access_level": "Write",
             "action": "CreateInAppTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an in-app message template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "template"
+            ]
         },
         "CreateJourney": {
             "access_level": "Write",
             "action": "CreateJourney",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a Journey for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "journeys"
             ]
         },
         "CreatePushTemplate": {
             "access_level": "Write",
             "action": "CreatePushTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a push notification template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "template"
+            ]
         },
         "CreateRecommenderConfiguration": {
             "access_level": "Write",
             "action": "CreateRecommenderConfiguration",
             "condition_keys": [],
             "description": "Grants permission to create an Amazon Pinpoint configuration for a recommender model",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "recommenders"
+            ]
         },
         "CreateSegment": {
             "access_level": "Write",
             "action": "CreateSegment",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a segment that is based on endpoint data reported to Pinpoint by your app. To allow a user to create a segment by importing endpoint data from outside of Pinpoint, allow the mobiletargeting:CreateImportJob action",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "CreateSmsTemplate": {
             "access_level": "Write",
             "action": "CreateSmsTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create an sms message template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "template"
+            ]
         },
         "CreateVoiceTemplate": {
             "access_level": "Write",
             "action": "CreateVoiceTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a voice message template",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "template"
+            ]
         },
         "DeleteAdmChannel": {
             "access_level": "Write",
             "action": "DeleteAdmChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the ADM channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteApnsChannel": {
             "access_level": "Write",
             "action": "DeleteApnsChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the APNs channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteApnsSandboxChannel": {
             "access_level": "Write",
             "action": "DeleteApnsSandboxChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the APNs sandbox channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteApnsVoipChannel": {
             "access_level": "Write",
             "action": "DeleteApnsVoipChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the APNs VoIP channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteApnsVoipSandboxChannel": {
             "access_level": "Write",
             "action": "DeleteApnsVoipSandboxChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the APNs VoIP sandbox channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteApp": {
             "access_level": "Write",
             "action": "DeleteApp",
             "condition_keys": [],
             "description": "Grants permission to delete a specific campaign",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "DeleteBaiduChannel": {
             "access_level": "Write",
             "action": "DeleteBaiduChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the Baidu channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteCampaign": {
             "access_level": "Write",
             "action": "DeleteCampaign",
             "condition_keys": [],
             "description": "Grants permission to delete a specific campaign",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign"
             ]
         },
         "DeleteEmailChannel": {
             "access_level": "Write",
             "action": "DeleteEmailChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the email channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteEmailTemplate": {
             "access_level": "Write",
             "action": "DeleteEmailTemplate",
             "condition_keys": [],
             "description": "Grants permission to delete an email template or an email template version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "DeleteEndpoint": {
             "access_level": "Write",
             "action": "DeleteEndpoint",
             "condition_keys": [],
             "description": "Grants permission to delete an endpoint",
             "orphan": false,
             "resources": [
-                "apps"
+                "endpoint"
             ]
         },
         "DeleteEventStream": {
             "access_level": "Write",
             "action": "DeleteEventStream",
             "condition_keys": [],
             "description": "Grants permission to delete the event stream for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "event-stream"
             ]
         },
         "DeleteGcmChannel": {
             "access_level": "Write",
             "action": "DeleteGcmChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the GCM channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteInAppTemplate": {
             "access_level": "Write",
             "action": "DeleteInAppTemplate",
             "condition_keys": [],
             "description": "Grants permission to delete an in-app message template or an in-app message template version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "DeleteJourney": {
             "access_level": "Write",
             "action": "DeleteJourney",
             "condition_keys": [],
             "description": "Grants permission to delete a specific journey",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey"
             ]
         },
         "DeletePushTemplate": {
             "access_level": "Write",
             "action": "DeletePushTemplate",
             "condition_keys": [],
             "description": "Grants permission to delete a push notification template or a push notification template version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "DeleteRecommenderConfiguration": {
             "access_level": "Write",
             "action": "DeleteRecommenderConfiguration",
             "condition_keys": [],
             "description": "Grants permission to delete an Amazon Pinpoint configuration for a recommender model",
             "orphan": false,
             "resources": [
-                "recommenders"
+                "recommender"
             ]
         },
         "DeleteSegment": {
             "access_level": "Write",
             "action": "DeleteSegment",
             "condition_keys": [],
             "description": "Grants permission to delete a specific segment",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "DeleteSmsChannel": {
             "access_level": "Write",
             "action": "DeleteSmsChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the SMS channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteSmsTemplate": {
             "access_level": "Write",
             "action": "DeleteSmsTemplate",
             "condition_keys": [],
             "description": "Grants permission to delete an sms message template or an sms message template version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "DeleteUserEndpoints": {
             "access_level": "Write",
             "action": "DeleteUserEndpoints",
             "condition_keys": [],
             "description": "Grants permission to delete all of the endpoints that are associated with a user ID",
             "orphan": false,
             "resources": [
-                "apps"
+                "user"
             ]
         },
         "DeleteVoiceChannel": {
             "access_level": "Write",
             "action": "DeleteVoiceChannel",
             "condition_keys": [],
             "description": "Grants permission to delete the Voice channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "DeleteVoiceTemplate": {
             "access_level": "Write",
             "action": "DeleteVoiceTemplate",
             "condition_keys": [],
             "description": "Grants permission to delete a voice message template or a voice message template version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "GetAdmChannel": {
             "access_level": "Read",
             "action": "GetAdmChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the Amazon Device Messaging (ADM) channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetApnsChannel": {
             "access_level": "Read",
             "action": "GetApnsChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the APNs channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetApnsSandboxChannel": {
             "access_level": "Read",
             "action": "GetApnsSandboxChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the APNs sandbox channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetApnsVoipChannel": {
             "access_level": "Read",
             "action": "GetApnsVoipChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the APNs VoIP channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetApnsVoipSandboxChannel": {
             "access_level": "Read",
             "action": "GetApnsVoipSandboxChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the APNs VoIP sandbox channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetApp": {
             "access_level": "Read",
             "action": "GetApp",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific app in your Amazon Pinpoint account",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetApplicationDateRangeKpi": {
             "access_level": "Read",
             "action": "GetApplicationDateRangeKpi",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard metric that applies to an application",
             "orphan": false,
             "resources": [
-                "apps"
+                "application-metrics"
             ]
         },
         "GetApplicationSettings": {
             "access_level": "List",
             "action": "GetApplicationSettings",
             "condition_keys": [],
             "description": "Grants permission to retrieve the default settings for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetApps": {
             "access_level": "Read",
             "action": "GetApps",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of apps in your Amazon Pinpoint account",
@@ -97769,457 +97947,449 @@
         "GetBaiduChannel": {
             "access_level": "Read",
             "action": "GetBaiduChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the Baidu channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetCampaign": {
             "access_level": "Read",
             "action": "GetCampaign",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific campaign",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign"
             ]
         },
         "GetCampaignActivities": {
             "access_level": "List",
             "action": "GetCampaignActivities",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the activities performed by a campaign",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign"
             ]
         },
         "GetCampaignDateRangeKpi": {
             "access_level": "Read",
             "action": "GetCampaignDateRangeKpi",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard metric that applies to a campaign",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign-metrics"
             ]
         },
         "GetCampaignVersion": {
             "access_level": "Read",
             "action": "GetCampaignVersion",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific campaign version",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign"
             ]
         },
         "GetCampaignVersions": {
             "access_level": "List",
             "action": "GetCampaignVersions",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the current and prior versions of a campaign",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign"
             ]
         },
         "GetCampaigns": {
             "access_level": "List",
             "action": "GetCampaigns",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about all campaigns for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetChannels": {
             "access_level": "List",
             "action": "GetChannels",
             "condition_keys": [],
             "description": "Grants permission to get all channels information for your app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channels"
             ]
         },
         "GetEmailChannel": {
             "access_level": "Read",
             "action": "GetEmailChannel",
             "condition_keys": [],
             "description": "Grants permission to obtain information about the email channel in an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetEmailTemplate": {
             "access_level": "Read",
             "action": "GetEmailTemplate",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific or the active version of an email template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "GetEndpoint": {
             "access_level": "Read",
             "action": "GetEndpoint",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific endpoint",
             "orphan": false,
             "resources": [
-                "apps"
+                "endpoint"
             ]
         },
         "GetEventStream": {
             "access_level": "Read",
             "action": "GetEventStream",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the event stream for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "event-stream"
             ]
         },
         "GetExportJob": {
             "access_level": "Read",
             "action": "GetExportJob",
             "condition_keys": [],
             "description": "Grants permission to obtain information about a specific export job",
             "orphan": false,
             "resources": [
-                "apps"
+                "export-job"
             ]
         },
         "GetExportJobs": {
             "access_level": "List",
             "action": "GetExportJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of all of the export jobs for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetGcmChannel": {
             "access_level": "Read",
             "action": "GetGcmChannel",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the GCM channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetImportJob": {
             "access_level": "Read",
             "action": "GetImportJob",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific import job",
             "orphan": false,
             "resources": [
-                "apps"
+                "import-job"
             ]
         },
         "GetImportJobs": {
             "access_level": "List",
             "action": "GetImportJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about all import jobs for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetInAppMessages": {
             "access_level": "Read",
             "action": "GetInAppMessages",
             "condition_keys": [],
             "description": "Grants permission to retrive in-app messages for the given endpoint id",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetInAppTemplate": {
             "access_level": "Read",
             "action": "GetInAppTemplate",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific or the active version of an in-app message template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "GetJourney": {
             "access_level": "Read",
             "action": "GetJourney",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific journey",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey"
             ]
         },
         "GetJourneyDateRangeKpi": {
             "access_level": "Read",
             "action": "GetJourneyDateRangeKpi",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard engagement metric that applies to a journey",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey-metrics"
             ]
         },
         "GetJourneyExecutionActivityMetrics": {
             "access_level": "Read",
             "action": "GetJourneyExecutionActivityMetrics",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard execution metric that applies to a journey activity",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey-execution-activity-metrics"
             ]
         },
         "GetJourneyExecutionMetrics": {
             "access_level": "Read",
             "action": "GetJourneyExecutionMetrics",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard execution metric that applies to a journey",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey-execution-metrics"
             ]
         },
         "GetJourneyRunExecutionActivityMetrics": {
             "access_level": "Read",
             "action": "GetJourneyRunExecutionActivityMetrics",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard execution metric that applies to a journey activity for a single journey run",
             "orphan": false,
             "resources": [
-                "journeys"
+                "journey"
             ]
         },
         "GetJourneyRunExecutionMetrics": {
             "access_level": "Read",
             "action": "GetJourneyRunExecutionMetrics",
             "condition_keys": [],
             "description": "Grants permission to retrieve (queries) pre-aggregated data for a standard execution metric that applies to a journey for a single journey run",
             "orphan": false,
             "resources": [
-                "journeys"
+                "journey"
             ]
         },
         "GetJourneyRuns": {
             "access_level": "List",
             "action": "GetJourneyRuns",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about all journey runs for a journey",
             "orphan": false,
             "resources": [
-                "journeys"
+                "journey"
             ]
         },
         "GetPushTemplate": {
             "access_level": "Read",
             "action": "GetPushTemplate",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific or the active version of an push notification template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "GetRecommenderConfiguration": {
             "access_level": "Read",
             "action": "GetRecommenderConfiguration",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about an Amazon Pinpoint configuration for a recommender model",
             "orphan": false,
             "resources": [
-                "recommenders"
+                "recommender"
             ]
         },
         "GetRecommenderConfigurations": {
             "access_level": "List",
             "action": "GetRecommenderConfigurations",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about all the recommender model configurations that are associated with an Amazon Pinpoint account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "recommenders"
+            ]
         },
         "GetReports": {
             "access_level": "Read",
             "action": "GetReports",
             "condition_keys": [],
             "description": "Grants permission to mobiletargeting:GetReports",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "reports"
+            ]
         },
         "GetSegment": {
             "access_level": "Read",
             "action": "GetSegment",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific segment",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "GetSegmentExportJobs": {
             "access_level": "List",
             "action": "GetSegmentExportJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about jobs that export endpoint definitions from segments to Amazon S3",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "GetSegmentImportJobs": {
             "access_level": "List",
             "action": "GetSegmentImportJobs",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about jobs that create segments by importing endpoint definitions from",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "GetSegmentVersion": {
             "access_level": "Read",
             "action": "GetSegmentVersion",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific segment version",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "GetSegmentVersions": {
             "access_level": "List",
             "action": "GetSegmentVersions",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the current and prior versions of a segment",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "GetSegments": {
             "access_level": "List",
             "action": "GetSegments",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the segments for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "GetSmsChannel": {
             "access_level": "Read",
             "action": "GetSmsChannel",
             "condition_keys": [],
             "description": "Grants permission to obtain information about the SMS channel in an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetSmsTemplate": {
             "access_level": "Read",
             "action": "GetSmsTemplate",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific or the active version of an sms message template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "GetUserEndpoints": {
             "access_level": "Read",
             "action": "GetUserEndpoints",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about the endpoints that are associated with a user ID",
             "orphan": false,
             "resources": [
-                "apps"
+                "user"
             ]
         },
         "GetVoiceChannel": {
             "access_level": "Read",
             "action": "GetVoiceChannel",
             "condition_keys": [],
             "description": "Grants permission to obtain information about the Voice channel in an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "GetVoiceTemplate": {
             "access_level": "Read",
             "action": "GetVoiceTemplate",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about a specific or the active version of a voice message template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "ListJourneys": {
             "access_level": "List",
             "action": "ListJourneys",
             "condition_keys": [],
             "description": "Grants permission to retrieve information about all journeys for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "ListTagsForResource": {
             "access_level": "Read",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Grants permission to list tags for a resource",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns",
-                "segments"
+                "app",
+                "campaign",
+                "journey",
+                "segment",
+                "template"
             ]
         },
         "ListTemplateVersions": {
             "access_level": "List",
             "action": "ListTemplateVersions",
             "condition_keys": [],
             "description": "Grants permission to retrieve all versions about a specific template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "ListTemplates": {
             "access_level": "List",
             "action": "ListTemplates",
             "condition_keys": [],
             "description": "Grants permission to retrieve metadata about the queried templates",
@@ -98241,376 +98411,376 @@
         "PutEventStream": {
             "access_level": "Write",
             "action": "PutEventStream",
             "condition_keys": [],
             "description": "Grants permission to create or update an event stream for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "event-stream"
             ]
         },
         "PutEvents": {
             "access_level": "Write",
             "action": "PutEvents",
             "condition_keys": [],
             "description": "Grants permission to create or update events for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "events"
             ]
         },
         "RemoveAttributes": {
             "access_level": "Write",
             "action": "RemoveAttributes",
             "condition_keys": [],
             "description": "Grants permission to remove the attributes for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "attribute"
             ]
         },
         "SendMessages": {
             "access_level": "Write",
             "action": "SendMessages",
             "condition_keys": [],
             "description": "Grants permission to send an SMS message or push notification to specific endpoints",
             "orphan": false,
             "resources": [
-                "apps"
+                "messages"
             ]
         },
         "SendOTPMessage": {
             "access_level": "Write",
             "action": "SendOTPMessage",
             "condition_keys": [],
             "description": "Grants permission to send an OTP code to a user of your application",
             "orphan": false,
             "resources": [
-                "apps"
+                "otp"
             ]
         },
         "SendUsersMessages": {
             "access_level": "Write",
             "action": "SendUsersMessages",
             "condition_keys": [],
             "description": "Grants permission to send an SMS message or push notification to all endpoints that are associated with a specific user ID",
             "orphan": false,
             "resources": [
-                "apps"
+                "messages"
             ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to add tags to a resource",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns",
-                "segments"
+                "app",
+                "campaign",
+                "journey",
+                "segment",
+                "template"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to remove tags from a resource",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns",
-                "segments"
+                "app",
+                "campaign",
+                "journey",
+                "segment",
+                "template"
             ]
         },
         "UpdateAdmChannel": {
             "access_level": "Write",
             "action": "UpdateAdmChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Amazon Device Messaging (ADM) channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateApnsChannel": {
             "access_level": "Write",
             "action": "UpdateApnsChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Apple Push Notification service (APNs) channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateApnsSandboxChannel": {
             "access_level": "Write",
             "action": "UpdateApnsSandboxChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Apple Push Notification service (APNs) sandbox channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateApnsVoipChannel": {
             "access_level": "Write",
             "action": "UpdateApnsVoipChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Apple Push Notification service (APNs) VoIP channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateApnsVoipSandboxChannel": {
             "access_level": "Write",
             "action": "UpdateApnsVoipSandboxChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Apple Push Notification service (APNs) VoIP sandbox channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateApplicationSettings": {
             "access_level": "Write",
             "action": "UpdateApplicationSettings",
             "condition_keys": [],
             "description": "Grants permission to update the default settings for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "UpdateBaiduChannel": {
             "access_level": "Write",
             "action": "UpdateBaiduChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Baidu channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateCampaign": {
             "access_level": "Write",
             "action": "UpdateCampaign",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific campaign",
             "orphan": false,
             "resources": [
-                "apps",
-                "campaigns"
+                "campaign"
             ]
         },
         "UpdateEmailChannel": {
             "access_level": "Write",
             "action": "UpdateEmailChannel",
             "condition_keys": [],
             "description": "Grants permission to update the email channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateEmailTemplate": {
             "access_level": "Write",
             "action": "UpdateEmailTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific email template under the same version or generate a new version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "UpdateEndpoint": {
             "access_level": "Write",
             "action": "UpdateEndpoint",
             "condition_keys": [],
             "description": "Grants permission to create an endpoint or update the information for an endpoint",
             "orphan": false,
             "resources": [
-                "apps"
+                "endpoint"
             ]
         },
         "UpdateEndpointsBatch": {
             "access_level": "Write",
             "action": "UpdateEndpointsBatch",
             "condition_keys": [],
             "description": "Grants permission to create or update endpoints as a batch operation",
             "orphan": false,
             "resources": [
-                "apps"
+                "app"
             ]
         },
         "UpdateGcmChannel": {
             "access_level": "Write",
             "action": "UpdateGcmChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Firebase Cloud Messaging (FCM) or Google Cloud Messaging (GCM) API key that allows to send push notifications to your Android app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateInAppTemplate": {
             "access_level": "Write",
             "action": "UpdateInAppTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific in-app message template under the same version or generate a new version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "UpdateJourney": {
             "access_level": "Write",
             "action": "UpdateJourney",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific journey",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey"
             ]
         },
         "UpdateJourneyState": {
             "access_level": "Write",
             "action": "UpdateJourneyState",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific journey state",
             "orphan": false,
             "resources": [
-                "apps",
-                "journeys"
+                "journey"
             ]
         },
         "UpdatePushTemplate": {
             "access_level": "Write",
             "action": "UpdatePushTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific push notification template under the same version or generate a new version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "UpdateRecommenderConfiguration": {
             "access_level": "Write",
             "action": "UpdateRecommenderConfiguration",
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Pinpoint configuration for a recommender model",
             "orphan": false,
             "resources": [
-                "recommenders"
+                "recommender"
             ]
         },
         "UpdateSegment": {
             "access_level": "Write",
             "action": "UpdateSegment",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific segment",
             "orphan": false,
             "resources": [
-                "apps",
-                "segments"
+                "segment"
             ]
         },
         "UpdateSmsChannel": {
             "access_level": "Write",
             "action": "UpdateSmsChannel",
             "condition_keys": [],
             "description": "Grants permission to update the SMS channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateSmsTemplate": {
             "access_level": "Write",
             "action": "UpdateSmsTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific sms message template under the same version or generate a new version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "UpdateTemplateActiveVersion": {
             "access_level": "Write",
             "action": "UpdateTemplateActiveVersion",
             "condition_keys": [],
             "description": "Grants permission to update the active version parameter of a specific template",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "UpdateVoiceChannel": {
             "access_level": "Write",
             "action": "UpdateVoiceChannel",
             "condition_keys": [],
             "description": "Grants permission to update the Voice channel for an app",
             "orphan": false,
             "resources": [
-                "apps"
+                "channel"
             ]
         },
         "UpdateVoiceTemplate": {
             "access_level": "Write",
             "action": "UpdateVoiceTemplate",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to update a specific voice message template under the same version or generate a new version",
             "orphan": false,
             "resources": [
-                "templates"
+                "template"
             ]
         },
         "VerifyOTPMessage": {
             "access_level": "Write",
             "action": "VerifyOTPMessage",
             "condition_keys": [],
             "description": "Grants permission to check the validity of One-Time Passwords (OTPs)",
             "orphan": false,
             "resources": [
-                "apps"
+                "verify-otp"
             ]
         }
     },
     "monitron": {
         "AssociateProjectAdminUser": {
             "access_level": "Permissions management",
             "action": "AssociateProjectAdminUser",
```

### Comparing `iam_actions-1.2.20230428/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230429/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230429/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/generate/generate.py` & `iam_actions-1.2.20230429/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230429/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230429/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/generate/services.py` & `iam_actions-1.2.20230429/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230428/iam_actions/policies.json` & `iam_actions-1.2.20230429/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999980513494492%*

 * *Differences: {"'serviceMap'": "{'Amazon Athena': {'Actions': {insert: [(3, 'CancelCapacityReservation'), (4, "*

 * *                 "'CreateCapacityReservation'), (20, 'GetCapacityAssignmentConfiguration'), (21, "*

 * *                 "'GetCapacityReservation'), (38, 'ListCapacityReservations'), (52, "*

 * *                 "'PutCapacityAssignmentConfiguration'), (61, 'UpdateCapacityReservation')]}}, "*

 * *                 "'Amazon OpenSearch Service': {'Actions': {insert: [(29, "*

 * *                 "'DescribeDomainNodes')]}}, 'Amazon Ope […]*

```diff
@@ -9778,14 +9778,16 @@
         "Amazon Athena": {
             "ARNFormat": "arn:aws:athena:${Region}:${Account}:${ResourceType}/${ResourcePath}",
             "ARNRegex": "^arn:aws:athena:.+",
             "Actions": [
                 "BatchGetNamedQuery",
                 "BatchGetPreparedStatement",
                 "BatchGetQueryExecution",
+                "CancelCapacityReservation",
+                "CreateCapacityReservation",
                 "CreateDataCatalog",
                 "CreateNamedQuery",
                 "CreateNotebook",
                 "CreatePreparedStatement",
                 "CreatePresignedNotebookUrl",
                 "CreateWorkGroup",
                 "DeleteDataCatalog",
@@ -9793,14 +9795,16 @@
                 "DeleteNotebook",
                 "DeletePreparedStatement",
                 "DeleteWorkGroup",
                 "ExportNotebook",
                 "GetCalculationExecution",
                 "GetCalculationExecutionCode",
                 "GetCalculationExecutionStatus",
+                "GetCapacityAssignmentConfiguration",
+                "GetCapacityReservation",
                 "GetDataCatalog",
                 "GetDatabase",
                 "GetNamedQuery",
                 "GetNotebookMetadata",
                 "GetPreparedStatement",
                 "GetQueryExecution",
                 "GetQueryResults",
@@ -9809,35 +9813,38 @@
                 "GetSession",
                 "GetSessionStatus",
                 "GetTableMetadata",
                 "GetWorkGroup",
                 "ImportNotebook",
                 "ListApplicationDPUSizes",
                 "ListCalculationExecutions",
+                "ListCapacityReservations",
                 "ListDataCatalogs",
                 "ListDatabases",
                 "ListEngineVersions",
                 "ListExecutors",
                 "ListNamedQueries",
                 "ListNotebookMetadata",
                 "ListNotebookSessions",
                 "ListPreparedStatements",
                 "ListQueryExecutions",
                 "ListSessions",
                 "ListTableMetadata",
                 "ListTagsForResource",
                 "ListWorkGroups",
+                "PutCapacityAssignmentConfiguration",
                 "StartCalculationExecution",
                 "StartQueryExecution",
                 "StartSession",
                 "StopCalculationExecution",
                 "StopQueryExecution",
                 "TagResource",
                 "TerminateSession",
                 "UntagResource",
+                "UpdateCapacityReservation",
                 "UpdateDataCatalog",
                 "UpdateNamedQuery",
                 "UpdateNotebook",
                 "UpdateNotebookMetadata",
                 "UpdatePreparedStatement",
                 "UpdateWorkGroup"
             ],
@@ -15970,21 +15977,23 @@
                 "aws:TagKeys"
             ]
         },
         "Amazon OpenSearch Serverless": {
             "ARNFormat": "arn:aws:aoss:${Region}:${Account}:${Resource}",
             "ARNRegex": "^arn:aws:aoss:.+",
             "Actions": [
+                "APIAccessAll",
                 "BatchGetCollection",
                 "BatchGetVpcEndpoint",
                 "CreateAccessPolicy",
                 "CreateCollection",
                 "CreateSecurityConfig",
                 "CreateSecurityPolicy",
                 "CreateVpcEndpoint",
+                "DashboardsAccessAll",
                 "DeleteAccessPolicy",
                 "DeleteCollection",
                 "DeleteSecurityConfig",
                 "DeleteSecurityPolicy",
                 "DeleteVpcEndpoint",
                 "GetAccessPolicy",
                 "GetAccountSettings",
@@ -16046,14 +16055,15 @@
                 "DeletePackage",
                 "DeleteVpcEndpoint",
                 "DescribeDomain",
                 "DescribeDomainAutoTunes",
                 "DescribeDomainChangeProgress",
                 "DescribeDomainConfig",
                 "DescribeDomainHealth",
+                "DescribeDomainNodes",
                 "DescribeDomains",
                 "DescribeDryRunProgress",
                 "DescribeElasticsearchDomain",
                 "DescribeElasticsearchDomainConfig",
                 "DescribeElasticsearchDomains",
                 "DescribeElasticsearchInstanceTypeLimits",
                 "DescribeInboundConnections",
```

### Comparing `iam_actions-1.2.20230428/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230429/iam_actions/resourcetypes.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998463632764934%*

 * *Differences: {"'connect'": "{'evaluation-form': OrderedDict([('arn_pattern', "*

 * *              "'arn:*:connect:*:*:instance/*/evaluation-form/*'), ('condition_keys', "*

 * *              "'aws:ResourceTag/${TagKey}')]), 'contact-evaluation': OrderedDict([('arn_pattern', "*

 * *              "'arn:*:connect:*:*:instance/*/contact-evaluation/*'), ('condition_keys', "*

 * *              "'aws:ResourceTag/${TagKey}')])}",*

 * * "'kafka'": "{'vpc-connection': OrderedDict([('arn_pattern', "*

 * *            "'arn:*:kafka:*:*:vpc-connection/*/*/*'), ('c […]*

```diff
@@ -1356,22 +1356,30 @@
             "arn_pattern": "arn:*:connect:*:*:instance/*/agent-state/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "contact": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/contact/*",
             "condition_keys": null
         },
+        "contact-evaluation": {
+            "arn_pattern": "arn:*:connect:*:*:instance/*/contact-evaluation/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "contact-flow": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/contact-flow/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "contact-flow-module": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/flow-module/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "evaluation-form": {
+            "arn_pattern": "arn:*:connect:*:*:instance/*/evaluation-form/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
         "hierarchy-group": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/agent-group/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "hours-of-operation": {
             "arn_pattern": "arn:*:connect:*:*:instance/*/operating-hours/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
@@ -3631,14 +3639,18 @@
         "topic": {
             "arn_pattern": "arn:*:kafka:*:*:topic/*/*/*",
             "condition_keys": null
         },
         "transactional-id": {
             "arn_pattern": "arn:*:kafka:*:*:transactional-id/*/*/*",
             "condition_keys": null
+        },
+        "vpc-connection": {
+            "arn_pattern": "arn:*:kafka:*:*:vpc-connection/*/*/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "kafka-cluster": {
         "cluster": {
             "arn_pattern": "arn:*:kafka:*:*:cluster/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
@@ -4265,41 +4277,129 @@
     "mobilehub": {
         "project": {
             "arn_pattern": "arn:*:mobilehub:*:*:project/*",
             "condition_keys": null
         }
     },
     "mobiletargeting": {
-        "apps": {
+        "app": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
-        "campaigns": {
+        "application-metrics": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/kpis/daterange/*",
+            "condition_keys": null
+        },
+        "apps": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*",
+            "condition_keys": null
+        },
+        "attribute": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/attributes/*",
+            "condition_keys": null
+        },
+        "campaign": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/campaigns/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
-        "journeys": {
+        "campaign-metrics": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/campaigns/*/kpis/daterange/*",
+            "condition_keys": null
+        },
+        "channel": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/channels/*",
+            "condition_keys": null
+        },
+        "channels": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/channels",
+            "condition_keys": null
+        },
+        "endpoint": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/endpoints/*",
+            "condition_keys": null
+        },
+        "event-stream": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/eventstream",
+            "condition_keys": null
+        },
+        "events": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/events",
+            "condition_keys": null
+        },
+        "export-job": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/jobs/export/*",
+            "condition_keys": null
+        },
+        "import-job": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/jobs/import/*",
+            "condition_keys": null
+        },
+        "journey": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/journeys/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
+        "journey-execution-activity-metrics": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/journeys/*/activities/*/execution-metrics",
+            "condition_keys": null
+        },
+        "journey-execution-metrics": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/journeys/*/execution-metrics",
+            "condition_keys": null
+        },
+        "journey-metrics": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/journeys/*/kpis/daterange/*",
+            "condition_keys": null
+        },
+        "journeys": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/journeys",
+            "condition_keys": null
+        },
+        "messages": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/messages",
+            "condition_keys": null
+        },
+        "otp": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/otp",
+            "condition_keys": null
+        },
         "phone-number-validate": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:phone/number/validate",
             "condition_keys": null
         },
+        "recommender": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:recommenders/*",
+            "condition_keys": null
+        },
         "recommenders": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:recommenders/*",
             "condition_keys": null
         },
-        "segments": {
+        "reports": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:reports",
+            "condition_keys": null
+        },
+        "segment": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/segments/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
-        "templates": {
+        "template": {
             "arn_pattern": "arn:*:mobiletargeting:*:*:templates/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "templates": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:templates",
+            "condition_keys": null
+        },
+        "user": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/users/*",
+            "condition_keys": null
+        },
+        "verify-otp": {
+            "arn_pattern": "arn:*:mobiletargeting:*:*:apps/*/verify-otp",
+            "condition_keys": null
         }
     },
     "monitron": {
         "project": {
             "arn_pattern": "arn:*:monitron:*:*:project/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
```

### Comparing `iam_actions-1.2.20230428/iam_actions/services.json` & `iam_actions-1.2.20230429/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999795855656584%*

 * *Differences: {"'aoss'": "{'Actions': {insert: [(0, 'APIAccessAll'), (8, 'DashboardsAccessAll')]}}",*

 * * "'athena'": "{'Actions': {insert: [(3, 'CancelCapacityReservation'), (4, "*

 * *             "'CreateCapacityReservation'), (20, 'GetCapacityAssignmentConfiguration'), (21, "*

 * *             "'GetCapacityReservation'), (38, 'ListCapacityReservations'), (52, "*

 * *             "'PutCapacityAssignmentConfiguration'), (61, 'UpdateCapacityReservation')]}}",*

 * * "'es'": "{'Actions': {insert: [(29, 'DescribeDomainNodes')]}}"}*

```diff
@@ -496,21 +496,23 @@
         "ARNFormats": [
             "arn:aws:aoss:${Region}:${Account}:${Resource}"
         ],
         "ARNRegexes": [
             "^arn:aws:aoss:.+"
         ],
         "Actions": [
+            "APIAccessAll",
             "BatchGetCollection",
             "BatchGetVpcEndpoint",
             "CreateAccessPolicy",
             "CreateCollection",
             "CreateSecurityConfig",
             "CreateSecurityPolicy",
             "CreateVpcEndpoint",
+            "DashboardsAccessAll",
             "DeleteAccessPolicy",
             "DeleteCollection",
             "DeleteSecurityConfig",
             "DeleteSecurityPolicy",
             "DeleteVpcEndpoint",
             "GetAccessPolicy",
             "GetAccountSettings",
@@ -1298,14 +1300,16 @@
         "ARNRegexes": [
             "^arn:aws:athena:.+"
         ],
         "Actions": [
             "BatchGetNamedQuery",
             "BatchGetPreparedStatement",
             "BatchGetQueryExecution",
+            "CancelCapacityReservation",
+            "CreateCapacityReservation",
             "CreateDataCatalog",
             "CreateNamedQuery",
             "CreateNotebook",
             "CreatePreparedStatement",
             "CreatePresignedNotebookUrl",
             "CreateWorkGroup",
             "DeleteDataCatalog",
@@ -1313,14 +1317,16 @@
             "DeleteNotebook",
             "DeletePreparedStatement",
             "DeleteWorkGroup",
             "ExportNotebook",
             "GetCalculationExecution",
             "GetCalculationExecutionCode",
             "GetCalculationExecutionStatus",
+            "GetCapacityAssignmentConfiguration",
+            "GetCapacityReservation",
             "GetDataCatalog",
             "GetDatabase",
             "GetNamedQuery",
             "GetNotebookMetadata",
             "GetPreparedStatement",
             "GetQueryExecution",
             "GetQueryResults",
@@ -1329,35 +1335,38 @@
             "GetSession",
             "GetSessionStatus",
             "GetTableMetadata",
             "GetWorkGroup",
             "ImportNotebook",
             "ListApplicationDPUSizes",
             "ListCalculationExecutions",
+            "ListCapacityReservations",
             "ListDataCatalogs",
             "ListDatabases",
             "ListEngineVersions",
             "ListExecutors",
             "ListNamedQueries",
             "ListNotebookMetadata",
             "ListNotebookSessions",
             "ListPreparedStatements",
             "ListQueryExecutions",
             "ListSessions",
             "ListTableMetadata",
             "ListTagsForResource",
             "ListWorkGroups",
+            "PutCapacityAssignmentConfiguration",
             "StartCalculationExecution",
             "StartQueryExecution",
             "StartSession",
             "StopCalculationExecution",
             "StopQueryExecution",
             "TagResource",
             "TerminateSession",
             "UntagResource",
+            "UpdateCapacityReservation",
             "UpdateDataCatalog",
             "UpdateNamedQuery",
             "UpdateNotebook",
             "UpdateNotebookMetadata",
             "UpdatePreparedStatement",
             "UpdateWorkGroup"
         ],
@@ -7883,14 +7892,15 @@
             "DeletePackage",
             "DeleteVpcEndpoint",
             "DescribeDomain",
             "DescribeDomainAutoTunes",
             "DescribeDomainChangeProgress",
             "DescribeDomainConfig",
             "DescribeDomainHealth",
+            "DescribeDomainNodes",
             "DescribeDomains",
             "DescribeDryRunProgress",
             "DescribeElasticsearchDomain",
             "DescribeElasticsearchDomainConfig",
             "DescribeElasticsearchDomains",
             "DescribeElasticsearchInstanceTypeLimits",
             "DescribeInboundConnections",
```

### Comparing `iam_actions-1.2.20230428/pyproject.toml` & `iam_actions-1.2.20230429/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230428"
+version = "1.2.20230429"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230428/setup.py` & `iam_actions-1.2.20230429/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230428',
+    'version': '1.2.20230429',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230428/PKG-INFO` & `iam_actions-1.2.20230429/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230428
+Version: 1.2.20230429
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

