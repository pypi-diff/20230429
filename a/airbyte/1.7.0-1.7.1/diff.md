# Comparing `tmp/airbyte-1.7.0.tar.gz` & `tmp/airbyte-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-1.7.0.tar", last modified: Fri Apr 28 00:47:53 2023, max compression
+gzip compressed data, was "airbyte-1.7.1.tar", last modified: Sat Apr 29 00:44:59 2023, max compression
```

## Comparing `airbyte-1.7.0.tar` & `airbyte-1.7.1.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.839788 airbyte-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-28 00:47:41.000000 airbyte-1.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-28 00:47:53.839788 airbyte-1.7.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6503 2023-04-28 00:47:41.000000 airbyte-1.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 00:47:53.839788 airbyte-1.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1092 2023-04-28 00:47:41.000000 airbyte-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.803788 airbyte-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.807788 airbyte-1.7.0/src/airbyte/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4743 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/destinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4852 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/jobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.807788 airbyte-1.7.0/src/airbyte/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.807788 airbyte-1.7.0/src/airbyte/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/canceljob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      648 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/createconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/createdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      686 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/createjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/createsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/createworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/deleteconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/deletedestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      621 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/deletesource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      866 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/getconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      876 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/getdestination.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      796 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/getjob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      826 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/getsource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1087 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/getstreamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/getworkspace.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1699 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/listconnections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1710 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/listdestinations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1609 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/listjobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1655 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/listsources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1674 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/operations/listworkspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.839788 airbyte-1.7.0/src/airbyte/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)    49282 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3221 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectioncreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1849 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectionresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectionschedulecreate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectionscheduleresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      958 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectionsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectionstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3470 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9280 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_aws_datalake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4621 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12163 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10913 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_bigquery_denormalized.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_cassandra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6155 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_convex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1805 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_databend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_databricks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2758 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_elasticsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3763 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1340 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_firestore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21064 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2050 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1438 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_keen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1848 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_kinesis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6303 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_mariadb_columnstore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_meilisearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9207 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8131 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6070 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6770 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11145 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2751 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_pubsub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5813 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_pulsar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2242 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_rabbitmq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8038 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_redis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13990 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1231 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_rockset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18907 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8944 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_s3_glue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1724 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_scylla.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1591 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_sftp_json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16090 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1772 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destination_typesense.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      784 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destinationcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destinationresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      823 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/destinationsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/geographyenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/jobcreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/jobresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      797 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/jobsresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/jobstatusenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/jobtypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/scheduletypeenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      334 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3381 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_airtable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7512 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_alloydb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4949 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_amazon_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5155 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_amazon_seller_partner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3925 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_amazon_sqs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2384 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_amplitude.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_apify_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2787 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_asana.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3317 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_auth0.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2024 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_aws_cloudtrail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3052 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_azure_blob_storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1583 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_azure_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1626 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_bamboo_hr.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_bigcommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1581 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_bigquery.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2747 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_bing_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2513 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_braintree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1241 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_braze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2235 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_chargebee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2017 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_chartmogul.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5721 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_clickhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2902 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_clickup_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1375 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_close_com.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      736 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_coda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_coin_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2056 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_coinmarketcap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1097 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_configcat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1292 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_confluence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      939 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_datascope.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1166 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_delighted.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1206 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_dixa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_dockerhub.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_dremio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_dynamodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4290 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_e2e_test_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_emailoctopus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1969 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_exchange_rates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17577 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_facebook_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      959 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_facebook_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2135 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_faker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4615 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_fauna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10292 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_file_secure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1789 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_firebolt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2012 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_freshcaller.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1965 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_freshdesk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_freshsales.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_gcs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_getlago.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4331 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_github.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4138 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_gitlab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      782 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_glassfrog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_gnews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5971 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5200 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_analytics_data_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4958 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_analytics_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1228 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_directory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5221 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_search_console.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_sheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1592 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_webfonts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_greenhouse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      891 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_gridly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_harvest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_hubplanner.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3659 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_hubspot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_insightly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_instagram.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      767 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_instatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1420 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_intercom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_ip2whois.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1401 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_iterable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3231 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_jira.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      860 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_k6_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1919 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_klarna.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1329 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_klaviyo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_kustomer_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_launchdarkly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      755 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_lemlist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3573 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_linkedin_ads.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3001 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_linkedin_pages.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1545 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_linnworks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1109 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_lokalise.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2737 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mailchimp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1646 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mailgun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1469 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mailjet_sms.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1968 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_marketo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_metabase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4239 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_microsoft_teams.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6239 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mixpanel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2579 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_monday.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4408 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mongodb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12204 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mssql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_my_hours.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12826 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_mysql.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_netsuite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3014 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_notion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2245 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_nytimes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2997 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_okta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_omnisend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2687 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_onesignal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3397 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_openweather.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10203 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_oracle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2756 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_orb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1323 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_orbit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1807 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_outreach.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1983 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_paypal_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1745 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_paystack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pendo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_persistiq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2544 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pexels_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3230 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pinterest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1954 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pipedrive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3908 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pocket.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pokeapi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2971 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_polygon_stock_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7531 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_postgres.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1620 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_posthog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1003 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_postmarkapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1464 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_prestashop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      629 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_public_apis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_punk_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1172 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_pypi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1809 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_qualaroo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3532 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_quickbooks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1061 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_railz.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_recharge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_recreation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1157 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_recruitee.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1496 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_recurly.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2259 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_redshift.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_retently.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      838 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_rki_covid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_rss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13300 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_s3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3775 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_salesforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_salesforce_singer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_salesloft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sap_fieldglass.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_secoda.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1365 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sendgrid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      856 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sendinblue.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3347 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_senseforce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1958 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sentry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3641 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sftp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3465 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sftp_bulk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3207 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_shopify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1131 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_shortio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4276 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_slack.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_smaily.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_smartengage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4171 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_smartsheets.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_snapchat_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4397 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_snowflake.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2200 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_sonar_cloud.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      994 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_spacex_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3703 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_square.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2096 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_strava.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2523 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_stripe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2696 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_survey_sparrow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3729 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_surveymonkey.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_tempo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2974 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_the_guardian_api.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4457 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_tiktok_marketing.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_todoist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_trello.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3841 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_trustpilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1792 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_tvmaze_schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1657 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_twilio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_twilio_taskrouter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2173 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_twitter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1785 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_typeform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_us_census.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      850 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_vantage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_webflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      643 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_whisky_hunter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2395 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_wikipedia_pageviews.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_woocommerce.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2460 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_xero.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      585 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_xkcd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_yandex_metrica.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_younium.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      834 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_youtube_analytics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3556 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_chat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3139 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_sunshine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2062 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_support.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1783 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_talk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zenloop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3094 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zoho_crm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      731 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zoom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1700 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/source_zuora.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1046 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/sourcecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      857 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/sourceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/sourcesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1594 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/streamconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/streamconfigurations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1772 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/streamproperties.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      468 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/workspacecreaterequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/workspaceresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      813 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/models/shared/workspacesresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4628 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/sources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1838 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.839788 airbyte-1.7.0/src/airbyte/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/utils/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-28 00:47:41.000000 airbyte-1.7.0/src/airbyte/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 00:47:53.807788 airbyte-1.7.0/src/airbyte.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-28 00:47:53.000000 airbyte-1.7.0/src/airbyte.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-04-28 00:47:53.000000 airbyte-1.7.0/src/airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 00:47:53.000000 airbyte-1.7.0/src/airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-28 00:47:53.000000 airbyte-1.7.0/src/airbyte.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 00:47:53.000000 airbyte-1.7.0/src/airbyte.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.847635 airbyte-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-29 00:44:48.000000 airbyte-1.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-29 00:44:59.847635 airbyte-1.7.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6503 2023-04-29 00:44:48.000000 airbyte-1.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 00:44:59.847635 airbyte-1.7.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1092 2023-04-29 00:44:48.000000 airbyte-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.811633 airbyte-1.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.815634 airbyte-1.7.1/src/airbyte/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4743 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4813 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/destinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4852 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/jobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.815634 airbyte-1.7.1/src/airbyte/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.815634 airbyte-1.7.1/src/airbyte/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1490 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/canceljob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/createconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      650 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/createdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      682 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/createjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      620 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/createsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      638 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/createworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      633 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/deleteconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      637 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/deletedestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      617 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/deletesource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      861 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/getconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/getdestination.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      791 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/getjob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      821 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/getsource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1081 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/getstreamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/getworkspace.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1691 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/listconnections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/listdestinations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1601 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/listjobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1647 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/listsources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1666 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/operations/listworkspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.847635 airbyte-1.7.1/src/airbyte/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49282 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3212 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectioncreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectionresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectionschedulecreate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1098 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectionscheduleresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      955 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      255 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectionstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      391 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/connectionsyncmodeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3462 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9258 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_aws_datalake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4610 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12146 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10897 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_bigquery_denormalized.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_cassandra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6136 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_convex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1798 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_databend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8016 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_databricks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2752 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_elasticsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3749 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_firestore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21027 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2044 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1434 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_keen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1841 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_kinesis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6284 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_mariadb_columnstore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_meilisearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9179 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8107 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6051 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6750 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11112 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_pubsub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5795 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_pulsar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_rabbitmq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8012 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_redis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13955 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1227 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_rockset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18868 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8927 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_s3_glue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1717 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_scylla.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1585 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_sftp_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16047 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destination_typesense.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      781 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destinationcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      883 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destinationresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/destinationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      216 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/geographyenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/jobcreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/jobresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/jobsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/jobstatusenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      289 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/jobtypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      213 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/scheduletypeenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      242 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/scheduletypewithbasicenum_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      333 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3371 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_airtable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7489 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_alloydb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4938 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_amazon_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5139 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_amazon_seller_partner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3915 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_amazon_sqs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2378 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_amplitude.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1295 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_apify_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2779 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_asana.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3308 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_auth0.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2019 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_aws_cloudtrail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3043 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_azure_blob_storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_azure_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1621 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_bamboo_hr.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_bigcommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1577 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_bigquery.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2739 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_bing_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_braintree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1237 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_braze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_chargebee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_chartmogul.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5703 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_clickhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2895 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_clickup_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1372 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_close_com.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_coda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2568 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_coin_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2052 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_coinmarketcap.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1094 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_configcat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_confluence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_datascope.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1163 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_delighted.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_dixa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_dockerhub.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      952 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_dremio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2742 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_dynamodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4278 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_e2e_test_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      945 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_emailoctopus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1964 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_exchange_rates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17556 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_facebook_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_facebook_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2129 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_faker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4604 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_fauna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10260 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_file_secure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_firebolt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2006 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_freshcaller.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1960 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_freshdesk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1103 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_freshsales.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1207 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_gcs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_getlago.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4321 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_github.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4124 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_gitlab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_glassfrog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9609 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_gnews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5956 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5187 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_analytics_data_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4945 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_analytics_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_directory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5207 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_search_console.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3260 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_sheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1587 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_webfonts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_google_workspace_admin_reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      915 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_greenhouse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      888 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_gridly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_harvest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_hubplanner.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3650 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_hubspot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1119 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_insightly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1582 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_instagram.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      765 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_instatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_intercom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1175 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_ip2whois.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1398 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_iterable.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3222 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_jira.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      858 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_k6_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_klarna.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1326 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_klaviyo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1128 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_kustomer_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_launchdarkly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      753 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_lemlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3563 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_linkedin_ads.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_linkedin_pages.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1540 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_linnworks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_lokalise.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2728 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mailchimp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mailgun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mailjet_sms.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1963 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_marketo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1819 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_metabase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4227 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_microsoft_teams.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6224 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mixpanel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_monday.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4394 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mongodb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12174 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mssql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1383 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_my_hours.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12789 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_mysql.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2469 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_netsuite.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3005 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_notion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2239 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_nytimes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2987 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_okta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_omnisend.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2679 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_onesignal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3391 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_openweather.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_oracle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2748 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_orb.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1319 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_orbit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1801 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_outreach.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1977 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_paypal_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1741 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_paystack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      711 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pendo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      894 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_persistiq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2537 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pexels_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3220 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pinterest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1949 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pipedrive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3896 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pocket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      778 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pokeapi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2961 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_polygon_stock_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7508 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_postgres.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1616 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_posthog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1000 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_postmarkapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_prestashop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_public_apis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1216 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_punk_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1169 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_pypi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1804 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_qualaroo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3521 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_quickbooks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_railz.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_recharge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_recreation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1154 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_recruitee.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1492 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_recurly.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_redshift.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_retently.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      836 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_rki_covid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_rss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13269 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_s3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3765 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_salesforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3502 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_salesforce_singer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3530 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_salesloft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      788 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sap_fieldglass.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_secoda.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1362 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sendgrid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      854 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sendinblue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_senseforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sentry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sftp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3453 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sftp_bulk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3197 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_shopify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1127 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_shortio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4264 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_slack.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_smaily.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      772 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_smartengage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4159 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_smartsheets.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2123 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_snapchat_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4381 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_snowflake.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2194 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_sonar_cloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      991 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_spacex_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_square.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_strava.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2517 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_stripe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2690 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_survey_sparrow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3720 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_surveymonkey.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      820 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_tempo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2967 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_the_guardian_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4444 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_tiktok_marketing.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      852 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_todoist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2013 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_trello.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3829 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_trustpilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1787 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_tvmaze_schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1652 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_twilio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_twilio_taskrouter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2168 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_twitter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1781 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_typeform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1307 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_us_census.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      848 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_vantage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1078 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_webflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      642 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_whisky_hunter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_wikipedia_pageviews.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_woocommerce.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2451 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_xero.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      584 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_xkcd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_yandex_metrica.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1437 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_younium.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      832 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_youtube_analytics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_chat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3128 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_sunshine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2057 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_support.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1779 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_talk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1879 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zenloop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3086 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zoho_crm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zoom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1694 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/source_zuora.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/sourcecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/sourceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/sourcesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1590 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/streamconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/streamconfigurations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1766 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/streamproperties.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      467 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/workspacecreaterequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/workspaceresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/models/shared/workspacesresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3591 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4628 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/sources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1838 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.847635 airbyte-1.7.1/src/airbyte/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25535 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/utils/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4056 2023-04-29 00:44:48.000000 airbyte-1.7.1/src/airbyte/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 00:44:59.815634 airbyte-1.7.1/src/airbyte.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-04-29 00:44:59.000000 airbyte-1.7.1/src/airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-04-29 00:44:59.000000 airbyte-1.7.1/src/airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 00:44:59.000000 airbyte-1.7.1/src/airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-29 00:44:59.000000 airbyte-1.7.1/src/airbyte.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-29 00:44:59.000000 airbyte-1.7.1/src/airbyte.egg-info/top_level.txt
```

### Comparing `airbyte-1.7.0/LICENSE.md` & `airbyte-1.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/PKG-INFO` & `airbyte-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airbyte Version: 1.7.0 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: airbyte Version: 1.7.1 Summary: Python Client SDK
 for Airbyte API Home-page: UNKNOWN Author: Speakeasy License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown License-
 File: LICENSE.md
  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
                           4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
```

### Comparing `airbyte-1.7.0/README.md` & `airbyte-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/setup.py` & `airbyte-1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="airbyte",
-    version="1.7.0",
+    version="1.7.1",
     author="Speakeasy",
     description="Python Client SDK for Airbyte API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.7",
```

### Comparing `airbyte-1.7.0/src/airbyte/connections.py` & `airbyte-1.7.1/src/airbyte/connections.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/destinations.py` & `airbyte-1.7.1/src/airbyte/destinations.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/jobs.py` & `airbyte-1.7.1/src/airbyte/jobs.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/__init__.py` & `airbyte-1.7.1/src/airbyte/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/canceljob.py` & `airbyte-1.7.1/src/airbyte/models/operations/canceljob.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CancelJobRequest:
     
     job_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'jobId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class CancelJobResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     job_response: Optional[shared_jobresponse.JobResponse] = dataclasses.field(default=None)
-
     r"""Cancel a Job."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/createconnection.py` & `airbyte-1.7.1/src/airbyte/models/operations/createconnection.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,12 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateConnectionResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     connection_response: Optional[shared_connectionresponse.ConnectionResponse] = dataclasses.field(default=None)
-
     r"""Successful operation"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/createdestination.py` & `airbyte-1.7.1/src/airbyte/models/operations/createsource.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import destinationresponse as shared_destinationresponse
+from ..shared import sourceresponse as shared_sourceresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateDestinationResponse:
+class CreateSourceResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
-    destination_response: Optional[shared_destinationresponse.DestinationResponse] = dataclasses.field(default=None)
-
-    r"""Successful operation"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
+    source_response: Optional[shared_sourceresponse.SourceResponse] = dataclasses.field(default=None)
+    r"""Successful operation"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/createjob.py` & `airbyte-1.7.1/src/airbyte/models/operations/createjob.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,16 +7,12 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateJobResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     job_response: Optional[shared_jobresponse.JobResponse] = dataclasses.field(default=None)
-
     r"""Kicks off a new Job based on the JobType. The connectionId is the resource that Job will be run for."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/createsource.py` & `airbyte-1.7.1/src/airbyte/models/operations/getsource.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 import dataclasses
 import requests as requests_http
 from ..shared import sourceresponse as shared_sourceresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateSourceResponse:
+class GetSourceRequest:
+    
+    source_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'sourceId', 'style': 'simple', 'explode': False }})
     
-    content_type: str = dataclasses.field()
 
+@dataclasses.dataclass
+class GetSourceResponse:
+    
+    content_type: str = dataclasses.field()
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     source_response: Optional[shared_sourceresponse.SourceResponse] = dataclasses.field(default=None)
-
-    r"""Successful operation"""
+    r"""Get a Source by the id in the path."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/createworkspace.py` & `airbyte-1.7.1/src/airbyte/models/operations/createworkspace.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,12 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class CreateWorkspaceResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     workspace_response: Optional[shared_workspaceresponse.WorkspaceResponse] = dataclasses.field(default=None)
-
     r"""Successful operation"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/deleteconnection.py` & `airbyte-1.7.1/src/airbyte/models/operations/deleteconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,16 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteConnectionRequest:
     
     connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class DeleteConnectionResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/deletedestination.py` & `airbyte-1.7.1/src/airbyte/models/operations/deletedestination.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,20 +6,16 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteDestinationRequest:
     
     destination_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'destinationId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class DeleteDestinationResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/deletesource.py` & `airbyte-1.7.1/src/airbyte/models/operations/deletesource.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,16 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class DeleteSourceRequest:
     
     source_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'sourceId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class DeleteSourceResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/getconnection.py` & `airbyte-1.7.1/src/airbyte/models/operations/getconnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetConnectionRequest:
     
     connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetConnectionResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     connection_response: Optional[shared_connectionresponse.ConnectionResponse] = dataclasses.field(default=None)
-
     r"""Get a Connection by the id in the path."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/getdestination.py` & `airbyte-1.7.1/src/airbyte/models/operations/getdestination.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetDestinationRequest:
     
     destination_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'destinationId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetDestinationResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     destination_response: Optional[shared_destinationresponse.DestinationResponse] = dataclasses.field(default=None)
-
     r"""Get a Destination by the id in the path."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/getjob.py` & `airbyte-1.7.1/src/airbyte/models/operations/getjob.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetJobRequest:
     
     job_id: int = dataclasses.field(metadata={'path_param': { 'field_name': 'jobId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetJobResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     job_response: Optional[shared_jobresponse.JobResponse] = dataclasses.field(default=None)
-
     r"""Get a Job by the id in the path."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/getsource.py` & `airbyte-1.7.1/src/airbyte/models/operations/createdestination.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from ..shared import sourceresponse as shared_sourceresponse
+from ..shared import destinationresponse as shared_destinationresponse
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetSourceRequest:
-    
-    source_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'sourceId', 'style': 'simple', 'explode': False }})
-
-    
-
-@dataclasses.dataclass
-class GetSourceResponse:
+class CreateDestinationResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
+    destination_response: Optional[shared_destinationresponse.DestinationResponse] = dataclasses.field(default=None)
+    r"""Successful operation"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
-    source_response: Optional[shared_sourceresponse.SourceResponse] = dataclasses.field(default=None)
-
-    r"""Get a Source by the id in the path."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/getstreamproperties.py` & `airbyte-1.7.1/src/airbyte/models/operations/getstreamproperties.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,21 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetStreamPropertiesRequest:
     
     destination_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'destinationId', 'style': 'form', 'explode': True }})
-
     r"""ID of the destination"""
     source_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'sourceId', 'style': 'form', 'explode': True }})
-
     r"""ID of the source"""
     
 
 @dataclasses.dataclass
 class GetStreamPropertiesResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     stream_properties: Optional[shared_streamproperties.StreamProperties] = dataclasses.field(default=None)
-
     r"""Get the available streams properties for a source/destination pair."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/getworkspace.py` & `airbyte-1.7.1/src/airbyte/models/operations/getworkspace.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,23 +7,18 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class GetWorkspaceRequest:
     
     workspace_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'workspaceId', 'style': 'simple', 'explode': False }})
-
     
 
 @dataclasses.dataclass
 class GetWorkspaceResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     workspace_response: Optional[shared_workspaceresponse.WorkspaceResponse] = dataclasses.field(default=None)
-
     r"""Get a Workspace by the id in the path."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/listconnections.py` & `airbyte-1.7.1/src/airbyte/models/operations/listconnections.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,33 +7,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListConnectionsRequest:
     
     include_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'includeDeleted', 'style': 'form', 'explode': True }})
-
     r"""Include deleted connections in the returned results."""
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-
     r"""Set the limit on the number of Connections returned. The default is 20."""
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-
     r"""Set the offset to start at when returning Connections. The default is 0"""
     workspace_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'workspaceIds', 'style': 'form', 'explode': True }})
-
     r"""The UUIDs of the workspaces you wish to list connections for. Empty list will retrieve all allowed workspaces."""
     
 
 @dataclasses.dataclass
 class ListConnectionsResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     connections_response: Optional[shared_connectionsresponse.ConnectionsResponse] = dataclasses.field(default=None)
-
     r"""Successful operation"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/listdestinations.py` & `airbyte-1.7.1/src/airbyte/models/operations/listdestinations.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListDestinationsRequest:
     
     include_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'includeDeleted', 'style': 'form', 'explode': True }})
-
     r"""Include deleted destinations in the returned results."""
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-
     r"""Set the limit on the number of destinations returned. The default is 20."""
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-
     r"""Set the offset to start at when returning destinations. The default is 0"""
     workspace_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'workspaceIds', 'style': 'form', 'explode': True }})
-
     r"""The UUIDs of the workspaces you wish to list destinations for. Empty list will retrieve all allowed workspaces."""
     
 
 @dataclasses.dataclass
 class ListDestinationsResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     destinations_response: Optional[shared_destinationsresponse.DestinationsResponse] = dataclasses.field(default=None)
-
     r"""Successful operation"""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/listjobs.py` & `airbyte-1.7.1/src/airbyte/models/operations/listjobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListJobsRequest:
     
     connection_id: str = dataclasses.field(metadata={'query_param': { 'field_name': 'connectionId', 'style': 'form', 'explode': True }})
-
     r"""Filter the Jobs by connectionId."""
     job_type: Optional[shared_jobtypeenum_enum.JobTypeEnumEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'jobType', 'style': 'form', 'explode': True }})
-
     r"""Filter the Jobs by jobType."""
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-
     r"""Set the limit on the number of Jobs returned. The default is 20 Jobs."""
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-
     r"""Set the offset to start at when returning Jobs. The default is 0."""
     
 
 @dataclasses.dataclass
 class ListJobsResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     jobs_response: Optional[shared_jobsresponse.JobsResponse] = dataclasses.field(default=None)
-
     r"""List all the Jobs by connectionId."""
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/listsources.py` & `airbyte-1.7.1/src/airbyte/models/operations/listsources.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,33 +7,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListSourcesRequest:
     
     include_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'includeDeleted', 'style': 'form', 'explode': True }})
-
     r"""Include deleted sources in the returned results."""
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-
     r"""Set the limit on the number of sources returned. The default is 20."""
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-
     r"""Set the offset to start at when returning sources. The default is 0"""
     workspace_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'workspaceIds', 'style': 'form', 'explode': True }})
-
     r"""The UUIDs of the workspaces you wish to list sources for. Empty list will retrieve all allowed workspaces."""
     
 
 @dataclasses.dataclass
 class ListSourcesResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     sources_response: Optional[shared_sourcesresponse.SourcesResponse] = dataclasses.field(default=None)
-
     r"""Successful operation"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/operations/listworkspaces.py` & `airbyte-1.7.1/src/airbyte/models/operations/listworkspaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,33 +7,25 @@
 from typing import Optional
 
 
 @dataclasses.dataclass
 class ListWorkspacesRequest:
     
     include_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'includeDeleted', 'style': 'form', 'explode': True }})
-
     r"""Include deleted workspaces in the returned results."""
     limit: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'limit', 'style': 'form', 'explode': True }})
-
     r"""Set the limit on the number of workspaces returned. The default is 20."""
     offset: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'offset', 'style': 'form', 'explode': True }})
-
     r"""Set the offset to start at when returning workspaces. The default is 0"""
     workspace_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'workspaceIds', 'style': 'form', 'explode': True }})
-
     r"""The UUIDs of the workspaces you wish to fetch. Empty list will retrieve all allowed workspaces."""
     
 
 @dataclasses.dataclass
 class ListWorkspacesResponse:
     
     content_type: str = dataclasses.field()
-
     status_code: int = dataclasses.field()
-
     raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-
     workspaces_response: Optional[shared_workspacesresponse.WorkspacesResponse] = dataclasses.field(default=None)
-
     r"""Successful operation"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/__init__.py` & `airbyte-1.7.1/src/airbyte/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/connectioncreaterequest.py` & `airbyte-1.7.1/src/airbyte/models/shared/connectioncreaterequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,31 +18,22 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionCreateRequest:
     
     destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})
-
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-
     configurations: Optional[shared_streamconfigurations.StreamConfigurations] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configurations'), 'exclude': lambda f: f is None }})
-
     r"""A list of configured stream options for a connection."""
     data_residency: Optional[shared_geographyenum_enum.GeographyEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency'), 'exclude': lambda f: f is None }})
-
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-
     r"""Optional name of the connection"""
     namespace_definition: Optional[ConnectionCreateRequestNamespaceDefinitionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceDefinition'), 'exclude': lambda f: f is None }})
-
     r"""Define the location where the data will be stored in the destination"""
     namespace_format: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('namespaceFormat'), 'exclude': lambda f: f is None }})
-
     r"""Used when namespaceDefinition is 'custom_format'. If blank then behaves like namespaceDefinition = 'destination'. If \\"${SOURCE_NAMESPACE}\\" then behaves like namespaceDefinition = 'source'."""
     prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prefix'), 'exclude': lambda f: f is None }})
-
     r"""Prefix that will be prepended to the name of each stream when it is written to the destination (ex. “airbyte_” causes “projects” => “airbyte_projects”)."""
     schedule: Optional[shared_connectionschedulecreate.ConnectionScheduleCreate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule'), 'exclude': lambda f: f is None }})
-
     r"""schedule for when the the connection should run, per the schedule type"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/connectionresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/connectionresponse.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionResponse:
     r"""Provides details of a single connection."""
     
     connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
-
     data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})
-
     destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})
-
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
     schedule: shared_connectionscheduleresponse.ConnectionScheduleResponse = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schedule') }})
-
     r"""schedule for when the the connection should run, per the schedule type"""
     source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-
     status: shared_connectionstatusenum_enum.ConnectionStatusEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/connectionschedulecreate.py` & `airbyte-1.7.1/src/airbyte/models/shared/connectionschedulecreate.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,11 +10,9 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionScheduleCreate:
     r"""schedule for when the the connection should run, per the schedule type"""
     
     schedule_type: shared_scheduletypeenum_enum.ScheduleTypeEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheduleType') }})
-
     cron_expression: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cronExpression'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/connectionscheduleresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/connectionscheduleresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionScheduleResponse:
     r"""schedule for when the the connection should run, per the schedule type"""
     
     schedule_type: shared_scheduletypewithbasicenum_enum.ScheduleTypeWithBasicEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheduleType') }})
-
     basic_timing: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('basicTiming'), 'exclude': lambda f: f is None }})
-
     cron_expression: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cronExpression'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/connectionsresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/connectionsresponse.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,13 +10,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ConnectionsResponse:
     r"""Successful operation"""
     
     data: list[shared_connectionresponse.ConnectionResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
-
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_amazon_sqs.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_amazon_sqs.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,30 +41,22 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAmazonSqs:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationAmazonSqsAmazonSqsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     queue_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('queue_url') }})
-
     r"""URL of the SQS Queue"""
     region: DestinationAmazonSqsAWSRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
-
     r"""AWS Region of the SQS Queue"""
     access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key'), 'exclude': lambda f: f is None }})
-
     r"""The Access Key ID of the AWS IAM Role to use for sending  messages"""
     message_body_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message_body_key'), 'exclude': lambda f: f is None }})
-
     r"""Use this property to extract the contents of the named key in the input record to use as the SQS message body. If not set, the entire content of the input record data is used as the message body."""
     message_delay: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message_delay'), 'exclude': lambda f: f is None }})
-
     r"""Modify the Message Delay of the individual message from the Queue's default (seconds)."""
     message_group_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message_group_id'), 'exclude': lambda f: f is None }})
-
     r"""The tag that specifies that a message belongs to a specific message group. This parameter applies only to, and is REQUIRED by, FIFO queues."""
     secret_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key'), 'exclude': lambda f: f is None }})
-
     r"""The Secret Key of the AWS IAM Role to use for sending messages"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_aws_datalake.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_aws_datalake.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,38 +14,33 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAwsDatalakeCredentialsIAMUser:
     r"""Choose How to Authenticate to AWS."""
     
     aws_access_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_access_key_id') }})
-
     r"""AWS User Access Key Id"""
     aws_secret_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_secret_access_key') }})
-
     r"""Secret Access Key"""
     credentials_title: DestinationAwsDatalakeCredentialsIAMUserCredentialsTitleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title') }})
-
     r"""Name of the credentials"""
     
 class DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum(str, Enum):
     r"""Name of the credentials"""
     IAM_ROLE = 'IAM Role'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAwsDatalakeCredentialsIAMRole:
     r"""Choose How to Authenticate to AWS."""
     
     credentials_title: DestinationAwsDatalakeCredentialsIAMRoleCredentialsTitleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title') }})
-
     r"""Name of the credentials"""
     role_arn: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role_arn') }})
-
     r"""Will assume this role to write data to s3"""
     
 class DestinationAwsDatalakeAwsDatalakeEnum(str, Enum):
     AWS_DATALAKE = 'aws-datalake'
 
 class DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum(str, Enum):
     r"""The compression algorithm used to compress data."""
@@ -60,17 +55,15 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAwsDatalakeFormatParquetColumnarStorage:
     r"""Format of the data output."""
     
     format_type: DestinationAwsDatalakeFormatParquetColumnarStorageFormatTypeWildcardEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression_codec: Optional[DestinationAwsDatalakeFormatParquetColumnarStorageCompressionCodecOptionalEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_codec'), 'exclude': lambda f: f is None }})
-
     r"""The compression algorithm used to compress data."""
     
 class DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum(str, Enum):
     r"""The compression algorithm used to compress data."""
     UNCOMPRESSED = 'UNCOMPRESSED'
     GZIP = 'GZIP'
 
@@ -80,17 +73,15 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSON:
     r"""Format of the data output."""
     
     format_type: DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONFormatTypeWildcardEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression_codec: Optional[DestinationAwsDatalakeFormatJSONLinesNewlineDelimitedJSONCompressionCodecOptionalEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_codec'), 'exclude': lambda f: f is None }})
-
     r"""The compression algorithm used to compress data."""
     
 class DestinationAwsDatalakeChooseHowToPartitionDataEnum(str, Enum):
     r"""Partition data by cursor fields when a cursor field is a date"""
     NO_PARTITIONING = 'NO PARTITIONING'
     DATE = 'DATE'
     YEAR = 'YEAR'
@@ -131,45 +122,32 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAwsDatalake:
     r"""The values required to configure the destination."""
     
     bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bucket_name') }})
-
     r"""The name of the S3 bucket. Read more <a href=\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html\\">here</a>."""
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     r"""Choose How to Authenticate to AWS."""
     destination_type: DestinationAwsDatalakeAwsDatalakeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     lakeformation_database_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lakeformation_database_name') }})
-
     r"""The default database this destination will use to create tables in per stream. Can be changed per connection by customizing the namespace."""
     region: DestinationAwsDatalakeS3BucketRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
-
     r"""The region of the S3 bucket. See <a href=\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions\\">here</a> for all region codes."""
     aws_account_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_account_id'), 'exclude': lambda f: f is None }})
-
     r"""target aws account id"""
     bucket_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bucket_prefix'), 'exclude': lambda f: f is None }})
-
     r"""S3 prefix"""
     format: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
-
     r"""Format of the data output."""
     glue_catalog_float_as_decimal: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('glue_catalog_float_as_decimal'), 'exclude': lambda f: f is None }})
-
     r"""Cast float/double as decimal(38,18). This can help achieve higher accuracy and represent numbers correctly as received from the source."""
     lakeformation_database_default_tag_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lakeformation_database_default_tag_key'), 'exclude': lambda f: f is None }})
-
     r"""Add a default tag key to databases created by this destination"""
     lakeformation_database_default_tag_values: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lakeformation_database_default_tag_values'), 'exclude': lambda f: f is None }})
-
     r"""Add default values for the `Tag Key` to databases created by this destination. Comma separate for multiple values."""
     lakeformation_governed_tables: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lakeformation_governed_tables'), 'exclude': lambda f: f is None }})
-
     r"""Whether to create tables as LF governed tables."""
     partitioning: Optional[DestinationAwsDatalakeChooseHowToPartitionDataEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('partitioning'), 'exclude': lambda f: f is None }})
-
     r"""Partition data by cursor fields when a cursor field is a date"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_azure_blob_storage.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_azure_blob_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON:
     r"""Output data format"""
     
     format_type: DestinationAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     
 class DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum(str, Enum):
     r"""Whether the input json data should be normalized (flattened) in the output CSV. Please refer to docs for details."""
     NO_FLATTENING = 'No flattening'
     ROOT_LEVEL_FLATTENING = 'Root level flattening'
 
 class DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum(str, Enum):
@@ -33,42 +32,32 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAzureBlobStorageFormatCSVCommaSeparatedValues:
     r"""Output data format"""
     
     flattening: DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesNormalizationFlatteningEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flattening') }})
-
     r"""Whether the input json data should be normalized (flattened) in the output CSV. Please refer to docs for details."""
     format_type: DestinationAzureBlobStorageFormatCSVCommaSeparatedValuesFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationAzureBlobStorage:
     r"""The values required to configure the destination."""
     
     azure_blob_storage_account_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_key') }})
-
     r"""The Azure blob storage account key."""
     azure_blob_storage_account_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_name') }})
-
     r"""The account's name of the Azure Blob Storage."""
     destination_type: DestinationAzureBlobStorageAzureBlobStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     format: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-
     r"""Output data format"""
     azure_blob_storage_container_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_container_name'), 'exclude': lambda f: f is None }})
-
     r"""The name of the Azure blob storage container. If not exists - will be created automatically. May be empty, then will be created automatically airbytecontainer+timestamp"""
     azure_blob_storage_endpoint_domain_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_endpoint_domain_name'), 'exclude': lambda f: f is None }})
-
     r"""This is Azure Blob Storage endpoint domain name. Leave default value (or leave it empty if run container from command line) to use Microsoft native from example."""
     azure_blob_storage_output_buffer_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_output_buffer_size'), 'exclude': lambda f: f is None }})
-
     r"""The amount of megabytes to buffer for the output stream to Azure. This will impact memory footprint on workers, but may need adjustment for performance and appropriate block size in Azure."""
     azure_blob_storage_spill_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_spill_size'), 'exclude': lambda f: f is None }})
-
     r"""The amount of megabytes after which the connector should spill the records in a new blob object. Make sure to configure size greater than individual records. Enter 0 if not applicable"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_bigquery.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKey:
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     
     credential_type: DestinationBigqueryLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential_type') }})
-
     hmac_key_access_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hmac_key_access_id') }})
-
     r"""HMAC key access ID. When linked to a service account, this ID is 61 characters long; when linked to a user account, it is 24 characters long."""
     hmac_key_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hmac_key_secret') }})
-
     r"""The corresponding secret for the access ID. It is a 40-character base-64 encoded string."""
     
 class DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum(str, Enum):
     r"""This upload method is supposed to temporary store records in GCS bucket. By this select you can chose if these records should be removed from GCS when migration has finished. The default \\"Delete all tmp files from GCS\\" value is used if not set explicitly."""
     DELETE_ALL_TMP_FILES_FROM_GCS = 'Delete all tmp files from GCS'
     KEEP_ALL_TMP_FILES_IN_GCS = 'Keep all tmp files in GCS'
 
@@ -82,68 +79,54 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryLoadingMethodGCSStaging:
     r"""Loading method used to send select the way data will be uploaded to BigQuery. <br/><b>Standard Inserts</b> - Direct uploading using SQL INSERT statements. This method is extremely inefficient and provided only for quick testing. In almost all cases, you should use staging. <br/><b>GCS Staging</b> - Writes large batches of records to a file, uploads the file to GCS, then uses <b>COPY INTO table</b> to upload the file. Recommended for most workloads for better speed and scalability. Read more about GCS Staging <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#gcs-staging\\">here</a>."""
     
     credential: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential') }})
-
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     gcs_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_name') }})
-
     r"""The name of the GCS bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/naming-buckets\\">here</a>."""
     gcs_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_path') }})
