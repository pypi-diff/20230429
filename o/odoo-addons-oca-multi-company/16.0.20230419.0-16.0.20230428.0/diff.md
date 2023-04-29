# Comparing `tmp/odoo_addons_oca_multi_company-16.0.20230419.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_multi_company-16.0.20230428.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1433 bytes, number of entries: 4
--rw-r--r--  2.0 unx      542 b- defN 23-Apr-19 05:28 odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 05:28 odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-19 05:28 odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      424 b- defN 23-Apr-19 05:28 odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/RECORD
-4 files, 1059 bytes uncompressed, 595 bytes compressed:  43.8%
+Zip file size: 1443 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      614 b- defN 23-Apr-29 05:24 odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 05:24 odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-29 05:24 odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      424 b- defN 23-Apr-29 05:24 odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/RECORD
+4 files, 1131 bytes uncompressed, 605 bytes compressed:  46.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/METADATA
+Filename: odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/WHEEL
+Filename: odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/RECORD
+Filename: odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_multi_company-16.0.20230419.0.dist-info/METADATA` & `odoo_addons_oca_multi_company-16.0.20230428.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-multi-company
-Version: 16.0.20230419.0
+Version: 16.0.20230428.0
 Summary: Meta package for oca-multi-company Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-account-invoice-inter-company (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-product-category-company (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-product-tax-multicompany-default (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-res-company-search-view (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