-
     r"""Directory under the GCS bucket where data will be written."""
     method: DestinationBigqueryLoadingMethodGCSStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     keep_files_in_gcs_bucket: Optional[DestinationBigqueryLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keep_files_in_gcs-bucket'), 'exclude': lambda f: f is None }})
-
     r"""This upload method is supposed to temporary store records in GCS bucket. By this select you can chose if these records should be removed from GCS when migration has finished. The default \\"Delete all tmp files from GCS\\" value is used if not set explicitly."""
     
 class DestinationBigqueryLoadingMethodStandardInsertsMethodEnum(str, Enum):
     STANDARD = 'Standard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryLoadingMethodStandardInserts:
     r"""Loading method used to send select the way data will be uploaded to BigQuery. <br/><b>Standard Inserts</b> - Direct uploading using SQL INSERT statements. This method is extremely inefficient and provided only for quick testing. In almost all cases, you should use staging. <br/><b>GCS Staging</b> - Writes large batches of records to a file, uploads the file to GCS, then uses <b>COPY INTO table</b> to upload the file. Recommended for most workloads for better speed and scalability. Read more about GCS Staging <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#gcs-staging\\">here</a>."""
     
     method: DestinationBigqueryLoadingMethodStandardInsertsMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class DestinationBigqueryTransformationQueryRunTypeEnum(str, Enum):
     r"""Interactive run type means that the query is executed as soon as possible, and these queries count towards concurrent rate limit and daily limit. Read more about interactive run type <a href=\\"https://cloud.google.com/bigquery/docs/running-queries#queries\\">here</a>. Batch queries are queued and started as soon as idle resources are available in the BigQuery shared resource pool, which usually occurs within a few minutes. Batch queries don’t count towards your concurrent rate limit. Read more about batch queries <a href=\\"https://cloud.google.com/bigquery/docs/running-queries#batch\\">here</a>. The default \\"interactive\\" value is used if not set explicitly."""
     INTERACTIVE = 'interactive'
     BATCH = 'batch'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigquery:
     r"""The values required to configure the destination."""
     
     dataset_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_id') }})
-
     r"""The default BigQuery Dataset ID that tables are replicated to if the source does not specify a namespace. Read more <a href=\\"https://cloud.google.com/bigquery/docs/datasets#create-dataset\\">here</a>."""
     dataset_location: DestinationBigqueryDatasetLocationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_location') }})
-
     r"""The location of the dataset. Warning: Changes made after creation will not be applied. Read more <a href=\\"https://cloud.google.com/bigquery/docs/locations\\">here</a>."""
     destination_type: DestinationBigqueryBigqueryEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""The GCP project ID for the project containing the target BigQuery dataset. Read more <a href=\\"https://cloud.google.com/resource-manager/docs/creating-managing-projects#identifying_projects\\">here</a>."""
     big_query_client_buffer_size_mb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('big_query_client_buffer_size_mb'), 'exclude': lambda f: f is None }})
-
     r"""Google BigQuery client's chunk (buffer) size (MIN=1, MAX = 15) for each table. The size that will be written by a single RPC. Written data will be buffered and only flushed upon reaching this size or closing the channel. The default 15MB value is used if not set explicitly. Read more <a href=\\"https://googleapis.dev/python/bigquery/latest/generated/google.cloud.bigquery.client.Client.html\\">here</a>."""
     credentials_json: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json'), 'exclude': lambda f: f is None }})
-
     r"""The contents of the JSON service account key. Check out the <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#service-account-key\\">docs</a> if you need help generating this key. Default credentials will be used if this field is left empty."""
     loading_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('loading_method'), 'exclude': lambda f: f is None }})
-
     r"""Loading method used to send select the way data will be uploaded to BigQuery. <br/><b>Standard Inserts</b> - Direct uploading using SQL INSERT statements. This method is extremely inefficient and provided only for quick testing. In almost all cases, you should use staging. <br/><b>GCS Staging</b> - Writes large batches of records to a file, uploads the file to GCS, then uses <b>COPY INTO table</b> to upload the file. Recommended for most workloads for better speed and scalability. Read more about GCS Staging <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#gcs-staging\\">here</a>."""
     transformation_priority: Optional[DestinationBigqueryTransformationQueryRunTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transformation_priority'), 'exclude': lambda f: f is None }})
-
     r"""Interactive run type means that the query is executed as soon as possible, and these queries count towards concurrent rate limit and daily limit. Read more about interactive run type <a href=\\"https://cloud.google.com/bigquery/docs/running-queries#queries\\">here</a>. Batch queries are queued and started as soon as idle resources are available in the BigQuery shared resource pool, which usually occurs within a few minutes. Batch queries don’t count towards your concurrent rate limit. Read more about batch queries <a href=\\"https://cloud.google.com/bigquery/docs/running-queries#batch\\">here</a>. The default \\"interactive\\" value is used if not set explicitly."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_bigquery_denormalized.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_bigquery_denormalized.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKey:
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     
     credential_type: DestinationBigqueryDenormalizedLoadingMethodGCSStagingCredentialHMACKeyCredentialTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential_type') }})
-
     hmac_key_access_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hmac_key_access_id') }})
-
     r"""HMAC key access ID. When linked to a service account, this ID is 61 characters long; when linked to a user account, it is 24 characters long."""
     hmac_key_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hmac_key_secret') }})
-
     r"""The corresponding secret for the access ID. It is a 40-character base-64 encoded string."""
     
 class DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum(str, Enum):
     r"""This upload method is supposed to temporary store records in GCS bucket. By this select you can chose if these records should be removed from GCS when migration has finished. The default \\"Delete all tmp files from GCS\\" value is used if not set explicitly."""
     DELETE_ALL_TMP_FILES_FROM_GCS = 'Delete all tmp files from GCS'
     KEEP_ALL_TMP_FILES_IN_GCS = 'Keep all tmp files in GCS'
 
@@ -82,60 +79,47 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryDenormalizedLoadingMethodGCSStaging:
     r"""Loading method used to send select the way data will be uploaded to BigQuery. <br/><b>Standard Inserts</b> - Direct uploading using SQL INSERT statements. This method is extremely inefficient and provided only for quick testing. In almost all cases, you should use staging. <br/><b>GCS Staging</b> - Writes large batches of records to a file, uploads the file to GCS, then uses <b>COPY INTO table</b> to upload the file. Recommended for most workloads for better speed and scalability. Read more about GCS Staging <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#gcs-staging\\">here</a>."""
     
     credential: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential') }})
-
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     gcs_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_name') }})
-
     r"""The name of the GCS bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/naming-buckets\\">here</a>."""
     gcs_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_path') }})
-
     r"""Directory under the GCS bucket where data will be written. Read more <a href=\\"https://cloud.google.com/storage/docs/locations\\">here</a>."""
     method: DestinationBigqueryDenormalizedLoadingMethodGCSStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     keep_files_in_gcs_bucket: Optional[DestinationBigqueryDenormalizedLoadingMethodGCSStagingGCSTmpFilesAfterwardProcessingEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keep_files_in_gcs-bucket'), 'exclude': lambda f: f is None }})
-
     r"""This upload method is supposed to temporary store records in GCS bucket. By this select you can chose if these records should be removed from GCS when migration has finished. The default \\"Delete all tmp files from GCS\\" value is used if not set explicitly."""
     
 class DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum(str, Enum):
     STANDARD = 'Standard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryDenormalizedLoadingMethodStandardInserts:
     r"""Loading method used to send select the way data will be uploaded to BigQuery. <br/><b>Standard Inserts</b> - Direct uploading using SQL INSERT statements. This method is extremely inefficient and provided only for quick testing. In almost all cases, you should use staging. <br/><b>GCS Staging</b> - Writes large batches of records to a file, uploads the file to GCS, then uses <b>COPY INTO table</b> to upload the file. Recommended for most workloads for better speed and scalability. Read more about GCS Staging <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#gcs-staging\\">here</a>."""
     
     method: DestinationBigqueryDenormalizedLoadingMethodStandardInsertsMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationBigqueryDenormalized:
     r"""The values required to configure the destination."""
     
     dataset_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_id') }})
-
     r"""The default BigQuery Dataset ID that tables are replicated to if the source does not specify a namespace. Read more <a href=\\"https://cloud.google.com/bigquery/docs/datasets#create-dataset\\">here</a>."""
     destination_type: DestinationBigqueryDenormalizedBigqueryDenormalizedEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""The GCP project ID for the project containing the target BigQuery dataset. Read more <a href=\\"https://cloud.google.com/resource-manager/docs/creating-managing-projects#identifying_projects\\">here</a>."""
     big_query_client_buffer_size_mb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('big_query_client_buffer_size_mb'), 'exclude': lambda f: f is None }})
-
     r"""Google BigQuery client's chunk (buffer) size (MIN=1, MAX = 15) for each table. The size that will be written by a single RPC. Written data will be buffered and only flushed upon reaching this size or closing the channel. The default 15MB value is used if not set explicitly. Read more <a href=\\"https://googleapis.dev/python/bigquery/latest/generated/google.cloud.bigquery.client.Client.html\\">here</a>."""
     credentials_json: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json'), 'exclude': lambda f: f is None }})
-
     r"""The contents of the JSON service account key. Check out the <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#service-account-key\\">docs</a> if you need help generating this key. Default credentials will be used if this field is left empty."""
     dataset_location: Optional[DestinationBigqueryDenormalizedDatasetLocationEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_location'), 'exclude': lambda f: f is None }})
-
     r"""The location of the dataset. Warning: Changes made after creation will not be applied. The default \\"US\\" value is used if not set explicitly. Read more <a href=\\"https://cloud.google.com/bigquery/docs/locations\\">here</a>."""
     loading_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('loading_method'), 'exclude': lambda f: f is None }})
-
     r"""Loading method used to send select the way data will be uploaded to BigQuery. <br/><b>Standard Inserts</b> - Direct uploading using SQL INSERT statements. This method is extremely inefficient and provided only for quick testing. In almost all cases, you should use staging. <br/><b>GCS Staging</b> - Writes large batches of records to a file, uploads the file to GCS, then uses <b>COPY INTO table</b> to upload the file. Recommended for most workloads for better speed and scalability. Read more about GCS Staging <a href=\\"https://docs.airbyte.com/integrations/destinations/bigquery#gcs-staging\\">here</a>."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_cassandra.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_cassandra.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,30 +13,22 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationCassandra:
     r"""The values required to configure the destination."""
     
     address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
-
     r"""Address to connect to."""
     destination_type: DestinationCassandraCassandraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     keyspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keyspace') }})
-
     r"""Default Cassandra keyspace to create data in."""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Password associated with Cassandra."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of Cassandra."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access Cassandra."""
     datacenter: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datacenter'), 'exclude': lambda f: f is None }})
-
     r"""Datacenter of the cassandra cluster."""
     replication: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication'), 'exclude': lambda f: f is None }})
-
     r"""Indicates to how many nodes the data should be replicated to."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_clickhouse.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_clickhouse.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,92 +17,73 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationClickhouseTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationClickhouseTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationClickhouseTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationClickhouseTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationClickhouse:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationClickhouseClickhouseEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""HTTP port of the database."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with the username."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_convex.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_gridly.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class DestinationConvexConvexEnum(str, Enum):
-    CONVEX = 'convex'
+class SourceGridlyGridlyEnum(str, Enum):
+    GRIDLY = 'gridly'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DestinationConvex:
-    r"""The values required to configure the destination."""
+class SourceGridly:
+    r"""The values required to configure the source."""
     
-    access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key') }})
-
-    r"""API access key used to send data to a Convex deployment."""
-    deployment_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deployment_url') }})
-
-    r"""URL of the Convex deployment that is the destination"""
-    destination_type: DestinationConvexConvexEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    grid_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grid_id') }})
+    r"""ID of a grid, or can be ID of a branch"""
+    source_type: SourceGridlyGridlyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_databend.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_databend.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationDatabend:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationDatabendDatabendEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with the username."""
     port: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     r"""Port of the database."""
     table: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('table'), 'exclude': lambda f: f is None }})
-
     r"""The default  table was written to."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_databricks.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_databricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,21 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationDatabricksDataSourceAzureBlobStorage:
     r"""Storage on which the delta lake is built."""
     
     azure_blob_storage_account_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_name') }})
-
     r"""The account's name of the Azure Blob Storage."""
     azure_blob_storage_container_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_container_name') }})
-
     r"""The name of the Azure blob storage container."""
     azure_blob_storage_sas_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_sas_token') }})
-
     r"""Shared access signature (SAS) token to grant limited access to objects in your storage account."""
     data_source_type: DestinationDatabricksDataSourceAzureBlobStorageDataSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_source_type') }})
-
     azure_blob_storage_endpoint_domain_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_endpoint_domain_name'), 'exclude': lambda f: f is None }})
-
     r"""This is Azure Blob Storage endpoint domain name. Leave default value (or leave it empty if run container from command line) to use Microsoft native from example."""
     
 class DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum(str, Enum):
     S3_STORAGE = 'S3_STORAGE'
 
 class DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum(str, Enum):
     r"""The region of the S3 staging bucket to use if utilising a copy strategy."""
@@ -66,78 +61,60 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationDatabricksDataSourceAmazonS3:
     r"""Storage on which the delta lake is built."""
     
     data_source_type: DestinationDatabricksDataSourceAmazonS3DataSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_source_type') }})
-
     s3_access_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_access_key_id') }})
-
     r"""The Access Key Id granting allow one to access the above S3 staging bucket. Airbyte requires Read and Write permissions to the given bucket."""
     s3_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_name') }})
-
     r"""The name of the S3 bucket to use for intermittent staging of the data."""
     s3_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_path') }})
-
     r"""The directory under the S3 bucket where data will be written."""
     s3_bucket_region: DestinationDatabricksDataSourceAmazonS3S3BucketRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_region') }})
-
     r"""The region of the S3 staging bucket to use if utilising a copy strategy."""
     s3_secret_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_secret_access_key') }})
-
     r"""The corresponding secret to the above access key id."""
     file_name_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_name_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The pattern allows you to set the file-name format for the S3 staging file(s)"""
     
 class DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum(str, Enum):
     MANAGED_TABLES_STORAGE = 'MANAGED_TABLES_STORAGE'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationDatabricksDataSourceRecommendedManagedTables:
     r"""Storage on which the delta lake is built."""
     
     data_source_type: DestinationDatabricksDataSourceRecommendedManagedTablesDataSourceTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_source_type') }})
-
     
 class DestinationDatabricksDatabricksEnum(str, Enum):
     DATABRICKS = 'databricks'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationDatabricks:
     r"""The values required to configure the destination."""
     
     accept_terms: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accept_terms') }})
-
     r"""You must agree to the Databricks JDBC Driver <a href=\\"https://databricks.com/jdbc-odbc-driver-license\\">Terms & Conditions</a> to use this connector."""
     data_source: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_source') }})
-
     r"""Storage on which the delta lake is built."""
     databricks_http_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('databricks_http_path') }})
-
     r"""Databricks Cluster HTTP Path."""
     databricks_personal_access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('databricks_personal_access_token') }})
-
     r"""Databricks Personal Access Token for making authenticated requests."""
     databricks_server_hostname: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('databricks_server_hostname') }})
-
     r"""Databricks Cluster Server Hostname."""
     destination_type: DestinationDatabricksDatabricksEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     database: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database'), 'exclude': lambda f: f is None }})
-
     r"""The name of the catalog. If not specified otherwise, the \\"hive_metastore\\" will be used."""
     databricks_port: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('databricks_port'), 'exclude': lambda f: f is None }})
-
     r"""Databricks Cluster Port."""
     purge_staging_data: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purge_staging_data'), 'exclude': lambda f: f is None }})
-
     r"""Default to 'true'. Switch it to 'false' for debugging purpose."""
     schema: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema'), 'exclude': lambda f: f is None }})
-
     r"""The default schema tables are written. If not specified otherwise, the \\"default\\" will be used."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_dynamodb.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,24 +42,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationDynamodb:
     r"""The values required to configure the destination."""
     
     access_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key_id') }})
-
     r"""The access key id to access the DynamoDB. Airbyte requires Read and Write permissions to the DynamoDB."""
     destination_type: DestinationDynamodbDynamodbEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     dynamodb_region: DestinationDynamodbDynamoDBRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamodb_region') }})
-
     r"""The region of the DynamoDB."""
     dynamodb_table_name_prefix: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamodb_table_name_prefix') }})
-
     r"""The prefix to use when naming DynamoDB tables."""
     secret_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_access_key') }})
-
     r"""The corresponding secret to the access key id."""
     dynamodb_endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dynamodb_endpoint'), 'exclude': lambda f: f is None }})
-
     r"""This is your DynamoDB endpoint url.(if you are working with AWS DynamoDB, just leave empty)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_elasticsearch.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_elasticsearch.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,57 +13,46 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationElasticsearchAuthenticationMethodUsernamePassword:
     r"""Basic auth header with a username and password"""
     
     method: DestinationElasticsearchAuthenticationMethodUsernamePasswordMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Basic auth password to access a secure Elasticsearch server"""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Basic auth username to access a secure Elasticsearch server"""
     
 class DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum(str, Enum):
     SECRET = 'secret'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationElasticsearchAuthenticationMethodAPIKeySecret:
     r"""Use a api key and secret combination to authenticate"""
     
     api_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKeyId') }})
-
     r"""The Key ID to used when accessing an enterprise Elasticsearch instance."""
     api_key_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKeySecret') }})
-
     r"""The secret associated with the API Key ID."""
     method: DestinationElasticsearchAuthenticationMethodAPIKeySecretMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class DestinationElasticsearchElasticsearchEnum(str, Enum):
     ELASTICSEARCH = 'elasticsearch'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationElasticsearch:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationElasticsearchElasticsearchEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
-
     r"""The full url of the Elasticsearch server"""
     authentication_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authenticationMethod'), 'exclude': lambda f: f is None }})
-
     r"""The type of authentication to be used"""
     ca_certificate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ca_certificate'), 'exclude': lambda f: f is None }})
-
     r"""CA certificate"""
     upsert: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('upsert'), 'exclude': lambda f: f is None }})
-
     r"""If a primary key identifier is defined in the source, an upsert will be performed using the primary key value as the elasticsearch doc id. Does not support composite primary keys."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_firebolt.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_firebolt.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,63 +16,49 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationFireboltLoadingMethodExternalTableViaS3:
     r"""Loading method used to select the way data will be uploaded to Firebolt"""
     
     aws_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_key_id') }})
-
     r"""AWS access key granting read and write access to S3."""
     aws_key_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_key_secret') }})
-
     r"""Corresponding secret part of the AWS Key"""
     method: DestinationFireboltLoadingMethodExternalTableViaS3MethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     s3_bucket: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket') }})
-
     r"""The name of the S3 bucket."""
     s3_region: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_region') }})
-
     r"""Region name of the S3 bucket."""
     
 class DestinationFireboltLoadingMethodSQLInsertsMethodEnum(str, Enum):
     SQL = 'SQL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationFireboltLoadingMethodSQLInserts:
     r"""Loading method used to select the way data will be uploaded to Firebolt"""
     
     method: DestinationFireboltLoadingMethodSQLInsertsMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationFirebolt:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The database to connect to."""
     destination_type: DestinationFireboltFireboltEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Firebolt password."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Firebolt email address you use to login."""
     account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
-
     r"""Firebolt account to login."""
     engine: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('engine'), 'exclude': lambda f: f is None }})
-
     r"""Engine name or url to connect to."""
     host: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host'), 'exclude': lambda f: f is None }})
-
     r"""The host name of your Firebolt database."""
     loading_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('loading_method'), 'exclude': lambda f: f is None }})
-
     r"""Loading method used to select the way data will be uploaded to Firebolt"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_firestore.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_firestore.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationFirestore:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationFirestoreFirestoreEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""The GCP project ID for the project containing the target BigQuery dataset."""
     credentials_json: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json'), 'exclude': lambda f: f is None }})
-
     r"""The contents of the JSON service account key. Check out the <a href=\\"https://docs.airbyte.io/integrations/destinations/firestore\\">docs</a> if you need help generating this key. Default credentials will be used if this field is left empty."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_gcs.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_gcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsCredentialHMACKey:
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     
     credential_type: DestinationGcsCredentialHMACKeyCredentialTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential_type') }})
-
     hmac_key_access_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hmac_key_access_id') }})
-
     r"""When linked to a service account, this ID is 61 characters long; when linked to a user account, it is 24 characters long. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys#overview\\">here</a>."""
     hmac_key_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hmac_key_secret') }})
-
     r"""The corresponding secret for the access ID. It is a 40-character base-64 encoded string.  Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys#secrets\\">here</a>."""
     
 class DestinationGcsGcsEnum(str, Enum):
     GCS = 'gcs'
 
 class DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum(str, Enum):
     r"""The compression algorithm used to compress data pages."""
@@ -44,96 +41,83 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatParquetColumnarStorage:
     r"""Output data format. One of the following formats must be selected - <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-avro#advantages_of_avro\\">AVRO</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-parquet#parquet_schemas\\">PARQUET</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-csv#loading_csv_data_into_a_table\\">CSV</a> format, or <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-json#loading_json_data_into_a_new_table\\">JSONL</a> format."""
     
     format_type: DestinationGcsFormatParquetColumnarStorageFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     block_size_mb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_size_mb'), 'exclude': lambda f: f is None }})
-
     r"""This is the size of a row group being buffered in memory. It limits the memory usage when writing. Larger values will improve the IO when reading, but consume more memory when writing. Default: 128 MB."""
     compression_codec: Optional[DestinationGcsFormatParquetColumnarStorageCompressionCodecEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_codec'), 'exclude': lambda f: f is None }})
-
     r"""The compression algorithm used to compress data pages."""
     dictionary_encoding: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dictionary_encoding'), 'exclude': lambda f: f is None }})
-
     r"""Default: true."""
     dictionary_page_size_kb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dictionary_page_size_kb'), 'exclude': lambda f: f is None }})
-
     r"""There is one dictionary page per column per row group when dictionary encoding is used. The dictionary page size works like the page size but for dictionary. Default: 1024 KB."""
     max_padding_size_mb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_padding_size_mb'), 'exclude': lambda f: f is None }})
-
     r"""Maximum size allowed as padding to align row groups. This is also the minimum size of a row group. Default: 8 MB."""
     page_size_kb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page_size_kb'), 'exclude': lambda f: f is None }})
-
     r"""The page size is for compression. A block is composed of pages. A page is the smallest unit that must be read fully to access a single record. If this value is too small, the compression will deteriorate. Default: 1024 KB."""
     
 class DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum(str, Enum):
     GZIP = 'GZIP'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIP:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum(str, Enum):
     NO_COMPRESSION = 'No Compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationGcsFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum(str, Enum):
     JSONL = 'JSONL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatJSONLinesNewlineDelimitedJSON:
     r"""Output data format. One of the following formats must be selected - <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-avro#advantages_of_avro\\">AVRO</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-parquet#parquet_schemas\\">PARQUET</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-csv#loading_csv_data_into_a_table\\">CSV</a> format, or <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-json#loading_json_data_into_a_new_table\\">JSONL</a> format."""
     
     format_type: DestinationGcsFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression'), 'exclude': lambda f: f is None }})
-
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
 class DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum(str, Enum):
     GZIP = 'GZIP'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIP:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".csv.gz\\")."""
     
     compression_type: Optional[DestinationGcsFormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum(str, Enum):
     NO_COMPRESSION = 'No Compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompression:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".csv.gz\\")."""
     
     compression_type: Optional[DestinationGcsFormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum(str, Enum):
     r"""Whether the input JSON data should be normalized (flattened) in the output CSV. Please refer to docs for details."""
     NO_FLATTENING = 'No flattening'
     ROOT_LEVEL_FLATTENING = 'Root level flattening'
 
 class DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum(str, Enum):
@@ -142,120 +126,105 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatCSVCommaSeparatedValues:
     r"""Output data format. One of the following formats must be selected - <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-avro#advantages_of_avro\\">AVRO</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-parquet#parquet_schemas\\">PARQUET</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-csv#loading_csv_data_into_a_table\\">CSV</a> format, or <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-json#loading_json_data_into_a_new_table\\">JSONL</a> format."""
     
     format_type: DestinationGcsFormatCSVCommaSeparatedValuesFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression'), 'exclude': lambda f: f is None }})
-
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".csv.gz\\")."""
     flattening: Optional[DestinationGcsFormatCSVCommaSeparatedValuesNormalizationEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flattening'), 'exclude': lambda f: f is None }})
-
     r"""Whether the input JSON data should be normalized (flattened) in the output CSV. Please refer to docs for details."""
     
 class DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum(str, Enum):
     SNAPPY = 'snappy'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvroCompressionCodecSnappy:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationGcsFormatAvroApacheAvroCompressionCodecSnappyCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     
 class DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum(str, Enum):
     ZSTANDARD = 'zstandard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvroCompressionCodecZstandard:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationGcsFormatAvroApacheAvroCompressionCodecZstandardCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     compression_level: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_level'), 'exclude': lambda f: f is None }})
-
     r"""Negative levels are 'fast' modes akin to lz4 or snappy, levels above 9 are generally for archival purposes, and levels above 18 use a lot of memory."""
     include_checksum: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_checksum'), 'exclude': lambda f: f is None }})
-
     r"""If true, include a checksum with each data block."""
     
 class DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum(str, Enum):
     XZ = 'xz'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvroCompressionCodecXz:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationGcsFormatAvroApacheAvroCompressionCodecXzCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     compression_level: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_level'), 'exclude': lambda f: f is None }})
-
     r"""The presets 0-3 are fast presets with medium compression. The presets 4-6 are fairly slow presets with high compression. The default preset is 6. The presets 7-9 are like the preset 6 but use bigger dictionaries and have higher compressor and decompressor memory requirements. Unless the uncompressed size of the file exceeds 8 MiB, 16 MiB, or 32 MiB, it is waste of memory to use the presets 7, 8, or 9, respectively. Read more <a href=\\"https://commons.apache.org/proper/commons-compress/apidocs/org/apache/commons/compress/compressors/xz/XZCompressorOutputStream.html#XZCompressorOutputStream-java.io.OutputStream-int-\\">here</a> for details."""
     
 class DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum(str, Enum):
     BZIP2 = 'bzip2'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationGcsFormatAvroApacheAvroCompressionCodecBzip2CodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     
 class DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum(str, Enum):
     DEFLATE = 'Deflate'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvroCompressionCodecDeflate:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationGcsFormatAvroApacheAvroCompressionCodecDeflateCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     compression_level: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_level'), 'exclude': lambda f: f is None }})
-
     r"""0: no compression & fastest, 9: best compression & slowest."""
     
 class DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum(str, Enum):
     NO_COMPRESSION = 'no compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompression:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationGcsFormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     
 class DestinationGcsFormatAvroApacheAvroFormatTypeEnum(str, Enum):
     AVRO = 'Avro'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcsFormatAvroApacheAvro:
     r"""Output data format. One of the following formats must be selected - <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-avro#advantages_of_avro\\">AVRO</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-parquet#parquet_schemas\\">PARQUET</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-csv#loading_csv_data_into_a_table\\">CSV</a> format, or <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-json#loading_json_data_into_a_new_table\\">JSONL</a> format."""
     
     compression_codec: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_codec') }})
-
     r"""The compression algorithm used to compress data. Default to no compression."""
     format_type: DestinationGcsFormatAvroApacheAvroFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     
 class DestinationGCSGCSBucketRegionEnum(str, Enum):
     r"""Select a Region of the GCS Bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/locations\\">here</a>."""
     NORTHAMERICA_NORTHEAST1 = 'northamerica-northeast1'
     NORTHAMERICA_NORTHEAST2 = 'northamerica-northeast2'
     US_CENTRAL1 = 'us-central1'
     US_EAST1 = 'us-east1'
@@ -294,24 +263,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGcs:
     r"""The values required to configure the destination."""
     
     credential: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credential') }})
-
     r"""An HMAC key is a type of credential and can be associated with a service account or a user account in Cloud Storage. Read more <a href=\\"https://cloud.google.com/storage/docs/authentication/hmackeys\\">here</a>."""
     destination_type: DestinationGcsGcsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     format: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-
     r"""Output data format. One of the following formats must be selected - <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-avro#advantages_of_avro\\">AVRO</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-parquet#parquet_schemas\\">PARQUET</a> format, <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-csv#loading_csv_data_into_a_table\\">CSV</a> format, or <a href=\\"https://cloud.google.com/bigquery/docs/loading-data-cloud-storage-json#loading_json_data_into_a_new_table\\">JSONL</a> format."""
     gcs_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_name') }})
-
     r"""You can find the bucket name in the App Engine Admin console Application Settings page, under the label Google Cloud Storage Bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/naming-buckets\\">here</a>."""
     gcs_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_path') }})
-
     r"""GCS Bucket Path string Subdirectory under the above bucket to sync the data into."""
     gcs_bucket_region: Optional[DestinationGCSGCSBucketRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket_region'), 'exclude': lambda f: f is None }})
-
     r"""Select a Region of the GCS Bucket. Read more <a href=\\"https://cloud.google.com/storage/docs/locations\\">here</a>."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_google_sheets.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_google_sheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,34 +9,28 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGoogleSheetsAuthenticationViaGoogleOAuth:
     r"""Google API Credentials for connecting to Google Sheets and Google Drive APIs"""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Google Sheets developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Google Sheets developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining new access token."""
     
 class DestinationGoogleSheetsGoogleSheetsEnum(str, Enum):
     GOOGLE_SHEETS = 'google-sheets'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationGoogleSheets:
     r"""The values required to configure the destination."""
     
     credentials: DestinationGoogleSheetsAuthenticationViaGoogleOAuth = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     r"""Google API Credentials for connecting to Google Sheets and Google Drive APIs"""
     destination_type: DestinationGoogleSheetsGoogleSheetsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     spreadsheet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spreadsheet_id') }})
-
     r"""The link to your spreadsheet. See <a href='https://docs.airbyte.com/integrations/destinations/google-sheets#sheetlink'>this guide</a> for more details."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_keen.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_keen.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationKeen:
     r"""The values required to configure the destination."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""To get Keen Master API Key, navigate to the Access tab from the left-hand, side panel and check the Project Details section."""
     destination_type: DestinationKeenKeenEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""To get Keen Project ID, navigate to the Access tab from the left-hand, side panel and check the Project Details section."""
     infer_timestamp: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('infer_timestamp'), 'exclude': lambda f: f is None }})
-
     r"""Allow connector to guess keen.timestamp value based on the streamed data."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_kinesis.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_kinesis.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,27 +12,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationKinesis:
     r"""The values required to configure the destination."""
     
     access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accessKey') }})
-
     r"""Generate the AWS Access Key for current user."""
     buffer_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bufferSize') }})
-
     r"""Buffer size for storing kinesis records before being batch streamed."""
     destination_type: DestinationKinesisKinesisEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     endpoint: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint') }})
-
     r"""AWS Kinesis endpoint."""
     private_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('privateKey') }})
-
     r"""The AWS Private Key - a string of numbers and letters that are unique for each account, also known as a \\"recovery phrase\\"."""
     region: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
-
     r"""AWS region. Your account determines the Regions that are available to you."""
     shard_count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shardCount') }})
-
     r"""Number of shards to which the data should be streamed."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_mariadb_columnstore.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_mariadb_columnstore.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,92 +17,73 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMariadbColumnstoreTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMariadbColumnstoreTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMariadbColumnstoreTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMariadbColumnstoreTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationMariadbColumnstoreTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMariadbColumnstore:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationMariadbColumnstoreMariadbColumnstoreEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The Port of the database."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The Username which is used to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The Password associated with the username."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_meilisearch.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_rockset.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,25 +3,24 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class DestinationMeilisearchMeilisearchEnum(str, Enum):
-    MEILISEARCH = 'meilisearch'
+class DestinationRocksetRocksetEnum(str, Enum):
+    ROCKSET = 'rockset'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DestinationMeilisearch:
+class DestinationRockset:
     r"""The values required to configure the destination."""
     
-    destination_type: DestinationMeilisearchMeilisearchEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
-    host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
-    r"""Hostname of the MeiliSearch instance."""
-    api_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key'), 'exclude': lambda f: f is None }})
-
-    r"""MeiliSearch API Key. See the <a href=\\"https://docs.airbyte.com/integrations/destinations/meilisearch\\">docs</a> for more information on how to obtain this key."""
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    r"""Rockset api key"""
+    destination_type: DestinationRocksetRocksetEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
+    workspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace') }})
+    r"""The Rockset workspace in which collections will be created + written to."""
+    api_server: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_server'), 'exclude': lambda f: f is None }})
+    r"""Rockset api URL"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_mongodb.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_mongodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,168 +13,140 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbAuthTypeLoginPassword:
     r"""Login/Password."""
     
     authorization: DestinationMongodbAuthTypeLoginPasswordAuthorizationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorization') }})
-
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Password associated with the username."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     
 class DestinationMongodbAuthTypeNoneAuthorizationEnum(str, Enum):
     NONE = 'none'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbAuthTypeNone:
     r"""None."""
     
     authorization: DestinationMongodbAuthTypeNoneAuthorizationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorization') }})
-
     
 class DestinationMongodbMongodbEnum(str, Enum):
     MONGODB = 'mongodb'
 
 class DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum(str, Enum):
     ATLAS = 'atlas'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbInstanceTypeMongoDBAtlas:
     r"""MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     
     cluster_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cluster_url') }})
-
     r"""URL of a cluster to connect to."""
     instance: DestinationMongodbInstanceTypeMongoDBAtlasInstanceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance') }})
-
     
 class DestinationMongodbInstanceTypeReplicaSetInstanceEnum(str, Enum):
     REPLICA = 'replica'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbInstanceTypeReplicaSet:
     r"""MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     
     instance: DestinationMongodbInstanceTypeReplicaSetInstanceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance') }})
-
     server_addresses: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('server_addresses') }})
-
     r"""The members of a replica set. Please specify `host`:`port` of each member seperated by comma."""
     replica_set: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replica_set'), 'exclude': lambda f: f is None }})
-
     r"""A replica set name."""
     
 class DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum(str, Enum):
     STANDALONE = 'standalone'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbInstanceTypeStandaloneMongoDbInstance:
     r"""MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The Host of a Mongo database to be replicated."""
     instance: DestinationMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance') }})
-
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The Port of a Mongo database to be replicated."""
     
 class DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMongodbTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMongodbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodbTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationMongodbTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMongodb:
     r"""The values required to configure the destination."""
     
     auth_type: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     r"""Authorization type."""
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationMongodbMongodbEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     instance_type: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance_type'), 'exclude': lambda f: f is None }})
-
     r"""MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_mssql.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_mssql.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,126 +16,102 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMssqlSslMethodEncryptedVerifyCertificate:
     r"""Verify and use the certificate provided by the server."""
     
     ssl_method: DestinationMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_method') }})
-
     host_name_in_certificate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hostNameInCertificate'), 'exclude': lambda f: f is None }})
-
     r"""Specifies the host name of the server. The value of this property must match the subject property of the certificate."""
     
 class DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum(str, Enum):
     ENCRYPTED_TRUST_SERVER_CERTIFICATE = 'encrypted_trust_server_certificate'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMssqlSslMethodEncryptedTrustServerCertificate:
     r"""Use the certificate provided by the server without verification. (For testing purposes only!)"""
     
     ssl_method: DestinationMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_method') }})
-
     
 class DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMssqlTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMssqlTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMssqlTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationMssqlTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMssql:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The name of the MSSQL database."""
     destination_type: DestinationMssqlMssqlEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The host name of the MSSQL database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The port of the MSSQL database."""
     schema: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema') }})
-
     r"""The default schema tables are written to if the source does not specify a namespace. The usual value for this field is \\"public\\"."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username which is used to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with this username."""
     ssl_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_method'), 'exclude': lambda f: f is None }})
-
     r"""The encryption method which is used to communicate with the database."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_mysql.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,92 +17,73 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMysqlTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMysqlTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMysqlTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationMysqlTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationMysql:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationMysqlMysqlEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with the username."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_oracle.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_oracle.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,95 +17,75 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationOracleTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationOracleTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationOracleTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationOracleTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationOracle:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationOracleOracleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The port of the database."""
     sid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sid') }})
-
     r"""The System Identifier uniquely distinguishes the instance from any other instance on the same computer."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username to access the database. This user must have CREATE USER privileges in the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with the username."""
     schema: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema'), 'exclude': lambda f: f is None }})
-
     r"""The default schema is used as the target schema for all statements issued from the connection that do not explicitly specify a schema name. The usual value for this field is \\"airbyte\\".  In Oracle, schemas and users are the same thing, so the \\"user\\" parameter is used as the login credentials and this is used for the default Airbyte message schema."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_postgres.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,197 +16,164 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresSslModeVerifyFull:
     r"""Verify-full SSL mode."""
     
     ca_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ca_certificate') }})
-
     r"""CA certificate"""
     client_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_certificate') }})
-
     r"""Client certificate"""
     client_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key') }})
-
     r"""Client key"""
     mode: DestinationPostgresSslModeVerifyFullModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     client_key_password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key_password'), 'exclude': lambda f: f is None }})
-
     r"""Password for keystorage. This field is optional. If you do not add it - the password will be generated automatically."""
     
 class DestinationPostgresSslModeVerifyCaModeEnum(str, Enum):
     VERIFY_CA = 'verify-ca'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresSslModeVerifyCa:
     r"""Verify-ca SSL mode."""
     
     ca_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ca_certificate') }})
-
     r"""CA certificate"""
     mode: DestinationPostgresSslModeVerifyCaModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     client_key_password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key_password'), 'exclude': lambda f: f is None }})
-
     r"""Password for keystorage. This field is optional. If you do not add it - the password will be generated automatically."""
     
 class DestinationPostgresSslModeRequireModeEnum(str, Enum):
     REQUIRE = 'require'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresSslModeRequire:
     r"""Require SSL mode."""
     
     mode: DestinationPostgresSslModeRequireModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class DestinationPostgresSslModePreferModeEnum(str, Enum):
     PREFER = 'prefer'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresSslModePrefer:
     r"""Prefer SSL mode."""
     
     mode: DestinationPostgresSslModePreferModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class DestinationPostgresSslModeAllowModeEnum(str, Enum):
     ALLOW = 'allow'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresSslModeAllow:
     r"""Allow SSL mode."""
     
     mode: DestinationPostgresSslModeAllowModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class DestinationPostgresSslModeDisableModeEnum(str, Enum):
     DISABLE = 'disable'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresSslModeDisable:
     r"""Disable SSL."""
     
     mode: DestinationPostgresSslModeDisableModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationPostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationPostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgresTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationPostgresTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPostgres:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationPostgresPostgresEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database."""
     schema: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema') }})
-
     r"""The default schema tables are written to if the source does not specify a namespace. The usual value for this field is \\"public\\"."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with the username."""
     ssl_mode: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_mode'), 'exclude': lambda f: f is None }})
-
     r"""SSL connection modes.
      <b>disable</b> - Chose this mode to disable encryption of communication between Airbyte and destination database
      <b>allow</b> - Chose this mode to enable encryption only when required by the source database
      <b>prefer</b> - Chose this mode to allow unencrypted connection only if the source database does not support encryption
      <b>require</b> - Chose this mode to always require encryption. If the source database server does not support encryption, connection will fail
       <b>verify-ca</b> - Chose this mode to always require encryption and to verify that the source database server has a valid SSL certificate
       <b>verify-full</b> - This is the most secure mode. Chose this mode to always require encryption and to verify the identity of the source database server
      See more information - <a href=\"https://jdbc.postgresql.org/documentation/head/ssl-client.html\"> in the docs</a>.
     """
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_pubsub.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_pubsub.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,24 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPubsub:
     r"""The values required to configure the destination."""
     
     batching_enabled: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_enabled') }})
-
     r"""If TRUE messages will be buffered instead of sending them one by one"""
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""The contents of the JSON service account key. Check out the <a href=\\"https://docs.airbyte.com/integrations/destinations/pubsub\\">docs</a> if you need help generating this key."""
     destination_type: DestinationPubsubPubsubEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     ordering_enabled: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ordering_enabled') }})
-
     r"""If TRUE PubSub publisher will have <a href=\\"https://cloud.google.com/pubsub/docs/ordering\\">message ordering</a> enabled. Every message will have an ordering key of stream"""
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""The GCP project ID for the project containing the target PubSub."""
     topic_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_id') }})
-
     r"""The PubSub topic ID in the given GCP project ID."""
     batching_delay_threshold: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_delay_threshold'), 'exclude': lambda f: f is None }})
-
     r"""Number of ms before the buffer is flushed"""
     batching_element_count_threshold: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_element_count_threshold'), 'exclude': lambda f: f is None }})
-
     r"""Number of messages before the buffer is flushed"""
     batching_request_bytes_threshold: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_request_bytes_threshold'), 'exclude': lambda f: f is None }})
-
     r"""Number of bytes before the buffer is flushed"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_pulsar.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_pulsar.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,60 +26,42 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationPulsar:
     r"""The values required to configure the destination."""
     
     batching_enabled: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_enabled') }})
-
     r"""Control whether automatic batching of messages is enabled for the producer."""
     batching_max_messages: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_max_messages') }})
-
     r"""Maximum number of messages permitted in a batch."""
     batching_max_publish_delay: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batching_max_publish_delay') }})
-
     r"""Time period in milliseconds within which the messages sent will be batched."""
     block_if_queue_full: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_if_queue_full') }})
-
     r"""If the send operation should block when the outgoing message queue is full."""
     brokers: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('brokers') }})
-
     r"""A list of host/port pairs to use for establishing the initial connection to the Pulsar cluster."""
     compression_type: DestinationPulsarCompressionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type') }})
-
     r"""Compression type for the producer."""
     destination_type: DestinationPulsarPulsarEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     max_pending_messages: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_pending_messages') }})
-
     r"""The maximum size of a queue holding pending messages."""
     max_pending_messages_across_partitions: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_pending_messages_across_partitions') }})
-
     r"""The maximum number of pending messages across partitions."""
     send_timeout_ms: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('send_timeout_ms') }})
-
     r"""If a message is not acknowledged by a server before the send-timeout expires, an error occurs (in ms)."""
     topic_namespace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_namespace') }})
-
     r"""The administrative unit of the topic, which acts as a grouping mechanism for related topics. Most topic configuration is performed at the namespace level. Each tenant has one or multiple namespaces."""
     topic_pattern: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_pattern') }})
-
     r"""Topic pattern in which the records will be sent. You can use patterns like '{namespace}' and/or '{stream}' to send the message to a specific topic based on these values. Notice that the topic name will be transformed to a standard naming convention."""
     topic_tenant: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_tenant') }})
-
     r"""The topic tenant within the instance. Tenants are essential to multi-tenancy in Pulsar, and spread across clusters."""
     topic_type: DestinationPulsarTopicTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_type') }})
-
     r"""It identifies type of topic. Pulsar supports two kind of topics: persistent and non-persistent. In persistent topic, all messages are durably persisted on disk (that means on multiple disks unless the broker is standalone), whereas non-persistent topic does not persist message into storage disk."""
     use_tls: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('use_tls') }})
-
     r"""Whether to use TLS encryption on the connection."""
     producer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('producer_name'), 'exclude': lambda f: f is None }})
-
     r"""Name for the producer. If not filled, the system will generate a globally unique name which can be accessed with."""
     producer_sync: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('producer_sync'), 'exclude': lambda f: f is None }})
-
     r"""Wait synchronously until the record has been sent to Pulsar."""
     topic_test: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('topic_test'), 'exclude': lambda f: f is None }})
-
     r"""Topic to test if Airbyte can produce messages."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_rabbitmq.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_rabbitmq.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,33 +13,24 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRabbitmq:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationRabbitmqRabbitmqEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The RabbitMQ host name."""
     routing_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('routing_key') }})
-
     r"""The routing key."""
     exchange: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('exchange'), 'exclude': lambda f: f is None }})
-
     r"""The exchange name."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password to connect."""
     port: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     r"""The RabbitMQ port."""
     ssl: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl'), 'exclude': lambda f: f is None }})
-
     r"""SSL enabled."""
     username: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username'), 'exclude': lambda f: f is None }})
-
     r"""The username to connect."""
     virtual_host: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('virtual_host'), 'exclude': lambda f: f is None }})
-
     r"""The RabbitMQ virtual host name."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_redis.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,134 +20,108 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedisSslModeVerifyFull:
     r"""Verify-full SSL mode."""
     
     ca_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ca_certificate') }})
-
     r"""CA certificate"""
     client_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_certificate') }})
-
     r"""Client certificate"""
     client_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key') }})
-
     r"""Client key"""
     mode: DestinationRedisSslModeVerifyFullModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     client_key_password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key_password'), 'exclude': lambda f: f is None }})
-
     r"""Password for keystorage. If you do not add it - the password will be generated automatically."""
     
 class DestinationRedisSslModeDisableModeEnum(str, Enum):
     DISABLE = 'disable'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedisSslModeDisable:
     r"""Disable SSL."""
     
     mode: DestinationRedisSslModeDisableModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedisTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationRedisTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedisTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationRedisTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedisTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationRedisTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedis:
     r"""The values required to configure the destination."""
     
     cache_type: DestinationRedisCacheTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cache_type') }})
-
     r"""Redis cache type to store data in."""
     destination_type: DestinationRedisRedisEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Redis host to connect to."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of Redis."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username associated with Redis."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with Redis."""
     ssl: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl'), 'exclude': lambda f: f is None }})
-
     r"""Indicates whether SSL encryption protocol will be used to connect to Redis. It is recommended to use SSL connection if possible."""
     ssl_mode: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_mode'), 'exclude': lambda f: f is None }})
-
     r"""SSL connection modes.
       <li><b>verify-full</b> - This is the most secure mode. Always require encryption and verifies the identity of the source database server
     """
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_redshift.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,95 +17,81 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationRedshiftTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: DestinationRedshiftTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: DestinationRedshiftTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 class DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum(str, Enum):
     AES_CBC_ENVELOPE = 'aes_cbc_envelope'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryption:
     r"""Staging data will be encrypted using AES-CBC envelope encryption."""
     
     encryption_type: DestinationRedshiftUploadingMethodS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_type') }})
-
     key_encrypting_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key_encrypting_key'), 'exclude': lambda f: f is None }})
-
     r"""The key, base64-encoded. Must be either 128, 192, or 256 bits. Leave blank to have Airbyte generate an ephemeral key for each sync."""
     
 class DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum(str, Enum):
     NONE = 'none'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryption:
     r"""Staging data will be stored in plaintext."""
     
     encryption_type: DestinationRedshiftUploadingMethodS3StagingEncryptionNoEncryptionEncryptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_type') }})
-
     
 class DestinationRedshiftUploadingMethodS3StagingMethodEnum(str, Enum):
     S3_STAGING = 'S3 Staging'
 
 class DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum(str, Enum):
     r"""The region of the S3 staging bucket to use if utilising a COPY strategy. See <a href=\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html#:~:text=In-,Region,-%2C%20choose%20the%20AWS\\">AWS docs</a> for details."""
     UNKNOWN = ''
@@ -136,84 +122,63 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftUploadingMethodS3Staging:
     r"""The method how the data will be uploaded to the database."""
     
     access_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key_id') }})
-
     r"""This ID grants access to the above S3 staging bucket. Airbyte requires Read and Write permissions to the given bucket. See <a href=\\"https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys\\">AWS docs</a> on how to generate an access key ID and secret access key."""
     method: DestinationRedshiftUploadingMethodS3StagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     s3_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_name') }})
-
     r"""The name of the staging S3 bucket to use if utilising a COPY strategy. COPY is recommended for production workloads for better speed and scalability. See <a href=\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html\\">AWS docs</a> for more details."""
     s3_bucket_region: DestinationRedshiftUploadingMethodS3StagingS3BucketRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_region') }})
-
     r"""The region of the S3 staging bucket to use if utilising a COPY strategy. See <a href=\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html#:~:text=In-,Region,-%2C%20choose%20the%20AWS\\">AWS docs</a> for details."""
     secret_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_access_key') }})
-
     r"""The corresponding secret to the above access key id. See <a href=\\"https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys\\">AWS docs</a> on how to generate an access key ID and secret access key."""
     encryption: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption'), 'exclude': lambda f: f is None }})
-
     r"""How to encrypt the staging data"""
     file_buffer_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_buffer_count'), 'exclude': lambda f: f is None }})
-
     r"""Number of file buffers allocated for writing data. Increasing this number is beneficial for connections using Change Data Capture (CDC) and up to the number of streams within a connection. Increasing the number of file buffers past the maximum number of streams has deteriorating effects"""
     file_name_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_name_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The pattern allows you to set the file-name format for the S3 staging file(s)"""
     purge_staging_data: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purge_staging_data'), 'exclude': lambda f: f is None }})
-
     r"""Whether to delete the staging files from S3 after completing the sync. See <a href=\\"https://docs.airbyte.com/integrations/destinations/redshift/#:~:text=the%20root%20directory.-,Purge%20Staging%20Data,-Whether%20to%20delete\\"> docs</a> for details."""
     s3_bucket_path: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_path'), 'exclude': lambda f: f is None }})
-
     r"""The directory under the S3 bucket where data will be written. If not provided, then defaults to the root directory. See <a href=\\"https://docs.aws.amazon.com/prescriptive-guidance/latest/defining-bucket-names-data-lakes/faq.html#:~:text=be%20globally%20unique.-,For%20S3%20bucket%20paths,-%2C%20you%20can%20use\\">path's name recommendations</a> for more details."""
     
 class DestinationRedshiftUploadingMethodStandardMethodEnum(str, Enum):
     STANDARD = 'Standard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshiftUploadingMethodStandard:
     r"""The method how the data will be uploaded to the database."""
     
     method: DestinationRedshiftUploadingMethodStandardMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationRedshift:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     destination_type: DestinationRedshiftRedshiftEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Host Endpoint of the Redshift Cluster (must include the cluster-id, region and end with .redshift.amazonaws.com)"""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Password associated with the username."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database."""
     schema: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema') }})
-
     r"""The default schema tables are written to if the source does not specify a namespace. Unless specifically configured, the usual value for this field is \\"public\\"."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     uploading_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('uploading_method'), 'exclude': lambda f: f is None }})
-
     r"""The method how the data will be uploaded to the database."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_rockset.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_woocommerce.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import date
 from enum import Enum
-from typing import Optional
+from marshmallow import fields
 
-class DestinationRocksetRocksetEnum(str, Enum):
-    ROCKSET = 'rockset'
+class SourceWoocommerceWoocommerceEnum(str, Enum):
+    WOOCOMMERCE = 'woocommerce'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class DestinationRockset:
-    r"""The values required to configure the destination."""
+class SourceWoocommerce:
+    r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""Rockset api key"""
-    destination_type: DestinationRocksetRocksetEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
-    workspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace') }})
-
-    r"""The Rockset workspace in which collections will be created + written to."""
-    api_server: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_server'), 'exclude': lambda f: f is None }})
-
-    r"""Rockset api URL"""
+    r"""Customer Key for API in WooCommerce shop"""
+    api_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_secret') }})
+    r"""Customer Secret for API in WooCommerce shop"""
+    shop: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shop') }})
+    r"""The name of the store. For https://EXAMPLE.com, the shop name is 'EXAMPLE.com'."""
+    source_type: SourceWoocommerceWoocommerceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
+    r"""The date you would like to replicate data from. Format: YYYY-MM-DD"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_s3.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,57 +26,48 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatParquetColumnarStorage:
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     
     format_type: DestinationS3FormatParquetColumnarStorageFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     block_size_mb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_size_mb'), 'exclude': lambda f: f is None }})
-
     r"""This is the size of a row group being buffered in memory. It limits the memory usage when writing. Larger values will improve the IO when reading, but consume more memory when writing. Default: 128 MB."""
     compression_codec: Optional[DestinationS3FormatParquetColumnarStorageCompressionCodecEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_codec'), 'exclude': lambda f: f is None }})
-
     r"""The compression algorithm used to compress data pages."""
     dictionary_encoding: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dictionary_encoding'), 'exclude': lambda f: f is None }})
-
     r"""Default: true."""
     dictionary_page_size_kb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dictionary_page_size_kb'), 'exclude': lambda f: f is None }})
-
     r"""There is one dictionary page per column per row group when dictionary encoding is used. The dictionary page size works like the page size but for dictionary. Default: 1024 KB."""
     max_padding_size_mb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_padding_size_mb'), 'exclude': lambda f: f is None }})
-
     r"""Maximum size allowed as padding to align row groups. This is also the minimum size of a row group. Default: 8 MB."""
     page_size_kb: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page_size_kb'), 'exclude': lambda f: f is None }})
-
     r"""The page size is for compression. A block is composed of pages. A page is the smallest unit that must be read fully to access a single record. If this value is too small, the compression will deteriorate. Default: 1024 KB."""
     
 class DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum(str, Enum):
     GZIP = 'GZIP'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIP:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum(str, Enum):
     NO_COMPRESSION = 'No Compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompression:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationS3FormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum(str, Enum):
     r"""Whether the input json data should be normalized (flattened) in the output JSON Lines. Please refer to docs for details."""
     NO_FLATTENING = 'No flattening'
     ROOT_LEVEL_FLATTENING = 'Root level flattening'
 
 class DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum(str, Enum):
@@ -85,45 +76,40 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatJSONLinesNewlineDelimitedJSON:
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     
     format_type: DestinationS3FormatJSONLinesNewlineDelimitedJSONFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression'), 'exclude': lambda f: f is None }})
-
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     flattening: Optional[DestinationS3FormatJSONLinesNewlineDelimitedJSONFlatteningEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flattening'), 'exclude': lambda f: f is None }})
-
     r"""Whether the input json data should be normalized (flattened) in the output JSON Lines. Please refer to docs for details."""
     
 class DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum(str, Enum):
     GZIP = 'GZIP'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIP:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".csv.gz\\")."""
     
     compression_type: Optional[DestinationS3FormatCSVCommaSeparatedValuesCompressionGZIPCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum(str, Enum):
     NO_COMPRESSION = 'No Compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompression:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".csv.gz\\")."""
     
     compression_type: Optional[DestinationS3FormatCSVCommaSeparatedValuesCompressionNoCompressionCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum(str, Enum):
     r"""Whether the input json data should be normalized (flattened) in the output CSV. Please refer to docs for details."""
     NO_FLATTENING = 'No flattening'
     ROOT_LEVEL_FLATTENING = 'Root level flattening'
 
 class DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum(str, Enum):
@@ -132,120 +118,105 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatCSVCommaSeparatedValues:
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     
     flattening: DestinationS3FormatCSVCommaSeparatedValuesFlatteningEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flattening') }})
-
     r"""Whether the input json data should be normalized (flattened) in the output CSV. Please refer to docs for details."""
     format_type: DestinationS3FormatCSVCommaSeparatedValuesFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression'), 'exclude': lambda f: f is None }})
-
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".csv.gz\\")."""
     
 class DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum(str, Enum):
     SNAPPY = 'snappy'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvroCompressionCodecSnappy:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationS3FormatAvroApacheAvroCompressionCodecSnappyCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     
 class DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum(str, Enum):
     ZSTANDARD = 'zstandard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvroCompressionCodecZstandard:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationS3FormatAvroApacheAvroCompressionCodecZstandardCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     compression_level: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_level') }})
-
     r"""Negative levels are 'fast' modes akin to lz4 or snappy, levels above 9 are generally for archival purposes, and levels above 18 use a lot of memory."""
     include_checksum: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_checksum'), 'exclude': lambda f: f is None }})
-
     r"""If true, include a checksum with each data block."""
     
 class DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum(str, Enum):
     XZ = 'xz'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvroCompressionCodecXz:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationS3FormatAvroApacheAvroCompressionCodecXzCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     compression_level: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_level') }})
-
     r"""See <a href=\\"https://commons.apache.org/proper/commons-compress/apidocs/org/apache/commons/compress/compressors/xz/XZCompressorOutputStream.html#XZCompressorOutputStream-java.io.OutputStream-int-\\">here</a> for details."""
     
 class DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum(str, Enum):
     BZIP2 = 'bzip2'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvroCompressionCodecBzip2:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationS3FormatAvroApacheAvroCompressionCodecBzip2CodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     
 class DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum(str, Enum):
     DEFLATE = 'Deflate'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvroCompressionCodecDeflate:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationS3FormatAvroApacheAvroCompressionCodecDeflateCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     compression_level: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_level') }})
-
     r"""0: no compression & fastest, 9: best compression & slowest."""
     
 class DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum(str, Enum):
     NO_COMPRESSION = 'no compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvroCompressionCodecNoCompression:
     r"""The compression algorithm used to compress data. Default to no compression."""
     
     codec: DestinationS3FormatAvroApacheAvroCompressionCodecNoCompressionCodecEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('codec') }})
-
     
 class DestinationS3FormatAvroApacheAvroFormatTypeEnum(str, Enum):
     AVRO = 'Avro'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3FormatAvroApacheAvro:
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     
     compression_codec: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_codec') }})
-
     r"""The compression algorithm used to compress data. Default to no compression."""
     format_type: DestinationS3FormatAvroApacheAvroFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     
 class DestinationS3S3BucketRegionEnum(str, Enum):
     r"""The region of the S3 bucket. See <a href=\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions\\">here</a> for all region codes."""
     UNKNOWN = ''
     US_EAST_1 = 'us-east-1'
     US_EAST_2 = 'us-east-2'
     US_WEST_1 = 'us-west-1'
@@ -275,36 +246,26 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationS3S3Enum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     format: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     s3_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_name') }})
-
     r"""The name of the S3 bucket. Read more <a href=\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html\\">here</a>."""
     s3_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_path') }})
-
     r"""Directory under the S3 bucket where data will be written. Read more <a href=\\"https://docs.airbyte.com/integrations/destinations/s3#:~:text=to%20format%20the-,bucket%20path,-%3A\\">here</a>"""
     s3_bucket_region: DestinationS3S3BucketRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_region') }})
-
     r"""The region of the S3 bucket. See <a href=\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions\\">here</a> for all region codes."""
     access_key_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key_id'), 'exclude': lambda f: f is None }})
-
     r"""The access key ID to access the S3 bucket. Airbyte requires Read and Write permissions to the given bucket. Read more <a href=\\"https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys\\">here</a>."""
     file_name_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_name_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The pattern allows you to set the file-name format for the S3 staging file(s)"""
     s3_endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_endpoint'), 'exclude': lambda f: f is None }})
-
     r"""Your S3 endpoint url. Read more <a href=\\"https://docs.aws.amazon.com/general/latest/gr/s3.html#:~:text=Service%20endpoints-,Amazon%20S3%20endpoints,-When%20you%20use\\">here</a>"""
     s3_path_format: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_path_format'), 'exclude': lambda f: f is None }})
-
     r"""Format string on how data will be organized inside the S3 bucket directory. Read more <a href=\\"https://docs.airbyte.com/integrations/destinations/s3#:~:text=The%20full%20path%20of%20the%20output%20data%20with%20the%20default%20S3%20path%20format\\">here</a>"""
     secret_access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_access_key'), 'exclude': lambda f: f is None }})
-
     r"""The corresponding secret to the access key ID. Read more <a href=\\"https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys\\">here</a>"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_s3_glue.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_s3_glue.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,25 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIP:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionGZIPCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum(str, Enum):
     NO_COMPRESSION = 'No Compression'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompression:
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     
     compression_type: Optional[DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONCompressionNoCompressionCompressionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum(str, Enum):
     r"""Whether the input json data should be normalized (flattened) in the output JSON Lines. Please refer to docs for details."""
     NO_FLATTENING = 'No flattening'
     ROOT_LEVEL_FLATTENING = 'Root level flattening'
 
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum(str, Enum):
@@ -45,20 +43,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3GlueFormatJSONLinesNewlineDelimitedJSON:
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     
     format_type: DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     compression: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('compression'), 'exclude': lambda f: f is None }})
-
     r"""Whether the output files should be compressed. If compression is selected, the output filename will have an extra extension (GZIP: \\".jsonl.gz\\")."""
     flattening: Optional[DestinationS3GlueFormatJSONLinesNewlineDelimitedJSONFlatteningEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('flattening'), 'exclude': lambda f: f is None }})
-
     r"""Whether the input json data should be normalized (flattened) in the output JSON Lines. Please refer to docs for details."""
     
 class DestinationS3GlueSerializationLibraryEnum(str, Enum):
     r"""The library that your query engine will use for reading and writing data in your lake."""
     ORG_OPENX_DATA_JSONSERDE_JSON_SER_DE = 'org.openx.data.jsonserde.JsonSerDe'
     ORG_APACHE_HIVE_HCATALOG_DATA_JSON_SER_DE = 'org.apache.hive.hcatalog.data.JsonSerDe'
 
@@ -94,42 +89,30 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationS3Glue:
     r"""The values required to configure the destination."""
     
     destination_type: DestinationS3GlueS3GlueEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     format: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-
     r"""Format of the data output. See <a href=\\"https://docs.airbyte.com/integrations/destinations/s3/#supported-output-schema\\">here</a> for more details"""
     glue_database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('glue_database') }})
-
     r"""Name of the glue database for creating the tables, leave blank if no integration"""
     glue_serialization_library: DestinationS3GlueSerializationLibraryEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('glue_serialization_library') }})
-
     r"""The library that your query engine will use for reading and writing data in your lake."""
     s3_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_name') }})
-
     r"""The name of the S3 bucket. Read more <a href=\\"https://docs.aws.amazon.com/AmazonS3/latest/userguide/create-bucket-overview.html\\">here</a>."""
     s3_bucket_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_path') }})
-
     r"""Directory under the S3 bucket where data will be written. Read more <a href=\\"https://docs.airbyte.com/integrations/destinations/s3#:~:text=to%20format%20the-,bucket%20path,-%3A\\">here</a>"""
     s3_bucket_region: DestinationS3GlueS3BucketRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_region') }})
-
     r"""The region of the S3 bucket. See <a href=\\"https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html#concepts-available-regions\\">here</a> for all region codes."""
     access_key_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key_id'), 'exclude': lambda f: f is None }})
-
     r"""The access key ID to access the S3 bucket. Airbyte requires Read and Write permissions to the given bucket. Read more <a href=\\"https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys\\">here</a>."""
     file_name_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_name_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The pattern allows you to set the file-name format for the S3 staging file(s)"""
     s3_endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_endpoint'), 'exclude': lambda f: f is None }})
-
     r"""Your S3 endpoint url. Read more <a href=\\"https://docs.aws.amazon.com/general/latest/gr/s3.html#:~:text=Service%20endpoints-,Amazon%20S3%20endpoints,-When%20you%20use\\">here</a>"""
     s3_path_format: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_path_format'), 'exclude': lambda f: f is None }})
-
     r"""Format string on how data will be organized inside the S3 bucket directory. Read more <a href=\\"https://docs.airbyte.com/integrations/destinations/s3#:~:text=The%20full%20path%20of%20the%20output%20data%20with%20the%20default%20S3%20path%20format\\">here</a>"""
     secret_access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_access_key'), 'exclude': lambda f: f is None }})
-
     r"""The corresponding secret to the access key ID. Read more <a href=\\"https://docs.aws.amazon.com/general/latest/gr/aws-sec-cred-types.html#access-keys-and-secret-access-keys\\">here</a>"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_scylla.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_scylla.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationScylla:
     r"""The values required to configure the destination."""
     
     address: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address') }})
-
     r"""Address to connect to."""
     destination_type: DestinationScyllaScyllaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     keyspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('keyspace') }})
-
     r"""Default Scylla keyspace to create data in."""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Password associated with Scylla."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of Scylla."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access Scylla."""
     replication: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication'), 'exclude': lambda f: f is None }})
-
     r"""Indicates to how many nodes the data should be replicated to."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_sftp_json.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_sftp_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSftpJSON:
     r"""The values required to configure the destination."""
     
     destination_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destination_path') }})
-
     r"""Path to the directory where json files will be written."""
     destination_type: DestinationSftpJSONSftpJSONEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the SFTP server."""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Password associated with the username."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the SFTP server."""
     port: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     r"""Port of the SFTP server."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_snowflake.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,57 +12,47 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeCredentialsUsernameAndPassword:
     
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Enter the password associated with the username."""
     auth_type: Optional[DestinationSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum(str, Enum):
     KEY_PAIR_AUTHENTICATION = 'Key Pair Authentication'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeCredentialsKeyPairAuthentication:
     
     private_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('private_key') }})
-
     r"""RSA Private key to use for Snowflake connection. See the <a href=\\"https://docs.airbyte.com/integrations/destinations/snowflake\\">docs</a> for more information on how to obtain this key."""
     auth_type: Optional[DestinationSnowflakeCredentialsKeyPairAuthenticationAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     private_key_password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('private_key_password'), 'exclude': lambda f: f is None }})
-
     r"""Passphrase for private key"""
     
 class DestinationSnowflakeCredentialsOAuth20AuthTypeEnum(str, Enum):
     O_AUTH2_0 = 'OAuth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Enter you application's Access Token"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Enter your application's Refresh Token"""
     auth_type: Optional[DestinationSnowflakeCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
     r"""Enter your application's Client ID"""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""Enter your application's Client secret"""
     
 class DestinationSnowflakeSnowflakeEnum(str, Enum):
     SNOWFLAKE = 'snowflake'
 
 class DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum(str, Enum):
     AZURE_BLOB_STAGING = 'Azure Blob Staging'
@@ -70,75 +60,63 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodAzureBlobStorageStaging:
     r"""Recommended for large production workloads for better speed and scalability."""
     
     azure_blob_storage_account_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_name') }})
-
     r"""Enter your Azure Blob Storage account name"""
     azure_blob_storage_container_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_container_name') }})
-
     r"""Enter your Azure Blob Storage <a href=\\"https://docs.microsoft.com/en-us/rest/api/storageservices/naming-and-referencing-containers--blobs--and-metadata#container-names\\">container name</a>"""
     azure_blob_storage_sas_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_sas_token') }})
-
     r"""Enter the <a href=\\"https://docs.snowflake.com/en/user-guide/data-load-azure-config.html#option-2-generating-a-sas-token\\">Shared access signature</a> (SAS) token to grant Snowflake limited access to objects in your Azure Blob Storage account"""
     method: DestinationSnowflakeLoadingMethodAzureBlobStorageStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     azure_blob_storage_endpoint_domain_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_endpoint_domain_name'), 'exclude': lambda f: f is None }})
-
     r"""Enter the Azure Blob Storage <a href=\\"https://docs.microsoft.com/en-us/azure/storage/common/storage-account-overview#storage-account-endpoints\\">endpoint domain name</a>"""
     
 class DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum(str, Enum):
     GCS_STAGING = 'GCS Staging'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodGoogleCloudStorageStaging:
     r"""Recommended for large production workloads for better speed and scalability."""
     
     bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bucket_name') }})
-
     r"""Enter the <a href=\\"https://cloud.google.com/storage/docs/creating-buckets\\">Cloud Storage bucket name</a>"""
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""Enter your <a href=\\"https://cloud.google.com/iam/docs/creating-managing-service-account-keys#creating_service_account_keys\\">Google Cloud service account key</a> in the JSON format with read/write access to your Cloud Storage staging bucket"""
     method: DestinationSnowflakeLoadingMethodGoogleCloudStorageStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""Enter the <a href=\\"https://cloud.google.com/resource-manager/docs/creating-managing-projects#identifying_projects\\">Google Cloud project ID</a>"""
     
 class DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum(str, Enum):
     AES_CBC_ENVELOPE = 'aes_cbc_envelope'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryption:
     r"""Staging data will be encrypted using AES-CBC envelope encryption."""
     
     encryption_type: DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionAESCBCEnvelopeEncryptionEncryptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_type') }})
-
     key_encrypting_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key_encrypting_key'), 'exclude': lambda f: f is None }})
-
     r"""The key, base64-encoded. Must be either 128, 192, or 256 bits. Leave blank to have Airbyte generate an ephemeral key for each sync."""
     
 class DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum(str, Enum):
     NONE = 'none'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryption:
     r"""Staging data will be stored in plaintext."""
     
     encryption_type: DestinationSnowflakeLoadingMethodAWSS3StagingEncryptionNoEncryptionEncryptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_type') }})
-
     
 class DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum(str, Enum):
     S3_STAGING = 'S3 Staging'
 
 class DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum(str, Enum):
     r"""Enter the region where your S3 bucket resides"""
     UNKNOWN = ''
@@ -169,92 +147,71 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodAWSS3Staging:
     r"""Recommended for large production workloads for better speed and scalability."""
     
     access_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key_id') }})
-
     r"""Enter your <a href=\\"https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html\\">AWS access key ID</a>. Airbyte requires Read and Write permissions on your S3 bucket"""
     method: DestinationSnowflakeLoadingMethodAWSS3StagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     s3_bucket_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_name') }})
-
     r"""Enter your S3 bucket name"""
     secret_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_access_key') }})
-
     r"""Enter your <a href=\\"https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html\\">AWS secret access key</a>"""
     encryption: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption'), 'exclude': lambda f: f is None }})
-
     r"""Choose a data encryption method for the staging data"""
     file_name_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_name_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The pattern allows you to set the file-name format for the S3 staging file(s)"""
     purge_staging_data: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('purge_staging_data'), 'exclude': lambda f: f is None }})
-
     r"""Toggle to delete staging files from the S3 bucket after a successful sync"""
     s3_bucket_region: Optional[DestinationSnowflakeLoadingMethodAWSS3StagingS3BucketRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('s3_bucket_region'), 'exclude': lambda f: f is None }})
-
     r"""Enter the region where your S3 bucket resides"""
     
 class DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum(str, Enum):
     INTERNAL_STAGING = 'Internal Staging'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodRecommendedInternalStaging:
     r"""Recommended for large production workloads for better speed and scalability."""
     
     method: DestinationSnowflakeLoadingMethodRecommendedInternalStagingMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum(str, Enum):
     STANDARD = 'Standard'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflakeLoadingMethodSelectAnotherOption:
     r"""Select another option"""
     
     method: DestinationSnowflakeLoadingMethodSelectAnotherOptionMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationSnowflake:
     r"""The values required to configure the destination."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Enter the name of the <a href=\\"https://docs.snowflake.com/en/sql-reference/ddl-database.html#database-schema-share-ddl\\">database</a> you want to sync data into"""
     destination_type: DestinationSnowflakeSnowflakeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Enter your Snowflake account's <a href=\\"https://docs.snowflake.com/en/user-guide/admin-account-identifier.html#using-an-account-locator-as-an-identifier\\">locator</a> (in the format <account_locator>.<region>.<cloud>.snowflakecomputing.com)"""
     role: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role') }})
-
     r"""Enter the <a href=\\"https://docs.snowflake.com/en/user-guide/security-access-control-overview.html#roles\\">role</a> that you want to use to access Snowflake"""
     schema: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema') }})
-
     r"""Enter the name of the default <a href=\\"https://docs.snowflake.com/en/sql-reference/ddl-database.html#database-schema-share-ddl\\">schema</a>"""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Enter the name of the user you want to use to access the database"""
     warehouse: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warehouse') }})
-
     r"""Enter the name of the <a href=\\"https://docs.snowflake.com/en/user-guide/warehouses-overview.html#overview-of-warehouses\\">warehouse</a> that you want to sync data into"""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     file_buffer_count: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_buffer_count'), 'exclude': lambda f: f is None }})
-
     r"""Number of file buffers allocated for writing data. Increasing this number is beneficial for connections using Change Data Capture (CDC) and up to the number of streams within a connection. Increasing the number of file buffers past the maximum number of streams has deteriorating effects"""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Enter the additional properties to pass to the JDBC URL string when connecting to the database (formatted as key=value pairs separated by the symbol &). Example: key1=value1&key2=value2&key3=value3"""
     loading_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('loading_method'), 'exclude': lambda f: f is None }})
-
     r"""Select a data staging method"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destination_typesense.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_typesense.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationTypesense:
     r"""The values required to configure the destination."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Typesense API Key"""
     destination_type: DestinationTypesenseTypesenseEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the Typesense instance without protocol."""
     batch_size: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batch_size'), 'exclude': lambda f: f is None }})
-
     r"""How many documents should be imported together. Default 1000"""
     port: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     r"""Port of the Typesense instance. Ex: 8108, 80, 443. Default is 443"""
     protocol: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('protocol'), 'exclude': lambda f: f is None }})
-
     r"""Protocol of the Typesense instance. Ex: http or https. Default is https"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destinationcreaterequest.py` & `airbyte-1.7.1/src/airbyte/models/shared/destinationcreaterequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,11 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationCreateRequest:
     
     configuration: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configuration') }})
-
     r"""The values required to configure the destination."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destinationresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/destinationresponse.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,11 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationResponse:
     r"""Provides details of a single destination."""
     
     destination_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationId') }})
-
     destination_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
-
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/destinationsresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/destinationsresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,13 +9,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class DestinationsResponse:
     r"""Successful operation"""
     
     data: list[shared_destinationresponse.DestinationResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-
     next: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next') }})
-
     previous: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/jobcreaterequest.py` & `airbyte-1.7.1/src/airbyte/models/shared/jobcreaterequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class JobCreateRequest:
     r"""Creates a new Job from the configuration provided in the request body."""
     
     connection_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionId') }})
-
     job_type: shared_jobtypeenum_enum.JobTypeEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobType') }})
-
     r"""Enum that describes the different types of jobs that the platform runs."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/jobresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/jobresponse.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,17 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class JobResponse:
     r"""Provides details of a single job."""
     
     job_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobId') }})
-
     job_type: shared_jobtypeenum_enum.JobTypeEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jobType') }})
-
     r"""Enum that describes the different types of jobs that the platform runs."""
     start_time: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('startTime') }})
-
     status: shared_jobstatusenum_enum.JobStatusEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
-
     bytes_synced: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bytesSynced'), 'exclude': lambda f: f is None }})
-
     duration: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('duration'), 'exclude': lambda f: f is None }})
-
     r"""Duration of a sync in ISO_8601 format"""
     last_updated_at: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastUpdatedAt'), 'exclude': lambda f: f is None }})
-
     rows_synced: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rowsSynced'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/jobsresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/jobsresponse.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,13 +9,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class JobsResponse:
     r"""List all the Jobs by connectionId."""
     
     data: list[shared_jobresponse.JobResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-
     next: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next') }})
-
     previous: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_airtable.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_airtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,52 +15,42 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAirtableCredentialsPersonalAccessToken:
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""The Personal Access Token for the Airtable account. See the <a href=\\"https://airtable.com/developers/web/guides/personal-access-tokens\\">Support Guide</a> for more information on how to obtain this token."""
     auth_method: Optional[SourceAirtableCredentialsPersonalAccessTokenAuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     
 class SourceAirtableCredentialsOAuth20AuthMethodEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAirtableCredentialsOAuth20:
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The client ID of the Airtable developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The client secret the Airtable developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The key to refresh the expired access token."""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access Token for making authenticated requests."""
     auth_method: Optional[SourceAirtableCredentialsOAuth20AuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     token_expiry_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date-time when the access token should be refreshed."""
     
 class SourceAirtableAirtableEnum(str, Enum):
     AIRTABLE = 'airtable'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAirtable:
     r"""The values required to configure the source."""
     
     source_type: SourceAirtableAirtableEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_alloydb.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_alloydb.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAlloydbReplicationMethodStandard:
     r"""Standard replication requires no setup on the DB side but will not be able to represent deletions incrementally."""
     
     method: SourceAlloydbReplicationMethodStandardMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class SourceAlloydbAlloydbEnum(str, Enum):
     ALLOYDB = 'alloydb'
 
 class SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
@@ -29,103 +28,81 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAlloydbTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceAlloydbTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAlloydbTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceAlloydbTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAlloydbTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: SourceAlloydbTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAlloydb:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database."""
     source_type: SourceAlloydbAlloydbEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (Eg. key1=value1&key2=value2&key3=value3). For more information read about <a href=\\"https://jdbc.postgresql.org/documentation/head/connect.html\\">JDBC URL parameters</a>."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with the username."""
     replication_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_method'), 'exclude': lambda f: f is None }})
-
     r"""Replication method for extracting data from the database."""
     schemas: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schemas'), 'exclude': lambda f: f is None }})
-
     r"""The list of schemas (case sensitive) to sync from. Defaults to public."""
     ssl_mode: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_mode'), 'exclude': lambda f: f is None }})
-
     r"""SSL connection modes.
       Read more <a href=\"https://jdbc.postgresql.org/documentation/head/ssl-client.html\"> in the docs</a>.
     """
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_amazon_ads.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_amazon_ads.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,38 +37,27 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAmazonAds:
     r"""The values required to configure the source."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The client ID of your Amazon Ads developer application. See the <a href=\\"https://advertising.amazon.com/API/docs/en-us/get-started/generate-api-tokens#retrieve-your-client-id-and-client-secret\\">docs</a> for more information."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The client secret of your Amazon Ads developer application. See the <a href=\\"https://advertising.amazon.com/API/docs/en-us/get-started/generate-api-tokens#retrieve-your-client-id-and-client-secret\\">docs</a> for more information."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Amazon Ads refresh token. See the <a href=\\"https://advertising.amazon.com/API/docs/en-us/get-started/generate-api-tokens\\">docs</a> for more information on how to obtain this token."""
     source_type: SourceAmazonAdsAmazonAdsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     auth_type: Optional[SourceAmazonAdsAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     look_back_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('look_back_window'), 'exclude': lambda f: f is None }})
-
     r"""The amount of days to go back in time to get the updated data from Amazon Ads"""
     profiles: Optional[list[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('profiles'), 'exclude': lambda f: f is None }})
-
     r"""Profile IDs you want to fetch data for. See <a href=\\"https://advertising.amazon.com/API/docs/en-us/concepts/authorization/profiles\\">docs</a> for more details."""
     region: Optional[SourceAmazonAdsRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
-
     r"""Region to pull data from (EU/NA/FE). See <a href=\\"https://advertising.amazon.com/API/docs/en-us/info/api-overview#api-endpoints\\">docs</a> for more details."""
     report_record_types: Optional[list[SourceAmazonAdsReportRecordTypesEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('report_record_types'), 'exclude': lambda f: f is None }})
-
     r"""Optional configuration which accepts an array of string of record types. Leave blank for default behaviour to pull all report types. Use this config option only if you want to pull specific report type(s). See <a href=\\"https://advertising.amazon.com/API/docs/en-us/reporting/v2/report-types\\">docs</a> for more details"""
     start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'exclude': lambda f: f is None }})
-
     r"""The Start date for collecting reports, should not be more than 60 days in the past. In YYYY-MM-DD format"""
     state_filter: Optional[list[SourceAmazonAdsStateFilterEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state_filter'), 'exclude': lambda f: f is None }})
-
     r"""Reflects the state of the Display, Product, and Brand Campaign streams as enabled, paused, or archived. If you do not populate this field, it will be ignored completely."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_amazon_seller_partner.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_amazon_seller_partner.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,53 +46,37 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAmazonSellerPartner:
     r"""The values required to configure the source."""
     
     app_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('app_id') }})
-
     r"""Your Amazon App ID"""
     aws_environment: SourceAmazonSellerPartnerAWSEnvironmentEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_environment') }})
-
     r"""An enumeration."""
     lwa_app_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lwa_app_id') }})
-
     r"""Your Login with Amazon Client ID."""
     lwa_client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lwa_client_secret') }})
-
     r"""Your Login with Amazon Client Secret."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The Refresh Token obtained via OAuth flow authorization."""
     region: SourceAmazonSellerPartnerAWSRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
-
     r"""An enumeration."""
     replication_start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_start_date') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     source_type: SourceAmazonSellerPartnerAmazonSellerPartnerEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     auth_type: Optional[SourceAmazonSellerPartnerAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     aws_access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_access_key'), 'exclude': lambda f: f is None }})
-
     r"""Specifies the AWS access key used as part of the credentials to authenticate the user."""
     aws_secret_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_secret_key'), 'exclude': lambda f: f is None }})
-
     r"""Specifies the AWS secret key used as part of the credentials to authenticate the user."""
     max_wait_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_wait_seconds'), 'exclude': lambda f: f is None }})
-
     r"""Sometimes report can take up to 30 minutes to generate. This will set the limit for how long to wait for a successful report."""
     period_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('period_in_days'), 'exclude': lambda f: f is None }})
-
     r"""Will be used for stream slicing for initial full_refresh sync when no updated state is present for reports that support sliced incremental sync."""
     replication_end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_end_date'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data after this date will not be replicated."""
     report_options: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('report_options'), 'exclude': lambda f: f is None }})
-
     r"""Additional information passed to reports. This varies by report type. Must be a valid json string."""
     role_arn: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role_arn'), 'exclude': lambda f: f is None }})
-
     r"""Specifies the Amazon Resource Name (ARN) of an IAM role that you want to use to perform operations requested using this profile. (Needs permission to 'Assume Role' STS)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_amazon_sqs.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_amazon_sqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,36 +41,26 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAmazonSqs:
     r"""The values required to configure the source."""
     
     delete_messages: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('delete_messages') }})
-
     r"""If Enabled, messages will be deleted from the SQS Queue after being read. If Disabled, messages are left in the queue and can be read more than once. WARNING: Enabling this option can result in data loss in cases of failure, use with caution, see documentation for more detail."""
     queue_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('queue_url') }})
-
     r"""URL of the SQS Queue"""
     region: SourceAmazonSqsAWSRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
-
     r"""AWS Region of the SQS Queue"""
     source_type: SourceAmazonSqsAmazonSqsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key'), 'exclude': lambda f: f is None }})
-
     r"""The Access Key ID of the AWS IAM Role to use for pulling messages"""
     attributes_to_return: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attributes_to_return'), 'exclude': lambda f: f is None }})
-
     r"""Comma separated list of Mesage Attribute names to return"""
     max_batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_batch_size'), 'exclude': lambda f: f is None }})
-
     r"""Max amount of messages to get in one batch (10 max)"""
     max_wait_time: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_wait_time'), 'exclude': lambda f: f is None }})
-
     r"""Max amount of time in seconds to wait for messages in a single poll (20 max)"""
     secret_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key'), 'exclude': lambda f: f is None }})
-
     r"""The Secret Key of the AWS IAM Role to use for pulling messages"""
     visibility_timeout: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('visibility_timeout'), 'exclude': lambda f: f is None }})
-
     r"""Modify the Visibility Timeout of the individual message from the Queue's default (seconds)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_amplitude.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_amplitude.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAmplitude:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Amplitude API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/amplitude#setup-guide\\">setup guide</a> for more information on how to obtain this key."""
     secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
-
     r"""Amplitude Secret Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/amplitude#setup-guide\\">setup guide</a> for more information on how to obtain this key."""
     source_type: SourceAmplitudeAmplitudeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""UTC date and time in the format 2021-01-25T00:00:00Z. Any data before this date will not be replicated."""
     data_region: Optional[SourceAmplitudeDataRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_region'), 'exclude': lambda f: f is None }})
-
     r"""Amplitude data region server"""
     request_time_range: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('request_time_range'), 'exclude': lambda f: f is None }})
-
     r"""According to <a href=\\"https://www.docs.developers.amplitude.com/analytics/apis/export-api/#considerations\\">Considerations</a> too big time range in request can cause a timeout error. In this case, set shorter time interval in hours."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_apify_dataset.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_apify_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceApifyDataset:
     r"""The values required to configure the source."""
     
     dataset_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('datasetId') }})
-
     r"""ID of the dataset you would like to load to Airbyte."""
     source_type: SourceApifyDatasetApifyDatasetEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     clean: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clean'), 'exclude': lambda f: f is None }})
-
     r"""If set to true, only clean items will be downloaded from the dataset. See description of what clean means in <a href=\\"https://docs.apify.com/api/v2#/reference/datasets/item-collection/get-items\\">Apify API docs</a>. If not sure, set clean to false."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_asana.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_asana.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,48 +14,40 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAsanaCredentialsAuthenticateViaAsanaOauth:
     r"""Choose how to authenticate to Github"""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     option_title: Optional[SourceAsanaCredentialsAuthenticateViaAsanaOauthCredentialsTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title'), 'exclude': lambda f: f is None }})
-
     r"""OAuth Credentials"""
     
 class SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum(str, Enum):
     r"""PAT Credentials"""
     PAT_CREDENTIALS = 'PAT Credentials'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAsanaCredentialsAuthenticateWithPersonalAccessToken:
     r"""Choose how to authenticate to Github"""
     
     personal_access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('personal_access_token') }})
-
     r"""Asana Personal Access Token (generate yours <a href=\\"https://app.asana.com/0/developer-console\\">here</a>)."""
     option_title: Optional[SourceAsanaCredentialsAuthenticateWithPersonalAccessTokenCredentialsTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title'), 'exclude': lambda f: f is None }})
-
     r"""PAT Credentials"""
     
 class SourceAsanaAsanaEnum(str, Enum):
     ASANA = 'asana'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAsana:
     r"""The values required to configure the source."""
     
     source_type: SourceAsanaAsanaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to Github"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_auth0.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_auth0.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,49 +12,40 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAuth0CredentialsOAuth2AccessToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Also called <a href=\\"https://auth0.com/docs/secure/tokens/access-tokens/get-management-api-access-tokens-for-testing\\">API Access Token </a> The access token used to call the Auth0 Management API Token. It's a JWT that contains specific grant permissions knowns as scopes."""
     auth_type: SourceAuth0CredentialsOAuth2AccessTokenAuthenticationMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     
 class SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum(str, Enum):
     OAUTH2_CONFIDENTIAL_APPLICATION = 'oauth2_confidential_application'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAuth0CredentialsOAuth2ConfidentialApplication:
     
     audience: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('audience') }})
-
     r"""The audience for the token, which is your API. You can find this in the Identifier field on your  <a href=\\"https://manage.auth0.com/#/apis\\">API's settings tab</a>"""
     auth_type: SourceAuth0CredentialsOAuth2ConfidentialApplicationAuthenticationMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""Your application's Client ID. You can find this value on the <a href=\\"https://manage.auth0.com/#/applications\\">application's settings tab</a> after you login the admin portal."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""Your application's Client Secret. You can find this value on the <a href=\\"https://manage.auth0.com/#/applications\\">application's settings tab</a> after you login the admin portal."""
     
 class SourceAuth0Auth0Enum(str, Enum):
     AUTH0 = 'auth0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAuth0:
     r"""The values required to configure the source."""
     
     base_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base_url') }})
-
     r"""The Authentication API is served over HTTPS. All URLs referenced in the documentation have the following base `https://YOUR_DOMAIN`"""
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     source_type: SourceAuth0Auth0Enum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_aws_cloudtrail.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_aws_cloudtrail.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAwsCloudtrail:
     r"""The values required to configure the source."""
     
     aws_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_key_id') }})
-
     r"""AWS CloudTrail Access Key ID. See the <a href=\\"https://docs.airbyte.com/integrations/sources/aws-cloudtrail\\">docs</a> for more information on how to obtain this key."""
     aws_region_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_region_name') }})
-
     r"""The default AWS Region to use, for example, us-west-1 or us-west-2. When specifying a Region inline during client initialization, this property is named region_name."""
     aws_secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_secret_key') }})
-
     r"""AWS CloudTrail Access Key ID. See the <a href=\\"https://docs.airbyte.com/integrations/sources/aws-cloudtrail\\">docs</a> for more information on how to obtain this key."""
     source_type: SourceAwsCloudtrailAwsCloudtrailEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date you would like to replicate data. Data in AWS CloudTrail is available for last 90 days only. Format: YYYY-MM-DD."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_azure_blob_storage.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_azure_blob_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,42 +13,33 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSON:
     r"""Input data format"""
     
     format_type: SourceAzureBlobStorageFormatJSONLinesNewlineDelimitedJSONFormatTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format_type') }})
-
     
 class SourceAzureBlobStorageAzureBlobStorageEnum(str, Enum):
     AZURE_BLOB_STORAGE = 'azure-blob-storage'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAzureBlobStorage:
     r"""The values required to configure the source."""
     
     azure_blob_storage_account_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_key') }})
-
     r"""The Azure blob storage account key."""
     azure_blob_storage_account_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_account_name') }})
-
     r"""The account's name of the Azure Blob Storage."""
     azure_blob_storage_container_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_container_name') }})
-
     r"""The name of the Azure blob storage container."""
     format: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-
     r"""Input data format"""
     source_type: SourceAzureBlobStorageAzureBlobStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     azure_blob_storage_blobs_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_blobs_prefix'), 'exclude': lambda f: f is None }})
-
     r"""The Azure blob storage prefix to be applied"""
     azure_blob_storage_endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_endpoint'), 'exclude': lambda f: f is None }})
-
     r"""This is Azure Blob Storage endpoint domain name. Leave default value (or leave it empty if run container from command line) to use Microsoft native from example."""
     azure_blob_storage_schema_inference_limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('azure_blob_storage_schema_inference_limit'), 'exclude': lambda f: f is None }})
-
     r"""The Azure blob storage blobs to scan for inferring the schema, useful on large amounts of data with consistent structure"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_azure_table.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_azure_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceAzureTable:
     r"""The values required to configure the source."""
     
     source_type: SourceAzureTableAzureTableEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     storage_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage_access_key') }})
-
     r"""Azure Table Storage Access Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/azure-table\\">docs</a> for more information on how to obtain this key."""
     storage_account_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage_account_name') }})
-
     r"""The name of your storage account."""
     storage_endpoint_suffix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage_endpoint_suffix'), 'exclude': lambda f: f is None }})
-
     r"""Azure Table Storage service account URL suffix. See the <a href=\\"https://docs.airbyte.com/integrations/sources/azure-table\\">docs</a> for more information on how to obtain endpoint suffix"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_bamboo_hr.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_bamboo_hr.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceBambooHr:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Api key of bamboo hr"""
     source_type: SourceBambooHrBambooHrEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     subdomain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain') }})
-
     r"""Sub Domain of bamboo hr"""
     custom_reports_fields: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_reports_fields'), 'exclude': lambda f: f is None }})
-
     r"""Comma-separated list of fields to include in custom reports."""
     custom_reports_include_default_fields: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_reports_include_default_fields'), 'exclude': lambda f: f is None }})
-
     r"""If true, the custom reports endpoint will include the default fields defined here: https://documentation.bamboohr.com/docs/list-of-field-names."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_bigcommerce.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_bigcommerce.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceBigcommerce:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token for making authenticated requests."""
     source_type: SourceBigcommerceBigcommerceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The date you would like to replicate data. Format: YYYY-MM-DD."""
     store_hash: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('store_hash') }})
-
     r"""The hash code of the store. For https://api.bigcommerce.com/stores/HASH_CODE/v3/, The store's hash code is 'HASH_CODE'."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_bigquery.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceBigquery:
     r"""The values required to configure the source."""
     
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""The contents of your Service Account Key JSON file. See the <a href=\\"https://docs.airbyte.com/integrations/sources/bigquery#setup-the-bigquery-source-in-airbyte\\">docs</a> for more information on how to obtain this key."""
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""The GCP project ID for the project containing the target BigQuery dataset."""
     source_type: SourceBigqueryBigqueryEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_id'), 'exclude': lambda f: f is None }})
-
     r"""The dataset ID to search for tables and views. If you are only loading data from one dataset, setting this option could result in much faster schema discovery."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_bing_ads.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_bing_ads.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,21 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceBingAds:
     r"""The values required to configure the source."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Microsoft Advertising developer application."""
     developer_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('developer_token') }})
-
     r"""Developer token associated with user. See more info <a href=\\"https://docs.microsoft.com/en-us/advertising/guides/get-started?view=bingads-13#get-developer-token\\"> in the docs</a>."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Refresh Token to renew the expired Access Token."""
     reports_start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reports_start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The start date from which to begin replicating report data. Any data generated before this date will not be replicated in reports. This is a UTC date in YYYY-MM-DD format."""
     source_type: SourceBingAdsBingAdsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     auth_method: Optional[SourceBingAdsAuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""The Client Secret of your Microsoft Advertising developer application."""
     tenant_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tenant_id'), 'exclude': lambda f: f is None }})
-
     r"""The Tenant ID of your Microsoft Advertising developer application. Set this to \\"common\\" unless you know you need a different value."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_braintree.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_braintree.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,24 +23,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceBraintree:
     r"""The values required to configure the source."""
     
     environment: SourceBraintreeEnvironmentEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('environment') }})
-
     r"""Environment specifies where the data will come from."""
     merchant_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('merchant_id') }})
-
     r"""The unique identifier for your entire gateway account. See the <a href=\\"https://docs.airbyte.com/integrations/sources/braintree\\">docs</a> for more information on how to obtain this ID."""
     private_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('private_key') }})
-
     r"""Braintree Private Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/braintree\\">docs</a> for more information on how to obtain this key."""
     public_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('public_key') }})
-
     r"""Braintree Public Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/braintree\\">docs</a> for more information on how to obtain this key."""
     source_type: SourceBraintreeBraintreeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_braze.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_braze.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceBraze:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Braze REST API key"""
     source_type: SourceBrazeBrazeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""Rows after this date will be synced"""
     url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-
     r"""Braze REST API endpoint"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_chargebee.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_chargebee.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,21 +20,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceChargebee:
     r"""The values required to configure the source."""
     
     product_catalog: SourceChargebeeProductCatalogEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('product_catalog') }})
-
     r"""Product Catalog version of your Chargebee site. Instructions on how to find your version you may find <a href=\\"https://apidocs.chargebee.com/docs/api?prod_cat_ver=2\\">here</a> under `API Version` section."""
     site: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('site') }})
-
     r"""The site prefix for your Chargebee instance."""
     site_api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('site_api_key') }})
-
     r"""Chargebee API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/chargebee\\">docs</a> for more information on how to obtain this key."""
     source_type: SourceChargebeeChargebeeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2021-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_chartmogul.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_chartmogul.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,18 +22,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceChartmogul:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your Chartmogul API key. See <a href=\\"https://help.chartmogul.com/hc/en-us/articles/4407796325906-Creating-and-Managing-API-keys#creating-an-api-key\\"> the docs </a> for info on how to obtain this."""
     interval: SourceChartmogulIntervalEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('interval') }})
-
     r"""Some APIs such as <a href=\\"https://dev.chartmogul.com/reference/endpoint-overview-metrics-api\\">Metrics</a> require intervals to cluster data."""
     source_type: SourceChartmogulChartmogulEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. When feasible, any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_clickhouse.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_clickhouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,89 +17,71 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceClickhouseTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceClickhouseTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceClickhouseTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceClickhouseTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceClickhouseTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: SourceClickhouseTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceClickhouse:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The name of the database."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The host endpoint of the Clickhouse cluster."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The port of the database."""
     source_type: SourceClickhouseClickhouseEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username which is used to access the database."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with this username."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_clickup_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_clickup_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,27 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceClickupAPI:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Every ClickUp API call required authentication. This field is your personal API token. See <a href=\\"https://clickup.com/api/developer-portal/authentication/#personal-token\\">here</a>."""
     source_type: SourceClickupAPIClickupAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     folder_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('folder_id'), 'exclude': lambda f: f is None }})
-
     r"""The ID of your folder in your space. Retrieve it from the `/space/{space_id}/folder` of the ClickUp API. See <a href=\\"https://clickup.com/api/clickupreference/operation/GetFolders/\\">here</a>."""
     include_closed_tasks: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_closed_tasks'), 'exclude': lambda f: f is None }})
-
     r"""Include or exclude closed tasks. By default, they are excluded. See <a https://clickup.com/api/clickupreference/operation/GetTasks/#!in=query&path=include_closed&t=request\\">here</a>."""
     list_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('list_id'), 'exclude': lambda f: f is None }})
-
     r"""The ID of your list in your folder. Retrieve it from the `/folder/{folder_id}/list` of the ClickUp API. See <a href=\\"https://clickup.com/api/clickupreference/operation/GetLists/\\">here</a>."""
     space_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('space_id'), 'exclude': lambda f: f is None }})
-
     r"""The ID of your space in your workspace. Retrieve it from the `/team/{team_id}/space` of the ClickUp API. See <a href=\\"https://clickup.com/api/clickupreference/operation/GetSpaces/\\">here</a>."""
     team_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('team_id'), 'exclude': lambda f: f is None }})
-
     r"""The ID of your team in ClickUp. Retrieve it from the `/team` of the ClickUp API. See <a href=\\"https://clickup.com/api/clickupreference/operation/GetAuthorizedTeams/\\">here</a>."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_close_com.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_close_com.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceCloseCom:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Close.com API key (usually starts with 'api_'; find yours <a href=\\"https://app.close.com/settings/api/\\">here</a>)."""
     source_type: SourceCloseComCloseComEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The start date to sync data. Leave blank for full sync. Format: YYYY-MM-DD."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_coda.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_coda.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceCoda:
     r"""The values required to configure the source."""
     
     auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
-
     r"""Bearer token"""
     source_type: SourceCodaCodaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_coin_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_coin_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,38 +18,30 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceCoinAPI:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key"""
     environment: SourceCoinAPIEnvironmentEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('environment') }})
-
     r"""The environment to use. Either sandbox or production."""
     period: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('period') }})
-
     r"""The period to use. See the documentation for a list. https://docs.coinapi.io/#list-all-periods-get"""
     source_type: SourceCoinAPICoinAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The start date in ISO 8601 format."""
     symbol_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('symbol_id') }})
-
     r"""The symbol ID to use. See the documentation for a list.
     https://docs.coinapi.io/#list-all-symbols-get
     """
     end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
-
     r"""The end date in ISO 8601 format. If not supplied, data will be returned
     from the start date to the current time, or when the count of result
     elements reaches its limit.
     """
     limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
-
     r"""The maximum number of elements to return. If not supplied, the default
     is 100. For numbers larger than 100, each 100 items is counted as one
     request for pricing purposes. Maximum value is 100000.
     """
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_coinmarketcap.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_coinmarketcap.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceCoinmarketcap:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your API Key. See <a href=\\"https://coinmarketcap.com/api/documentation/v1/#section/Authentication\\">here</a>. The token is case sensitive."""
     data_type: SourceCoinmarketcapDataTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_type') }})
-
     r"""/latest: Latest market ticker quotes and averages for cryptocurrencies and exchanges. /historical: Intervals of historic market data like OHLCV data or data for use in charting libraries. See <a href=\\"https://coinmarketcap.com/api/documentation/v1/#section/Endpoint-Overview\\">here</a>."""
     source_type: SourceCoinmarketcapCoinmarketcapEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     symbols: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('symbols'), 'exclude': lambda f: f is None }})
-
     r"""Cryptocurrency symbols. (only used for quotes stream)"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_configcat.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_configcat.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceConfigcat:
     r"""The values required to configure the source."""
     
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Basic auth password. See <a href=\\"https://api.configcat.com/docs/#section/Authentication\\">here</a>."""
     source_type: SourceConfigcatConfigcatEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Basic auth user name. See <a href=\\"https://api.configcat.com/docs/#section/Authentication\\">here</a>."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_confluence.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_confluence.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceConfluence:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Please follow the Jira confluence for generating an API token: <a href=\\"https://support.atlassian.com/atlassian-account/docs/manage-api-tokens-for-your-atlassian-account/\\">generating an API token</a>."""
     domain_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_name') }})
-
     r"""Your Confluence domain name"""
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""Your Confluence login email"""
     source_type: SourceConfluenceConfluenceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_datascope.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_datascope.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceDatascope:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key"""
     source_type: SourceDatascopeDatascopeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""Start date for the data to be replicated"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_delighted.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_delighted.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceDelighted:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""A Delighted API key."""
     since: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('since'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate the data"""
     source_type: SourceDelightedDelightedEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_dixa.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_dixa.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceDixa:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Dixa API token"""
     source_type: SourceDixaDixaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The connector pulls records updated from this date onwards."""
     batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batch_size'), 'exclude': lambda f: f is None }})
-
     r"""Number of days to batch into one request. Max 31."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_dockerhub.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_dockerhub.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceDockerhub:
     r"""The values required to configure the source."""
     
     docker_username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('docker_username') }})
-
     r"""Username of DockerHub person or organization (for https://hub.docker.com/v2/repositories/USERNAME/ API call)"""
     source_type: SourceDockerhubDockerhubEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_dremio.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_shortio.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourceDremioDremioEnum(str, Enum):
-    DREMIO = 'dremio'
+class SourceShortioShortioEnum(str, Enum):
+    SHORTIO = 'shortio'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceDremio:
+class SourceShortio:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""API Key that is generated when you authenticate to Dremio API"""
-    base_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base_url') }})
-
-    r"""URL of your Dremio instance"""
-    source_type: SourceDremioDremioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    domain_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_id') }})
+    secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
+    r"""Short.io Secret Key"""
+    source_type: SourceShortioShortioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_dynamodb.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_dynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,24 +42,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceDynamodb:
     r"""The values required to configure the source."""
     
     access_key_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key_id') }})
-
     r"""The access key id to access Dynamodb. Airbyte requires read permissions to the database"""
     secret_access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_access_key') }})
-
     r"""The corresponding secret to the access key id."""
     source_type: SourceDynamodbDynamodbEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint'), 'exclude': lambda f: f is None }})
-
     r"""the URL of the Dynamodb database"""
     region: Optional[SourceDynamodbDynamodbRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
-
     r"""The region of the Dynamodb database"""
     reserved_attribute_names: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reserved_attribute_names'), 'exclude': lambda f: f is None }})
-
     r"""Comma separated reserved attribute names present in your tables"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_e2e_test_cloud.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_e2e_test_cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,38 +13,32 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceE2eTestCloudMockCatalogMultiSchema:
     r"""A catalog with multiple data streams, each with a different schema."""
     
     stream_schemas: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stream_schemas') }})
-
     r"""A Json object specifying multiple data streams and their schemas. Each key in this object is one stream name. Each value is the schema for that stream. The schema should be compatible with <a href=\\"https://json-schema.org/draft-07/json-schema-release-notes.html\\">draft-07</a>. See <a href=\\"https://cswr.github.io/JsonSchema/spec/introduction/\\">this doc</a> for examples."""
     type: SourceE2eTestCloudMockCatalogMultiSchemaTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-
     
 class SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum(str, Enum):
     SINGLE_STREAM = 'SINGLE_STREAM'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceE2eTestCloudMockCatalogSingleSchema:
     r"""A catalog with one or multiple streams that share the same schema."""
     
     stream_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stream_name') }})
-
     r"""Name of the data stream."""
     stream_schema: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stream_schema') }})
-
     r"""A Json schema for the stream. The schema should be compatible with <a href=\\"https://json-schema.org/draft-07/json-schema-release-notes.html\\">draft-07</a>. See <a href=\\"https://cswr.github.io/JsonSchema/spec/introduction/\\">this doc</a> for examples."""
     type: SourceE2eTestCloudMockCatalogSingleSchemaTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-
     stream_duplication: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stream_duplication'), 'exclude': lambda f: f is None }})
-
     r"""Duplicate the stream for easy load testing. Each stream name will have a number suffix. For example, if the stream name is \\"ds\\", the duplicated streams will be \\"ds_0\\", \\"ds_1\\", etc."""
     
 class SourceE2eTestCloudE2eTestCloudEnum(str, Enum):
     E2E_TEST_CLOUD = 'e2e-test-cloud'
 
 class SourceE2eTestCloudTypeEnum(str, Enum):
     CONTINUOUS_FEED = 'CONTINUOUS_FEED'
@@ -52,22 +46,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceE2eTestCloud:
     r"""The values required to configure the source."""
     
     max_messages: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_messages') }})
-
     r"""Number of records to emit per stream. Min 1. Max 100 billion."""
     mock_catalog: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mock_catalog') }})
-
     source_type: SourceE2eTestCloudE2eTestCloudEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     message_interval_ms: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message_interval_ms'), 'exclude': lambda f: f is None }})
-
     r"""Interval between messages in ms. Min 0 ms. Max 60000 ms (1 minute)."""
     seed: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is None }})
-
     r"""When the seed is unspecified, the current time millis will be used as the seed. Range: [0, 1000000]."""
     type: Optional[SourceE2eTestCloudTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_emailoctopus.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_emailoctopus.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceEmailoctopus:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""EmailOctopus API Key. See the <a href=\\"https://help.emailoctopus.com/article/165-how-to-create-and-delete-api-keys\\">docs</a> for information on how to generate this key."""
     source_type: SourceEmailoctopusEmailoctopusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_exchange_rates.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_exchange_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,21 +15,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceExchangeRates:
     r"""The values required to configure the source."""
     
     access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key') }})
-
     r"""Your API Key. See <a href=\\"https://apilayer.com/marketplace/exchangerates_data-api\\">here</a>. The key is case sensitive."""
     source_type: SourceExchangeRatesExchangeRatesEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""Start getting data from that date."""
     base: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base'), 'exclude': lambda f: f is None }})
-
     r"""ISO reference currency. See <a href=\\"https://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html\\">here</a>. Free plan doesn't support Source Currency Switching, default base currency is EUR"""
     ignore_weekends: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ignore_weekends'), 'exclude': lambda f: f is None }})
-
     r"""Ignore weekends? (Exchanges don't run on weekends)"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_facebook_marketing.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_facebook_marketing.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,79 +206,58 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFacebookMarketingInsightConfig:
     r"""Config for custom insights"""
     
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
     r"""The name value of insight"""
     action_breakdowns: Optional[list[SourceFacebookMarketingInsightConfigValidActionBreakdownsEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action_breakdowns'), 'exclude': lambda f: f is None }})
-
     r"""A list of chosen action_breakdowns for action_breakdowns"""
     breakdowns: Optional[list[SourceFacebookMarketingInsightConfigValidBreakdownsEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('breakdowns'), 'exclude': lambda f: f is None }})
-
     r"""A list of chosen breakdowns for breakdowns"""
     end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date until which you'd like to replicate data for this stream, in the format YYYY-MM-DDT00:00:00Z. All data generated between the start date and this end date will be replicated. Not setting this option will result in always syncing the latest data."""
     fields_: Optional[list[SourceFacebookMarketingInsightConfigValidEnumsEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fields'), 'exclude': lambda f: f is None }})
-
     r"""A list of chosen fields for fields parameter"""
     insights_lookback_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('insights_lookback_window'), 'exclude': lambda f: f is None }})
-
     r"""The attribution window"""
     level: Optional[SourceFacebookMarketingInsightConfigLevelEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('level'), 'exclude': lambda f: f is None }})
-
     r"""Chosen level for API"""
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date from which you'd like to replicate data for this stream, in the format YYYY-MM-DDT00:00:00Z."""
     time_increment: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('time_increment'), 'exclude': lambda f: f is None }})
-
     r"""Time window in days by which to aggregate statistics. The sync will be chunked into N day intervals, where N is the number of days you specified. For example, if you set this value to 7, then all statistics will be reported as 7-day aggregates by starting from the start_date. If the start and end dates are October 1st and October 30th, then the connector will output 5 records: 01 - 06, 07 - 13, 14 - 20, 21 - 27, and 28 - 30 (3 days only)."""
     
 class SourceFacebookMarketingFacebookMarketingEnum(str, Enum):
     FACEBOOK_MARKETING = 'facebook-marketing'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFacebookMarketing:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The value of the generated access token. From your App’s Dashboard, click on \\"Marketing API\\" then \\"Tools\\". Select permissions <b>ads_management, ads_read, read_insights, business_management</b>. Then click on \\"Get token\\". See the <a href=\\"https://docs.airbyte.com/integrations/sources/facebook-marketing\\">docs</a> for more information."""
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
-
     r"""The Facebook Ad account ID to use when pulling data from the Facebook Marketing API. Open your Meta Ads Manager. The Ad account ID number is in the account dropdown menu or in your browser's address bar. See the <a href=\\"https://www.facebook.com/business/help/1492627900875762\\">docs</a> for more information."""
     source_type: SourceFacebookMarketingFacebookMarketingEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
     action_breakdowns_allow_empty: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('action_breakdowns_allow_empty'), 'exclude': lambda f: f is None }})
-
     r"""Allows action_breakdowns to be an empty list"""
     custom_insights: Optional[list[SourceFacebookMarketingInsightConfig]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_insights'), 'exclude': lambda f: f is None }})
-
     r"""A list which contains ad statistics entries, each entry must have a name and can contains fields, breakdowns or action_breakdowns. Click on \\"add\\" to fill this field."""
     end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
-
     r"""The date until which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DDT00:00:00Z. All data generated between the start date and this end date will be replicated. Not setting this option will result in always syncing the latest data."""
     fetch_thumbnail_images: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fetch_thumbnail_images'), 'exclude': lambda f: f is None }})
-
     r"""Set to active if you want to fetch the thumbnail_url and store the result in thumbnail_data_url for each Ad Creative."""
     include_deleted: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_deleted'), 'exclude': lambda f: f is None }})
-
     r"""Set to active if you want to include data from deleted Campaigns, Ads, and AdSets."""
     insights_lookback_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('insights_lookback_window'), 'exclude': lambda f: f is None }})
-
     r"""The attribution window. Facebook freezes insight data 28 days after it was generated, which means that all data from the past 28 days may have changed since we last emitted it, so you can retrieve refreshed insights from the past by setting this parameter. If you set a custom lookback window value in Facebook account, please provide the same value here."""
     max_batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max_batch_size'), 'exclude': lambda f: f is None }})
-
     r"""Maximum batch size used when sending batch requests to Facebook API. Most users do not need to set this field unless they specifically need to tune the connector to address specific issues or use cases."""
     page_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page_size'), 'exclude': lambda f: f is None }})
-
     r"""Page size used when sending requests to Facebook API to specify number of records per page when response has pagination. Most users do not need to set this field unless they specifically need to tune the connector to address specific issues or use cases."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_facebook_pages.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_facebook_pages.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFacebookPages:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Facebook Page Access Token"""
     page_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page_id') }})
-
     r"""Page ID"""
     source_type: SourceFacebookPagesFacebookPagesEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_faker.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_faker.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,24 +13,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFaker:
     r"""The values required to configure the source."""
     
     count: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('count') }})
-
     r"""How many users should be generated in total.  This setting does not apply to the purchases or products stream."""
     source_type: SourceFakerFakerEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     parallelism: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parallelism'), 'exclude': lambda f: f is None }})
-
     r"""How many parallel workers should we use to generate fake data?  Choose a value equal to the number of CPUs you will allocate to this source."""
     records_per_slice: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('records_per_slice'), 'exclude': lambda f: f is None }})
-
     r"""How many fake records will be in each page (stream slice), before a state message is emitted?"""
     records_per_sync: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('records_per_sync'), 'exclude': lambda f: f is None }})
-
     r"""How many fake records will be returned for each sync, for each stream?  By default, it will take 2 syncs to create the requested 1000 records."""
     seed: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is None }})
-
     r"""Manually control the faker random seed to return the same values on subsequent runs (leave -1 for random)"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_fauna.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_fauna.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,16 @@
     r"""<b>This only applies to incremental syncs.</b> <br>
     Enabling deletion mode informs your destination of deleted documents.<br>
     Disabled - Leave this feature disabled, and ignore deleted documents.<br>
     Enabled - Enables this feature. When a document is deleted, the connector exports a record with a \"deleted at\" column containing the time that the document was deleted.
     """
     
     column: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('column') }})
-
     r"""Name of the \\"deleted at\\" column."""
     deletion_mode: SourceFaunaCollectionDeletionsEnabledDeletionModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deletion_mode') }})
-
     
 class SourceFaunaCollectionDeletionsDisabledDeletionModeEnum(str, Enum):
     IGNORE = 'ignore'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
@@ -36,31 +34,28 @@
     r"""<b>This only applies to incremental syncs.</b> <br>
     Enabling deletion mode informs your destination of deleted documents.<br>
     Disabled - Leave this feature disabled, and ignore deleted documents.<br>
     Enabled - Enables this feature. When a document is deleted, the connector exports a record with a \"deleted at\" column containing the time that the document was deleted.
     """
     
     deletion_mode: SourceFaunaCollectionDeletionsDisabledDeletionModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deletion_mode') }})
-
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFaunaCollection:
     r"""Settings for the Fauna Collection."""
     
     deletions: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('deletions') }})
-
     r"""<b>This only applies to incremental syncs.</b> <br>
     Enabling deletion mode informs your destination of deleted documents.<br>
     Disabled - Leave this feature disabled, and ignore deleted documents.<br>
     Enabled - Enables this feature. When a document is deleted, the connector exports a record with a \"deleted at\" column containing the time that the document was deleted.
     """
     page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page_size') }})
-
     r"""The page size used when reading documents from the database. The larger the page size, the faster the connector processes documents. However, if a page is too large, the connector may fail. <br>
     Choose your page size based on how large the documents are. <br>
     See <a href=\"https://docs.fauna.com/fauna/current/learn/understanding/types#page\">the docs</a>.
     """
     
 class SourceFaunaFaunaEnum(str, Enum):
     FAUNA = 'fauna'
@@ -68,24 +63,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFauna:
     r"""The values required to configure the source."""
     
     domain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain') }})
-
     r"""Domain of Fauna to query. Defaults db.fauna.com. See <a href=https://docs.fauna.com/fauna/current/learn/understanding/region_groups#how-to-use-region-groups>the docs</a>."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Endpoint port."""
     scheme: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheme') }})
-
     r"""URL scheme."""
     secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret') }})
-
     r"""Fauna secret, used when authenticating with the database."""
     source_type: SourceFaunaFaunaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     collection: Optional[SourceFaunaCollection] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('collection'), 'exclude': lambda f: f is None }})
-
     r"""Settings for the Fauna Collection."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_file_secure.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_file_secure.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,153 +24,121 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderSFTPSecureFileTransferProtocol:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     storage: SourceFileSecureProviderSFTPSecureFileTransferProtocolStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})
-
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     port: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     
 class SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum(str, Enum):
     SCP = 'SCP'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderSCPSecureCopyProtocol:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     storage: SourceFileSecureProviderSCPSecureCopyProtocolStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})
-
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     port: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     
 class SourceFileSecureProviderSSHSecureShellStorageEnum(str, Enum):
     SSH = 'SSH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderSSHSecureShell:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     storage: SourceFileSecureProviderSSHSecureShellStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})
-
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     port: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port'), 'exclude': lambda f: f is None }})
-
     
 class SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum(str, Enum):
     AZ_BLOB = 'AzBlob'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderAzBlobAzureBlobStorage:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     storage: SourceFileSecureProviderAzBlobAzureBlobStorageStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     storage_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage_account') }})
-
     r"""The globally unique name of the storage account that the desired blob sits within. See <a href=\\"https://docs.microsoft.com/en-us/azure/storage/common/storage-account-overview\\" target=\\"_blank\\">here</a> for more details."""
     sas_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sas_token'), 'exclude': lambda f: f is None }})
-
     r"""To access Azure Blob Storage, this connector would need credentials with the proper permissions. One option is a SAS (Shared Access Signature) token. If accessing publicly available data, this field is not necessary."""
     shared_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shared_key'), 'exclude': lambda f: f is None }})
-
     r"""To access Azure Blob Storage, this connector would need credentials with the proper permissions. One option is a storage account shared key (aka account key or access key). If accessing publicly available data, this field is not necessary."""
     
 class SourceFileSecureProviderS3AmazonWebServicesStorageEnum(str, Enum):
     S3 = 'S3'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderS3AmazonWebServices:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     storage: SourceFileSecureProviderS3AmazonWebServicesStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     aws_access_key_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_access_key_id'), 'exclude': lambda f: f is None }})
-
     r"""In order to access private Buckets stored on AWS S3, this connector would need credentials with the proper permissions. If accessing publicly available data, this field is not necessary."""
     aws_secret_access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_secret_access_key'), 'exclude': lambda f: f is None }})
-
     r"""In order to access private Buckets stored on AWS S3, this connector would need credentials with the proper permissions. If accessing publicly available data, this field is not necessary."""
     
 class SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum(str, Enum):
     GCS = 'GCS'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderGCSGoogleCloudStorage:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     storage: SourceFileSecureProviderGCSGoogleCloudStorageStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     service_account_json: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_account_json'), 'exclude': lambda f: f is None }})
-
     r"""In order to access private Buckets stored on Google Cloud, this connector would need a service account json credentials with the proper permissions as described <a href=\\"https://cloud.google.com/iam/docs/service-accounts\\" target=\\"_blank\\">here</a>. Please generate the credentials.json file and copy/paste its content to this field (expecting JSON formats). If accessing publicly available data, this field is not necessary."""
     
 class SourceFileSecureProviderHTTPSPublicWebStorageEnum(str, Enum):
     HTTPS = 'HTTPS'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecureProviderHTTPSPublicWeb:
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     
     storage: SourceFileSecureProviderHTTPSPublicWebStorageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('storage') }})
-
     user_agent: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user_agent'), 'exclude': lambda f: f is None }})
-
     r"""Add User-Agent to request"""
     
 class SourceFileSecureFileSecureEnum(str, Enum):
     FILE_SECURE = 'file-secure'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFileSecure:
     r"""The values required to configure the source."""
     
     dataset_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_name') }})
-
     r"""The Name of the final table to replicate this file into (should include letters, numbers dash and underscores only)."""
     format: SourceFileSecureFileFormatEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format') }})
-
     r"""The Format of the file which should be replicated (Warning: some formats may be experimental, please refer to the docs)."""
     provider: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider') }})
-
     r"""The storage Provider or Location of the file(s) which should be replicated."""
     source_type: SourceFileSecureFileSecureEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-
     r"""The URL path to access the file which should be replicated."""
     reader_options: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reader_options'), 'exclude': lambda f: f is None }})
-
     r"""This should be a string in JSON format. It depends on the chosen file format to provide additional options and tune its behavior."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_firebolt.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_firebolt.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,27 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFirebolt:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The database to connect to."""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Firebolt password."""
     source_type: SourceFireboltFireboltEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Firebolt email address you use to login."""
     account: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account'), 'exclude': lambda f: f is None }})
-
     r"""Firebolt account to login."""
     engine: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('engine'), 'exclude': lambda f: f is None }})
-
     r"""Engine name or url to connect to."""
     host: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host'), 'exclude': lambda f: f is None }})
-
     r"""The host name of your Firebolt database."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_freshcaller.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_freshcaller.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFreshcaller:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Freshcaller API Key. See the <a href=\\"https://docs.airbyte.io/integrations/sources/freshcaller\\">docs</a> for more information on how to obtain this key."""
     domain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain') }})
-
     r"""Used to construct Base URL for the Freshcaller APIs"""
     source_type: SourceFreshcallerFreshcallerEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""UTC date and time. Any data created after this date will be replicated."""
     requests_per_minute: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requests_per_minute'), 'exclude': lambda f: f is None }})
-
     r"""The number of requests per minute that this source allowed to use. There is a rate limit of 50 requests per minute per app per account."""
     sync_lag_minutes: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sync_lag_minutes'), 'exclude': lambda f: f is None }})
-
     r"""Lag in minutes for each sync, i.e., at time T, data for the time range [prev_sync_time, T-30] will be fetched"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_freshdesk.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_freshdesk.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,21 +16,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFreshdesk:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Freshdesk API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/freshdesk\\">docs</a> for more information on how to obtain this key."""
     domain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain') }})
-
     r"""Freshdesk domain"""
     source_type: SourceFreshdeskFreshdeskEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     requests_per_minute: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('requests_per_minute'), 'exclude': lambda f: f is None }})
-
     r"""The number of requests per minute that this source allowed to use. There is a rate limit of 50 requests per minute per app per account."""
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time. Any data created after this date will be replicated. If this parameter is not set, all data will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_freshsales.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_freshsales.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceFreshsales:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Freshsales API Key. See <a href=\\"https://crmsupport.freshworks.com/support/solutions/articles/50000002503-how-to-find-my-api-key-\\">here</a>. The key is case sensitive."""
     domain_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_name') }})
-
     r"""The Name of your Freshsales domain"""
     source_type: SourceFreshsalesFreshsalesEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_gcs.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_gcs.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGcs:
     r"""The values required to configure the source."""
     
     gcs_bucket: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_bucket') }})
-
     r"""GCS bucket name"""
     gcs_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('gcs_path') }})
-
     r"""GCS path to data"""
     service_account: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_account') }})
-
     r"""Enter your Google Cloud <a href=\\"https://cloud.google.com/iam/docs/creating-managing-service-account-keys#creating_service_account_keys\\">service account key</a> in JSON format"""
     source_type: SourceGcsGcsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_getlago.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_getlago.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGetlago:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your API Key. See <a href=\\"https://doc.getlago.com/docs/api/intro\\">here</a>."""
     source_type: SourceGetlagoGetlagoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_github.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,54 +16,44 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGithubCredentialsPersonalAccessToken:
     r"""Choose how to authenticate to GitHub"""
     
     personal_access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('personal_access_token') }})
-
     r"""Log into GitHub and then generate a <a href=\\"https://github.com/settings/tokens\\">personal access token</a>. To load balance your API quota consumption across multiple API tokens, input multiple tokens separated with \\",\\" """
     option_title: Optional[SourceGithubCredentialsPersonalAccessTokenOptionTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title'), 'exclude': lambda f: f is None }})
-
     
 class SourceGithubCredentialsOAuthOptionTitleEnum(str, Enum):
     O_AUTH_CREDENTIALS = 'OAuth Credentials'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGithubCredentialsOAuth:
     r"""Choose how to authenticate to GitHub"""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""OAuth access token"""
     option_title: Optional[SourceGithubCredentialsOAuthOptionTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title'), 'exclude': lambda f: f is None }})
-
     
 class SourceGithubGithubEnum(str, Enum):
     GITHUB = 'github'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGithub:
     r"""The values required to configure the source."""
     
     repository: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('repository') }})
-
     r"""Space-delimited list of GitHub organizations/repositories, e.g. `airbytehq/airbyte` for single repository, `airbytehq/*` for get all repositories from organization and `airbytehq/airbyte airbytehq/another-repo` for multiple repositories."""
     source_type: SourceGithubGithubEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data from GitHub in the format YYYY-MM-DDT00:00:00Z. For the streams which support this configuration, only data generated on or after the start date will be replicated. This field doesn't apply to all streams, see the <a href=\\"https://docs.airbyte.com/integrations/sources/github\\">docs</a> for more info"""
     branch: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('branch'), 'exclude': lambda f: f is None }})
-
     r"""Space-delimited list of GitHub repository branches to pull commits for, e.g. `airbytehq/airbyte/master`. If no branches are specified for a repository, the default branch will be pulled."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to GitHub"""
     page_size_for_large_streams: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('page_size_for_large_streams'), 'exclude': lambda f: f is None }})
-
     r"""The Github connector contains several streams with a large amount of data. The page size of such streams depends on the size of your repository. We recommended that you specify values between 10 and 30."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_gitlab.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_gitlab.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,64 +15,50 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGitlabCredentialsPrivateToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Log into your Gitlab account and then generate a personal Access Token."""
     auth_type: Optional[SourceGitlabCredentialsPrivateTokenAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceGitlabCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGitlabCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token for making authenticated requests."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The API ID of the Gitlab developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The API Secret the Gitlab developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The key to refresh the expired access_token."""
     token_expiry_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date-time when the access token should be refreshed."""
     auth_type: Optional[SourceGitlabCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceGitlabGitlabEnum(str, Enum):
     GITLAB = 'gitlab'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGitlab:
     r"""The values required to configure the source."""
     
     api_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_url') }})
-
     r"""Please enter your basic URL from GitLab instance."""
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     source_type: SourceGitlabGitlabEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for GitLab API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
     groups: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('groups'), 'exclude': lambda f: f is None }})
-
     r"""Space-delimited list of groups. e.g. airbyte.io."""
     projects: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('projects'), 'exclude': lambda f: f is None }})
-
     r"""Space-delimited list of projects. e.g. airbyte.io/documentation meltano/tap-gitlab."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_glassfrog.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_glassfrog.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGlassfrog:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API key provided by Glassfrog"""
     source_type: SourceGlassfrogGlassfrogEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_gnews.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_gnews.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,18 +100,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGnews:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key"""
     query: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
-
     r"""This parameter allows you to specify your search keywords to find the news articles you are looking for. The keywords will be used to return the most relevant articles. It is possible to use logical operators  with keywords. - Phrase Search Operator: This operator allows you to make an exact search. Keywords surrounded by
       quotation marks are used to search for articles with the exact same keyword sequence. 
       For example the query: \"Apple iPhone\" will return articles matching at least once this sequence of keywords.
     - Logical AND Operator: This operator allows you to make sure that several keywords are all used in the article
       search. By default the space character acts as an AND operator, it is possible to replace the space character 
       by AND to obtain the same result. For example the query: Apple Microsoft is equivalent to Apple AND Microsoft
     - Logical OR Operator: This operator allows you to retrieve articles matching the keyword a or the keyword b.
@@ -120,40 +118,31 @@
       the keyword Microsoft
     - Logical NOT Operator: This operator allows you to remove from the results the articles corresponding to the
       specified keywords. To use it, you need to add NOT in front of each word or phrase surrounded by quotes.
       For example the query: Apple NOT iPhone will return all articles matching the keyword Apple but not the keyword
       iPhone
     """
     source_type: SourceGnewsGnewsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     country: Optional[SourceGnewsCountryEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to specify the country where the news articles returned by the API were published, the contents of the articles are not necessarily related to the specified country. You have to set as value the 2 letters code of the country you want to filter."""
     end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to filter the articles that have a publication date smaller than or equal to the  specified value. The date must respect the following format: YYYY-MM-DD hh:mm:ss (in UTC)"""
     in_: Optional[list[SourceGnewsInEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('in'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to choose in which attributes the keywords are searched. The attributes that can be set are title, description and content. It is possible to combine several attributes."""
     language: Optional[SourceGnewsLanguageEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('language'), 'exclude': lambda f: f is None }})
-
     nullable: Optional[list[SourceGnewsNullableEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('nullable'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to specify the attributes that you allow to return null values. The attributes that  can be set are title, description and content. It is possible to combine several attributes"""
     sortby: Optional[SourceGnewsSortByEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sortby'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to choose with which type of sorting the articles should be returned. Two values  are possible:
       - publishedAt = sort by publication date, the articles with the most recent publication date are returned first
       - relevance = sort by best match to keywords, the articles with the best match are returned first
     """
     start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to filter the articles that have a publication date greater than or equal to the  specified value. The date must respect the following format: YYYY-MM-DD hh:mm:ss (in UTC)"""
     top_headlines_query: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('top_headlines_query'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to specify your search keywords to find the news articles you are looking for. The keywords will be used to return the most relevant articles. It is possible to use logical operators  with keywords. - Phrase Search Operator: This operator allows you to make an exact search. Keywords surrounded by
       quotation marks are used to search for articles with the exact same keyword sequence. 
       For example the query: \"Apple iPhone\" will return articles matching at least once this sequence of keywords.
     - Logical AND Operator: This operator allows you to make sure that several keywords are all used in the article
       search. By default the space character acts as an AND operator, it is possible to replace the space character 
       by AND to obtain the same result. For example the query: Apple Microsoft is equivalent to Apple AND Microsoft
     - Logical OR Operator: This operator allows you to retrieve articles matching the keyword a or the keyword b.
@@ -162,10 +151,9 @@
       the keyword Microsoft
     - Logical NOT Operator: This operator allows you to remove from the results the articles corresponding to the
       specified keywords. To use it, you need to add NOT in front of each word or phrase surrounded by quotes.
       For example the query: Apple NOT iPhone will return all articles matching the keyword Apple but not the keyword
       iPhone
     """
     top_headlines_topic: Optional[SourceGnewsTopHeadlinesTopicEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('top_headlines_topic'), 'exclude': lambda f: f is None }})
-
     r"""This parameter allows you to change the category for the request."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_ads.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_ads.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,65 +11,50 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAdsGoogleCredentials:
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Google Ads developer application. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/google-ads#setup-guide\\">docs</a>"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Google Ads developer application. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/google-ads#setup-guide\\">docs</a>"""
     developer_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('developer_token') }})
-
     r"""Developer token granted by Google to use their APIs. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/google-ads#setup-guide\\">docs</a>"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining a new access token. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/google-ads#setup-guide\\">docs</a>"""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access Token for making authenticated requests. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/google-ads#setup-guide\\">docs</a>"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAdsCustomQueries:
     
     query: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
-
     r"""A custom defined GAQL query for building the report. Should not contain segments.date expression because it is used by incremental streams. See Google's <a href=\\"https://developers.google.com/google-ads/api/fields/v11/overview_query_builder\\">query builder</a> for more information."""
     table_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('table_name') }})
-
     r"""The table name in your destination database for choosen query."""
     
 class SourceGoogleAdsGoogleAdsEnum(str, Enum):
     GOOGLE_ADS = 'google-ads'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAds:
     r"""The values required to configure the source."""
     
     credentials: SourceGoogleAdsGoogleCredentials = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customer_id') }})
-
     r"""Comma separated list of (client) customer IDs. Each customer ID must be specified as a 10-digit number without dashes. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/google-ads#setup-guide\\">docs</a>. Metrics streams like AdGroupAdReport cannot be requested for a manager account."""
     source_type: SourceGoogleAdsGoogleAdsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25. Any data before this date will not be replicated."""
     conversion_window_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('conversion_window_days'), 'exclude': lambda f: f is None }})
-
     r"""A conversion window is the period of time after an ad interaction (such as an ad click or video view) during which a conversion, such as a purchase, is recorded in Google Ads. For more information, see Google's <a href=\\"https://support.google.com/google-ads/answer/3123169?hl=en\\">documentation</a>."""
     custom_queries: Optional[list[SourceGoogleAdsCustomQueries]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_queries'), 'exclude': lambda f: f is None }})
-
     end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time in the format 2017-01-25. Any data after this date will not be replicated."""
     login_customer_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('login_customer_id'), 'exclude': lambda f: f is None }})
-
     r"""If your access to the customer account is through a manager account, this field is required and must be set to the customer ID of the manager account (10-digit number without dashes). More information about this field you can see <a href=\\"https://developers.google.com/google-ads/api/docs/concepts/call-structure#cid\\">here</a>"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_analytics_data_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_analytics_data_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,63 +15,50 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthentication:
     r"""Credentials for the service"""
     
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""The JSON key of the service account to use for authorization"""
     auth_type: Optional[SourceGoogleAnalyticsDataAPICredentialsServiceAccountKeyAuthenticationAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum(str, Enum):
     CLIENT = 'Client'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauth:
     r"""Credentials for the service"""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Google Analytics developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Google Analytics developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining a new access token."""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access Token for making authenticated requests."""
     auth_type: Optional[SourceGoogleAnalyticsDataAPICredentialsAuthenticateViaGoogleOauthAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum(str, Enum):
     GOOGLE_ANALYTICS_DATA_API = 'google-analytics-data-api'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsDataAPI:
     r"""The values required to configure the source."""
     
     date_ranges_start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date_ranges_start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The start date from which to replicate report data in the format YYYY-MM-DD. Data generated before this date will not be included in the report."""
     property_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('property_id') }})
-
     r"""A Google Analytics GA4 property identifier whose events are tracked. Specified in the URL path and not the body"""
     source_type: SourceGoogleAnalyticsDataAPIGoogleAnalyticsDataAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Credentials for the service"""
     custom_reports: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_reports'), 'exclude': lambda f: f is None }})
-
     r"""A JSON array describing the custom reports you want to sync from Google Analytics. See <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4/#custom-reports\\">the docs</a> for more information about the exact format you can use to fill out this field."""
     window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-
     r"""The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4/#sampling-in-reports\\">the docs</a>. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_analytics_v4.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_analytics_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,63 +13,50 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthentication:
     r"""Credentials for the service"""
     
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""The JSON key of the service account to use for authorization"""
     auth_type: Optional[SourceGoogleAnalyticsV4CredentialsServiceAccountKeyAuthenticationAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum(str, Enum):
     CLIENT = 'Client'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauth:
     r"""Credentials for the service"""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Google Analytics developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Google Analytics developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining a new access token."""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access Token for making authenticated requests."""
     auth_type: Optional[SourceGoogleAnalyticsV4CredentialsAuthenticateViaGoogleOauthAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum(str, Enum):
     GOOGLE_ANALYTICS_V4 = 'google-analytics-v4'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleAnalyticsV4:
     r"""The values required to configure the source."""
     
     source_type: SourceGoogleAnalyticsV4GoogleAnalyticsV4Enum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The date in the format YYYY-MM-DD. Any data before this date will not be replicated."""
     view_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('view_id') }})
-
     r"""The ID for the Google Analytics View you want to fetch data from. This can be found from the <a href=\\"https://ga-dev-tools.appspot.com/account-explorer/\\">Google Analytics Account Explorer</a>."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Credentials for the service"""
     custom_reports: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_reports'), 'exclude': lambda f: f is None }})
-
     r"""A JSON array describing the custom reports you want to sync from Google Analytics. See <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4#data-processing-latency\\">the docs</a> for more information about the exact format you can use to fill out this field."""
     window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-
     r"""The time increment used by the connector when requesting data from the Google Analytics API. More information is available in the <a href=\\"https://docs.airbyte.com/integrations/sources/google-analytics-v4/#sampling-in-reports\\">the docs</a>. The bigger this value is, the faster the sync will be, but the more likely that sampling will be applied to your data, potentially causing inaccuracies in the returned results. We recommend setting this to 1 unless you have a hard requirement to make the sync faster at the expense of accuracy. The minimum allowed value for this field is 1, and the maximum is 364."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_directory.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleDirectory:
     r"""The values required to configure the source."""
     
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""The contents of the JSON service account key. See the <a href=\\"https://developers.google.com/admin-sdk/directory/v1/guides/delegation\\">docs</a> for more information on how to generate this key."""
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""The email of the user, which has permissions to access the Google Workspace Admin APIs."""
     source_type: SourceGoogleDirectoryGoogleDirectoryEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_search_console.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_search_console.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,64 +14,50 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthentication:
     
     auth_type: SourceGoogleSearchConsoleAuthorizationServiceAccountKeyAuthenticationAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""The email of the user which has permissions to access the Google Workspace Admin APIs."""
     service_account_info: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_account_info') }})
-
     r"""The JSON key of the service account to use for authorization. Read more <a href=\\"https://cloud.google.com/iam/docs/creating-managing-service-account-keys\\">here</a>."""
     
 class SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum(str, Enum):
     CLIENT = 'Client'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleSearchConsoleAuthorizationOAuth:
     
     auth_type: SourceGoogleSearchConsoleAuthorizationOAuthAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The client ID of your Google Search Console developer application. Read more <a href=\\"https://developers.google.com/webmaster-tools/v1/how-tos/authorizing\\">here</a>."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The client secret of your Google Search Console developer application. Read more <a href=\\"https://developers.google.com/webmaster-tools/v1/how-tos/authorizing\\">here</a>."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining a new access token. Read more <a href=\\"https://developers.google.com/webmaster-tools/v1/how-tos/authorizing\\">here</a>."""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access token for making authenticated requests. Read more <a href=\\"https://developers.google.com/webmaster-tools/v1/how-tos/authorizing\\">here</a>."""
     
 class SourceGoogleSearchConsoleGoogleSearchConsoleEnum(str, Enum):
     GOOGLE_SEARCH_CONSOLE = 'google-search-console'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleSearchConsole:
     r"""The values required to configure the source."""
     
     authorization: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorization') }})
-
     site_urls: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('site_urls') }})
-
     r"""The URLs of the website property attached to your GSC account. Read more <a href=\\"https://support.google.com/webmasters/answer/34592?hl=en\\">here</a>."""
     source_type: SourceGoogleSearchConsoleGoogleSearchConsoleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date in the format 2017-01-25. Any data before this date will not be replicated."""
     custom_reports: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('custom_reports'), 'exclude': lambda f: f is None }})
-
     r"""A JSON array describing the custom reports you want to sync from Google Search Console. See <a href=\\"https://docs.airbyte.com/integrations/sources/google-search-console#step-2-set-up-the-google-search-console-connector-in-airbyte\\">the docs</a> for more information about the exact format you can use to fill out this field."""
     end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date in the format 2017-01-25. Any data after this date will not be replicated. Must be greater or equal to the start date field."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_sheets.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_sheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,54 +13,44 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleSheetsCredentialsServiceAccountKeyAuthentication:
     r"""Credentials for connecting to the Google Sheets API"""
     
     auth_type: SourceGoogleSheetsCredentialsServiceAccountKeyAuthenticationAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     service_account_info: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_account_info') }})
-
     r"""Enter your Google Cloud <a href=\\"https://cloud.google.com/iam/docs/creating-managing-service-account-keys#creating_service_account_keys\\">service account key</a> in JSON format"""
     
 class SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum(str, Enum):
     CLIENT = 'Client'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuth:
     r"""Credentials for connecting to the Google Sheets API"""
     
     auth_type: SourceGoogleSheetsCredentialsAuthenticateViaGoogleOAuthAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""Enter your Google application's Client ID"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""Enter your Google application's Client Secret"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Enter your Google application's refresh token"""
     
 class SourceGoogleSheetsGoogleSheetsEnum(str, Enum):
     GOOGLE_SHEETS = 'google-sheets'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleSheets:
     r"""The values required to configure the source."""
     
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     r"""Credentials for connecting to the Google Sheets API"""
     source_type: SourceGoogleSheetsGoogleSheetsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     spreadsheet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spreadsheet_id') }})
-
     r"""Enter the link to the Google spreadsheet you want to sync"""
     row_batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('row_batch_size'), 'exclude': lambda f: f is None }})
-
     r"""Number of rows fetched when making a Google Sheet API call. Defaults to 200."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_webfonts.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_webfonts.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleWebfonts:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API key is required to access google apis, For getting your's goto google console and generate api key for Webfonts"""
     source_type: SourceGoogleWebfontsGoogleWebfontsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     alt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alt'), 'exclude': lambda f: f is None }})
-
     r"""Optional, Available params- json, media, proto"""
     pretty_print: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prettyPrint'), 'exclude': lambda f: f is None }})
-
     r"""Optional, boolean type"""
     sort: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sort'), 'exclude': lambda f: f is None }})
-
     r"""Optional, to find how to sort"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_google_workspace_admin_reports.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_google_workspace_admin_reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGoogleWorkspaceAdminReports:
     r"""The values required to configure the source."""
     
     credentials_json: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_json') }})
-
     r"""The contents of the JSON service account key. See the <a href=\\"https://developers.google.com/admin-sdk/reports/v1/guides/delegation\\">docs</a> for more information on how to generate this key."""
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""The email of the user, which has permissions to access the Google Workspace Admin APIs."""
     source_type: SourceGoogleWorkspaceAdminReportsGoogleWorkspaceAdminReportsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     lookback: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback'), 'exclude': lambda f: f is None }})
-
     r"""Sets the range of time shown in the report. Reports API allows from up to 180 days ago."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_greenhouse.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_greenhouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceGreenhouse:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Greenhouse API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/greenhouse\\">docs</a> for more information on how to generate this key."""
     source_type: SourceGreenhouseGreenhouseEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_gridly.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_linnworks.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 
-class SourceGridlyGridlyEnum(str, Enum):
-    GRIDLY = 'gridly'
+class SourceLinnworksLinnworksEnum(str, Enum):
+    LINNWORKS = 'linnworks'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceGridly:
+class SourceLinnworks:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    grid_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('grid_id') }})
-
-    r"""ID of a grid, or can be ID of a branch"""
-    source_type: SourceGridlyGridlyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    application_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('application_id') }})
+    r"""Linnworks Application ID"""
+    application_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('application_secret') }})
+    r"""Linnworks Application Secret"""
+    source_type: SourceLinnworksLinnworksEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
+    token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_harvest.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_harvest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceHarvest:
     r"""The values required to configure the source."""
     
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
-
     r"""Harvest account ID. Required for all Harvest requests in pair with Personal Access Token"""
     replication_start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     source_type: SourceHarvestHarvestEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to Harvest."""
     replication_end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data after this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_hubplanner.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_hubplanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceHubplanner:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Hubplanner API key. See https://github.com/hubplanner/API#authentication for more details."""
     source_type: SourceHubplannerHubplannerEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_hubspot.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_hubspot.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,54 +17,45 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceHubspotCredentialsPrivateApp:
     r"""Choose how to authenticate to HubSpot."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""HubSpot Access token. See the <a href=\\"https://developers.hubspot.com/docs/api/private-apps\\">Hubspot docs</a> if you need help finding this token."""
     credentials_title: SourceHubspotCredentialsPrivateAppCredentialsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title') }})
-
     r"""Name of the credentials set"""
     
 class SourceHubspotCredentialsOAuthCredentialsEnum(str, Enum):
     r"""Name of the credentials"""
     O_AUTH_CREDENTIALS = 'OAuth Credentials'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceHubspotCredentialsOAuth:
     r"""Choose how to authenticate to HubSpot."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your HubSpot developer application. See the <a href=\\"https://legacydocs.hubspot.com/docs/methods/oauth2/oauth2-quickstart\\">Hubspot docs</a> if you need help finding this ID."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The client secret for your HubSpot developer application. See the <a href=\\"https://legacydocs.hubspot.com/docs/methods/oauth2/oauth2-quickstart\\">Hubspot docs</a> if you need help finding this secret."""
     credentials_title: SourceHubspotCredentialsOAuthCredentialsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title') }})
-
     r"""Name of the credentials"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Refresh token to renew an expired access token. See the <a href=\\"https://legacydocs.hubspot.com/docs/methods/oauth2/oauth2-quickstart\\">Hubspot docs</a> if you need help finding this token."""
     
 class SourceHubspotHubspotEnum(str, Enum):
     HUBSPOT = 'hubspot'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceHubspot:
     r"""The values required to configure the source."""
     
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     r"""Choose how to authenticate to HubSpot."""
     source_type: SourceHubspotHubspotEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_insightly.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_insightly.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceInsightly:
     r"""The values required to configure the source."""
     
     source_type: SourceInsightlyInsightlyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The date from which you'd like to replicate data for Insightly in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated. Note that it will be used only for incremental streams."""
     token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
     r"""Your Insightly API token."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_instagram.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_instagram.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceInstagram:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The value of the access token generated with <b>instagram_basic, instagram_manage_insights, pages_show_list, pages_read_engagement, Instagram Public Content Access</b> permissions. See the <a href=\\"https://docs.airbyte.com/integrations/sources/instagram/#step-1-set-up-instagram\\">docs</a> for more information"""
     source_type: SourceInstagramInstagramEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for User Insights, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_instatus.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_instatus.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceInstatus:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Instatus REST API key"""
     source_type: SourceInstatusInstatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_intercom.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_intercom.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceIntercom:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access token for making authenticated requests. See the <a href=\\"https://developers.intercom.com/building-apps/docs/authentication-types#how-to-get-your-access-token\\">Intercom docs</a> for more information."""
     source_type: SourceIntercomIntercomEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_ip2whois.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_ip2whois.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceIp2whois:
     r"""The values required to configure the source."""
     
     source_type: SourceIp2whoisIp2whoisEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     api_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key'), 'exclude': lambda f: f is None }})
-
     r"""Your API Key. See <a href=\\"https://www.ip2whois.com/developers-api\\">here</a>."""
     domain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain'), 'exclude': lambda f: f is None }})
-
     r"""Domain name. See <a href=\\"https://www.ip2whois.com/developers-api\\">here</a>."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_iterable.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_iterable.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceIterable:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Iterable API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/iterable\\">docs</a> for more information on how to obtain this key."""
     source_type: SourceIterableIterableEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for Iterable, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_jira.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_jira.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,33 +16,24 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceJira:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Jira API Token. See the <a href=\\"https://docs.airbyte.com/integrations/sources/jira\\">docs</a> for more information on how to generate this key."""
     domain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain') }})
-
     r"""The Domain for your Jira account, e.g. airbyteio.atlassian.net, airbyteio.jira.com, jira.your-domain.com"""
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""The user email for your Jira account."""
     source_type: SourceJiraJiraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     enable_experimental_streams: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('enable_experimental_streams'), 'exclude': lambda f: f is None }})
-
     r"""Allow the use of experimental streams which rely on undocumented Jira API endpoints. See https://docs.airbyte.com/integrations/sources/jira#experimental-tables for more info."""
     expand_issue_changelog: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expand_issue_changelog'), 'exclude': lambda f: f is None }})
-
     r"""Expand the changelog when replicating issues."""
     projects: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('projects'), 'exclude': lambda f: f is None }})
-
     r"""List of Jira project keys to replicate data for."""
     render_fields: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('render_fields'), 'exclude': lambda f: f is None }})
-
     r"""Render issue fields in HTML format in addition to Jira JSON-like format."""
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date from which you want to replicate data from Jira, use the format YYYY-MM-DDT00:00:00Z. Note that this field only applies to certain streams, and only data generated on or after the start date will be replicated. For more information, refer to the <a href=\\"https://docs.airbyte.com/integrations/sources/jira/\\">documentation</a>."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_k6_cloud.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_k6_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceK6Cloud:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Your API Token. See <a href=\\"https://k6.io/docs/cloud/integrations/token/\\">here</a>. The key is case sensitive."""
     source_type: SourceK6CloudK6CloudEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_klarna.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_klarna.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceKlarna:
     r"""The values required to configure the source."""
     
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""A string which is associated with your Merchant ID and is used to authorize use of Klarna's APIs (https://developers.klarna.com/api/#authentication)"""
     playground: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playground') }})
-
     r"""Propertie defining if connector is used against playground or production environment"""
     region: SourceKlarnaRegionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region') }})
-
     r"""Base url region (For playground eu https://docs.klarna.com/klarna-payments/api/payments-api/#tag/API-URLs). Supported 'eu', 'us', 'oc'"""
     source_type: SourceKlarnaKlarnaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Consists of your Merchant ID (eid) - a unique number that identifies your e-store, combined with a random string (https://developers.klarna.com/api/#authentication)"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_klaviyo.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_klaviyo.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceKlaviyo:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Klaviyo API Key. See our <a href=\\"https://docs.airbyte.com/integrations/sources/klaviyo\\">docs</a> if you need help finding this key."""
     source_type: SourceKlaviyoKlaviyoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_kustomer_singer.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_kustomer_singer.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceKustomerSinger:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Kustomer API Token. See the <a href=\\"https://developer.kustomer.com/kustomer-api-docs/reference/authentication\\">docs</a> on how to obtain this"""
     source_type: SourceKustomerSingerKustomerSingerEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The date from which you'd like to replicate the data"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_launchdarkly.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_launchdarkly.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLaunchdarkly:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Your Access token. See <a href=\\"https://apidocs.launchdarkly.com/#section/Overview/Authentication\\">here</a>."""
     source_type: SourceLaunchdarklyLaunchdarklyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_lemlist.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_lemlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLemlist:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Lemlist API key."""
     source_type: SourceLemlistLemlistEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_linkedin_ads.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_linkedin_ads.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,52 +14,42 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLinkedinAdsCredentialsAccessToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The token value generated using the authentication code. See the <a href=\\"https://docs.airbyte.com/integrations/sources/linkedin-ads#authentication\\">docs</a> to obtain yours."""
     auth_method: Optional[SourceLinkedinAdsCredentialsAccessTokenAuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     
 class SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum(str, Enum):
     O_AUTH2_0 = 'oAuth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLinkedinAdsCredentialsOAuth20:
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The client ID of the LinkedIn Ads developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The client secret the LinkedIn Ads developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The key to refresh the expired access token."""
     auth_method: Optional[SourceLinkedinAdsCredentialsOAuth20AuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     
 class SourceLinkedinAdsLinkedinAdsEnum(str, Enum):
     LINKEDIN_ADS = 'linkedin-ads'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLinkedinAds:
     r"""The values required to configure the source."""
     
     source_type: SourceLinkedinAdsLinkedinAdsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date in the format 2020-09-17. Any data before this date will not be replicated."""
     account_ids: Optional[list[int]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_ids'), 'exclude': lambda f: f is None }})
-
     r"""Specify the account IDs separated by a space, to pull the data from. Leave empty, if you want to pull the data from all associated accounts. See the <a href=\\"https://www.linkedin.com/help/linkedin/answer/a424270/find-linkedin-ads-account-details?lang=en\\">LinkedIn Ads docs</a> for more info."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_linkedin_pages.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_linkedin_pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,49 +12,40 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLinkedinPagesCredentialsAccessToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The token value generated using the LinkedIn Developers OAuth Token Tools. See the <a href=\\"https://docs.airbyte.com/integrations/sources/linkedin-pages/\\">docs</a> to obtain yours."""
     auth_method: Optional[SourceLinkedinPagesCredentialsAccessTokenAuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     
 class SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum(str, Enum):
     O_AUTH2_0 = 'oAuth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLinkedinPagesCredentialsOAuth20:
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The client ID of the LinkedIn developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The client secret of the LinkedIn developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token value generated using the LinkedIn Developers OAuth Token Tools. See the <a href=\\"https://docs.airbyte.com/integrations/sources/linkedin-pages/\\">docs</a> to obtain yours."""
     auth_method: Optional[SourceLinkedinPagesCredentialsOAuth20AuthMethodEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method'), 'exclude': lambda f: f is None }})
-
     
 class SourceLinkedinPagesLinkedinPagesEnum(str, Enum):
     LINKEDIN_PAGES = 'linkedin-pages'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLinkedinPages:
     r"""The values required to configure the source."""
     
     org_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('org_id') }})
-
     r"""Specify the Organization ID"""
     source_type: SourceLinkedinPagesLinkedinPagesEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_linnworks.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_snapchat_marketing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
+from datetime import date
 from enum import Enum
 from marshmallow import fields
+from typing import Optional
 
-class SourceLinnworksLinnworksEnum(str, Enum):
-    LINNWORKS = 'linnworks'
+class SourceSnapchatMarketingSnapchatMarketingEnum(str, Enum):
+    SNAPCHAT_MARKETING = 'snapchat-marketing'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceLinnworks:
+class SourceSnapchatMarketing:
     r"""The values required to configure the source."""
     
-    application_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('application_id') }})
-
-    r"""Linnworks Application ID"""
-    application_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('application_secret') }})
-
-    r"""Linnworks Application Secret"""
-    source_type: SourceLinnworksLinnworksEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
-    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
-    token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
+    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
+    r"""The Client ID of your Snapchat developer application."""
+    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
+    r"""The Client Secret of your Snapchat developer application."""
+    refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
+    r"""Refresh Token to renew the expired Access Token."""
+    source_type: SourceSnapchatMarketingSnapchatMarketingEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""Date in the format 2017-01-25. Any data after this date will not be replicated."""
+    start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""Date in the format 2022-01-01. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_lokalise.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_lokalise.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceLokalise:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Lokalise API Key with read-access. Available at Profile settings > API tokens. See <a href=\\"https://docs.lokalise.com/en/articles/1929556-api-tokens\\">here</a>."""
     project_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id') }})
-
     r"""Lokalise project ID. Available at Project Settings > General."""
     source_type: SourceLokaliseLokaliseEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mailchimp.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mailchimp.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,48 +12,39 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMailchimpCredentialsAPIKey:
     
     apikey: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apikey') }})
-
     r"""Mailchimp API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/mailchimp\\">docs</a> for information on how to generate this key."""
     auth_type: SourceMailchimpCredentialsAPIKeyAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     
 class SourceMailchimpCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMailchimpCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""An access token generated using the above client ID and secret."""
     auth_type: SourceMailchimpCredentialsOAuth20AuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
     r"""The Client ID of your OAuth application."""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""The Client Secret of your OAuth application."""
     
 class SourceMailchimpMailchimpEnum(str, Enum):
     MAILCHIMP = 'mailchimp'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMailchimp:
     r"""The values required to configure the source."""
     
     source_type: SourceMailchimpMailchimpEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     campaign_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('campaign_id'), 'exclude': lambda f: f is None }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mailgun.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mailgun.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMailgun:
     r"""The values required to configure the source."""
     
     private_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('private_key') }})
-
     r"""Primary account API key to access your Mailgun data."""
     source_type: SourceMailgunMailgunEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     domain_region: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_region'), 'exclude': lambda f: f is None }})
-
     r"""Domain region code. 'EU' or 'US' are possible values. The default is 'US'."""
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time in the format 2020-10-01 00:00:00. Any data before this date will not be replicated. If omitted, defaults to 3 days ago."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mailjet_sms.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mailjet_sms.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMailjetSms:
     r"""The values required to configure the source."""
     
     source_type: SourceMailjetSmsMailjetSmsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
     r"""Your access token. See <a href=\\"https://dev.mailjet.com/sms/reference/overview/authentication\\">here</a>."""
     end_date: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
-
     r"""Retrieve SMS messages created before the specified timestamp. Required format - Unix timestamp."""
     start_date: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'exclude': lambda f: f is None }})
-
     r"""Retrieve SMS messages created after the specified timestamp. Required format - Unix timestamp."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_marketo.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_marketo.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMarketo:
     r"""The values required to configure the source."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Marketo developer application. See <a href=\\"https://docs.airbyte.com/integrations/sources/marketo\\"> the docs </a> for info on how to obtain this."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Marketo developer application. See <a href=\\"https://docs.airbyte.com/integrations/sources/marketo\\"> the docs </a> for info on how to obtain this."""
     domain_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_url') }})
-
     r"""Your Marketo Base URL. See <a href=\\"https://docs.airbyte.com/integrations/sources/marketo\\"> the docs </a> for info on how to obtain this."""
     source_type: SourceMarketoMarketoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_metabase.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_metabase.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,25 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMetabase:
     r"""The values required to configure the source."""
     
     instance_api_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance_api_url') }})
-
     r"""URL to your metabase instance API"""
     source_type: SourceMetabaseMetabaseEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     session_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('session_token'), 'exclude': lambda f: f is None }})
-
     r"""To generate your session token, you need to run the following command: ``` curl -X POST \ 
       -H \"Content-Type: application/json\" \
       -d '{\"username\": \"person@metabase.com\", \"password\": \"fakepassword\"}' \
       http://localhost:3000/api/session
     ``` Then copy the value of the `id` field returned by a successful call to that API.
     Note that by default, sessions are good for 14 days and needs to be regenerated.
     """
     username: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_microsoft_teams.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_microsoft_teams.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,60 +13,48 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoft:
     r"""Choose how to authenticate to Microsoft"""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Microsoft Teams developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Microsoft Teams developer application."""
     tenant_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tenant_id') }})
-
     r"""A globally unique identifier (GUID) that is different than your organization name or domain. Follow these steps to obtain: open one of the Teams where you belong inside the Teams Application -> Click on the … next to the Team title -> Click on Get link to team -> Copy the link to the team and grab the tenant ID form the URL"""
     auth_type: Optional[SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum(str, Enum):
     CLIENT = 'Client'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20:
     r"""Choose how to authenticate to Microsoft"""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Microsoft Teams developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Microsoft Teams developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""A Refresh Token to renew the expired Access Token."""
     tenant_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tenant_id') }})
-
     r"""A globally unique identifier (GUID) that is different than your organization name or domain. Follow these steps to obtain: open one of the Teams where you belong inside the Teams Application -> Click on the … next to the Team title -> Click on Get link to team -> Copy the link to the team and grab the tenant ID form the URL"""
     auth_type: Optional[SourceMicrosoftTeamsCredentialsAuthenticateViaMicrosoftOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceMicrosoftTeamsMicrosoftTeamsEnum(str, Enum):
     MICROSOFT_TEAMS = 'microsoft-teams'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMicrosoftTeams:
     r"""The values required to configure the source."""
     
     period: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('period') }})
-
     r"""Specifies the length of time over which the Team Device Report stream is aggregated. The supported values are: D7, D30, D90, and D180."""
     source_type: SourceMicrosoftTeamsMicrosoftTeamsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to Microsoft"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mixpanel.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mixpanel.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,36 +16,31 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMixpanelCredentialsProjectSecret:
     r"""Choose how to authenticate to Mixpanel"""
     
     api_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_secret') }})
-
     r"""Mixpanel project secret. See the <a href=\\"https://developer.mixpanel.com/reference/project-secret#managing-a-projects-secret\\">docs</a> for more information on how to obtain this."""
     option_title: Optional[SourceMixpanelCredentialsProjectSecretOptionTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title'), 'exclude': lambda f: f is None }})
-
     
 class SourceMixpanelCredentialsServiceAccountOptionTitleEnum(str, Enum):
     SERVICE_ACCOUNT = 'Service Account'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMixpanelCredentialsServiceAccount:
     r"""Choose how to authenticate to Mixpanel"""
     
     secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret') }})
-
     r"""Mixpanel Service Account Secret. See the <a href=\\"https://developer.mixpanel.com/reference/service-accounts\\">docs</a> for more information on how to obtain this."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Mixpanel Service Account Username. See the <a href=\\"https://developer.mixpanel.com/reference/service-accounts\\">docs</a> for more information on how to obtain this."""
     option_title: Optional[SourceMixpanelCredentialsServiceAccountOptionTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title'), 'exclude': lambda f: f is None }})
-
     
 class SourceMixpanelRegionEnum(str, Enum):
     r"""The region of mixpanel domain instance either US or EU."""
     US = 'US'
     EU = 'EU'
 
 class SourceMixpanelMixpanelEnum(str, Enum):
@@ -54,36 +49,26 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMixpanel:
     r"""The values required to configure the source."""
     
     source_type: SourceMixpanelMixpanelEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     attribution_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attribution_window'), 'exclude': lambda f: f is None }})
-
     r"""A period of time for attributing results to ads and the lookback period after those actions occur during which ad results are counted. Default attribution window is 5 days."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to Mixpanel"""
     date_window_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date_window_size'), 'exclude': lambda f: f is None }})
-
     r"""Defines window size in days, that used to slice through data. You can reduce it, if amount of data in each window is too big for your environment."""
     end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date in the format YYYY-MM-DD. Any data after this date will not be replicated. Left empty to always sync to most recent date"""
     project_id: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_id'), 'exclude': lambda f: f is None }})
-
     r"""Your project ID number. See the <a href=\\"https://help.mixpanel.com/hc/en-us/articles/115004490503-Project-Settings#project-id\\">docs</a> for more information on how to obtain this."""
     project_timezone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_timezone'), 'exclude': lambda f: f is None }})
-
     r"""Time zone in which integer date times are stored. The project timezone may be found in the project settings in the <a href=\\"https://help.mixpanel.com/hc/en-us/articles/115004547203-Manage-Timezones-for-Projects-in-Mixpanel\\">Mixpanel console</a>."""
     region: Optional[SourceMixpanelRegionEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
-
     r"""The region of mixpanel domain instance either US or EU."""
     select_properties_by_default: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('select_properties_by_default'), 'exclude': lambda f: f is None }})
-
     r"""Setting this config parameter to TRUE ensures that new properties on events and engage records are captured. Otherwise new properties will be ignored."""
     start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date in the format YYYY-MM-DD. Any data before this date will not be replicated. If this option is not set, the connector will replicate data from up to one year ago by default."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_monday.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_monday.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,49 +12,40 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMondayCredentialsAPIToken:
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""API Token for making authenticated requests."""
     auth_type: SourceMondayCredentialsAPITokenAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     
 class SourceMondayCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMondayCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token for making authenticated requests."""
     auth_type: SourceMondayCredentialsOAuth20AuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your OAuth application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your OAuth application."""
     subdomain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain'), 'exclude': lambda f: f is None }})
-
     r"""Slug/subdomain of the account, or the first part of the URL that comes before .monday.com"""
     
 class SourceMondayMondayEnum(str, Enum):
     MONDAY = 'monday'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMonday:
     r"""The values required to configure the source."""
     
     source_type: SourceMondayMondayEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mongodb.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,75 +13,61 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMongodbInstanceTypeMongoDBAtlas:
     r"""The MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     
     cluster_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cluster_url') }})
-
     r"""The URL of a cluster to connect to."""
     instance: SourceMongodbInstanceTypeMongoDBAtlasInstanceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance') }})
-
     
 class SourceMongodbInstanceTypeReplicaSetInstanceEnum(str, Enum):
     REPLICA = 'replica'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMongodbInstanceTypeReplicaSet:
     r"""The MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     
     instance: SourceMongodbInstanceTypeReplicaSetInstanceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance') }})
-
     server_addresses: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('server_addresses') }})
-
     r"""The members of a replica set. Please specify `host`:`port` of each member separated by comma."""
     replica_set: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replica_set'), 'exclude': lambda f: f is None }})
-
     r"""A replica set in MongoDB is a group of mongod processes that maintain the same data set."""
     
 class SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum(str, Enum):
     STANDALONE = 'standalone'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMongodbInstanceTypeStandaloneMongoDbInstance:
     r"""The MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The host name of the Mongo database."""
     instance: SourceMongodbInstanceTypeStandaloneMongoDbInstanceInstanceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance') }})
-
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The port of the Mongo database."""
     
 class SourceMongodbMongodbEnum(str, Enum):
     MONGODB = 'mongodb'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMongodb:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The database you want to replicate."""
     source_type: SourceMongodbMongodbEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     auth_source: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_source'), 'exclude': lambda f: f is None }})
-
     r"""The authentication source where the user information is stored."""
     instance_type: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('instance_type'), 'exclude': lambda f: f is None }})
-
     r"""The MongoDb instance to connect to. For MongoDB Atlas and Replica Set TLS connection is used by default."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with this username."""
     user: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user'), 'exclude': lambda f: f is None }})
-
     r"""The username which is used to access the database."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mssql.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mssql.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,165 +23,135 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlReplicationMethodLogicalReplicationCDC:
     r"""CDC uses {TBC} to detect inserts, updates, and deletes. This needs to be configured on the source database itself."""
     
     method: SourceMssqlReplicationMethodLogicalReplicationCDCMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     data_to_sync: Optional[SourceMssqlReplicationMethodLogicalReplicationCDCDataToSyncEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data_to_sync'), 'exclude': lambda f: f is None }})
-
     r"""What data should be synced under the CDC. \\"Existing and New\\" will read existing data as a snapshot, and sync new changes through CDC. \\"New Changes Only\\" will skip the initial snapshot, and only sync new changes through CDC."""
     initial_waiting_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('initial_waiting_seconds'), 'exclude': lambda f: f is None }})
-
     r"""The amount of time the connector will wait when it launches to determine if there is new data to sync or not. Defaults to 300 seconds. Valid range: 120 seconds to 1200 seconds. Read about <a href=\\"https://docs.airbyte.com/integrations/sources/mysql/#change-data-capture-cdc\\">initial waiting time</a>."""
     snapshot_isolation: Optional[SourceMssqlReplicationMethodLogicalReplicationCDCInitialSnapshotIsolationLevelEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('snapshot_isolation'), 'exclude': lambda f: f is None }})
-
     r"""Existing data in the database are synced through an initial snapshot. This parameter controls the isolation level that will be used during the initial snapshotting. If you choose the \\"Snapshot\\" level, you must enable the <a href=\\"https://docs.microsoft.com/en-us/dotnet/framework/data/adonet/sql/snapshot-isolation-in-sql-server\\">snapshot isolation mode</a> on the database."""
     
 class SourceMssqlReplicationMethodStandardMethodEnum(str, Enum):
     STANDARD = 'STANDARD'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlReplicationMethodStandard:
     r"""Standard replication requires no setup on the DB side but will not be able to represent deletions incrementally."""
     
     method: SourceMssqlReplicationMethodStandardMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class SourceMssqlMssqlEnum(str, Enum):
     MSSQL = 'mssql'
 
 class SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum(str, Enum):
     ENCRYPTED_VERIFY_CERTIFICATE = 'encrypted_verify_certificate'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlSslMethodEncryptedVerifyCertificate:
     r"""Verify and use the certificate provided by the server."""
     
     ssl_method: SourceMssqlSslMethodEncryptedVerifyCertificateSslMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_method') }})
-
     host_name_in_certificate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hostNameInCertificate'), 'exclude': lambda f: f is None }})
-
     r"""Specifies the host name of the server. The value of this property must match the subject property of the certificate."""
     
 class SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum(str, Enum):
     ENCRYPTED_TRUST_SERVER_CERTIFICATE = 'encrypted_trust_server_certificate'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlSslMethodEncryptedTrustServerCertificate:
     r"""Use the certificate provided by the server without verification. (For testing purposes only!)"""
     
     ssl_method: SourceMssqlSslMethodEncryptedTrustServerCertificateSslMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_method') }})
-
     
 class SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceMssqlTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceMssqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssqlTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: SourceMssqlTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMssql:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The name of the database."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The port of the database."""
     source_type: SourceMssqlMssqlEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username which is used to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with the username."""
     replication_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_method'), 'exclude': lambda f: f is None }})
-
     r"""The replication method used for extracting data from the database. STANDARD replication requires no setup on the DB side but will not be able to represent deletions incrementally. CDC uses {TBC} to detect inserts, updates, and deletes. This needs to be configured on the source database itself."""
     schemas: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schemas'), 'exclude': lambda f: f is None }})
-
     r"""The list of schemas to sync from. Defaults to user. Case sensitive."""
     ssl_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_method'), 'exclude': lambda f: f is None }})
-
     r"""The encryption method which is used when communicating with the database."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_my_hours.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_my_hours.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMyHours:
     r"""The values required to configure the source."""
     
     email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
     r"""Your My Hours username"""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""The password associated to the username"""
     source_type: SourceMyHoursMyHoursEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""Start date for collecting time logs"""
     logs_batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('logs_batch_size'), 'exclude': lambda f: f is None }})
-
     r"""Pagination size used for retrieving logs in days"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_mysql.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,204 +13,167 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlReplicationMethodLogicalReplicationCDC:
     r"""CDC uses the Binlog to detect inserts, updates, and deletes. This needs to be configured on the source database itself."""
     
     method: SourceMysqlReplicationMethodLogicalReplicationCDCMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     initial_waiting_seconds: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('initial_waiting_seconds'), 'exclude': lambda f: f is None }})
-
     r"""The amount of time the connector will wait when it launches to determine if there is new data to sync or not. Defaults to 300 seconds. Valid range: 120 seconds to 1200 seconds. Read about <a href=\\"https://docs.airbyte.com/integrations/sources/mysql/#change-data-capture-cdc\\">initial waiting time</a>."""
     server_time_zone: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('server_time_zone'), 'exclude': lambda f: f is None }})
-
     r"""Enter the configured MySQL server timezone. This should only be done if the configured timezone in your MySQL instance does not conform to IANNA standard."""
     
 class SourceMysqlReplicationMethodStandardMethodEnum(str, Enum):
     STANDARD = 'STANDARD'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlReplicationMethodStandard:
     r"""Standard replication requires no setup on the DB side but will not be able to represent deletions incrementally."""
     
     method: SourceMysqlReplicationMethodStandardMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class SourceMysqlMysqlEnum(str, Enum):
     MYSQL = 'mysql'
 
 class SourceMysqlSslModeVerifyIdentityModeEnum(str, Enum):
     VERIFY_IDENTITY = 'verify_identity'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlSslModeVerifyIdentity:
     r"""Always connect with SSL. Verify both CA and Hostname."""
     
     ca_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ca_certificate') }})
-
     r"""CA certificate"""
     mode: SourceMysqlSslModeVerifyIdentityModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     client_certificate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_certificate'), 'exclude': lambda f: f is None }})
-
     r"""Client certificate (this is not a required field, but if you want to use it, you will need to add the <b>Client key</b> as well)"""
     client_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key'), 'exclude': lambda f: f is None }})
-
     r"""Client key (this is not a required field, but if you want to use it, you will need to add the <b>Client certificate</b> as well)"""
     client_key_password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key_password'), 'exclude': lambda f: f is None }})
-
     r"""Password for keystorage. This field is optional. If you do not add it - the password will be generated automatically."""
     
 class SourceMysqlSslModeVerifyCAModeEnum(str, Enum):
     VERIFY_CA = 'verify_ca'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlSslModeVerifyCA:
     r"""Always connect with SSL. Verifies CA, but allows connection even if Hostname does not match."""
     
     ca_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ca_certificate') }})
-
     r"""CA certificate"""
     mode: SourceMysqlSslModeVerifyCAModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     client_certificate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_certificate'), 'exclude': lambda f: f is None }})
-
     r"""Client certificate (this is not a required field, but if you want to use it, you will need to add the <b>Client key</b> as well)"""
     client_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key'), 'exclude': lambda f: f is None }})
-
     r"""Client key (this is not a required field, but if you want to use it, you will need to add the <b>Client certificate</b> as well)"""
     client_key_password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_key_password'), 'exclude': lambda f: f is None }})
-
     r"""Password for keystorage. This field is optional. If you do not add it - the password will be generated automatically."""
     
 class SourceMysqlSslModeRequiredModeEnum(str, Enum):
     REQUIRED = 'required'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlSslModeRequired:
     r"""Always connect with SSL. If the MySQL server doesn’t support SSL, the connection will not be established. Certificate Authority (CA) and Hostname are not verified."""
     
     mode: SourceMysqlSslModeRequiredModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class SourceMysqlSslModePreferredModeEnum(str, Enum):
     PREFERRED = 'preferred'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlSslModePreferred:
     r"""Automatically attempt SSL connection. If the MySQL server does not support SSL, continue with a regular connection."""
     
     mode: SourceMysqlSslModePreferredModeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mode') }})
-
     
 class SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceMysqlTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceMysqlTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysqlTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: SourceMysqlTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceMysql:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The database name."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The host name of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The port to connect to."""
     replication_method: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_method') }})
-
     r"""Replication method to use for extracting data from the database."""
     source_type: SourceMysqlMysqlEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username which is used to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3). For more information read about <a href=\\"https://dev.mysql.com/doc/connector-j/8.0/en/connector-j-reference-jdbc-url-format.html\\">JDBC URL parameters</a>."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with the username."""
     ssl_mode: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_mode'), 'exclude': lambda f: f is None }})
-
     r"""SSL connection modes. Read more <a href=\\"https://dev.mysql.com/doc/connector-j/8.0/en/connector-j-reference-using-ssl.html\\"> in the docs</a>."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_netsuite.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_netsuite.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,33 +13,24 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceNetsuite:
     r"""The values required to configure the source."""
     
     consumer_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('consumer_key') }})
-
     r"""Consumer key associated with your integration"""
     consumer_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('consumer_secret') }})
-
     r"""Consumer secret associated with your integration"""
     realm: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('realm') }})
-
     r"""Netsuite realm e.g. 2344535, as for `production` or 2344535_SB1, as for the `sandbox`"""
     source_type: SourceNetsuiteNetsuiteEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_datetime: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_datetime') }})
-
     r"""Starting point for your data replication, in format of \\"YYYY-MM-DDTHH:mm:ssZ\\" """
     token_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_key') }})
-
     r"""Access token key"""
     token_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_secret') }})
-
     r"""Access token secret"""
     object_types: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_types'), 'exclude': lambda f: f is None }})
-
     r"""The API names of the Netsuite objects you want to sync. Setting this speeds up the connection setup process by limiting the number of schemas that need to be retrieved from Netsuite."""
     window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-
     r"""The amount of days used to query the data with date chunks. Set smaller value, if you have lots of data."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_notion.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_notion.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,51 +16,42 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceNotionCredentialsAccessToken:
     r"""Pick an authentication method."""
     
     auth_type: SourceNotionCredentialsAccessTokenAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
     r"""Notion API access token, see the <a href=\\"https://developers.notion.com/docs/authorization\\">docs</a> for more information on how to obtain this token."""
     
 class SourceNotionCredentialsOAuth20AuthTypeEnum(str, Enum):
     O_AUTH2_0 = 'OAuth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceNotionCredentialsOAuth20:
     r"""Pick an authentication method."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token is a token you received by complete the OauthWebFlow of Notion."""
     auth_type: SourceNotionCredentialsOAuth20AuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The ClientID of your Notion integration."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The ClientSecret of your Notion integration."""
     
 class SourceNotionNotionEnum(str, Enum):
     NOTION = 'notion'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceNotion:
     r"""The values required to configure the source."""
     
     source_type: SourceNotionNotionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00.000Z. Any data before this date will not be replicated."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Pick an authentication method."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_nytimes.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_nytimes.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceNytimes:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key"""
     period: SourceNytimesPeriodUsedForMostPopularStreamsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('period') }})
-
     r"""Period of time (in days)"""
     source_type: SourceNytimesNytimesEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""Start date to begin the article retrieval (format YYYY-MM)"""
     end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""End date to stop the article retrieval (format YYYY-MM)"""
     share_type: Optional[SourceNytimesShareTypeUsedForMostPopularSharedStreamEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('share_type'), 'exclude': lambda f: f is None }})
-
     r"""Share Type"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_okta.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_okta.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,52 +12,42 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOktaCredentialsAPIToken:
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""An Okta token. See the <a href=\\"https://docs.airbyte.com/integrations/sources/okta\\">docs</a> for instructions on how to generate it."""
     auth_type: SourceOktaCredentialsAPITokenAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     
 class SourceOktaCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOktaCredentialsOAuth20:
     
     auth_type: SourceOktaCredentialsOAuth20AuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your OAuth application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your OAuth application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Refresh Token to obtain new Access Token, when it's expired."""
     
 class SourceOktaOktaEnum(str, Enum):
     OKTA = 'okta'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOkta:
     r"""The values required to configure the source."""
     
     source_type: SourceOktaOktaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     domain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain'), 'exclude': lambda f: f is None }})
-
     r"""The Okta domain. See the <a href=\\"https://docs.airbyte.com/integrations/sources/okta\\">docs</a> for instructions on how to find it."""
     start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'exclude': lambda f: f is None }})
-
     r"""UTC date and time in the format YYYY-MM-DDTHH:MM:SSZ. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_omnisend.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pokeapi.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourceOmnisendOmnisendEnum(str, Enum):
-    OMNISEND = 'omnisend'
+class SourcePokeapiPokeapiEnum(str, Enum):
+    POKEAPI = 'pokeapi'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceOmnisend:
+class SourcePokeapi:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""API Key"""
-    source_type: SourceOmnisendOmnisendEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    pokemon_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pokemon_name') }})
+    r"""Pokemon requested from the API."""
+    source_type: SourcePokeapiPokeapiEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_onesignal.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_onesignal.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,37 +12,29 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOnesignalApplications:
     
     app_api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('app_api_key') }})
-
     app_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('app_id') }})
-
     app_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('app_name'), 'exclude': lambda f: f is None }})
-
     
 class SourceOnesignalOnesignalEnum(str, Enum):
     ONESIGNAL = 'onesignal'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOnesignal:
     r"""The values required to configure the source."""
     
     applications: list[SourceOnesignalApplications] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('applications') }})
-
     r"""Applications keys, see the <a href=\\"https://documentation.onesignal.com/docs/accounts-and-keys\\">docs</a> for more information on how to obtain this data"""
     outcome_names: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('outcome_names') }})
-
     r"""Comma-separated list of names and the value (sum/count) for the returned outcome data. See the <a href=\\"https://documentation.onesignal.com/reference/view-outcomes\\">docs</a> for more details"""
     source_type: SourceOnesignalOnesignalEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for OneSignal API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
     user_auth_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user_auth_key') }})
-
     r"""OneSignal User Auth Key, see the <a href=\\"https://documentation.onesignal.com/docs/accounts-and-keys#user-auth-key\\">docs</a> for more information on how to obtain this key."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_openweather.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_openweather.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,24 +71,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOpenweather:
     r"""The values required to configure the source."""
     
     appid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('appid') }})
-
     r"""Your OpenWeather API Key. See <a href=\\"https://openweathermap.org/api\\">here</a>. The key is case sensitive."""
     lat: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lat') }})
-
     r"""Latitude for which you want to get weather condition from. (min -90, max 90)"""
     lon: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lon') }})
-
     r"""Longitude for which you want to get weather condition from. (min -180, max 180)"""
     source_type: SourceOpenweatherOpenweatherEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     lang: Optional[SourceOpenweatherLanguageEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lang'), 'exclude': lambda f: f is None }})
-
     r"""You can use lang parameter to get the output in your language. The contents of the description field will be translated. See <a href=\\"https://openweathermap.org/api/one-call-api#multi\\">here</a> for the list of supported languages."""
     units: Optional[SourceOpenweatherUnitsEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('units'), 'exclude': lambda f: f is None }})
-
     r"""Units of measurement. standard, metric and imperial units are available. If you do not use the units parameter, standard units will be applied by default."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_oracle.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,45 +13,39 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleConnectionDataSystemIDSID:
     r"""Use SID (Oracle System Identifier)"""
     
     sid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sid') }})
-
     connection_type: Optional[SourceOracleConnectionDataSystemIDSIDConnectionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceOracleConnectionDataServiceNameConnectionTypeEnum(str, Enum):
     SERVICE_NAME = 'service_name'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleConnectionDataServiceName:
     r"""Use service name"""
     
     service_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_name') }})
-
     connection_type: Optional[SourceOracleConnectionDataServiceNameConnectionTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum(str, Enum):
     ENCRYPTED_VERIFY_CERTIFICATE = 'encrypted_verify_certificate'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleEncryptionTLSEncryptedVerifyCertificate:
     r"""Verify and use the certificate provided by the server."""
     
     encryption_method: SourceOracleEncryptionTLSEncryptedVerifyCertificateEncryptionMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_method') }})
-
     ssl_certificate: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_certificate') }})
-
     r"""Privacy Enhanced Mail (PEM) files are concatenated certificate containers frequently used in certificate installations."""
     
 class SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum(str, Enum):
     r"""This parameter defines what encryption algorithm is used."""
     AES256 = 'AES256'
     RC4_56 = 'RC4_56'
     THREE_DES168 = '3DES168'
@@ -62,17 +56,15 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleEncryptionNativeNetworkEncryptionNNE:
     r"""The native network encryption gives you the ability to encrypt database connections, without the configuration overhead of TCP/IP and SSL/TLS and without the need to open and listen on different ports."""
     
     encryption_method: SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_method') }})
-
     encryption_algorithm: Optional[SourceOracleEncryptionNativeNetworkEncryptionNNEEncryptionAlgorithmEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption_algorithm'), 'exclude': lambda f: f is None }})
-
     r"""This parameter defines what encryption algorithm is used."""
     
 class SourceOracleOracleEnum(str, Enum):
     ORACLE = 'oracle'
 
 class SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
@@ -81,102 +73,81 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceOracleTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourceOracleTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class SourceOracleTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracleTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: SourceOracleTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOracle:
     r"""The values required to configure the source."""
     
     encryption: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encryption') }})
-
     r"""The encryption method with is used when communicating with the database."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database.
     Oracle Corporations recommends the following port numbers:
     1521 - Default listening port for client connections to the listener. 
     2484 - Recommended and officially registered listening port for client connections to the listener using TCP/IP with SSL
     """
     source_type: SourceOracleOracleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username which is used to access the database."""
     connection_data: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connection_data'), 'exclude': lambda f: f is None }})
-
     r"""Connect data that will be used for DB connection"""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""The password associated with the username."""
     schemas: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schemas'), 'exclude': lambda f: f is None }})
-
     r"""The list of schemas to sync from. Defaults to user. Case sensitive."""
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_orb.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_orb.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,22 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOrb:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Orb API Key, issued from the Orb admin console."""
     source_type: SourceOrbOrbEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""UTC date and time in the format 2022-03-01T00:00:00Z. Any data with created_at before this data will not be synced. For Subscription Usage, this becomes the `timeframe_start` API parameter."""
     lookback_window_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window_days'), 'exclude': lambda f: f is None }})
-
     r"""When set to N, the connector will always refresh resources created within the past N days. By default, updated objects that are not newly created are not incrementally synced."""
     numeric_event_properties_keys: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('numeric_event_properties_keys'), 'exclude': lambda f: f is None }})
-
     r"""Property key names to extract from all events, in order to enrich ledger entries corresponding to an event deduction."""
     plan_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('plan_id'), 'exclude': lambda f: f is None }})
-
     r"""Orb Plan ID to filter subscriptions that should have usage fetched."""
     string_event_properties_keys: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('string_event_properties_keys'), 'exclude': lambda f: f is None }})
-
     r"""Property key names to extract from all events, in order to enrich ledger entries corresponding to an event deduction."""
     subscription_usage_grouping_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subscription_usage_grouping_key'), 'exclude': lambda f: f is None }})
-
     r"""Property key name to group subscription usage by."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_orbit.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_orbit.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOrbit:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Authorizes you to work with Orbit workspaces associated with the token."""
     source_type: SourceOrbitOrbitEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     workspace: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspace') }})
-
     r"""The unique name of the workspace that your API token is associated with."""
     start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'exclude': lambda f: f is None }})
-
     r"""Date in the format 2022-06-26. Only load members whose last activities are after this date."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_outreach.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_outreach.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceOutreach:
     r"""The values required to configure the source."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Outreach developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Outreach developer application."""
     redirect_uri: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('redirect_uri') }})
-
     r"""A Redirect URI is the location where the authorization server sends the user once the app has been successfully authorized and granted an authorization code or access token."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining the new access token."""
     source_type: SourceOutreachOutreachEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The date from which you'd like to replicate data for Outreach API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_paypal_transaction.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_paypal_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,24 +13,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePaypalTransaction:
     r"""The values required to configure the source."""
     
     is_sandbox: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox') }})
-
     r"""Determines whether to use the sandbox or production environment."""
     source_type: SourcePaypalTransactionPaypalTransactionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""Start Date for data extraction in <a href=\\"https://datatracker.ietf.org/doc/html/rfc3339#section-5.6\\">ISO format</a>. Date must be in range from 3 years till 12 hrs before present time."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
     r"""The Client ID of your Paypal developer application."""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""The Client Secret of your Paypal developer application."""
     refresh_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token'), 'exclude': lambda f: f is None }})
-
     r"""The key to refresh the expired access token."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_paystack.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_paystack.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePaystack:
     r"""The values required to configure the source."""
     
     secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
-
     r"""The Paystack API key (usually starts with 'sk_live_'; find yours <a href=\\"https://dashboard.paystack.com/#/settings/developer\\">here</a>)."""
     source_type: SourcePaystackPaystackEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     lookback_window_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window_days'), 'exclude': lambda f: f is None }})
-
     r"""When set, the connector will always reload data from the past N days, where N is the value set here. This is useful if your data is updated after creation."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pendo.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_tempo.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourcePendoPendoEnum(str, Enum):
-    PENDO = 'pendo'
+class SourceTempoTempoEnum(str, Enum):
+    TEMPO = 'tempo'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePendo:
+class SourceTempo:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    source_type: SourcePendoPendoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
+    r"""Tempo API Token. Go to Tempo>Settings, scroll down to Data Access and select API integration."""
+    source_type: SourceTempoTempoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_persistiq.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pypi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
+from typing import Optional
 
-class SourcePersistiqPersistiqEnum(str, Enum):
-    PERSISTIQ = 'persistiq'
+class SourcePypiPypiEnum(str, Enum):
+    PYPI = 'pypi'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePersistiq:
+class SourcePypi:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""PersistIq API Key. See the <a href=\\"https://apidocs.persistiq.com/#authentication\\">docs</a> for more information on where to find that key."""
-    source_type: SourcePersistiqPersistiqEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    project_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_name') }})
+    r"""Name of the project/package. Can only be in lowercase with hyphen. This is the name used using pip command for installing the package."""
+    source_type: SourcePypiPypiEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version'), 'exclude': lambda f: f is None }})
+    r"""Version of the project/package.  Use it to find a particular release instead of all releases."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pexels_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pexels_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePexelsAPI:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API key is required to access pexels api, For getting your's goto https://www.pexels.com/api/documentation and create account for free."""
     query: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
-
     r"""Optional, the search query, Example Ocean, Tigers, Pears, etc."""
     source_type: SourcePexelsAPIPexelsAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     color: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('color'), 'exclude': lambda f: f is None }})
-
     r"""Optional, Desired photo color. Supported colors red, orange, yellow, green, turquoise, blue, violet, pink, brown, black, gray, white or any hexidecimal color code."""
     locale: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('locale'), 'exclude': lambda f: f is None }})
-
     r"""Optional, The locale of the search you are performing. The current supported locales are 'en-US' 'pt-BR' 'es-ES' 'ca-ES' 'de-DE' 'it-IT' 'fr-FR' 'sv-SE' 'id-ID' 'pl-PL' 'ja-JP' 'zh-TW' 'zh-CN' 'ko-KR' 'th-TH' 'nl-NL' 'hu-HU' 'vi-VN' 'cs-CZ' 'da-DK' 'fi-FI' 'uk-UA' 'el-GR' 'ro-RO' 'nb-NO' 'sk-SK' 'tr-TR' 'ru-RU'."""
     orientation: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('orientation'), 'exclude': lambda f: f is None }})
-
     r"""Optional, Desired photo orientation. The current supported orientations are landscape, portrait or square"""
     size: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('size'), 'exclude': lambda f: f is None }})
-
     r"""Optional, Minimum photo size. The current supported sizes are large(24MP), medium(12MP) or small(4MP)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pinterest.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pinterest.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,37 +12,31 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePinterestCredentialsAccessToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The Access Token to make authenticated requests."""
     auth_method: SourcePinterestCredentialsAccessTokenAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
     
 class SourcePinterestCredentialsOAuth20AuthMethodEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePinterestCredentialsOAuth20:
     
     auth_method: SourcePinterestCredentialsOAuth20AuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Refresh Token to obtain new Access Token, when it's expired."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
     r"""The Client ID of your OAuth application"""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""The Client Secret of your OAuth application."""
     
 class SourcePinterestPinterestEnum(str, Enum):
     PINTEREST = 'pinterest'
 
 class SourcePinterestStatusEnum(str, Enum):
     ACTIVE = 'ACTIVE'
@@ -52,17 +46,13 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePinterest:
     r"""The values required to configure the source."""
     
     source_type: SourcePinterestPinterestEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""A date in the format YYYY-MM-DD. If you have not set a date, it would be defaulted to latest allowed date by api (914 days from today)."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     status: Optional[list[SourcePinterestStatusEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-
     r"""Entity statuses based off of campaigns, ad_groups, and ads. If you do not have a status set, it will be ignored completely."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pipedrive.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pipedrive.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,29 +15,24 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePipedriveAPIKeyAuthentication:
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""The Pipedrive API Token."""
     auth_type: SourcePipedriveAPIKeyAuthenticationAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     
 class SourcePipedrivePipedriveEnum(str, Enum):
     PIPEDRIVE = 'pipedrive'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePipedrive:
     r"""The values required to configure the source."""
     
     replication_start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated. When specified and not None, then stream will behave as incremental"""
     source_type: SourcePipedrivePipedriveEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     authorization: Optional[SourcePipedriveAPIKeyAuthentication] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authorization'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pocket.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,42 +37,30 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePocket:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The user's Pocket access token."""
     consumer_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('consumer_key') }})
-
     r"""Your application's Consumer Key."""
     source_type: SourcePocketPocketEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     content_type: Optional[SourcePocketContentTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('content_type'), 'exclude': lambda f: f is None }})
-
     r"""Select the content type of the items to retrieve."""
     detail_type: Optional[SourcePocketDetailTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detail_type'), 'exclude': lambda f: f is None }})
-
     r"""Select the granularity of the information about each item."""
     domain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain'), 'exclude': lambda f: f is None }})
-
     r"""Only return items from a particular `domain`."""
     favorite: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('favorite'), 'exclude': lambda f: f is None }})
-
     r"""Retrieve only favorited items."""
     search: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('search'), 'exclude': lambda f: f is None }})
-
     r"""Only return items whose title or url contain the `search` string."""
     since: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('since'), 'exclude': lambda f: f is None }})
-
     r"""Only return items modified since the given timestamp."""
     sort: Optional[SourcePocketSortByEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sort'), 'exclude': lambda f: f is None }})
-
     r"""Sort retrieved items by the given criteria."""
     state: Optional[SourcePocketStateEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('state'), 'exclude': lambda f: f is None }})
-
     r"""Select the state of the items to retrieve."""
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-
     r"""Return only items tagged with this tag name. Use _untagged_ for retrieving only untagged items."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pokeapi.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_postmarkapp.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourcePokeapiPokeapiEnum(str, Enum):
-    POKEAPI = 'pokeapi'
+class SourcePostmarkappPostmarkappEnum(str, Enum):
+    POSTMARKAPP = 'postmarkapp'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePokeapi:
+class SourcePostmarkapp:
     r"""The values required to configure the source."""
     
-    pokemon_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pokemon_name') }})
-
-    r"""Pokemon requested from the API."""
-    source_type: SourcePokeapiPokeapiEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    source_type: SourcePostmarkappPostmarkappEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    x_postmark_account_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('X-Postmark-Account-Token') }})
+    r"""API Key for account"""
+    x_postmark_server_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('X-Postmark-Server-Token') }})
+    r"""API Key for server"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_polygon_stock_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_polygon_stock_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,36 +15,26 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePolygonStockAPI:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apiKey') }})
-
     r"""Your API ACCESS Key"""
     end_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The target date for the aggregate window."""
     multiplier: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('multiplier') }})
-
     r"""The size of the timespan multiplier."""
     source_type: SourcePolygonStockAPIPolygonStockAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The beginning date for the aggregate window."""
     stocks_ticker: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stocksTicker') }})
-
     r"""The exchange symbol that this item is traded under."""
     timespan: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('timespan') }})
-
     r"""The size of the time window."""
     adjusted: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('adjusted'), 'exclude': lambda f: f is None }})
-
     r"""Determines whether or not the results are adjusted for splits. By default, results are adjusted and set to true. Set this to false to get results that are NOT adjusted for splits."""
     limit: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('limit'), 'exclude': lambda f: f is None }})
-
     r"""The target date for the aggregate window."""
     sort: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sort'), 'exclude': lambda f: f is None }})
-
     r"""Sort the results by timestamp. asc will return results in ascending order (oldest at the top), desc will return results in descending order (newest at the top)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_postgres.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_postgres.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePostgresReplicationMethodStandard:
     r"""Standard replication requires no setup on the DB side but will not be able to represent deletions incrementally."""
     
     method: SourcePostgresReplicationMethodStandardMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('method') }})
-
     
 class SourcePostgresPostgresEnum(str, Enum):
     POSTGRES = 'postgres'
 
 class SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
@@ -29,103 +28,81 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePostgresTunnelMethodPasswordAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourcePostgresTunnelMethodPasswordAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and password authentication"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host"""
     tunnel_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum(str, Enum):
     r"""Connect through a jump server tunnel host using username and ssh key"""
     SSH_KEY_AUTH = 'SSH_KEY_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePostgresTunnelMethodSSHKeyAuthentication:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     tunnel_host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_host') }})
-
     r"""Hostname of the jump server host that allows inbound ssh tunnel."""
     tunnel_method: SourcePostgresTunnelMethodSSHKeyAuthenticationTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""Connect through a jump server tunnel host using username and ssh key"""
     tunnel_port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_port') }})
-
     r"""Port on the proxy/jump server that accepts inbound ssh connections."""
     tunnel_user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_user') }})
-
     r"""OS-level username for logging into the jump server host."""
     
 class SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum(str, Enum):
     r"""No ssh tunnel needed to connect to database"""
     NO_TUNNEL = 'NO_TUNNEL'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePostgresTunnelMethodNoTunnel:
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
     
     tunnel_method: SourcePostgresTunnelMethodNoTunnelTunnelMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method') }})
-
     r"""No ssh tunnel needed to connect to database"""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePostgres:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Hostname of the database."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database."""
     source_type: SourcePostgresPostgresEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (Eg. key1=value1&key2=value2&key3=value3). For more information read about <a href=\\"https://jdbc.postgresql.org/documentation/head/connect.html\\">JDBC URL parameters</a>."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""Password associated with the username."""
     replication_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('replication_method'), 'exclude': lambda f: f is None }})
-
     r"""Replication method for extracting data from the database."""
     schemas: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schemas'), 'exclude': lambda f: f is None }})
-
     r"""The list of schemas (case sensitive) to sync from. Defaults to public."""
     ssl_mode: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ssl_mode'), 'exclude': lambda f: f is None }})
-
     r"""SSL connection modes.
       Read more <a href=\"https://jdbc.postgresql.org/documentation/head/ssl-client.html\"> in the docs</a>.
     """
     tunnel_method: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tunnel_method'), 'exclude': lambda f: f is None }})
-
     r"""Whether to initiate an SSH tunnel before connecting to the database, and if so, which kind of authentication to use."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_posthog.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_posthog.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePosthog:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key. See the <a href=\\"https://docs.airbyte.com/integrations/sources/posthog\\">docs</a> for information on how to generate this key."""
     source_type: SourcePosthogPosthogEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate the data. Any data before this date will not be replicated."""
     base_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base_url'), 'exclude': lambda f: f is None }})
-
     r"""Base PostHog url. Defaults to PostHog Cloud (https://app.posthog.com)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_postmarkapp.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_younium.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
+from typing import Optional
 
-class SourcePostmarkappPostmarkappEnum(str, Enum):
-    POSTMARKAPP = 'postmarkapp'
+class SourceYouniumYouniumEnum(str, Enum):
+    YOUNIUM = 'younium'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePostmarkapp:
+class SourceYounium:
     r"""The values required to configure the source."""
     
-    source_type: SourcePostmarkappPostmarkappEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    x_postmark_account_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('X-Postmark-Account-Token') }})
-
-    r"""API Key for account"""
-    x_postmark_server_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('X-Postmark-Server-Token') }})
-
-    r"""API Key for server"""
+    legal_entity: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('legal_entity') }})
+    r"""Legal Entity that data should be pulled from"""
+    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
+    r"""Account password for younium account API key"""
+    source_type: SourceYouniumYouniumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
+    r"""Username for Younium account"""
+    playground: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playground'), 'exclude': lambda f: f is None }})
+    r"""Property defining if connector is used against playground or production environment"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_prestashop.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_prestashop.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePrestashop:
     r"""The values required to configure the source."""
     
     access_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_key') }})
-
     r"""Your PrestaShop access key. See <a href=\\"https://devdocs.prestashop.com/1.7/webservice/tutorials/creating-access/#create-an-access-key\\"> the docs </a> for info on how to obtain this."""
     source_type: SourcePrestashopPrestashopEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The Start date in the format YYYY-MM-DD."""
     url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-
     r"""Shop URL without trailing slash."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_public_apis.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_public_apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePublicApis:
     r"""The values required to configure the source."""
     
     source_type: SourcePublicApisPublicApisEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_punk_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_punk_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourcePunkAPI:
     r"""The values required to configure the source."""
     
     brewed_after: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('brewed_after') }})
-
     r"""To extract specific data with Unique ID"""
     brewed_before: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('brewed_before') }})
-
     r"""To extract specific data with Unique ID"""
     source_type: SourcePunkAPIPunkAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
     r"""To extract specific data with Unique ID"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_pypi.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_spacex_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,20 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class SourcePypiPypiEnum(str, Enum):
-    PYPI = 'pypi'
+class SourceSpacexAPISpacexAPIEnum(str, Enum):
+    SPACEX_API = 'spacex-api'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcePypi:
+class SourceSpacexAPI:
     r"""The values required to configure the source."""
     
-    project_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project_name') }})
-
-    r"""Name of the project/package. Can only be in lowercase with hyphen. This is the name used using pip command for installing the package."""
-    source_type: SourcePypiPypiEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    version: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('version'), 'exclude': lambda f: f is None }})
-
-    r"""Version of the project/package.  Use it to find a particular release instead of all releases."""
+    source_type: SourceSpacexAPISpacexAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
+    options: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_qualaroo.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_qualaroo.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceQualaroo:
     r"""The values required to configure the source."""
     
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-
     r"""A Qualaroo token. See the <a href=\\"https://help.qualaroo.com/hc/en-us/articles/201969438-The-REST-Reporting-API\\">docs</a> for instructions on how to generate it."""
     source_type: SourceQualarooQualarooEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
     r"""A Qualaroo token. See the <a href=\\"https://help.qualaroo.com/hc/en-us/articles/201969438-The-REST-Reporting-API\\">docs</a> for instructions on how to generate it."""
     survey_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('survey_ids'), 'exclude': lambda f: f is None }})
-
     r"""IDs of the surveys from which you'd like to replicate data. If left empty, data from all surveys to which you have access will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_quickbooks.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_quickbooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,47 +15,36 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceQuickbooksCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access token fot making authenticated requests."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""Identifies which app is making the request. Obtain this value from the Keys tab on the app profile via My Apps on the developer site. There are two versions of this key: development and production."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""Obtain this value from the Keys tab on the app profile via My Apps on the developer site. There are two versions of this key: development and production."""
     realm_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('realm_id') }})
-
     r"""Labeled Company ID. The Make API Calls panel is populated with the realm id and the current access token."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""A token used when refreshing the access token."""
     token_expiry_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date-time when the access token should be refreshed."""
     auth_type: Optional[SourceQuickbooksCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceQuickbooksQuickbooksEnum(str, Enum):
     QUICKBOOKS = 'quickbooks'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceQuickbooks:
     r"""The values required to configure the source."""
     
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     sandbox: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sandbox') }})
-
     r"""Determines whether to use the sandbox or production environment."""
     source_type: SourceQuickbooksQuickbooksEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The default value to use if no bookmark exists for an endpoint (rfc3339 date string). E.g, 2021-03-20T00:00:00+00:00. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_railz.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_railz.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRailz:
     r"""The values required to configure the source."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""Client ID (client_id)"""
     secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
-
     r"""Secret key (secret_key)"""
     source_type: SourceRailzRailzEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""Start date"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_recharge.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_recharge.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRecharge:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The value of the Access Token generated. See the <a href=\\"https://docs.airbyte.com/integrations/sources/recharge\\">docs</a> for more information."""
     source_type: SourceRechargeRechargeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for Recharge API, in the format YYYY-MM-DDT00:00:00Z. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_recreation.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_recreation.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,11 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRecreation:
     r"""The values required to configure the source."""
     
     apikey: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apikey') }})
-
     r"""API Key"""
     source_type: SourceRecreationRecreationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     query_campsites: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query_campsites'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_recruitee.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_recruitee.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRecruitee:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Recruitee API Key. See <a href=\\"https://docs.recruitee.com/reference/getting-started#generate-api-token\\">here</a>."""
     company_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('company_id') }})
-
     r"""Recruitee Company ID. You can also find this ID on the <a href=\\"https://app.recruitee.com/#/settings/api_tokens\\">Recruitee API tokens page</a>."""
     source_type: SourceRecruiteeRecruiteeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_recurly.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_recurly.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRecurly:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Recurly API Key. See the  <a href=\\"https://docs.airbyte.com/integrations/sources/recurly\\">docs</a> for more information on how to generate this key."""
     source_type: SourceRecurlyRecurlyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     begin_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('begin_time'), 'exclude': lambda f: f is None }})
-
     r"""ISO8601 timestamp from which the replication from Recurly API will start from."""
     end_time: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_time'), 'exclude': lambda f: f is None }})
-
     r"""ISO8601 timestamp to which the replication from Recurly API will stop. Records after that date won't be imported."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_redshift.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_redshift.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,30 +13,22 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRedshift:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""Name of the database."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""Host Endpoint of the Redshift Cluster (must include the cluster-id, region and end with .redshift.amazonaws.com)."""
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""Password associated with the username."""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""Port of the database."""
     source_type: SourceRedshiftRedshiftEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""Username to use to access the database."""
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     schemas: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schemas'), 'exclude': lambda f: f is None }})
-
     r"""The list of schemas to sync from. Specify one or more explicitly or keep empty to process all schemas. Schema names are case sensitive."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_retently.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_retently.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,12 +13,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRetently:
     r"""The values required to configure the source."""
     
     source_type: SourceRetentlyRetentlyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to Retently"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_rki_covid.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_rki_covid.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRkiCovid:
     r"""The values required to configure the source."""
     
     source_type: SourceRkiCovidRkiCovidEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""UTC date in the format 2017-01-25. Any data before this date will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_rss.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceRss:
     r"""The values required to configure the source."""
     
     source_type: SourceRssRssEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url') }})
-
     r"""RSS Feed URL"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_s3.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_s3.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,142 +19,111 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3FormatJsonl:
     r"""This connector uses <a href=\\"https://arrow.apache.org/docs/python/json.html\\" target=\\"_blank\\">PyArrow</a> for JSON Lines (jsonl) file parsing."""
     
     block_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_size'), 'exclude': lambda f: f is None }})
-
     r"""The chunk size in bytes to process at a time in memory from each file. If your data is particularly wide and failing during schema detection, increasing this should solve it. Beware of raising this too high as you could hit OOM errors."""
     filetype: Optional[SourceS3FormatJsonlFiletypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filetype'), 'exclude': lambda f: f is None }})
-
     newlines_in_values: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newlines_in_values'), 'exclude': lambda f: f is None }})
-
     r"""Whether newline characters are allowed in JSON values. Turning this on may affect performance. Leave blank to default to False."""
     unexpected_field_behavior: Optional[SourceS3FormatJsonlUnexpectedFieldBehaviorEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unexpected_field_behavior'), 'exclude': lambda f: f is None }})
-
     r"""How JSON fields outside of explicit_schema (if given) are treated. Check <a href=\\"https://arrow.apache.org/docs/python/generated/pyarrow.json.ParseOptions.html\\" target=\\"_blank\\">PyArrow documentation</a> for details"""
     
 class SourceS3FormatAvroFiletypeEnum(str, Enum):
     AVRO = 'avro'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3FormatAvro:
     r"""This connector utilises <a href=\\"https://fastavro.readthedocs.io/en/latest/\\" target=\\"_blank\\">fastavro</a> for Avro parsing."""
     
     filetype: Optional[SourceS3FormatAvroFiletypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filetype'), 'exclude': lambda f: f is None }})
-
     
 class SourceS3FormatParquetFiletypeEnum(str, Enum):
     PARQUET = 'parquet'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3FormatParquet:
     r"""This connector utilises <a href=\\"https://arrow.apache.org/docs/python/generated/pyarrow.parquet.ParquetFile.html\\" target=\\"_blank\\">PyArrow (Apache Arrow)</a> for Parquet parsing."""
     
     batch_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('batch_size'), 'exclude': lambda f: f is None }})
-
     r"""Maximum number of records per batch read from the input files. Batches may be smaller if there aren’t enough rows in the file. This option can help avoid out-of-memory errors if your data is particularly wide."""
     buffer_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('buffer_size'), 'exclude': lambda f: f is None }})
-
     r"""Perform read buffering when deserializing individual column chunks. By default every group column will be loaded fully to memory. This option can help avoid out-of-memory errors if your data is particularly wide."""
     columns: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('columns'), 'exclude': lambda f: f is None }})
-
     r"""If you only want to sync a subset of the columns from the file(s), add the columns you want here as a comma-delimited list. Leave it empty to sync all columns."""
     filetype: Optional[SourceS3FormatParquetFiletypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filetype'), 'exclude': lambda f: f is None }})
-
     
 class SourceS3FormatCSVFiletypeEnum(str, Enum):
     CSV = 'csv'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3FormatCSV:
     r"""This connector utilises <a href=\\"https: // arrow.apache.org/docs/python/generated/pyarrow.csv.open_csv.html\\" target=\\"_blank\\">PyArrow (Apache Arrow)</a> for CSV parsing."""
     
     additional_reader_options: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('additional_reader_options'), 'exclude': lambda f: f is None }})
-
     r"""Optionally add a valid JSON string here to provide additional options to the csv reader. Mappings must correspond to options <a href=\\"https://arrow.apache.org/docs/python/generated/pyarrow.csv.ConvertOptions.html#pyarrow.csv.ConvertOptions\\" target=\\"_blank\\">detailed here</a>. 'column_types' is used internally to handle schema so overriding that would likely cause problems."""
     advanced_options: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('advanced_options'), 'exclude': lambda f: f is None }})
-
     r"""Optionally add a valid JSON string here to provide additional <a href=\\"https://arrow.apache.org/docs/python/generated/pyarrow.csv.ReadOptions.html#pyarrow.csv.ReadOptions\\" target=\\"_blank\\">Pyarrow ReadOptions</a>. Specify 'column_names' here if your CSV doesn't have header, or if you want to use custom column names. 'block_size' and 'encoding' are already used above, specify them again here will override the values above."""
     block_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('block_size'), 'exclude': lambda f: f is None }})
-
     r"""The chunk size in bytes to process at a time in memory from each file. If your data is particularly wide and failing during schema detection, increasing this should solve it. Beware of raising this too high as you could hit OOM errors."""
     delimiter: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('delimiter'), 'exclude': lambda f: f is None }})
-
     r"""The character delimiting individual cells in the CSV data. This may only be a 1-character string. For tab-delimited data enter '\t'."""
     double_quote: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('double_quote'), 'exclude': lambda f: f is None }})
-
     r"""Whether two quotes in a quoted CSV value denote a single quote in the data."""
     encoding: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('encoding'), 'exclude': lambda f: f is None }})
-
     r"""The character encoding of the CSV data. Leave blank to default to <strong>UTF8</strong>. See <a href=\\"https://docs.python.org/3/library/codecs.html#standard-encodings\\" target=\\"_blank\\">list of python encodings</a> for allowable options."""
     escape_char: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('escape_char'), 'exclude': lambda f: f is None }})
-
     r"""The character used for escaping special characters. To disallow escaping, leave this field blank."""
     filetype: Optional[SourceS3FormatCSVFiletypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('filetype'), 'exclude': lambda f: f is None }})
-
     infer_datatypes: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('infer_datatypes'), 'exclude': lambda f: f is None }})
-
     r"""Configures whether a schema for the source should be inferred from the current data or not. If set to false and a custom schema is set, then the manually enforced schema is used. If a schema is not manually set, and this is set to false, then all fields will be read as strings"""
     newlines_in_values: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('newlines_in_values'), 'exclude': lambda f: f is None }})
-
     r"""Whether newline characters are allowed in CSV values. Turning this on may affect performance. Leave blank to default to False."""
     quote_char: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quote_char'), 'exclude': lambda f: f is None }})
-
     r"""The character used for quoting CSV values. To disallow quoting, make this field blank."""
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3S3AmazonWebServices:
     r"""Use this to load files from S3 or S3-compatible services"""
     
     bucket: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('bucket') }})
-
     r"""Name of the S3 bucket where the file(s) exist."""
     aws_access_key_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_access_key_id'), 'exclude': lambda f: f is None }})
-
     r"""In order to access private Buckets stored on AWS S3, this connector requires credentials with the proper permissions. If accessing publicly available data, this field is not necessary."""
     aws_secret_access_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('aws_secret_access_key'), 'exclude': lambda f: f is None }})
-
     r"""In order to access private Buckets stored on AWS S3, this connector requires credentials with the proper permissions. If accessing publicly available data, this field is not necessary."""
     endpoint: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('endpoint'), 'exclude': lambda f: f is None }})
-
     r"""Endpoint to an S3 compatible service. Leave empty to use AWS."""
     path_prefix: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path_prefix'), 'exclude': lambda f: f is None }})
-
     r"""By providing a path-like prefix (e.g. myFolder/thisTable/) under which all the relevant files sit, we can optimize finding these in S3. This is optional but recommended if your bucket contains many folders/files which you don't need to replicate."""
     
 class SourceS3S3Enum(str, Enum):
     S3 = 's3'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceS3:
     r"""The values required to configure the source."""
     
     dataset: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset') }})
-
     r"""The name of the stream you would like this source to output. Can contain letters, numbers, or underscores."""
     path_pattern: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('path_pattern') }})
-
     r"""A regular expression which tells the connector which files to replicate. All files which match this pattern will be replicated. Use | to separate multiple patterns. See <a href=\\"https://facelessuser.github.io/wcmatch/glob/\\" target=\\"_blank\\">this page</a> to understand pattern syntax (GLOBSTAR and SPLIT flags are enabled). Use pattern <strong>**</strong> to pick up all files."""
     provider: SourceS3S3AmazonWebServices = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('provider') }})
-
     r"""Use this to load files from S3 or S3-compatible services"""
     source_type: SourceS3S3Enum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     format: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('format'), 'exclude': lambda f: f is None }})
-
     r"""The format of the files you'd like to replicate"""
     schema: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema'), 'exclude': lambda f: f is None }})
-
     r"""Optionally provide a schema to enforce, as a valid JSON string. Ensure this is a mapping of <strong>{ \\"column\\" : \\"type\\" }</strong>, where types are valid <a href=\\"https://json-schema.org/understanding-json-schema/reference/type.html\\" target=\\"_blank\\">JSON Schema datatypes</a>. Leave as {} to auto-infer the schema."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_salesforce.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_surveymonkey.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,62 +6,49 @@
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 
-class SourceSalesforceAuthTypeEnum(str, Enum):
-    CLIENT = 'Client'
-
-class SourceSalesforceSalesforceEnum(str, Enum):
-    SALESFORCE = 'salesforce'
-
-class SourceSalesforceStreamsCriteriaSearchCriteriaEnum(str, Enum):
-    STARTS_WITH = 'starts with'
-    ENDS_WITH = 'ends with'
-    CONTAINS = 'contains'
-    EXACTS = 'exacts'
-    STARTS_NOT_WITH = 'starts not with'
-    ENDS_NOT_WITH = 'ends not with'
-    NOT_CONTAINS = 'not contains'
-    NOT_EXACTS = 'not exacts'
+class SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum(str, Enum):
+    OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSalesforceStreamsCriteria:
+class SourceSurveymonkeySurveyMonkeyAuthorizationMethod:
+    r"""The authorization method to use to retrieve data from SurveyMonkey"""
+    
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
+    r"""Access Token for making authenticated requests. See the <a href=\\"https://docs.airbyte.io/integrations/sources/surveymonkey\\">docs</a> for information on how to generate this key."""
+    auth_method: SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
+    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
+    r"""The Client ID of the SurveyMonkey developer application."""
+    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
+    r"""The Client Secret of the SurveyMonkey developer application."""
     
-    criteria: SourceSalesforceStreamsCriteriaSearchCriteriaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('criteria') }})
+class SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum(str, Enum):
+    r"""Depending on the originating datacenter of the SurveyMonkey account, the API access URL may be different."""
+    USA = 'USA'
+    EUROPE = 'Europe'
+    CANADA = 'Canada'
 
-    value: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value') }})
+class SourceSurveymonkeySurveymonkeyEnum(str, Enum):
+    SURVEYMONKEY = 'surveymonkey'
 
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSalesforce:
+class SourceSurveymonkey:
     r"""The values required to configure the source."""
     
-    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
-    r"""Enter your Salesforce developer application's <a href=\\"https://developer.salesforce.com/forums/?id=9062I000000DLgbQAG\\">Client ID</a>"""
-    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
-    r"""Enter your Salesforce developer application's <a href=\\"https://developer.salesforce.com/forums/?id=9062I000000DLgbQAG\\">Client secret</a>"""
-    refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
-    r"""Enter your application's <a href=\\"https://developer.salesforce.com/docs/atlas.en-us.mobile_sdk.meta/mobile_sdk/oauth_refresh_token_flow.htm\\">Salesforce Refresh Token</a> used for Airbyte to access your Salesforce account."""
-    source_type: SourceSalesforceSalesforceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    auth_type: Optional[SourceSalesforceAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
-    is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
-
-    r"""Toggle if you're using a <a href=\\"https://help.salesforce.com/s/articleView?id=sf.deploy_sandboxes_parent.htm&type=5\\">Salesforce Sandbox</a>"""
-    start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
-    r"""Enter the date in the YYYY-MM-DD format. Airbyte will replicate the data added on and after this date. If this field is blank, Airbyte will replicate the data for last two years."""
-    streams_criteria: Optional[list[SourceSalesforceStreamsCriteria]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streams_criteria'), 'exclude': lambda f: f is None }})
-
-    r"""Filter streams relevant to you"""
+    source_type: SourceSurveymonkeySurveymonkeyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
+    credentials: Optional[SourceSurveymonkeySurveyMonkeyAuthorizationMethod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
+    r"""The authorization method to use to retrieve data from SurveyMonkey"""
+    origin: Optional[SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('origin'), 'exclude': lambda f: f is None }})
+    r"""Depending on the originating datacenter of the SurveyMonkey account, the API access URL may be different."""
+    survey_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('survey_ids'), 'exclude': lambda f: f is None }})
+    r"""IDs of the surveys from which you'd like to replicate data. If left empty, data from all boards to which you have access will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_salesforce_singer.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_salesforce_singer.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,33 +18,24 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSalesforceSinger:
     r"""The values required to configure the source."""
     
     api_type: SourceSalesforceSingerAPITypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_type') }})
-
     r"""Unless you know that you are transferring a very small amount of data, prefer using the BULK API. This will help avoid using up all of your API call quota with Salesforce. Valid values are BULK or REST."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Consumer Key that can be found when viewing your app in Salesforce"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Consumer Secret that can be found when viewing your app in Salesforce"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Salesforce Refresh Token used for Airbyte to access your Salesforce account. If you don't know what this is, follow this <a href=\\"https://medium.com/@bpmmendis94/obtain-access-refresh-tokens-from-salesforce-rest-api-a324fe4ccd9b\\">guide</a> to retrieve it."""
     source_type: SourceSalesforceSingerSalesforceSingerEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
-
     r"""Whether or not the the app is in a Salesforce sandbox. If you do not know what this, assume it is false. We provide more info on this field in the <a href=\\"https://docs.airbyte.io/integrations/destinations/salesforce#is_sandbox\\">docs</a>."""
     quota_percent_per_run: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quota_percent_per_run'), 'exclude': lambda f: f is None }})
-
     r"""determines the maximum allowed API quota percentage the connector is allowed to consume per sync job"""
     quota_percent_total: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('quota_percent_total'), 'exclude': lambda f: f is None }})
-
     r"""Determines the maximum allowed API quota percentage the connector is allowed to consume at any time"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_salesloft.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_salesloft.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,55 +15,44 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSalesloftCredentialsAuthenticateViaAPIKey:
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key for making authenticated requests. More instruction on how to find this value in our <a href=\\"https://docs.airbyte.com/integrations/sources/salesloft#setup-guide\\">docs</a>"""
     auth_type: SourceSalesloftCredentialsAuthenticateViaAPIKeyAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     
 class SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSalesloftCredentialsAuthenticateViaOAuth:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token for making authenticated requests."""
     auth_type: SourceSalesloftCredentialsAuthenticateViaOAuthAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Salesloft developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Salesloft developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The token for obtaining a new access token."""
     token_expiry_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date-time when the access token should be refreshed."""
     
 class SourceSalesloftSalesloftEnum(str, Enum):
     SALESLOFT = 'salesloft'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSalesloft:
     r"""The values required to configure the source."""
     
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     source_type: SourceSalesloftSalesloftEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for Salesloft API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sap_fieldglass.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sap_fieldglass.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSapFieldglass:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""API Key"""
     source_type: SourceSapFieldglassSapFieldglassEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_secoda.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_secoda.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSecoda:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your API Access Key. See <a href=\\"https://docs.secoda.co/secoda-api/authentication\\">here</a>. The key is case sensitive."""
     source_type: SourceSecodaSecodaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sendgrid.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sendgrid.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSendgrid:
     r"""The values required to configure the source."""
     
     apikey: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('apikey') }})
-
     r"""API Key, use <a href=\\"https://app.sendgrid.com/settings/api_keys/\\">admin</a> to generate this key."""
     source_type: SourceSendgridSendgridEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_time: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_time'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""Start time in ISO8601 format. Any data before this time point will not be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sendinblue.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sendinblue.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSendinblue:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your API Key. See <a href=\\"https://developers.sendinblue.com/docs/getting-started\\">here</a>."""
     source_type: SourceSendinblueSendinblueEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_senseforce.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_senseforce.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSenseforce:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Your API access token. See <a href=\\"https://manual.senseforce.io/manual/sf-platform/public-api/get-your-access-token/\\">here</a>. The toke is case sensitive."""
     backend_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('backend_url') }})
-
     r"""Your Senseforce API backend URL. This is the URL shown during the Login screen. See <a href=\\"https://manual.senseforce.io/manual/sf-platform/public-api/get-your-access-token/\\">here</a> for more details. (Note: Most Senseforce backend APIs have the term 'galaxy' in their ULR)"""
     dataset_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataset_id') }})
-
     r"""The ID of the dataset you want to synchronize. The ID can be found in the URL when opening the dataset. See <a href=\\"https://manual.senseforce.io/manual/sf-platform/public-api/get-your-access-token/\\">here</a> for more details. (Note: As the Senseforce API only allows to synchronize a specific dataset, each dataset you  want to synchronize needs to be implemented as a separate airbyte source)."""
     source_type: SourceSenseforceSenseforceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25. Only data with \\"Timestamp\\" after this date will be replicated. Important note: This start date must be set to the first day of where your dataset provides data.  If your dataset has data from 2020-10-10 10:21:10, set the start_date to 2020-10-10 or later"""
     slice_range: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('slice_range'), 'exclude': lambda f: f is None }})
-
     r"""The time increment used by the connector when requesting data from the Senseforce API. The bigger the value is, the less requests will be made and faster the sync will be. On the other hand, the more seldom the state is persisted and the more likely one could run into rate limites.  Furthermore, consider that large chunks of time might take a long time for the Senseforce query to return data - meaning it could take in effect longer than with more smaller time slices. If there are a lot of data per day, set this setting to 1. If there is only very little data per day, you might change the setting to 10 or more."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sentry.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sentry.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,24 +13,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSentry:
     r"""The values required to configure the source."""
     
     auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
-
     r"""Log into Sentry and then <a href=\\"https://sentry.io/settings/account/api/auth-tokens/\\">create authentication tokens</a>.For self-hosted, you can find or create authentication tokens by visiting \\"{instance_url_prefix}/settings/account/api/auth-tokens/\\" """
     organization: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organization') }})
-
     r"""The slug of the organization the groups belong to."""
     project: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project') }})
-
     r"""The name (slug) of the Project you want to sync."""
     source_type: SourceSentrySentryEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     discover_fields: Optional[list[Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('discover_fields'), 'exclude': lambda f: f is None }})
-
     r"""Fields to retrieve when fetching discover events"""
     hostname: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hostname'), 'exclude': lambda f: f is None }})
-
     r"""Host name of Sentry API server.For self-hosted, specify your host name here. Otherwise, leave it empty."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sftp.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,63 +14,51 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSftpCredentialsSSHKeyAuthentication:
     r"""The server authentication method"""
     
     auth_method: SourceSftpCredentialsSSHKeyAuthenticationAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
     r"""Connect through ssh key"""
     auth_ssh_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_ssh_key') }})
-
     r"""OS-level user account ssh key credentials in RSA PEM format ( created with ssh-keygen -t rsa -m PEM -f myuser_rsa )"""
     
 class SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum(str, Enum):
     r"""Connect through password authentication"""
     SSH_PASSWORD_AUTH = 'SSH_PASSWORD_AUTH'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSftpCredentialsPasswordAuthentication:
     r"""The server authentication method"""
     
     auth_method: SourceSftpCredentialsPasswordAuthenticationAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
     r"""Connect through password authentication"""
     auth_user_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_user_password') }})
-
     r"""OS-level password for logging into the jump server host"""
     
 class SourceSftpSftpEnum(str, Enum):
     SFTP = 'sftp'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSftp:
     r"""The values required to configure the source."""
     
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The server host address"""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The server port"""
     source_type: SourceSftpSftpEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     user: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user') }})
-
     r"""The server user"""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""The server authentication method"""
     file_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The regular expression to specify files for sync in a chosen Folder Path"""
     file_types: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_types'), 'exclude': lambda f: f is None }})
-
     r"""Coma separated file types. Currently only 'csv' and 'json' types are supported."""
     folder_path: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('folder_path'), 'exclude': lambda f: f is None }})
-
     r"""The directory to search files for sync"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sftp_bulk.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sftp_bulk.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,42 +21,30 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSftpBulk:
     r"""The values required to configure the source."""
     
     folder_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('folder_path') }})
-
     r"""The directory to search files for sync"""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The server host address"""
     port: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('port') }})
-
     r"""The server port"""
     source_type: SourceSftpBulkSftpBulkEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
     stream_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('stream_name') }})
-
     r"""The name of the stream or table you want to create"""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The server user"""
     file_most_recent: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_most_recent'), 'exclude': lambda f: f is None }})
-
     r"""Sync only the most recent file for the configured folder path and file pattern"""
     file_pattern: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_pattern'), 'exclude': lambda f: f is None }})
-
     r"""The regular expression to specify files for sync in a chosen Folder Path"""
     file_type: Optional[SourceSftpBulkFileTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('file_type'), 'exclude': lambda f: f is None }})
-
     r"""The file type you want to sync. Currently only 'csv' and 'json' files are supported."""
     password: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password'), 'exclude': lambda f: f is None }})
-
     r"""OS-level password for logging into the jump server host"""
     private_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('private_key'), 'exclude': lambda f: f is None }})
-
     r"""The private key"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_shopify.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_shopify.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,54 +13,44 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceShopifyCredentialsOAuth20:
     r"""OAuth2.0"""
     
     auth_method: SourceShopifyCredentialsOAuth20AuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""The Access Token for making authenticated requests."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
     r"""The Client ID of the Shopify developer application."""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""The Client Secret of the Shopify developer application."""
     
 class SourceShopifyCredentialsAPIPasswordAuthMethodEnum(str, Enum):
     API_PASSWORD = 'api_password'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceShopifyCredentialsAPIPassword:
     r"""API Password Auth"""
     
     api_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_password') }})
-
     r"""The API Password for your private application in the `Shopify` store."""
     auth_method: SourceShopifyCredentialsAPIPasswordAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
     
 class SourceShopifyShopifyEnum(str, Enum):
     SHOPIFY = 'shopify'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceShopify:
     r"""The values required to configure the source."""
     
     shop: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shop') }})
-
     r"""The name of your Shopify store found in the URL. For example, if your URL was https://NAME.myshopify.com, then the name would be 'NAME'."""
     source_type: SourceShopifyShopifyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""The date you would like to replicate data from. Format: YYYY-MM-DD. Any data before this date will not be replicated."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""The authorization method to use to retrieve data from Shopify"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_shortio.py` & `airbyte-1.7.1/src/airbyte/models/shared/sourcecreaterequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
-
-class SourceShortioShortioEnum(str, Enum):
-    SHORTIO = 'shortio'
+from typing import Any, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceShortio:
-    r"""The values required to configure the source."""
+class SourceCreateRequest:
     
-    domain_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domain_id') }})
-
-    secret_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret_key') }})
-
-    r"""Short.io Secret Key"""
-    source_type: SourceShortioShortioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
-    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
+    configuration: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configuration') }})
+    r"""The values required to configure the source."""
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
+    secret_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secretId'), 'exclude': lambda f: f is None }})
+    r"""Optional secretID obtained through the public API OAuth redirect flow."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_slack.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,60 +16,48 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSlackCredentialsAPIToken:
     r"""Choose how to authenticate into Slack"""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""A Slack bot token. See the <a href=\\"https://docs.airbyte.com/integrations/sources/slack\\">docs</a> for instructions on how to generate it."""
     option_title: SourceSlackCredentialsAPITokenOptionTitleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title') }})
-
     
 class SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum(str, Enum):
     DEFAULT_O_AUTH2_0_AUTHORIZATION = 'Default OAuth2.0 authorization'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSlackCredentialsSignInViaSlackOAuth:
     r"""Choose how to authenticate into Slack"""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Slack access_token. See our <a href=\\"https://docs.airbyte.com/integrations/sources/slack\\">docs</a> if you need help generating the token."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""Slack client_id. See our <a href=\\"https://docs.airbyte.com/integrations/sources/slack\\">docs</a> if you need help finding this id."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""Slack client_secret. See our <a href=\\"https://docs.airbyte.com/integrations/sources/slack\\">docs</a> if you need help finding this secret."""
     option_title: SourceSlackCredentialsSignInViaSlackOAuthOptionTitleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('option_title') }})
-
     
 class SourceSlackSlackEnum(str, Enum):
     SLACK = 'slack'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSlack:
     r"""The values required to configure the source."""
     
     join_channels: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('join_channels') }})
-
     r"""Whether to join all channels or to sync data only from channels the bot is already in.  If false, you'll need to manually add the bot to all the channels from which you'd like to sync messages."""
     lookback_window: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window') }})
-
     r"""How far into the past to look for messages in threads."""
     source_type: SourceSlackSlackEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     channel_filter: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('channel_filter'), 'exclude': lambda f: f is None }})
-
     r"""A channel name list (without leading '#' char) which limit the channels from which you'd like to sync. Empty list means no filter."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate into Slack"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_smaily.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_smaily.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSmaily:
     r"""The values required to configure the source."""
     
     api_password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_password') }})
-
     r"""API user password. See https://smaily.com/help/api/general/create-api-user/"""
     api_subdomain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_subdomain') }})
-
     r"""API Subdomain. See https://smaily.com/help/api/general/create-api-user/"""
     api_username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_username') }})
-
     r"""API user username. See https://smaily.com/help/api/general/create-api-user/"""
     source_type: SourceSmailySmailyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_smartengage.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zoom.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourceSmartengageSmartengageEnum(str, Enum):
-    SMARTENGAGE = 'smartengage'
+class SourceZoomZoomEnum(str, Enum):
+    ZOOM = 'zoom'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSmartengage:
+class SourceZoom:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""API Key"""
-    source_type: SourceSmartengageSmartengageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    jwt_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jwt_token') }})
+    r"""JWT Token"""
+    source_type: SourceZoomZoomEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_smartsheets.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_smartsheets.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,58 +15,46 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSmartsheetsCredentialsAPIAccessToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The access token to use for accessing your data from Smartsheets. This access token must be generated by a user with at least read access to the data you'd like to replicate. Generate an access token in the Smartsheets main menu by clicking Account > Apps & Integrations > API Access. See the <a href=\\"https://docs.airbyte.com/integrations/sources/smartsheets/#setup-guide\\">setup guide</a> for information on how to obtain this token."""
     auth_type: Optional[SourceSmartsheetsCredentialsAPIAccessTokenAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceSmartsheetsCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSmartsheetsCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token for making authenticated requests."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The API ID of the SmartSheets developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The API Secret the SmartSheets developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The key to refresh the expired access_token."""
     token_expiry_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date-time when the access token should be refreshed."""
     auth_type: Optional[SourceSmartsheetsCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceSmartsheetsSmartsheetsEnum(str, Enum):
     SMARTSHEETS = 'smartsheets'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSmartsheets:
     r"""The values required to configure the source."""
     
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     source_type: SourceSmartsheetsSmartsheetsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     spreadsheet_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('spreadsheet_id') }})
-
     r"""The spreadsheet ID. Find it by opening the spreadsheet then navigating to File > Properties"""
     start_datetime: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_datetime'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""Only rows modified after this date/time will be replicated. This should be an ISO 8601 string, for instance: `2000-01-01T13:00:00`"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_snapchat_marketing.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zoho_crm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,60 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date
+from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 
-class SourceSnapchatMarketingSnapchatMarketingEnum(str, Enum):
-    SNAPCHAT_MARKETING = 'snapchat-marketing'
+class SourceZohoCrmDataCenterLocationEnum(str, Enum):
+    r"""Please choose the region of your Data Center location. More info by this <a href=\\"https://www.zoho.com/crm/developer/docs/api/v2/multi-dc.html\\">Link</a>"""
+    US = 'US'
+    AU = 'AU'
+    EU = 'EU'
+    IN = 'IN'
+    CN = 'CN'
+    JP = 'JP'
+
+class SourceZohoCRMZohoCRMEditionEnum(str, Enum):
+    r"""Choose your Edition of Zoho CRM to determine API Concurrency Limits"""
+    FREE = 'Free'
+    STANDARD = 'Standard'
+    PROFESSIONAL = 'Professional'
+    ENTERPRISE = 'Enterprise'
+    ULTIMATE = 'Ultimate'
+
+class SourceZohoCrmEnvironmentEnum(str, Enum):
+    r"""Please choose the environment"""
+    PRODUCTION = 'Production'
+    DEVELOPER = 'Developer'
+    SANDBOX = 'Sandbox'
+
+class SourceZohoCrmZohoCrmEnum(str, Enum):
+    ZOHO_CRM = 'zoho-crm'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSnapchatMarketing:
+class SourceZohoCrm:
     r"""The values required to configure the source."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
-    r"""The Client ID of your Snapchat developer application."""
+    r"""OAuth2.0 Client ID"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
-    r"""The Client Secret of your Snapchat developer application."""
+    r"""OAuth2.0 Client Secret"""
+    dc_region: SourceZohoCrmDataCenterLocationEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dc_region') }})
+    r"""Please choose the region of your Data Center location. More info by this <a href=\\"https://www.zoho.com/crm/developer/docs/api/v2/multi-dc.html\\">Link</a>"""
+    edition: SourceZohoCRMZohoCRMEditionEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('edition') }})
+    r"""Choose your Edition of Zoho CRM to determine API Concurrency Limits"""
+    environment: SourceZohoCrmEnvironmentEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('environment') }})
+    r"""Please choose the environment"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
-    r"""Refresh Token to renew the expired Access Token."""
-    source_type: SourceSnapchatMarketingSnapchatMarketingEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
-    r"""Date in the format 2017-01-25. Any data after this date will not be replicated."""
-    start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
-    r"""Date in the format 2022-01-01. Any data before this date will not be replicated."""
+    r"""OAuth2.0 Refresh Token"""
+    source_type: SourceZohoCrmZohoCrmEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_datetime: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_datetime'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""ISO 8601, for instance: `YYYY-MM-DD`, `YYYY-MM-DD HH:MM:SS+HH:MM`"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_snowflake.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,70 +12,54 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSnowflakeCredentialsUsernameAndPassword:
     
     auth_type: SourceSnowflakeCredentialsUsernameAndPasswordAuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
     r"""The password associated with the username."""
     username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
     r"""The username you created to allow Airbyte to access the database."""
     
 class SourceSnowflakeCredentialsOAuth20AuthTypeEnum(str, Enum):
     O_AUTH = 'OAuth'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSnowflakeCredentialsOAuth20:
     
     auth_type: SourceSnowflakeCredentialsOAuth20AuthTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type') }})
-
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Snowflake developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Snowflake developer application."""
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access Token for making authenticated requests."""
     refresh_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token'), 'exclude': lambda f: f is None }})
-
     r"""Refresh Token for making authenticated requests."""
     
 class SourceSnowflakeSnowflakeEnum(str, Enum):
     SNOWFLAKE = 'snowflake'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSnowflake:
     r"""The values required to configure the source."""
     
     database: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('database') }})
-
     r"""The database you created for Airbyte to access data."""
     host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
-
     r"""The host domain of the snowflake instance (must include the account, region, cloud environment, and end with snowflakecomputing.com)."""
     role: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('role') }})
-
     r"""The role you created for Airbyte to access Snowflake."""
     source_type: SourceSnowflakeSnowflakeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     warehouse: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('warehouse') }})
-
     r"""The warehouse you created for Airbyte to access data."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     jdbc_url_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jdbc_url_params'), 'exclude': lambda f: f is None }})
-
     r"""Additional properties to pass to the JDBC URL string when connecting to the database formatted as 'key=value' pairs separated by the symbol '&'. (example: key1=value1&key2=value2&key3=value3)."""
     schema: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('schema'), 'exclude': lambda f: f is None }})
-
     r"""The source Snowflake schema tables. Leave empty to access tables from multiple schemas."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_sonar_cloud.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_sonar_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSonarCloud:
     r"""The values required to configure the source."""
     
     component_keys: list[Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('component_keys') }})
-
     r"""Comma-separated list of component keys."""
     organization: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('organization') }})
-
     r"""Organization key. See <a href=\\"https://docs.sonarcloud.io/appendices/project-information/#project-and-organization-keys\\">here</a>."""
     source_type: SourceSonarCloudSonarCloudEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     user_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('user_token') }})
-
     r"""Your User Token. See <a href=\\"https://docs.sonarcloud.io/advanced-setup/user-accounts/\\">here</a>. The token is case sensitive."""
     end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""To retrieve issues created before the given date (inclusive)."""
     start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""To retrieve issues created after the given date (inclusive)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_spacex_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/streamconfiguration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import connectionsyncmodeenum_enum as shared_connectionsyncmodeenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 
-class SourceSpacexAPISpacexAPIEnum(str, Enum):
-    SPACEX_API = 'spacex-api'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSpacexAPI:
-    r"""The values required to configure the source."""
+class StreamConfiguration:
+    r"""Configurations for a single stream."""
     
-    source_type: SourceSpacexAPISpacexAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-
-    options: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})
-
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    cursor_field: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('cursorField'), 'exclude': lambda f: f is None }})
+    r"""Path to the field that will be used to determine if a record is new or modified since the last sync. This field is REQUIRED if `sync_mode` is `incremental` unless there is a default."""
+    primary_key: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('primaryKey'), 'exclude': lambda f: f is None }})
+    r"""Paths to the fields that will be used as primary key. This field is REQUIRED if `destination_sync_mode` is `*_dedup` unless it is already supplied by the source schema."""
+    sync_mode: Optional[shared_connectionsyncmodeenum_enum.ConnectionSyncModeEnumEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncMode'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_square.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_square.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,57 +15,46 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSquareCredentialsAPIKey:
     r"""Choose how to authenticate to Square."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""The API key for a Square application"""
     credentials_title: Optional[SourceSquareCredentialsAPIKeyCredentialsTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title'), 'exclude': lambda f: f is None }})
-
     
 class SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum(str, Enum):
     O_AUTH_CREDENTIALS = 'OAuth Credentials'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSquareCredentialsOauthAuthentication:
     r"""Choose how to authenticate to Square."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Square-issued ID of your application"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Square-issued application secret for your application"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""A refresh token generated using the above client ID and secret"""
     credentials_title: Optional[SourceSquareCredentialsOauthAuthenticationCredentialsTitleEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials_title'), 'exclude': lambda f: f is None }})
-
     
 class SourceSquareSquareEnum(str, Enum):
     SQUARE = 'square'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSquare:
     r"""The values required to configure the source."""
     
     is_sandbox: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox') }})
-
     r"""Determines whether to use the sandbox or production environment."""
     source_type: SourceSquareSquareEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Choose how to authenticate to Square."""
     include_deleted_objects: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('include_deleted_objects'), 'exclude': lambda f: f is None }})
-
     r"""In some streams there is an option to include deleted objects (Items, Categories, Discounts, Taxes)"""
     start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""UTC date in the format YYYY-MM-DD. Any data before this date will not be replicated. If not set, all data will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_strava.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_strava.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,19 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceStrava:
     r"""The values required to configure the source."""
     
     athlete_id: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('athlete_id') }})
-
     r"""The Athlete ID of your Strava developer application."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The Client ID of your Strava developer application."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Client Secret of your Strava developer application."""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The Refresh Token with the activity: read_all permissions."""
     source_type: SourceStravaStravaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time. Any data before this date will not be replicated."""
     auth_type: Optional[SourceStravaAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_stripe.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_stripe.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,24 +16,18 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceStripe:
     r"""The values required to configure the source."""
     
     account_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_id') }})
-
     r"""Your Stripe account ID (starts with 'acct_', find yours <a href=\\"https://dashboard.stripe.com/settings/account\\">here</a>)."""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""Stripe API key (usually starts with 'sk_live_'; find yours <a href=\\"https://dashboard.stripe.com/apikeys\\">here</a>)."""
     source_type: SourceStripeStripeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Only data generated after this date will be replicated."""
     lookback_window_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window_days'), 'exclude': lambda f: f is None }})
-
     r"""When set, the connector will always re-export data from the past N days, where N is the value set here. This is useful if your data is frequently updated after creation. More info <a href=\\"https://docs.airbyte.com/integrations/sources/stripe#requirements\\">here</a>"""
     slice_range: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('slice_range'), 'exclude': lambda f: f is None }})
-
     r"""The time increment used by the connector when requesting data from the Stripe API. The bigger the value is, the less requests will be made and faster the sync will be. On the other hand, the more seldom the state is persisted."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_survey_sparrow.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_survey_sparrow.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,42 +13,36 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSurveySparrowRegionGlobalAccount:
     r"""Is your account location is EU based? If yes, the base url to retrieve data will be different."""
     
     url_base: Optional[SourceSurveySparrowRegionGlobalAccountURLBaseEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url_base'), 'exclude': lambda f: f is None }})
-
     
 class SourceSurveySparrowRegionEUBasedAccountURLBaseEnum(str, Enum):
     HTTPS_EU_API_SURVEYSPARROW_COM_V3 = 'https://eu-api.surveysparrow.com/v3'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSurveySparrowRegionEUBasedAccount:
     r"""Is your account location is EU based? If yes, the base url to retrieve data will be different."""
     
     url_base: Optional[SourceSurveySparrowRegionEUBasedAccountURLBaseEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('url_base'), 'exclude': lambda f: f is None }})
-
     
 class SourceSurveySparrowSurveySparrowEnum(str, Enum):
     SURVEY_SPARROW = 'survey-sparrow'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceSurveySparrow:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Your access token. See <a href=\\"https://developers.surveysparrow.com/rest-apis#authentication\\">here</a>. The key is case sensitive."""
     source_type: SourceSurveySparrowSurveySparrowEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     region: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
-
     r"""Is your account location is EU based? If yes, the base url to retrieve data will be different."""
     survey_id: Optional[list[Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('survey_id'), 'exclude': lambda f: f is None }})
-
     r"""A List of your survey ids for survey-specific stream"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_surveymonkey.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_twitter.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,58 +6,26 @@
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 
-class SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum(str, Enum):
-    OAUTH2_0 = 'oauth2.0'
+class SourceTwitterTwitterEnum(str, Enum):
+    TWITTER = 'twitter'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceSurveymonkeySurveyMonkeyAuthorizationMethod:
-    r"""The authorization method to use to retrieve data from SurveyMonkey"""
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
-    r"""Access Token for making authenticated requests. See the <a href=\\"https://docs.airbyte.io/integrations/sources/surveymonkey\\">docs</a> for information on how to generate this key."""
-    auth_method: SourceSurveymonkeySurveyMonkeyAuthorizationMethodAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
-    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
-    r"""The Client ID of the SurveyMonkey developer application."""
-    client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
-    r"""The Client Secret of the SurveyMonkey developer application."""
-    
-class SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum(str, Enum):
-    r"""Depending on the originating datacenter of the SurveyMonkey account, the API access URL may be different."""
-    USA = 'USA'
-    EUROPE = 'Europe'
-    CANADA = 'Canada'
-
-class SourceSurveymonkeySurveymonkeyEnum(str, Enum):
-    SURVEYMONKEY = 'surveymonkey'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SourceSurveymonkey:
+class SourceTwitter:
     r"""The values required to configure the source."""
     
-    source_type: SourceSurveymonkeySurveymonkeyEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
-    r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
-    credentials: Optional[SourceSurveymonkeySurveyMonkeyAuthorizationMethod] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
-    r"""The authorization method to use to retrieve data from SurveyMonkey"""
-    origin: Optional[SourceSurveymonkeyOriginDatacenterOfTheSurveyMonkeyAccountEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('origin'), 'exclude': lambda f: f is None }})
-
-    r"""Depending on the originating datacenter of the SurveyMonkey account, the API access URL may be different."""
-    survey_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('survey_ids'), 'exclude': lambda f: f is None }})
-
-    r"""IDs of the surveys from which you'd like to replicate data. If left empty, data from all boards to which you have access will be replicated."""
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    r"""App only Bearer Token. See the <a href=\\"https://developer.twitter.com/en/docs/authentication/oauth-2-0/bearer-tokens\\">docs</a> for more information on how to obtain this token."""
+    query: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
+    r"""Query for matching Tweets. You can learn how to build this query by reading <a href=\\"https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query\\"> build a query guide </a>."""
+    source_type: SourceTwitterTwitterEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""The end date for retrieving tweets must be a minimum of 10 seconds prior to the request time."""
+    start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""The start date for retrieving tweets cannot be more than 7 days in the past."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_tempo.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_todoist.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourceTempoTempoEnum(str, Enum):
-    TEMPO = 'tempo'
+class SourceTodoistTodoistEnum(str, Enum):
+    TODOIST = 'todoist'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceTempo:
+class SourceTodoist:
     r"""The values required to configure the source."""
     
-    api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
-    r"""Tempo API Token. Go to Tempo>Settings, scroll down to Data Access and select API integration."""
-    source_type: SourceTempoTempoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    source_type: SourceTodoistTodoistEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
+    r"""Your API Token. See <a href=\\"https://todoist.com/app/settings/integrations/\\">here</a>. The token is case sensitive."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_the_guardian_api.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_the_guardian_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,27 +13,20 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTheGuardianAPI:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your API Key. See <a href=\\"https://open-platform.theguardian.com/access/\\">here</a>. The key is case sensitive."""
     source_type: SourceTheGuardianAPITheGuardianAPIEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""Use this to set the minimum date (YYYY-MM-DD) of the results. Results older than the start_date will not be shown."""
     end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
-
     r"""(Optional) Use this to set the maximum date (YYYY-MM-DD) of the results. Results newer than the end_date will not be shown. Default is set to the current date (today) for incremental syncs."""
     query: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query'), 'exclude': lambda f: f is None }})
-
     r"""(Optional) The query (q) parameter filters the results to only those that include that search term. The q parameter supports AND, OR and NOT operators."""
     section: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('section'), 'exclude': lambda f: f is None }})
-
     r"""(Optional) Use this to filter the results by a particular section. See <a href=\\"https://content.guardianapis.com/sections?api-key=test\\">here</a> for a list of all sections, and <a href=\\"https://open-platform.theguardian.com/documentation/section\\">here</a> for the sections endpoint documentation."""
     tag: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tag'), 'exclude': lambda f: f is None }})
-
     r"""(Optional) A tag is a piece of data that is used by The Guardian to categorise content. Use this parameter to filter results by showing only the ones matching the entered tag. See <a href=\\"https://content.guardianapis.com/tags?api-key=test\\">here</a> for a list of all tags, and <a href=\\"https://open-platform.theguardian.com/documentation/tag\\">here</a> for the tags endpoint documentation."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_tiktok_marketing.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_tiktok_marketing.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,63 +15,50 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTiktokMarketingCredentialsSandboxAccessToken:
     r"""Authentication method"""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The long-term authorized access token."""
     advertiser_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('advertiser_id') }})
-
     r"""The Advertiser ID which generated for the developer's Sandbox application."""
     auth_type: Optional[SourceTiktokMarketingCredentialsSandboxAccessTokenAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTiktokMarketingCredentialsOAuth20:
     r"""Authentication method"""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Long-term Authorized Access Token."""
     app_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('app_id') }})
-
     r"""The Developer Application App ID."""
     secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secret') }})
-
     r"""The Developer Application Secret."""
     advertiser_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('advertiser_id'), 'exclude': lambda f: f is None }})
-
     r"""The Advertiser ID to filter reports and streams. Let this empty to retrieve all."""
     auth_type: Optional[SourceTiktokMarketingCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceTiktokMarketingTiktokMarketingEnum(str, Enum):
     TIKTOK_MARKETING = 'tiktok-marketing'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTiktokMarketing:
     r"""The values required to configure the source."""
     
     source_type: SourceTiktokMarketingTiktokMarketingEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     attribution_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('attribution_window'), 'exclude': lambda f: f is None }})
-
     r"""The attribution window in days."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     r"""Authentication method"""
     end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The date until which you'd like to replicate data for all incremental streams, in the format YYYY-MM-DD. All data generated between start_date and this date will be replicated. Not setting this option will result in always syncing the data till the current date."""
     start_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
     r"""The Start Date in format: YYYY-MM-DD. Any data before this date will not be replicated. If this parameter is not set, all data will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_todoist.py` & `airbyte-1.7.1/src/airbyte/models/shared/destination_meilisearch.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
+from typing import Optional
 
-class SourceTodoistTodoistEnum(str, Enum):
-    TODOIST = 'todoist'
+class DestinationMeilisearchMeilisearchEnum(str, Enum):
+    MEILISEARCH = 'meilisearch'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceTodoist:
-    r"""The values required to configure the source."""
+class DestinationMeilisearch:
+    r"""The values required to configure the destination."""
     
-    source_type: SourceTodoistTodoistEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
-    r"""Your API Token. See <a href=\\"https://todoist.com/app/settings/integrations/\\">here</a>. The token is case sensitive."""
+    destination_type: DestinationMeilisearchMeilisearchEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('destinationType') }})
+    host: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('host') }})
+    r"""Hostname of the MeiliSearch instance."""
+    api_key: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key'), 'exclude': lambda f: f is None }})
+    r"""MeiliSearch API Key. See the <a href=\\"https://docs.airbyte.com/integrations/destinations/meilisearch\\">docs</a> for more information on how to obtain this key."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_trello.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_trello.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTrello:
     r"""The values required to configure the source."""
     
     key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key') }})
-
     r"""Trello API key. See the <a href=\\"https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/#using-basic-oauth\\">docs</a> for instructions on how to generate it."""
     source_type: SourceTrelloTrelloEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2017-01-25T00:00:00Z. Any data before this date will not be replicated."""
     token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
     r"""Trello API token. See the <a href=\\"https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/#using-basic-oauth\\">docs</a> for instructions on how to generate it."""
     board_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('board_ids'), 'exclude': lambda f: f is None }})
-
     r"""IDs of the boards to replicate data from. If left empty, data from all boards to which you have access will be replicated."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_trustpilot.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_trustpilot.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,58 +16,46 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTrustpilotCredentialsAPIKey:
     r"""The API key authentication method gives you access to only the streams which are part of the Public API. When you want to get streams available via the Consumer API (e.g. the private reviews) you need to use authentication method OAuth 2.0."""
     
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The API key of the Trustpilot API application."""
     auth_type: Optional[SourceTrustpilotCredentialsAPIKeyAuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceTrustpilotCredentialsOAuth20AuthTypeEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTrustpilotCredentialsOAuth20:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Access Token for making authenticated requests."""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""The API key of the Trustpilot API application. (represents the OAuth Client ID)"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""The Secret of the Trustpilot API application. (represents the OAuth Client Secret)"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""The key to refresh the expired access_token."""
     token_expiry_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date-time when the access token should be refreshed."""
     auth_type: Optional[SourceTrustpilotCredentialsOAuth20AuthTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_type'), 'exclude': lambda f: f is None }})
-
     
 class SourceTrustpilotTrustpilotEnum(str, Enum):
     TRUSTPILOT = 'trustpilot'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTrustpilot:
     r"""The values required to configure the source."""
     
     business_units: list[str] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('business_units') }})
-
     r"""The names of business units which shall be synchronized. Some streams e.g. configured_business_units or private_reviews use this configuration."""
     credentials: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     source_type: SourceTrustpilotTrustpilotEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""For streams with sync. method incremental the start date time to be used"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_tvmaze_schedule.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_tvmaze_schedule.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,24 +13,19 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTvmazeSchedule:
     r"""The values required to configure the source."""
     
     domestic_schedule_country_code: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('domestic_schedule_country_code') }})
-
     r"""Country code for domestic TV schedule retrieval."""
     source_type: SourceTvmazeScheduleTvmazeScheduleEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
     r"""Start date for TV schedule retrieval. May be in the future."""
     end_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'exclude': lambda f: f is None }})
-
     r"""End date for TV schedule retrieval. May be in the future. Optional."""
     web_schedule_country_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('web_schedule_country_code'), 'exclude': lambda f: f is None }})
-
     r"""ISO 3166-1 country code for web TV schedule retrieval. Leave blank for
     all countries plus global web channels (e.g. Netflix). Alternatively,
     set to 'global' for just global web channels.
     """
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_twilio.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_twilio.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,21 +16,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTwilio:
     r"""The values required to configure the source."""
     
     account_sid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_sid') }})
-
     r"""Twilio account SID"""
     auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
-
     r"""Twilio Auth Token."""
     source_type: SourceTwilioTwilioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format 2020-10-01T00:00:00Z. Any data before this date will not be replicated."""
     lookback_window: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lookback_window'), 'exclude': lambda f: f is None }})
-
     r"""How far into the past to look for records. (in minutes)"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_twilio_taskrouter.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_twilio_taskrouter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTwilioTaskrouter:
     r"""The values required to configure the source."""
     
     account_sid: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('account_sid') }})
-
     r"""Twilio Account ID"""
     auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
-
     r"""Twilio Auth Token"""
     source_type: SourceTwilioTaskrouterTwilioTaskrouterEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_twitter.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_talk.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,33 +4,26 @@
 import dataclasses
 import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from marshmallow import fields
-from typing import Optional
+from typing import Any, Optional
 
-class SourceTwitterTwitterEnum(str, Enum):
-    TWITTER = 'twitter'
+class SourceZendeskTalkZendeskTalkEnum(str, Enum):
+    ZENDESK_TALK = 'zendesk-talk'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceTwitter:
+class SourceZendeskTalk:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""App only Bearer Token. See the <a href=\\"https://developer.twitter.com/en/docs/authentication/oauth-2-0/bearer-tokens\\">docs</a> for more information on how to obtain this token."""
-    query: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query') }})
-
-    r"""Query for matching Tweets. You can learn how to build this query by reading <a href=\\"https://developer.twitter.com/en/docs/twitter-api/tweets/search/integrate/build-a-query\\"> build a query guide </a>."""
-    source_type: SourceTwitterTwitterEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    end_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
-    r"""The end date for retrieving tweets must be a minimum of 10 seconds prior to the request time."""
-    start_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-
-    r"""The start date for retrieving tweets cannot be more than 7 days in the past."""
+    source_type: SourceZendeskTalkZendeskTalkEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""The date from which you'd like to replicate data for Zendesk Talk API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
+    subdomain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain') }})
+    r"""This is your Zendesk subdomain that can be found in your account URL. For example, in https://{MY_SUBDOMAIN}.zendesk.com/, where MY_SUBDOMAIN is the value of your subdomain."""
+    credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
+    r"""Zendesk service provides two authentication methods. Choose between: `OAuth2.0` or `API token`."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_typeform.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_typeform.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceTypeform:
     r"""The values required to configure the source."""
     
     source_type: SourceTypeformTypeformEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format: YYYY-MM-DDTHH:mm:ss[Z]. Any data before this date will not be replicated."""
     token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token') }})
-
     r"""The API Token for a Typeform account."""
     form_ids: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('form_ids'), 'exclude': lambda f: f is None }})
-
     r"""When this parameter is set, the connector will replicate data only from the input forms. Otherwise, all forms in your Typeform account will be replicated. You can find form IDs in your form URLs. For example, in the URL \\"https://mysite.typeform.com/to/u6nXL7\\" the form_id is u6nXL7. You can find form URLs on Share panel"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_us_census.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_us_census.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,14 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceUsCensus:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""Your API Key. Get your key <a href=\\"https://api.census.gov/data/key_signup.html\\">here</a>."""
     query_path: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query_path') }})
-
     r"""The path portion of the GET request"""
     source_type: SourceUsCensusUsCensusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     query_params: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('query_params'), 'exclude': lambda f: f is None }})
-
     r"""The query parameters portion of the GET request, without the api key"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_vantage.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_vantage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,12 +12,10 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceVantage:
     r"""The values required to configure the source."""
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Your API Access token. See <a href=\\"https://vantage.readme.io/reference/authentication\\">here</a>."""
     source_type: SourceVantageVantageEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_webflow.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_webflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,12 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceWebflow:
     r"""The values required to configure the source."""
     
     api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
     r"""The API token for authenticating to Webflow. See https://university.webflow.com/lesson/intro-to-the-webflow-api"""
     site_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('site_id') }})
-
     r"""The id of the Webflow site you are requesting data from. See https://developers.webflow.com/#sites"""
     source_type: SourceWebflowWebflowEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_whisky_hunter.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_whisky_hunter.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceWhiskyHunter:
     r"""The values required to configure the source."""
     
     source_type: SourceWhiskyHunterWhiskyHunterEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_wikipedia_pageviews.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_wikipedia_pageviews.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,30 +12,22 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceWikipediaPageviews:
     r"""The values required to configure the source."""
     
     access: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access') }})
-
     r"""If you want to filter by access method, use one of desktop, mobile-app or mobile-web. If you are interested in pageviews regardless of access method, use all-access."""
     agent: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('agent') }})
-
     r"""If you want to filter by agent type, use one of user, automated or spider. If you are interested in pageviews regardless of agent type, use all-agents."""
     article: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('article') }})
-
     r"""The title of any article in the specified project. Any spaces should be replaced with underscores. It also should be URI-encoded, so that non-URI-safe characters like %, / or ? are accepted."""
     country: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country') }})
-
     r"""The ISO 3166-1 alpha-2 code of a country for which to retrieve top articles."""
     end: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end') }})
-
     r"""The date of the last day to include, in YYYYMMDD or YYYYMMDDHH format."""
     project: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project') }})
-
     r"""If you want to filter by project, use the domain of any Wikimedia project."""
     source_type: SourceWikipediaPageviewsWikipediaPageviewsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start') }})
-
     r"""The date of the first day to include, in YYYYMMDD or YYYYMMDDHH format."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_woocommerce.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_yandex_metrica.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,32 +3,28 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from datetime import date
 from enum import Enum
 from marshmallow import fields
+from typing import Optional
 
-class SourceWoocommerceWoocommerceEnum(str, Enum):
-    WOOCOMMERCE = 'woocommerce'
+class SourceYandexMetricaYandexMetricaEnum(str, Enum):
+    YANDEX_METRICA = 'yandex-metrica'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceWoocommerce:
+class SourceYandexMetrica:
     r"""The values required to configure the source."""
     
-    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
-
-    r"""Customer Key for API in WooCommerce shop"""
-    api_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_secret') }})
-
-    r"""Customer Secret for API in WooCommerce shop"""
-    shop: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shop') }})
-
-    r"""The name of the store. For https://EXAMPLE.com, the shop name is 'EXAMPLE.com'."""
-    source_type: SourceWoocommerceWoocommerceEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
+    r"""Your Yandex Metrica API access token"""
+    counter_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('counter_id') }})
+    r"""Counter ID"""
+    source_type: SourceYandexMetricaYandexMetricaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
     start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
-
-    r"""The date you would like to replicate data from. Format: YYYY-MM-DD"""
+    r"""Starting point for your data replication, in format of \\"YYYY-MM-DD\\"."""
+    end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""Starting point for your data replication, in format of \\"YYYY-MM-DD\\". If not provided will sync till most recent date."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_xero.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_xero.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,42 +11,33 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceXeroAuthenticateViaXeroOAuth:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""Enter your Xero application's access token"""
     client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
     r"""Enter your Xero application's Client ID"""
     client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
     r"""Enter your Xero application's Client Secret"""
     refresh_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token') }})
-
     r"""Enter your Xero application's refresh token"""
     token_expiry_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token_expiry_date') }})
-
     r"""The date-time when the access token should be refreshed"""
     
 class SourceXeroXeroEnum(str, Enum):
     XERO = 'xero'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceXero:
     r"""The values required to configure the source."""
     
     authentication: SourceXeroAuthenticateViaXeroOAuth = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('authentication') }})
-
     source_type: SourceXeroXeroEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""UTC date and time in the format YYYY-MM-DDTHH:mm:ssZ. Any data with created_at before this data will not be synced."""
     tenant_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tenant_id') }})
-
     r"""Enter your Xero organization's Tenant ID"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_xkcd.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_xkcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceXkcd:
     r"""The values required to configure the source."""
     
     source_type: SourceXkcdXkcdEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_yandex_metrica.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_sunshine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,55 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import date
 from enum import Enum
-from marshmallow import fields
-from typing import Optional
+from typing import Any, Optional
 
-class SourceYandexMetricaYandexMetricaEnum(str, Enum):
-    YANDEX_METRICA = 'yandex-metrica'
+class SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum(str, Enum):
+    API_TOKEN = 'api_token'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceYandexMetrica:
-    r"""The values required to configure the source."""
+class SourceZendeskSunshineCredentialsAPIToken:
     
-    auth_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_token') }})
-
-    r"""Your Yandex Metrica API access token"""
-    counter_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('counter_id') }})
+    api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
+    r"""API Token. See the <a href=\\"https://docs.airbyte.io/integrations/sources/zendesk_sunshine\\">docs</a> for information on how to generate this key."""
+    auth_method: SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
+    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
+    r"""The user email for your Zendesk account"""
+    
+class SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum(str, Enum):
+    OAUTH2_0 = 'oauth2.0'
 
-    r"""Counter ID"""
-    source_type: SourceYandexMetricaYandexMetricaEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
 
-    start_date: date = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.dateisoformat(False), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso') }})
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SourceZendeskSunshineCredentialsOAuth20:
+    
+    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
+    r"""Long-term access Token for making authenticated requests."""
+    auth_method: SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
+    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
+    r"""The Client ID of your OAuth application."""
+    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
+    r"""The Client Secret of your OAuth application."""
+    
+class SourceZendeskSunshineZendeskSunshineEnum(str, Enum):
+    ZENDESK_SUNSHINE = 'zendesk-sunshine'
 
-    r"""Starting point for your data replication, in format of \\"YYYY-MM-DD\\"."""
-    end_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('end_date'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
 
-    r"""Starting point for your data replication, in format of \\"YYYY-MM-DD\\". If not provided will sync till most recent date."""
+@dataclass_json(undefined=Undefined.EXCLUDE)
+@dataclasses.dataclass
+class SourceZendeskSunshine:
+    r"""The values required to configure the source."""
+    
+    source_type: SourceZendeskSunshineZendeskSunshineEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""The date from which you'd like to replicate data for Zendesk Sunshine API, in the format YYYY-MM-DDT00:00:00Z."""
+    subdomain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain') }})
+    r"""The subdomain for your Zendesk Account."""
+    credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_younium.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zuora.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,31 +3,28 @@
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from typing import Optional
 
-class SourceYouniumYouniumEnum(str, Enum):
-    YOUNIUM = 'younium'
+class SourceZuoraZuoraEnum(str, Enum):
+    ZUORA = 'zuora'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceYounium:
+class SourceZuora:
     r"""The values required to configure the source."""
     
-    legal_entity: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('legal_entity') }})
-
-    r"""Legal Entity that data should be pulled from"""
-    password: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('password') }})
-
-    r"""Account password for younium account API key"""
-    source_type: SourceYouniumYouniumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    username: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('username') }})
-
-    r"""Username for Younium account"""
-    playground: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('playground'), 'exclude': lambda f: f is None }})
-
-    r"""Property defining if connector is used against playground or production environment"""
+    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
+    r"""Client ID"""
+    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
+    r"""Client Secret"""
+    source_type: SourceZuoraZuoraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
+    r"""Start Date in format: YYYY-MM-DD"""
+    is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
+    r"""Defines whether use the SANDBOX or PRODUCTION environment."""
+    window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
+    r"""The amount of days for each data-chunk begining from start_date. Bigger the value - faster the fetch. (Min=1, as for a Day; Max=364, as for a Year)."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_youtube_analytics.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_youtube_analytics.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,11 +13,9 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceYoutubeAnalytics:
     r"""The values required to configure the source."""
     
     credentials: dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     source_type: SourceYoutubeAnalyticsYoutubeAnalyticsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_chat.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,55 +15,44 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceZendeskChatCredentialsAccessToken:
     
     access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
     r"""The Access Token to make authenticated requests."""
     credentials: SourceZendeskChatCredentialsAccessTokenCredentialsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     
 class SourceZendeskChatCredentialsOAuth20CredentialsEnum(str, Enum):
     OAUTH2_0 = 'oauth2.0'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceZendeskChatCredentialsOAuth20:
     
     credentials: SourceZendeskChatCredentialsOAuth20CredentialsEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials') }})
-
     access_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token'), 'exclude': lambda f: f is None }})
-
     r"""Access Token for making authenticated requests."""
     client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id'), 'exclude': lambda f: f is None }})
-
     r"""The Client ID of your OAuth application"""
     client_secret: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret'), 'exclude': lambda f: f is None }})
-
     r"""The Client Secret of your OAuth application."""
     refresh_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('refresh_token'), 'exclude': lambda f: f is None }})
-
     r"""Refresh Token to obtain new Access Token, when it's expired."""
     
 class SourceZendeskChatZendeskChatEnum(str, Enum):
     ZENDESK_CHAT = 'zendesk-chat'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceZendeskChat:
     r"""The values required to configure the source."""
     
     source_type: SourceZendeskChatZendeskChatEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
     r"""The date from which you'd like to replicate data for Zendesk Chat API, in the format YYYY-MM-DDT00:00:00Z."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
     subdomain: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain'), 'exclude': lambda f: f is None }})
-
     r"""Required if you access Zendesk Chat from a Zendesk Support subdomain."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_sunshine.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zendesk_support.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from datetime import datetime
 from enum import Enum
+from marshmallow import fields
 from typing import Any, Optional
 
-class SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum(str, Enum):
-    API_TOKEN = 'api_token'
+class SourceZendeskSupportZendeskSupportEnum(str, Enum):
+    ZENDESK_SUPPORT = 'zendesk-support'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZendeskSunshineCredentialsAPIToken:
-    
-    api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
-    r"""API Token. See the <a href=\\"https://docs.airbyte.io/integrations/sources/zendesk_sunshine\\">docs</a> for information on how to generate this key."""
-    auth_method: SourceZendeskSunshineCredentialsAPITokenAuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
-    email: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('email') }})
-
-    r"""The user email for your Zendesk account"""
-    
-class SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum(str, Enum):
-    OAUTH2_0 = 'oauth2.0'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SourceZendeskSunshineCredentialsOAuth20:
-    
-    access_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('access_token') }})
-
-    r"""Long-term access Token for making authenticated requests."""
-    auth_method: SourceZendeskSunshineCredentialsOAuth20AuthMethodEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('auth_method') }})
-
-    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
-    r"""The Client ID of your OAuth application."""
-    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
-    r"""The Client Secret of your OAuth application."""
-    
-class SourceZendeskSunshineZendeskSunshineEnum(str, Enum):
-    ZENDESK_SUNSHINE = 'zendesk-sunshine'
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class SourceZendeskSunshine:
+class SourceZendeskSupport:
     r"""The values required to configure the source."""
     
-    source_type: SourceZendeskSunshineZendeskSunshineEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
-    r"""The date from which you'd like to replicate data for Zendesk Sunshine API, in the format YYYY-MM-DDT00:00:00Z."""
+    source_type: SourceZendeskSupportZendeskSupportEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
+    r"""The date from which you'd like to replicate data for Zendesk Support API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
     subdomain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain') }})
-
-    r"""The subdomain for your Zendesk Account."""
+    r"""This is your Zendesk subdomain that can be found in your account URL. For example, in https://{MY_SUBDOMAIN}.zendesk.com/, where MY_SUBDOMAIN is the value of your subdomain."""
     credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
+    r"""Zendesk service provides two authentication methods. Choose between: `OAuth2.0` or `API token`."""
+    ignore_pagination: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ignore_pagination'), 'exclude': lambda f: f is None }})
+    r"""Makes each stream read a single page of data."""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_zendesk_talk.py` & `airbyte-1.7.1/src/airbyte/models/shared/sourceresponse.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
-from typing import Any, Optional
-
-class SourceZendeskTalkZendeskTalkEnum(str, Enum):
-    ZENDESK_TALK = 'zendesk-talk'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZendeskTalk:
-    r"""The values required to configure the source."""
+class SourceResponse:
+    r"""Provides details of a single source."""
     
-    source_type: SourceZendeskTalkZendeskTalkEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    start_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso') }})
-
-    r"""The date from which you'd like to replicate data for Zendesk Talk API, in the format YYYY-MM-DDT00:00:00Z. All data generated after this date will be replicated."""
-    subdomain: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subdomain') }})
-
-    r"""This is your Zendesk subdomain that can be found in your account URL. For example, in https://{MY_SUBDOMAIN}.zendesk.com/, where MY_SUBDOMAIN is the value of your subdomain."""
-    credentials: Optional[Any] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('credentials'), 'exclude': lambda f: f is None }})
-
-    r"""Zendesk service provides two authentication methods. Choose between: `OAuth2.0` or `API token`."""
+    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
+    source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
+    source_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
+    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_zenloop.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_zenloop.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,16 @@
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class SourceZenloop:
     r"""The values required to configure the source."""
     
     api_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_token') }})
-
     r"""Zenloop API Token. You can get the API token in settings page <a href=\\"https://app.zenloop.com/settings/api\\">here</a>"""
     source_type: SourceZenloopZenloopEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     date_from: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('date_from'), 'exclude': lambda f: f is None }})
-
     r"""Zenloop date_from. Format: 2021-10-24T03:30:30Z or 2021-10-24. Leave empty if only data from current data should be synced"""
     survey_group_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('survey_group_id'), 'exclude': lambda f: f is None }})
-
     r"""Zenloop Survey Group ID. Can be found by pulling All Survey Groups via SurveyGroups stream. Leave empty to pull answers from all survey groups"""
     survey_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('survey_id'), 'exclude': lambda f: f is None }})
-
     r"""Zenloop Survey ID. Can be found <a href=\\"https://app.zenloop.com/settings/api\\">here</a>. Leave empty to pull answers from all surveys"""
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_zoom.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_pendo.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 
 from __future__ import annotations
 import dataclasses
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 
-class SourceZoomZoomEnum(str, Enum):
-    ZOOM = 'zoom'
+class SourcePendoPendoEnum(str, Enum):
+    PENDO = 'pendo'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZoom:
+class SourcePendo:
     r"""The values required to configure the source."""
     
-    jwt_token: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('jwt_token') }})
-
-    r"""JWT Token"""
-    source_type: SourceZoomZoomEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    source_type: SourcePendoPendoEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/source_zuora.py` & `airbyte-1.7.1/src/airbyte/models/shared/streamproperties.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import connectionsyncmodeenum_enum as shared_connectionsyncmodeenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from typing import Optional
 
-class SourceZuoraZuoraEnum(str, Enum):
-    ZUORA = 'zuora'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceZuora:
-    r"""The values required to configure the source."""
+class StreamProperties:
+    r"""The stream properties associated with a connection."""
     
-    client_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_id') }})
-
-    r"""Client ID"""
-    client_secret: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('client_secret') }})
-
-    r"""Client Secret"""
-    source_type: SourceZuoraZuoraEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
-    start_date: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('start_date') }})
-
-    r"""Start Date in format: YYYY-MM-DD"""
-    is_sandbox: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('is_sandbox'), 'exclude': lambda f: f is None }})
-
-    r"""Defines whether use the SANDBOX or PRODUCTION environment."""
-    window_in_days: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('window_in_days'), 'exclude': lambda f: f is None }})
-
-    r"""The amount of days for each data-chunk begining from start_date. Bigger the value - faster the fetch. (Min=1, as for a Day; Max=364, as for a Year)."""
+    default_cursor_field: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('defaultCursorField'), 'exclude': lambda f: f is None }})
+    property_fields: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('propertyFields'), 'exclude': lambda f: f is None }})
+    source_defined_cursor_field: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedCursorField'), 'exclude': lambda f: f is None }})
+    source_defined_primary_key: Optional[list[list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceDefinedPrimaryKey'), 'exclude': lambda f: f is None }})
+    stream_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streamName'), 'exclude': lambda f: f is None }})
+    sync_modes: Optional[list[shared_connectionsyncmodeenum_enum.ConnectionSyncModeEnumEnum]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('syncModes'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/sourcecreaterequest.py` & `airbyte-1.7.1/src/airbyte/models/shared/streamconfigurations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import streamconfiguration as shared_streamconfiguration
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from typing import Any, Optional
+from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceCreateRequest:
+class StreamConfigurations:
+    r"""A list of configured stream options for a connection."""
     
-    configuration: Any = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('configuration') }})
-
-    r"""The values required to configure the source."""
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
-    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
-
-    secret_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('secretId'), 'exclude': lambda f: f is None }})
-
-    r"""Optional secretID obtained through the public API OAuth redirect flow."""
+    streams: Optional[list[shared_streamconfiguration.StreamConfiguration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streams'), 'exclude': lambda f: f is None }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/sourceresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/workspaceresponse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ..shared import geographyenum_enum as shared_geographyenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourceResponse:
-    r"""Provides details of a single source."""
+class WorkspaceResponse:
+    r"""Provides details of a single workspace."""
     
+    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
-    source_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceId') }})
-
-    source_type: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
-
     workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/sourcesresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/workspacesresponse.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import sourceresponse as shared_sourceresponse
+from ..shared import workspaceresponse as shared_workspaceresponse
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class SourcesResponse:
+class WorkspacesResponse:
     r"""Successful operation"""
     
-    data: list[shared_sourceresponse.SourceResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-
+    data: list[shared_workspaceresponse.WorkspaceResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     next: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next') }})
-
     previous: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/streamconfigurations.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_persistiq.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import streamconfiguration as shared_streamconfiguration
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
-from typing import Optional
+from enum import Enum
+
+class SourcePersistiqPersistiqEnum(str, Enum):
+    PERSISTIQ = 'persistiq'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class StreamConfigurations:
-    r"""A list of configured stream options for a connection."""
+class SourcePersistiq:
+    r"""The values required to configure the source."""
     
-    streams: Optional[list[shared_streamconfiguration.StreamConfiguration]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('streams'), 'exclude': lambda f: f is None }})
-
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    r"""PersistIq API Key. See the <a href=\\"https://apidocs.persistiq.com/#authentication\\">docs</a> for more information on where to find that key."""
+    source_type: SourcePersistiqPersistiqEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/workspaceresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/source_dremio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import geographyenum_enum as shared_geographyenum_enum
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
+from enum import Enum
+
+class SourceDremioDremioEnum(str, Enum):
+    DREMIO = 'dremio'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WorkspaceResponse:
-    r"""Provides details of a single workspace."""
+class SourceDremio:
+    r"""The values required to configure the source."""
     
-    data_residency: shared_geographyenum_enum.GeographyEnumEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataResidency') }})
-
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-
-    workspace_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('workspaceId') }})
-
+    api_key: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('api_key') }})
+    r"""API Key that is generated when you authenticate to Dremio API"""
+    base_url: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('base_url') }})
+    r"""URL of your Dremio instance"""
+    source_type: SourceDremioDremioEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceType') }})
```

### Comparing `airbyte-1.7.0/src/airbyte/models/shared/workspacesresponse.py` & `airbyte-1.7.1/src/airbyte/models/shared/sourcesresponse.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ..shared import workspaceresponse as shared_workspaceresponse
+from ..shared import sourceresponse as shared_sourceresponse
 from airbyte import utils
 from dataclasses_json import Undefined, dataclass_json
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class WorkspacesResponse:
+class SourcesResponse:
     r"""Successful operation"""
     
-    data: list[shared_workspaceresponse.WorkspaceResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
-
+    data: list[shared_sourceresponse.SourceResponse] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data') }})
     next: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next') }})
-
     previous: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous') }})
-
```

### Comparing `airbyte-1.7.0/src/airbyte/sdk.py` & `airbyte-1.7.1/src/airbyte/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     streams: Streams
     workspaces: Workspaces
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "1.7.0"
-    _gen_version: str = "2.23.2"
+    _sdk_version: str = "1.7.1"
+    _gen_version: str = "2.23.4"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `airbyte-1.7.0/src/airbyte/sources.py` & `airbyte-1.7.1/src/airbyte/sources.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/streams.py` & `airbyte-1.7.1/src/airbyte/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/utils/retries.py` & `airbyte-1.7.1/src/airbyte/utils/retries.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/utils/utils.py` & `airbyte-1.7.1/src/airbyte/utils/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte/workspaces.py` & `airbyte-1.7.1/src/airbyte/workspaces.py`

 * *Files identical despite different names*

### Comparing `airbyte-1.7.0/src/airbyte.egg-info/PKG-INFO` & `airbyte-1.7.1/src/airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python Client SDK for Airbyte API
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: airbyte Version: 1.7.0 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: airbyte Version: 1.7.1 Summary: Python Client SDK
 for Airbyte API Home-page: UNKNOWN Author: Speakeasy License: UNKNOWN Platform:
 UNKNOWN Requires-Python: >=3.9 Description-Content-Type: text/markdown License-
 File: LICENSE.md
  [https://user-images.githubusercontent.com/68016351/222853569-b35cc448-6481-
                           4cf2-a237-bd5da47e94fd.png]
              Programatically control Airbyte Cloud through an API.
            [https://img.shields.io/static/v1?label=Docs&message=API
```

### Comparing `airbyte-1.7.0/src/airbyte.egg-info/SOURCES.txt` & `airbyte-1.7.1/src/airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

